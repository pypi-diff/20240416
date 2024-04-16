# Comparing `tmp/django-marina-23.7.tar.gz` & `tmp/django_marina-24.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-marina-23.7.tar", last modified: Thu Dec 28 11:52:44 2023, max compression
+gzip compressed data, was "django_marina-24.1.tar", last modified: Tue Apr 16 08:15:22 2024, max compression
```

## Comparing `django-marina-23.7.tar` & `django_marina-24.1.tar`

### file list

```diff
@@ -1,60 +1,32 @@
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-12-28 11:52:44.757532 django-marina-23.7/
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-12-28 11:52:44.751860 django-marina-23.7/.github/
--rw-r--r--   0 dylan      (501) staff       (20)      441 2021-04-09 08:41:59.000000 django-marina-23.7/.github/dependabot.yml
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-12-28 11:52:44.752331 django-marina-23.7/.github/workflows/
--rw-r--r--   0 dylan      (501) staff       (20)     1659 2023-10-10 07:07:24.000000 django-marina-23.7/.github/workflows/dependabot-auto-approve-and-merge.yml
--rw-r--r--   0 dylan      (501) staff       (20)     2867 2023-12-28 11:21:16.000000 django-marina-23.7/.github/workflows/test.yml
--rw-r--r--   0 dylan      (501) staff       (20)      113 2023-06-29 08:22:59.000000 django-marina-23.7/.gitignore
--rw-r--r--   0 dylan      (501) staff       (20)      206 2023-12-28 11:21:16.000000 django-marina-23.7/.readthedocs.yml
--rw-r--r--   0 dylan      (501) staff       (20)     3856 2023-12-28 11:52:39.000000 django-marina-23.7/CHANGELOG.md
--rw-r--r--   0 dylan      (501) staff       (20)     2320 2023-12-28 11:21:16.000000 django-marina-23.7/CONTRIBUTING.md
--rw-r--r--   0 dylan      (501) staff       (20)     1456 2019-04-27 05:10:10.000000 django-marina-23.7/LICENSE
--rw-r--r--   0 dylan      (501) staff       (20)     1090 2023-12-28 11:49:29.000000 django-marina-23.7/Makefile
--rw-r--r--   0 dylan      (501) staff       (20)     3725 2023-12-28 11:52:44.757310 django-marina-23.7/PKG-INFO
--rw-r--r--   0 dylan      (501) staff       (20)      725 2023-12-11 13:14:05.000000 django-marina-23.7/README.md
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-12-28 11:52:44.753545 django-marina-23.7/docs/
--rw-r--r--   0 dylan      (501) staff       (20)       30 2023-05-03 15:11:58.000000 django-marina-23.7/docs/changelog.rst
--rw-r--r--   0 dylan      (501) staff       (20)      566 2023-12-28 11:21:16.000000 django-marina-23.7/docs/conf.py
--rw-r--r--   0 dylan      (501) staff       (20)       34 2023-06-29 08:22:59.000000 django-marina-23.7/docs/contributing.rst
--rw-r--r--   0 dylan      (501) staff       (20)      217 2023-05-03 15:11:58.000000 django-marina-23.7/docs/db.rst
--rw-r--r--   0 dylan      (501) staff       (20)      169 2023-06-29 08:22:59.000000 django-marina-23.7/docs/index.rst
--rw-r--r--   0 dylan      (501) staff       (20)       55 2023-12-28 11:21:16.000000 django-marina-23.7/docs/requirements.txt
--rw-r--r--   0 dylan      (501) staff       (20)      220 2023-11-10 07:36:38.000000 django-marina-23.7/docs/test.rst
--rwxr-xr-x   0 dylan      (501) staff       (20)      252 2021-04-09 08:10:13.000000 django-marina-23.7/manage.py
--rw-r--r--   0 dylan      (501) staff       (20)     2579 2023-12-28 11:52:39.000000 django-marina-23.7/pyproject.toml
--rw-r--r--   0 dylan      (501) staff       (20)      117 2023-12-28 11:49:29.000000 django-marina-23.7/requirements-dev.txt
--rw-r--r--   0 dylan      (501) staff       (20)       40 2023-12-28 11:49:29.000000 django-marina-23.7/requirements-test.txt
--rw-r--r--   0 dylan      (501) staff       (20)       38 2023-12-28 11:52:44.757571 django-marina-23.7/setup.cfg
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-12-28 11:52:44.749132 django-marina-23.7/src/
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-12-28 11:52:44.753810 django-marina-23.7/src/django_marina/
--rw-r--r--   0 dylan      (501) staff       (20)       93 2023-12-24 09:31:31.000000 django-marina-23.7/src/django_marina/__about__.py
--rw-r--r--   0 dylan      (501) staff       (20)       69 2023-06-29 08:22:59.000000 django-marina-23.7/src/django_marina/__init__.py
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-12-28 11:52:44.754871 django-marina-23.7/src/django_marina/db/
--rw-r--r--   0 dylan      (501) staff       (20)      138 2020-06-15 08:02:46.000000 django-marina-23.7/src/django_marina/db/__init__.py
--rw-r--r--   0 dylan      (501) staff       (20)      709 2023-06-29 08:22:59.000000 django-marina-23.7/src/django_marina/db/migrations.py
--rw-r--r--   0 dylan      (501) staff       (20)     1998 2023-04-23 07:42:51.000000 django-marina-23.7/src/django_marina/db/models.py
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-12-28 11:52:44.755278 django-marina-23.7/src/django_marina/test/
--rw-r--r--   0 dylan      (501) staff       (20)      127 2021-12-04 17:34:31.000000 django-marina-23.7/src/django_marina/test/__init__.py
--rw-r--r--   0 dylan      (501) staff       (20)     1908 2021-07-01 04:27:53.000000 django-marina-23.7/src/django_marina/test/clients.py
--rw-r--r--   0 dylan      (501) staff       (20)     9271 2023-12-28 11:20:00.000000 django-marina-23.7/src/django_marina/test/test_cases.py
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-12-28 11:52:44.757007 django-marina-23.7/src/django_marina.egg-info/
--rw-r--r--   0 dylan      (501) staff       (20)     3725 2023-12-28 11:52:44.000000 django-marina-23.7/src/django_marina.egg-info/PKG-INFO
--rw-r--r--   0 dylan      (501) staff       (20)     1105 2023-12-28 11:52:44.000000 django-marina-23.7/src/django_marina.egg-info/SOURCES.txt
--rw-r--r--   0 dylan      (501) staff       (20)        1 2023-12-28 11:52:44.000000 django-marina-23.7/src/django_marina.egg-info/dependency_links.txt
--rw-r--r--   0 dylan      (501) staff       (20)       34 2023-12-28 11:52:44.000000 django-marina-23.7/src/django_marina.egg-info/requires.txt
--rw-r--r--   0 dylan      (501) staff       (20)       14 2023-12-28 11:52:44.000000 django-marina-23.7/src/django_marina.egg-info/top_level.txt
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-12-28 11:52:44.756399 django-marina-23.7/tests/
--rw-r--r--   0 dylan      (501) staff       (20)        0 2020-06-11 08:49:17.000000 django-marina-23.7/tests/__init__.py
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-12-28 11:52:44.756845 django-marina-23.7/tests/app/
--rw-r--r--   0 dylan      (501) staff       (20)        0 2020-06-13 09:16:54.000000 django-marina-23.7/tests/app/__init__.py
--rw-r--r--   0 dylan      (501) staff       (20)     1525 2021-04-28 07:14:00.000000 django-marina-23.7/tests/app/settings.py
--rw-r--r--   0 dylan      (501) staff       (20)      616 2021-04-28 07:14:00.000000 django-marina-23.7/tests/app/urls.py
--rw-r--r--   0 dylan      (501) staff       (20)     1832 2021-04-28 07:14:00.000000 django-marina-23.7/tests/app/views.py
--rw-r--r--   0 dylan      (501) staff       (20)      617 2023-04-23 07:22:32.000000 django-marina-23.7/tests/models.py
--rw-r--r--   0 dylan      (501) staff       (20)     1995 2023-04-23 07:22:32.000000 django-marina-23.7/tests/test_db.py
--rw-r--r--   0 dylan      (501) staff       (20)      694 2023-04-23 07:22:32.000000 django-marina-23.7/tests/test_extended_client.py
--rw-r--r--   0 dylan      (501) staff       (20)     8518 2023-12-28 11:20:00.000000 django-marina-23.7/tests/test_extended_test_case.py
--rw-r--r--   0 dylan      (501) staff       (20)      547 2020-06-15 08:02:46.000000 django-marina-23.7/tests/test_imports.py
--rw-r--r--   0 dylan      (501) staff       (20)      308 2023-06-29 08:22:59.000000 django-marina-23.7/tests/test_version.py
--rw-r--r--   0 dylan      (501) staff       (20)      768 2019-06-10 07:50:32.000000 django-marina-23.7/tests/urls.py
--rw-r--r--   0 dylan      (501) staff       (20)      983 2023-12-28 11:21:16.000000 django-marina-23.7/tox.ini
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-04-16 08:15:22.888069 django_marina-24.1/
+-rw-r--r--   0 dylan      (501) staff       (20)     1456 2019-04-27 05:10:10.000000 django_marina-24.1/LICENSE
+-rw-r--r--   0 dylan      (501) staff       (20)     3686 2024-04-16 08:15:22.887852 django_marina-24.1/PKG-INFO
+-rw-r--r--   0 dylan      (501) staff       (20)      725 2023-12-11 13:14:05.000000 django_marina-24.1/README.md
+-rw-r--r--   0 dylan      (501) staff       (20)     2526 2024-04-16 08:15:14.000000 django_marina-24.1/pyproject.toml
+-rw-r--r--   0 dylan      (501) staff       (20)       38 2024-04-16 08:15:22.888115 django_marina-24.1/setup.cfg
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-04-16 08:15:22.883818 django_marina-24.1/src/
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-04-16 08:15:22.884749 django_marina-24.1/src/django_marina/
+-rw-r--r--   0 dylan      (501) staff       (20)       93 2023-12-24 09:31:31.000000 django_marina-24.1/src/django_marina/__about__.py
+-rw-r--r--   0 dylan      (501) staff       (20)       69 2023-06-29 08:22:59.000000 django_marina-24.1/src/django_marina/__init__.py
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-04-16 08:15:22.885973 django_marina-24.1/src/django_marina/db/
+-rw-r--r--   0 dylan      (501) staff       (20)      138 2020-06-15 08:02:46.000000 django_marina-24.1/src/django_marina/db/__init__.py
+-rw-r--r--   0 dylan      (501) staff       (20)      709 2023-06-29 08:22:59.000000 django_marina-24.1/src/django_marina/db/migrations.py
+-rw-r--r--   0 dylan      (501) staff       (20)     1998 2023-04-23 07:42:51.000000 django_marina-24.1/src/django_marina/db/models.py
+-rw-r--r--   0 dylan      (501) staff       (20)      439 2024-04-16 07:24:59.000000 django_marina-24.1/src/django_marina/html.py
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-04-16 08:15:22.886359 django_marina-24.1/src/django_marina/test/
+-rw-r--r--   0 dylan      (501) staff       (20)      127 2021-12-04 17:34:31.000000 django_marina-24.1/src/django_marina/test/__init__.py
+-rw-r--r--   0 dylan      (501) staff       (20)     1908 2021-07-01 04:27:53.000000 django_marina-24.1/src/django_marina/test/clients.py
+-rw-r--r--   0 dylan      (501) staff       (20)     9930 2024-04-16 07:24:59.000000 django_marina-24.1/src/django_marina/test/test_cases.py
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-04-16 08:15:22.887646 django_marina-24.1/src/django_marina.egg-info/
+-rw-r--r--   0 dylan      (501) staff       (20)     3686 2024-04-16 08:15:22.000000 django_marina-24.1/src/django_marina.egg-info/PKG-INFO
+-rw-r--r--   0 dylan      (501) staff       (20)      671 2024-04-16 08:15:22.000000 django_marina-24.1/src/django_marina.egg-info/SOURCES.txt
+-rw-r--r--   0 dylan      (501) staff       (20)        1 2024-04-16 08:15:22.000000 django_marina-24.1/src/django_marina.egg-info/dependency_links.txt
+-rw-r--r--   0 dylan      (501) staff       (20)       34 2024-04-16 08:15:22.000000 django_marina-24.1/src/django_marina.egg-info/requires.txt
+-rw-r--r--   0 dylan      (501) staff       (20)       14 2024-04-16 08:15:22.000000 django_marina-24.1/src/django_marina.egg-info/top_level.txt
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-04-16 08:15:22.887461 django_marina-24.1/tests/
+-rw-r--r--   0 dylan      (501) staff       (20)     1995 2023-04-23 07:22:32.000000 django_marina-24.1/tests/test_db.py
+-rw-r--r--   0 dylan      (501) staff       (20)      694 2023-04-23 07:22:32.000000 django_marina-24.1/tests/test_extended_client.py
+-rw-r--r--   0 dylan      (501) staff       (20)     8854 2024-04-16 07:24:59.000000 django_marina-24.1/tests/test_extended_test_case.py
+-rw-r--r--   0 dylan      (501) staff       (20)      235 2024-04-16 07:24:59.000000 django_marina-24.1/tests/test_html.py
+-rw-r--r--   0 dylan      (501) staff       (20)      547 2020-06-15 08:02:46.000000 django_marina-24.1/tests/test_imports.py
+-rw-r--r--   0 dylan      (501) staff       (20)      308 2023-06-29 08:22:59.000000 django_marina-24.1/tests/test_version.py
```

### Comparing `django-marina-23.7/LICENSE` & `django_marina-24.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-marina-23.7/PKG-INFO` & `django_marina-24.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-marina
-Version: 23.7
+Version: 24.1
 Summary: Django extensions by Zostera
 Author-email: Dylan Verheul <dylan@dyve.net>
 License: Copyright 2019 Zostera B.V.
         
         Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
         
         1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
