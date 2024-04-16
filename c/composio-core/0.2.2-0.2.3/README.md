# Comparing `tmp/composio_core-0.2.2.tar.gz` & `tmp/composio_core-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_core-0.2.2.tar", last modified: Tue Apr 16 12:27:02 2024, max compression
+gzip compressed data, was "composio_core-0.2.3.tar", last modified: Tue Apr 16 12:47:24 2024, max compression
```

## Comparing `composio_core-0.2.2.tar` & `composio_core-0.2.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-16 12:27:02.935875 composio_core-0.2.2/
--rw-r--r--   0 utkarsh    (501) staff       (20)       48 2024-03-15 13:37:31.000000 composio_core-0.2.2/MANIFEST.in
--rw-r--r--   0 utkarsh    (501) staff       (20)      796 2024-04-16 12:27:02.935673 composio_core-0.2.2/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)      102 2024-03-16 10:06:01.000000 composio_core-0.2.2/README.md
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-16 12:27:02.932740 composio_core-0.2.2/composio/
--rw-r--r--   0 utkarsh    (501) staff       (20)      159 2024-04-12 09:34:06.000000 composio_core-0.2.2/composio/__init__.py
--rwxr-xr-x   0 utkarsh    (501) staff       (20)    22056 2024-04-15 14:10:00.000000 composio_core-0.2.2/composio/composio_cli.py
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-16 12:27:02.934088 composio_core-0.2.2/composio/sdk/
--rw-r--r--   0 utkarsh    (501) staff       (20)       85 2024-03-27 14:52:24.000000 composio_core-0.2.2/composio/sdk/__init__.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     6837 2024-04-15 14:05:59.000000 composio_core-0.2.2/composio/sdk/core.py
--rw-r--r--   0 utkarsh    (501) staff       (20)    10226 2024-04-12 13:08:03.000000 composio_core-0.2.2/composio/sdk/enums.py
--rw-r--r--   0 utkarsh    (501) staff       (20)    19264 2024-04-15 14:02:12.000000 composio_core-0.2.2/composio/sdk/sdk.py
--rw-r--r--   0 utkarsh    (501) staff       (20)        0 2024-04-12 13:36:37.000000 composio_core-0.2.2/composio/sdk/shared.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     1358 2024-04-15 14:06:14.000000 composio_core-0.2.2/composio/sdk/storage.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     3328 2024-04-12 09:33:50.000000 composio_core-0.2.2/composio/sdk/utils.py
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-16 12:27:02.935183 composio_core-0.2.2/composio_core.egg-info/
--rw-r--r--   0 utkarsh    (501) staff       (20)      796 2024-04-16 12:27:02.000000 composio_core-0.2.2/composio_core.egg-info/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)      489 2024-04-16 12:27:02.000000 composio_core-0.2.2/composio_core.egg-info/SOURCES.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-04-16 12:27:02.000000 composio_core-0.2.2/composio_core.egg-info/dependency_links.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       60 2024-04-16 12:27:02.000000 composio_core-0.2.2/composio_core.egg-info/entry_points.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)      103 2024-04-16 12:27:02.000000 composio_core-0.2.2/composio_core.egg-info/requires.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)        9 2024-04-16 12:27:02.000000 composio_core-0.2.2/composio_core.egg-info/top_level.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)      528 2024-04-12 15:10:44.000000 composio_core-0.2.2/pyproject.toml
--rw-r--r--   0 utkarsh    (501) staff       (20)      130 2024-04-12 15:11:16.000000 composio_core-0.2.2/requirements.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-04-16 12:27:02.935920 composio_core-0.2.2/setup.cfg
--rw-r--r--   0 utkarsh    (501) staff       (20)     1127 2024-04-16 12:26:54.000000 composio_core-0.2.2/setup.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-16 12:47:24.882840 composio_core-0.2.3/
+-rw-r--r--   0 utkarsh    (501) staff       (20)       48 2024-03-15 13:37:31.000000 composio_core-0.2.3/MANIFEST.in
+-rw-r--r--   0 utkarsh    (501) staff       (20)      796 2024-04-16 12:47:24.882600 composio_core-0.2.3/PKG-INFO
+-rw-r--r--   0 utkarsh    (501) staff       (20)      102 2024-03-16 10:06:01.000000 composio_core-0.2.3/README.md
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-16 12:47:24.879231 composio_core-0.2.3/composio/
+-rw-r--r--   0 utkarsh    (501) staff       (20)      159 2024-04-12 09:34:06.000000 composio_core-0.2.3/composio/__init__.py
+-rwxr-xr-x   0 utkarsh    (501) staff       (20)    22056 2024-04-15 14:10:00.000000 composio_core-0.2.3/composio/composio_cli.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-16 12:47:24.880874 composio_core-0.2.3/composio/sdk/
+-rw-r--r--   0 utkarsh    (501) staff       (20)       85 2024-03-27 14:52:24.000000 composio_core-0.2.3/composio/sdk/__init__.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     6837 2024-04-15 14:05:59.000000 composio_core-0.2.3/composio/sdk/core.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)    10226 2024-04-12 13:08:03.000000 composio_core-0.2.3/composio/sdk/enums.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)    19268 2024-04-16 12:44:55.000000 composio_core-0.2.3/composio/sdk/sdk.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)        0 2024-04-12 13:36:37.000000 composio_core-0.2.3/composio/sdk/shared.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     1358 2024-04-15 14:06:14.000000 composio_core-0.2.3/composio/sdk/storage.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     3328 2024-04-12 09:33:50.000000 composio_core-0.2.3/composio/sdk/utils.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-16 12:47:24.882291 composio_core-0.2.3/composio_core.egg-info/
+-rw-r--r--   0 utkarsh    (501) staff       (20)      796 2024-04-16 12:47:24.000000 composio_core-0.2.3/composio_core.egg-info/PKG-INFO
+-rw-r--r--   0 utkarsh    (501) staff       (20)      489 2024-04-16 12:47:24.000000 composio_core-0.2.3/composio_core.egg-info/SOURCES.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-04-16 12:47:24.000000 composio_core-0.2.3/composio_core.egg-info/dependency_links.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       60 2024-04-16 12:47:24.000000 composio_core-0.2.3/composio_core.egg-info/entry_points.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)      103 2024-04-16 12:47:24.000000 composio_core-0.2.3/composio_core.egg-info/requires.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)        9 2024-04-16 12:47:24.000000 composio_core-0.2.3/composio_core.egg-info/top_level.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)      528 2024-04-12 15:10:44.000000 composio_core-0.2.3/pyproject.toml
+-rw-r--r--   0 utkarsh    (501) staff       (20)      130 2024-04-12 15:11:16.000000 composio_core-0.2.3/requirements.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-04-16 12:47:24.882882 composio_core-0.2.3/setup.cfg
+-rw-r--r--   0 utkarsh    (501) staff       (20)     1127 2024-04-16 12:46:46.000000 composio_core-0.2.3/setup.py
```

### Comparing `composio_core-0.2.2/PKG-INFO` & `composio_core-0.2.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composio_core
-Version: 0.2.2
+Version: 0.2.3
 Summary: Core package to act as a bridge between composio platform and other services.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Utkarsh
 Author-email: utkarsh@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `composio_core-0.2.2/composio/composio_cli.py` & `composio_core-0.2.3/composio/composio_cli.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.2.2/composio/sdk/core.py` & `composio_core-0.2.3/composio/sdk/core.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.2.2/composio/sdk/enums.py` & `composio_core-0.2.3/composio/sdk/enums.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.2.2/composio/sdk/sdk.py` & `composio_core-0.2.3/composio/sdk/sdk.py`

 * *Files 0% similar despite different names*

