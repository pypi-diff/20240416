# Comparing `tmp/bec_client-2.3.0.tar.gz` & `tmp/bec_client-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bec_client-2.3.0.tar", last modified: Fri Apr 12 15:46:45 2024, max compression
+gzip compressed data, was "bec_client-2.4.0.tar", last modified: Mon Apr 15 14:54:22 2024, max compression
```

## Comparing `bec_client-2.3.0.tar` & `bec_client-2.4.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 15:46:45.860102 bec_client-2.3.0/
--rw-r--r--   0 root         (0) root         (0)      406 2024-04-12 15:46:45.860102 bec_client-2.3.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 15:46:45.858101 bec_client-2.3.0/bec_client/
--rw-rw-rw-   0 root         (0) root         (0)       93 2024-04-10 11:18:35.000000 bec_client-2.3.0/bec_client/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1067 2024-04-10 11:18:35.000000 bec_client-2.3.0/bec_client/beamline_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     5750 2024-04-12 15:18:38.000000 bec_client-2.3.0/bec_client/bec_ipython_client.py
--rw-rw-rw-   0 root         (0) root         (0)     1972 2024-04-10 11:18:35.000000 bec_client-2.3.0/bec_client/bec_magics.py
--rw-rw-rw-   0 root         (0) root         (0)     1578 2024-04-12 15:18:38.000000 bec_client-2.3.0/bec_client/bec_startup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 15:46:45.859102 bec_client-2.3.0/bec_client/callbacks/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-12 15:46:36.000000 bec_client-2.3.0/bec_client/callbacks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9948 2024-04-10 11:18:35.000000 bec_client-2.3.0/bec_client/callbacks/ipython_live_updates.py
--rw-rw-rw-   0 root         (0) root         (0)    11955 2024-04-10 11:18:35.000000 bec_client-2.3.0/bec_client/callbacks/live_table.py
--rw-rw-rw-   0 root         (0) root         (0)     5502 2024-04-10 11:18:35.000000 bec_client-2.3.0/bec_client/callbacks/move_device.py
--rw-rw-rw-   0 root         (0) root         (0)     2202 2024-04-10 11:18:35.000000 bec_client-2.3.0/bec_client/callbacks/scan_progress.py
--rw-rw-rw-   0 root         (0) root         (0)     4475 2024-04-10 11:18:35.000000 bec_client-2.3.0/bec_client/callbacks/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 15:46:45.859102 bec_client-2.3.0/bec_client/high_level_interfaces/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-12 15:46:36.000000 bec_client-2.3.0/bec_client/high_level_interfaces/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1221 2024-04-12 15:18:38.000000 bec_client-2.3.0/bec_client/high_level_interfaces/bec_hli.py
--rw-rw-rw-   0 root         (0) root         (0)     5818 2024-04-12 15:18:38.000000 bec_client-2.3.0/bec_client/high_level_interfaces/spec_hli.py
--rw-rw-rw-   0 root         (0) root         (0)     2702 2024-04-12 15:05:02.000000 bec_client-2.3.0/bec_client/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 15:46:45.859102 bec_client-2.3.0/bec_client/plugins/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 15:46:45.859102 bec_client-2.3.0/bec_client/plugins/LamNI/
--rw-rw-rw-   0 root         (0) root         (0)      149 2024-04-10 11:18:35.000000 bec_client-2.3.0/bec_client/plugins/LamNI/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5508 2024-04-10 11:18:35.000000 bec_client-2.3.0/bec_client/plugins/LamNI/lamni_optics_mixin.py
--rwxrwxrwx   0 root         (0) root         (0)      872 2024-04-10 11:18:35.000000 bec_client-2.3.0/bec_client/plugins/LamNI/load_additional_correction.py
--rw-rw-rw-   0 root         (0) root         (0)    54693 2024-04-10 11:18:35.000000 bec_client-2.3.0/bec_client/plugins/LamNI/x_ray_eye_align.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 15:46:45.859102 bec_client-2.3.0/bec_client/plugins/SLS/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-12 15:46:36.000000 bec_client-2.3.0/bec_client/plugins/SLS/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4926 2024-04-10 11:18:35.000000 bec_client-2.3.0/bec_client/plugins/SLS/sls_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 15:46:45.859102 bec_client-2.3.0/bec_client/plugins/XTreme/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-12 15:46:36.000000 bec_client-2.3.0/bec_client/plugins/XTreme/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3631 2024-04-10 11:18:35.000000 bec_client-2.3.0/bec_client/plugins/XTreme/x-treme.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-12 15:46:36.000000 bec_client-2.3.0/bec_client/plugins/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 15:46:45.860102 bec_client-2.3.0/bec_client/plugins/cSAXS/
--rw-rw-rw-   0 root         (0) root         (0)      128 2024-04-10 11:18:35.000000 bec_client-2.3.0/bec_client/plugins/cSAXS/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4433 2024-04-10 11:18:35.000000 bec_client-2.3.0/bec_client/plugins/cSAXS/beamline_info.py
--rw-rw-rw-   0 root         (0) root         (0)      445 2024-04-10 11:18:35.000000 bec_client-2.3.0/bec_client/plugins/cSAXS/cSAXS_beamline.py
--rw-rw-rw-   0 root         (0) root         (0)     4308 2024-04-10 11:18:35.000000 bec_client-2.3.0/bec_client/plugins/cSAXS/csaxs_bl_checks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 15:46:45.860102 bec_client-2.3.0/bec_client/plugins/flomni/
--rw-rw-rw-   0 root         (0) root         (0)       27 2024-04-10 11:18:35.000000 bec_client-2.3.0/bec_client/plugins/flomni/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    77070 2024-04-12 15:18:38.000000 bec_client-2.3.0/bec_client/plugins/flomni/flomni.py
--rw-rw-rw-   0 root         (0) root         (0)     6391 2024-04-10 11:18:35.000000 bec_client-2.3.0/bec_client/plugins/flomni/flomni_optics_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     8902 2024-04-10 11:18:35.000000 bec_client-2.3.0/bec_client/plugins/flomni/x_ray_eye_align.py
--rw-rw-rw-   0 root         (0) root         (0)     2534 2024-04-10 11:18:35.000000 bec_client-2.3.0/bec_client/prettytable.py
--rw-rw-rw-   0 root         (0) root         (0)    11165 2024-04-10 11:18:35.000000 bec_client-2.3.0/bec_client/progressbar.py
--rw-rw-rw-   0 root         (0) root         (0)     4299 2024-04-10 11:18:35.000000 bec_client-2.3.0/bec_client/signals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 15:46:45.860102 bec_client-2.3.0/bec_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)      406 2024-04-12 15:46:45.000000 bec_client-2.3.0/bec_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1567 2024-04-12 15:46:45.000000 bec_client-2.3.0/bec_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 15:46:45.000000 bec_client-2.3.0/bec_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       45 2024-04-12 15:46:45.000000 bec_client-2.3.0/bec_client.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      162 2024-04-12 15:46:45.000000 bec_client-2.3.0/bec_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-04-12 15:46:45.000000 bec_client-2.3.0/bec_client.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      512 2024-04-12 15:46:45.861102 bec_client-2.3.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2117 2024-04-12 15:46:44.000000 bec_client-2.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 14:54:22.180040 bec_client-2.4.0/
+-rw-r--r--   0 root         (0) root         (0)      406 2024-04-15 14:54:22.180040 bec_client-2.4.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 14:54:22.178040 bec_client-2.4.0/bec_client/
+-rw-rw-rw-   0 root         (0) root         (0)       93 2024-04-15 13:12:21.000000 bec_client-2.4.0/bec_client/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1067 2024-04-15 13:12:21.000000 bec_client-2.4.0/bec_client/beamline_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     5750 2024-04-15 14:14:14.000000 bec_client-2.4.0/bec_client/bec_ipython_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     1972 2024-04-15 13:12:21.000000 bec_client-2.4.0/bec_client/bec_magics.py
+-rw-rw-rw-   0 root         (0) root         (0)     1578 2024-04-15 14:14:14.000000 bec_client-2.4.0/bec_client/bec_startup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 14:54:22.178040 bec_client-2.4.0/bec_client/callbacks/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-15 14:54:11.000000 bec_client-2.4.0/bec_client/callbacks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9948 2024-04-15 13:12:21.000000 bec_client-2.4.0/bec_client/callbacks/ipython_live_updates.py
+-rw-rw-rw-   0 root         (0) root         (0)    11955 2024-04-15 13:12:21.000000 bec_client-2.4.0/bec_client/callbacks/live_table.py
+-rw-rw-rw-   0 root         (0) root         (0)     5502 2024-04-15 13:12:21.000000 bec_client-2.4.0/bec_client/callbacks/move_device.py
+-rw-rw-rw-   0 root         (0) root         (0)     2202 2024-04-15 13:12:21.000000 bec_client-2.4.0/bec_client/callbacks/scan_progress.py
+-rw-rw-rw-   0 root         (0) root         (0)     4475 2024-04-15 13:12:21.000000 bec_client-2.4.0/bec_client/callbacks/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 14:54:22.179040 bec_client-2.4.0/bec_client/high_level_interfaces/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-15 14:54:11.000000 bec_client-2.4.0/bec_client/high_level_interfaces/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1221 2024-04-15 14:14:14.000000 bec_client-2.4.0/bec_client/high_level_interfaces/bec_hli.py
+-rw-rw-rw-   0 root         (0) root         (0)     5818 2024-04-15 14:14:14.000000 bec_client-2.4.0/bec_client/high_level_interfaces/spec_hli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2702 2024-04-15 14:14:14.000000 bec_client-2.4.0/bec_client/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 14:54:22.179040 bec_client-2.4.0/bec_client/plugins/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 14:54:22.179040 bec_client-2.4.0/bec_client/plugins/LamNI/
+-rw-rw-rw-   0 root         (0) root         (0)      149 2024-04-15 13:12:21.000000 bec_client-2.4.0/bec_client/plugins/LamNI/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5508 2024-04-15 13:12:21.000000 bec_client-2.4.0/bec_client/plugins/LamNI/lamni_optics_mixin.py
+-rwxrwxrwx   0 root         (0) root         (0)      872 2024-04-15 13:12:21.000000 bec_client-2.4.0/bec_client/plugins/LamNI/load_additional_correction.py
+-rw-rw-rw-   0 root         (0) root         (0)    54693 2024-04-15 13:12:21.000000 bec_client-2.4.0/bec_client/plugins/LamNI/x_ray_eye_align.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 14:54:22.179040 bec_client-2.4.0/bec_client/plugins/SLS/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-15 14:54:11.000000 bec_client-2.4.0/bec_client/plugins/SLS/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4926 2024-04-15 13:12:21.000000 bec_client-2.4.0/bec_client/plugins/SLS/sls_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 14:54:22.179040 bec_client-2.4.0/bec_client/plugins/XTreme/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-15 14:54:11.000000 bec_client-2.4.0/bec_client/plugins/XTreme/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3631 2024-04-15 13:12:21.000000 bec_client-2.4.0/bec_client/plugins/XTreme/x-treme.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-15 14:54:11.000000 bec_client-2.4.0/bec_client/plugins/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 14:54:22.180040 bec_client-2.4.0/bec_client/plugins/cSAXS/
+-rw-rw-rw-   0 root         (0) root         (0)      128 2024-04-15 13:12:21.000000 bec_client-2.4.0/bec_client/plugins/cSAXS/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4433 2024-04-15 13:12:21.000000 bec_client-2.4.0/bec_client/plugins/cSAXS/beamline_info.py
+-rw-rw-rw-   0 root         (0) root         (0)      445 2024-04-15 13:12:21.000000 bec_client-2.4.0/bec_client/plugins/cSAXS/cSAXS_beamline.py
+-rw-rw-rw-   0 root         (0) root         (0)     4308 2024-04-15 13:12:21.000000 bec_client-2.4.0/bec_client/plugins/cSAXS/csaxs_bl_checks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 14:54:22.180040 bec_client-2.4.0/bec_client/plugins/flomni/
+-rw-rw-rw-   0 root         (0) root         (0)       27 2024-04-15 13:12:21.000000 bec_client-2.4.0/bec_client/plugins/flomni/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    80368 2024-04-15 14:54:11.000000 bec_client-2.4.0/bec_client/plugins/flomni/flomni.py
+-rw-rw-rw-   0 root         (0) root         (0)     6391 2024-04-15 13:12:21.000000 bec_client-2.4.0/bec_client/plugins/flomni/flomni_optics_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     8902 2024-04-15 13:12:21.000000 bec_client-2.4.0/bec_client/plugins/flomni/x_ray_eye_align.py
+-rw-rw-rw-   0 root         (0) root         (0)     2534 2024-04-15 13:12:21.000000 bec_client-2.4.0/bec_client/prettytable.py
+-rw-rw-rw-   0 root         (0) root         (0)    11165 2024-04-15 13:12:21.000000 bec_client-2.4.0/bec_client/progressbar.py
+-rw-rw-rw-   0 root         (0) root         (0)     4299 2024-04-15 13:12:21.000000 bec_client-2.4.0/bec_client/signals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 14:54:22.180040 bec_client-2.4.0/bec_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      406 2024-04-15 14:54:22.000000 bec_client-2.4.0/bec_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1567 2024-04-15 14:54:22.000000 bec_client-2.4.0/bec_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-15 14:54:22.000000 bec_client-2.4.0/bec_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2024-04-15 14:54:22.000000 bec_client-2.4.0/bec_client.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      162 2024-04-15 14:54:22.000000 bec_client-2.4.0/bec_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-04-15 14:54:22.000000 bec_client-2.4.0/bec_client.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      512 2024-04-15 14:54:22.181041 bec_client-2.4.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2117 2024-04-15 14:54:20.000000 bec_client-2.4.0/setup.py
```

### Comparing `bec_client-2.3.0/bec_client/beamline_mixin.py` & `bec_client-2.4.0/bec_client/beamline_mixin.py`

 * *Files identical despite different names*

### Comparing `bec_client-2.3.0/bec_client/bec_ipython_client.py` & `bec_client-2.4.0/bec_client/bec_ipython_client.py`

 * *Files identical despite different names*

### Comparing `bec_client-2.3.0/bec_client/bec_magics.py` & `bec_client-2.4.0/bec_client/bec_magics.py`

 * *Files identical despite different names*

### Comparing `bec_client-2.3.0/bec_client/bec_startup.py` & `bec_client-2.4.0/bec_client/bec_startup.py`

 * *Files identical despite different names*

### Comparing `bec_client-2.3.0/bec_client/callbacks/ipython_live_updates.py` & `bec_client-2.4.0/bec_client/callbacks/ipython_live_updates.py`

 * *Files identical despite different names*

### Comparing `bec_client-2.3.0/bec_client/callbacks/live_table.py` & `bec_client-2.4.0/bec_client/callbacks/live_table.py`

 * *Files identical despite different names*

### Comparing `bec_client-2.3.0/bec_client/callbacks/move_device.py` & `bec_client-2.4.0/bec_client/callbacks/move_device.py`

 * *Files identical despite different names*

### Comparing `bec_client-2.3.0/bec_client/callbacks/scan_progress.py` & `bec_client-2.4.0/bec_client/callbacks/scan_progress.py`

 * *Files identical despite different names*

### Comparing `bec_client-2.3.0/bec_client/callbacks/utils.py` & `bec_client-2.4.0/bec_client/callbacks/utils.py`

 * *Files identical despite different names*

### Comparing `bec_client-2.3.0/bec_client/high_level_interfaces/bec_hli.py` & `bec_client-2.4.0/bec_client/high_level_interfaces/bec_hli.py`

 * *Files identical despite different names*

### Comparing `bec_client-2.3.0/bec_client/high_level_interfaces/spec_hli.py` & `bec_client-2.4.0/bec_client/high_level_interfaces/spec_hli.py`

 * *Files identical despite different names*

### Comparing `bec_client-2.3.0/bec_client/main.py` & `bec_client-2.4.0/bec_client/main.py`

 * *Files identical despite different names*

### Comparing `bec_client-2.3.0/bec_client/plugins/LamNI/lamni_optics_mixin.py` & `bec_client-2.4.0/bec_client/plugins/LamNI/lamni_optics_mixin.py`

 * *Files identical despite different names*

### Comparing `bec_client-2.3.0/bec_client/plugins/LamNI/load_additional_correction.py` & `bec_client-2.4.0/bec_client/plugins/LamNI/load_additional_correction.py`

 * *Files identical despite different names*

### Comparing `bec_client-2.3.0/bec_client/plugins/LamNI/x_ray_eye_align.py` & `bec_client-2.4.0/bec_client/plugins/LamNI/x_ray_eye_align.py`

 * *Files identical despite different names*

### Comparing `bec_client-2.3.0/bec_client/plugins/SLS/sls_info.py` & `bec_client-2.4.0/bec_client/plugins/SLS/sls_info.py`

 * *Files identical despite different names*

### Comparing `bec_client-2.3.0/bec_client/plugins/XTreme/x-treme.py` & `bec_client-2.4.0/bec_client/plugins/XTreme/x-treme.py`

 * *Files identical despite different names*

### Comparing `bec_client-2.3.0/bec_client/plugins/cSAXS/beamline_info.py` & `bec_client-2.4.0/bec_client/plugins/cSAXS/beamline_info.py`

 * *Files identical despite different names*

### Comparing `bec_client-2.3.0/bec_client/plugins/cSAXS/csaxs_bl_checks.py` & `bec_client-2.4.0/bec_client/plugins/cSAXS/csaxs_bl_checks.py`

 * *Files identical despite different names*

### Comparing `bec_client-2.3.0/bec_client/plugins/flomni/flomni.py` & `bec_client-2.4.0/bec_client/plugins/flomni/flomni.py`

 * *Files 4% similar despite different names*

```diff
@@ -1122,14 +1122,15 @@
         self._beam_is_okay = True
         self._stop_beam_check_event = None
         self.beam_check_thread = None
         self.corr_pos_y = []
         self.corr_angle_y = []
         self.corr_pos_y_2 = []
         self.corr_angle_y_2 = []
