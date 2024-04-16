# Comparing `tmp/haskellian_asyn_iter-0.1.3.tar.gz` & `tmp/haskellian_asyn_iter-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haskellian_asyn_iter-0.1.3.tar", last modified: Tue Apr 16 06:35:33 2024, max compression
+gzip compressed data, was "haskellian_asyn_iter-0.1.4.tar", last modified: Tue Apr 16 06:36:49 2024, max compression
```

## Comparing `haskellian_asyn_iter-0.1.3.tar` & `haskellian_asyn_iter-0.1.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-16 06:35:33.397021 haskellian_asyn_iter-0.1.3/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      374 2024-04-16 06:35:33.397021 haskellian_asyn_iter-0.1.3/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       60 2024-04-10 04:56:14.000000 haskellian_asyn_iter-0.1.3/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      550 2024-04-16 06:35:31.000000 haskellian_asyn_iter-0.1.3/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-16 06:35:33.397021 haskellian_asyn_iter-0.1.3/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-16 06:35:33.397021 haskellian_asyn_iter-0.1.3/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-16 06:35:33.387021 haskellian_asyn_iter-0.1.3/src/haskellian/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-16 06:35:33.387021 haskellian_asyn_iter-0.1.3/src/haskellian/asyn/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-16 06:35:33.397021 haskellian_asyn_iter-0.1.3/src/haskellian/asyn/iter/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      151 2024-04-10 07:00:49.000000 haskellian_asyn_iter-0.1.3/src/haskellian/asyn/iter/__init__.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-16 06:35:33.397021 haskellian_asyn_iter-0.1.3/src/haskellian/asyn/iter/iter/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       51 2024-04-10 05:17:31.000000 haskellian_asyn_iter-0.1.3/src/haskellian/asyn/iter/iter/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      409 2024-04-10 05:17:42.000000 haskellian_asyn_iter-0.1.3/src/haskellian/asyn/iter/iter/funcs.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1738 2024-04-12 05:42:50.000000 haskellian_asyn_iter-0.1.3/src/haskellian/asyn/iter/iter/iter.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      769 2024-04-10 07:02:38.000000 haskellian_asyn_iter-0.1.3/src/haskellian/asyn/iter/managed.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-16 06:35:33.397021 haskellian_asyn_iter-0.1.3/src/haskellian/asyn/iter/ops/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      169 2024-04-11 09:58:47.000000 haskellian_asyn_iter-0.1.3/src/haskellian/asyn/iter/ops/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2417 2024-04-11 09:58:17.000000 haskellian_asyn_iter-0.1.3/src/haskellian/asyn/iter/ops/ops.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      540 2024-04-10 05:09:46.000000 haskellian_asyn_iter-0.1.3/src/haskellian/asyn/iter/ops/prefetching.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-16 06:35:33.397021 haskellian_asyn_iter-0.1.3/src/haskellian_asyn_iter.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      374 2024-04-16 06:35:33.000000 haskellian_asyn_iter-0.1.3/src/haskellian_asyn_iter.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      576 2024-04-16 06:35:33.000000 haskellian_asyn_iter-0.1.3/src/haskellian_asyn_iter.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-16 06:35:33.000000 haskellian_asyn_iter-0.1.3/src/haskellian_asyn_iter.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       16 2024-04-16 06:35:33.000000 haskellian_asyn_iter-0.1.3/src/haskellian_asyn_iter.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       11 2024-04-16 06:35:33.000000 haskellian_asyn_iter-0.1.3/src/haskellian_asyn_iter.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-16 06:36:49.001520 haskellian_asyn_iter-0.1.4/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      374 2024-04-16 06:36:48.991520 haskellian_asyn_iter-0.1.4/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       60 2024-04-10 04:56:14.000000 haskellian_asyn_iter-0.1.4/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      550 2024-04-16 06:36:45.000000 haskellian_asyn_iter-0.1.4/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-16 06:36:49.001520 haskellian_asyn_iter-0.1.4/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-16 06:36:48.991520 haskellian_asyn_iter-0.1.4/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-16 06:36:48.981520 haskellian_asyn_iter-0.1.4/src/haskellian/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-16 06:36:48.991520 haskellian_asyn_iter-0.1.4/src/haskellian/asyn/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-16 06:36:48.991520 haskellian_asyn_iter-0.1.4/src/haskellian/asyn/iter/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      170 2024-04-16 06:36:14.000000 haskellian_asyn_iter-0.1.4/src/haskellian/asyn/iter/__init__.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-16 06:36:48.991520 haskellian_asyn_iter-0.1.4/src/haskellian/asyn/iter/iter/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       51 2024-04-10 05:17:31.000000 haskellian_asyn_iter-0.1.4/src/haskellian/asyn/iter/iter/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      409 2024-04-10 05:17:42.000000 haskellian_asyn_iter-0.1.4/src/haskellian/asyn/iter/iter/funcs.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1738 2024-04-12 05:42:50.000000 haskellian_asyn_iter-0.1.4/src/haskellian/asyn/iter/iter/iter.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      769 2024-04-10 07:02:38.000000 haskellian_asyn_iter-0.1.4/src/haskellian/asyn/iter/managed.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-16 06:36:48.991520 haskellian_asyn_iter-0.1.4/src/haskellian/asyn/iter/ops/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      169 2024-04-11 09:58:47.000000 haskellian_asyn_iter-0.1.4/src/haskellian/asyn/iter/ops/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2417 2024-04-11 09:58:17.000000 haskellian_asyn_iter-0.1.4/src/haskellian/asyn/iter/ops/ops.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      540 2024-04-10 05:09:46.000000 haskellian_asyn_iter-0.1.4/src/haskellian/asyn/iter/ops/prefetching.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-16 06:36:48.991520 haskellian_asyn_iter-0.1.4/src/haskellian_asyn_iter.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      374 2024-04-16 06:36:48.000000 haskellian_asyn_iter-0.1.4/src/haskellian_asyn_iter.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      576 2024-04-16 06:36:48.000000 haskellian_asyn_iter-0.1.4/src/haskellian_asyn_iter.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-16 06:36:48.000000 haskellian_asyn_iter-0.1.4/src/haskellian_asyn_iter.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       16 2024-04-16 06:36:48.000000 haskellian_asyn_iter-0.1.4/src/haskellian_asyn_iter.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       11 2024-04-16 06:36:48.000000 haskellian_asyn_iter-0.1.4/src/haskellian_asyn_iter.egg-info/top_level.txt
```

### Comparing `haskellian_asyn_iter-0.1.3/pyproject.toml` & `haskellian_asyn_iter-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "haskellian-asyn-iter"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "FP-style tools for async iterables"
 dependencies = [
   "haskellian-asyn"
 ]
```

### Comparing `haskellian_asyn_iter-0.1.3/src/haskellian/asyn/iter/iter/iter.py` & `haskellian_asyn_iter-0.1.4/src/haskellian/asyn/iter/iter/iter.py`

 * *Files identical despite different names*

### Comparing `haskellian_asyn_iter-0.1.3/src/haskellian/asyn/iter/managed.py` & `haskellian_asyn_iter-0.1.4/src/haskellian/asyn/iter/managed.py`

 * *Files identical despite different names*

### Comparing `haskellian_asyn_iter-0.1.3/src/haskellian/asyn/iter/ops/ops.py` & `haskellian_asyn_iter-0.1.4/src/haskellian/asyn/iter/ops/ops.py`

 * *Files identical despite different names*

### Comparing `haskellian_asyn_iter-0.1.3/src/haskellian/asyn/iter/ops/prefetching.py` & `haskellian_asyn_iter-0.1.4/src/haskellian/asyn/iter/ops/prefetching.py`

 * *Files identical despite different names*

### Comparing `haskellian_asyn_iter-0.1.3/src/haskellian_asyn_iter.egg-info/SOURCES.txt` & `haskellian_asyn_iter-0.1.4/src/haskellian_asyn_iter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

