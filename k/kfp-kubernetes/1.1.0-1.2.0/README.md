# Comparing `tmp/kfp-kubernetes-1.1.0.tar.gz` & `tmp/kfp-kubernetes-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kfp-kubernetes-1.1.0.tar", last modified: Fri Jan 12 00:10:39 2024, max compression
+gzip compressed data, was "kfp-kubernetes-1.2.0.tar", last modified: Mon Apr 15 22:01:19 2024, max compression
```

## Comparing `kfp-kubernetes-1.1.0.tar` & `kfp-kubernetes-1.2.0.tar`

### file list

```diff
@@ -1,19 +1,25 @@
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2024-01-12 00:10:39.304765 kfp-kubernetes-1.1.0/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4595 2024-01-12 00:10:39.304590 kfp-kubernetes-1.1.0/PKG-INFO
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3143 2023-11-13 23:05:28.000000 kfp-kubernetes-1.1.0/README.md
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2024-01-12 00:10:39.302101 kfp-kubernetes-1.1.0/kfp/
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2024-01-12 00:10:39.303414 kfp-kubernetes-1.1.0/kfp/kubernetes/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1051 2024-01-11 23:56:46.000000 kfp-kubernetes-1.1.0/kfp/kubernetes/__init__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      987 2023-11-13 23:05:28.000000 kfp-kubernetes-1.1.0/kfp/kubernetes/common.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    10075 2024-01-12 00:09:41.000000 kfp-kubernetes-1.1.0/kfp/kubernetes/kubernetes_executor_config_pb2.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1688 2023-11-13 23:05:28.000000 kfp-kubernetes-1.1.0/kfp/kubernetes/node_selector.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2837 2023-11-13 23:05:28.000000 kfp-kubernetes-1.1.0/kfp/kubernetes/secret.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     5882 2023-11-13 23:05:28.000000 kfp-kubernetes-1.1.0/kfp/kubernetes/volume.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2024-01-12 00:10:39.304215 kfp-kubernetes-1.1.0/kfp_kubernetes.egg-info/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4595 2024-01-12 00:10:39.000000 kfp-kubernetes-1.1.0/kfp_kubernetes.egg-info/PKG-INFO
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      390 2024-01-12 00:10:39.000000 kfp-kubernetes-1.1.0/kfp_kubernetes.egg-info/SOURCES.txt
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)        1 2024-01-12 00:10:39.000000 kfp-kubernetes-1.1.0/kfp_kubernetes.egg-info/dependency_links.txt
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      161 2024-01-12 00:10:39.000000 kfp-kubernetes-1.1.0/kfp_kubernetes.egg-info/requires.txt
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)        4 2024-01-12 00:10:39.000000 kfp-kubernetes-1.1.0/kfp_kubernetes.egg-info/top_level.txt
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)       38 2024-01-12 00:10:39.304833 kfp-kubernetes-1.1.0/setup.cfg
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2512 2024-01-11 23:56:46.000000 kfp-kubernetes-1.1.0/setup.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2024-04-15 22:01:19.642701 kfp-kubernetes-1.2.0/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     9950 2024-04-15 22:01:19.642510 kfp-kubernetes-1.2.0/PKG-INFO
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7082 2024-04-11 19:20:57.000000 kfp-kubernetes-1.2.0/README.md
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2024-04-15 22:01:19.638510 kfp-kubernetes-1.2.0/kfp/
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2024-04-15 22:01:19.641453 kfp-kubernetes-1.2.0/kfp/kubernetes/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1873 2024-04-15 20:46:30.000000 kfp-kubernetes-1.2.0/kfp/kubernetes/__init__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      987 2024-03-19 01:28:32.000000 kfp-kubernetes-1.2.0/kfp/kubernetes/common.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3171 2024-04-05 15:25:04.000000 kfp-kubernetes-1.2.0/kfp/kubernetes/config_map.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1630 2024-04-05 15:24:59.000000 kfp-kubernetes-1.2.0/kfp/kubernetes/field.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2186 2024-04-05 15:24:59.000000 kfp-kubernetes-1.2.0/kfp/kubernetes/image.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    19925 2024-04-15 21:56:50.000000 kfp-kubernetes-1.2.0/kfp/kubernetes/kubernetes_executor_config_pb2.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1688 2024-03-19 01:28:32.000000 kfp-kubernetes-1.2.0/kfp/kubernetes/node_selector.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2469 2024-04-05 15:24:59.000000 kfp-kubernetes-1.2.0/kfp/kubernetes/pod_metadata.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3000 2024-04-05 15:25:04.000000 kfp-kubernetes-1.2.0/kfp/kubernetes/secret.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1748 2024-04-05 15:24:59.000000 kfp-kubernetes-1.2.0/kfp/kubernetes/timeout.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3132 2024-04-05 15:24:59.000000 kfp-kubernetes-1.2.0/kfp/kubernetes/toleration.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     8606 2024-04-11 19:20:57.000000 kfp-kubernetes-1.2.0/kfp/kubernetes/volume.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2024-04-15 22:01:19.642291 kfp-kubernetes-1.2.0/kfp_kubernetes.egg-info/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     9950 2024-04-15 22:01:19.000000 kfp-kubernetes-1.2.0/kfp_kubernetes.egg-info/PKG-INFO
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      553 2024-04-15 22:01:19.000000 kfp-kubernetes-1.2.0/kfp_kubernetes.egg-info/SOURCES.txt
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)        1 2024-04-15 22:01:19.000000 kfp-kubernetes-1.2.0/kfp_kubernetes.egg-info/dependency_links.txt
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      164 2024-04-15 22:01:19.000000 kfp-kubernetes-1.2.0/kfp_kubernetes.egg-info/requires.txt
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)        4 2024-04-15 22:01:19.000000 kfp-kubernetes-1.2.0/kfp_kubernetes.egg-info/top_level.txt
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)       38 2024-04-15 22:01:19.642748 kfp-kubernetes-1.2.0/setup.cfg
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2515 2024-04-15 20:46:30.000000 kfp-kubernetes-1.2.0/setup.py
```

### Comparing `kfp-kubernetes-1.1.0/kfp/kubernetes/common.py` & `kfp-kubernetes-1.2.0/kfp/kubernetes/common.py`

 * *Files identical despite different names*

### Comparing `kfp-kubernetes-1.1.0/kfp/kubernetes/node_selector.py` & `kfp-kubernetes-1.2.0/kfp/kubernetes/node_selector.py`

 * *Files identical despite different names*

### Comparing `kfp-kubernetes-1.1.0/kfp/kubernetes/secret.py` & `kfp-kubernetes-1.2.0/kfp/kubernetes/secret.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,17 +21,16 @@
 
 
 def use_secret_as_env(
     task: PipelineTask,
     secret_name: str,
     secret_key_to_env: Dict[str, str],
 ) -> PipelineTask:
-    """Use a Kubernetes Secret as an environment variable as described in
-    https://kubernetes.io/docs/concepts/configuration/secret/#using-secrets-as-
-    environment-variables.
+    """Use a Kubernetes Secret as an environment variable as described by the `Kubernetes documentation
+    https://kubernetes.io/docs/concepts/configuration/secret/#using-secrets-as-environment-variables `_.
 
     Args:
         task: Pipeline task.
         secret_name: Name of the Secret.
         secret_key_to_env: Dictionary of Secret data key to environment variable name. For example, ``{'password': 'PASSWORD'}`` sets the data of the Secret's password field to the environment variable ``PASSWORD``.
 
     Returns:
@@ -58,32 +57,35 @@
     return task
 
 
 def use_secret_as_volume(
     task: PipelineTask,
     secret_name: str,
     mount_path: str,
+    optional: bool = False,
 ) -> PipelineTask:
     """Use a Kubernetes Secret by mounting its data to the task's container as
     described by the `Kubernetes documentation <https://kubernetes.io/docs/concepts/configuration/secret/#using-secrets-as-files-from-a-pod>`_.
 
     Args:
         task: Pipeline task.
         secret_name: Name of the Secret.
         mount_path: Path to which to mount the Secret data.
+        optional: Optional field specifying whether the Secret must be defined.
 
     Returns:
         Task object with updated secret configuration.
     """
 
     msg = common.get_existing_kubernetes_config_as_message(task)
 
     secret_as_vol = pb.SecretAsVolume(
         secret_name=secret_name,
         mount_path=mount_path,
+        optional=optional,
     )
 
     msg.secret_as_volume.append(secret_as_vol)
 
     task.platform_config['kubernetes'] = json_format.MessageToDict(msg)
 
     return task
```

### Comparing `kfp-kubernetes-1.1.0/setup.py` & `kfp-kubernetes-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import re
 
 import setuptools
 
 NAME = 'kfp-kubernetes'
 REQUIREMENTS = [
     'protobuf>=4.21.1,<5',
-    'kfp>=2.6.0',
+    'kfp>=2.6.0,<3',
 ]
 DEV_REQUIREMENTS = [
     'docformatter==1.4',
     'isort==5.10.1',
     'mypy==0.941',
     'pre-commit==2.19.0',
     'pycln==2.1.1',
```