+        self.progress = {}
         self.align = XrayEyeAlign(self.client, self)
 
     def start_x_ray_eye_alignment(self):
         user_input = input(
             "Starting Xrayeye alignment. Deleting any potential existing alignment for this sample. [Y/n]"
         )
         if user_input == "y" or user_input == "":
@@ -1514,21 +1515,30 @@
             num=int(180 / self.tomo_angle_stepsize) + 1,
             endpoint=True,
         )
         # reverse even sub-tomograms
         if not (subtomo_number % 2):
             angles = np.flip(angles)
         for angle in angles:
+            self.progress["subtomo"] = subtomo_number
+            self.progress["subtomo_projection"] = angles.index(angle)
+            self.progress["subtomo_total_projections"] = 180 / self.tomo_angle_stepsize
+            self.progress["projection"] = (subtomo_number - 1) * self.progress[
+                "subtomo_total_projections"
+            ] + self.progress["subtomo_projection"]
+            self.progress["total_projections"] = 180 / self.tomo_angle_stepsize * 8
+            self.progress["angle"] = angle
             self._tomo_scan_at_angle(angle, subtomo_number)
 
     def _tomo_scan_at_angle(self, angle, subtomo_number):
         successful = False
         error_caught = False
         if 0 <= angle < 180.05:
             print(f"Starting flOMNI scan for angle {angle} in subtomo {subtomo_number}")
