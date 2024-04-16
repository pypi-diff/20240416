# Comparing `tmp/meteo_hr-1.2.0.tar.gz` & `tmp/meteo_hr-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meteo_hr-1.2.0.tar", last modified: Wed Oct  4 14:41:10 2023, max compression
+gzip compressed data, was "meteo_hr-1.3.0.tar", last modified: Tue Apr 16 11:05:22 2024, max compression
```

## Comparing `meteo_hr-1.2.0.tar` & `meteo_hr-1.3.0.tar`

### file list

```diff
@@ -1,22 +1,25 @@
-drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2023-10-04 14:41:10.465576 meteo_hr-1.2.0/
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    35149 2023-06-30 10:06:17.000000 meteo_hr-1.2.0/LICENSE
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    41813 2023-10-04 14:41:10.465576 meteo_hr-1.2.0/PKG-INFO
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      476 2023-10-04 13:26:28.000000 meteo_hr-1.2.0/README.md
-drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2023-10-04 14:41:10.465576 meteo_hr-1.2.0/meteo_hr/
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      201 2023-10-04 13:26:28.000000 meteo_hr-1.2.0/meteo_hr/__init__.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       30 2023-06-30 10:06:17.000000 meteo_hr-1.2.0/meteo_hr/__main__.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2158 2023-10-04 13:26:28.000000 meteo_hr-1.2.0/meteo_hr/api.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2117 2023-10-04 13:26:28.000000 meteo_hr-1.2.0/meteo_hr/cache.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1783 2023-10-04 14:03:15.000000 meteo_hr-1.2.0/meteo_hr/cli.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     5598 2023-10-04 14:39:18.000000 meteo_hr-1.2.0/meteo_hr/output.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2630 2023-10-04 13:36:36.000000 meteo_hr-1.2.0/meteo_hr/parse.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      686 2023-10-04 13:26:28.000000 meteo_hr-1.2.0/meteo_hr/places.py
-drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2023-10-04 14:41:10.465576 meteo_hr-1.2.0/meteo_hr.egg-info/
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    41813 2023-10-04 14:41:10.000000 meteo_hr-1.2.0/meteo_hr.egg-info/PKG-INFO
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      374 2023-10-04 14:41:10.000000 meteo_hr-1.2.0/meteo_hr.egg-info/SOURCES.txt
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)        1 2023-10-04 14:41:10.000000 meteo_hr-1.2.0/meteo_hr.egg-info/dependency_links.txt
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       44 2023-10-04 14:41:10.000000 meteo_hr-1.2.0/meteo_hr.egg-info/entry_points.txt
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       96 2023-10-04 14:41:10.000000 meteo_hr-1.2.0/meteo_hr.egg-info/requires.txt
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)        9 2023-10-04 14:41:10.000000 meteo_hr-1.2.0/meteo_hr.egg-info/top_level.txt
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      895 2023-10-04 14:40:54.000000 meteo_hr-1.2.0/pyproject.toml
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       38 2023-10-04 14:41:10.465576 meteo_hr-1.2.0/setup.cfg
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-16 11:05:22.021379 meteo_hr-1.3.0/
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       30 2023-06-30 10:06:17.000000 meteo_hr-1.3.0/.gitignore
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    35149 2023-06-30 10:06:17.000000 meteo_hr-1.3.0/LICENSE
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      104 2023-06-30 10:06:17.000000 meteo_hr-1.3.0/Makefile
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    41813 2024-04-16 11:05:22.017379 meteo_hr-1.3.0/PKG-INFO
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      476 2023-10-04 13:26:28.000000 meteo_hr-1.3.0/README.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)   339312 2023-06-30 10:06:17.000000 meteo_hr-1.3.0/forecast.png
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-16 11:05:22.017379 meteo_hr-1.3.0/meteo_hr/
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      349 2024-04-16 11:01:19.000000 meteo_hr-1.3.0/meteo_hr/__init__.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       30 2023-06-30 10:06:17.000000 meteo_hr-1.3.0/meteo_hr/__main__.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2158 2023-10-04 13:26:28.000000 meteo_hr-1.3.0/meteo_hr/api.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2117 2023-10-04 13:26:28.000000 meteo_hr-1.3.0/meteo_hr/cache.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2125 2024-04-16 11:03:42.000000 meteo_hr-1.3.0/meteo_hr/cli.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     5681 2024-04-16 10:56:36.000000 meteo_hr-1.3.0/meteo_hr/output.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2630 2023-10-04 13:36:36.000000 meteo_hr-1.3.0/meteo_hr/parse.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      686 2023-10-04 13:26:28.000000 meteo_hr-1.3.0/meteo_hr/places.py
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-16 11:05:22.017379 meteo_hr-1.3.0/meteo_hr.egg-info/
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    41813 2024-04-16 11:05:22.000000 meteo_hr-1.3.0/meteo_hr.egg-info/PKG-INFO
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      407 2024-04-16 11:05:22.000000 meteo_hr-1.3.0/meteo_hr.egg-info/SOURCES.txt
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)        1 2024-04-16 11:05:22.000000 meteo_hr-1.3.0/meteo_hr.egg-info/dependency_links.txt
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       44 2024-04-16 11:05:22.000000 meteo_hr-1.3.0/meteo_hr.egg-info/entry_points.txt
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       96 2024-04-16 11:05:22.000000 meteo_hr-1.3.0/meteo_hr.egg-info/requires.txt
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)        9 2024-04-16 11:05:22.000000 meteo_hr-1.3.0/meteo_hr.egg-info/top_level.txt
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      941 2024-04-16 11:04:16.000000 meteo_hr-1.3.0/pyproject.toml
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       38 2024-04-16 11:05:22.021379 meteo_hr-1.3.0/setup.cfg
```

### Comparing `meteo_hr-1.2.0/LICENSE` & `meteo_hr-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `meteo_hr-1.2.0/PKG-INFO` & `meteo_hr-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meteo_hr
-Version: 1.2.0
+Version: 1.3.0
 Summary: CLI for printing weather forecast from meteo.hr
 Author-email: Ivan Habunek <ivan@habunek.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `meteo_hr-1.2.0/meteo_hr/api.py` & `meteo_hr-1.3.0/meteo_hr/api.py`

 * *Files identical despite different names*

### Comparing `meteo_hr-1.2.0/meteo_hr/cache.py` & `meteo_hr-1.3.0/meteo_hr/cache.py`

 * *Files identical despite different names*

### Comparing `meteo_hr-1.2.0/meteo_hr/cli.py` & `meteo_hr-1.3.0/meteo_hr/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,38 @@
 import argparse
 import logging
 import sys
 
 from difflib import SequenceMatcher
