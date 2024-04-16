# Comparing `tmp/ninja_snake_lib-0.2.0.tar.gz` & `tmp/ninja_snake_lib-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ninja_snake_lib-0.2.0.tar", max compression
+gzip compressed data, was "ninja_snake_lib-0.2.1.tar", max compression
```

## Comparing `ninja_snake_lib-0.2.0.tar` & `ninja_snake_lib-0.2.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1491 2023-08-11 11:51:49.282386 ninja_snake_lib-0.2.0/LICENSE
--rw-r--r--   0        0        0     4458 2023-08-11 20:09:08.357555 ninja_snake_lib-0.2.0/README.md
--rw-r--r--   0        0        0     1443 2023-08-11 17:20:07.275882 ninja_snake_lib-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      114 2023-08-11 11:51:50.720097 ninja_snake_lib-0.2.0/src/ninja_snake_lib/__init__.py
--rw-r--r--   0        0        0     1508 2023-08-11 11:51:50.818223 ninja_snake_lib-0.2.0/src/ninja_snake_lib/decorators.py
--rw-r--r--   0        0        0     1951 2023-08-04 19:54:32.269689 ninja_snake_lib-0.2.0/src/ninja_snake_lib/event.py
--rw-r--r--   0        0        0     6166 2023-08-11 13:05:22.059633 ninja_snake_lib-0.2.0/src/ninja_snake_lib/json_formatter.py
--rw-r--r--   0        0        0     3036 2023-08-11 13:58:55.402178 ninja_snake_lib-0.2.0/src/ninja_snake_lib/log_formatter.py
--rw-r--r--   0        0        0      770 2023-08-11 11:51:50.780599 ninja_snake_lib-0.2.0/src/ninja_snake_lib/read_dotenv.py
--rw-r--r--   0        0        0      643 2023-06-30 10:41:42.503497 ninja_snake_lib-0.2.0/src/ninja_snake_lib/setup_correlation_id.py
--rw-r--r--   0        0        0     3209 2023-08-04 19:56:38.037680 ninja_snake_lib-0.2.0/src/ninja_snake_lib/tracker.py
--rw-r--r--   0        0        0     5336 1970-01-01 00:00:00.000000 ninja_snake_lib-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1491 2024-04-16 20:35:03.420087 ninja_snake_lib-0.2.1/LICENSE
+-rw-r--r--   0        0        0     4458 2024-04-16 20:35:03.420087 ninja_snake_lib-0.2.1/README.md
+-rw-r--r--   0        0        0     1444 2024-04-16 20:37:17.844941 ninja_snake_lib-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      114 2024-04-16 20:35:03.420087 ninja_snake_lib-0.2.1/src/ninja_snake_lib/__init__.py
+-rw-r--r--   0        0        0     1508 2024-04-16 20:35:03.420087 ninja_snake_lib-0.2.1/src/ninja_snake_lib/decorators.py
+-rw-r--r--   0        0        0     1951 2024-04-16 20:35:03.420087 ninja_snake_lib-0.2.1/src/ninja_snake_lib/event.py
+-rw-r--r--   0        0        0     6166 2024-04-16 20:35:03.420087 ninja_snake_lib-0.2.1/src/ninja_snake_lib/json_formatter.py
+-rw-r--r--   0        0        0     3036 2024-04-16 20:35:03.424087 ninja_snake_lib-0.2.1/src/ninja_snake_lib/log_formatter.py
+-rw-r--r--   0        0        0      770 2024-04-16 20:35:03.424087 ninja_snake_lib-0.2.1/src/ninja_snake_lib/read_dotenv.py
+-rw-r--r--   0        0        0      643 2024-04-16 20:35:03.424087 ninja_snake_lib-0.2.1/src/ninja_snake_lib/setup_correlation_id.py
+-rw-r--r--   0        0        0     3209 2024-04-16 20:35:03.424087 ninja_snake_lib-0.2.1/src/ninja_snake_lib/tracker.py
+-rw-r--r--   0        0        0     5388 1970-01-01 00:00:00.000000 ninja_snake_lib-0.2.1/PKG-INFO
```

### Comparing `ninja_snake_lib-0.2.0/LICENSE` & `ninja_snake_lib-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ninja_snake_lib-0.2.0/README.md` & `ninja_snake_lib-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `ninja_snake_lib-0.2.0/pyproject.toml` & `ninja_snake_lib-0.2.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "NINJA-SNAKE-LIB"
-version = "0.2.0"
+version = "0.2.1"
 description = "Biblioteca utilitaria para projetos Python no Getninjas"
 authors = [
     "Carlos Sá <carlos.sa@getninjas.com.br>",
 ]
 license = "BSD"
 readme = "README.md"
 packages = [
@@ -20,15 +20,15 @@
 [tool.poetry.urls]
 "Código" = "https://github.com/getninjas/ninja-snake-lib"
 "Bug Tracker" = "https://github.com/getninjas/ninja-snake-lib/issues"
 
 
 [tool.poetry.dependencies]
 python = "^3.10"
-django = "^4.2.4"
+django = "^3.2.18"
 requests = "^2.31.0"
 json-log-formatter = "^0.5.2"
 contextvars = "^2.4"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.0"
 coverage = "^7.2.7"
```

