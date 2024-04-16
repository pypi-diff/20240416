# Comparing `tmp/baseapp-url-shortening-0.1.1.tar.gz` & `tmp/baseapp-url-shortening-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baseapp-url-shortening-0.1.1.tar", last modified: Sun Dec 10 07:37:22 2023, max compression
+gzip compressed data, was "baseapp-url-shortening-0.1.2.tar", last modified: Tue Apr 16 18:17:51 2024, max compression
```

## Comparing `baseapp-url-shortening-0.1.1.tar` & `baseapp-url-shortening-0.1.2.tar`

### file list

```diff
@@ -1,34 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 07:37:22.710000 baseapp-url-shortening-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2023-12-10 07:37:22.710000 baseapp-url-shortening-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2023-12-10 07:37:22.000000 baseapp-url-shortening-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 07:37:22.706000 baseapp-url-shortening-0.1.1/baseapp_url_shortening/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-10 07:37:22.000000 baseapp-url-shortening-0.1.1/baseapp_url_shortening/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2023-12-10 07:37:22.000000 baseapp-url-shortening-0.1.1/baseapp_url_shortening/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      110 2023-12-10 07:37:22.000000 baseapp-url-shortening-0.1.1/baseapp_url_shortening/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 07:37:22.706000 baseapp-url-shortening-0.1.1/baseapp_url_shortening/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2023-12-10 07:37:22.000000 baseapp-url-shortening-0.1.1/baseapp_url_shortening/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-10 07:37:22.000000 baseapp-url-shortening-0.1.1/baseapp_url_shortening/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      679 2023-12-10 07:37:22.000000 baseapp-url-shortening-0.1.1/baseapp_url_shortening/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 07:37:22.706000 baseapp-url-shortening-0.1.1/baseapp_url_shortening/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-10 07:37:22.000000 baseapp-url-shortening-0.1.1/baseapp_url_shortening/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       50 2023-12-10 07:37:22.000000 baseapp-url-shortening-0.1.1/baseapp_url_shortening/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2023-12-10 07:37:22.000000 baseapp-url-shortening-0.1.1/baseapp_url_shortening/tests/factories.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 07:37:22.706000 baseapp-url-shortening-0.1.1/baseapp_url_shortening/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-10 07:37:22.000000 baseapp-url-shortening-0.1.1/baseapp_url_shortening/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      359 2023-12-10 07:37:22.000000 baseapp-url-shortening-0.1.1/baseapp_url_shortening/tests/integration/test_url_shortening.py
--rw-r--r--   0 runner    (1001) docker     (127)       50 2023-12-10 07:37:22.000000 baseapp-url-shortening-0.1.1/baseapp_url_shortening/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      529 2023-12-10 07:37:22.000000 baseapp-url-shortening-0.1.1/baseapp_url_shortening/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2023-12-10 07:37:22.000000 baseapp-url-shortening-0.1.1/baseapp_url_shortening/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 07:37:22.706000 baseapp-url-shortening-0.1.1/baseapp_url_shortening.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2023-12-10 07:37:22.000000 baseapp-url-shortening-0.1.1/baseapp_url_shortening.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      912 2023-12-10 07:37:22.000000 baseapp-url-shortening-0.1.1/baseapp_url_shortening.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-10 07:37:22.000000 baseapp-url-shortening-0.1.1/baseapp_url_shortening.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2023-12-10 07:37:22.000000 baseapp-url-shortening-0.1.1/baseapp_url_shortening.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-12-10 07:37:22.000000 baseapp-url-shortening-0.1.1/baseapp_url_shortening.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      178 2023-12-10 07:37:22.000000 baseapp-url-shortening-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      523 2023-12-10 07:37:22.710000 baseapp-url-shortening-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      276 2023-12-10 07:37:22.000000 baseapp-url-shortening-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 07:37:22.710000 baseapp-url-shortening-0.1.1/testproject/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-10 07:37:22.000000 baseapp-url-shortening-0.1.1/testproject/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      192 2023-12-10 07:37:22.000000 baseapp-url-shortening-0.1.1/testproject/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      227 2023-12-10 07:37:22.000000 baseapp-url-shortening-0.1.1/testproject/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:17:51.611351 baseapp-url-shortening-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-16 18:17:51.611351 baseapp-url-shortening-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-16 18:17:49.000000 baseapp-url-shortening-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:17:51.607351 baseapp-url-shortening-0.1.2/baseapp_url_shortening/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 18:17:49.000000 baseapp-url-shortening-0.1.2/baseapp_url_shortening/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-16 18:17:49.000000 baseapp-url-shortening-0.1.2/baseapp_url_shortening/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-16 18:17:49.000000 baseapp-url-shortening-0.1.2/baseapp_url_shortening/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:17:51.611351 baseapp-url-shortening-0.1.2/baseapp_url_shortening/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-04-16 18:17:49.000000 baseapp-url-shortening-0.1.2/baseapp_url_shortening/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-16 18:17:49.000000 baseapp-url-shortening-0.1.2/baseapp_url_shortening/migrations/0002_alter_shorturl_full_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 18:17:49.000000 baseapp-url-shortening-0.1.2/baseapp_url_shortening/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-16 18:17:49.000000 baseapp-url-shortening-0.1.2/baseapp_url_shortening/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:17:51.611351 baseapp-url-shortening-0.1.2/baseapp_url_shortening/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 18:17:49.000000 baseapp-url-shortening-0.1.2/baseapp_url_shortening/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-16 18:17:49.000000 baseapp-url-shortening-0.1.2/baseapp_url_shortening/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-16 18:17:49.000000 baseapp-url-shortening-0.1.2/baseapp_url_shortening/tests/factories.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:17:51.611351 baseapp-url-shortening-0.1.2/baseapp_url_shortening/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 18:17:49.000000 baseapp-url-shortening-0.1.2/baseapp_url_shortening/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-16 18:17:49.000000 baseapp-url-shortening-0.1.2/baseapp_url_shortening/tests/integration/test_url_shortening.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-16 18:17:49.000000 baseapp-url-shortening-0.1.2/baseapp_url_shortening/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-16 18:17:49.000000 baseapp-url-shortening-0.1.2/baseapp_url_shortening/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-16 18:17:49.000000 baseapp-url-shortening-0.1.2/baseapp_url_shortening/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-16 18:17:49.000000 baseapp-url-shortening-0.1.2/baseapp_url_shortening/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:17:51.611351 baseapp-url-shortening-0.1.2/baseapp_url_shortening.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-16 18:17:51.000000 baseapp-url-shortening-0.1.2/baseapp_url_shortening.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-16 18:17:51.000000 baseapp-url-shortening-0.1.2/baseapp_url_shortening.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 18:17:51.000000 baseapp-url-shortening-0.1.2/baseapp_url_shortening.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-16 18:17:51.000000 baseapp-url-shortening-0.1.2/baseapp_url_shortening.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-16 18:17:51.000000 baseapp-url-shortening-0.1.2/baseapp_url_shortening.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-16 18:17:49.000000 baseapp-url-shortening-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-16 18:17:51.611351 baseapp-url-shortening-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-16 18:17:49.000000 baseapp-url-shortening-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:17:51.611351 baseapp-url-shortening-0.1.2/testproject/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 18:17:49.000000 baseapp-url-shortening-0.1.2/testproject/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-16 18:17:49.000000 baseapp-url-shortening-0.1.2/testproject/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-16 18:17:49.000000 baseapp-url-shortening-0.1.2/testproject/urls.py
```

### Comparing `baseapp-url-shortening-0.1.1/README.md` & `baseapp-url-shortening-0.1.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 # BaseApp URL Shortening
 
 Reusable app to enable url shortening.
 
 ## How to install:
 
