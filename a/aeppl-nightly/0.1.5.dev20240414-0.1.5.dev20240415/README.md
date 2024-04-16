# Comparing `tmp/aeppl_nightly-0.1.5.dev20240414.tar.gz` & `tmp/aeppl_nightly-0.1.5.dev20240415.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aeppl_nightly-0.1.5.dev20240414.tar", last modified: Sun Apr 14 00:32:00 2024, max compression
+gzip compressed data, was "aeppl_nightly-0.1.5.dev20240415.tar", last modified: Mon Apr 15 02:59:32 2024, max compression
```

## Comparing `aeppl_nightly-0.1.5.dev20240414.tar` & `aeppl_nightly-0.1.5.dev20240415.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:32:00.600783 aeppl_nightly-0.1.5.dev20240414/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-14 00:31:52.000000 aeppl_nightly-0.1.5.dev20240414/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-14 00:31:52.000000 aeppl_nightly-0.1.5.dev20240414/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-14 00:32:00.600783 aeppl_nightly-0.1.5.dev20240414/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5534 2024-04-14 00:31:52.000000 aeppl_nightly-0.1.5.dev20240414/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:32:00.600783 aeppl_nightly-0.1.5.dev20240414/aeppl/
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-14 00:31:52.000000 aeppl_nightly-0.1.5.dev20240414/aeppl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-14 00:32:00.600783 aeppl_nightly-0.1.5.dev20240414/aeppl/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5622 2024-04-14 00:31:52.000000 aeppl_nightly-0.1.5.dev20240414/aeppl/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)     8455 2024-04-14 00:31:52.000000 aeppl_nightly-0.1.5.dev20240414/aeppl/censoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-14 00:31:52.000000 aeppl_nightly-0.1.5.dev20240414/aeppl/convolutions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-04-14 00:31:52.000000 aeppl_nightly-0.1.5.dev20240414/aeppl/cumsum.py
--rw-r--r--   0 runner    (1001) docker     (127)     8667 2024-04-14 00:31:52.000000 aeppl_nightly-0.1.5.dev20240414/aeppl/dists.py
--rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-04-14 00:31:52.000000 aeppl_nightly-0.1.5.dev20240414/aeppl/joint_logprob.py
--rw-r--r--   0 runner    (1001) docker     (127)    21265 2024-04-14 00:31:52.000000 aeppl_nightly-0.1.5.dev20240414/aeppl/logprob.py
--rw-r--r--   0 runner    (1001) docker     (127)    15197 2024-04-14 00:31:52.000000 aeppl_nightly-0.1.5.dev20240414/aeppl/mixture.py
--rw-r--r--   0 runner    (1001) docker     (127)    24383 2024-04-14 00:31:52.000000 aeppl_nightly-0.1.5.dev20240414/aeppl/printing.py
--rw-r--r--   0 runner    (1001) docker     (127)    11894 2024-04-14 00:31:52.000000 aeppl_nightly-0.1.5.dev20240414/aeppl/rewriting.py
--rw-r--r--   0 runner    (1001) docker     (127)    21163 2024-04-14 00:31:52.000000 aeppl_nightly-0.1.5.dev20240414/aeppl/scan.py
--rw-r--r--   0 runner    (1001) docker     (127)     7038 2024-04-14 00:31:52.000000 aeppl_nightly-0.1.5.dev20240414/aeppl/tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)    30605 2024-04-14 00:31:52.000000 aeppl_nightly-0.1.5.dev20240414/aeppl/transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     7859 2024-04-14 00:31:52.000000 aeppl_nightly-0.1.5.dev20240414/aeppl/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:32:00.600783 aeppl_nightly-0.1.5.dev20240414/aeppl_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-14 00:32:00.000000 aeppl_nightly-0.1.5.dev20240414/aeppl_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-14 00:32:00.000000 aeppl_nightly-0.1.5.dev20240414/aeppl_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 00:32:00.000000 aeppl_nightly-0.1.5.dev20240414/aeppl_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 00:32:00.000000 aeppl_nightly-0.1.5.dev20240414/aeppl_nightly.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-14 00:32:00.000000 aeppl_nightly-0.1.5.dev20240414/aeppl_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-14 00:32:00.000000 aeppl_nightly-0.1.5.dev20240414/aeppl_nightly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-14 00:32:00.600783 aeppl_nightly-0.1.5.dev20240414/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-04-14 00:31:52.000000 aeppl_nightly-0.1.5.dev20240414/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:32:00.600783 aeppl_nightly-0.1.5.dev20240414/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-04-14 00:31:52.000000 aeppl_nightly-0.1.5.dev20240414/tests/test_abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)     5967 2024-04-14 00:31:52.000000 aeppl_nightly-0.1.5.dev20240414/tests/test_censoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-04-14 00:31:52.000000 aeppl_nightly-0.1.5.dev20240414/tests/test_composite_logprob.py
--rw-r--r--   0 runner    (1001) docker     (127)     4190 2024-04-14 00:31:52.000000 aeppl_nightly-0.1.5.dev20240414/tests/test_convolutions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-04-14 00:31:52.000000 aeppl_nightly-0.1.5.dev20240414/tests/test_cumsum.py
--rw-r--r--   0 runner    (1001) docker     (127)    25605 2024-04-14 00:31:52.000000 aeppl_nightly-0.1.5.dev20240414/tests/test_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)     9218 2024-04-14 00:31:52.000000 aeppl_nightly-0.1.5.dev20240414/tests/test_joint_logprob.py
--rw-r--r--   0 runner    (1001) docker     (127)    40106 2024-04-14 00:31:52.000000 aeppl_nightly-0.1.5.dev20240414/tests/test_logprob.py
--rw-r--r--   0 runner    (1001) docker     (127)    22582 2024-04-14 00:31:52.000000 aeppl_nightly-0.1.5.dev20240414/tests/test_mixture.py
--rw-r--r--   0 runner    (1001) docker     (127)     6965 2024-04-14 00:31:52.000000 aeppl_nightly-0.1.5.dev20240414/tests/test_printing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-14 00:31:52.000000 aeppl_nightly-0.1.5.dev20240414/tests/test_rewriting.py
--rw-r--r--   0 runner    (1001) docker     (127)    11007 2024-04-14 00:31:52.000000 aeppl_nightly-0.1.5.dev20240414/tests/test_scan.py
--rw-r--r--   0 runner    (1001) docker     (127)     8566 2024-04-14 00:31:52.000000 aeppl_nightly-0.1.5.dev20240414/tests/test_tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)    22973 2024-04-14 00:31:52.000000 aeppl_nightly-0.1.5.dev20240414/tests/test_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-04-14 00:31:52.000000 aeppl_nightly-0.1.5.dev20240414/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    70144 2024-04-14 00:31:52.000000 aeppl_nightly-0.1.5.dev20240414/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:59:32.813860 aeppl_nightly-0.1.5.dev20240415/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-15 02:59:26.000000 aeppl_nightly-0.1.5.dev20240415/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-15 02:59:26.000000 aeppl_nightly-0.1.5.dev20240415/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-15 02:59:32.813860 aeppl_nightly-0.1.5.dev20240415/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5534 2024-04-15 02:59:26.000000 aeppl_nightly-0.1.5.dev20240415/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:59:32.817860 aeppl_nightly-0.1.5.dev20240415/aeppl/
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-15 02:59:26.000000 aeppl_nightly-0.1.5.dev20240415/aeppl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-15 02:59:32.817860 aeppl_nightly-0.1.5.dev20240415/aeppl/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5622 2024-04-15 02:59:26.000000 aeppl_nightly-0.1.5.dev20240415/aeppl/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8455 2024-04-15 02:59:26.000000 aeppl_nightly-0.1.5.dev20240415/aeppl/censoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-15 02:59:26.000000 aeppl_nightly-0.1.5.dev20240415/aeppl/convolutions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-04-15 02:59:26.000000 aeppl_nightly-0.1.5.dev20240415/aeppl/cumsum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8667 2024-04-15 02:59:26.000000 aeppl_nightly-0.1.5.dev20240415/aeppl/dists.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-04-15 02:59:26.000000 aeppl_nightly-0.1.5.dev20240415/aeppl/joint_logprob.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21265 2024-04-15 02:59:26.000000 aeppl_nightly-0.1.5.dev20240415/aeppl/logprob.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15197 2024-04-15 02:59:26.000000 aeppl_nightly-0.1.5.dev20240415/aeppl/mixture.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24383 2024-04-15 02:59:26.000000 aeppl_nightly-0.1.5.dev20240415/aeppl/printing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11894 2024-04-15 02:59:26.000000 aeppl_nightly-0.1.5.dev20240415/aeppl/rewriting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21163 2024-04-15 02:59:26.000000 aeppl_nightly-0.1.5.dev20240415/aeppl/scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7038 2024-04-15 02:59:26.000000 aeppl_nightly-0.1.5.dev20240415/aeppl/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30605 2024-04-15 02:59:26.000000 aeppl_nightly-0.1.5.dev20240415/aeppl/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7859 2024-04-15 02:59:26.000000 aeppl_nightly-0.1.5.dev20240415/aeppl/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:59:32.813860 aeppl_nightly-0.1.5.dev20240415/aeppl_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-15 02:59:32.000000 aeppl_nightly-0.1.5.dev20240415/aeppl_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-15 02:59:32.000000 aeppl_nightly-0.1.5.dev20240415/aeppl_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 02:59:32.000000 aeppl_nightly-0.1.5.dev20240415/aeppl_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 02:59:32.000000 aeppl_nightly-0.1.5.dev20240415/aeppl_nightly.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-15 02:59:32.000000 aeppl_nightly-0.1.5.dev20240415/aeppl_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-15 02:59:32.000000 aeppl_nightly-0.1.5.dev20240415/aeppl_nightly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-15 02:59:32.817860 aeppl_nightly-0.1.5.dev20240415/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-04-15 02:59:26.000000 aeppl_nightly-0.1.5.dev20240415/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:59:32.813860 aeppl_nightly-0.1.5.dev20240415/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-04-15 02:59:26.000000 aeppl_nightly-0.1.5.dev20240415/tests/test_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5967 2024-04-15 02:59:26.000000 aeppl_nightly-0.1.5.dev20240415/tests/test_censoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-04-15 02:59:26.000000 aeppl_nightly-0.1.5.dev20240415/tests/test_composite_logprob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4190 2024-04-15 02:59:26.000000 aeppl_nightly-0.1.5.dev20240415/tests/test_convolutions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-04-15 02:59:26.000000 aeppl_nightly-0.1.5.dev20240415/tests/test_cumsum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25605 2024-04-15 02:59:26.000000 aeppl_nightly-0.1.5.dev20240415/tests/test_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9218 2024-04-15 02:59:26.000000 aeppl_nightly-0.1.5.dev20240415/tests/test_joint_logprob.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40106 2024-04-15 02:59:26.000000 aeppl_nightly-0.1.5.dev20240415/tests/test_logprob.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22582 2024-04-15 02:59:26.000000 aeppl_nightly-0.1.5.dev20240415/tests/test_mixture.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6965 2024-04-15 02:59:26.000000 aeppl_nightly-0.1.5.dev20240415/tests/test_printing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-15 02:59:26.000000 aeppl_nightly-0.1.5.dev20240415/tests/test_rewriting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11007 2024-04-15 02:59:26.000000 aeppl_nightly-0.1.5.dev20240415/tests/test_scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8566 2024-04-15 02:59:26.000000 aeppl_nightly-0.1.5.dev20240415/tests/test_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22973 2024-04-15 02:59:26.000000 aeppl_nightly-0.1.5.dev20240415/tests/test_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-04-15 02:59:26.000000 aeppl_nightly-0.1.5.dev20240415/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70144 2024-04-15 02:59:26.000000 aeppl_nightly-0.1.5.dev20240415/versioneer.py
```

### Comparing `aeppl_nightly-0.1.5.dev20240414/LICENSE` & `aeppl_nightly-0.1.5.dev20240415/LICENSE`

 * *Files identical despite different names*

### Comparing `aeppl_nightly-0.1.5.dev20240414/PKG-INFO` & `aeppl_nightly-0.1.5.dev20240415/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aeppl-nightly
-Version: 0.1.5.dev20240414
+Version: 0.1.5.dev20240415
 Summary: PPL tools for Aesara
 Home-page: https://github.com/aesara-devs/aeppl
 Author: aesara-devs
 Author-email: aesara.devs@gmail.com
 Keywords: aeppl,math,probability,symbolic,probabilistic programming
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `aeppl_nightly-0.1.5.dev20240414/README.md` & `aeppl_nightly-0.1.5.dev20240415/README.md`

 * *Files identical despite different names*

