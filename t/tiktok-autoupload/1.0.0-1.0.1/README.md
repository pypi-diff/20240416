# Comparing `tmp/tiktok_autoupload-1.0.0.tar.gz` & `tmp/tiktok_autoupload-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiktok_autoupload-1.0.0.tar", last modified: Tue Apr 16 13:42:01 2024, max compression
+gzip compressed data, was "tiktok_autoupload-1.0.1.tar", last modified: Tue Apr 16 18:11:34 2024, max compression
```

## Comparing `tiktok_autoupload-1.0.0.tar` & `tiktok_autoupload-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 agente3z  (1000) agente3z  (1000)        0 2024-04-16 13:42:01.674295 tiktok_autoupload-1.0.0/
--rw-r--r--   0 agente3z  (1000) agente3z  (1000)    35148 2024-04-16 13:28:12.000000 tiktok_autoupload-1.0.0/LICENSE
--rw-r--r--   0 agente3z  (1000) agente3z  (1000)    40903 2024-04-16 13:42:01.674295 tiktok_autoupload-1.0.0/PKG-INFO
--rw-r--r--   0 agente3z  (1000) agente3z  (1000)      443 2024-04-16 13:34:24.000000 tiktok_autoupload-1.0.0/pyproject.toml
--rw-r--r--   0 agente3z  (1000) agente3z  (1000)       38 2024-04-16 13:42:01.674295 tiktok_autoupload-1.0.0/setup.cfg
-drwxr-xr-x   0 agente3z  (1000) agente3z  (1000)        0 2024-04-16 13:42:01.674295 tiktok_autoupload-1.0.0/src/
-drwxr-xr-x   0 agente3z  (1000) agente3z  (1000)        0 2024-04-16 13:42:01.674295 tiktok_autoupload-1.0.0/src/tiktok_autoupload/
--rw-r--r--   0 agente3z  (1000) agente3z  (1000)       30 2024-04-16 13:26:52.000000 tiktok_autoupload-1.0.0/src/tiktok_autoupload/__init__,.py
--rw-r--r--   0 agente3z  (1000) agente3z  (1000)     4263 2024-04-16 13:32:22.000000 tiktok_autoupload-1.0.0/src/tiktok_autoupload/uploader.py
-drwxr-xr-x   0 agente3z  (1000) agente3z  (1000)        0 2024-04-16 13:42:01.674295 tiktok_autoupload-1.0.0/src/tiktok_autoupload.egg-info/
--rw-r--r--   0 agente3z  (1000) agente3z  (1000)    40903 2024-04-16 13:42:01.000000 tiktok_autoupload-1.0.0/src/tiktok_autoupload.egg-info/PKG-INFO
--rw-r--r--   0 agente3z  (1000) agente3z  (1000)      315 2024-04-16 13:42:01.000000 tiktok_autoupload-1.0.0/src/tiktok_autoupload.egg-info/SOURCES.txt
--rw-r--r--   0 agente3z  (1000) agente3z  (1000)        1 2024-04-16 13:42:01.000000 tiktok_autoupload-1.0.0/src/tiktok_autoupload.egg-info/dependency_links.txt
--rw-r--r--   0 agente3z  (1000) agente3z  (1000)       33 2024-04-16 13:42:01.000000 tiktok_autoupload-1.0.0/src/tiktok_autoupload.egg-info/requires.txt
--rw-r--r--   0 agente3z  (1000) agente3z  (1000)       18 2024-04-16 13:42:01.000000 tiktok_autoupload-1.0.0/src/tiktok_autoupload.egg-info/top_level.txt
+drwxr-xr-x   0 agente3z  (1000) agente3z  (1000)        0 2024-04-16 18:11:34.578356 tiktok_autoupload-1.0.1/
+-rw-r--r--   0 agente3z  (1000) agente3z  (1000)    35148 2024-04-16 13:28:12.000000 tiktok_autoupload-1.0.1/LICENSE
+-rw-r--r--   0 agente3z  (1000) agente3z  (1000)    40881 2024-04-16 18:11:34.578356 tiktok_autoupload-1.0.1/PKG-INFO
+-rw-r--r--   0 agente3z  (1000) agente3z  (1000)      433 2024-04-16 18:09:49.000000 tiktok_autoupload-1.0.1/pyproject.toml
+-rw-r--r--   0 agente3z  (1000) agente3z  (1000)       38 2024-04-16 18:11:34.578356 tiktok_autoupload-1.0.1/setup.cfg
+drwxr-xr-x   0 agente3z  (1000) agente3z  (1000)        0 2024-04-16 18:11:34.578356 tiktok_autoupload-1.0.1/src/
+drwxr-xr-x   0 agente3z  (1000) agente3z  (1000)        0 2024-04-16 18:11:34.578356 tiktok_autoupload-1.0.1/src/tiktok_autoupload/
+-rw-r--r--   0 agente3z  (1000) agente3z  (1000)       30 2024-04-16 13:26:52.000000 tiktok_autoupload-1.0.1/src/tiktok_autoupload/__init__,.py
+-rw-r--r--   0 agente3z  (1000) agente3z  (1000)     4263 2024-04-16 13:32:22.000000 tiktok_autoupload-1.0.1/src/tiktok_autoupload/uploader.py
+drwxr-xr-x   0 agente3z  (1000) agente3z  (1000)        0 2024-04-16 18:11:34.578356 tiktok_autoupload-1.0.1/src/tiktok_autoupload.egg-info/
+-rw-r--r--   0 agente3z  (1000) agente3z  (1000)    40881 2024-04-16 18:11:34.000000 tiktok_autoupload-1.0.1/src/tiktok_autoupload.egg-info/PKG-INFO
+-rw-r--r--   0 agente3z  (1000) agente3z  (1000)      315 2024-04-16 18:11:34.000000 tiktok_autoupload-1.0.1/src/tiktok_autoupload.egg-info/SOURCES.txt
+-rw-r--r--   0 agente3z  (1000) agente3z  (1000)        1 2024-04-16 18:11:34.000000 tiktok_autoupload-1.0.1/src/tiktok_autoupload.egg-info/dependency_links.txt
+-rw-r--r--   0 agente3z  (1000) agente3z  (1000)       26 2024-04-16 18:11:34.000000 tiktok_autoupload-1.0.1/src/tiktok_autoupload.egg-info/requires.txt
+-rw-r--r--   0 agente3z  (1000) agente3z  (1000)       18 2024-04-16 18:11:34.000000 tiktok_autoupload-1.0.1/src/tiktok_autoupload.egg-info/top_level.txt
```

### Comparing `tiktok_autoupload-1.0.0/LICENSE` & `tiktok_autoupload-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tiktok_autoupload-1.0.0/PKG-INFO` & `tiktok_autoupload-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiktok-autoupload
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python library to upload a video on tiktok using selenium
 Author: Christian Fiore
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -676,10 +676,9 @@
         may consider it more useful to permit linking proprietary applications with
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
 Project-URL: Homepage, https://github.com/agente3z/tiktok-autoupload
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pickle
 Requires-Dist: selenium
 Requires-Dist: selenium_stealth
```

### Comparing `tiktok_autoupload-1.0.0/src/tiktok_autoupload/uploader.py` & `tiktok_autoupload-1.0.1/src/tiktok_autoupload/uploader.py`

 * *Files identical despite different names*

### Comparing `tiktok_autoupload-1.0.0/src/tiktok_autoupload.egg-info/PKG-INFO` & `tiktok_autoupload-1.0.1/src/tiktok_autoupload.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiktok-autoupload
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python library to upload a video on tiktok using selenium
 Author: Christian Fiore
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -676,10 +676,9 @@
         may consider it more useful to permit linking proprietary applications with
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
 Project-URL: Homepage, https://github.com/agente3z/tiktok-autoupload
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pickle
 Requires-Dist: selenium
 Requires-Dist: selenium_stealth
```

