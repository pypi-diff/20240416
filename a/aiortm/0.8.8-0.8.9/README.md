# Comparing `tmp/aiortm-0.8.8.tar.gz` & `tmp/aiortm-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiortm-0.8.8.tar", max compression
+gzip compressed data, was "aiortm-0.8.9.tar", max compression
```

## Comparing `aiortm-0.8.8.tar` & `aiortm-0.8.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    11346 2024-01-28 17:19:37.179622 aiortm-0.8.8/LICENSE
--rw-r--r--   0        0        0     2785 2024-01-28 17:19:37.179622 aiortm-0.8.8/README.md
--rw-r--r--   0        0        0     3520 2024-01-28 17:19:38.223621 aiortm-0.8.8/pyproject.toml
--rw-r--r--   0        0        0      488 2024-01-28 17:19:38.223621 aiortm-0.8.8/src/aiortm/__init__.py
--rw-r--r--   0        0        0      694 2024-01-28 17:19:37.183622 aiortm-0.8.8/src/aiortm/cli/__init__.py
--rw-r--r--   0        0        0     3666 2024-01-28 17:19:37.183622 aiortm-0.8.8/src/aiortm/cli/app.py
--rw-r--r--   0        0        0     5379 2024-01-28 17:19:37.183622 aiortm-0.8.8/src/aiortm/client.py
--rw-r--r--   0        0        0     1117 2024-01-28 17:19:37.183622 aiortm-0.8.8/src/aiortm/exceptions.py
--rw-r--r--   0        0        0      658 2024-01-28 17:19:37.183622 aiortm-0.8.8/src/aiortm/model/__init__.py
--rw-r--r--   0        0        0     2158 2024-01-28 17:19:37.183622 aiortm-0.8.8/src/aiortm/model/contacts.py
--rw-r--r--   0        0        0      678 2024-01-28 17:19:37.183622 aiortm-0.8.8/src/aiortm/model/response.py
--rw-r--r--   0        0        0     5479 2024-01-28 17:19:37.183622 aiortm-0.8.8/src/aiortm/model/tasks.py
--rw-r--r--   0        0        0      597 2024-01-28 17:19:37.183622 aiortm-0.8.8/src/aiortm/model/timelines.py
--rw-r--r--   0        0        0        0 2024-01-28 17:19:37.183622 aiortm-0.8.8/src/aiortm/py.typed
--rw-r--r--   0        0        0     4045 1970-01-01 00:00:00.000000 aiortm-0.8.8/PKG-INFO
+-rw-r--r--   0        0        0    11346 2024-01-29 04:23:55.585343 aiortm-0.8.9/LICENSE
+-rw-r--r--   0        0        0     2785 2024-01-29 04:23:55.585343 aiortm-0.8.9/README.md
+-rw-r--r--   0        0        0     3520 2024-01-29 04:23:56.593345 aiortm-0.8.9/pyproject.toml
+-rw-r--r--   0        0        0      488 2024-01-29 04:23:56.593345 aiortm-0.8.9/src/aiortm/__init__.py
+-rw-r--r--   0        0        0      694 2024-01-29 04:23:55.589343 aiortm-0.8.9/src/aiortm/cli/__init__.py
+-rw-r--r--   0        0        0     3666 2024-01-29 04:23:55.589343 aiortm-0.8.9/src/aiortm/cli/app.py
+-rw-r--r--   0        0        0     5379 2024-01-29 04:23:55.589343 aiortm-0.8.9/src/aiortm/client.py
+-rw-r--r--   0        0        0     1117 2024-01-29 04:23:55.589343 aiortm-0.8.9/src/aiortm/exceptions.py
+-rw-r--r--   0        0        0      658 2024-01-29 04:23:55.589343 aiortm-0.8.9/src/aiortm/model/__init__.py
+-rw-r--r--   0        0        0     2158 2024-01-29 04:23:55.589343 aiortm-0.8.9/src/aiortm/model/contacts.py
+-rw-r--r--   0        0        0      678 2024-01-29 04:23:55.589343 aiortm-0.8.9/src/aiortm/model/response.py
+-rw-r--r--   0        0        0     5479 2024-01-29 04:23:55.589343 aiortm-0.8.9/src/aiortm/model/tasks.py
+-rw-r--r--   0        0        0      597 2024-01-29 04:23:55.589343 aiortm-0.8.9/src/aiortm/model/timelines.py
+-rw-r--r--   0        0        0        0 2024-01-29 04:23:55.589343 aiortm-0.8.9/src/aiortm/py.typed
+-rw-r--r--   0        0        0     4045 1970-01-01 00:00:00.000000 aiortm-0.8.9/PKG-INFO
```

### Comparing `aiortm-0.8.8/LICENSE` & `aiortm-0.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aiortm-0.8.8/README.md` & `aiortm-0.8.9/README.md`

 * *Files identical despite different names*

### Comparing `aiortm-0.8.8/pyproject.toml` & `aiortm-0.8.9/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 license = "Apache Software License 2.0"
 name = "aiortm"
 packages = [
   {include = "aiortm", from = "src"},
 ]
 readme = "README.md"
 repository = "https://github.com/MartinHjelmare/aiortm"