-Add dependencies to your `requirements/base.txt` file:
+Install in your environment:
 
-```
-baseapp-core @ git+https://github.com/silverlogic/baseapp-backend.git@v0.1#subdirectory=baseapp-core
-baseapp-reactions @ git+https://github.com/silverlogic/baseapp-backend.git@v0.1#subdirectory=baseapp-url-shortening
+```bash
+pip install baseapp-url-shortening
 ```
 
 And run provision or manually `pip install -r requirements/base.ext`
 
 If you want to develop, [install using this other guide](#how-to-develop).
 
 ## How to use
```

### Comparing `baseapp-url-shortening-0.1.1/baseapp_url_shortening/migrations/0001_initial.py` & `baseapp-url-shortening-0.1.2/baseapp_url_shortening/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `baseapp-url-shortening-0.1.1/baseapp_url_shortening.egg-info/SOURCES.txt` & `baseapp-url-shortening-0.1.2/baseapp_url_shortening.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -3,21 +3,23 @@
 setup.cfg
 setup.py
 baseapp_url_shortening/__init__.py
 baseapp_url_shortening/admin.py
 baseapp_url_shortening/apps.py
 baseapp_url_shortening/models.py
 baseapp_url_shortening/urls.py
+baseapp_url_shortening/utils.py
 baseapp_url_shortening/views.py
 baseapp_url_shortening.egg-info/PKG-INFO
 baseapp_url_shortening.egg-info/SOURCES.txt
 baseapp_url_shortening.egg-info/dependency_links.txt
 baseapp_url_shortening.egg-info/requires.txt
 baseapp_url_shortening.egg-info/top_level.txt
 baseapp_url_shortening/migrations/0001_initial.py
+baseapp_url_shortening/migrations/0002_alter_shorturl_full_url.py
 baseapp_url_shortening/migrations/__init__.py
 baseapp_url_shortening/tests/__init__.py
 baseapp_url_shortening/tests/conftest.py
 baseapp_url_shortening/tests/factories.py
 baseapp_url_shortening/tests/settings.py
 baseapp_url_shortening/tests/integration/__init__.py
 baseapp_url_shortening/tests/integration/test_url_shortening.py
```

### Comparing `baseapp-url-shortening-0.1.1/setup.cfg` & `baseapp-url-shortening-0.1.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = baseapp_url_shortening
-version = 0.1.1
+version = 0.1.2
 description = BaseApp URL Shortening
 long_description = file: README.md
 url = https://github.com/silverlogic/baseapp-backend
 author = The SilverLogic
 author_email = dev@tsl.io
 license = BSD-3-Clause  # Example license
```

