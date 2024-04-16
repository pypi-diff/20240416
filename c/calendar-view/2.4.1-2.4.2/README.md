# Comparing `tmp/calendar-view-2.4.1.tar.gz` & `tmp/calendar_view-2.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calendar-view-2.4.1.tar", last modified: Thu Jan 25 20:13:42 2024, max compression
+gzip compressed data, was "calendar_view-2.4.2.tar", last modified: Tue Apr 16 21:11:18 2024, max compression
```

## Comparing `calendar-view-2.4.1.tar` & `calendar_view-2.4.2.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 20:13:42.847966 calendar-view-2.4.1/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1077 2024-01-25 20:13:20.000000 calendar-view-2.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-01-25 20:13:20.000000 calendar-view-2.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11486 2024-01-25 20:13:42.843966 calendar-view-2.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10952 2024-01-25 20:13:20.000000 calendar-view-2.4.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 20:13:42.839965 calendar-view-2.4.1/calendar_view/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-01-25 20:13:20.000000 calendar-view-2.4.1/calendar_view/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 20:13:42.839965 calendar-view-2.4.1/calendar_view/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-01-25 20:13:36.000000 calendar-view-2.4.1/calendar_view/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-01-25 20:13:20.000000 calendar-view-2.4.1/calendar_view/calendar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 20:13:42.839965 calendar-view-2.4.1/calendar_view/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 20:13:20.000000 calendar-view-2.4.1/calendar_view/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 20:13:42.839965 calendar-view-2.4.1/calendar_view/config/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-01-25 20:13:36.000000 calendar-view-2.4.1/calendar_view/config/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-01-25 20:13:36.000000 calendar-view-2.4.1/calendar_view/config/__pycache__/style.cpython-312.pyc
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-01-25 20:13:20.000000 calendar-view-2.4.1/calendar_view/config/i18n.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-01-25 20:13:20.000000 calendar-view-2.4.1/calendar_view/config/style.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 20:13:42.843966 calendar-view-2.4.1/calendar_view/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 20:13:20.000000 calendar-view-2.4.1/calendar_view/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 20:13:42.843966 calendar-view-2.4.1/calendar_view/core/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-01-25 20:13:36.000000 calendar-view-2.4.1/calendar_view/core/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0 runner    (1001) docker     (127)     5503 2024-01-25 20:13:36.000000 calendar-view-2.4.1/calendar_view/core/__pycache__/config.cpython-312.pyc
--rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-01-25 20:13:36.000000 calendar-view-2.4.1/calendar_view/core/__pycache__/data.cpython-312.pyc
--rw-r--r--   0 runner    (1001) docker     (127)    12293 2024-01-25 20:13:36.000000 calendar-view-2.4.1/calendar_view/core/__pycache__/event.cpython-312.pyc
--rw-r--r--   0 runner    (1001) docker     (127)     8477 2024-01-25 20:13:36.000000 calendar-view-2.4.1/calendar_view/core/__pycache__/time_utils.cpython-312.pyc
--rw-r--r--   0 runner    (1001) docker     (127)     4136 2024-01-25 20:13:36.000000 calendar-view-2.4.1/calendar_view/core/__pycache__/utils.cpython-312.pyc
--rw-r--r--   0 runner    (1001) docker     (127)    18132 2024-01-25 20:13:20.000000 calendar-view-2.4.1/calendar_view/core/calendar_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-01-25 20:13:20.000000 calendar-view-2.4.1/calendar_view/core/calendar_grid.py
--rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-01-25 20:13:20.000000 calendar-view-2.4.1/calendar_view/core/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-01-25 20:13:20.000000 calendar-view-2.4.1/calendar_view/core/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     8888 2024-01-25 20:13:20.000000 calendar-view-2.4.1/calendar_view/core/event.py
--rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-01-25 20:13:20.000000 calendar-view-2.4.1/calendar_view/core/round_rectangle.py
--rw-r--r--   0 runner    (1001) docker     (127)     5426 2024-01-25 20:13:20.000000 calendar-view-2.4.1/calendar_view/core/time_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-01-25 20:13:20.000000 calendar-view-2.4.1/calendar_view/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 20:13:42.843966 calendar-view-2.4.1/calendar_view/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 20:13:20.000000 calendar-view-2.4.1/calendar_view/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 20:13:42.843966 calendar-view-2.4.1/calendar_view/resources/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-01-25 20:13:36.000000 calendar-view-2.4.1/calendar_view/resources/__pycache__/__init__.cpython-312.pyc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 20:13:42.843966 calendar-view-2.4.1/calendar_view/resources/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-01-25 20:13:20.000000 calendar-view-2.4.1/calendar_view/resources/fonts/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)   168260 2024-01-25 20:13:20.000000 calendar-view-2.4.1/calendar_view/resources/fonts/Roboto-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 20:13:20.000000 calendar-view-2.4.1/calendar_view/resources/fonts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 20:13:42.843966 calendar-view-2.4.1/calendar_view/resources/fonts/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-01-25 20:13:36.000000 calendar-view-2.4.1/calendar_view/resources/fonts/__pycache__/__init__.cpython-312.pyc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 20:13:42.843966 calendar-view-2.4.1/calendar_view.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11486 2024-01-25 20:13:42.000000 calendar-view-2.4.1/calendar_view.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-01-25 20:13:42.000000 calendar-view-2.4.1/calendar_view.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-25 20:13:42.000000 calendar-view-2.4.1/calendar_view.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-25 20:13:42.000000 calendar-view-2.4.1/calendar_view.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-01-25 20:13:42.000000 calendar-view-2.4.1/calendar_view.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-25 20:13:42.847966 calendar-view-2.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-01-25 20:13:20.000000 calendar-view-2.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 20:13:42.843966 calendar-view-2.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-01-25 20:13:20.000000 calendar-view-2.4.1/tests/test_calendar_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5498 2024-01-25 20:13:20.000000 calendar-view-2.4.1/tests/test_time_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:11:18.891823 calendar_view-2.4.2/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1077 2024-04-16 21:11:01.000000 calendar_view-2.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-16 21:11:01.000000 calendar_view-2.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11486 2024-04-16 21:11:18.891823 calendar_view-2.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10952 2024-04-16 21:11:01.000000 calendar_view-2.4.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:11:18.887823 calendar_view-2.4.2/calendar_view/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-16 21:11:01.000000 calendar_view-2.4.2/calendar_view/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:11:18.887823 calendar_view-2.4.2/calendar_view/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-16 21:11:17.000000 calendar_view-2.4.2/calendar_view/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-04-16 21:11:01.000000 calendar_view-2.4.2/calendar_view/calendar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:11:18.887823 calendar_view-2.4.2/calendar_view/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 21:11:01.000000 calendar_view-2.4.2/calendar_view/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:11:18.887823 calendar_view-2.4.2/calendar_view/config/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-16 21:11:17.000000 calendar_view-2.4.2/calendar_view/config/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-04-16 21:11:17.000000 calendar_view-2.4.2/calendar_view/config/__pycache__/style.cpython-312.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-16 21:11:01.000000 calendar_view-2.4.2/calendar_view/config/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-16 21:11:01.000000 calendar_view-2.4.2/calendar_view/config/style.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:11:18.887823 calendar_view-2.4.2/calendar_view/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 21:11:01.000000 calendar_view-2.4.2/calendar_view/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:11:18.891823 calendar_view-2.4.2/calendar_view/core/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-16 21:11:17.000000 calendar_view-2.4.2/calendar_view/core/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)     5503 2024-04-16 21:11:17.000000 calendar_view-2.4.2/calendar_view/core/__pycache__/config.cpython-312.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-04-16 21:11:17.000000 calendar_view-2.4.2/calendar_view/core/__pycache__/data.cpython-312.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)    12293 2024-04-16 21:11:17.000000 calendar_view-2.4.2/calendar_view/core/__pycache__/event.cpython-312.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)     8477 2024-04-16 21:11:17.000000 calendar_view-2.4.2/calendar_view/core/__pycache__/time_utils.cpython-312.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)     4136 2024-04-16 21:11:17.000000 calendar_view-2.4.2/calendar_view/core/__pycache__/utils.cpython-312.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)    18132 2024-04-16 21:11:01.000000 calendar_view-2.4.2/calendar_view/core/calendar_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-04-16 21:11:01.000000 calendar_view-2.4.2/calendar_view/core/calendar_grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-04-16 21:11:01.000000 calendar_view-2.4.2/calendar_view/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-16 21:11:01.000000 calendar_view-2.4.2/calendar_view/core/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8888 2024-04-16 21:11:01.000000 calendar_view-2.4.2/calendar_view/core/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-04-16 21:11:01.000000 calendar_view-2.4.2/calendar_view/core/round_rectangle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5426 2024-04-16 21:11:01.000000 calendar_view-2.4.2/calendar_view/core/time_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-04-16 21:11:01.000000 calendar_view-2.4.2/calendar_view/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:11:18.891823 calendar_view-2.4.2/calendar_view/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 21:11:01.000000 calendar_view-2.4.2/calendar_view/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:11:18.891823 calendar_view-2.4.2/calendar_view/resources/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-16 21:11:17.000000 calendar_view-2.4.2/calendar_view/resources/__pycache__/__init__.cpython-312.pyc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:11:18.891823 calendar_view-2.4.2/calendar_view/resources/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-16 21:11:01.000000 calendar_view-2.4.2/calendar_view/resources/fonts/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   168260 2024-04-16 21:11:01.000000 calendar_view-2.4.2/calendar_view/resources/fonts/Roboto-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 21:11:01.000000 calendar_view-2.4.2/calendar_view/resources/fonts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:11:18.891823 calendar_view-2.4.2/calendar_view/resources/fonts/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-16 21:11:17.000000 calendar_view-2.4.2/calendar_view/resources/fonts/__pycache__/__init__.cpython-312.pyc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:11:18.891823 calendar_view-2.4.2/calendar_view.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11486 2024-04-16 21:11:18.000000 calendar_view-2.4.2/calendar_view.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-16 21:11:18.000000 calendar_view-2.4.2/calendar_view.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 21:11:18.000000 calendar_view-2.4.2/calendar_view.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-16 21:11:18.000000 calendar_view-2.4.2/calendar_view.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-16 21:11:18.000000 calendar_view-2.4.2/calendar_view.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 21:11:18.891823 calendar_view-2.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-16 21:11:01.000000 calendar_view-2.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:11:18.891823 calendar_view-2.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-16 21:11:01.000000 calendar_view-2.4.2/tests/test_calendar_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5498 2024-04-16 21:11:01.000000 calendar_view-2.4.2/tests/test_time_utils.py
```

### Comparing `calendar-view-2.4.1/LICENSE` & `calendar_view-2.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `calendar-view-2.4.1/PKG-INFO` & `calendar_view-2.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calendar-view
-Version: 2.4.1
+Version: 2.4.2
 Summary: Library provides a graphical view of the calendar.
 Home-page: https://github.com/sakhnevych/calendar-view
 Author: Oleksandr Sakhnevych, Daniil Limariev
 Author-email: o.sakhnevych@gmail.com, danillim02102003@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `calendar-view-2.4.1/README.rst` & `calendar_view-2.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `calendar-view-2.4.1/calendar_view/calendar.py` & `calendar_view-2.4.2/calendar_view/calendar.py`

 * *Files identical despite different names*

