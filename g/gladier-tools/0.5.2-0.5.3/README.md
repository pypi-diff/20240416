# Comparing `tmp/gladier-tools-0.5.2.tar.gz` & `tmp/gladier_tools-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gladier-tools-0.5.2.tar", last modified: Sat Sep 23 01:06:46 2023, max compression
+gzip compressed data, was "gladier_tools-0.5.3.tar", last modified: Tue Apr 16 16:33:43 2024, max compression
```

## Comparing `gladier-tools-0.5.2.tar` & `gladier_tools-0.5.3.tar`

### file list

```diff
@@ -1,56 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-23 01:06:46.679680 gladier-tools-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2023-09-23 01:06:35.000000 gladier-tools-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-09-23 01:06:35.000000 gladier-tools-0.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2023-09-23 01:06:46.679680 gladier-tools-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2023-09-23 01:06:35.000000 gladier-tools-0.5.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-23 01:06:46.675680 gladier-tools-0.5.2/gladier_tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-23 01:06:35.000000 gladier-tools-0.5.2/gladier_tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-23 01:06:46.675680 gladier-tools-0.5.2/gladier_tools/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)      536 2023-09-23 01:06:35.000000 gladier-tools-0.5.2/gladier_tools/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3856 2023-09-23 01:06:35.000000 gladier-tools-0.5.2/gladier_tools/experimental/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-23 01:06:46.675680 gladier-tools-0.5.2/gladier_tools/experimental/globus/
--rw-r--r--   0 runner    (1001) docker     (127)      210 2023-09-23 01:06:35.000000 gladier-tools-0.5.2/gladier_tools/experimental/globus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2023-09-23 01:06:35.000000 gladier-tools-0.5.2/gladier_tools/experimental/globus/mkdir.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-23 01:06:46.675680 gladier-tools-0.5.2/gladier_tools/globus/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2023-09-23 01:06:35.000000 gladier-tools-0.5.2/gladier_tools/globus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2682 2023-09-23 01:06:35.000000 gladier-tools-0.5.2/gladier_tools/globus/transfer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-23 01:06:46.679680 gladier-tools-0.5.2/gladier_tools/posix/
--rw-r--r--   0 runner    (1001) docker     (127)      455 2023-09-23 01:06:35.000000 gladier-tools-0.5.2/gladier_tools/posix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2652 2023-09-23 01:06:35.000000 gladier-tools-0.5.2/gladier_tools/posix/asymmetric_decrypt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2023-09-23 01:06:35.000000 gladier-tools-0.5.2/gladier_tools/posix/asymmetric_encrypt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2453 2023-09-23 01:06:35.000000 gladier-tools-0.5.2/gladier_tools/posix/decrypt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2137 2023-09-23 01:06:35.000000 gladier-tools-0.5.2/gladier_tools/posix/encrypt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2023-09-23 01:06:35.000000 gladier-tools-0.5.2/gladier_tools/posix/https_download_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     4776 2023-09-23 01:06:35.000000 gladier-tools-0.5.2/gladier_tools/posix/shell_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2023-09-23 01:06:35.000000 gladier-tools-0.5.2/gladier_tools/posix/tar.py
--rw-r--r--   0 runner    (1001) docker     (127)     2084 2023-09-23 01:06:35.000000 gladier-tools-0.5.2/gladier_tools/posix/untar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-23 01:06:46.679680 gladier-tools-0.5.2/gladier_tools/publish/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2023-09-23 01:06:35.000000 gladier-tools-0.5.2/gladier_tools/publish/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7086 2023-09-23 01:06:35.000000 gladier-tools-0.5.2/gladier_tools/publish/publish.py
--rw-r--r--   0 runner    (1001) docker     (127)    18066 2023-09-23 01:06:35.000000 gladier-tools-0.5.2/gladier_tools/publish/publishv2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-23 01:06:46.679680 gladier-tools-0.5.2/gladier_tools/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-23 01:06:35.000000 gladier-tools-0.5.2/gladier_tools/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-23 01:06:46.679680 gladier-tools-0.5.2/gladier_tools/tests/posix/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-23 01:06:35.000000 gladier-tools-0.5.2/gladier_tools/tests/posix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2023-09-23 01:06:35.000000 gladier-tools-0.5.2/gladier_tools/tests/posix/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      438 2023-09-23 01:06:35.000000 gladier-tools-0.5.2/gladier_tools/tests/posix/mocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2023-09-23 01:06:35.000000 gladier-tools-0.5.2/gladier_tools/tests/posix/test_decrypt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2023-09-23 01:06:35.000000 gladier-tools-0.5.2/gladier_tools/tests/posix/test_encrypt.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2023-09-23 01:06:35.000000 gladier-tools-0.5.2/gladier_tools/tests/posix/test_gladier_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     3134 2023-09-23 01:06:35.000000 gladier-tools-0.5.2/gladier_tools/tests/posix/test_shell_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)      926 2023-09-23 01:06:35.000000 gladier-tools-0.5.2/gladier_tools/tests/posix/test_tar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2023-09-23 01:06:35.000000 gladier-tools-0.5.2/gladier_tools/tests/posix/test_untar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-23 01:06:46.679680 gladier-tools-0.5.2/gladier_tools/tests/publish/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-23 01:06:35.000000 gladier-tools-0.5.2/gladier_tools/tests/publish/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2023-09-23 01:06:35.000000 gladier-tools-0.5.2/gladier_tools/tests/publish/test_publish.py
--rw-r--r--   0 runner    (1001) docker     (127)    10520 2023-09-23 01:06:35.000000 gladier-tools-0.5.2/gladier_tools/tests/publish/test_publishv2.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-09-23 01:06:35.000000 gladier-tools-0.5.2/gladier_tools/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-23 01:06:46.675680 gladier-tools-0.5.2/gladier_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2023-09-23 01:06:46.000000 gladier-tools-0.5.2/gladier_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2023-09-23 01:06:46.000000 gladier-tools-0.5.2/gladier_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-23 01:06:46.000000 gladier-tools-0.5.2/gladier_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-09-23 01:06:46.000000 gladier-tools-0.5.2/gladier_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2023-09-23 01:06:46.000000 gladier-tools-0.5.2/gladier_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-09-23 01:06:35.000000 gladier-tools-0.5.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       88 2023-09-23 01:06:46.679680 gladier-tools-0.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2023-09-23 01:06:35.000000 gladier-tools-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:33:43.707886 gladier_tools-0.5.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-16 16:33:40.000000 gladier_tools-0.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-16 16:33:40.000000 gladier_tools-0.5.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-04-16 16:33:43.707886 gladier_tools-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-16 16:33:40.000000 gladier_tools-0.5.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:33:43.703886 gladier_tools-0.5.3/gladier_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 16:33:40.000000 gladier_tools-0.5.3/gladier_tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:33:43.703886 gladier_tools-0.5.3/gladier_tools/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-16 16:33:40.000000 gladier_tools-0.5.3/gladier_tools/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-04-16 16:33:40.000000 gladier_tools-0.5.3/gladier_tools/experimental/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:33:43.703886 gladier_tools-0.5.3/gladier_tools/experimental/globus/
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-16 16:33:40.000000 gladier_tools-0.5.3/gladier_tools/experimental/globus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-16 16:33:40.000000 gladier_tools-0.5.3/gladier_tools/experimental/globus/mkdir.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:33:43.703886 gladier_tools-0.5.3/gladier_tools/globus/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-16 16:33:40.000000 gladier_tools-0.5.3/gladier_tools/globus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-04-16 16:33:40.000000 gladier_tools-0.5.3/gladier_tools/globus/transfer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:33:43.703886 gladier_tools-0.5.3/gladier_tools/posix/
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-16 16:33:40.000000 gladier_tools-0.5.3/gladier_tools/posix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-04-16 16:33:40.000000 gladier_tools-0.5.3/gladier_tools/posix/asymmetric_decrypt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-04-16 16:33:40.000000 gladier_tools-0.5.3/gladier_tools/posix/asymmetric_encrypt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-04-16 16:33:40.000000 gladier_tools-0.5.3/gladier_tools/posix/decrypt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-04-16 16:33:40.000000 gladier_tools-0.5.3/gladier_tools/posix/encrypt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-16 16:33:40.000000 gladier_tools-0.5.3/gladier_tools/posix/https_download_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-04-16 16:33:40.000000 gladier_tools-0.5.3/gladier_tools/posix/shell_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-16 16:33:40.000000 gladier_tools-0.5.3/gladier_tools/posix/tar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-04-16 16:33:40.000000 gladier_tools-0.5.3/gladier_tools/posix/untar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:33:43.703886 gladier_tools-0.5.3/gladier_tools/publish/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-16 16:33:40.000000 gladier_tools-0.5.3/gladier_tools/publish/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7086 2024-04-16 16:33:40.000000 gladier_tools-0.5.3/gladier_tools/publish/publish.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18327 2024-04-16 16:33:40.000000 gladier_tools-0.5.3/gladier_tools/publish/publishv2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:33:43.703886 gladier_tools-0.5.3/gladier_tools/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 16:33:40.000000 gladier_tools-0.5.3/gladier_tools/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:33:43.707886 gladier_tools-0.5.3/gladier_tools/tests/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 16:33:40.000000 gladier_tools-0.5.3/gladier_tools/tests/experimental/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:33:43.707886 gladier_tools-0.5.3/gladier_tools/tests/experimental/globus/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 16:33:40.000000 gladier_tools-0.5.3/gladier_tools/tests/experimental/globus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-16 16:33:40.000000 gladier_tools-0.5.3/gladier_tools/tests/experimental/globus/test_mkdir.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:33:43.707886 gladier_tools-0.5.3/gladier_tools/tests/posix/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 16:33:40.000000 gladier_tools-0.5.3/gladier_tools/tests/posix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-16 16:33:40.000000 gladier_tools-0.5.3/gladier_tools/tests/posix/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-16 16:33:40.000000 gladier_tools-0.5.3/gladier_tools/tests/posix/mocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-04-16 16:33:40.000000 gladier_tools-0.5.3/gladier_tools/tests/posix/test_decrypt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-04-16 16:33:40.000000 gladier_tools-0.5.3/gladier_tools/tests/posix/test_encrypt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-16 16:33:40.000000 gladier_tools-0.5.3/gladier_tools/tests/posix/test_gladier_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-04-16 16:33:40.000000 gladier_tools-0.5.3/gladier_tools/tests/posix/test_shell_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-16 16:33:40.000000 gladier_tools-0.5.3/gladier_tools/tests/posix/test_tar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-16 16:33:40.000000 gladier_tools-0.5.3/gladier_tools/tests/posix/test_untar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:33:43.707886 gladier_tools-0.5.3/gladier_tools/tests/publish/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 16:33:40.000000 gladier_tools-0.5.3/gladier_tools/tests/publish/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-04-16 16:33:40.000000 gladier_tools-0.5.3/gladier_tools/tests/publish/test_publish.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11137 2024-04-16 16:33:40.000000 gladier_tools-0.5.3/gladier_tools/tests/publish/test_publishv2.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-16 16:33:40.000000 gladier_tools-0.5.3/gladier_tools/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:33:43.707886 gladier_tools-0.5.3/gladier_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-04-16 16:33:43.000000 gladier_tools-0.5.3/gladier_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-16 16:33:43.000000 gladier_tools-0.5.3/gladier_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 16:33:43.000000 gladier_tools-0.5.3/gladier_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-16 16:33:43.000000 gladier_tools-0.5.3/gladier_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-16 16:33:43.000000 gladier_tools-0.5.3/gladier_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-16 16:33:40.000000 gladier_tools-0.5.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-16 16:33:43.707886 gladier_tools-0.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-16 16:33:40.000000 gladier_tools-0.5.3/setup.py
```

### Comparing `gladier-tools-0.5.2/LICENSE` & `gladier_tools-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gladier-tools-0.5.2/PKG-INFO` & `gladier_tools-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gladier-tools
-Version: 0.5.2
+Version: 0.5.3
 Summary: A set of reusable Gladier Tools
 Home-page: https://github.com/globus-gladier/gladier-tools
 Maintainer: The Gladier Team
 Maintainer-email: 
 License: Apache 2.0
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `gladier-tools-0.5.2/README.rst` & `gladier_tools-0.5.3/README.rst`

 * *Files identical despite different names*

