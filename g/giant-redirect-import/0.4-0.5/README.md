# Comparing `tmp/giant_redirect_import-0.4.tar.gz` & `tmp/giant_redirect_import-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "giant_redirect_import-0.4.tar", max compression
+gzip compressed data, was "giant_redirect_import-0.5.tar", max compression
```

## Comparing `giant_redirect_import-0.4.tar` & `giant_redirect_import-0.5.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1069 2023-05-26 08:46:49.460663 giant_redirect_import-0.4/LICENSE
--rw-r--r--   0        0        0     1663 2023-05-26 08:46:49.460663 giant_redirect_import-0.4/README.md
--rw-r--r--   0        0        0        0 2023-05-26 08:46:49.460663 giant_redirect_import-0.4/giant_redirect_import/__init__.py
--rw-r--r--   0        0        0     2757 2023-10-27 10:30:36.011478 giant_redirect_import-0.4/giant_redirect_import/admin.py
--rw-r--r--   0        0        0      104 2023-09-29 09:47:31.628312 giant_redirect_import-0.4/giant_redirect_import/apps.py
--rw-r--r--   0        0        0     2084 2023-05-26 08:46:49.460663 giant_redirect_import-0.4/giant_redirect_import/forms.py
--rw-r--r--   0        0        0        0 2023-05-26 08:46:49.460663 giant_redirect_import-0.4/giant_redirect_import/tests/__init__.py
--rw-r--r--   0        0        0     1134 2023-10-16 06:43:28.895782 giant_redirect_import-0.4/pyproject.toml
--rw-r--r--   0        0        0     2656 1970-01-01 00:00:00.000000 giant_redirect_import-0.4/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-16 12:33:05.043704 giant_redirect_import-0.5/LICENSE
+-rw-r--r--   0        0        0     1663 2024-04-16 12:33:05.043863 giant_redirect_import-0.5/README.md
+-rw-r--r--   0        0        0        0 2024-04-16 12:33:05.046044 giant_redirect_import-0.5/giant_redirect_import/__init__.py
+-rw-r--r--   0        0        0     2757 2024-04-16 12:33:05.046221 giant_redirect_import-0.5/giant_redirect_import/admin.py
+-rw-r--r--   0        0        0      104 2024-04-16 12:33:05.046331 giant_redirect_import-0.5/giant_redirect_import/apps.py
+-rw-r--r--   0        0        0     2084 2024-04-16 12:33:05.046454 giant_redirect_import-0.5/giant_redirect_import/forms.py
+-rw-r--r--   0        0        0        0 2024-04-16 12:33:05.046579 giant_redirect_import-0.5/giant_redirect_import/tests/__init__.py
+-rw-r--r--   0        0        0     1111 2024-04-16 13:51:34.476320 giant_redirect_import-0.5/pyproject.toml
+-rw-r--r--   0        0        0     2531 1970-01-01 00:00:00.000000 giant_redirect_import-0.5/setup.py
+-rw-r--r--   0        0        0     2655 1970-01-01 00:00:00.000000 giant_redirect_import-0.5/PKG-INFO
```

### Comparing `giant_redirect_import-0.4/LICENSE` & `giant_redirect_import-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `giant_redirect_import-0.4/README.md` & `giant_redirect_import-0.5/README.md`

 * *Files identical despite different names*

### Comparing `giant_redirect_import-0.4/giant_redirect_import/admin.py` & `giant_redirect_import-0.5/giant_redirect_import/admin.py`

 * *Files identical despite different names*

### Comparing `giant_redirect_import-0.4/giant_redirect_import/forms.py` & `giant_redirect_import-0.5/giant_redirect_import/forms.py`

 * *Files identical despite different names*

### Comparing `giant_redirect_import-0.4/pyproject.toml` & `giant_redirect_import-0.5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "giant-redirect-import"
-version = "0.4"
+version = "0.5"
 description = "Reusable package which adds an option to bulk import redirects from a csv file"
 authors = ["Will-Hoey <will.hoey@hotmail.co.uk>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/giantmade/giant-redirect-import"
 repository = "https://github.com/giantmade/giant-redirect-import"
 keywords = ["import", "app"]
@@ -21,25 +21,24 @@
     { include = "giant_redirect_import" }
 ]
 
 [tool.poetry.dependencies]
 django = "^3.2"
 python = "^3.10"
 django-import-export = "^3.2.0"
-django-cms = "^3.10"
+django-cms = "^4.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 black = ">22.7"
 pytest-django = "^3.9.0"
 pytest-cov = "^2.10.0"
 pytest-mock = "^3.2.0"
 
 
 [[tool.poetry.source]]
 name = "TestPyPi"
 url = "https://test.pypi.org/simple/"
-priority = "explicit"
 
 [build-system]
 requires = ["poetry>=1.0.0"]
 build-backend = "poetry.masonry.api"
```

### Comparing `giant_redirect_import-0.4/PKG-INFO` & `giant_redirect_import-0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: giant-redirect-import
-Version: 0.4
+Version: 0.5
 Summary: Reusable package which adds an option to bulk import redirects from a csv file
 Home-page: https://github.com/giantmade/giant-redirect-import
 License: MIT
 Keywords: import,app
 Author: Will-Hoey
 Author-email: will.hoey@hotmail.co.uk
 Requires-Python: >=3.10,<4.0
@@ -13,15 +13,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: django (>=3.2,<4.0)
-Requires-Dist: django-cms (>=3.10,<4.0)
+Requires-Dist: django-cms (>=4.0,<5.0)
 Requires-Dist: django-import-export (>=3.2.0,<4.0.0)
 Project-URL: Repository, https://github.com/giantmade/giant-redirect-import
 Description-Content-Type: text/markdown
 
 # Giant Redirect Import
 
 A re-usable package which can be used in any project that requires a Redirect import via a CSV file.
```