### Comparing `calendar-view-2.4.1/calendar_view/config/__pycache__/style.cpython-312.pyc` & `calendar_view-2.4.2/calendar_view/config/__pycache__/style.cpython-312.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xcb0d0d0a
-moddate:  0xe0c0b265 (Thu Jan 25 20:13:20 2024 UTC)
+moddate:  0x65e91e66 (Tue Apr 16 21:11:01 2024 UTC)
 files sz: 1356
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 3
    flags     : 0
    code
```

### Comparing `calendar-view-2.4.1/calendar_view/config/i18n.py` & `calendar_view-2.4.2/calendar_view/config/i18n.py`

 * *Files identical despite different names*

### Comparing `calendar-view-2.4.1/calendar_view/config/style.py` & `calendar_view-2.4.2/calendar_view/config/style.py`

 * *Files identical despite different names*

### Comparing `calendar-view-2.4.1/calendar_view/core/__pycache__/config.cpython-312.pyc` & `calendar_view-2.4.2/calendar_view/core/__pycache__/config.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Thu Jan 25 20:13:20 2024 UTC, .py size: 3558 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e0c0 b265 e60d 0000  ...........e....
+00000000: cb0d 0d0a 0000 0000 65e9 1e66 e60d 0000  ........e..f....
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 00f3 6800 0000 9700 6400 6401  ......h.....d.d.
 00000030: 6c00 5a00 6400 6402 6c01 6d02 5a02 6d03  l.Z.d.d.l.m.Z.m.
 00000040: 5a03 0100 6400 6403 6c04 6d05 5a05 6d06  Z...d.d.l.m.Z.m.
 00000050: 5a06 6d07 5a07 0100 6400 6404 6c08 6d09  Z.m.Z...d.d.l.m.
 00000060: 5a09 0100 6400 6405 6c0a 6d0b 5a0b 0100  Z...d.d.l.m.Z...
 00000070: 6507 6406 1900 0000 5a0c 0200 4700 6407  e.d.....Z...G.d.