-from meteo_hr import cache
+from meteo_hr import cache, __version__
 from meteo_hr.api import fetch_forecast_html
 from meteo_hr.output import bold, print_chart, print_forecast
 from meteo_hr.parse import parse_forecast
 from meteo_hr.places import list_3d, list_7d
 
 
 def make_parser():
     parser = argparse.ArgumentParser(allow_abbrev=False)
     parser.add_argument("place", nargs="*", type=str)
-    parser.add_argument("-l", "--list", action="store_true")
-    parser.add_argument("-d", "--debug", action="store_true")
-    parser.add_argument("-7", "--week", action="store_true")
-    parser.add_argument("-c", "--clear-cache", action="store_true")
+    parser.add_argument("-l", "--list", action="store_true", help="list places for which forecast is available")
+    parser.add_argument("-d", "--debug", action="store_true", help="print debug info")
+    parser.add_argument("-7", "--week", action="store_true", help="show weekly forecast instad of 3-day")
+    parser.add_argument("-c", "--clear-cache", action="store_true", help="clear cached data")
+    parser.add_argument("-v", "--version", action="store_true", help="print version and exit")
     return parser
 
 
 def main():
     parser = make_parser()
     args = parser.parse_args()
 
+    if args.version:
+        print(f"meteo_hr version {__version__}")
+        return
+
     if args.debug:
         logging.basicConfig(level=logging.DEBUG)
 
     if args.clear_cache:
         cache.clear()
 
     places = list_7d() if args.week else list_3d()
```

### Comparing `meteo_hr-1.2.0/meteo_hr/output.py` & `meteo_hr-1.3.0/meteo_hr/output.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,14 +121,15 @@
     "magla, malo do umjereno oblačno": "\N{fog}\N{fog}",
     "magla, nebo vedro": "\N{fog}\uFE0F",
     "malo oblačno, danju sunčano": "\N{white sun with small cloud}\uFE0F",
     "oblačno i maglovito": "\N{cloud}\uFE0F",
     "oblačno uz malu količinu kiše te moguću grmljavinu": "\N{white sun behind cloud with rain}\uFE0F",
     "oblačno uz malu količinu kiše": "\N{white sun behind cloud with rain}\uFE0F",
     "oblačno uz moguću grmljavinu": "\N{cloud with lightning}\uFE0F",
+    "oblačno uz umjerenu količinu kiše i snijega": "\N{cloud with snow}\uFE0F",
     "oblačno uz umjerenu količinu kiše te moguću grmljavinu": "\N{cloud with rain}\uFE0F",
     "oblačno uz umjerenu količinu kiše": "\N{cloud with rain}\uFE0F",
     "oblačno uz znatnu količinu kiše te moguću grmljavinu": "\N{thunder cloud and rain}\uFE0F",
     "oblačno uz znatnu količinu kiše": "\N{cloud with rain}\uFE0F",
     "oblačno": "\N{cloud}\uFE0F",
     "pretežno oblačno": "\N{cloud}\uFE0F",
     "promjenljivo oblačno uz malu količinu kiše te moguću grmljavinu": "\N{white sun behind cloud with rain}\uFE0F",
```

### Comparing `meteo_hr-1.2.0/meteo_hr/parse.py` & `meteo_hr-1.3.0/meteo_hr/parse.py`

 * *Files identical despite different names*

### Comparing `meteo_hr-1.2.0/meteo_hr/places.py` & `meteo_hr-1.3.0/meteo_hr/places.py`

 * *Files identical despite different names*

### Comparing `meteo_hr-1.2.0/meteo_hr.egg-info/PKG-INFO` & `meteo_hr-1.3.0/meteo_hr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: meteo-hr
-Version: 1.2.0
+Name: meteo_hr
+Version: 1.3.0
 Summary: CLI for printing weather forecast from meteo.hr
 Author-email: Ivan Habunek <ivan@habunek.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `meteo_hr-1.2.0/pyproject.toml` & `meteo_hr-1.3.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
-requires = ["setuptools>=61.0"]
+requires = ["setuptools>=64", "setuptools_scm>=8"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "meteo_hr"
-version = "1.2.0"
 authors = [{ name="Ivan Habunek", email="ivan@habunek.com" }]
 description = "CLI for printing weather forecast from meteo.hr"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
+dynamic = ["version"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
     "Environment :: Console",
 ]
 dependencies = [
@@ -34,7 +34,9 @@
 "Homepage" = "https://git.sr.ht/~ihabunek/meteo_hr"
 
 [project.scripts]
 meteo = "meteo_hr.cli:main"
 
 [tool.pyright]
 include = ["meteo_hr"]
+
+[tool.setuptools_scm]
```