### Comparing `ninja_snake_lib-0.2.0/src/ninja_snake_lib/decorators.py` & `ninja_snake_lib-0.2.1/src/ninja_snake_lib/decorators.py`

 * *Files identical despite different names*

### Comparing `ninja_snake_lib-0.2.0/src/ninja_snake_lib/event.py` & `ninja_snake_lib-0.2.1/src/ninja_snake_lib/event.py`

 * *Files identical despite different names*

### Comparing `ninja_snake_lib-0.2.0/src/ninja_snake_lib/json_formatter.py` & `ninja_snake_lib-0.2.1/src/ninja_snake_lib/json_formatter.py`

 * *Files identical despite different names*

### Comparing `ninja_snake_lib-0.2.0/src/ninja_snake_lib/log_formatter.py` & `ninja_snake_lib-0.2.1/src/ninja_snake_lib/log_formatter.py`

 * *Files identical despite different names*

### Comparing `ninja_snake_lib-0.2.0/src/ninja_snake_lib/read_dotenv.py` & `ninja_snake_lib-0.2.1/src/ninja_snake_lib/read_dotenv.py`

 * *Files identical despite different names*

### Comparing `ninja_snake_lib-0.2.0/src/ninja_snake_lib/setup_correlation_id.py` & `ninja_snake_lib-0.2.1/src/ninja_snake_lib/setup_correlation_id.py`

 * *Files identical despite different names*

### Comparing `ninja_snake_lib-0.2.0/src/ninja_snake_lib/tracker.py` & `ninja_snake_lib-0.2.1/src/ninja_snake_lib/tracker.py`

 * *Files identical despite different names*

### Comparing `ninja_snake_lib-0.2.0/PKG-INFO` & `ninja_snake_lib-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
-Name: ninja-snake-lib
-Version: 0.2.0
+Name: NINJA-SNAKE-LIB
+Version: 0.2.1
 Summary: Biblioteca utilitaria para projetos Python no Getninjas
 License: BSD
 Author: Carlos Sá
 Author-email: carlos.sa@getninjas.com.br
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: contextvars (>=2.4,<3.0)
-Requires-Dist: django (>=4.2.4,<5.0.0)
+Requires-Dist: django (>=3.2.18,<4.0.0)
 Requires-Dist: json-log-formatter (>=0.5.2,<0.6.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Project-URL: Bug Tracker, https://github.com/getninjas/ninja-snake-lib/issues
 Project-URL: Código, https://github.com/getninjas/ninja-snake-lib
 Description-Content-Type: text/markdown
 
 # Ninja Snake Lib
```