```

### Comparing `calendar-view-2.4.1/calendar_view/core/__pycache__/data.cpython-312.pyc` & `calendar_view-2.4.2/calendar_view/core/__pycache__/data.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Thu Jan 25 20:13:20 2024 UTC, .py size: 1675 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e0c0 b265 8b06 0000  ...........e....
+00000000: cb0d 0d0a 0000 0000 65e9 1e66 8b06 0000  ........e..f....
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 00f3 7e00 0000 9700 6400 6401  ......~.....d.d.
 00000030: 6c00 5a00 6400 6402 6c01 6d02 5a02 0100  l.Z.d.d.l.m.Z...
 00000040: 6400 6403 6c03 6d04 5a04 0100 6400 6404  d.d.l.m.Z...d.d.
 00000050: 6c05 6d06 5a06 0100 0200 4700 6405 8400  l.m.Z.....G.d...
 00000060: 6406 6507 ab03 0000 0000 0000 5a08 6407  d.e.........Z.d.
 00000070: 6504 6602 6408 8404 5a09 6409 6506 6407  e.f.d...Z.d.e.d.
```

### Comparing `calendar-view-2.4.1/calendar_view/core/__pycache__/event.cpython-312.pyc` & `calendar_view-2.4.2/calendar_view/core/__pycache__/event.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Thu Jan 25 20:13:20 2024 UTC, .py size: 8888 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e0c0 b265 b822 0000  ...........e."..
+00000000: cb0d 0d0a 0000 0000 65e9 1e66 b822 0000  ........e..f."..
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 00f3 7400 0000 9700 6400 6401  ......t.....d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 6d03  l.m.Z...d.d.l.m.
 00000040: 5a03 0100 6400 6403 6c04 6d05 5a05 0100  Z...d.d.l.m.Z...
 00000050: 6400 6404 6c06 ad02 0100 0200 4700 6405  d.d.l.......G.d.
 00000060: 8400 6406 6507 ab03 0000 0000 0000 5a08  ..d.e.........Z.
 00000070: 0200 4700 6407 8400 6408 6507 ab03 0000  ..G.d...d.e.....
