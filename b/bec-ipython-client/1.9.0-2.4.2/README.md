# Comparing `tmp/bec_ipython_client-1.9.0.tar.gz` & `tmp/bec_ipython_client-2.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bec_ipython_client-1.9.0.tar", last modified: Thu Feb 22 19:50:20 2024, max compression
+gzip compressed data, was "bec_ipython_client-2.4.2.tar", last modified: Tue Apr 16 15:05:13 2024, max compression
```

## Comparing `bec_ipython_client-1.9.0.tar` & `bec_ipython_client-2.4.2.tar`

### file list

```diff
@@ -1,49 +1,57 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 19:50:20.333848 bec_ipython_client-1.9.0/
--rw-r--r--   0 root         (0) root         (0)      458 2024-02-22 19:50:20.333848 bec_ipython_client-1.9.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 19:50:20.331848 bec_ipython_client-1.9.0/bec_client/
--rw-rw-rw-   0 root         (0) root         (0)       85 2024-02-22 18:57:01.000000 bec_ipython_client-1.9.0/bec_client/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1067 2024-02-22 18:57:01.000000 bec_ipython_client-1.9.0/bec_client/beamline_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     5040 2024-02-22 18:57:01.000000 bec_ipython_client-1.9.0/bec_client/bec_client.py
--rw-rw-rw-   0 root         (0) root         (0)     1972 2024-02-22 18:57:01.000000 bec_ipython_client-1.9.0/bec_client/bec_magics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 19:50:20.333848 bec_ipython_client-1.9.0/bec_client/bin/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-22 19:50:05.000000 bec_ipython_client-1.9.0/bec_client/bin/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      830 2024-02-22 18:57:01.000000 bec_ipython_client-1.9.0/bec_client/bin/bec
--rw-rw-rw-   0 root         (0) root         (0)     2860 2024-02-22 18:57:01.000000 bec_ipython_client-1.9.0/bec_client/bin/bec_startup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 19:50:20.331848 bec_ipython_client-1.9.0/bec_client/callbacks/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-22 19:50:05.000000 bec_ipython_client-1.9.0/bec_client/callbacks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8460 2024-02-22 18:57:01.000000 bec_ipython_client-1.9.0/bec_client/callbacks/ipython_live_updates.py
--rw-rw-rw-   0 root         (0) root         (0)    10363 2024-02-22 19:40:05.000000 bec_ipython_client-1.9.0/bec_client/callbacks/live_table.py
--rw-rw-rw-   0 root         (0) root         (0)     4873 2024-02-22 18:57:01.000000 bec_ipython_client-1.9.0/bec_client/callbacks/move_device.py
--rw-rw-rw-   0 root         (0) root         (0)     1960 2024-02-22 18:57:01.000000 bec_ipython_client-1.9.0/bec_client/callbacks/scan_progress.py
--rw-rw-rw-   0 root         (0) root         (0)     3891 2024-02-22 18:57:01.000000 bec_ipython_client-1.9.0/bec_client/callbacks/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 19:50:20.332848 bec_ipython_client-1.9.0/bec_client/high_level_interfaces/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-22 19:50:05.000000 bec_ipython_client-1.9.0/bec_client/high_level_interfaces/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6854 2024-02-22 18:57:01.000000 bec_ipython_client-1.9.0/bec_client/high_level_interfaces/spec_hli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 19:50:20.332848 bec_ipython_client-1.9.0/bec_client/plugins/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 19:50:20.332848 bec_ipython_client-1.9.0/bec_client/plugins/LamNI/
--rw-rw-rw-   0 root         (0) root         (0)      149 2024-02-22 18:57:01.000000 bec_ipython_client-1.9.0/bec_client/plugins/LamNI/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5519 2024-02-22 18:57:01.000000 bec_ipython_client-1.9.0/bec_client/plugins/LamNI/lamni_optics_mixin.py
--rwxrwxrwx   0 root         (0) root         (0)      895 2024-02-22 18:57:01.000000 bec_ipython_client-1.9.0/bec_client/plugins/LamNI/load_additional_correction.py
--rw-rw-rw-   0 root         (0) root         (0)    54705 2024-02-22 18:57:01.000000 bec_ipython_client-1.9.0/bec_client/plugins/LamNI/x_ray_eye_align.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 19:50:20.332848 bec_ipython_client-1.9.0/bec_client/plugins/SLS/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-22 19:50:05.000000 bec_ipython_client-1.9.0/bec_client/plugins/SLS/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4926 2024-02-22 18:57:01.000000 bec_ipython_client-1.9.0/bec_client/plugins/SLS/sls_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 19:50:20.332848 bec_ipython_client-1.9.0/bec_client/plugins/XTreme/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-22 19:50:05.000000 bec_ipython_client-1.9.0/bec_client/plugins/XTreme/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3631 2024-02-22 18:57:01.000000 bec_ipython_client-1.9.0/bec_client/plugins/XTreme/x-treme.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-22 19:50:05.000000 bec_ipython_client-1.9.0/bec_client/plugins/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 19:50:20.333848 bec_ipython_client-1.9.0/bec_client/plugins/cSAXS/
--rw-rw-rw-   0 root         (0) root         (0)       79 2024-02-22 18:57:01.000000 bec_ipython_client-1.9.0/bec_client/plugins/cSAXS/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4433 2024-02-22 18:57:01.000000 bec_ipython_client-1.9.0/bec_client/plugins/cSAXS/beamline_info.py
--rw-rw-rw-   0 root         (0) root         (0)      445 2024-02-22 18:57:01.000000 bec_ipython_client-1.9.0/bec_client/plugins/cSAXS/cSAXS_beamline.py
--rw-rw-rw-   0 root         (0) root         (0)     2534 2024-02-22 18:57:01.000000 bec_ipython_client-1.9.0/bec_client/prettytable.py
--rw-rw-rw-   0 root         (0) root         (0)     8442 2024-02-22 18:57:01.000000 bec_ipython_client-1.9.0/bec_client/progressbar.py
--rw-rw-rw-   0 root         (0) root         (0)     4299 2024-02-22 18:57:01.000000 bec_ipython_client-1.9.0/bec_client/signals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 19:50:20.333848 bec_ipython_client-1.9.0/bec_ipython_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)      458 2024-02-22 19:50:20.000000 bec_ipython_client-1.9.0/bec_ipython_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1325 2024-02-22 19:50:20.000000 bec_ipython_client-1.9.0/bec_ipython_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-22 19:50:20.000000 bec_ipython_client-1.9.0/bec_ipython_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      151 2024-02-22 19:50:20.000000 bec_ipython_client-1.9.0/bec_ipython_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-02-22 19:50:20.000000 bec_ipython_client-1.9.0/bec_ipython_client.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      519 2024-02-22 19:50:20.334848 bec_ipython_client-1.9.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2053 2024-02-22 19:50:16.000000 bec_ipython_client-1.9.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:05:13.535278 bec_ipython_client-2.4.2/
+-rw-r--r--   0 root         (0) root         (0)      414 2024-04-16 15:05:13.535278 bec_ipython_client-2.4.2/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:05:13.533278 bec_ipython_client-2.4.2/bec_ipython_client/
+-rw-rw-rw-   0 root         (0) root         (0)       79 2024-04-16 14:21:24.000000 bec_ipython_client-2.4.2/bec_ipython_client/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1067 2024-04-16 14:21:24.000000 bec_ipython_client-2.4.2/bec_ipython_client/beamline_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     1980 2024-04-16 14:21:24.000000 bec_ipython_client-2.4.2/bec_ipython_client/bec_magics.py
+-rw-rw-rw-   0 root         (0) root         (0)     1588 2024-04-16 14:21:24.000000 bec_ipython_client-2.4.2/bec_ipython_client/bec_startup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:05:13.533278 bec_ipython_client-2.4.2/bec_ipython_client/callbacks/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-16 15:05:02.000000 bec_ipython_client-2.4.2/bec_ipython_client/callbacks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9941 2024-04-16 14:21:24.000000 bec_ipython_client-2.4.2/bec_ipython_client/callbacks/ipython_live_updates.py
+-rw-rw-rw-   0 root         (0) root         (0)    11964 2024-04-16 14:21:24.000000 bec_ipython_client-2.4.2/bec_ipython_client/callbacks/live_table.py
+-rw-rw-rw-   0 root         (0) root         (0)     5503 2024-04-16 14:21:24.000000 bec_ipython_client-2.4.2/bec_ipython_client/callbacks/move_device.py
+-rw-rw-rw-   0 root         (0) root         (0)     2260 2024-04-16 14:21:24.000000 bec_ipython_client-2.4.2/bec_ipython_client/callbacks/scan_progress.py
+-rw-rw-rw-   0 root         (0) root         (0)     4460 2024-04-16 14:21:24.000000 bec_ipython_client-2.4.2/bec_ipython_client/callbacks/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:05:13.534278 bec_ipython_client-2.4.2/bec_ipython_client/high_level_interfaces/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-16 15:05:02.000000 bec_ipython_client-2.4.2/bec_ipython_client/high_level_interfaces/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1221 2024-04-16 14:21:24.000000 bec_ipython_client-2.4.2/bec_ipython_client/high_level_interfaces/bec_hli.py
+-rw-rw-rw-   0 root         (0) root         (0)     5818 2024-04-16 14:21:24.000000 bec_ipython_client-2.4.2/bec_ipython_client/high_level_interfaces/spec_hli.py
+-rw-rw-rw-   0 root         (0) root         (0)     8453 2024-04-16 14:21:24.000000 bec_ipython_client-2.4.2/bec_ipython_client/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:05:13.534278 bec_ipython_client-2.4.2/bec_ipython_client/plugins/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:05:13.534278 bec_ipython_client-2.4.2/bec_ipython_client/plugins/LamNI/
+-rw-rw-rw-   0 root         (0) root         (0)      149 2024-04-16 14:21:24.000000 bec_ipython_client-2.4.2/bec_ipython_client/plugins/LamNI/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5516 2024-04-16 14:21:24.000000 bec_ipython_client-2.4.2/bec_ipython_client/plugins/LamNI/lamni_optics_mixin.py
+-rwxrwxrwx   0 root         (0) root         (0)      872 2024-04-16 14:21:24.000000 bec_ipython_client-2.4.2/bec_ipython_client/plugins/LamNI/load_additional_correction.py
+-rw-rw-rw-   0 root         (0) root         (0)    54701 2024-04-16 14:21:24.000000 bec_ipython_client-2.4.2/bec_ipython_client/plugins/LamNI/x_ray_eye_align.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:05:13.534278 bec_ipython_client-2.4.2/bec_ipython_client/plugins/SLS/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-16 15:05:02.000000 bec_ipython_client-2.4.2/bec_ipython_client/plugins/SLS/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4934 2024-04-16 14:21:24.000000 bec_ipython_client-2.4.2/bec_ipython_client/plugins/SLS/sls_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:05:13.534278 bec_ipython_client-2.4.2/bec_ipython_client/plugins/XTreme/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-16 15:05:02.000000 bec_ipython_client-2.4.2/bec_ipython_client/plugins/XTreme/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3631 2024-04-16 14:21:24.000000 bec_ipython_client-2.4.2/bec_ipython_client/plugins/XTreme/x-treme.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-16 15:05:02.000000 bec_ipython_client-2.4.2/bec_ipython_client/plugins/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:05:13.534278 bec_ipython_client-2.4.2/bec_ipython_client/plugins/cSAXS/
+-rw-rw-rw-   0 root         (0) root         (0)      128 2024-04-16 14:21:24.000000 bec_ipython_client-2.4.2/bec_ipython_client/plugins/cSAXS/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4441 2024-04-16 14:21:24.000000 bec_ipython_client-2.4.2/bec_ipython_client/plugins/cSAXS/beamline_info.py
+-rw-rw-rw-   0 root         (0) root         (0)      445 2024-04-16 14:21:24.000000 bec_ipython_client-2.4.2/bec_ipython_client/plugins/cSAXS/cSAXS_beamline.py
+-rw-rw-rw-   0 root         (0) root         (0)     4308 2024-04-16 14:21:24.000000 bec_ipython_client-2.4.2/bec_ipython_client/plugins/cSAXS/csaxs_bl_checks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:05:13.535278 bec_ipython_client-2.4.2/bec_ipython_client/plugins/flomni/
+-rw-rw-rw-   0 root         (0) root         (0)       27 2024-04-16 14:21:24.000000 bec_ipython_client-2.4.2/bec_ipython_client/plugins/flomni/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    80400 2024-04-16 14:21:24.000000 bec_ipython_client-2.4.2/bec_ipython_client/plugins/flomni/flomni.py
+-rw-rw-rw-   0 root         (0) root         (0)     6399 2024-04-16 14:21:24.000000 bec_ipython_client-2.4.2/bec_ipython_client/plugins/flomni/flomni_optics_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     8918 2024-04-16 14:21:24.000000 bec_ipython_client-2.4.2/bec_ipython_client/plugins/flomni/x_ray_eye_align.py
+-rw-rw-rw-   0 root         (0) root         (0)     2534 2024-04-16 14:21:24.000000 bec_ipython_client-2.4.2/bec_ipython_client/prettytable.py
+-rw-rw-rw-   0 root         (0) root         (0)    11165 2024-04-16 14:21:24.000000 bec_ipython_client-2.4.2/bec_ipython_client/progressbar.py
+-rw-rw-rw-   0 root         (0) root         (0)     4299 2024-04-16 14:21:24.000000 bec_ipython_client-2.4.2/bec_ipython_client/signals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:05:13.535278 bec_ipython_client-2.4.2/bec_ipython_client/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-16 15:05:02.000000 bec_ipython_client-2.4.2/bec_ipython_client/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7753 2024-04-16 14:21:24.000000 bec_ipython_client-2.4.2/bec_ipython_client/tests/end2end_fixtures.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:05:13.535278 bec_ipython_client-2.4.2/bec_ipython_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      414 2024-04-16 15:05:13.000000 bec_ipython_client-2.4.2/bec_ipython_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1938 2024-04-16 15:05:13.000000 bec_ipython_client-2.4.2/bec_ipython_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 15:05:13.000000 bec_ipython_client-2.4.2/bec_ipython_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      134 2024-04-16 15:05:13.000000 bec_ipython_client-2.4.2/bec_ipython_client.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      162 2024-04-16 15:05:13.000000 bec_ipython_client-2.4.2/bec_ipython_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2024-04-16 15:05:13.000000 bec_ipython_client-2.4.2/bec_ipython_client.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      520 2024-04-16 15:05:13.536278 bec_ipython_client-2.4.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2254 2024-04-16 15:05:11.000000 bec_ipython_client-2.4.2/setup.py
```

### Comparing `bec_ipython_client-1.9.0/bec_client/beamline_mixin.py` & `bec_ipython_client-2.4.2/bec_ipython_client/beamline_mixin.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-1.9.0/bec_client/bec_magics.py` & `bec_ipython_client-2.4.2/bec_ipython_client/bec_magics.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 from IPython.core.magic import Magics, line_magic, magics_class
 
 if TYPE_CHECKING:
-    from bec_client import BECClient
+    from bec_ipython_client import BECClient
 
 
 @magics_class
 class BECMagics(Magics):
     def __init__(self, shell, client: BECClient):
         super(BECMagics, self).__init__(shell)
         self.client = client
```

### Comparing `bec_ipython_client-1.9.0/bec_client/callbacks/ipython_live_updates.py` & `bec_ipython_client-2.4.2/bec_ipython_client/callbacks/ipython_live_updates.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,45 +1,53 @@
 from __future__ import annotations
 
-import asyncio
 import collections
 import time
 from typing import TYPE_CHECKING
 
+from bec_ipython_client.callbacks.scan_progress import LiveUpdatesScanProgress
 from bec_lib import bec_logger
 from bec_lib.bec_errors import ScanInterruption
 
-from bec_client.callbacks.scan_progress import LiveUpdatesScanProgress
-
 from .live_table import LiveUpdatesTable
 from .move_device import LiveUpdatesReadbackProgressbar
 from .utils import ScanRequestMixin, check_alarms
 
 if TYPE_CHECKING:
     from bec_lib import messages
+    from bec_lib.client import BECClient
     from bec_lib.queue_items import QueueItem
 
-    from bec_client import BECClient
-
 logger = bec_logger.logger
 
 
 class IPythonLiveUpdates:
     def __init__(self, client: BECClient) -> None:
+        """Class to handle live updates for IPython, also works in Jupyterlab.
+
+        Args:
+            client (BECClient): The BECClient instance.
+        """
         self.client = client
         self._interrupted_request = None
         self._active_callback = None
         self._processed_instructions = 0
         self._active_request = None
         self._user_callback = None
         self._request_block_index = collections.defaultdict(lambda: 0)
         self._request_block_id = None
         self.print_table_data = True