@@ -18,15 +18,14 @@
 Project-URL: Documentation, https://django-marina.readthedocs.io/
 Project-URL: Homepage, https://github.com/zostera/django-marina
 Project-URL: Issues, https://github.com/zostera/django-marina/issues
 Project-URL: Source, https://github.com/zostera/django-marina
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
 Classifier: Framework :: Django :: 5.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -36,15 +35,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: Django>=3.2
+Requires-Dist: Django>=4.1
 Requires-Dist: beautifulsoup4>=4.8.0
 
 # django-marina
 
 [![image](https://github.com/zostera/django-marina/workflows/CI/badge.svg?branch=main)](https://github.com/zostera/django-marina/actions?workflow=CI)
 [![Coverage Status](https://coveralls.io/repos/github/zostera/django-marina/badge.svg?branch=main)](https://coveralls.io/github/zostera/django-marina?branch=main)
 [![Latest PyPI version](https://img.shields.io/pypi/v/django-marina.svg)](https://pypi.python.org/pypi/django-marina)
```

### Comparing `django-marina-23.7/README.md` & `django_marina-24.1/README.md`

 * *Files identical despite different names*

### Comparing `django-marina-23.7/pyproject.toml` & `django_marina-24.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 [build-system]
 build-backend = "setuptools.build_meta"
-requires = ["setuptools>=64", "setuptools_scm>=8"]
+requires = ["setuptools>=64"]
 
 [project]
 authors = [
   {name = "Dylan Verheul", email = "dylan@dyve.net"},
 ]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Environment :: Web Environment",
   "Framework :: Django",
-  "Framework :: Django :: 3.2",
   "Framework :: Django :: 4.1",
   "Framework :: Django :: 4.2",
   "Framework :: Django :: 5.0",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: BSD License",
   "Operating System :: OS Independent",
   "Programming Language :: Python :: 3",
@@ -23,23 +22,23 @@
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Topic :: Software Development :: Libraries",
   "Topic :: Utilities",
 ]
 dependencies = [
-  "Django>=3.2",
+  "Django>=4.1",
   "beautifulsoup4>=4.8.0",
 ]
 description = "Django extensions by Zostera"
 license = {file = "LICENSE"}
 name = "django-marina"
 readme = "README.md"
 requires-python = ">=3.8"
-version = "23.7"
+version = "24.1"
 
 [project.urls]
 Changelog = "https://github.com/zostera/django-marina/blob/main/CHANGELOG.md"
 Documentation = "https://django-marina.readthedocs.io/"
 Homepage = "https://github.com/zostera/django-marina"
 Issues = "https://github.com/zostera/django-marina/issues"
 Source = "https://github.com/zostera/django-marina"
```

### Comparing `django-marina-23.7/src/django_marina/db/migrations.py` & `django_marina-24.1/src/django_marina/db/migrations.py`

 * *Files identical despite different names*

### Comparing `django-marina-23.7/src/django_marina/db/models.py` & `django_marina-24.1/src/django_marina/db/models.py`

 * *Files identical despite different names*

### Comparing `django-marina-23.7/src/django_marina/test/clients.py` & `django_marina-24.1/src/django_marina/test/clients.py`

 * *Files identical despite different names*

### Comparing `django-marina-23.7/src/django_marina/test/test_cases.py` & `django_marina-24.1/src/django_marina/test/test_cases.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from http import HTTPStatus
 
 from django.contrib.messages import get_messages
 from django.test import TestCase
 
+from django_marina.html import remove_attrs
+
 from .clients import ExtendedClient
 
 
 def _login_url(next):
     """Return login url that Django uses in its redirect to login."""
     from django.contrib.auth.views import redirect_to_login
 
@@ -44,15 +46,18 @@
         :param response: HttpResponse
         :param status_code: int
         :param msg_prefix: str
         """
         self.assertEqual(
             response.status_code,
             status_code,
-            _msg_prefix_add(msg_prefix, f"Invalid response code {response.status_code} (expected {status_code})."),
+            _msg_prefix_add(
+                msg_prefix,
+                f"Invalid response code {response.status_code} (expected {status_code}).",
+            ),
         )
 
     def assertResponseOk(self, response):
         """
         Assert that response has status code OK.
 
         :param response: HttpResponse
@@ -149,38 +154,55 @@
 
         # Search with string kwarg for selectors, by applying it to found tags
         if string is not None:
             results = [result for result in results if result.find(string=string)]
 
         return len(results)
 
-    def _assert_soup(self, response, soup_method, soup_args, soup_kwargs, status_code, count, msg_prefix):
+    def _assert_soup(
+        self,
+        response,
+        soup_method,
+        soup_args,
+        soup_kwargs,
+        status_code,
+        count,
+        msg_prefix,
+    ):
         """Handle assertions that use BeautifulSoup, with interface similar to assertContains and assertNotContains."""
         self.assertEqual(
             response.status_code,
             status_code,
             _msg_prefix_add(
                 msg_prefix,
                 f"Couldn't retrieve content: Response code was {response.status_code} (expected {status_code}).",
             ),
         )
 
         soup_query = f"{soup_args} {soup_kwargs}"
         num_results = self._get_soup_num_results(response, soup_method, soup_args, soup_kwargs)
 
         if count == 0:
-            self.assertEqual(num_results, 0, _msg_prefix_add(msg_prefix, f"Response should not contain {soup_query}"))
+            self.assertEqual(
+                num_results,
+                0,
+                _msg_prefix_add(msg_prefix, f"Response should not contain {soup_query}"),
+            )
         elif count is None:
-            self.assertTrue(num_results != 0, _msg_prefix_add(msg_prefix, f"Couldn't find {soup_query} in response"))
+            self.assertTrue(
+                num_results != 0,
+                _msg_prefix_add(msg_prefix, f"Couldn't find {soup_query} in response"),
+            )
         else:
             self.assertEqual(
                 num_results,
                 count,
                 _msg_prefix_add(
-                    msg_prefix, f"Found {num_results} instances of {soup_query} in response (expected {count})"
+                    msg_prefix,
+                    f"Found {num_results} instances of {soup_query} in response (expected {count})",
                 ),
             )
 
     def assertContainsTag(self, response, name=None, count=None, status_code=200, msg_prefix="", **kwargs):
         """
         Assert that tag can be found in response, using BeautifulSoup find notation.
 
@@ -238,7 +260,15 @@
             soup_method="select",
             soup_args=[selector],
             soup_kwargs=kwargs,
             status_code=status_code,
             count=0,
             msg_prefix=msg_prefix,
         )
+
+    def assertHTMLEqual(self, html1, html2, msg=None, ignore_attrs=None):
+        """
+        Assert that the strings html1 and html2 are equal, except for certain attributes to ignore.
+
+        The comparison is based on HTML semantics.
+        """
+        return super().assertHTMLEqual(remove_attrs(html1, ignore_attrs), remove_attrs(html2, ignore_attrs), msg)
```

### Comparing `django-marina-23.7/src/django_marina.egg-info/PKG-INFO` & `django_marina-24.1/src/django_marina.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-marina
-Version: 23.7
+Version: 24.1
 Summary: Django extensions by Zostera
 Author-email: Dylan Verheul <dylan@dyve.net>
 License: Copyright 2019 Zostera B.V.
         
         Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
         
         1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
@@ -18,15 +18,14 @@
 Project-URL: Documentation, https://django-marina.readthedocs.io/
 Project-URL: Homepage, https://github.com/zostera/django-marina
 Project-URL: Issues, https://github.com/zostera/django-marina/issues
 Project-URL: Source, https://github.com/zostera/django-marina
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
 Classifier: Framework :: Django :: 5.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -36,15 +35,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: Django>=3.2
+Requires-Dist: Django>=4.1
 Requires-Dist: beautifulsoup4>=4.8.0
 
 # django-marina
 
 [![image](https://github.com/zostera/django-marina/workflows/CI/badge.svg?branch=main)](https://github.com/zostera/django-marina/actions?workflow=CI)
 [![Coverage Status](https://coveralls.io/repos/github/zostera/django-marina/badge.svg?branch=main)](https://coveralls.io/github/zostera/django-marina?branch=main)
 [![Latest PyPI version](https://img.shields.io/pypi/v/django-marina.svg)](https://pypi.python.org/pypi/django-marina)
```

### Comparing `django-marina-23.7/src/django_marina.egg-info/SOURCES.txt` & `django_marina-24.1/src/django_marina.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,47 +1,23 @@
-.gitignore
-.readthedocs.yml
-CHANGELOG.md
-CONTRIBUTING.md
 LICENSE
-Makefile
 README.md
-manage.py
 pyproject.toml
-requirements-dev.txt
-requirements-test.txt
-tox.ini
-.github/dependabot.yml
-.github/workflows/dependabot-auto-approve-and-merge.yml
-.github/workflows/test.yml
-docs/changelog.rst
-docs/conf.py
-docs/contributing.rst
-docs/db.rst
-docs/index.rst
-docs/requirements.txt
-docs/test.rst
 src/django_marina/__about__.py
 src/django_marina/__init__.py
+src/django_marina/html.py
 src/django_marina.egg-info/PKG-INFO
 src/django_marina.egg-info/SOURCES.txt
 src/django_marina.egg-info/dependency_links.txt
 src/django_marina.egg-info/requires.txt
 src/django_marina.egg-info/top_level.txt
 src/django_marina/db/__init__.py
 src/django_marina/db/migrations.py
 src/django_marina/db/models.py
 src/django_marina/test/__init__.py
 src/django_marina/test/clients.py
 src/django_marina/test/test_cases.py
-tests/__init__.py
-tests/models.py
 tests/test_db.py
 tests/test_extended_client.py
 tests/test_extended_test_case.py
+tests/test_html.py
 tests/test_imports.py
-tests/test_version.py
-tests/urls.py
-tests/app/__init__.py
-tests/app/settings.py
-tests/app/urls.py
-tests/app/views.py
+tests/test_version.py
```

### Comparing `django-marina-23.7/tests/test_db.py` & `django_marina-24.1/tests/test_db.py`

 * *Files identical despite different names*

### Comparing `django-marina-23.7/tests/test_extended_client.py` & `django_marina-24.1/tests/test_extended_client.py`

 * *Files identical despite different names*

### Comparing `django-marina-23.7/tests/test_extended_test_case.py` & `django_marina-24.1/tests/test_extended_test_case.py`

 * *Files 2% similar despite different names*

```diff
@@ -173,7 +173,16 @@
         with self.assertRaises(AssertionError):
             self.assertHasMessage(response, message)
 
         response = self.client.get(url, data={"message": message})
         self.assertHasMessage(response, message)
         with self.assertRaises(AssertionError):
             self.assertHasMessage(response, partial_message)
+
+
+class HtmlTestCase(ExtendedTestCase):
+    def test_assert_html_equal(self):
+        html1 = '<span aria-foo="bar">foo-bar</span>'
+        html2 = "<span>foo-bar</span>"
+        with self.assertRaises(AssertionError):
+            self.assertHTMLEqual(html1, html2)
+        self.assertHTMLEqual(html1, html2, ignore_attrs=["aria-foo"])
```

### Comparing `django-marina-23.7/tests/test_imports.py` & `django_marina-24.1/tests/test_imports.py`

 * *Files identical despite different names*