```

### Comparing `calendar-view-2.4.1/calendar_view/core/__pycache__/time_utils.cpython-312.pyc` & `calendar_view-2.4.2/calendar_view/core/__pycache__/time_utils.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Thu Jan 25 20:13:20 2024 UTC, .py size: 5426 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e0c0 b265 3215 0000  ...........e2...
+00000000: cb0d 0d0a 0000 0000 65e9 1e66 3215 0000  ........e..f2...
 00000010: e300 0000 0000 0000 0000 0000 0010 0000  ................
 00000020: 0000 0000 00f3 6c01 0000 9700 6400 6401  ......l.....d.d.
 00000030: 6c00 5a00 6400 6402 6c01 6d02 5a02 6d03  l.Z.d.d.l.m.Z.m.
 00000040: 5a03 6d04 5a04 6d01 5a01 0100 6400 6403  Z.m.Z.m.Z...d.d.
 00000050: 6c05 6d06 5a06 6d07 5a07 0100 6400 6404  l.m.Z.m.Z...d.d.
 00000060: 6c08 6d09 5a09 0100 6405 5a0a 0200 6502  l.m.Z...d.Z...e.
 00000070: 6400 6400 ab02 0000 0000 0000 5a0b 6400  d.d.........Z.d.
```

### Comparing `calendar-view-2.4.1/calendar_view/core/__pycache__/utils.cpython-312.pyc` & `calendar_view-2.4.2/calendar_view/core/__pycache__/utils.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Thu Jan 25 20:13:20 2024 UTC, .py size: 2207 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e0c0 b265 9f08 0000  ...........e....
+00000000: cb0d 0d0a 0000 0000 65e9 1e66 9f08 0000  ........e..f....
 00000010: e300 0000 0000 0000 0000 0000 0004 0000  ................
 00000020: 0000 0000 00f3 5400 0000 9700 6400 6401  ......T.....d.d.
 00000030: 6c00 6d01 5a01 6d02 5a02 6d03 5a03 0100  l.m.Z.m.Z.m.Z...
 00000040: 6400 6402 6c04 6d05 5a05 6d06 5a06 6d07  d.d.l.m.Z.m.Z.m.
 00000050: 5a07 0100 0200 4700 6403 8400 6404 ab02  Z.....G.d...d...
 00000060: 0000 0000 0000 5a08 0200 4700 6405 8400  ......Z...G.d...
 00000070: 6406 ab02 0000 0000 0000 5a09 7907 2908  d.........Z.y.).
