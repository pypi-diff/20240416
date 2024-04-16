# Comparing `tmp/dynamizer-0.2.8.tar.gz` & `tmp/dynamizer-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamizer-0.2.8.tar", max compression
+gzip compressed data, was "dynamizer-0.2.9.tar", max compression
```

## Comparing `dynamizer-0.2.8.tar` & `dynamizer-0.2.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1069 2023-09-07 02:38:33.142866 dynamizer-0.2.8/LICENSE
--rw-r--r--   0        0        0     4700 2023-09-07 02:38:33.142866 dynamizer-0.2.8/README.md
--rw-r--r--   0        0        0    11277 2023-11-12 02:51:36.100021 dynamizer-0.2.8/dynamizer/__init__.py
--rw-r--r--   0        0        0      186 2023-09-11 02:43:16.988680 dynamizer-0.2.8/dynamizer/errors.py
--rw-r--r--   0        0        0     2402 2023-09-07 04:47:37.284940 dynamizer-0.2.8/dynamizer/mock.py
--rw-r--r--   0        0        0      601 2023-11-12 02:52:34.564348 dynamizer-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     5212 1970-01-01 00:00:00.000000 dynamizer-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-12-18 05:03:07.835104 dynamizer-0.2.9/LICENSE
+-rw-r--r--   0        0        0     4700 2023-12-18 05:03:07.835104 dynamizer-0.2.9/README.md
+-rw-r--r--   0        0        0    11727 2023-12-18 06:24:32.456372 dynamizer-0.2.9/dynamizer/__init__.py
+-rw-r--r--   0        0        0      186 2023-12-18 05:03:07.839104 dynamizer-0.2.9/dynamizer/errors.py
+-rw-r--r--   0        0        0     2402 2023-12-18 05:03:07.839104 dynamizer-0.2.9/dynamizer/mock.py
+-rw-r--r--   0        0        0      601 2023-12-18 06:28:53.224655 dynamizer-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     5263 1970-01-01 00:00:00.000000 dynamizer-0.2.9/PKG-INFO
```

### Comparing `dynamizer-0.2.8/LICENSE` & `dynamizer-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dynamizer-0.2.8/README.md` & `dynamizer-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `dynamizer-0.2.8/dynamizer/__init__.py` & `dynamizer-0.2.9/dynamizer/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,14 +70,15 @@
 @dataclasses.dataclass(kw_only=True, frozen=True)
 class DynamiteModel:
     """Base class for dynamite models."""
 
     created_at: datetime.datetime = None
     updated_at: datetime.datetime = None
     _serial: int = dataclasses.field(compare=False, default=None)
+    _sequence: int = dataclasses.field(compare=False, default=None)
 
     def __post_init__(self):
         now_utc = datetime.datetime.now(datetime.timezone.utc)
         if not self.created_at:
             object.__setattr__(self, "created_at", now_utc)
         if not self.updated_at:
             object.__setattr__(self, "updated_at", now_utc)
@@ -100,41 +101,47 @@
     def __get_field_update_args(self, new_serial: int = None):
         """
         Get the update args associated with fields.
 
         :param new_serial:
             The new serial to use, if not provided, one will be randomly generated.
         """
-        exclude = {"created_at", "_serial"}
-        set_parts = ["#c = if_not_exists(#c, :c)"]
+        exclude = {"created_at", "_serial", "_sequence"}
+        set_parts = ["#c = :c", "#s = :ns"]
+        add_parts = ["#seq :inc"]
         remove_parts = []
-        values = {}
-        fields = {}
+        values = {
+            ":inc": {"N": "1"},
+            ":c": {"S": self.created_at.isoformat()},
+            ":ns": {"N": str(new_serial or random.randint(1, 1_000_000_000_000))},
+        }
+        fields = {
+            "#s": "_serial",
+            "#seq": "_sequence",
+            "#c": "created_at",
+        }
+        if self._sequence is None:
+            add_parts = []
+            set_parts.append("#seq = :inc")
 
         for i, field in enumerate(self.__managed_fields):
             if field.name in exclude:
                 continue
             value = getattr(self, field.name)
             fields[f"#d{i}"] = field.name
             if value is None:
                 remove_parts.append(f"#d{i}")
             else:
                 set_parts.append(f"#d{i} = :d{i}")
                 values[f":d{i}"] = self.__serialize_field(field)
 
-        fields["#s"] = "_serial"
         if self._serial:
             values[":s"] = {"N": str(self._serial)}
-        values[":ns"] = {"N": str(new_serial or random.randint(1, 1_000_000_000_000))}
-        set_parts.append("#s = :ns")
-
-        fields["#c"] = "created_at"
-        values[":c"] = {"S": self.created_at.isoformat()}
 
-        return (set_parts, remove_parts, values, fields)
+        return (add_parts, set_parts, remove_parts, values, fields)
 
     def __get_secondary_key_update_args(self):
         """Get the update args associated with index keys."""
         remove_parts = []
         values = {}
         fields = {}
         keys = self.__get_hash_range_keys()
@@ -156,24 +163,26 @@
         :param table:
             The dynamodb table the update is targeting.
         :param force:
             Whether to force the update, ignoring the serial token.
         :param new_serial:
             The new serial to use, if not provided, one will be randomly generated.
         """
-        (sets, removes, values, fields) = self.__get_field_update_args(new_serial)
+        (adds, sets, removes, values, fields) = self.__get_field_update_args(new_serial)
         (rms, vls, flds) = self.__get_secondary_key_update_args()
         removes.extend(rms)
         values.update(vls)
         fields.update(flds)
 
         conditional_expression = "attribute_not_exists(#s)"
         update_expression = ""
+        if adds:
+            update_expression = f'{update_expression} ADD {", ".join(adds)}'
         if removes:
-            update_expression = f'{update_expression}REMOVE {", ".join(removes)}'
+            update_expression = f'{update_expression} REMOVE {", ".join(removes)}'
         update_expression = f'{update_expression} SET {", ".join(sets)}'
         if self._serial:
             conditional_expression = "#s = :s"
         result = {
             "TableName": table,
             "Key": self.__base_update_key_args(),
             "UpdateExpression": update_expression,
@@ -207,15 +216,15 @@
         """
         Allow the model to continue from a previous state specified by `prev`.
 
         Dynamite models have a token to prevent writing over a previous update.
         If it is desired to start from a fresh model and overwrite existing state,
         then this can be used to enable it without requiring forcing.
         """
-        return dataclasses.replace(self, _serial=prev._serial)
+        return dataclasses.replace(self, _serial=prev._serial, _sequence=prev._sequence)
 
     def __base_update_key_args(self) -> dict:
         """Generate the key argument for a dynamo update operation."""
         return {
             "hash_key": {
                 "S": (self.hash_key() if callable(self.hash_key) else self.hash_key)
             },
@@ -233,14 +242,15 @@
         except botocore.exceptions.ClientError as err:
             if err.response["Error"]["Code"] == "ConditionalCheckFailedException":
                 raise errors.ConcurrentUpdateError()
             raise err
         return dataclasses.replace(
             to_save,
             _serial=int(response["Attributes"]["_serial"]["N"]),
+            _sequence=int(response["Attributes"]["_sequence"]["N"]),
         )
 
     def _base_delete(
         self,
         client,
         table: str,
     ):
```

### Comparing `dynamizer-0.2.8/dynamizer/mock.py` & `dynamizer-0.2.9/dynamizer/mock.py`

 * *Files identical despite different names*

### Comparing `dynamizer-0.2.8/pyproject.toml` & `dynamizer-0.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dynamizer"
-version = "0.2.8"
+version = "0.2.9"
 description = "Dynamodb model maker."
 authors = ["Kevin Schiroo <kjschiroo@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `dynamizer-0.2.8/PKG-INFO` & `dynamizer-0.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: dynamizer
-Version: 0.2.8
+Version: 0.2.9
 Summary: Dynamodb model maker.
 License: MIT
 Author: Kevin Schiroo
 Author-email: kjschiroo@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: mock
 Requires-Dist: moto[dynamodb] (>=4.1.11,<5.0.0) ; extra == "mock"
 Description-Content-Type: text/markdown
 
 # Dynamizer
 
 A supportive set of defaults for dynamodb. Dynamizer doesn't aim to
```