### Comparing `gladier-tools-0.5.2/gladier_tools/experimental/__init__.py` & `gladier_tools-0.5.3/gladier_tools/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `gladier-tools-0.5.2/gladier_tools/experimental/base.py` & `gladier_tools-0.5.3/gladier_tools/experimental/base.py`

 * *Files identical despite different names*

### Comparing `gladier-tools-0.5.2/gladier_tools/experimental/globus/mkdir.py` & `gladier_tools-0.5.3/gladier_tools/experimental/globus/mkdir.py`

 * *Files identical despite different names*

### Comparing `gladier-tools-0.5.2/gladier_tools/globus/transfer.py` & `gladier_tools-0.5.3/gladier_tools/globus/transfer.py`

 * *Files identical despite different names*

### Comparing `gladier-tools-0.5.2/gladier_tools/posix/asymmetric_decrypt.py` & `gladier_tools-0.5.3/gladier_tools/posix/asymmetric_decrypt.py`

 * *Files identical despite different names*

### Comparing `gladier-tools-0.5.2/gladier_tools/posix/asymmetric_encrypt.py` & `gladier_tools-0.5.3/gladier_tools/posix/asymmetric_encrypt.py`

 * *Files identical despite different names*

### Comparing `gladier-tools-0.5.2/gladier_tools/posix/decrypt.py` & `gladier_tools-0.5.3/gladier_tools/posix/decrypt.py`

 * *Files identical despite different names*