### Comparing `aeppl_nightly-0.1.5.dev20240414/aeppl/abstract.py` & `aeppl_nightly-0.1.5.dev20240415/aeppl/abstract.py`

 * *Files identical despite different names*

### Comparing `aeppl_nightly-0.1.5.dev20240414/aeppl/censoring.py` & `aeppl_nightly-0.1.5.dev20240415/aeppl/censoring.py`

 * *Files identical despite different names*

### Comparing `aeppl_nightly-0.1.5.dev20240414/aeppl/convolutions.py` & `aeppl_nightly-0.1.5.dev20240415/aeppl/convolutions.py`

 * *Files identical despite different names*

### Comparing `aeppl_nightly-0.1.5.dev20240414/aeppl/cumsum.py` & `aeppl_nightly-0.1.5.dev20240415/aeppl/cumsum.py`

 * *Files identical despite different names*

### Comparing `aeppl_nightly-0.1.5.dev20240414/aeppl/dists.py` & `aeppl_nightly-0.1.5.dev20240415/aeppl/dists.py`

 * *Files identical despite different names*

### Comparing `aeppl_nightly-0.1.5.dev20240414/aeppl/joint_logprob.py` & `aeppl_nightly-0.1.5.dev20240415/aeppl/joint_logprob.py`

 * *Files identical despite different names*

