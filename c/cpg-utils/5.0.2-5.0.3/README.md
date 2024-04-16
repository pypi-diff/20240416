# Comparing `tmp/cpg-utils-5.0.2.tar.gz` & `tmp/cpg-utils-5.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpg-utils-5.0.2.tar", last modified: Mon Apr 15 21:48:02 2024, max compression
+gzip compressed data, was "cpg-utils-5.0.3.tar", last modified: Tue Apr 16 02:32:25 2024, max compression
```

## Comparing `cpg-utils-5.0.2.tar` & `cpg-utils-5.0.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:48:02.262892 cpg-utils-5.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-15 21:47:59.000000 cpg-utils-5.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-15 21:48:02.262892 cpg-utils-5.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-15 21:47:59.000000 cpg-utils-5.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:48:02.262892 cpg-utils-5.0.2/cpg_utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-15 21:47:59.000000 cpg-utils-5.0.2/cpg_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14297 2024-04-15 21:47:59.000000 cpg-utils-5.0.2/cpg_utils/cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-04-15 21:47:59.000000 cpg-utils-5.0.2/cpg_utils/cloudpath_hail_az.py
--rw-r--r--   0 runner    (1001) docker     (127)    16312 2024-04-15 21:47:59.000000 cpg-utils-5.0.2/cpg_utils/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-15 21:47:59.000000 cpg-utils-5.0.2/cpg_utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    26173 2024-04-15 21:47:59.000000 cpg-utils-5.0.2/cpg_utils/cromwell.py
--rw-r--r--   0 runner    (1001) docker     (127)    13229 2024-04-15 21:47:59.000000 cpg-utils-5.0.2/cpg_utils/cromwell_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    13980 2024-04-15 21:47:59.000000 cpg-utils-5.0.2/cpg_utils/dataproc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8362 2024-04-15 21:47:59.000000 cpg-utils-5.0.2/cpg_utils/git.py
--rw-r--r--   0 runner    (1001) docker     (127)    25920 2024-04-15 21:47:59.000000 cpg-utils-5.0.2/cpg_utils/hail_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-15 21:47:59.000000 cpg-utils-5.0.2/cpg_utils/membership.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 21:47:59.000000 cpg-utils-5.0.2/cpg_utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-04-15 21:47:59.000000 cpg-utils-5.0.2/cpg_utils/slack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:48:02.262892 cpg-utils-5.0.2/cpg_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-15 21:48:02.000000 cpg-utils-5.0.2/cpg_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-15 21:48:02.000000 cpg-utils-5.0.2/cpg_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 21:48:02.000000 cpg-utils-5.0.2/cpg_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-15 21:48:02.000000 cpg-utils-5.0.2/cpg_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-15 21:48:02.000000 cpg-utils-5.0.2/cpg_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-04-15 21:47:59.000000 cpg-utils-5.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 21:48:02.262892 cpg-utils-5.0.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1348 2024-04-15 21:47:59.000000 cpg-utils-5.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:48:02.262892 cpg-utils-5.0.2/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 21:47:59.000000 cpg-utils-5.0.2/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5766 2024-04-15 21:47:59.000000 cpg-utils-5.0.2/test/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-04-15 21:47:59.000000 cpg-utils-5.0.2/test/test_cromwell.py
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-15 21:47:59.000000 cpg-utils-5.0.2/test/test_doctests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:32:25.322719 cpg-utils-5.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-16 02:32:22.000000 cpg-utils-5.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-16 02:32:25.322719 cpg-utils-5.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-16 02:32:22.000000 cpg-utils-5.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:32:25.322719 cpg-utils-5.0.3/cpg_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-16 02:32:22.000000 cpg-utils-5.0.3/cpg_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14297 2024-04-16 02:32:22.000000 cpg-utils-5.0.3/cpg_utils/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-04-16 02:32:22.000000 cpg-utils-5.0.3/cpg_utils/cloudpath_hail_az.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16312 2024-04-16 02:32:22.000000 cpg-utils-5.0.3/cpg_utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-16 02:32:22.000000 cpg-utils-5.0.3/cpg_utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26173 2024-04-16 02:32:22.000000 cpg-utils-5.0.3/cpg_utils/cromwell.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13229 2024-04-16 02:32:22.000000 cpg-utils-5.0.3/cpg_utils/cromwell_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14012 2024-04-16 02:32:22.000000 cpg-utils-5.0.3/cpg_utils/dataproc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8362 2024-04-16 02:32:22.000000 cpg-utils-5.0.3/cpg_utils/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25920 2024-04-16 02:32:22.000000 cpg-utils-5.0.3/cpg_utils/hail_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-16 02:32:22.000000 cpg-utils-5.0.3/cpg_utils/membership.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 02:32:22.000000 cpg-utils-5.0.3/cpg_utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-04-16 02:32:22.000000 cpg-utils-5.0.3/cpg_utils/slack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:32:25.322719 cpg-utils-5.0.3/cpg_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-16 02:32:25.000000 cpg-utils-5.0.3/cpg_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-16 02:32:25.000000 cpg-utils-5.0.3/cpg_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 02:32:25.000000 cpg-utils-5.0.3/cpg_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-16 02:32:25.000000 cpg-utils-5.0.3/cpg_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-16 02:32:25.000000 cpg-utils-5.0.3/cpg_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-04-16 02:32:22.000000 cpg-utils-5.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 02:32:25.322719 cpg-utils-5.0.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1348 2024-04-16 02:32:22.000000 cpg-utils-5.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:32:25.322719 cpg-utils-5.0.3/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 02:32:22.000000 cpg-utils-5.0.3/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5766 2024-04-16 02:32:22.000000 cpg-utils-5.0.3/test/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-04-16 02:32:22.000000 cpg-utils-5.0.3/test/test_cromwell.py
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-16 02:32:22.000000 cpg-utils-5.0.3/test/test_doctests.py
```

### Comparing `cpg-utils-5.0.2/LICENSE` & `cpg-utils-5.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.2/PKG-INFO` & `cpg-utils-5.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpg-utils
-Version: 5.0.2
+Version: 5.0.3
 Summary: Library of convenience functions specific to the CPG
 Home-page: https://github.com/populationgenomics/cpg-utils
 License: MIT
 Keywords: bioinformatics
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cpg-utils-5.0.2/README.md` & `cpg-utils-5.0.3/README.md`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.2/cpg_utils/__init__.py` & `cpg-utils-5.0.3/cpg_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.2/cpg_utils/cloud.py` & `cpg-utils-5.0.3/cpg_utils/cloud.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.2/cpg_utils/cloudpath_hail_az.py` & `cpg-utils-5.0.3/cpg_utils/cloudpath_hail_az.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.2/cpg_utils/config.py` & `cpg-utils-5.0.3/cpg_utils/config.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.2/cpg_utils/constants.py` & `cpg-utils-5.0.3/cpg_utils/constants.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.2/cpg_utils/cromwell.py` & `cpg-utils-5.0.3/cpg_utils/cromwell.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.2/cpg_utils/cromwell_model.py` & `cpg-utils-5.0.3/cpg_utils/cromwell_model.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.2/cpg_utils/dataproc.py` & `cpg-utils-5.0.3/cpg_utils/dataproc.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from shlex import quote
 from typing import Any, Collection
 
 import hailtop.batch as hb
 
 from cpg_utils.config import (
     AR_GUID_NAME,
-    dataset_path,
+    config_retrieve,
     get_access_level,
     get_gcloud_set_project,
     get_gcp_project,
     try_get_ar_guid,
 )
 from cpg_utils.constants import GCLOUD_ACTIVATE_AUTH
 from cpg_utils.git import (
@@ -277,15 +277,15 @@
     # The spark-env property can be used to set environment variables in jobs that run
     # on the Dataproc cluster. We propagate some currently set environment variables
     # this way.
     spark_env = [f'spark-env:CPG_CONFIG_PATH={os.getenv("CPG_CONFIG_PATH")}']
 
     # Note that the options and their values must be separated by an equal sign.
     # Using a space will break some options like --label
-    tmp_bucket = dataset_path('', 'tmp').split('://')[1]
+    tmp_bucket = config_retrieve(['storage', 'default', 'tmp']).removeprefix('gs://')
     start_job_command = [
         'hailctl dataproc start',
         f'--region={region}',
         f'--service-account={dataproc_sa}',
         f'--max-age={max_age}',
         f'--num-workers={num_workers}',
         f'--num-secondary-workers={num_secondary_workers}',
```