### Comparing `gladier-tools-0.5.2/gladier_tools/posix/encrypt.py` & `gladier_tools-0.5.3/gladier_tools/posix/encrypt.py`

 * *Files identical despite different names*

### Comparing `gladier-tools-0.5.2/gladier_tools/posix/https_download_file.py` & `gladier_tools-0.5.3/gladier_tools/posix/https_download_file.py`

 * *Files identical despite different names*

### Comparing `gladier-tools-0.5.2/gladier_tools/posix/shell_cmd.py` & `gladier_tools-0.5.3/gladier_tools/posix/shell_cmd.py`

 * *Files identical despite different names*

### Comparing `gladier-tools-0.5.2/gladier_tools/posix/tar.py` & `gladier_tools-0.5.3/gladier_tools/posix/tar.py`

 * *Files identical despite different names*

### Comparing `gladier-tools-0.5.2/gladier_tools/posix/untar.py` & `gladier_tools-0.5.3/gladier_tools/posix/untar.py`

 * *Files identical despite different names*

### Comparing `gladier-tools-0.5.2/gladier_tools/publish/publish.py` & `gladier_tools-0.5.3/gladier_tools/publish/publish.py`

 * *Files identical despite different names*

### Comparing `gladier-tools-0.5.2/gladier_tools/publish/publishv2.py` & `gladier_tools-0.5.3/gladier_tools/publish/publishv2.py`

 * *Files 4% similar despite different names*

