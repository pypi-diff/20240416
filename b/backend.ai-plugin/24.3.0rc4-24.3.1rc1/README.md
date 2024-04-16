# Comparing `tmp/backend.ai-plugin-24.3.0rc4.tar.gz` & `tmp/backend.ai-plugin-24.3.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backend.ai-plugin-24.3.0rc4.tar", last modified: Fri Apr  5 03:40:04 2024, max compression
+gzip compressed data, was "backend.ai-plugin-24.3.1rc1.tar", last modified: Tue Apr 16 17:08:33 2024, max compression
```

## Comparing `backend.ai-plugin-24.3.0rc4.tar` & `backend.ai-plugin-24.3.1rc1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:04.173375 backend.ai-plugin-24.3.0rc4/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-05 03:40:03.000000 backend.ai-plugin-24.3.0rc4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-05 03:40:04.173375 backend.ai-plugin-24.3.0rc4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:04.169375 backend.ai-plugin-24.3.0rc4/ai/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:04.169375 backend.ai-plugin-24.3.0rc4/ai/backend/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:04.173375 backend.ai-plugin-24.3.0rc4/ai/backend/plugin/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-05 03:40:03.000000 backend.ai-plugin-24.3.0rc4/ai/backend/plugin/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-05 03:40:03.000000 backend.ai-plugin-24.3.0rc4/ai/backend/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8202 2024-04-05 03:40:03.000000 backend.ai-plugin-24.3.0rc4/ai/backend/plugin/entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-05 03:40:03.000000 backend.ai-plugin-24.3.0rc4/ai/backend/plugin/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:04.173375 backend.ai-plugin-24.3.0rc4/backend.ai_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-05 03:40:04.000000 backend.ai-plugin-24.3.0rc4/backend.ai_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-05 03:40:04.000000 backend.ai-plugin-24.3.0rc4/backend.ai_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 03:40:04.000000 backend.ai-plugin-24.3.0rc4/backend.ai_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 03:40:04.000000 backend.ai-plugin-24.3.0rc4/backend.ai_plugin.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 03:40:03.000000 backend.ai-plugin-24.3.0rc4/backend.ai_plugin.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-05 03:40:04.000000 backend.ai-plugin-24.3.0rc4/backend.ai_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-05 03:40:03.000000 backend.ai-plugin-24.3.0rc4/backend_shim.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 03:40:04.173375 backend.ai-plugin-24.3.0rc4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-05 03:40:03.000000 backend.ai-plugin-24.3.0rc4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:08:33.763074 backend.ai-plugin-24.3.1rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-16 17:08:33.000000 backend.ai-plugin-24.3.1rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-16 17:08:33.763074 backend.ai-plugin-24.3.1rc1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:08:33.759074 backend.ai-plugin-24.3.1rc1/ai/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:08:33.759074 backend.ai-plugin-24.3.1rc1/ai/backend/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:08:33.759074 backend.ai-plugin-24.3.1rc1/ai/backend/plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-16 17:08:33.000000 backend.ai-plugin-24.3.1rc1/ai/backend/plugin/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-16 17:08:33.000000 backend.ai-plugin-24.3.1rc1/ai/backend/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8202 2024-04-16 17:08:33.000000 backend.ai-plugin-24.3.1rc1/ai/backend/plugin/entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-16 17:08:33.000000 backend.ai-plugin-24.3.1rc1/ai/backend/plugin/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:08:33.759074 backend.ai-plugin-24.3.1rc1/backend.ai_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-16 17:08:33.000000 backend.ai-plugin-24.3.1rc1/backend.ai_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-16 17:08:33.000000 backend.ai-plugin-24.3.1rc1/backend.ai_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 17:08:33.000000 backend.ai-plugin-24.3.1rc1/backend.ai_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 17:08:33.000000 backend.ai-plugin-24.3.1rc1/backend.ai_plugin.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 17:08:33.000000 backend.ai-plugin-24.3.1rc1/backend.ai_plugin.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-16 17:08:33.000000 backend.ai-plugin-24.3.1rc1/backend.ai_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-16 17:08:33.000000 backend.ai-plugin-24.3.1rc1/backend_shim.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 17:08:33.763074 backend.ai-plugin-24.3.1rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-16 17:08:33.000000 backend.ai-plugin-24.3.1rc1/setup.py
```

### Comparing `backend.ai-plugin-24.3.0rc4/PKG-INFO` & `backend.ai-plugin-24.3.1rc1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-plugin
-Version: 24.3.0rc4
+Version: 24.3.1rc1
 Summary: Backend.AI Plugin Subsystem
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: MIT
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
```

### Comparing `backend.ai-plugin-24.3.0rc4/ai/backend/plugin/entrypoint.py` & `backend.ai-plugin-24.3.1rc1/ai/backend/plugin/entrypoint.py`

 * *Files identical despite different names*

### Comparing `backend.ai-plugin-24.3.0rc4/backend.ai_plugin.egg-info/PKG-INFO` & `backend.ai-plugin-24.3.1rc1/backend.ai_plugin.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-plugin
-Version: 24.3.0rc4
+Version: 24.3.1rc1
 Summary: Backend.AI Plugin Subsystem
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: MIT
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
```

### Comparing `backend.ai-plugin-24.3.0rc4/backend_shim.py` & `backend.ai-plugin-24.3.1rc1/backend_shim.py`

 * *Files identical despite different names*

### Comparing `backend.ai-plugin-24.3.0rc4/setup.py` & `backend.ai-plugin-24.3.1rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,11 +46,11 @@
     ),
     'project_urls': {
         'Documentation': 'https://docs.backend.ai/',
         'Source': 'https://github.com/lablup/backend.ai',
     },
     'python_requires': '>=3.12,<3.13',
     'url': 'https://github.com/lablup/backend.ai',
-    'version': """24.03.0rc4
+    'version': """24.03.1rc1
 """,
     'zip_safe': False,
 })
```