```diff
@@ -413,15 +413,15 @@
         return actions
 
     def get_connection(self, app_name: Union[str, App]) -> ConnectedAccount:
         if isinstance(app_name, App):
             app_name = app_name.value
         connected_accounts = self.client.get_connected_accounts(
             entity_id=self.entity_id,
-            status="ACTIVE"
+            showActiveOnly=True
         )
         for account in connected_accounts:
             if app_name == account.appUniqueId:
                 return account
             
     def is_app_authenticated(self, app_name: Union[str, App]) -> bool:
         connected_account = self.get_connection(app_name)
```

### Comparing `composio_core-0.2.2/composio/sdk/storage.py` & `composio_core-0.2.3/composio/sdk/storage.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.2.2/composio/sdk/utils.py` & `composio_core-0.2.3/composio/sdk/utils.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.2.2/composio_core.egg-info/PKG-INFO` & `composio_core-0.2.3/composio_core.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composio_core
-Version: 0.2.2
+Version: 0.2.3
 Summary: Core package to act as a bridge between composio platform and other services.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Utkarsh
 Author-email: utkarsh@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `composio_core-0.2.2/pyproject.toml` & `composio_core-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `composio_core-0.2.2/setup.py` & `composio_core-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     """Customized setuptools install command."""
 
     def run(self):
         install.run(self)
 
 setup(
     name="composio_core",
-    version="0.2.2",
+    version="0.2.3",
     author="Utkarsh",
     author_email="utkarsh@composio.dev",
     description="Core package to act as a bridge between composio platform and other services.",
     long_description=open(readme_path).read(),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
```

