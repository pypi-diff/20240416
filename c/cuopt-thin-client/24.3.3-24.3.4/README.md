# Comparing `tmp/cuopt_thin_client-24.3.3.tar.gz` & `tmp/cuopt_thin_client-24.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cuopt_thin_client-24.3.3.tar", last modified: Mon Mar 11 23:28:38 2024, max compression
+gzip compressed data, was "cuopt_thin_client-24.3.4.tar", last modified: Mon Apr  5 07:00:00 1993, max compression
```

## Comparing `cuopt_thin_client-24.3.3.tar` & `cuopt_thin_client-24.3.4.tar`

### file list

```diff
@@ -1,13 +1,2 @@
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2024-03-11 23:28:38.693495 cuopt_thin_client-24.3.3/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      464 2024-03-11 23:28:38.000000 cuopt_thin_client-24.3.3/ERROR.txt
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2024-02-13 20:52:43.000000 cuopt_thin_client-24.3.3/LICENSE.md
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       17 2024-03-11 23:28:38.000000 cuopt_thin_client-24.3.3/PACKAGE_NAME
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1654 2024-03-11 23:28:38.693495 cuopt_thin_client-24.3.3/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      271 2024-03-11 23:28:38.000000 cuopt_thin_client-24.3.3/README.rst
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2024-03-11 23:28:38.693495 cuopt_thin_client-24.3.3/cuopt_thin_client.egg-info/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1654 2024-03-11 23:28:38.000000 cuopt_thin_client-24.3.3/cuopt_thin_client.egg-info/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      217 2024-03-11 23:28:38.000000 cuopt_thin_client-24.3.3/cuopt_thin_client.egg-info/SOURCES.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2024-03-11 23:28:38.000000 cuopt_thin_client-24.3.3/cuopt_thin_client.egg-info/dependency_links.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2024-03-11 23:28:38.000000 cuopt_thin_client-24.3.3/cuopt_thin_client.egg-info/top_level.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2024-03-11 23:28:38.693495 cuopt_thin_client-24.3.3/setup.cfg
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4864 2024-02-13 20:52:43.000000 cuopt_thin_client-24.3.3/setup.py
+-rw-r--r--   0        0        0      217 1993-04-05 07:00:00.000000 pyproject.toml
+-rw-r--r--   0        0        0     6674 1993-04-05 07:00:00.000000 PKG-INFO
```

