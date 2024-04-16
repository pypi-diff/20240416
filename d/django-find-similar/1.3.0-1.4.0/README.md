# Comparing `tmp/django-find-similar-1.3.0.tar.gz` & `tmp/django_find_similar-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-find-similar-1.3.0.tar", last modified: Mon Nov  6 14:30:11 2023, max compression
+gzip compressed data, was "django_find_similar-1.4.0.tar", last modified: Tue Apr 16 14:52:19 2024, max compression
```

## Comparing `django-find-similar-1.3.0.tar` & `django_find_similar-1.4.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 14:30:11.078651 django-find-similar-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2023-11-06 14:30:01.000000 django-find-similar-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7283 2023-11-06 14:30:11.078651 django-find-similar-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6118 2023-11-06 14:30:01.000000 django-find-similar-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 14:30:11.074651 django-find-similar-1.3.0/django_find_similar/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-06 14:30:01.000000 django-find-similar-1.3.0/django_find_similar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2023-11-06 14:30:01.000000 django-find-similar-1.3.0/django_find_similar/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      275 2023-11-06 14:30:01.000000 django-find-similar-1.3.0/django_find_similar/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      377 2023-11-06 14:30:01.000000 django-find-similar-1.3.0/django_find_similar/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 14:30:11.074651 django-find-similar-1.3.0/django_find_similar/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     3160 2023-11-06 14:30:01.000000 django-find-similar-1.3.0/django_find_similar/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-06 14:30:01.000000 django-find-similar-1.3.0/django_find_similar/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 14:30:11.078651 django-find-similar-1.3.0/django_find_similar/models/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2023-11-06 14:30:01.000000 django-find-similar-1.3.0/django_find_similar/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      890 2023-11-06 14:30:01.000000 django-find-similar-1.3.0/django_find_similar/models/adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2023-11-06 14:30:01.000000 django-find-similar-1.3.0/django_find_similar/models/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2023-11-06 14:30:01.000000 django-find-similar-1.3.0/django_find_similar/models/text.py
--rw-r--r--   0 runner    (1001) docker     (127)       88 2023-11-06 14:30:01.000000 django-find-similar-1.3.0/django_find_similar/package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 14:30:11.078651 django-find-similar-1.3.0/django_find_similar/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-11-06 14:30:01.000000 django-find-similar-1.3.0/django_find_similar/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2023-11-06 14:30:01.000000 django-find-similar-1.3.0/django_find_similar/tests/test_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2023-11-06 14:30:01.000000 django-find-similar-1.3.0/django_find_similar/tests/test_forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     3015 2023-11-06 14:30:01.000000 django-find-similar-1.3.0/django_find_similar/tests/tests_models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 14:30:11.074651 django-find-similar-1.3.0/django_find_similar.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7283 2023-11-06 14:30:11.000000 django-find-similar-1.3.0/django_find_similar.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      748 2023-11-06 14:30:11.000000 django-find-similar-1.3.0/django_find_similar.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-06 14:30:11.000000 django-find-similar-1.3.0/django_find_similar.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-11-06 14:30:11.000000 django-find-similar-1.3.0/django_find_similar.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-06 14:30:11.078651 django-find-similar-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3213 2023-11-06 14:30:01.000000 django-find-similar-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:52:19.641166 django_find_similar-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-16 14:52:15.000000 django_find_similar-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7253 2024-04-16 14:52:19.641166 django_find_similar-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6093 2024-04-16 14:52:15.000000 django_find_similar-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:52:19.637166 django_find_similar-1.4.0/django_find_similar/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 14:52:15.000000 django_find_similar-1.4.0/django_find_similar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-16 14:52:15.000000 django_find_similar-1.4.0/django_find_similar/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-16 14:52:15.000000 django_find_similar-1.4.0/django_find_similar/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-16 14:52:15.000000 django_find_similar-1.4.0/django_find_similar/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:52:19.637166 django_find_similar-1.4.0/django_find_similar/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     3160 2024-04-16 14:52:15.000000 django_find_similar-1.4.0/django_find_similar/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 14:52:15.000000 django_find_similar-1.4.0/django_find_similar/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:52:19.641166 django_find_similar-1.4.0/django_find_similar/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-16 14:52:15.000000 django_find_similar-1.4.0/django_find_similar/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-16 14:52:15.000000 django_find_similar-1.4.0/django_find_similar/models/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-16 14:52:15.000000 django_find_similar-1.4.0/django_find_similar/models/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-04-16 14:52:15.000000 django_find_similar-1.4.0/django_find_similar/models/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-16 14:52:15.000000 django_find_similar-1.4.0/django_find_similar/package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:52:19.641166 django_find_similar-1.4.0/django_find_similar/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-16 14:52:15.000000 django_find_similar-1.4.0/django_find_similar/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-16 14:52:15.000000 django_find_similar-1.4.0/django_find_similar/tests/test_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-16 14:52:15.000000 django_find_similar-1.4.0/django_find_similar/tests/test_forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-04-16 14:52:15.000000 django_find_similar-1.4.0/django_find_similar/tests/tests_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:52:19.641166 django_find_similar-1.4.0/django_find_similar.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7253 2024-04-16 14:52:19.000000 django_find_similar-1.4.0/django_find_similar.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-16 14:52:19.000000 django_find_similar-1.4.0/django_find_similar.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 14:52:19.000000 django_find_similar-1.4.0/django_find_similar.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-16 14:52:19.000000 django_find_similar-1.4.0/django_find_similar.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 14:52:19.641166 django_find_similar-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-04-16 14:52:15.000000 django_find_similar-1.4.0/setup.py
```

### Comparing `django-find-similar-1.3.0/LICENSE` & `django_find_similar-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-find-similar-1.3.0/PKG-INFO` & `django_find_similar-1.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: django-find-similar
-Version: 1.3.0
+Version: 1.4.0
 Summary: find-similar integration for django
 Home-page: https://github.com/findsimilar/django-find-similar
 Author: quillcraftsman
 Author-email: quill@craftsman.lol
 License: MIT