```diff
@@ -90,22 +90,28 @@
 
     def get_remote_file_manifest(filepath, destination_path, url_host, algorithms):
         dataset = pathlib.Path(filepath)
         destination = pathlib.Path(destination_path)
         if not dataset.exists():
             raise ValueError(f"File does not exist: {filepath}")
 
-        file_list = [dataset] if dataset.is_file() else list(dataset.iterdir())
+        if dataset.is_file():
+            file_list = [dataset]
+        else:
+            # Glob together all directories, then iterate over them for all files
+            file_list = [dir.iterdir() for dir in dataset.glob("**")]
+            file_list = [f for subgroup in file_list for f in subgroup]
         file_list = [
             (
                 local_abspath,
                 destination
                 / str(local_abspath.relative_to(dataset.parent)).lstrip("/"),
             )
             for local_abspath in file_list
+            if not local_abspath.is_dir()
         ]
 
         manifest_entries = []
         for subfile, remote_short_path in file_list:
             rfm = {alg: compute_checksum(subfile, alg) for alg in algorithms}
             # mimetype = analysis.mimetypes.detect_type(subfile)
             rfm.update(
@@ -282,16 +288,16 @@
             'dataset': 'foo.txt',
             'destination': '/~/my-test-dir',
             'source_collection': 'my-source-globus-collection',
             'destination_collection': 'my-destination-globus-collection',
             'index': 'my-globus-search-index-uuid',
             'visible_to': ['public'],
             # Ingest and Transfer are disabled by default, allowing for 'dry-run' testing.
-            # 'ingest_enabled': True,
-            # 'transfer_enabled': True,
+            # 'enable_publish': True,
+            # 'enable_transfer': True,
         },
         'funcx_endpoint_non_compute': '4b116d3c-1703-4f8f-9f6f-39921e5864df',
 
     :param dataset: Path to file or directory, which will be catalogued in Globus Search and transferred
         to the remote destination
     :param destination: Location on destination collection where data should be stored
     :param source_collection: The source Globus Collection where data is stored
@@ -350,19 +356,19 @@
             "Publishv2ChoiceTransfer": {
                 "Comment": "Determine if the document should be cataloged in Globus Search",
                 "Type": "Choice",
                 "Choices": [
                     {
                         "And": [
                             {
-                                "Variable": "$.input.publishv2.transfer_enabled",
+                                "Variable": "$.input.publishv2.enable_transfer",
                                 "IsPresent": True,
                             },
                             {
-                                "Variable": "$.input.publishv2.transfer_enabled",
+                                "Variable": "$.input.publishv2.enable_transfer",
                                 "BooleanEquals": True,
                             },
                         ],
                         "Next": "Publishv2Transfer",
                     }
                 ],
                 "Default": "Publishv2SkipTransfer",
@@ -384,19 +390,19 @@
             "Publishv2ChoiceIngest": {
                 "Comment": "Determine if the document should be cataloged in Globus Search",
                 "Type": "Choice",
                 "Choices": [
                     {
                         "And": [
                             {
-                                "Variable": "$.input.publishv2.ingest_enabled",
+                                "Variable": "$.input.publishv2.enable_publish",
                                 "IsPresent": True,
                             },
                             {
-                                "Variable": "$.input.publishv2.ingest_enabled",
+                                "Variable": "$.input.publishv2.enable_publish",
                                 "BooleanEquals": True,
                             },
                         ],
                         "Next": "Publishv2Ingest",
                     }
                 ],
                 "Default": "Publishv2SkipIngest",
```