### Comparing `aeppl_nightly-0.1.5.dev20240414/aeppl/logprob.py` & `aeppl_nightly-0.1.5.dev20240415/aeppl/logprob.py`

 * *Files identical despite different names*

### Comparing `aeppl_nightly-0.1.5.dev20240414/aeppl/mixture.py` & `aeppl_nightly-0.1.5.dev20240415/aeppl/mixture.py`

 * *Files identical despite different names*

### Comparing `aeppl_nightly-0.1.5.dev20240414/aeppl/printing.py` & `aeppl_nightly-0.1.5.dev20240415/aeppl/printing.py`

 * *Files identical despite different names*

### Comparing `aeppl_nightly-0.1.5.dev20240414/aeppl/rewriting.py` & `aeppl_nightly-0.1.5.dev20240415/aeppl/rewriting.py`

 * *Files identical despite different names*

### Comparing `aeppl_nightly-0.1.5.dev20240414/aeppl/scan.py` & `aeppl_nightly-0.1.5.dev20240415/aeppl/scan.py`

 * *Files identical despite different names*

### Comparing `aeppl_nightly-0.1.5.dev20240414/aeppl/tensor.py` & `aeppl_nightly-0.1.5.dev20240415/aeppl/tensor.py`

 * *Files identical despite different names*