-Project-URL: Documentation, https://django.findsimilar.org
+Project-URL: Documentation, https://dfs.craftsman.lol
 Project-URL: Source, https://github.com/findsimilar/django-find-similar
 Project-URL: Tracker, https://github.com/findsimilar/django-find-similar/issues
 Project-URL: Release notes, https://github.com/findsimilar/django-find-similar/releases
 Project-URL: Changelog, https://github.com/findsimilar/django-find-similar/releases
 Project-URL: Download, https://pypi.org/project/django-find-similar/
 Keywords: python,django,find-similar,integration
 Classifier: Development Status :: 4 - Beta
@@ -115,30 +115,30 @@
 
 - Django models
 - Django forms
 
 ## Requirements
 
 - django, find-similar
-- See more in [Full Documentation](https://django.findsimilar.org/about.html#requirements)
+- See more in [Full Documentation](https://dfs.craftsman.lol/about.html#requirements)
 
 ## Development Status
 
 - Package already available on [PyPi](https://pypi.org/project/django-find-similar/)
-- See more in [Full Documentation](https://django.findsimilar.org/about.html#development-status)
+- See more in [Full Documentation](https://dfs.craftsman.lol/about.html#development-status)
 
 ## Install
 
 ### with pip
 
 ```commandline
 pip install django-find-similar
 ```
 
-See more in [Full Documentation](https://django.findsimilar.org/install.html)
+See more in [Full Documentation](https://dfs.craftsman.lol/install.html)
 
 ## Quickstart
 
 ```python
 from django_find_similar.models import FindSimilarInput, Text
 
 input_data = {
@@ -165,14 +165,14 @@
 ### More examples in [Full Documentation][documentation_path]
 
 ## Contributing
 
 You are welcome! To easy start please check:
 - [Full Documentation][documentation_path]
 - [Contributing](CONTRIBUTING.md)
-- [Developer Documentation](https://django.findsimilar.org/dev_documentation.html)
+- [Developer Documentation](https://dfs.craftsman.lol/dev_documentation.html)
 - [Code of Conduct](CODE_OF_CONDUCT.md)
 - [Security Policy](SECURITY.md)
 - [Governance](GOVERNANCE.md)
 - [Support](SUPPORT.md)
 
-[documentation_path]: https://django.findsimilar.org
+[documentation_path]: https://dfs.craftsman.lol
```

### Comparing `django-find-similar-1.3.0/README.md` & `django_find_similar-1.4.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -88,30 +88,30 @@
 
 - Django models
 - Django forms
 
 ## Requirements
 
 - django, find-similar
-- See more in [Full Documentation](https://django.findsimilar.org/about.html#requirements)
+- See more in [Full Documentation](https://dfs.craftsman.lol/about.html#requirements)
 
 ## Development Status
 
 - Package already available on [PyPi](https://pypi.org/project/django-find-similar/)
-- See more in [Full Documentation](https://django.findsimilar.org/about.html#development-status)
+- See more in [Full Documentation](https://dfs.craftsman.lol/about.html#development-status)
 
 ## Install
 
 ### with pip
 
 ```commandline
 pip install django-find-similar
 ```
 
-See more in [Full Documentation](https://django.findsimilar.org/install.html)
+See more in [Full Documentation](https://dfs.craftsman.lol/install.html)
 
 ## Quickstart
 
 ```python
 from django_find_similar.models import FindSimilarInput, Text
 
 input_data = {
@@ -138,14 +138,14 @@
 ### More examples in [Full Documentation][documentation_path]
 
 ## Contributing
 
 You are welcome! To easy start please check:
 - [Full Documentation][documentation_path]
 - [Contributing](CONTRIBUTING.md)
-- [Developer Documentation](https://django.findsimilar.org/dev_documentation.html)
+- [Developer Documentation](https://dfs.craftsman.lol/dev_documentation.html)
 - [Code of Conduct](CODE_OF_CONDUCT.md)
 - [Security Policy](SECURITY.md)
 - [Governance](GOVERNANCE.md)
 - [Support](SUPPORT.md)
 
-[documentation_path]: https://django.findsimilar.org
+[documentation_path]: https://dfs.craftsman.lol
```

### Comparing `django-find-similar-1.3.0/django_find_similar/migrations/0001_initial.py` & `django_find_similar-1.4.0/django_find_similar/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-find-similar-1.3.0/django_find_similar/models/adapter.py` & `django_find_similar-1.4.0/django_find_similar/models/adapter.py`

 * *Files identical despite different names*

### Comparing `django-find-similar-1.3.0/django_find_similar/models/result.py` & `django_find_similar-1.4.0/django_find_similar/models/result.py`

 * *Files identical despite different names*

### Comparing `django-find-similar-1.3.0/django_find_similar/models/text.py` & `django_find_similar-1.4.0/django_find_similar/models/text.py`

 * *Files identical despite different names*

### Comparing `django-find-similar-1.3.0/django_find_similar/tests/test_adapter.py` & `django_find_similar-1.4.0/django_find_similar/tests/test_adapter.py`

 * *Files identical despite different names*

### Comparing `django-find-similar-1.3.0/django_find_similar/tests/test_forms.py` & `django_find_similar-1.4.0/django_find_similar/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `django-find-similar-1.3.0/django_find_similar/tests/tests_models.py` & `django_find_similar-1.4.0/django_find_similar/tests/tests_models.py`

 * *Files identical despite different names*

### Comparing `django-find-similar-1.3.0/django_find_similar.egg-info/PKG-INFO` & `django_find_similar-1.4.0/django_find_similar.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: django-find-similar
-Version: 1.3.0
+Version: 1.4.0
 Summary: find-similar integration for django
 Home-page: https://github.com/findsimilar/django-find-similar
 Author: quillcraftsman
 Author-email: quill@craftsman.lol
 License: MIT
-Project-URL: Documentation, https://django.findsimilar.org
+Project-URL: Documentation, https://dfs.craftsman.lol
 Project-URL: Source, https://github.com/findsimilar/django-find-similar
 Project-URL: Tracker, https://github.com/findsimilar/django-find-similar/issues
 Project-URL: Release notes, https://github.com/findsimilar/django-find-similar/releases
 Project-URL: Changelog, https://github.com/findsimilar/django-find-similar/releases
 Project-URL: Download, https://pypi.org/project/django-find-similar/
 Keywords: python,django,find-similar,integration
 Classifier: Development Status :: 4 - Beta
@@ -115,30 +115,30 @@
 
 - Django models
 - Django forms
 
 ## Requirements
 
 - django, find-similar
-- See more in [Full Documentation](https://django.findsimilar.org/about.html#requirements)
+- See more in [Full Documentation](https://dfs.craftsman.lol/about.html#requirements)
 
 ## Development Status
 
 - Package already available on [PyPi](https://pypi.org/project/django-find-similar/)
-- See more in [Full Documentation](https://django.findsimilar.org/about.html#development-status)
+- See more in [Full Documentation](https://dfs.craftsman.lol/about.html#development-status)
 
 ## Install
 
 ### with pip
 
 ```commandline
 pip install django-find-similar
 ```
 
-See more in [Full Documentation](https://django.findsimilar.org/install.html)
+See more in [Full Documentation](https://dfs.craftsman.lol/install.html)
 
 ## Quickstart
 
 ```python
 from django_find_similar.models import FindSimilarInput, Text
 
 input_data = {
@@ -165,14 +165,14 @@
 ### More examples in [Full Documentation][documentation_path]
 
 ## Contributing
 
 You are welcome! To easy start please check:
 - [Full Documentation][documentation_path]
 - [Contributing](CONTRIBUTING.md)
-- [Developer Documentation](https://django.findsimilar.org/dev_documentation.html)
+- [Developer Documentation](https://dfs.craftsman.lol/dev_documentation.html)
 - [Code of Conduct](CODE_OF_CONDUCT.md)
 - [Security Policy](SECURITY.md)
 - [Governance](GOVERNANCE.md)
 - [Support](SUPPORT.md)
 
-[documentation_path]: https://django.findsimilar.org
+[documentation_path]: https://dfs.craftsman.lol
```

### Comparing `django-find-similar-1.3.0/django_find_similar.egg-info/SOURCES.txt` & `django_find_similar-1.4.0/django_find_similar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-find-similar-1.3.0/setup.py` & `django_find_similar-1.4.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         return val.strip().replace("'", '')
     return None
 
 
 PACKAGE_NAME = "django_find_similar"
 
 PROJECT_URLS = {
-    'Documentation': 'https://django.findsimilar.org',
+    'Documentation': 'https://dfs.craftsman.lol',
     'Source': 'https://github.com/findsimilar/django-find-similar',
     'Tracker': 'https://github.com/findsimilar/django-find-similar/issues',
     'Release notes': 'https://github.com/findsimilar/django-find-similar/releases',
     'Changelog': 'https://github.com/findsimilar/django-find-similar/releases',
     'Download': 'https://pypi.org/project/django-find-similar/',
 }
```

