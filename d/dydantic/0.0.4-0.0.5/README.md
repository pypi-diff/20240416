# Comparing `tmp/dydantic-0.0.4.tar.gz` & `tmp/dydantic-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dydantic-0.0.4.tar", max compression
+gzip compressed data, was "dydantic-0.0.5.tar", max compression
```

## Comparing `dydantic-0.0.4.tar` & `dydantic-0.0.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1067 2024-04-06 05:52:07.999927 dydantic-0.0.4/LICENSE
--rw-r--r--   0        0        0     2847 2024-04-12 23:11:08.576469 dydantic-0.0.4/README.md
--rw-r--r--   0        0        0     1979 2024-04-08 06:06:13.745492 dydantic-0.0.4/dydantic/__init__.py
--rw-r--r--   0        0        0    18614 2024-04-12 23:39:20.289421 dydantic-0.0.4/dydantic/_utils.py
--rw-r--r--   0        0        0        0 2024-04-06 06:24:35.972780 dydantic-0.0.4/dydantic/py.typed
--rw-r--r--   0        0        0     1312 2024-04-12 23:39:20.289839 dydantic-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     3467 1970-01-01 00:00:00.000000 dydantic-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-06 05:52:07.999927 dydantic-0.0.5/LICENSE
+-rw-r--r--   0        0        0     2847 2024-04-12 23:11:08.576469 dydantic-0.0.5/README.md
+-rw-r--r--   0        0        0     1979 2024-04-08 06:06:13.745492 dydantic-0.0.5/dydantic/__init__.py
+-rw-r--r--   0        0        0    18628 2024-04-15 23:58:29.574296 dydantic-0.0.5/dydantic/_utils.py
+-rw-r--r--   0        0        0        0 2024-04-06 06:24:35.972780 dydantic-0.0.5/dydantic/py.typed
+-rw-r--r--   0        0        0     1312 2024-04-15 23:58:29.574807 dydantic-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     3467 1970-01-01 00:00:00.000000 dydantic-0.0.5/PKG-INFO
```

### Comparing `dydantic-0.0.4/LICENSE` & `dydantic-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dydantic-0.0.4/README.md` & `dydantic-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `dydantic-0.0.4/dydantic/__init__.py` & `dydantic-0.0.5/dydantic/__init__.py`

 * *Files identical despite different names*

### Comparing `dydantic-0.0.4/dydantic/_utils.py` & `dydantic-0.0.5/dydantic/_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -386,21 +386,22 @@
     required: List[str],
     root_schema: Dict[str, Any],
 ) -> Any:
     type_ = _json_schema_to_pydantic_type(json_schema, root_schema, name_=name.title())
     description = json_schema.get("description")
     examples = json_schema.get("examples")
     is_required = name in required
-    default = ... if is_required else None
 
     field_kwargs = {
         "description": description,
         "examples": examples,
-        "default": default,
     }
+    if not is_required:
+        field_kwargs["default"] = None
+    default = ... if is_required else None
 
     if isinstance(type_, type) and issubclass(type_, (int, float)):
         if "minimum" in json_schema:
             field_kwargs["ge"] = json_schema["minimum"]
         if "exclusiveMinimum" in json_schema:
             field_kwargs["gt"] = json_schema["exclusiveMinimum"]
         if "maximum" in json_schema:
@@ -472,15 +473,14 @@
     if all_of_schemas:
         all_of_types = [
             _json_schema_to_pydantic_type(schema, root_schema)
             for schema in all_of_schemas
         ]
         if len(all_of_types) == 1:
             return all_of_types[0]
-        breakpoint()
         return tuple(all_of_types)
 
     type_ = json_schema.get("type")
 
     if type_ == "string":
         return str
     elif type_ == "integer":
```

### Comparing `dydantic-0.0.4/pyproject.toml` & `dydantic-0.0.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dydantic"
-version = "0.0.4"
+version = "0.0.5"
 description = "Dynamically generate pydantic models from JSON schema."
 authors = ["William Fu-Hinthorn <13333726+hinthornw@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `dydantic-0.0.4/PKG-INFO` & `dydantic-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dydantic
-Version: 0.0.4
+Version: 0.0.5
 Summary: Dynamically generate pydantic models from JSON schema.
 License: MIT
 Author: William Fu-Hinthorn
 Author-email: 13333726+hinthornw@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