```

### Comparing `calendar-view-2.4.1/calendar_view/core/calendar_events.py` & `calendar_view-2.4.2/calendar_view/core/calendar_events.py`

 * *Files identical despite different names*

### Comparing `calendar-view-2.4.1/calendar_view/core/calendar_grid.py` & `calendar_view-2.4.2/calendar_view/core/calendar_grid.py`

 * *Files identical despite different names*

### Comparing `calendar-view-2.4.1/calendar_view/core/config.py` & `calendar_view-2.4.2/calendar_view/core/config.py`

 * *Files identical despite different names*

### Comparing `calendar-view-2.4.1/calendar_view/core/data.py` & `calendar_view-2.4.2/calendar_view/core/data.py`

 * *Files identical despite different names*

### Comparing `calendar-view-2.4.1/calendar_view/core/event.py` & `calendar_view-2.4.2/calendar_view/core/event.py`

 * *Files identical despite different names*

### Comparing `calendar-view-2.4.1/calendar_view/core/round_rectangle.py` & `calendar_view-2.4.2/calendar_view/core/round_rectangle.py`

 * *Files identical despite different names*

### Comparing `calendar-view-2.4.1/calendar_view/core/time_utils.py` & `calendar_view-2.4.2/calendar_view/core/time_utils.py`

 * *Files identical despite different names*

### Comparing `calendar-view-2.4.1/calendar_view/core/utils.py` & `calendar_view-2.4.2/calendar_view/core/utils.py`

 * *Files identical despite different names*

### Comparing `calendar-view-2.4.1/calendar_view/resources/fonts/LICENSE.txt` & `calendar_view-2.4.2/calendar_view/resources/fonts/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `calendar-view-2.4.1/calendar_view/resources/fonts/Roboto-Regular.ttf` & `calendar_view-2.4.2/calendar_view/resources/fonts/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `calendar-view-2.4.1/calendar_view.egg-info/PKG-INFO` & `calendar_view-2.4.2/calendar_view.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calendar-view
-Version: 2.4.1
+Version: 2.4.2
 Summary: Library provides a graphical view of the calendar.
 Home-page: https://github.com/sakhnevych/calendar-view
 Author: Oleksandr Sakhnevych, Daniil Limariev
 Author-email: o.sakhnevych@gmail.com, danillim02102003@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `calendar-view-2.4.1/calendar_view.egg-info/SOURCES.txt` & `calendar_view-2.4.2/calendar_view.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `calendar-view-2.4.1/setup.py` & `calendar_view-2.4.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.rst", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="calendar-view",
-    version="2.4.1",
+    version="2.4.2",
     author="Oleksandr Sakhnevych, Daniil Limariev",
     author_email="o.sakhnevych@gmail.com, danillim02102003@gmail.com",
     description="Library provides a graphical view of the calendar.",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/sakhnevych/calendar-view",
     packages=setuptools.find_packages(),
```

### Comparing `calendar-view-2.4.1/tests/test_calendar_config.py` & `calendar_view-2.4.2/tests/test_calendar_config.py`

 * *Files identical despite different names*

### Comparing `calendar-view-2.4.1/tests/test_time_utils.py` & `calendar_view-2.4.2/tests/test_time_utils.py`

 * *Files identical despite different names*

