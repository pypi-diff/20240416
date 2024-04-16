# Comparing `tmp/giant_redirect_import-0.6.tar.gz` & `tmp/giant_redirect_import-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "giant_redirect_import-0.6.tar", max compression
+gzip compressed data, was "giant_redirect_import-0.7.tar", max compression
```

## Comparing `giant_redirect_import-0.6.tar` & `giant_redirect_import-0.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1069 2024-04-16 12:33:05.043704 giant_redirect_import-0.6/LICENSE
--rw-r--r--   0        0        0     1663 2024-04-16 12:33:05.043863 giant_redirect_import-0.6/README.md
--rw-r--r--   0        0        0        0 2024-04-16 12:33:05.046044 giant_redirect_import-0.6/giant_redirect_import/__init__.py
--rw-r--r--   0        0        0     2757 2024-04-16 12:33:05.046221 giant_redirect_import-0.6/giant_redirect_import/admin.py
--rw-r--r--   0        0        0      104 2024-04-16 12:33:05.046331 giant_redirect_import-0.6/giant_redirect_import/apps.py
--rw-r--r--   0        0        0     2084 2024-04-16 12:33:05.046454 giant_redirect_import-0.6/giant_redirect_import/forms.py
--rw-r--r--   0        0        0        0 2024-04-16 12:33:05.046579 giant_redirect_import-0.6/giant_redirect_import/tests/__init__.py
--rw-r--r--   0        0        0     1111 2024-04-16 14:36:41.000214 giant_redirect_import-0.6/pyproject.toml
--rw-r--r--   0        0        0     2531 1970-01-01 00:00:00.000000 giant_redirect_import-0.6/setup.py
--rw-r--r--   0        0        0     2655 1970-01-01 00:00:00.000000 giant_redirect_import-0.6/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-16 12:33:05.043704 giant_redirect_import-0.7/LICENSE
+-rw-r--r--   0        0        0     1663 2024-04-16 12:33:05.043863 giant_redirect_import-0.7/README.md
+-rw-r--r--   0        0        0        0 2024-04-16 12:33:05.046044 giant_redirect_import-0.7/giant_redirect_import/__init__.py
+-rw-r--r--   0        0        0     2757 2024-04-16 12:33:05.046221 giant_redirect_import-0.7/giant_redirect_import/admin.py
+-rw-r--r--   0        0        0      104 2024-04-16 12:33:05.046331 giant_redirect_import-0.7/giant_redirect_import/apps.py
+-rw-r--r--   0        0        0     2084 2024-04-16 12:33:05.046454 giant_redirect_import-0.7/giant_redirect_import/forms.py
+-rw-r--r--   0        0        0        0 2024-04-16 12:33:05.046579 giant_redirect_import-0.7/giant_redirect_import/tests/__init__.py
+-rw-r--r--   0        0        0     1111 2024-04-16 14:51:28.169329 giant_redirect_import-0.7/pyproject.toml
+-rw-r--r--   0        0        0     2531 1970-01-01 00:00:00.000000 giant_redirect_import-0.7/setup.py
+-rw-r--r--   0        0        0     2655 1970-01-01 00:00:00.000000 giant_redirect_import-0.7/PKG-INFO
```

### Comparing `giant_redirect_import-0.6/LICENSE` & `giant_redirect_import-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `giant_redirect_import-0.6/README.md` & `giant_redirect_import-0.7/README.md`

 * *Files identical despite different names*

### Comparing `giant_redirect_import-0.6/giant_redirect_import/admin.py` & `giant_redirect_import-0.7/giant_redirect_import/admin.py`

 * *Files identical despite different names*

### Comparing `giant_redirect_import-0.6/giant_redirect_import/forms.py` & `giant_redirect_import-0.7/giant_redirect_import/forms.py`

 * *Files identical despite different names*

### Comparing `giant_redirect_import-0.6/pyproject.toml` & `giant_redirect_import-0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "giant-redirect-import"
-version = "0.6"
+version = "0.7"
 description = "Reusable package which adds an option to bulk import redirects from a csv file"
 authors = ["Will-Hoey <will.hoey@hotmail.co.uk>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/giantmade/giant-redirect-import"
 repository = "https://github.com/giantmade/giant-redirect-import"
 keywords = ["import", "app"]
@@ -18,15 +18,15 @@
     "LICENSE",
 ]
 packages = [
     { include = "giant_redirect_import" }
 ]
 
 [tool.poetry.dependencies]
-django = "^5.0"
+django = "~4.2"
 python = "^3.10"
 django-import-export = "^3.2.0"
 django-cms = "^4.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 black = ">22.7"
```

### Comparing `giant_redirect_import-0.6/setup.py` & `giant_redirect_import-0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['django-cms>=4.0,<5.0',
  'django-import-export>=3.2.0,<4.0.0',
- 'django>=5.0,<6.0']
+ 'django>=4.2,<4.3']
 
 setup_kwargs = {
     'name': 'giant-redirect-import',
-    'version': '0.6',
+    'version': '0.7',
     'description': 'Reusable package which adds an option to bulk import redirects from a csv file',
     'long_description': '# Giant Redirect Import\n\nA re-usable package which can be used in any project that requires a Redirect import via a CSV file.\n\nThis will include a basic form to upload a CSV file in the standard `Redirect` app supplied via django.\n\n## Installation\n\nTo install with the package manager, run:\n\n    $ poetry add giant-redirect-import\n\nYou should then add `"giant_redirect_import"` to the `INSTALLED_APPS` in your settings file, this MUST be directly above `django.contrib.redirects`.\n\nIn `base.py` there should also be a `REDIRECT_IMPORT_DEFAULT_SITE_ID`.\n\n\n## Configuration\n\nThis application exposes the following settings:\n\n- `REDIRECT_IMPORT_DEFAULT_SITE_ID` is the default site id used when importing and creating the redirects, this is usually the same as the SITE_ID.\n ## Preparing for release\n \n In order to prep the package for a new release on TestPyPi and PyPi there is one key thing that you need to do. You need to update the version number in the `pyproject.toml`.\n This is so that the package can be published without running into version number conflicts. The version numbering must also follow the Semantic Version rules which can be found here https://semver.org/.\n \n ## Publishing\n \n Publishing a package with poetry is incredibly easy. Once you have checked that the version number has been updated (not the same as a previous version) then you only need to run two commands.\n \n    $ `poetry build` \n\nwill package the project up for you into a way that can be published.\n \n    $ `poetry publish`\n\nwill publish the package to PyPi. You will need to enter the username and password for the account which can be found in the company password manager\n',
     'author': 'Will-Hoey',
     'author_email': 'will.hoey@hotmail.co.uk',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/giantmade/giant-redirect-import',
```

### Comparing `giant_redirect_import-0.6/PKG-INFO` & `giant_redirect_import-0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: giant-redirect-import
-Version: 0.6
+Version: 0.7
 Summary: Reusable package which adds an option to bulk import redirects from a csv file
 Home-page: https://github.com/giantmade/giant-redirect-import
 License: MIT
 Keywords: import,app
 Author: Will-Hoey
 Author-email: will.hoey@hotmail.co.uk
 Requires-Python: >=3.10,<4.0
@@ -12,15 +12,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: django (>=5.0,<6.0)
+Requires-Dist: django (>=4.2,<4.3)
 Requires-Dist: django-cms (>=4.0,<5.0)
 Requires-Dist: django-import-export (>=3.2.0,<4.0.0)
 Project-URL: Repository, https://github.com/giantmade/giant-redirect-import
 Description-Content-Type: text/markdown
 
 # Giant Redirect Import
```

