# Comparing `tmp/pycloudevents-0.1.3.tar.gz` & `tmp/pycloudevents-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycloudevents-0.1.3.tar", last modified: Tue Apr 16 06:00:02 2024, max compression
+gzip compressed data, was "pycloudevents-0.1.4.tar", last modified: Tue Apr 16 06:40:37 2024, max compression
```

## Comparing `pycloudevents-0.1.3.tar` & `pycloudevents-0.1.4.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0    11357 2024-04-16 05:59:50.172518 pycloudevents-0.1.3/LICENSE
--rw-r--r--   0        0        0     3497 2024-04-16 05:59:50.172518 pycloudevents-0.1.3/README.md
--rw-r--r--   0        0        0      805 2024-04-16 06:00:02.828579 pycloudevents-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       62 2024-04-16 05:59:50.176518 pycloudevents-0.1.3/src/pycloudevents/__init__.py
--rw-r--r--   0        0        0     6696 2024-04-16 05:59:50.176518 pycloudevents-0.1.3/src/pycloudevents/cloudevent.py
--rw-r--r--   0        0        0       44 2024-04-16 05:59:50.176518 pycloudevents-0.1.3/src/pycloudevents/exceptions.py
--rw-r--r--   0        0        0      651 2024-04-16 05:59:50.176518 pycloudevents-0.1.3/tests/__init__.py
--rw-r--r--   0        0        0     1297 2024-04-16 05:59:50.176518 pycloudevents-0.1.3/tests/test_spec_1_0.py
--rw-r--r--   0        0        0     4074 1970-01-01 00:00:00.000000 pycloudevents-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-16 06:40:21.099001 pycloudevents-0.1.4/LICENSE
+-rw-r--r--   0        0        0     3497 2024-04-16 06:40:21.099001 pycloudevents-0.1.4/README.md
+-rw-r--r--   0        0        0      805 2024-04-16 06:40:37.723030 pycloudevents-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0       62 2024-04-16 06:40:21.099001 pycloudevents-0.1.4/src/pycloudevents/__init__.py
+-rw-r--r--   0        0        0     7038 2024-04-16 06:40:21.099001 pycloudevents-0.1.4/src/pycloudevents/cloudevent.py
+-rw-r--r--   0        0        0       44 2024-04-16 06:40:21.099001 pycloudevents-0.1.4/src/pycloudevents/exceptions.py
+-rw-r--r--   0        0        0      651 2024-04-16 06:40:21.099001 pycloudevents-0.1.4/tests/__init__.py
+-rw-r--r--   0        0        0     1344 2024-04-16 06:40:21.099001 pycloudevents-0.1.4/tests/test_cloudevent.py
+-rw-r--r--   0        0        0     1297 2024-04-16 06:40:21.099001 pycloudevents-0.1.4/tests/test_spec_1_0.py
+-rw-r--r--   0        0        0     4074 1970-01-01 00:00:00.000000 pycloudevents-0.1.4/PKG-INFO
```

### Comparing `pycloudevents-0.1.3/LICENSE` & `pycloudevents-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pycloudevents-0.1.3/README.md` & `pycloudevents-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pycloudevents-0.1.3/pyproject.toml` & `pycloudevents-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pycloudevents"
-version = "0.1.3"
+version = "0.1.4"
 description = "A third party cloudevents 1.0 SDK for Python."
 authors = [
     { name = "-LAN-", email = "laipz8200@outlook.com" },
 ]
 dependencies = []
 requires-python = ">=3.11"
 readme = "README.md"
```

### Comparing `pycloudevents-0.1.3/src/pycloudevents/cloudevent.py` & `pycloudevents-0.1.4/src/pycloudevents/cloudevent.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,24 @@
 
         self._validation_errors: list[str] = []
 
     def __getattr__(self, name: str) -> Any:
         attr = self._extensions.get(name)
         return attr
 
+    def _to_string(self):
+        subject = f'"{self._subject}"' if self._subject else ""
+        return f'<pycloudevents.CloudEvent ({self._specversion}) "{self._type}" "{self._id}" "{self._source}" {subject}>'
+
+    def __repr__(self) -> str:
+        return self._to_string()
+
+    def __str__(self) -> str:
+        return self._to_string()
+
     @property
     def id(self) -> str:
         return self._id
 
     @property
     def specversion(self) -> str:
         return self._specversion
```

### Comparing `pycloudevents-0.1.3/tests/__init__.py` & `pycloudevents-0.1.4/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pycloudevents-0.1.3/tests/test_spec_1_0.py` & `pycloudevents-0.1.4/tests/test_spec_1_0.py`

 * *Files identical despite different names*

### Comparing `pycloudevents-0.1.3/PKG-INFO` & `pycloudevents-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycloudevents
-Version: 0.1.3
+Version: 0.1.4
 Summary: A third party cloudevents 1.0 SDK for Python.
 Keywords: cloudevents
 Author-Email: -LAN- <laipz8200@outlook.com>
 License: Apache2.0
 Project-URL: Homepage, https://github.com/laipz8200/pycloudevents
 Project-URL: Repository, https://github.com/laipz8200/pycloudevents
 Project-URL: Documentation, https://github.com/laipz8200/pycloudevents/blob/main/README.md
```

