# Comparing `tmp/pycloudevents-0.1.1.tar.gz` & `tmp/pycloudevents-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycloudevents-0.1.1.tar", last modified: Mon Apr 15 08:56:05 2024, max compression
+gzip compressed data, was "pycloudevents-0.1.2.tar", last modified: Mon Apr 15 09:22:29 2024, max compression
```

## Comparing `pycloudevents-0.1.1.tar` & `pycloudevents-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11357 2024-04-15 08:55:48.586001 pycloudevents-0.1.1/LICENSE
--rw-r--r--   0        0        0     2949 2024-04-15 08:55:48.586001 pycloudevents-0.1.1/README.md
--rw-r--r--   0        0        0      480 2024-04-15 08:56:05.449992 pycloudevents-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       62 2024-04-15 08:55:48.586001 pycloudevents-0.1.1/src/pycloudevents/__init__.py
--rw-r--r--   0        0        0     6620 2024-04-15 08:55:48.586001 pycloudevents-0.1.1/src/pycloudevents/cloudevent.py
--rw-r--r--   0        0        0       44 2024-04-15 08:55:48.586001 pycloudevents-0.1.1/src/pycloudevents/exceptions.py
--rw-r--r--   0        0        0      651 2024-04-15 08:55:48.586001 pycloudevents-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0     1297 2024-04-15 08:55:48.586001 pycloudevents-0.1.1/tests/test_spec_1_0.py
--rw-r--r--   0        0        0     3189 1970-01-01 00:00:00.000000 pycloudevents-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-15 09:22:15.689315 pycloudevents-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2949 2024-04-15 09:22:15.689315 pycloudevents-0.1.2/README.md
+-rw-r--r--   0        0        0      480 2024-04-15 09:22:29.113386 pycloudevents-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       62 2024-04-15 09:22:15.689315 pycloudevents-0.1.2/src/pycloudevents/__init__.py
+-rw-r--r--   0        0        0     6689 2024-04-15 09:22:15.689315 pycloudevents-0.1.2/src/pycloudevents/cloudevent.py
+-rw-r--r--   0        0        0       44 2024-04-15 09:22:15.693315 pycloudevents-0.1.2/src/pycloudevents/exceptions.py
+-rw-r--r--   0        0        0      651 2024-04-15 09:22:15.693315 pycloudevents-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0     1297 2024-04-15 09:22:15.693315 pycloudevents-0.1.2/tests/test_spec_1_0.py
+-rw-r--r--   0        0        0     3189 1970-01-01 00:00:00.000000 pycloudevents-0.1.2/PKG-INFO
```

### Comparing `pycloudevents-0.1.1/LICENSE` & `pycloudevents-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pycloudevents-0.1.1/README.md` & `pycloudevents-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pycloudevents-0.1.1/src/pycloudevents/cloudevent.py` & `pycloudevents-0.1.2/src/pycloudevents/cloudevent.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,15 +113,15 @@
             except ValueError:
                 self._validation_errors.append("time must be in ISO8601 format")
 
         if self._validation_errors:
             return False
         return True
 
-    def to_json(self, *args, **kwargs):
+    def to_structured(self, *args, **kwargs):
         """
         A function that converts the object attributes into a JSON format.
 
         Parameters:
             *args: Variable length argument list.
             **kwargs: Arbitrary keyword arguments.
 
@@ -142,15 +142,16 @@
             v["dataschema"] = self._dataschema
         if self._subject is not None:
             v["subject"] = self._subject
         if self._time is not None:
             v["time"] = self._time
         return json.dumps(v, *args, **kwargs)
 
-    to_structured = to_json
+    def to_json(self, *args, **kwargs):
+        return self.to_structured(*args, **kwargs)
 
     @classmethod
     def from_json(cls, json_str: str, *args, **kwargs):
         """
         Class method to create an instance from a JSON string.
 
         Args:
```

### Comparing `pycloudevents-0.1.1/tests/__init__.py` & `pycloudevents-0.1.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pycloudevents-0.1.1/tests/test_spec_1_0.py` & `pycloudevents-0.1.2/tests/test_spec_1_0.py`

 * *Files identical despite different names*

### Comparing `pycloudevents-0.1.1/PKG-INFO` & `pycloudevents-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycloudevents
-Version: 0.1.1
+Version: 0.1.2
 Summary: A third party cloudevents 1.0 SDK for Python.
 Author-Email: -LAN- <laipz8200@outlook.com>
 License: Apache2.0
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 
 # PyCloudEvents
```