+            self._print_progress()
             while not successful:
                 self._start_beam_check()
                 if not self.special_angles:
                     self._current_special_angles = []
                 if self._current_special_angles:
                     next_special_angle = self._current_special_angles[0]
                     if np.isclose(angle, next_special_angle, atol=0.5):
@@ -1558,33 +1568,40 @@
                 self._write_tomo_scan_number(scan_nr, angle, subtomo_number)
 
     def tomo_scan(self, subtomo_start=1, start_angle=None, projection_number=None):
         """start a tomo scan"""
         bec = builtins.__dict__.get("bec")
         scans = builtins.__dict__.get("scans")
         self._current_special_angles = self.special_angles.copy()
+        # a new tomo scan was started
+        if (
+            (self.tomo_type == 1 and subtomo_start == 1 and start_angle is None)
+            or (self.tomo_type == 2 and projection_number == None)
+            or (self.tomo_type == 3 and projection_number == None)
+        ):
 
-        if subtomo_start == 1 and start_angle is None:
             # pylint: disable=undefined-variable
             if bec.active_account != "":
                 self.tomo_id = self.add_sample_database(
                     self.sample_name,
                     str(datetime.date.today()),
                     bec.active_account.decode(),
                     bec.queue.next_scan_number,
                     "flomni",
                     "test additional info",
                     "BEC",
                 )
                 self.write_pdf_report()
             else:
                 self.tomo_id = 0