### Comparing `aeppl_nightly-0.1.5.dev20240414/aeppl/transforms.py` & `aeppl_nightly-0.1.5.dev20240415/aeppl/transforms.py`

 * *Files identical despite different names*

### Comparing `aeppl_nightly-0.1.5.dev20240414/aeppl/utils.py` & `aeppl_nightly-0.1.5.dev20240415/aeppl/utils.py`

 * *Files identical despite different names*

### Comparing `aeppl_nightly-0.1.5.dev20240414/aeppl_nightly.egg-info/PKG-INFO` & `aeppl_nightly-0.1.5.dev20240415/aeppl_nightly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aeppl-nightly
-Version: 0.1.5.dev20240414
+Version: 0.1.5.dev20240415
 Summary: PPL tools for Aesara
 Home-page: https://github.com/aesara-devs/aeppl
 Author: aesara-devs
 Author-email: aesara.devs@gmail.com
 Keywords: aeppl,math,probability,symbolic,probabilistic programming
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `aeppl_nightly-0.1.5.dev20240414/aeppl_nightly.egg-info/SOURCES.txt` & `aeppl_nightly-0.1.5.dev20240415/aeppl_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aeppl_nightly-0.1.5.dev20240414/setup.cfg` & `aeppl_nightly-0.1.5.dev20240415/setup.cfg`

 * *Files identical despite different names*

