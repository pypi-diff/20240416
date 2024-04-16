# Comparing `tmp/pyaffalddk-2.0.22.tar.gz` & `tmp/pyaffalddk-2.0.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaffalddk-2.0.22.tar", last modified: Sun Apr  7 11:55:53 2024, max compression
+gzip compressed data, was "pyaffalddk-2.0.23.tar", last modified: Tue Apr 16 12:03:02 2024, max compression
```

## Comparing `pyaffalddk-2.0.22.tar` & `pyaffalddk-2.0.23.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 11:55:53.192197 pyaffalddk-2.0.22/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-07 11:55:42.000000 pyaffalddk-2.0.22/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-07 11:55:53.192197 pyaffalddk-2.0.22/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-07 11:55:42.000000 pyaffalddk-2.0.22/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 11:55:53.192197 pyaffalddk-2.0.22/pyaffalddk/
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-07 11:55:42.000000 pyaffalddk-2.0.22/pyaffalddk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11188 2024-04-07 11:55:42.000000 pyaffalddk-2.0.22/pyaffalddk/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    11021 2024-04-07 11:55:42.000000 pyaffalddk-2.0.22/pyaffalddk/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-07 11:55:42.000000 pyaffalddk-2.0.22/pyaffalddk/data.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-07 11:55:42.000000 pyaffalddk-2.0.22/pyaffalddk/images.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 11:55:53.192197 pyaffalddk-2.0.22/pyaffalddk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-07 11:55:53.000000 pyaffalddk-2.0.22/pyaffalddk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-07 11:55:53.000000 pyaffalddk-2.0.22/pyaffalddk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 11:55:53.000000 pyaffalddk-2.0.22/pyaffalddk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-07 11:55:53.000000 pyaffalddk-2.0.22/pyaffalddk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 11:55:53.192197 pyaffalddk-2.0.22/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-07 11:55:42.000000 pyaffalddk-2.0.22/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 12:03:02.659210 pyaffalddk-2.0.23/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-16 12:02:57.000000 pyaffalddk-2.0.23/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-16 12:03:02.655210 pyaffalddk-2.0.23/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-16 12:02:57.000000 pyaffalddk-2.0.23/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 12:03:02.655210 pyaffalddk-2.0.23/pyaffalddk/
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-16 12:02:57.000000 pyaffalddk-2.0.23/pyaffalddk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11189 2024-04-16 12:02:57.000000 pyaffalddk-2.0.23/pyaffalddk/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11165 2024-04-16 12:02:57.000000 pyaffalddk-2.0.23/pyaffalddk/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-16 12:02:57.000000 pyaffalddk-2.0.23/pyaffalddk/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-16 12:02:57.000000 pyaffalddk-2.0.23/pyaffalddk/images.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 12:03:02.655210 pyaffalddk-2.0.23/pyaffalddk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-16 12:03:02.000000 pyaffalddk-2.0.23/pyaffalddk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-16 12:03:02.000000 pyaffalddk-2.0.23/pyaffalddk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 12:03:02.000000 pyaffalddk-2.0.23/pyaffalddk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-16 12:03:02.000000 pyaffalddk-2.0.23/pyaffalddk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 12:03:02.659210 pyaffalddk-2.0.23/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-16 12:02:57.000000 pyaffalddk-2.0.23/setup.py
```

### Comparing `pyaffalddk-2.0.22/LICENSE` & `pyaffalddk-2.0.23/LICENSE`

 * *Files identical despite different names*

### Comparing `pyaffalddk-2.0.22/PKG-INFO` & `pyaffalddk-2.0.23/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaffalddk
-Version: 2.0.22
+Version: 2.0.23
 Summary: Gets garbage collection data from danish Municipalities
 Home-page: https://github.com/briis/pyaffalddk
 Author: briis
 Author-email: bjarne@briis.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyaffalddk-2.0.22/pyaffalddk/__init__.py` & `pyaffalddk-2.0.23/pyaffalddk/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,10 +11,10 @@
     AffaldDKNoConnection,
 )
 from pyaffalddk.data import PickupEvents, PickupType, AffaldDKAddressInfo
 
 from pyaffalddk.const import ICON_LIST, MUNICIPALITIES_ARRAY, NAME_ARRAY, NAME_LIST, WEEKDAYS, WEEKDAYS_SHORT
 
 __title__ = "pyaffalddk"
-__version__ = "2.0.22"
+__version__ = "2.0.23"
 __author__ = "briis"
 __license__ = "MIT"
```

### Comparing `pyaffalddk-2.0.22/pyaffalddk/api.py` & `pyaffalddk-2.0.23/pyaffalddk/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -317,8 +317,8 @@
     days_ahead = (target_weekday - current_weekday) % 7
     next_date: dt.date = dt.datetime.now() + dt.timedelta(days=days_ahead)
     return next_date
 
 
 def list_to_string(list: list[str]) -> str:
     """Convert a list to a string."""
-    return ", ".join(list)
+    return " | ".join(list)
```

### Comparing `pyaffalddk-2.0.22/pyaffalddk/const.py` & `pyaffalddk-2.0.23/pyaffalddk/const.py`

 * *Files 0% similar despite different names*

```diff
@@ -166,23 +166,25 @@
     "metalglas": [
         "Glas/metal (1 stk.)",
         "240 l Glas/metal Egenløsning (1 stk.)",
         "Metal/Glas 240 l - 2-kammer (1 stk.)",
         "Glas/metal, afstand over 5 meter (1 stk.)",
         "240 L - Metal og Glas (1 stk.)",
         "240 l glas/metal - 4 tømninger (1 stk.)",
+        "240 liter - Metal/Glas - tømmes hver 8. uge (1 stk.)",
     ],
     "pappi": [
         "Plast/papir (1 stk.)",
         "370 l Plast+MDK/Papir - Egenløsning (1 stk.)",
         "Papir/Plast og MDK 240 l - 2-kammer (1 stk.)",
         "Plast/papir, afstand over 5 meter (1 stk.)",
         "240 L - Plast og Papir (1 stk.)",
         "240L genbrug (1 stk.)",
         "240 l PMDK/PP 3 ugers tømning (1 stk.)",
+        "240 liter - Plast, MDK, papir, pap – tømmes hver 2. uge (1 stk.)",
     ],
     "farligtaffald": [
         "",
     ],
     "farligtaffaldmiljoboks": [
         "Miljøkasse (1 stk.)",
         "Miljøboks",
```

### Comparing `pyaffalddk-2.0.22/pyaffalddk/data.py` & `pyaffalddk-2.0.23/pyaffalddk/data.py`

 * *Files identical despite different names*

### Comparing `pyaffalddk-2.0.22/pyaffalddk/images.py` & `pyaffalddk-2.0.23/pyaffalddk/images.py`

 * *Files identical despite different names*

### Comparing `pyaffalddk-2.0.22/pyaffalddk.egg-info/PKG-INFO` & `pyaffalddk-2.0.23/pyaffalddk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaffalddk
-Version: 2.0.22
+Version: 2.0.23
 Summary: Gets garbage collection data from danish Municipalities
 Home-page: https://github.com/briis/pyaffalddk
 Author: briis
 Author-email: bjarne@briis.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyaffalddk-2.0.22/setup.py` & `pyaffalddk-2.0.23/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyaffalddk",
-    version="2.0.22",
+    version="2.0.23",
     author="briis",
     author_email="bjarne@briis.com",
     description="Gets garbage collection data from danish Municipalities",
     license="MIT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/briis/pyaffalddk",
```