### Comparing `cpg-utils-5.0.2/cpg_utils/git.py` & `cpg-utils-5.0.3/cpg_utils/git.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.2/cpg_utils/hail_batch.py` & `cpg-utils-5.0.3/cpg_utils/hail_batch.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.2/cpg_utils/membership.py` & `cpg-utils-5.0.3/cpg_utils/membership.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.2/cpg_utils/slack.py` & `cpg-utils-5.0.3/cpg_utils/slack.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.2/cpg_utils.egg-info/PKG-INFO` & `cpg-utils-5.0.3/cpg_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpg-utils
-Version: 5.0.2
+Version: 5.0.3
 Summary: Library of convenience functions specific to the CPG
 Home-page: https://github.com/populationgenomics/cpg-utils
 License: MIT
 Keywords: bioinformatics
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cpg-utils-5.0.2/cpg_utils.egg-info/SOURCES.txt` & `cpg-utils-5.0.3/cpg_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.2/pyproject.toml` & `cpg-utils-5.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.2/setup.py` & `cpg-utils-5.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 with open('README.md') as f:
     long_description = f.read()
 
 setup(
     name='cpg-utils',
     # This tag is automatically updated by bumpversion
-    version='5.0.2',
+    version='5.0.3',
     description='Library of convenience functions specific to the CPG',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/populationgenomics/cpg-utils',
     license='MIT',
     packages=find_packages(),
     package_data={
```

### Comparing `cpg-utils-5.0.2/test/test_config.py` & `cpg-utils-5.0.3/test/test_config.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.2/test/test_cromwell.py` & `cpg-utils-5.0.3/test/test_cromwell.py`

 * *Files identical despite different names*

