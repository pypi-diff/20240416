# Comparing `tmp/cogflow-1.8.1.tar.gz` & `tmp/cogflow-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cogflow-1.8.1.tar", last modified: Mon Apr 15 14:01:35 2024, max compression
+gzip compressed data, was "cogflow-1.8.2.tar", last modified: Mon Apr 15 15:06:16 2024, max compression
```

## Comparing `cogflow-1.8.1.tar` & `cogflow-1.8.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 14:01:35.090990 cogflow-1.8.1/
--rw-rw-rw-   0        0        0      401 2024-04-15 14:01:35.075410 cogflow-1.8.1/PKG-INFO
--rw-rw-rw-   0        0        0     4024 2024-04-15 10:04:49.000000 cogflow-1.8.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-15 14:01:35.043374 cogflow-1.8.1/cogflow/
--rw-rw-rw-   0        0        0      757 2024-04-15 10:41:15.000000 cogflow-1.8.1/cogflow/__init__.py
--rw-rw-rw-   0        0        0     4029 2024-04-15 10:27:20.000000 cogflow-1.8.1/cogflow/dataset_plugin.py
--rw-rw-rw-   0        0        0     8959 2024-04-15 10:26:32.000000 cogflow-1.8.1/cogflow/kubeflowplugin.py
--rw-rw-rw-   0        0        0    11107 2024-04-15 10:33:52.000000 cogflow-1.8.1/cogflow/mlflowplugin.py
--rw-rw-rw-   0        0        0      714 2024-04-15 10:04:49.000000 cogflow-1.8.1/cogflow/plugin_config.py
--rw-rw-rw-   0        0        0      620 2024-04-15 10:04:49.000000 cogflow-1.8.1/cogflow/plugin_status.py
--rw-rw-rw-   0        0        0      174 2024-04-15 10:04:49.000000 cogflow-1.8.1/cogflow/pluginerrors.py
--rw-rw-rw-   0        0        0     5492 2024-04-15 10:36:36.000000 cogflow-1.8.1/cogflow/pluginmanager.py
-drwxrwxrwx   0        0        0        0 2024-04-15 14:01:35.069507 cogflow-1.8.1/cogflow.egg-info/
--rw-rw-rw-   0        0        0      401 2024-04-15 14:01:34.000000 cogflow-1.8.1/cogflow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      367 2024-04-15 14:01:34.000000 cogflow-1.8.1/cogflow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 14:01:34.000000 cogflow-1.8.1/cogflow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      214 2024-04-15 14:01:34.000000 cogflow-1.8.1/cogflow.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-15 14:01:34.000000 cogflow-1.8.1/cogflow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-15 14:01:35.090990 cogflow-1.8.1/setup.cfg
--rw-rw-rw-   0        0        0     1594 2024-04-15 14:01:29.000000 cogflow-1.8.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 15:06:16.165543 cogflow-1.8.2/
+-rw-rw-rw-   0        0        0      401 2024-04-15 15:06:16.160454 cogflow-1.8.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4024 2024-04-15 10:04:49.000000 cogflow-1.8.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-15 15:06:16.132716 cogflow-1.8.2/cogflow/
+-rw-rw-rw-   0        0        0      757 2024-04-15 10:41:15.000000 cogflow-1.8.2/cogflow/__init__.py
+-rw-rw-rw-   0        0        0     5035 2024-04-15 14:31:58.000000 cogflow-1.8.2/cogflow/dataset_plugin.py
+-rw-rw-rw-   0        0        0     8959 2024-04-15 10:26:32.000000 cogflow-1.8.2/cogflow/kubeflowplugin.py
+-rw-rw-rw-   0        0        0    11107 2024-04-15 10:33:52.000000 cogflow-1.8.2/cogflow/mlflowplugin.py
+-rw-rw-rw-   0        0        0      714 2024-04-15 10:04:49.000000 cogflow-1.8.2/cogflow/plugin_config.py
+-rw-rw-rw-   0        0        0      620 2024-04-15 10:04:49.000000 cogflow-1.8.2/cogflow/plugin_status.py
+-rw-rw-rw-   0        0        0      174 2024-04-15 10:04:49.000000 cogflow-1.8.2/cogflow/pluginerrors.py
+-rw-rw-rw-   0        0        0     5492 2024-04-15 10:36:36.000000 cogflow-1.8.2/cogflow/pluginmanager.py
+drwxrwxrwx   0        0        0        0 2024-04-15 15:06:16.157997 cogflow-1.8.2/cogflow.egg-info/
+-rw-rw-rw-   0        0        0      401 2024-04-15 15:06:15.000000 cogflow-1.8.2/cogflow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      367 2024-04-15 15:06:15.000000 cogflow-1.8.2/cogflow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 15:06:15.000000 cogflow-1.8.2/cogflow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      214 2024-04-15 15:06:15.000000 cogflow-1.8.2/cogflow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-15 15:06:15.000000 cogflow-1.8.2/cogflow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-15 15:06:16.165543 cogflow-1.8.2/setup.cfg
+-rw-rw-rw-   0        0        0     1594 2024-04-15 15:05:52.000000 cogflow-1.8.2/setup.py
```

### Comparing `cogflow-1.8.1/README.md` & `cogflow-1.8.2/README.md`

 * *Files identical despite different names*

### Comparing `cogflow-1.8.1/cogflow/__init__.py` & `cogflow-1.8.2/cogflow/__init__.py`

 * *Files identical despite different names*

### Comparing `cogflow-1.8.1/cogflow/kubeflowplugin.py` & `cogflow-1.8.2/cogflow/kubeflowplugin.py`

 * *Files identical despite different names*

### Comparing `cogflow-1.8.1/cogflow/mlflowplugin.py` & `cogflow-1.8.2/cogflow/mlflowplugin.py`

 * *Files identical despite different names*

### Comparing `cogflow-1.8.1/cogflow/plugin_config.py` & `cogflow-1.8.2/cogflow/plugin_config.py`

 * *Files identical despite different names*

### Comparing `cogflow-1.8.1/cogflow/plugin_status.py` & `cogflow-1.8.2/cogflow/plugin_status.py`

 * *Files identical despite different names*

### Comparing `cogflow-1.8.1/cogflow/pluginmanager.py` & `cogflow-1.8.2/cogflow/pluginmanager.py`

 * *Files identical despite different names*

### Comparing `cogflow-1.8.1/setup.py` & `cogflow-1.8.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 """
 
 from setuptools import setup, find_packages
 
 setup(
     name="cogflow",
-    version="1.8.1",
+    version="1.8.2",
     author="Sai_kireeti",
     author_email="sai.kireeti@hiro-microdatacenters.nl",
     description="cog modules",
     packages=find_packages(),
     install_requires=[
         "mlflow==2.10.2",
         "kfp==1.8.22",
```

