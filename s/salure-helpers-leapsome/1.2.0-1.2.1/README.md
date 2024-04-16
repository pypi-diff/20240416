# Comparing `tmp/salure_helpers_leapsome-1.2.0.tar.gz` & `tmp/salure_helpers_leapsome-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/salure_helpers_leapsome-1.2.0.tar", last modified: Thu Apr  4 09:59:33 2024, max compression
+gzip compressed data, was "dist/salure_helpers_leapsome-1.2.1.tar", last modified: Tue Apr 16 09:08:53 2024, max compression
```

## Comparing `salure_helpers_leapsome-1.2.0.tar` & `salure_helpers_leapsome-1.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 09:59:33.000000 salure_helpers_leapsome-1.2.0/
--rw-r--r--   0 root         (0) root         (0)      268 2024-04-04 09:59:33.000000 salure_helpers_leapsome-1.2.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 09:59:33.000000 salure_helpers_leapsome-1.2.0/salure_helpers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 09:59:33.000000 salure_helpers_leapsome-1.2.0/salure_helpers/leapsome/
--rw-rw-rw-   0 root         (0) root         (0)      127 2024-04-04 09:59:16.000000 salure_helpers_leapsome-1.2.0/salure_helpers/leapsome/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4576 2024-04-04 09:59:16.000000 salure_helpers_leapsome-1.2.0/salure_helpers/leapsome/api_interface.py
--rw-rw-rw-   0 root         (0) root         (0)     3869 2024-04-04 09:59:16.000000 salure_helpers_leapsome-1.2.0/salure_helpers/leapsome/sftp_interface.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 09:59:33.000000 salure_helpers_leapsome-1.2.0/salure_helpers_leapsome.egg-info/
--rw-r--r--   0 root         (0) root         (0)      268 2024-04-04 09:59:33.000000 salure_helpers_leapsome-1.2.0/salure_helpers_leapsome.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      407 2024-04-04 09:59:33.000000 salure_helpers_leapsome-1.2.0/salure_helpers_leapsome.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 09:59:33.000000 salure_helpers_leapsome-1.2.0/salure_helpers_leapsome.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 09:59:33.000000 salure_helpers_leapsome-1.2.0/salure_helpers_leapsome.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       89 2024-04-04 09:59:33.000000 salure_helpers_leapsome-1.2.0/salure_helpers_leapsome.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-04-04 09:59:33.000000 salure_helpers_leapsome-1.2.0/salure_helpers_leapsome.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-04 09:59:33.000000 salure_helpers_leapsome-1.2.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      534 2024-04-04 09:59:16.000000 salure_helpers_leapsome-1.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 09:08:53.000000 salure_helpers_leapsome-1.2.1/
+-rw-r--r--   0 root         (0) root         (0)      268 2024-04-16 09:08:53.000000 salure_helpers_leapsome-1.2.1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 09:08:53.000000 salure_helpers_leapsome-1.2.1/salure_helpers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 09:08:53.000000 salure_helpers_leapsome-1.2.1/salure_helpers/leapsome/
+-rw-rw-rw-   0 root         (0) root         (0)      127 2024-04-16 09:08:34.000000 salure_helpers_leapsome-1.2.1/salure_helpers/leapsome/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4607 2024-04-16 09:08:34.000000 salure_helpers_leapsome-1.2.1/salure_helpers/leapsome/api_interface.py
+-rw-rw-rw-   0 root         (0) root         (0)     3869 2024-04-16 09:08:34.000000 salure_helpers_leapsome-1.2.1/salure_helpers/leapsome/sftp_interface.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 09:08:53.000000 salure_helpers_leapsome-1.2.1/salure_helpers_leapsome.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      268 2024-04-16 09:08:53.000000 salure_helpers_leapsome-1.2.1/salure_helpers_leapsome.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      407 2024-04-16 09:08:53.000000 salure_helpers_leapsome-1.2.1/salure_helpers_leapsome.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 09:08:53.000000 salure_helpers_leapsome-1.2.1/salure_helpers_leapsome.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 09:08:53.000000 salure_helpers_leapsome-1.2.1/salure_helpers_leapsome.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       89 2024-04-16 09:08:53.000000 salure_helpers_leapsome-1.2.1/salure_helpers_leapsome.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-04-16 09:08:53.000000 salure_helpers_leapsome-1.2.1/salure_helpers_leapsome.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-16 09:08:53.000000 salure_helpers_leapsome-1.2.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      534 2024-04-16 09:08:34.000000 salure_helpers_leapsome-1.2.1/setup.py
```

### Comparing `salure_helpers_leapsome-1.2.0/salure_helpers/leapsome/api_interface.py` & `salure_helpers_leapsome-1.2.1/salure_helpers/leapsome/api_interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
                 break
 
         # Since the objectives are split into objectives, key results and contributors, and you can have multiple key_results per objective, we need to split them
         df_key_results = df[['id', 'keyResults']].copy()
         df_key_results = df_key_results.explode('keyResults')
         df_key_results = pd.concat([df_key_results.drop(['keyResults'], axis=1), df_key_results['keyResults'].apply(pd.Series)], axis=1)
         metric_expanded = df_key_results['metric'].apply(pd.Series)
-        df_key_results = df_key_results.join(metric_expanded)
+        df_key_results = df_key_results.join(metric_expanded, how='left', rsuffix='_metric')
         df_key_results = df_key_results.drop(columns=['metric'])
 
         # Same goes for contributors
         df_contributors = df[['id', 'contributors']].copy()
         df_contributors = df_contributors.explode('contributors')
         df_contributors = pd.concat([df_contributors.drop(['contributors'], axis=1), df_contributors['contributors'].apply(pd.Series)], axis=1)
         df_contributors.columns.values[1] = 'user_id'
```

### Comparing `salure_helpers_leapsome-1.2.0/salure_helpers/leapsome/sftp_interface.py` & `salure_helpers_leapsome-1.2.1/salure_helpers/leapsome/sftp_interface.py`

 * *Files identical despite different names*

### Comparing `salure_helpers_leapsome-1.2.0/setup.py` & `salure_helpers_leapsome-1.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='salure_helpers_leapsome',
-    version='1.2.0',
+    version='1.2.1',
     description='Leapsome wrapper from Salure',
     long_description='Leapsome wrapper from Salure',
     author='D&A Salure',
     author_email='support@salureconnnect.com',
     packages=["salure_helpers.leapsome"],
     license='Salure License',
     install_requires=[
```