-version = "0.8.8"
+version = "0.8.9"
 
 [tool.poetry.scripts]
 aiortm = 'aiortm.cli:cli'
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/MartinHjelmare/aiortm/issues"
 "Changelog" = "https://github.com/MartinHjelmare/aiortm/blob/main/CHANGELOG.md"
```

### Comparing `aiortm-0.8.8/src/aiortm/cli/__init__.py` & `aiortm-0.8.9/src/aiortm/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `aiortm-0.8.8/src/aiortm/cli/app.py` & `aiortm-0.8.9/src/aiortm/cli/app.py`

 * *Files identical despite different names*

### Comparing `aiortm-0.8.8/src/aiortm/client.py` & `aiortm-0.8.9/src/aiortm/client.py`

 * *Files identical despite different names*

### Comparing `aiortm-0.8.8/src/aiortm/exceptions.py` & `aiortm-0.8.9/src/aiortm/exceptions.py`

 * *Files identical despite different names*

### Comparing `aiortm-0.8.8/src/aiortm/model/__init__.py` & `aiortm-0.8.9/src/aiortm/model/__init__.py`

 * *Files identical despite different names*

### Comparing `aiortm-0.8.8/src/aiortm/model/contacts.py` & `aiortm-0.8.9/src/aiortm/model/contacts.py`

 * *Files identical despite different names*

### Comparing `aiortm-0.8.8/src/aiortm/model/response.py` & `aiortm-0.8.9/src/aiortm/model/response.py`

 * *Files identical despite different names*

### Comparing `aiortm-0.8.8/src/aiortm/model/tasks.py` & `aiortm-0.8.9/src/aiortm/model/tasks.py`

 * *Files identical despite different names*

### Comparing `aiortm-0.8.8/src/aiortm/model/timelines.py` & `aiortm-0.8.9/src/aiortm/model/timelines.py`

 * *Files identical despite different names*

### Comparing `aiortm-0.8.8/PKG-INFO` & `aiortm-0.8.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiortm
-Version: 0.8.8
+Version: 0.8.9
 Summary: Use the Remember the Milk API with aiohttp.
 Home-page: https://github.com/MartinHjelmare/aiortm
 License: Apache Software License 2.0
 Author: Martin Hjelmare
 Author-email: marhje52@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: aiortm Version: 0.8.8 Summary: Use the Remember the
+Metadata-Version: 2.1 Name: aiortm Version: 0.8.9 Summary: Use the Remember the
 Milk API with aiohttp. Home-page: https://github.com/MartinHjelmare/aiortm
 License: Apache Software License 2.0 Author: Martin Hjelmare Author-email:
 marhje52@gmail.com Requires-Python: >=3.9,<4.0 Classifier: Development Status
 :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers Classifier:
 License :: Other/Proprietary License Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