### Comparing `gladier-tools-0.5.2/gladier_tools/tests/posix/test_decrypt.py` & `gladier_tools-0.5.3/gladier_tools/tests/posix/test_decrypt.py`

 * *Files identical despite different names*

### Comparing `gladier-tools-0.5.2/gladier_tools/tests/posix/test_encrypt.py` & `gladier_tools-0.5.3/gladier_tools/tests/posix/test_encrypt.py`

 * *Files identical despite different names*

### Comparing `gladier-tools-0.5.2/gladier_tools/tests/posix/test_gladier_tools.py` & `gladier_tools-0.5.3/gladier_tools/tests/posix/test_gladier_tools.py`

 * *Files identical despite different names*

### Comparing `gladier-tools-0.5.2/gladier_tools/tests/posix/test_shell_cmd.py` & `gladier_tools-0.5.3/gladier_tools/tests/posix/test_shell_cmd.py`

 * *Files identical despite different names*

### Comparing `gladier-tools-0.5.2/gladier_tools/tests/posix/test_tar.py` & `gladier_tools-0.5.3/gladier_tools/tests/posix/test_tar.py`

 * *Files identical despite different names*

### Comparing `gladier-tools-0.5.2/gladier_tools/tests/posix/test_untar.py` & `gladier_tools-0.5.3/gladier_tools/tests/posix/test_untar.py`

 * *Files identical despite different names*

### Comparing `gladier-tools-0.5.2/gladier_tools/tests/publish/test_publish.py` & `gladier_tools-0.5.3/gladier_tools/tests/publish/test_publish.py`

 * *Files identical despite different names*

### Comparing `gladier-tools-0.5.2/gladier_tools/tests/publish/test_publishv2.py` & `gladier_tools-0.5.3/gladier_tools/tests/publish/test_publishv2.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import pytest
 from unittest import mock
 import pathlib
+import datetime
 import json
 from datacite import schema42, schema43
 from gladier_tools.publish.publishv2 import publishv2_gather_metadata
 
 mock_data = pathlib.Path(__file__).resolve().parent.parent / "mock_data/publish/"
 
 minimum_dc_metadata = {
@@ -39,15 +40,29 @@
         "visible_to": ["public"],
         "enable_metadata_dc": True,
         "groups": [],
     }
 
 
 def test_publish(publish_input):