+
         with scans.dataset_id_on_hold:
             if self.tomo_type == 1:
                 # 8 equally spaced sub-tomograms
+                self.progress["tomo_type"] = "Equally spaced sub-tomograms"
                 for ii in range(subtomo_start, 9):
                     self.sub_tomo_scan(ii, start_angle=start_angle)
                     start_angle = None
 
             elif self.tomo_type == 2:
                 # Golden ratio tomography
                 previous_subtomo_number = -1
@@ -1599,14 +1616,32 @@
                         if (
                             subtomo_number % 2 == 1
                             and ii > 10
                             and self.golden_projections_at_0_deg_for_damage_estimation == 1
                         ):
                             self._tomo_scan_at_angle(0, subtomo_number)
                         previous_subtomo_number = subtomo_number
+                    self.progress["tomo_type"] = "Golden ratio tomography"
+                    self.progress["subtomo"] = subtomo_number
+                    self.progress["projection"] = ii
+                    self.progress["angle"] = angle
+                    if self.golden_ratio_bunch_size > 0:
+                        self.progress["subtomo_total_projections"] = self.golden_ratio_bunch_size
+                        self.progress["subtomo_projection"] = (
+                            ii - (subtomo_number - 1) * self.golden_ratio_bunch_size
+                        )
+                    else:
+                        self.progress["subtomo_total_projections"] = 0
+                        self.progress["subtomo_projection"] = 0
+
+                    if self.golden_max_number_of_projections > 0:
+                        self.progress["total_projections"] = self.golden_max_number_of_projections
+                    else:
+                        self.progress["total_projections"] = 0
+
                     self._tomo_scan_at_angle(angle, subtomo_number)
                     ii += 1
                     if (
                         ii > self.golden_max_number_of_projections
                         and self.golden_max_number_of_projections > 0
                     ):
                         print(
@@ -1629,27 +1664,52 @@
                         if (
                             subtomo_number % 2 == 1
                             and ii > 10
                             and self.golden_projections_at_0_deg_for_damage_estimation == 1
                         ):
                             self._tomo_scan_at_angle(0, subtomo_number)
                         previous_subtomo_number = subtomo_number
+                    self.progress["tomo_type"] = (
+                        "Equally spaced tomography, golden ratio starting angle"
+                    )
+                    self.progress["subtomo"] = subtomo_number
+                    self.progress["projection"] = ii
+                    self.progress["angle"] = angle
+
+                    self.progress["subtomo_total_projections"] = 180 / self.tomo_angle_stepsize
+                    self.progress["subtomo_projection"] = (
+                        ii - (subtomo_number - 1) * self.progress["subtomo_total_projections"]
+                    )
+
+                    if self.golden_max_number_of_projections > 0:
+                        self.progress["total_projections"] = self.golden_max_number_of_projections
+                    else:
+                        self.progress["total_projections"] = 0
                     self._tomo_scan_at_angle(angle, subtomo_number)
                     ii += 1
                     if (
                         ii > self.golden_max_number_of_projections
                         and self.golden_max_number_of_projections > 0
                     ):
                         print(
                             f"Golden ratio tomography stopped automatically after the requested {self.golden_max_number_of_projections} projections"
                         )
                         break
             else:
                 raise FlomniError("undefined tomo type")
 
+    def _print_progress(self):
+        print("\x1b[95mProgress report:")
+        print(f"Tomo type: ....................... {self.progress['tomo_type']}")
+        print(f"Projection: ...................... {self.progress['projection']}")
+        print(f"Total projections expected ....... {self.progress['total_projections']}")
+        print(f"Angle: ........................... {self.progress['angle']}")
+        print(f"Current subtomo: ................. {self.progress['subtomo']}")
+        print(f"Current projection within subtomo: {self.progress['subtomo_projection']}\x1b[0m")
+
     def add_sample_database(
         self, samplename, date, eaccount, scan_number, setup, sample_additional_info, user
     ):
         """Add a sample to the omny sample database. This also retrieves the tomo id."""
         subprocess.run(
             f"wget --user=omny --password=samples -q -O /tmp/currsamplesnr.txt 'https://omny.web.psi.ch/samples/newmeasurement.php?sample={samplename}&date={date}&eaccount={eaccount}&scannr={scan_number}&setup={setup}&additional={sample_additional_info}&user={user}'",
             shell=True,
```

### Comparing `bec_client-2.3.0/bec_client/plugins/flomni/flomni_optics_mixin.py` & `bec_client-2.4.0/bec_client/plugins/flomni/flomni_optics_mixin.py`

 * *Files identical despite different names*

### Comparing `bec_client-2.3.0/bec_client/plugins/flomni/x_ray_eye_align.py` & `bec_client-2.4.0/bec_client/plugins/flomni/x_ray_eye_align.py`

 * *Files identical despite different names*

### Comparing `bec_client-2.3.0/bec_client/prettytable.py` & `bec_client-2.4.0/bec_client/prettytable.py`

 * *Files identical despite different names*

### Comparing `bec_client-2.3.0/bec_client/progressbar.py` & `bec_client-2.4.0/bec_client/progressbar.py`

 * *Files identical despite different names*

### Comparing `bec_client-2.3.0/bec_client/signals.py` & `bec_client-2.4.0/bec_client/signals.py`

 * *Files identical despite different names*

### Comparing `bec_client-2.3.0/bec_client.egg-info/SOURCES.txt` & `bec_client-2.4.0/bec_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bec_client-2.3.0/setup.cfg` & `bec_client-2.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `bec_client-2.3.0/setup.py` & `bec_client-2.4.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 current_path = pathlib.Path(__file__).parent.resolve()
 
 bec_lib = f"{current_path}/../bec_lib/"
 
 
-__version__ = "2.3.0"
+__version__ = "2.4.0"
 
 
 def run_install(setup_args: dict, bec_deps: list, editable=False):
     """
     Run the setup function with the given arguments.
 
     Args:
```