+        self._current_queue = None
 
     def _process_report_instructions(self, report_instructions: list) -> None:
+        """Process instructions for the live updates.
+
+        Args:
+            report_instructions (list): The list of report instructions.
+        """
         scan_type = self._active_request.content["scan_type"]
         if scan_type in ["open_scan_def", "close_scan_def"]:
             self._process_instruction({"table_wait": 0})
             return
         if scan_type == "close_scan_group":
             return
 
@@ -51,101 +59,105 @@
             return
 
         for instr in remaining_report_instructions:
             self._process_instruction(instr)
             self._processed_instructions += 1
 
     def _process_instruction(self, instr: dict):
+        """Process the received instruction based on scan_report_type.
+
+        Args:
+            instr (dict): The instruction to process.
+        """
         scan_report_type = list(instr.keys())[0]
         scan_def_id = self.client.scans._scan_def_id
         if scan_def_id is None:
             if scan_report_type == "readback":
-                asyncio.run(
+                LiveUpdatesReadbackProgressbar(
+                    self.client,
+                    report_instruction=instr,
+                    request=self._active_request,
+                    callbacks=self._user_callback,
+                ).run()
+            elif scan_report_type == "table_wait":
+                LiveUpdatesTable(
+                    self.client,
+                    report_instruction=instr,
+                    request=self._active_request,
+                    callbacks=self._user_callback,
+                    print_table_data=self.print_table_data,
+                ).run()
+            elif scan_report_type == "scan_progress":
+                LiveUpdatesScanProgress(
+                    self.client,
+                    report_instruction=instr,
+                    request=self._active_request,
+                    callbacks=self._user_callback,
+                ).run()
+            else:
+                raise ValueError(f"Unknown scan report type: {scan_report_type}")
+        else:
+            if self._active_callback:
+                if scan_report_type == "readback":
                     LiveUpdatesReadbackProgressbar(
                         self.client,
                         report_instruction=instr,
                         request=self._active_request,
                         callbacks=self._user_callback,
                     ).run()
-                )
-            elif scan_report_type == "table_wait":
-                asyncio.run(
-                    LiveUpdatesTable(
-                        self.client,
-                        report_instruction=instr,
+                else:
+                    self._active_callback.resume(
                         request=self._active_request,
-                        callbacks=self._user_callback,
-                        print_table_data=self.print_table_data,
-                    ).run()
-                )
-            elif scan_report_type == "scan_progress":
-                asyncio.run(
-                    LiveUpdatesScanProgress(
-                        self.client,
                         report_instruction=instr,
-                        request=self._active_request,
                         callbacks=self._user_callback,
-                    ).run()
-                )
-            else:
-                raise ValueError(f"Unknown scan report type: {scan_report_type}")
-        else:
-            if self._active_callback:
-                if scan_report_type == "readback":
-                    asyncio.run(
-                        LiveUpdatesReadbackProgressbar(
-                            self.client,
-                            report_instruction=instr,
-                            request=self._active_request,
-                            callbacks=self._user_callback,
-                        ).run()
-                    )
-                else:
-                    asyncio.run(
-                        self._active_callback.resume(
-                            request=self._active_request,
-                            report_instruction=instr,
-                            callbacks=self._user_callback,
-                        )
                     )
 
                 return
 
             self._active_callback = LiveUpdatesTable(
                 self.client,
                 report_instruction=instr,
                 request=self._active_request,
                 callbacks=self._user_callback,
                 print_table_data=self.print_table_data,
             )
-            asyncio.run(self._active_callback.run())
+            self._active_callback.run()
+
+    def _available_req_blocks(self, queue: QueueItem, request: messages.ScanQueueMessage):
+        """Get the available request blocks.
 
-    def _available_req_blocks(self, queue, request):
+        Args:
+            queue (QueueItem): The queue item.
+            request (messages.ScanQueueMessage): The request message.
+        """
         available_blocks = [
             req_block
             for req_block in queue.request_blocks
             if req_block["RID"] == request.metadata["RID"]
         ]
         return available_blocks
 
-    def process_request(self, request, scan_report_type, callbacks):
+    def process_request(
+        self, request: messages.ScanQueueMessage, scan_report_type: str, callbacks: any
+    ) -> None:
+        """Process the request and report instructions."""
         # pylint: disable=protected-access
         try:
             with self.client._sighandler:
                 # pylint: disable=protected-access
                 self._active_request = request
                 self._user_callback = callbacks
                 scan_request = ScanRequestMixin(self.client, request.metadata["RID"])
-                asyncio.run(scan_request.wait())
+                scan_request.wait()
 
                 # get the corresponding queue item
                 while not scan_request.request_storage.storage[-1].queue:
                     time.sleep(0.01)
 
-                queue = scan_request.request_storage.storage[-1].queue
+                self._current_queue = queue = scan_request.request_storage.storage[-1].queue
                 self._request_block_id = req_id = self._active_request.metadata.get("RID")
 
                 while queue.status not in ["COMPLETED", "ABORTED", "HALTED"]:
                     if self._process_queue(queue, request, req_id):
                         break
 
                 available_blocks = self._available_req_blocks(queue, request)
@@ -153,17 +165,38 @@
                 report_instructions = req_block.get("report_instructions", [])
                 self._process_report_instructions(report_instructions)
 
             self._reset()
 
         except ScanInterruption as scan_interr:
             self._interrupted_request = (request, scan_report_type)
+            if self._current_queue and self.client._service_config.abort_on_ctrl_c:
+                self._wait_for_cleanup()
             self._reset(forced=True)
             raise scan_interr
 
+    def _wait_for_cleanup(self):
+        """Wait for the scan to be cleaned up."""
+        try:
+            if not self._element_in_queue():
+                return
+            print("Waiting for the scan to be cleaned up...")
+            while self._element_in_queue():
+                time.sleep(0.1)
+        except KeyboardInterrupt:
+            self.client.queue.request_scan_halt()
+
+    def _element_in_queue(self) -> bool:
+        queue = self.client.queue.queue_storage.current_scan_queue.get("primary", {}).get(
+            "info", []
+        )
+        if not queue:
+            return False
+        return self._current_queue.queue_id in queue[0].get("queue_id")
+
     def _process_queue(
         self, queue: QueueItem, request: messages.ScanQueueMessage, req_id: str
     ) -> bool:
         """
         Process the queue and return True if the scan is completed.
 
         Args:
@@ -203,25 +236,32 @@
 
         if not queue.active_request_block:
             return True
 
         return False
 
     def _reset(self, forced=False):
+        """Reset the active request and callback.
+
+        Args:
+            forced(bool): If True, the reset is forced.
+        """
         self._interrupted_request = None
 
+        self._current_queue = None
         self._user_callback = None
         self._processed_instructions = 0
         scan_closed = forced or (self._active_request.content["scan_type"] == "close_scan_def")
         self._active_request = None
 
         if self.client.scans._scan_def_id and not scan_closed:
             self._request_block_index[self._request_block_id] += 1
             return
 
         if scan_closed:
             self._active_callback = None
 
     def continue_request(self):
+        """Continue the interrupted request."""
         if not self._interrupted_request:
             return
         self.process_request(*self._interrupted_request, self._user_callback)
```

### Comparing `bec_ipython_client-1.9.0/bec_client/callbacks/live_table.py` & `bec_ipython_client-2.4.2/bec_ipython_client/callbacks/live_table.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from __future__ import annotations
 
-import asyncio
+import time
 from collections.abc import Callable
 from typing import TYPE_CHECKING
 
+from bec_ipython_client.prettytable import PrettyTable
+from bec_ipython_client.progressbar import ScanProgressBar
 from bec_lib import bec_logger, messages
 
-from bec_client.prettytable import PrettyTable
-from bec_client.progressbar import ScanProgressBar
-
 from .utils import LiveUpdatesBase, check_alarms
 
 if TYPE_CHECKING:
-    from bec_client.bec_client import BECClient
+    from bec_lib.client import BECClient
 
 logger = bec_logger.logger
 
 
 def sort_devices(devices, scan_devices) -> list:
     """sort the devices to ensure that the table starts with scan motors"""
     for scan_dev in list(scan_devices)[::-1]:
@@ -54,58 +53,61 @@
         )
         self.scan_queue_request = None
         self.scan_item = None
         self.dev_values = None
         self.point_data = None
         self.point_id = 0
         self.table = None
+        self.__print_table_data = None
         self._print_table_data = (
             print_table_data if print_table_data is not None else self.REPORT_TYPE == "table_wait"
         )
 
-    async def wait_for_scan_to_start(self):
+    def wait_for_scan_to_start(self):
         """wait until the scan starts"""
         while True:
             queue_pos = self.scan_item.queue.queue_position
             self.check_alarms()
             if self.scan_item.status == "closed":
                 break
             if queue_pos is None:
-                logger.debug(f"Could not find queue entry for scanID {self.scan_item.scanID}")
+                logger.debug(f"Could not find queue entry for scan_id {self.scan_item.scan_id}")
                 continue
             if queue_pos == 0:
                 break
             print(
                 f"Scan is enqueued and is waiting for execution. Current position in queue: {queue_pos + 1}.",
                 end="\r",
                 flush=True,
             )
-            await asyncio.sleep(0.1)
+            time.sleep(0.1)
         while not self.scan_item.scan_number:
-            await asyncio.sleep(0.05)
+            time.sleep(0.05)
 
-    async def wait_for_scan_item_to_finish(self):
+    def wait_for_scan_item_to_finish(self):
         """wait for scan completion"""
         while True:
             if self.scan_item.end_time:
                 if self.scan_item.open_queue_group:
                     break
                 if self.scan_item.queue.queue_position is None:
                     break
             self.check_alarms()
-            await asyncio.sleep(0.1)
+            time.sleep(0.1)
 
     def check_alarms(self):
+        """check for alarms"""
         check_alarms(self.bec)
 
-    async def resume(self, request, report_instruction, callbacks):
+    def resume(self, request: messages.ScanQueueMessage, report_instruction: str, callbacks):
+        """resume the scan after a pause"""
         super().__init__(
             self.bec, request=request, report_instruction=report_instruction, callbacks=callbacks
         )
-        await self.process_request()
+        self.process_request()
 
     @property
     def devices(self):
         """get the devices for the callback"""
         if self.point_data.metadata["scan_type"] == "step":
             return self.get_devices_from_scan_data(self.scan_item.data[0])
         if self.point_data.metadata["scan_type"] == "fly":
@@ -126,50 +128,65 @@
         devices = [dev.name for dev in monitored_devices]
         devices = sort_devices(devices, scan_devices)
         if len(devices) > self.MAX_DEVICES:
             return devices[0 : self.MAX_DEVICES]
         return devices
 
     def _prepare_table(self) -> PrettyTable:
+        """Prepares the custom table for the live updates."""
         header = self._get_header()
         max_len = max(len(head) for head in header)
         return PrettyTable(header, padding=max_len)
 
     def _get_header(self) -> list:
+        """get the header for the table with up to self.MAX_DEVICES as entries
+
+        Returns:
+            list: header for the table
+        """
         header = ["seq. num"]
         for dev in self.devices:
             if dev in self.bec.device_manager.devices:
                 obj = self.bec.device_manager.devices[dev]
                 header.extend(obj._hints)
             else:
                 header.append(dev)
         return header
 
-    async def update_scan_item(self):
+    def update_scan_item(self, timeout: float = 15):
         """get the current scan item"""
+        start = time.time()
         while self.scan_queue_request.scan is None:
             self.check_alarms()
-            await asyncio.sleep(0.1)
+            time.sleep(0.1)
+            if time.time() - start > timeout:
+                raise TimeoutError("Could not find scan item.")
         self.scan_item = self.scan_queue_request.scan
 
-    async def core(self):
+    def core(self):
+        """core function to run the live updates for the table"""
         req_ID = self.scan_queue_request.requestID
         while True:
             request_block = [
                 req for req in self.scan_item.queue.request_blocks if req["RID"] == req_ID
             ][0]
             if not request_block["is_scan"]:
                 break
             if request_block["report_instructions"]:
                 break
             self.check_alarms()
 
-        await self._run_update(self.report_instruction[self.REPORT_TYPE])
+        self._run_update(self.report_instruction[self.REPORT_TYPE])
+
+    def _run_update(self, target_num_points: int):
+        """run the update loop with the progress bar
 
-    async def _run_update(self, target_num_points):
+        Args:
+            target_num_points (int): number of points to be collected
+        """
         with ScanProgressBar(
             scan_number=self.scan_item.scan_number, clear_on_exit=self._print_table_data
         ) as progressbar:
             while True:
                 self.check_alarms()
                 self.point_data = self.scan_item.data.get(self.point_id)
                 if self.scan_item.num_points:
@@ -184,25 +201,54 @@
                     progressbar.update(self.point_id)
 
                     # process sync callbacks
                     self.bec.callbacks.poll()
                     self.scan_item.poll_callbacks()
                 else:
                     logger.debug("waiting for new data point")
-                    await asyncio.sleep(0.1)
+                    time.sleep(0.1)
 
                 if not self.scan_item.num_points:
                     continue
 
                 if self.point_id == target_num_points:
                     break
                 if self.point_id > self.scan_item.num_points:
                     raise RuntimeError("Received more points than expected.")
 
+    @property
+    def _print_table_data(self) -> bool:
+        """Checks if the table should be printed or not.
+
+        Returns:
+            bool: True/False
+        """
+        if not self.__print_table_data:
+            return False
+        try:
+            # pylint: disable=protected-access
+            # pylint: disable=undefined-variable
+            if get_ipython().__class__.__name__ == "ZMQInteractiveShell":
+                self.__print_table_data = False
+                return False
+        except Exception:
+            pass
+        return self.__print_table_data
+
+    @_print_table_data.setter
+    def _print_table_data(self, value: bool):
+        """Set the print_table_data attribute.
+
+        Args:
+            value (bool): value to set
+        """
+        self.__print_table_data = value
+
     def print_table_data(self):
+        """print the table data for the current point_id"""
         if not self._print_table_data:
             return
 
         if not self.table:
             self.dev_values = (len(self._get_header()) - 1) * [0]
             self.table = self._prepare_table()
             print(self.table.get_header_lines())
@@ -240,42 +286,45 @@
                 else:
                     print_value = "N/A"
                 self.dev_values[ind] = print_value
                 ind += 1
         print(self.table.get_row(str(self.point_id), *self.dev_values))
 
     def close_table(self):
+        """close the table and print the footer"""
         if not self.table:
             return
         elapsed_time = self.scan_item.end_time - self.scan_item.start_time
         print(
             self.table.get_footer(
-                f"Scan {self.scan_item.scan_number} finished. Scan ID {self.scan_item.scanID}. Elapsed time: {elapsed_time:.2f} s"
+                f"Scan {self.scan_item.scan_number} finished. Scan ID {self.scan_item.scan_id}. Elapsed time: {elapsed_time:.2f} s"
             )
         )
 
-    async def process_request(self):
+    def process_request(self):
+        """process the request and start the core loop for live updates"""
         if self.request.content["scan_type"] == "close_scan_def":
-            await self.wait_for_scan_item_to_finish()
+            self.wait_for_scan_item_to_finish()
             self.close_table()
             return
 
-        await self.wait_for_request_acceptance()
-        await asyncio.wait_for(self.update_scan_item(), timeout=15)
-        await self.wait_for_scan_to_start()
+        self.wait_for_request_acceptance()
+        self.update_scan_item(timeout=15)
+        self.wait_for_scan_to_start()
 
         if self.table:
             self.table = None
         else:
             if self._print_table_data:
                 print(f"\nStarting scan {self.scan_item.scan_number}.")
 
-        await self.core()
+        self.core()
 
-    async def run(self):
+    def run(self):
+        """run the live updates"""
         if self.request.content["scan_type"] == "open_scan_def":
-            await self.wait_for_request_acceptance()
+            self.wait_for_request_acceptance()
             return
-        await self.process_request()
-        await self.wait_for_scan_item_to_finish()
+        self.process_request()
+        self.wait_for_scan_item_to_finish()
         if self._print_table_data:
             self.close_table()
```

### Comparing `bec_ipython_client-1.9.0/bec_client/callbacks/move_device.py` & `bec_ipython_client-2.4.2/bec_ipython_client/callbacks/move_device.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,40 @@
 from __future__ import annotations
 
 from collections.abc import Callable
 from typing import TYPE_CHECKING
 
 import numpy as np
 
-from bec_client.progressbar import DeviceProgressBar
+from bec_ipython_client.progressbar import DeviceProgressBar
 from bec_lib import DeviceManagerBase, MessageEndpoints, messages
 
 from .utils import LiveUpdatesBase, check_alarms
 
 if TYPE_CHECKING:
-    from bec_client.bec_client import BECClient
+    from bec_lib.client import BECClient
 
 
 class ReadbackDataMixin:
-    def __init__(self, device_manager: DeviceManagerBase, devices) -> None:
+    def __init__(self, device_manager: DeviceManagerBase, devices: list) -> None:
+        """Mixin to get the current device values and request-done messages.
+
+        Args:
+            device_manager (DeviceManagerBase): device manager
+            devices (list): list of devices to monitor
+        """
         self.device_manager = device_manager
         self.devices = devices
 
-    def get_device_values(self):
-        """get the current device values"""
+    def get_device_values(self) -> list:
+        """get the current device values
+
+        Returns:
+            list: list of device values
+        """
         values = []
         for dev in self.devices:
             val = self.device_manager.devices[dev].read(cached=True)
             if not val:
                 values.append(np.nan)
                 continue
             # pylint: disable=protected-access
@@ -34,24 +44,28 @@
                 values.append(val.get(hints[0]).get("value"))
             else:
                 values.append(val.get(list(val.keys())[0]).get("value"))
         return values
 
     def get_request_done_msgs(self):
         """get all request-done messages"""
-        pipe = self.device_manager.producer.pipeline()
+        pipe = self.device_manager.connector.pipeline()
         for dev in self.devices:
-            self.device_manager.producer.get(MessageEndpoints.device_req_status(dev), pipe)
-        return self.device_manager.producer.execute_pipeline(pipe)
+            self.device_manager.connector.get(MessageEndpoints.device_req_status(dev), pipe)
+        return self.device_manager.connector.execute_pipeline(pipe)
+
+    def wait_for_RID(self, request: messages.ScanQueueMessage) -> None:
+        """wait for the readback's metadata to match the request ID
 
-    def wait_for_RID(self, request):
-        """wait for the readback's metadata to match the request ID"""
+        Args:
+            request (messages.ScanQueueMessage): request message
+        """
         while True:
             msgs = [
-                self.device_manager.producer.get(MessageEndpoints.device_readback(dev))
+                self.device_manager.connector.get(MessageEndpoints.device_readback(dev))
                 for dev in self.devices
             ]
             if all(msg.metadata.get("RID") == request.metadata["RID"] for msg in msgs if msg):
                 break
             check_alarms(self.device_manager.parent)
 
 
@@ -75,18 +89,19 @@
             bec, report_instruction=report_instruction, request=request, callbacks=callbacks
         )
         if report_instruction:
             self.devices = report_instruction["readback"]["devices"]
         else:
             self.devices = list(request.content["parameter"]["args"].keys())
 
-    async def core(self):
+    def core(self):
+        """core function to monitor the device values and update the progressbar accordingly."""
         data_source = ReadbackDataMixin(self.bec.device_manager, self.devices)
         start_values = data_source.get_device_values()
-        await self.wait_for_request_acceptance()
+        self.wait_for_request_acceptance()
         data_source.wait_for_RID(self.request)
         if self.report_instruction:
             self.devices = self.report_instruction["readback"]["devices"]
             target_values = self.report_instruction["readback"]["end"]
 
             start_instr = self.report_instruction["readback"].get("start")
             if start_instr:
@@ -111,19 +126,22 @@
 
                 msgs = data_source.get_request_done_msgs()
                 request_ids = [
                     msg.metadata["RID"] if (msg and msg.metadata.get("RID")) else None
                     for msg in msgs
                 ]
                 if set(request_ids) != set([self.request.metadata["RID"]]):
-                    await progress.sleep()
+                    progress.sleep()
                     continue
 
                 req_done = True
                 for dev, msg in zip(self.devices, msgs):
                     if not msg:
                         continue
                     if msg.content.get("success", False):
                         progress.set_finished(dev)
+                # pylint: disable=protected-access
+                progress._progress.refresh()
 
-    async def run(self):
-        await self.core()
+    def run(self):
+        """run the progressbar."""
+        self.core()
```

### Comparing `bec_ipython_client-1.9.0/bec_client/callbacks/utils.py` & `bec_ipython_client-2.4.2/bec_ipython_client/callbacks/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 from __future__ import annotations
 
 import abc
-import asyncio
 import threading
 import time
 import traceback
 from collections.abc import Callable
 from typing import TYPE_CHECKING
 
 from bec_lib import bec_logger, messages
 from bec_lib.request_items import RequestItem
 
 if TYPE_CHECKING:
-    from bec_client.bec_client import BECClient
+    from bec_lib.client import BECClient
 
 logger = bec_logger.logger
 
 
 class ScanRequestError(Exception):
-    pass
+    """Error raised when a scan request is rejected"""
 
 
 def set_event_delayed(event: threading.Event, delay: int) -> None:
     """Set event with a delay
 
     Args:
         event (threading.Event): event that should be set
@@ -47,26 +46,34 @@
     def __init__(
         self,
         bec: BECClient,
         report_instruction: dict = None,
         request: messages.ScanQueueMessage = None,
         callbacks: list[Callable] = None,
     ) -> None:
+        """Base class for live updates
+
+        Args:
+            bec (BECClient): BECClient instance
+            report_instruction (dict, optional): report instruction. Defaults to None.
+            request (messages.ScanQueueMessage, optional): scan queue request. Defaults to None.
+            callbacks (list[Callable], optional): list of callback functions. Defaults to None.
+        """
         self.bec = bec
         self.request = request
         self.RID = request.metadata["RID"]
         self.scan_queue_request = None
         self.report_instruction = report_instruction
         if callbacks is None:
             self.callbacks = []
         self.callbacks = callbacks if isinstance(callbacks, list) else [callbacks]
 
-    async def wait_for_request_acceptance(self):
+    def wait_for_request_acceptance(self):
         scan_request = ScanRequestMixin(self.bec, self.RID)
-        await scan_request.wait()
+        scan_request.wait()
         self.scan_queue_request = scan_request.scan_queue_request
 
     @abc.abstractmethod
     def run(self):
         pass
 
     def emit_point(self, data: dict, metadata: dict = None):
@@ -78,51 +85,61 @@
             except Exception:
                 content = traceback.format_exc()
                 logger.warning(f"Failed to run callback function: {content}")
 
 
 class ScanRequestMixin:
     def __init__(self, bec: BECClient, RID: str) -> None:
+        """Mixin to handle scan request acceptance
+
+        Args:
+            bec (BECClient): BECClient instance
+            RID (str): request ID
+        """
         self.bec = bec
         self.request_storage = self.bec.queue.request_storage
         self.RID = RID
         self.scan_queue_request = None
 
-    async def _wait_for_scan_request(self) -> RequestItem:
-        """wait for scan queuest"""
+    def _wait_for_scan_request(self) -> RequestItem:
+        """wait for scan queuest
+
+        Returns:
+            RequestItem: scan queue request
+        """
         logger.debug("Waiting for request ID")
         start = time.time()
         while self.request_storage.find_request_by_ID(self.RID) is None:
-            await asyncio.sleep(0.1)
+            time.sleep(0.1)
             check_alarms(self.bec)
         logger.debug(f"Waiting for request ID finished after {time.time()-start} s.")
         return self.request_storage.find_request_by_ID(self.RID)
 
-    async def _wait_for_scan_request_decision(self):
+    def _wait_for_scan_request_decision(self):
         """wait for a scan queuest decision"""
         logger.debug("Waiting for decision")
         start = time.time()
         while self.scan_queue_request.decision_pending:
-            await asyncio.sleep(0.1)
+            time.sleep(0.1)
             check_alarms(self.bec)
         logger.debug(f"Waiting for decision finished after {time.time()-start} s.")
 
-    async def wait(self):
+    def wait(self):
         """wait for the request acceptance"""
-        self.scan_queue_request = await self._wait_for_scan_request()
+        self.scan_queue_request = self._wait_for_scan_request()
 
-        await self._wait_for_scan_request_decision()
+        self._wait_for_scan_request_decision()
         check_alarms(self.bec)
 
         while self.scan_queue_request.accepted is None:
-            await asyncio.sleep(0.01)
+            time.sleep(0.1)
             check_alarms(self.bec)
 
         if not self.scan_queue_request.accepted[0]:
             raise ScanRequestError(
                 "Scan was rejected by the server:"
                 f" {self.scan_queue_request.response.content.get('message')}"
             )
 
         while self.scan_queue_request.queue is None:
-            await asyncio.sleep(0.01)
+            time.sleep(0.1)
             check_alarms(self.bec)
```

### Comparing `bec_ipython_client-1.9.0/bec_client/high_level_interfaces/spec_hli.py` & `bec_ipython_client-2.4.2/bec_ipython_client/high_level_interfaces/spec_hli.py`

 * *Files 26% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         steps=steps,
         exp_time=exp_time,
         relative=True,
         **kwargs
     )
 
 
-def ascan(motor1, m1_from, m1_to, steps, exp_time, **kwargs):
+def ascan(motor1, m1_from, m1_to, steps, exp_time, **kwargs) -> ScanReport:
     """Absolute line scan with one device.
 
     Args:
         motor1 (Device): Device that should be scanned.
         m1_from (float): Start position.
         m1_to (float): End position.
         steps (int): Number of steps.
@@ -88,15 +88,15 @@
         >>> ascan(dev.motor1, -5, 5, 10, 0.1)
     """
     return scans.line_scan(
         motor1, m1_from, m1_to, steps=steps, exp_time=exp_time, relative=False, **kwargs
     )
 
 
-def a2scan(motor1, m1_from, m1_to, motor2, m2_from, m2_to, steps, exp_time, **kwargs):
+def a2scan(motor1, m1_from, m1_to, motor2, m2_from, m2_to, steps, exp_time, **kwargs) -> ScanReport:
     """Absolute line scan with two devices.
 
     Args:
         motor1 (Device): First device that should be scanned.
         m1_from (float): Start position of the first device.
         m1_to (float): End position of the first device.
         motor2 (Device): Second device that should be scanned.
@@ -121,15 +121,17 @@
         steps=steps,
         exp_time=exp_time,
         relative=False,
         **kwargs
     )
 
 
-def dmesh(motor1, m1_from, m1_to, m1_steps, motor2, m2_from, m2_to, m2_steps, exp_time, **kwargs):
+def dmesh(
+    motor1, m1_from, m1_to, m1_steps, motor2, m2_from, m2_to, m2_steps, exp_time, **kwargs
+) -> ScanReport:
     """Relative mesh scan (grid scan) with two devices.
 
     Args:
         motor1 (Device): First device that should be scanned.
         m1_from (float): Start position of the first device relative to its current position.
         m1_to (float): End position of the first device relative to its current position.
         m1_steps (int): Number of steps for motor1.
@@ -155,15 +157,17 @@
         m2_to,
         m2_steps,
         exp_time=exp_time,
         relative=True,
     )
 
 
-def amesh(motor1, m1_from, m1_to, m1_steps, motor2, m2_from, m2_to, m2_steps, exp_time, **kwargs):
+def amesh(
+    motor1, m1_from, m1_to, m1_steps, motor2, m2_from, m2_to, m2_steps, exp_time, **kwargs
+) -> ScanReport:
     """Absolute mesh scan (grid scan) with two devices.
 
     Args:
         motor1 (Device): First device that should be scanned.
         m1_from (float): Start position of the first device.
         m1_to (float): End position of the first device.
         m1_steps (int): Number of steps for motor1.
@@ -187,59 +191,7 @@
         motor2,
         m2_from,
         m2_to,
         m2_steps,
         exp_time=exp_time,
         relative=False,
     )
-
-
-def umv(*args) -> ScanReport:
-    """Updated absolute move (i.e. blocking) for one or more devices.
-
-    Returns:
-        ScanReport: Status object.
-
-    Examples:
-        >>> umv(dev.samx, 1)
-        >>> umv(dev.samx, 1, dev.samy, 2)
-    """
-    return scans.umv(*args, relative=False)
-
-
-def umvr(*args) -> ScanReport:
-    """Updated relative move (i.e. blocking) for one or more devices.
-
-    Returns:
-        ScanReport: Status object.
-
-    Examples:
-        >>> umvr(dev.samx, 1)
-        >>> umvr(dev.samx, 1, dev.samy, 2)
-    """
-    return scans.umv(*args, relative=True)
-
-
-def mv(*args) -> ScanReport:
-    """Absolute move for one or more devices.
-
-    Returns:
-        ScanReport: Status object.
-
-    Examples:
-        >>> mv(dev.samx, 1)
-        >>> mv(dev.samx, 1, dev.samy, 2)
-    """
-    return scans.mv(*args, relative=False)
-
-
-def mvr(*args) -> ScanReport:
-    """Relative move for one or more devices.
-
-    Returns:
-        ScanReport: Status object.
-
-    Examples:
-        >>> mvr(dev.samx, 1)
-        >>> mvr(dev.samx, 1, dev.samy, 2)
-    """
-    return scans.mv(*args, relative=True)
```

### Comparing `bec_ipython_client-1.9.0/bec_client/plugins/LamNI/lamni_optics_mixin.py` & `bec_ipython_client-2.4.2/bec_ipython_client/plugins/LamNI/lamni_optics_mixin.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import builtins
 import time
 
 from rich import box
 from rich.console import Console
 from rich.table import Table
 
-from bec_client.plugins.cSAXS import epics_get, epics_put, fshclose
+from bec_ipython_client.plugins.cSAXS import epics_put, fshclose
 
 # import builtins to avoid linter errors
 dev = builtins.__dict__.get("dev")
 umv = builtins.__dict__.get("umv")
 bec = builtins.__dict__.get("bec")
```

### Comparing `bec_ipython_client-1.9.0/bec_client/plugins/LamNI/load_additional_correction.py` & `bec_ipython_client-2.4.2/bec_ipython_client/plugins/LamNI/load_additional_correction.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 def lamni_read_additional_correction():
     # "additional_correction_shift"
     # [0][] x , [1][] y, [2][] angle, [3][0] number of elements
-    import numpy as np
 
     with open("correction_lamni_um_S01405_.txt", "r") as f:
         num_elements = f.readline()
         int_num_elements = int(num_elements.split(" ")[2])
         print(int_num_elements)
         corr_pos_x = []
         corr_pos_y = []
```

### Comparing `bec_ipython_client-1.9.0/bec_client/plugins/LamNI/x_ray_eye_align.py` & `bec_ipython_client-2.4.2/bec_ipython_client/plugins/LamNI/x_ray_eye_align.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from collections import defaultdict
 from pathlib import Path
 
 import h5py
 import numpy as np
 from typeguard import typechecked
 
-from bec_client.plugins.cSAXS import epics_get, epics_put, fshclose, fshopen
+from bec_ipython_client.plugins.cSAXS import epics_get, epics_put, fshopen
 from bec_lib import bec_logger
 from bec_lib.alarm_handler import AlarmBase
 from bec_lib.pdf_writer import PDFWriter
 
 from .lamni_optics_mixin import LamNIOpticsMixin
 
 logger = bec_logger.logger
@@ -327,15 +327,15 @@
 
         self.client.set_global_var("tomo_fov_offset", self.shift_xy)
 
     def write_output(self):
         with open(
             os.path.expanduser("~/Data10/specES1/internal/xrayeye_alignmentvalues"), "w"
         ) as alignment_values_file:
-            alignment_values_file.write(f"angle\thorizontal\tvertical\n")
+            alignment_values_file.write("angle\thorizontal\tvertical\n")
             for k in range(2, 11):
                 fovx_offset = (self.alignment_values[0][0] - self.alignment_values[k][0]) * 1000
                 fovy_offset = (self.alignment_values[k][1] - self.alignment_values[0][1]) * 1000
                 print(
                     f"Writing to file new alignment: number {k}, value x {fovx_offset}, y"
                     f" {fovy_offset}"
                 )
@@ -1090,15 +1090,15 @@
         last_scan_number = bec.queue.next_scan_number - 1
         ptycho_queue_file = os.path.abspath(
             os.path.join(ptycho_queue_path, f"scan_{last_scan_number:05d}.dat")
         )
         with open(ptycho_queue_file, "w") as queue_file:
             scans = " ".join([str(scan) for scan in self._current_scan_list])
             queue_file.write(f"p.scan_number {scans}\n")
-            queue_file.write(f"p.check_nextscan_started 1\n")
+            queue_file.write("p.check_nextscan_started 1\n")
 
     def write_pdf_report(self):
         """create and write the pdf report with the current LamNI settings"""
         dev = builtins.__dict__.get("dev")
         header = (
             " \n" * 3
             + "  :::            :::       :::   :::   ::::    ::: ::::::::::: \n"
```

### Comparing `bec_ipython_client-1.9.0/bec_client/plugins/SLS/sls_info.py` & `bec_ipython_client-2.4.2/bec_ipython_client/plugins/SLS/sls_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import builtins
 
 from rich import box
 from rich.table import Table
 
-from bec_client.beamline_mixin import BeamlineShowInfo
+from bec_ipython_client.beamline_mixin import BeamlineShowInfo
 
 
 class SLSInfo(BeamlineShowInfo):
     def _get_sls_info(self) -> dict:
         dev = builtins.__dict__.get("dev")
         info = dev.sls_info.read(cached=True)
         return info
```

### Comparing `bec_ipython_client-1.9.0/bec_client/plugins/XTreme/x-treme.py` & `bec_ipython_client-2.4.2/bec_ipython_client/plugins/XTreme/x-treme.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-1.9.0/bec_client/plugins/cSAXS/beamline_info.py` & `bec_ipython_client-2.4.2/bec_ipython_client/plugins/cSAXS/beamline_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import builtins
 
 from rich import box
 from rich.table import Table
 
-from bec_client.beamline_mixin import BeamlineShowInfo
+from bec_ipython_client.beamline_mixin import BeamlineShowInfo
 
 
 class BeamlineInfo(BeamlineShowInfo):
     def show(self):
         """Display information about the current beamline status"""
         console = self._get_console()
```

### Comparing `bec_ipython_client-1.9.0/bec_client/prettytable.py` & `bec_ipython_client-2.4.2/bec_ipython_client/prettytable.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-1.9.0/bec_client/progressbar.py` & `bec_ipython_client-2.4.2/bec_ipython_client/progressbar.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,25 @@
 import abc
-import asyncio
+import time
 from typing import Any
 
 import numpy as np
 import rich.progress
 from rich.text import Text
 
+from bec_lib import bec_logger
+
+logger = bec_logger.logger
+
 
 class MoveTaskProgressColumn(rich.progress.TaskProgressColumn):
+    """Custom progress column for the move device progress bar"""
+
     def render(self, task) -> Text:
+        """Renders the text for the progress bar"""
         if task.total is None and self.show_speed:
             return self.render_speed(task.finished_speed or task.speed)
         if task.fields.get("fields"):
             _text = f"[progress.percentage]{task.fields['fields'].get('current_pos'):10.2f} / {task.fields['fields'].get('target_pos'):10.2f} / {task.percentage:>3.0f} %"
         else:
             _text = f"[progress.percentage]{task.percentage:>3.0f}%"
         if self.markup:
@@ -21,15 +28,18 @@
             text = Text(_text, style=self.style, justify=self.justify)
         if self.highlighter:
             self.highlighter.highlight(text)
         return text
 
 
 class ScanTaskProgressColumn(rich.progress.TaskProgressColumn):
+    """Custom progress column for the scan progress bar"""
+
     def render(self, task) -> Text:
+        """Renders the text for the progress bar"""
         if task.total is None and self.show_speed:
             return self.render_speed(task.finished_speed or task.speed)
         if task.fields.get("fields"):
             _text = f"[progress.percentage]{int(task.fields['fields'].get('current_scan_pos'))} / {task.percentage:>3.0f} %"
         else:
             _text = f"[progress.percentage]{task.percentage:>3.0f}%"
         if self.markup:
@@ -70,159 +80,229 @@
         Returns:
             tuple[rich.progress.ProgressColumn, ...]: columns
         """
         return rich.progress.Progress.get_default_columns()
 
     def start(self) -> None:
         """Start the Progress handler and initialize the tasks."""
-        self._progress = rich.progress.Progress(*self.columns, transient=self.clear_on_exit)
+        self._progress = rich.progress.Progress(
+            *self.columns, transient=self.clear_on_exit, auto_refresh=False
+        )
         self._progress.start()
         self._init_tasks()
+        self._progress.refresh()
 
-    async def sleep(self):
-        await asyncio.sleep(1 / self.UPDATE_FREQUENCY)
+    def sleep(self):
+        """Sleep for a short time to avoid busy waiting."""
+        time.sleep(1 / self.UPDATE_FREQUENCY)
 
     def stop(self) -> None:
         """Stop the Progress handler"""
         self._progress.stop()
 
     @abc.abstractmethod
     def _init_tasks(self) -> None:
-        """Initialize tasks by appending new items to self._progress"""
+        """Initialize tasks by appending new items to self._progress."""
 
     @property
     def finished(self) -> bool:
         """True if all tasks have been completed.
 
         Returns:
             bool: True if all tasks have been completed.
         """
         return self._progress.finished
 
     @abc.abstractmethod
     def _update_task(self, task: int, value: Any) -> None:
-        """Update routine that is applied to each tasks during self.update calls
+        """Update routine that is applied to each tasks during self.update calls.
 
         Args:
             task (int): task ID
             value (Any): updated value received from self.update
 
         """
 
-    def update(self, values):
+    def update(self, values: list):
+        """Update the progress bar with new values.
+
+        Args:
+            values (list): list of values to update the progress bar with.
+        """
         if not isinstance(values, list):
             values = [values]
         for i, task in enumerate(self._tasks):
             self._update_task(task=task, value=values[i])
 
     def __enter__(self):
+        """Start the progress bar when entering a context."""
         self.start()
         return self
 
     def __exit__(self, *args):
+        """Stop the progress bar when exiting a context."""
         self.stop()
 
 
 class ScanProgressBar(ProgressBarBase):
     def __init__(self, scan_number: int, clear_on_exit=False) -> None:
+        """Progress bar for a scan.
+
+        Args:
+            scan_number (int): scan number
+            clear_on_exit (bool, optional): remove progress bar after completion. Defaults to False.
+        """
         super().__init__(clear_on_exit)
         self._max_points = None
         self.scan_number = scan_number
 
     @property
     def columns(self) -> tuple:
+        """Columns used for a new Progress instance.
+
+        Returns:
+            tuple: columns
+        """
         return (
             rich.progress.TextColumn("[progress.description]{task.description}"),
             rich.progress.BarColumn(),
             ScanTaskProgressColumn(),
             rich.progress.TimeRemainingColumn(),
             rich.progress.TimeElapsedColumn(),
         )
 
     def _init_tasks(self):
+        """Initialize tasks by appending new items to self._progress."""
         self._tasks.append(
             self._progress.add_task(f"[green] Scan {self.scan_number}: ", total=self.max_points)
         )
 
     def _update_tasks_total(self, max_points: int) -> None:
+        """Update the total number of steps for the progress bar.
+
+        Args:
+            max_points (int): total number of steps
+        """
         self._progress.tasks[0].total = max_points
 
     @property
     def max_points(self) -> int:
+        """Total number of steps for the progress bar.
+
+        Returns: int: total number of steps
+        """
         return self._max_points
 
     @max_points.setter
     def max_points(self, max_points: int) -> None:
+        """Setter for the total number of steps for the progress bar.
+
+        Args:
+            max_points (int): total number of steps
+        """
         self._max_points = max_points
         self._update_tasks_total(max_points)
 
     def _update_task(self, task: int, value):
+        """Update routine that is applied to each tasks during self.update calls.
+
+        Args:
+            task (int): task ID
+            value (Any): updated value received from self.update
+        """
         if self.max_points:
             self._progress.update(
                 self._tasks[task],
                 completed=value,
                 fields={"current_scan_pos": value},
+                refresh=True,
             )
+            self._progress.refresh()
         else:
             self._progress.update(
                 self._tasks[task],
                 fields={"current_scan_pos": value},
+                refresh=True,
             )
+            self._progress.refresh()
 
 
 class DeviceProgressBar(ProgressBarBase):
     def __init__(
         self,
         devices: list[str],
         target_values: list[float],
         start_values: list[float] = None,
         clear_on_exit: bool = False,
     ) -> None:
+        """Progress bar for moving devices.
+
+        Args:
+            devices (list[str]): list of device names
+            target_values (list[float]): list of target values
+            start_values (list[float], optional): list of start values. Defaults to None.
+            clear_on_exit (bool, optional): remove progress bar after completion. Defaults to False.
+        """
         self.target_values = target_values
         self.start_values = start_values
         self.devices = devices
 
         super().__init__(clear_on_exit)
 
         self._tasks = []
 
     @property
     def columns(self):
+        """Columns used for a new Progress instance."""
         return (
             rich.progress.TextColumn("[progress.description]{task.description}"),
             rich.progress.BarColumn(),
             MoveTaskProgressColumn(),
             rich.progress.TimeRemainingColumn(),
             rich.progress.TimeElapsedColumn(),
         )
 
     def _init_tasks(self):
+        """Initialize tasks by appending new items to self._progress."""
         for ii, dev in enumerate(self.devices):
             self._tasks.append(
                 self._progress.add_task(
                     f"[green] {dev}:{self.start_values[ii]:10.2f}", total=self.NUM_STEPS
                 )
             )
 
     def _update_task(self, task: Any, value: float) -> None:
+        """Update routine that is applied to each tasks during self.update calls.
+
+        Args:
+            task (Any): task ID
+            value (float): updated value received from self.update
+        """
         if self._progress.tasks[task].finished:
             return
 
         movement_range = self.target_values[task] - self.start_values[task]
         if np.abs(movement_range) > 0:
             completed = np.abs((value - self.start_values[task]) / movement_range * self.NUM_STEPS)
         else:
             completed = self.NUM_STEPS
         self._progress.update(
             task,
             completed=completed,
             fields={"current_pos": value, "target_pos": self.target_values[task]},
+            refresh=True,
         )
+        self._progress.refresh()
 
     def set_finished(self, device):
+        """Set a progressbar for a device as finished.
+
+        Args:
+            device (str): device name
+        """
         device_index = self.devices.index(device)
         self._progress.advance(self._tasks[device_index], self.NUM_STEPS)
 
 
 if __name__ == "__main__":
     pass
     # devices = ["samx", "samy"]
```

### Comparing `bec_ipython_client-1.9.0/bec_client/signals.py` & `bec_ipython_client-2.4.2/bec_ipython_client/signals.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-1.9.0/bec_ipython_client.egg-info/SOURCES.txt` & `bec_ipython_client-2.4.2/bec_ipython_client.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,44 @@
 setup.cfg
 setup.py
-./bec_client/__init__.py
-./bec_client/beamline_mixin.py
-./bec_client/bec_client.py
-./bec_client/bec_magics.py
-./bec_client/prettytable.py
-./bec_client/progressbar.py
-./bec_client/signals.py
-./bec_client/bin/__init__.py
-./bec_client/bin/bec_startup.py
-./bec_client/callbacks/__init__.py
-./bec_client/callbacks/ipython_live_updates.py
-./bec_client/callbacks/live_table.py
-./bec_client/callbacks/move_device.py
-./bec_client/callbacks/scan_progress.py
-./bec_client/callbacks/utils.py
-./bec_client/high_level_interfaces/__init__.py
-./bec_client/high_level_interfaces/spec_hli.py
-./bec_client/plugins/__init__.py
-./bec_client/plugins/LamNI/__init__.py
-./bec_client/plugins/LamNI/lamni_optics_mixin.py
-./bec_client/plugins/LamNI/load_additional_correction.py
-./bec_client/plugins/LamNI/x_ray_eye_align.py
-./bec_client/plugins/SLS/__init__.py
-./bec_client/plugins/SLS/sls_info.py
-./bec_client/plugins/XTreme/__init__.py
-./bec_client/plugins/XTreme/x-treme.py
-./bec_client/plugins/cSAXS/__init__.py
-./bec_client/plugins/cSAXS/beamline_info.py
-./bec_client/plugins/cSAXS/cSAXS_beamline.py
-bec_client/bin/bec
+./bec_ipython_client/__init__.py
+./bec_ipython_client/beamline_mixin.py
+./bec_ipython_client/bec_magics.py
+./bec_ipython_client/bec_startup.py
+./bec_ipython_client/main.py
+./bec_ipython_client/prettytable.py
+./bec_ipython_client/progressbar.py
+./bec_ipython_client/signals.py
+./bec_ipython_client/callbacks/__init__.py
+./bec_ipython_client/callbacks/ipython_live_updates.py
+./bec_ipython_client/callbacks/live_table.py
+./bec_ipython_client/callbacks/move_device.py
+./bec_ipython_client/callbacks/scan_progress.py
+./bec_ipython_client/callbacks/utils.py
+./bec_ipython_client/high_level_interfaces/__init__.py
+./bec_ipython_client/high_level_interfaces/bec_hli.py
+./bec_ipython_client/high_level_interfaces/spec_hli.py
+./bec_ipython_client/plugins/__init__.py
+./bec_ipython_client/plugins/LamNI/__init__.py
+./bec_ipython_client/plugins/LamNI/lamni_optics_mixin.py
+./bec_ipython_client/plugins/LamNI/load_additional_correction.py
+./bec_ipython_client/plugins/LamNI/x_ray_eye_align.py
+./bec_ipython_client/plugins/SLS/__init__.py
+./bec_ipython_client/plugins/SLS/sls_info.py
+./bec_ipython_client/plugins/XTreme/__init__.py
+./bec_ipython_client/plugins/XTreme/x-treme.py
+./bec_ipython_client/plugins/cSAXS/__init__.py
+./bec_ipython_client/plugins/cSAXS/beamline_info.py
+./bec_ipython_client/plugins/cSAXS/cSAXS_beamline.py
+./bec_ipython_client/plugins/cSAXS/csaxs_bl_checks.py
+./bec_ipython_client/plugins/flomni/__init__.py
+./bec_ipython_client/plugins/flomni/flomni.py
+./bec_ipython_client/plugins/flomni/flomni_optics_mixin.py
+./bec_ipython_client/plugins/flomni/x_ray_eye_align.py
+./bec_ipython_client/tests/__init__.py
+./bec_ipython_client/tests/end2end_fixtures.py
 bec_ipython_client.egg-info/PKG-INFO
 bec_ipython_client.egg-info/SOURCES.txt
 bec_ipython_client.egg-info/dependency_links.txt
+bec_ipython_client.egg-info/entry_points.txt
 bec_ipython_client.egg-info/requires.txt
 bec_ipython_client.egg-info/top_level.txt
```

### Comparing `bec_ipython_client-1.9.0/setup.cfg` & `bec_ipython_client-2.4.2/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 	Development Status :: 3 - Alpha
 	Topic :: Scientific/Engineering
 
 [options]
 package_dir = 
 	= .
 packages = find:
-python_requires = >=3.9
+python_requires = >=3.10
 
 [options.packages.find]
 where = .
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `bec_ipython_client-1.9.0/setup.py` & `bec_ipython_client-2.4.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 current_path = pathlib.Path(__file__).parent.resolve()
 
 bec_lib = f"{current_path}/../bec_lib/"
 
 
-__version__ = "1.9.0"
+__version__ = "2.4.2"
 
 
 def run_install(setup_args: dict, bec_deps: list, editable=False):
     """
     Run the setup function with the given arguments.
 
     Args:
@@ -38,37 +38,41 @@
     setup_args["install_requires"].extend(install_deps)
     print(setup_args)
     setup(**setup_args)
 
 
 if __name__ == "__main__":
     setup_args_in = {
-        "scripts": ["bec_client/bin/bec"],
+        "entry_points": {
+            "console_scripts": ["bec = bec_ipython_client.main:main"],
+            "pytest11": ["bec_lib_end2end_fixtures = bec_ipython_client.tests.end2end_fixtures"],
+        },
         "install_requires": [
             "numpy",
             "requests",
             "typeguard",
             "ipython",
             "rich",
             "pyepics",
             "h5py",
         ],
         "version": __version__,
         "extras_require": {
             "dev": [
                 "pytest",
                 "pytest-random-order",
-                "pytest-asyncio",
                 "pytest-timeout",
-                "flaky",
+                "pytest-retry",
+                "pytest-redis",
                 "coverage",
                 "black",
+                "isort",
                 "pylint",
             ]
         },
     }
     bec_deps_in = [("bec_lib", "bec_lib", bec_lib)]
-    is_local = os.path.dirname(os.path.abspath(__file__)).split("/")[-1] == "bec_client"
+    is_local = os.path.dirname(os.path.abspath(__file__)).split("/")[-1] == "bec_ipython_client"
     is_build = "bdist_wheel" in sys.argv
 
     editable_in = is_local and not is_build
     run_install(setup_args_in, bec_deps_in, editable=editable_in)
```