-    publishv2_gather_metadata(**publish_input).keys() == ("search", "transfer")
+    assert set(publishv2_gather_metadata(**publish_input)) == {"search", "transfer"}
+
+
+def test_publish_nested_dataset(publish_input):
+    publish_input["dataset"] = mock_data / "nested_dataset_folder"
+    metadata = publishv2_gather_metadata(**publish_input)
+    assert set(metadata) == {"search", "transfer"}
+
+    files = metadata["search"]["content"]["files"]
+    assert len(files) == 2
+    urls = {f["url"] for f in files}
+    assert urls == {
+        "globus://my_globus_collection/my-new-project/nested_dataset_folder/bar.txt",
+        "globus://my_globus_collection/my-new-project/nested_dataset_folder/nested_folder/foo.txt",
+    }
 
 
 def test_json_serializable(publish_input):
     assert json.dumps(publishv2_gather_metadata(**publish_input))
 
 
 def test_publish_dc(publish_input):
@@ -64,15 +79,15 @@
                 "identifierType": "GlobusSearchSubject",
             }
         ],
         # timestamp contains seconds, which is hard to check. Skip it!
         # '2023-03-17T17:14:31.832955Z'
         # 'dates': [{'date': '2023-03-16T07:44:14.044091', 'dateType': 'Created'}],
         "formats": ["text/plain"],
-        "publicationYear": "2023",
+        "publicationYear": str(datetime.datetime.now().year),
         "publisher": "",
         "types": {"resourceType": "Dataset", "resourceTypeGeneral": "Dataset"},
         "subjects": [],
         "titles": [{"title": "test_dataset_folder"}],
         "version": "1",
         "schemaVersion": "http://datacite.org/schema/kernel-4",
     }
@@ -265,15 +280,17 @@
     }
 
 
 def test_publish_collection_valid_basepath(publish_input):
     """Test Guest Collection basepath where the share point is the parent of the source
     dataset being published."""
     publish_input["source_collection_basepath"] = publish_input["dataset"].parent
-    source_file = publishv2_gather_metadata(**publish_input)["transfer"]["transfer_items"][0]
+    source_file = publishv2_gather_metadata(**publish_input)["transfer"][
+        "transfer_items"
+    ][0]
     assert source_file["source_path"] == f"/{publish_input['dataset'].name}"
 
 
 def test_publish_collection_source_basepath_mismatch(publish_input):
     """Test Guest Collection basepath where the share point is the parent of the source
     dataset being published."""
     publish_input["source_collection_basepath"] = (
```

### Comparing `gladier-tools-0.5.2/gladier_tools.egg-info/PKG-INFO` & `gladier_tools-0.5.3/gladier_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gladier-tools
-Version: 0.5.2
+Version: 0.5.3
 Summary: A set of reusable Gladier Tools
 Home-page: https://github.com/globus-gladier/gladier-tools
 Maintainer: The Gladier Team
 Maintainer-email: 
 License: Apache 2.0
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `gladier-tools-0.5.2/gladier_tools.egg-info/SOURCES.txt` & `gladier_tools-0.5.3/gladier_tools.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,17 @@
 gladier_tools/posix/shell_cmd.py
 gladier_tools/posix/tar.py
 gladier_tools/posix/untar.py
 gladier_tools/publish/__init__.py
 gladier_tools/publish/publish.py
 gladier_tools/publish/publishv2.py
 gladier_tools/tests/__init__.py
+gladier_tools/tests/experimental/__init__.py
+gladier_tools/tests/experimental/globus/__init__.py
+gladier_tools/tests/experimental/globus/test_mkdir.py
 gladier_tools/tests/posix/__init__.py
 gladier_tools/tests/posix/conftest.py
 gladier_tools/tests/posix/mocks.py
 gladier_tools/tests/posix/test_decrypt.py
 gladier_tools/tests/posix/test_encrypt.py
 gladier_tools/tests/posix/test_gladier_tools.py
 gladier_tools/tests/posix/test_shell_cmd.py
```

### Comparing `gladier-tools-0.5.2/setup.py` & `gladier_tools-0.5.3/setup.py`

 * *Files identical despite different names*