### Comparing `aeppl_nightly-0.1.5.dev20240414/setup.py` & `aeppl_nightly-0.1.5.dev20240415/setup.py`

 * *Files identical despite different names*

### Comparing `aeppl_nightly-0.1.5.dev20240414/tests/test_abstract.py` & `aeppl_nightly-0.1.5.dev20240415/tests/test_abstract.py`

 * *Files identical despite different names*

### Comparing `aeppl_nightly-0.1.5.dev20240414/tests/test_censoring.py` & `aeppl_nightly-0.1.5.dev20240415/tests/test_censoring.py`

 * *Files identical despite different names*

### Comparing `aeppl_nightly-0.1.5.dev20240414/tests/test_composite_logprob.py` & `aeppl_nightly-0.1.5.dev20240415/tests/test_composite_logprob.py`

 * *Files identical despite different names*

### Comparing `aeppl_nightly-0.1.5.dev20240414/tests/test_convolutions.py` & `aeppl_nightly-0.1.5.dev20240415/tests/test_convolutions.py`

 * *Files identical despite different names*

### Comparing `aeppl_nightly-0.1.5.dev20240414/tests/test_cumsum.py` & `aeppl_nightly-0.1.5.dev20240415/tests/test_cumsum.py`

 * *Files identical despite different names*

### Comparing `aeppl_nightly-0.1.5.dev20240414/tests/test_dist.py` & `aeppl_nightly-0.1.5.dev20240415/tests/test_dist.py`

 * *Files identical despite different names*

### Comparing `aeppl_nightly-0.1.5.dev20240414/tests/test_joint_logprob.py` & `aeppl_nightly-0.1.5.dev20240415/tests/test_joint_logprob.py`

 * *Files identical despite different names*

### Comparing `aeppl_nightly-0.1.5.dev20240414/tests/test_logprob.py` & `aeppl_nightly-0.1.5.dev20240415/tests/test_logprob.py`

 * *Files identical despite different names*

### Comparing `aeppl_nightly-0.1.5.dev20240414/tests/test_mixture.py` & `aeppl_nightly-0.1.5.dev20240415/tests/test_mixture.py`

 * *Files identical despite different names*

### Comparing `aeppl_nightly-0.1.5.dev20240414/tests/test_printing.py` & `aeppl_nightly-0.1.5.dev20240415/tests/test_printing.py`

 * *Files identical despite different names*

### Comparing `aeppl_nightly-0.1.5.dev20240414/tests/test_rewriting.py` & `aeppl_nightly-0.1.5.dev20240415/tests/test_rewriting.py`

 * *Files identical despite different names*

### Comparing `aeppl_nightly-0.1.5.dev20240414/tests/test_scan.py` & `aeppl_nightly-0.1.5.dev20240415/tests/test_scan.py`

 * *Files identical despite different names*

### Comparing `aeppl_nightly-0.1.5.dev20240414/tests/test_tensor.py` & `aeppl_nightly-0.1.5.dev20240415/tests/test_tensor.py`

 * *Files identical despite different names*

### Comparing `aeppl_nightly-0.1.5.dev20240414/tests/test_transforms.py` & `aeppl_nightly-0.1.5.dev20240415/tests/test_transforms.py`

 * *Files identical despite different names*

### Comparing `aeppl_nightly-0.1.5.dev20240414/tests/test_utils.py` & `aeppl_nightly-0.1.5.dev20240415/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `aeppl_nightly-0.1.5.dev20240414/versioneer.py` & `aeppl_nightly-0.1.5.dev20240415/versioneer.py`

 * *Files identical despite different names*

