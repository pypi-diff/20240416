# Comparing `tmp/pyaardvark-0.7.1.tar.gz` & `tmp/pyaardvark-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaardvark-0.7.1.tar", last modified: Wed Dec  7 21:55:59 2022, max compression
+gzip compressed data, was "pyaardvark-0.8.1.tar", last modified: Tue Apr 16 15:44:29 2024, max compression
```

## Comparing `pyaardvark-0.7.1.tar` & `pyaardvark-0.8.1.tar`

### file list

```diff
@@ -1,54 +1,61 @@
-drwxr-xr-x   0 mw        (1000) mw        (1000)        0 2022-12-07 21:55:59.849273 pyaardvark-0.7.1/
--rw-r--r--   0 mw        (1000) mw        (1000)      234 2022-12-06 22:08:42.000000 pyaardvark-0.7.1/AUTHORS
--rw-r--r--   0 mw        (1000) mw        (1000)    24486 2014-02-06 18:35:28.000000 pyaardvark-0.7.1/COPYING
--rw-r--r--   0 mw        (1000) mw        (1000)      186 2022-12-06 22:08:42.000000 pyaardvark-0.7.1/MANIFEST.in
--rw-r--r--   0 mw        (1000) mw        (1000)     3936 2022-12-07 21:55:59.849273 pyaardvark-0.7.1/PKG-INFO
--rw-r--r--   0 mw        (1000) mw        (1000)     2937 2022-12-07 21:54:19.000000 pyaardvark-0.7.1/README.rst
-drwxr-xr-x   0 mw        (1000) mw        (1000)        0 2022-12-07 21:55:59.845273 pyaardvark-0.7.1/docs/
--rw-r--r--   0 mw        (1000) mw        (1000)      255 2022-12-06 22:08:42.000000 pyaardvark-0.7.1/docs/api.rst
--rw-r--r--   0 mw        (1000) mw        (1000)     7800 2014-02-11 22:28:44.000000 pyaardvark-0.7.1/docs/conf.py
--rw-r--r--   0 mw        (1000) mw        (1000)     7800 2014-02-11 18:14:34.000000 pyaardvark-0.7.1/docs/conf.py~
--rw-r--r--   0 mw        (1000) mw        (1000)       77 2014-02-11 18:14:34.000000 pyaardvark-0.7.1/docs/defines.rst.inc
--rw-r--r--   0 mw        (1000) mw        (1000)      452 2014-02-11 18:14:34.000000 pyaardvark-0.7.1/docs/index.rst
--rw-r--r--   0 mw        (1000) mw        (1000)     4720 2022-12-06 22:08:42.000000 pyaardvark-0.7.1/docs/intro.rst
--rw-r--r--   0 mw        (1000) mw        (1000)     2363 2014-02-12 21:58:07.000000 pyaardvark-0.7.1/docs/intro.rst~
-drwxr-xr-x   0 mw        (1000) mw        (1000)        0 2022-12-07 21:55:59.845273 pyaardvark-0.7.1/pyaardvark/
--rw-r--r--   0 mw        (1000) mw        (1000)      949 2022-12-06 22:08:42.000000 pyaardvark-0.7.1/pyaardvark/__init__.py
--rw-r--r--   0 mw        (1000) mw        (1000)    22687 2022-12-07 15:41:12.000000 pyaardvark-0.7.1/pyaardvark/aardvark.py
--rw-r--r--   0 mw        (1000) mw        (1000)     6290 2022-12-06 22:08:42.000000 pyaardvark-0.7.1/pyaardvark/cli_tool.py
--rw-r--r--   0 mw        (1000) mw        (1000)     4852 2022-12-06 22:08:42.000000 pyaardvark-0.7.1/pyaardvark/constants.py
-drwxr-xr-x   0 mw        (1000) mw        (1000)        0 2022-12-07 21:55:59.845273 pyaardvark-0.7.1/pyaardvark/ext/
--rw-r--r--   0 mw        (1000) mw        (1000)     6042 2022-12-06 22:08:42.000000 pyaardvark-0.7.1/pyaardvark/ext/LICENSE.txt
--rw-r--r--   0 mw        (1000) mw        (1000)        0 2014-02-06 18:35:28.000000 pyaardvark-0.7.1/pyaardvark/ext/__init__.py
-drwxr-xr-x   0 mw        (1000) mw        (1000)        0 2022-12-07 21:55:59.845273 pyaardvark-0.7.1/pyaardvark/ext/linux32/
--rw-r--r--   0 mw        (1000) mw        (1000)        0 2014-02-07 23:43:39.000000 pyaardvark-0.7.1/pyaardvark/ext/linux32/__init__.py
--rw-r--r--   0 mw        (1000) mw        (1000)    59952 2022-09-30 10:00:00.000000 pyaardvark-0.7.1/pyaardvark/ext/linux32/aardvark.so
-drwxr-xr-x   0 mw        (1000) mw        (1000)        0 2022-12-07 21:55:59.845273 pyaardvark-0.7.1/pyaardvark/ext/linux64/
--rw-r--r--   0 mw        (1000) mw        (1000)        0 2014-02-07 23:43:39.000000 pyaardvark-0.7.1/pyaardvark/ext/linux64/__init__.py
--rw-r--r--   0 mw        (1000) mw        (1000)    70104 2022-09-30 10:00:00.000000 pyaardvark-0.7.1/pyaardvark/ext/linux64/aardvark.so
-drwxr-xr-x   0 mw        (1000) mw        (1000)        0 2022-12-07 21:55:59.845273 pyaardvark-0.7.1/pyaardvark/ext/osx64/
--rw-r--r--   0 mw        (1000) mw        (1000)        0 2022-12-06 22:08:42.000000 pyaardvark-0.7.1/pyaardvark/ext/osx64/__init__.py
--rw-r--r--   0 mw        (1000) mw        (1000)    72228 2022-09-30 10:00:00.000000 pyaardvark-0.7.1/pyaardvark/ext/osx64/aardvark.so
-drwxr-xr-x   0 mw        (1000) mw        (1000)        0 2022-12-07 21:55:59.845273 pyaardvark-0.7.1/pyaardvark/ext/osxarm/
--rw-r--r--   0 mw        (1000) mw        (1000)        0 2022-12-07 15:42:17.000000 pyaardvark-0.7.1/pyaardvark/ext/osxarm/__init__.py
--rw-r--r--   0 mw        (1000) mw        (1000)    91968 2022-09-30 10:00:00.000000 pyaardvark-0.7.1/pyaardvark/ext/osxarm/aardvark.so
-drwxr-xr-x   0 mw        (1000) mw        (1000)        0 2022-12-07 21:55:59.845273 pyaardvark-0.7.1/pyaardvark/ext/win32/
--rw-r--r--   0 mw        (1000) mw        (1000)        0 2022-12-06 22:08:42.000000 pyaardvark-0.7.1/pyaardvark/ext/win32/__init__.py
--rw-r--r--   0 mw        (1000) mw        (1000)    70865 2022-09-30 10:00:00.000000 pyaardvark-0.7.1/pyaardvark/ext/win32/aardvark.pyd
-drwxr-xr-x   0 mw        (1000) mw        (1000)        0 2022-12-07 21:55:59.849273 pyaardvark-0.7.1/pyaardvark/ext/win64/
--rw-r--r--   0 mw        (1000) mw        (1000)        0 2022-12-06 22:08:42.000000 pyaardvark-0.7.1/pyaardvark/ext/win64/__init__.py
--rw-r--r--   0 mw        (1000) mw        (1000)    64415 2022-09-30 10:00:00.000000 pyaardvark-0.7.1/pyaardvark/ext/win64/aardvark.pyd
--rw-r--r--   0 mw        (1000) mw        (1000)       64 2022-12-07 21:55:59.000000 pyaardvark-0.7.1/pyaardvark/version.py
-drwxr-xr-x   0 mw        (1000) mw        (1000)        0 2022-12-07 21:55:59.845273 pyaardvark-0.7.1/pyaardvark.egg-info/
--rw-r--r--   0 mw        (1000) mw        (1000)     3936 2022-12-07 21:55:59.000000 pyaardvark-0.7.1/pyaardvark.egg-info/PKG-INFO
--rw-r--r--   0 mw        (1000) mw        (1000)      996 2022-12-07 21:55:59.000000 pyaardvark-0.7.1/pyaardvark.egg-info/SOURCES.txt
--rw-r--r--   0 mw        (1000) mw        (1000)        1 2022-12-07 21:55:59.000000 pyaardvark-0.7.1/pyaardvark.egg-info/dependency_links.txt
--rw-r--r--   0 mw        (1000) mw        (1000)       54 2022-12-07 21:55:59.000000 pyaardvark-0.7.1/pyaardvark.egg-info/entry_points.txt
--rw-r--r--   0 mw        (1000) mw        (1000)        7 2022-12-07 21:55:59.000000 pyaardvark-0.7.1/pyaardvark.egg-info/requires.txt
--rw-r--r--   0 mw        (1000) mw        (1000)       17 2022-12-07 21:55:59.000000 pyaardvark-0.7.1/pyaardvark.egg-info/top_level.txt
--rw-r--r--   0 mw        (1000) mw        (1000)       38 2022-12-07 21:55:59.849273 pyaardvark-0.7.1/setup.cfg
--rw-r--r--   0 mw        (1000) mw        (1000)     2557 2022-12-07 21:54:19.000000 pyaardvark-0.7.1/setup.py
-drwxr-xr-x   0 mw        (1000) mw        (1000)        0 2022-12-07 21:55:59.849273 pyaardvark-0.7.1/tests/
--rw-r--r--   0 mw        (1000) mw        (1000)        0 2014-04-15 18:05:42.000000 pyaardvark-0.7.1/tests/__init__.py
--rw-r--r--   0 mw        (1000) mw        (1000)    19947 2022-12-07 21:54:19.000000 pyaardvark-0.7.1/tests/test_aardvark.py
--rw-r--r--   0 mw        (1000) mw        (1000)      191 2022-12-07 21:54:19.000000 pyaardvark-0.7.1/tests/test_ext.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:44:29.130422 pyaardvark-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-16 15:44:25.000000 pyaardvark-0.8.1/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)    24486 2024-04-16 15:44:25.000000 pyaardvark-0.8.1/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-16 15:44:25.000000 pyaardvark-0.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-04-16 15:44:29.130422 pyaardvark-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-04-16 15:44:25.000000 pyaardvark-0.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:44:29.126422 pyaardvark-0.8.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-16 15:44:25.000000 pyaardvark-0.8.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7800 2024-04-16 15:44:25.000000 pyaardvark-0.8.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-16 15:44:25.000000 pyaardvark-0.8.1/docs/defines.rst.inc
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-16 15:44:25.000000 pyaardvark-0.8.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-04-16 15:44:25.000000 pyaardvark-0.8.1/docs/intro.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:44:29.126422 pyaardvark-0.8.1/pyaardvark/
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-16 15:44:25.000000 pyaardvark-0.8.1/pyaardvark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20562 2024-04-16 15:44:25.000000 pyaardvark-0.8.1/pyaardvark/aardvark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5608 2024-04-16 15:44:25.000000 pyaardvark-0.8.1/pyaardvark/cli_tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-04-16 15:44:25.000000 pyaardvark-0.8.1/pyaardvark/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:44:29.126422 pyaardvark-0.8.1/pyaardvark/ext/
+-rw-r--r--   0 runner    (1001) docker     (127)     6137 2024-04-16 15:44:25.000000 pyaardvark-0.8.1/pyaardvark/ext/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-16 15:44:25.000000 pyaardvark-0.8.1/pyaardvark/ext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:44:29.126422 pyaardvark-0.8.1/pyaardvark/ext/linux32/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:44:25.000000 pyaardvark-0.8.1/pyaardvark/ext/linux32/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    84644 2024-04-16 15:44:25.000000 pyaardvark-0.8.1/pyaardvark/ext/linux32/aardvark.so
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:44:29.126422 pyaardvark-0.8.1/pyaardvark/ext/linux64/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:44:25.000000 pyaardvark-0.8.1/pyaardvark/ext/linux64/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69608 2024-04-16 15:44:25.000000 pyaardvark-0.8.1/pyaardvark/ext/linux64/aardvark.so
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:44:29.126422 pyaardvark-0.8.1/pyaardvark/ext/linuxarm32/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:44:25.000000 pyaardvark-0.8.1/pyaardvark/ext/linuxarm32/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53500 2024-04-16 15:44:25.000000 pyaardvark-0.8.1/pyaardvark/ext/linuxarm32/aardvark.so
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:44:29.130422 pyaardvark-0.8.1/pyaardvark/ext/linuxarm64/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:44:25.000000 pyaardvark-0.8.1/pyaardvark/ext/linuxarm64/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72360 2024-04-16 15:44:25.000000 pyaardvark-0.8.1/pyaardvark/ext/linuxarm64/aardvark.so
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:44:29.130422 pyaardvark-0.8.1/pyaardvark/ext/osx64/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:44:25.000000 pyaardvark-0.8.1/pyaardvark/ext/osx64/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67684 2024-04-16 15:44:25.000000 pyaardvark-0.8.1/pyaardvark/ext/osx64/aardvark.so
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:44:29.130422 pyaardvark-0.8.1/pyaardvark/ext/osxarm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:44:25.000000 pyaardvark-0.8.1/pyaardvark/ext/osxarm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   105456 2024-04-16 15:44:25.000000 pyaardvark-0.8.1/pyaardvark/ext/osxarm/aardvark.so
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:44:29.130422 pyaardvark-0.8.1/pyaardvark/ext/win32/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:44:25.000000 pyaardvark-0.8.1/pyaardvark/ext/win32/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60416 2024-04-16 15:44:25.000000 pyaardvark-0.8.1/pyaardvark/ext/win32/aardvark.pyd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:44:29.130422 pyaardvark-0.8.1/pyaardvark/ext/win64/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:44:25.000000 pyaardvark-0.8.1/pyaardvark/ext/win64/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57856 2024-04-16 15:44:25.000000 pyaardvark-0.8.1/pyaardvark/ext/win64/aardvark.pyd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:44:29.130422 pyaardvark-0.8.1/pyaardvark/ext/winarm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:44:25.000000 pyaardvark-0.8.1/pyaardvark/ext/winarm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54784 2024-04-16 15:44:25.000000 pyaardvark-0.8.1/pyaardvark/ext/winarm/aardvark.pyd
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-16 15:44:29.000000 pyaardvark-0.8.1/pyaardvark/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:44:29.130422 pyaardvark-0.8.1/pyaardvark.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-04-16 15:44:29.000000 pyaardvark-0.8.1/pyaardvark.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-16 15:44:29.000000 pyaardvark-0.8.1/pyaardvark.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 15:44:29.000000 pyaardvark-0.8.1/pyaardvark.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-16 15:44:29.000000 pyaardvark-0.8.1/pyaardvark.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-16 15:44:29.000000 pyaardvark-0.8.1/pyaardvark.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-16 15:44:29.000000 pyaardvark-0.8.1/pyaardvark.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 15:44:29.130422 pyaardvark-0.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-04-16 15:44:25.000000 pyaardvark-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:44:29.130422 pyaardvark-0.8.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:44:25.000000 pyaardvark-0.8.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19125 2024-04-16 15:44:25.000000 pyaardvark-0.8.1/tests/test_aardvark.py
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-16 15:44:25.000000 pyaardvark-0.8.1/tests/test_ext.py
```

### Comparing `pyaardvark-0.7.1/COPYING` & `pyaardvark-0.8.1/COPYING`

 * *Files identical despite different names*

### Comparing `pyaardvark-0.7.1/PKG-INFO` & `pyaardvark-0.8.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,116 +1,103 @@
 Metadata-Version: 2.1
 Name: pyaardvark
-Version: 0.7.1
+Version: 0.8.1
 Summary: Total Phase Aardvark library
 Home-page: http://github.com/kontron/python-aardvark
 Author: Michael Walle
 Author-email: michael.walle@kontron.com
 License: LGPLv2+
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Description-Content-Type: text/markdown
 License-File: COPYING
 License-File: AUTHORS
+Requires-Dist: future
 
-Python binding for Total Phase Aardvark
-=======================================
+# Python binding for Total Phase Aardvark
 
-|BuildStatus| |PyPiVersion| |PyPiPythonVersions|
+![BuildStatus](https://github.com/kontron/python-aardvark/actions/workflows/python-package.yml/badge.svg)
+![PyPiVersion](https://badge.fury.io/py/pyaardvark.svg)
+![Python versions](https://img.shields.io/pypi/pyversions/pyaardvark.svg)
 
-The `Total Phase`_ Aardvark is an USB |I2C|/SPI host adapter.
+The [Total Phase](http://www.totalphase.com) Aardvark is an USB I²C/SPI
+host adapter.
 
+## Rationale
 
-Rationale
----------
-
-The manufacturer already provides an python binding. So why a new one? This
-is correct, but the python binding you can find in the
-``aardvark-linux-api`` package is very C oriented. Eg. you need to pass
+The manufacturer already provides an python binding. So why a new one?
+This is correct, but the python binding you can find in the
+`aardvark-linux-api` package is very C oriented. Eg. you need to pass
 arrays as method parameters, which are then modified by the binding.
 Instead, this binding tries to be more pythonic.
 
+## Features
 
-Features
---------
-
-* simple interface
-* CLI tool for easy testing
-* |I2C| and SPI support
-* support for control signals like target power and internal |I2C| pullups
-* rudimental |I2C| slave support
-* Support for Linux, Windows and OSX
-
-
-(Still) Missing Features
-------------------------
+- simple interface
+- CLI tool for easy testing
+- I²C and SPI support
+- support for control signals like target power and internal I²C
+  pullups
+- rudimental I²C slave support
+- Support for Linux, Windows and OSX
 
-* more documentation (please bear with me)
-* GPIO support
+## (Still) Missing Features
 
+- more documentation (please bear with me)
+- GPIO support
 
-Documentation
--------------
+## Documentation
 
 You can find the most up to date documentation at:
-http://pyaardvark.rtfd.org
+<http://pyaardvark.rtfd.org>
 
+## Requirements
 
-Requirements
-------------
+You need an either an x86, an amd64, an aarch64, an arm32 or a M1 machine. This
+is because the binding uses a binary-only module supplied by the manufacturer,
+Total Phase. Linux, Windows, and OSX are supported.
 
-You need an either a x86 or an amd64 machine. This is because the binding
-uses a binary-only module supplied by the manufacturer, Total Phase.
-Linux, Windows, and OSX is supported.
+### Python 2.7 support
 
+The last version with python 2.7 support is 0.7.1.
 
-Contributing
-------------
+### Monitor support
 
-Contributions are always welcome. You may send patches directly (eg. ``git
-send-email``), do a github pull request or just file an issue.
+Total Phase removed the monitor support in their binary modules in version 6.00.
+The last pyaardvark version which use the old binaries and thus still support
+montoring is 0.7.x.
 
-If you are doing code changes or additions please:
+## Contributing
 
-* respect the coding style (eg. PEP8),
-* provide well-formed commit message (see `this blog post
-  <http://tbaggery.com/2008/04/19/a-note-about-git-commit-messages.html>`_.)
-* add a Signed-off-by line (eg. ``git commit -s``)
+Contributions are always welcome. You may send patches directly (eg. `git
+send-email`), do a github pull request or just file an issue.
 
+If you are doing code changes or additions please:
+- respect the coding style (eg. PEP8),
+- provide well-formed commit message (see [this blog
+  post](http://tbaggery.com/2008/04/19/a-note-about-git-commit-messages.html).)
+- add a Signed-off-by line (eg. `git commit -s`)
 
-License
--------
+## License
 
 This library is free software; you can redistribute it and/or modify it
 under the terms of the GNU Lesser General Public License as published by
 the Free Software Foundation; either version 2.1 of the License, or (at
 your option) any later version.
 
 This library is distributed in the hope that it will be useful, but WITHOUT
 ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or
-FITNESS FOR A PARTICULAR PURPOSE.  See the GNU Lesser General Public
-License for more details.
+FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General Public License
+for more details.
 
 You should have received a copy of the GNU Lesser General Public License
 along with this library; if not, write to the Free Software Foundation,
-Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301  USA
-
-.. _Total Phase: http://www.totalphase.com
-.. |I2C| replace:: I\ :sup:`2`\ C
-.. |BuildStatus| image:: https://travis-ci.org/kontron/python-aardvark.png?branch=master
-                 :target: https://travis-ci.org/kontron/python-aardvark
-.. |PyPiVersion| image:: https://badge.fury.io/py/pyaardvark.svg
-                 :target: http://badge.fury.io/py/pyaardvark
-.. |PyPiPythonVersions| image:: https://img.shields.io/pypi/pyversions/pyaardvark.svg
-                        :alt: Python versions
-                        :target: http://badge.fury.io/py/pyaardvark
+Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyaardvark-0.7.1/docs/conf.py` & `pyaardvark-0.8.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyaardvark-0.7.1/docs/intro.rst` & `pyaardvark-0.8.1/docs/intro.rst`

 * *Files identical despite different names*

### Comparing `pyaardvark-0.7.1/pyaardvark/__init__.py` & `pyaardvark-0.8.1/pyaardvark/__init__.py`

 * *Files identical despite different names*

### Comparing `pyaardvark-0.7.1/pyaardvark/aardvark.py` & `pyaardvark-0.8.1/pyaardvark/aardvark.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,48 +14,18 @@
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301  USA
 
 from builtins import bytes
 import array
 import logging
-import sys
 
 from .constants import *
-
-if sys.platform.startswith('linux'):
-    try:
-        from .ext.linux32 import aardvark as api
-    except ImportError:
-        try:
-            from .ext.linux64 import aardvark as api
-        except ImportError:
-            api = None
-elif sys.platform.startswith('win32'):
-    try:
-        from .ext.win32 import aardvark as api
-    except ImportError:
-        try:
-            from .ext.win64 import aardvark as api
-        except ImportError:
-            api = None
-elif sys.platform.startswith('darwin'):
-    try:
-        from .ext.osx64 import aardvark as api
-    except ImportError:
-        try:
-            from .ext.osxarm import aardvark as api
-        except ImportError:
-            api = None
-else:
-    api = None
-
-if not api:
-    raise RuntimeError('Unable to find suitable binary interface. '
-            'Unsupported platform?')
+from .constants import *
+from .ext import api
 
 log = logging.getLogger(__name__)
 
 def _raise_error_if_negative(val):
     """Raises an :class:`IOError` if `val` is negative."""
     if val < 0:
         raise IOError(val, api.py_aa_status_string(val))
@@ -474,16 +444,15 @@
         if timeout is None:
             timeout = -1
 
         ret = api.py_aa_async_poll(self.handle, timeout)
         _raise_error_if_negative(ret)
 
         events = list()
-        for event in (POLL_I2C_READ, POLL_I2C_WRITE, POLL_SPI,
-                POLL_I2C_MONITOR):
+        for event in (POLL_I2C_READ, POLL_I2C_WRITE, POLL_SPI):
             if ret & event:
                 events.append(event)
         return events
 
     def enable_i2c_slave(self, slave_address):
         """Enable I2C slave mode.
 
@@ -542,52 +511,14 @@
     @property
     def i2c_slave_last_transmit_size(self):
         """Returns the number of bytes transmitted by the slave."""
         ret = api.py_aa_i2c_slave_write_stats(self.handle)
         _raise_error_if_negative(ret)
         return ret
 
-    def enable_i2c_monitor(self):
-        """Activate the I2C monitor.
-
-        Enabling the monitor will disable all other functions of the adapter.
-
-        Raises an :exc:`IOError` if the hardware adapter does not support
-        monitor mode.
-        """
-        ret = api.py_aa_i2c_monitor_enable(self.handle)
-        _raise_error_if_negative(ret)
-
-    def disable_i2c_monitor(self):
-        """Disable the I2C monitor.
-
-        Raises an :exc:`IOError` if the hardware adapter does not support
-        monitor mode.
-        """
-        ret = api.py_aa_i2c_monitor_disable(self.handle)
-        _raise_error_if_negative(ret)
-
-    def i2c_monitor_read(self):
-        """Retrieved any data fetched by the monitor.
-
-        This function has an integrated timeout mechanism. You should use
-        :func:`poll` to determine if there is any data available.
-
-        Returns a list of data bytes and special symbols. There are three
-        special symbols: `I2C_MONITOR_NACK`, I2C_MONITOR_START and
-        I2C_MONITOR_STOP.
-
-        """
-        data = array.array('H', (0,) * self.BUFFER_SIZE)
-        ret = api.py_aa_i2c_monitor_read(self.handle, self.BUFFER_SIZE,
-                data)
-        _raise_error_if_negative(ret)
-        del data[ret:]
-        return data.tolist()
-
     @property
     def spi_bitrate(self):
         """SPI bitrate in kHz. Not every bitrate is supported by the host
         adapter. Therefore, the actual bitrate may be less than the value which
         is set. The slowest bitrate supported is 125kHz. Any smaller value will
         be rounded up to 125kHz.
```

### Comparing `pyaardvark-0.7.1/pyaardvark/cli_tool.py` & `pyaardvark-0.8.1/pyaardvark/cli_tool.py`

 * *Files 7% similar despite different names*

```diff
@@ -67,35 +67,14 @@
     print_hex(data)
 
 def scan(a, args):
     for dev in pyaardvark.find_devices():
         dev['in_use'] = ' [IN USE]' if dev['in_use'] else ''
         print('Device #%(port)d: %(serial_number)s%(in_use)s' % dev)
 
-def monitor(a, args):
-    def data_to_str(d):
-        if d == pyaardvark.I2C_MONITOR_START:
-            return 'STA'
-        elif d == pyaardvark.I2C_MONITOR_STOP:
-            return 'STP\n'
-        elif d == pyaardvark.I2C_MONITOR_NACK:
-            return '*'
-        else:
-            return '%02x' % d
-
-    a.enable_i2c_monitor()
-    try:
-        while True:
-            a.poll()
-            data = a.i2c_monitor_read()
-            data = map(data_to_str, data)
-            print(*data, end='')
-    except KeyboardInterrupt:
-        print()
-
 def main(args=None):
     parser = argparse.ArgumentParser(
             description='Total Phase I2C/SPI host adapter CLI.')
     parser.add_argument('-v', action='store_true', dest='verbose',
             help='be more verbose')
     parser.add_argument('-d', '--device', type=int, dest='device', default=0,
             help='set device number')
@@ -113,18 +92,14 @@
     _sub = parser.add_subparsers(title='Commands')
 
     # scan sub command
     subparser = _sub.add_parser('scan',
             help='Find attached Aardvark devices')
     subparser.set_defaults(func=scan)
 
-    # monitor sub command
-    subparser = _sub.add_parser('monitor', help='Listen on I2C bus')
-    subparser.set_defaults(func=monitor)
-
     # spi subcommand
     subparser = _sub.add_parser('spi', help='SPI commands')
     subparser.add_argument('data', nargs='+', type=byte, metavar="DATA",
             help='byte to write')
     subparser.set_defaults(func=spi)
 
     # i2c subcommand
```

### Comparing `pyaardvark-0.7.1/pyaardvark/constants.py` & `pyaardvark-0.8.1/pyaardvark/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -135,19 +135,14 @@
 TARGET_POWER_BOTH = 0x03
 TARGET_POWER_QUERY = 0x80
 
 POLL_NO_DATA = 0x00
 POLL_I2C_READ = 0x01
 POLL_I2C_WRITE = 0x02
 POLL_SPI = 0x04
-POLL_I2C_MONITOR = 0x08
-
-I2C_MONITOR_NACK = 0x0100
-I2C_MONITOR_START = 0xff00
-I2C_MONITOR_STOP = 0xff01
 
 I2C_STATUS_OK = 0
 I2C_STATUS_BUS_ERROR = 1
 I2C_STATUS_SLA_ACK = 2
 I2C_STATUS_SLA_NACK = 3
 I2C_STATUS_DATA_NACK = 4
 I2C_STATUS_ARB_LOST = 5
```

### Comparing `pyaardvark-0.7.1/pyaardvark/ext/LICENSE.txt` & `pyaardvark-0.8.1/pyaardvark/ext/LICENSE.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,129 +1,139 @@
-                          LICENSE AGREEMENT
+                     END USER LICENSE AGREEMENT
 
-               Aardvark I2C/SPI Software and Firmware
-              Copyright (c) 2003-2022 Total Phase, Inc.
+                   Aardvark Software and Firmware
+             Copyright (c) 2003-2024 Total Phase, Inc.
                         All rights reserved.
 
 
 PREAMBLE:
   The accompanying software, firmware, documentation, and related
   materials ("Product") are the sole property of Total Phase, Inc.
-  ("Total Phase").  Its use and distribution is subject to the
-  terms in this License Agreement ("Agreement").
+  ("Total Phase").  Its use and distribution are subject to the
+  terms in this License Agreement ("Agreement").  This Agreement
+  applies to all uses of the Product including whether the Product
+  is downloaded directly from Total Phase or the Product is obtained
+  as part of a package from a third party.
 
   By the use or distribution of the Product, you are consenting to
   be bound by the terms of this Agreement.  If you do not agree, do
   not use or distribute the Product in whole or in part.
 
 
 TERMS OF USE:
-  Permission to use, copy, modify, and distribute the Product
-  is hereby granted, subject to the conditions stated below:
+  Permission to use, copy, and distribute the Product is hereby
+  granted, subject to the following conditions:
 
-  a. The Product is licensed only for use with other Total Phase
-     products.  Any other use is permitted only with the express
-     written permission of Total Phase.
-
-  b. The Product may only be copied unmodified in its entirety,
-     with all of the files intact including a verbatim copy of this
-     Agreement.  Distribution of modified copies is permitted only
-     with the express written permission of Total Phase.
-
-  c. The Product must not be placed on any publicly-accessible
-     Internet server including, but not limited to, web servers, ftp
-     servers, and file sharing systems.  Instead, a link should be
-     placed to the Total Phase website where the latest versions
-     may be obtained.
-
-  d. As a special exemption, a copy of the shared object file,
-     aardvark.dll or aardvark.so ("Shared Object File"), may be
-     distributed separately from the Product, provided that it is part
-     of a separate work ("Separate Work").  Such Shared Object Files
-     carry with them all of the rights and limitations outlined in
-     this Agreement, except that it may not be further distributed
-     unless part of the Separate Work.
-
-     Before publicly distributing the Shared Object Files, whether
-     gratis or for a fee, you must notify Total Phase by electronic
-     mail to: sales@totalphase.com to the attention of General
-     Manager. Provide a description of the Separate Work, specifically
-     mentioning how any Total Phase hardware and the Shared Object
-     Files will be integrated into the Separate Work and your proposed
-     method of distribution. Total Phase will acknowledge the
-     notification within one week.
-
-     You are required to include a copy of this Agreement with your
-     Separate Work.
-
-  e. Any separate works which include the Product must be plainly
-     marked as such, and must not be misrepresented as the original
-     software.
-
-  f. You may not modify, translate, reverse-engineer, decompile,
-     disassemble (except and solely to the extent that an applicable
-     statute expressly and specifically prohibits such restrictions),
-     or create derivative works of the Product.  A separate work
-     that only makes use of the unmodified shared object file is not
-     considered a derivative work.
+  The Product is licensed only for use with other Total Phase
+  products.  Any other use is permitted only with the express
+  written permission of Total Phase.
+
+  The Product may only be copied unmodified in its entirety, with
+  all of the files intact including a verbatim copy of this
+  Agreement.  Distribution of modified copies is permitted only with
+  the express written permission of Total Phase.
+
+  The Product must not be placed on any publicly-accessible Internet
+  server including but not limited to web servers, ftp servers, and
+  file sharing systems.  Instead, a link should be placed to the
+  Total Phase website where the latest versions may be obtained.
+
+  You may not modify, translate, reverse-engineer, decompile,
+  disassemble (except and solely to the extent that an applicable
+  statute expressly and specifically prohibits such restrictions),
+  or create derivative works of the Product.
+
+
+SEPARATE WORK:
+  A separate work that only makes use of the shared library files
+  aardvark.dll, aardvark.so, aardvark_net.dll, or aardvark_py.py
+  without modification is not a derivative work and is considered a
+  "Separate Work".
+
+  You may distribute a Separate Work to a third party only if you
+  comply with all of the following: (i) you obtained the Product
+  directly from Total Phase; (ii) you notify Total Phase in writing
+  via electronic mail to sales@totalphase.com with a description of
+  the Separate Work and your method of distribution; (iii) you
+  receive written approval from Total Phase; (iv) you label or mark
+  the Separate Work in a way that clearly distinguishes it from the
+  Product; and (v) you include this End User License Agreement with
+  the Separate Work.
 
 
 PROPRIETARY RIGHTS:
   The Product is owned by Total Phase and is protected by United
   States copyright laws and international treaty provisions.  All
   copyright, patent, trade secret, trademarks, and other intellectual
-  and proprietary rights in the Product are and shall remain the
+  and proprietary rights in the Product are and will remain the
   valuable property of Total Phase.  You agree to take all necessary
   steps to ensure that this property is protected and that the
   provisions of this Agreement are not violated by you or by any
   person under your control or in your service.
 
 
 TERMINATION:
   Your rights under this license will terminate automatically if you
   fail to comply with the terms and conditions set forth herein.
 
-  If any provision of this license agreement is held to be
-  unenforceable, that provision shall be reformed only to the extent
-  necessary to make it enforceable; and the balance of this license
-  agreement shall remain in full force and effect.
+  If any provision of this Agreement is held to be unenforceable,
+  that provision should be reformed only to the extent required to
+  comply with law while preserving the original intent as much as
+  possible; the balance of this Agreement will remain in full force
+  and effect.
 
 
 SAFETY-CRITICAL SYSTEMS POLICY:
-  The Product is not authorized for use in life support devices or
-  systems.  Life support devices or systems include, but are not
-  limited to, surgical implants, medical systems, and other
-  safety-critical systems in which failure of a Total Phase product
-  could cause personal injury or loss of life.
-
-  The Product is not fault-tolerant and is not designed, manufactured
-  or intended for use or resale in hazardous environments requiring
-  fail-safe performance, such as in the operation of nuclear facilities,
-  aircraft navigation or communication systems, air traffic control,
-  or weapons systems, in which the failure of the Product could lead
-  directly to death, personal injury, or severe physical or environ-
-  mental damage.  Such use is unauthorized by Total Phase.
-
-  Should the Product be used in any such unauthorized manner, Buyer
-  agrees to indemnify and hold harmless Total Phase, its officers,
-  employees, affiliates, and distributors from any and all claims
-  arising from such use, even if such claim alleges that Total Phase
+  You may not use the Product in life support devices or systems.
+  Life support devices or systems include, but are not limited to,
+  surgical implants, medical systems, and other safety-critical
+  systems in which failure of a Total Phase product could cause
+  personal injury or loss of life.
+
+  The Product is not fault-tolerant and is not designed, manufactured,
+  or allowed for use or resale in hazardous environments requiring
+  fail-safe performance, such as in the operation of nuclear
+  facilities, aircraft navigation or communication systems, air
+  traffic control, or weapons systems, in which the failure of the
+  Product could lead directly to death, personal injury, or severe
+  physical or environmental damage.
+
+
+INDEMNITY:
+  You agree to indemnify, defend, and hold harmless Total Phase, its
+  officers, employees, affiliates, and distributors from any and all
+  claims and costs, including reasonable legal fees, arising from your
+  breach of this Agreement, use of the Product, use or distribution
+  of a Separate Work, any claim that a Separate Work infringes the
+  intellectual property or proprietary right of a third party, or your
+  act, error, or omission, even if such claim alleges that Total Phase
   was negligent in the design or manufacture of the Product.
 
 
 DISCLAIMER:
-  THE PRODUCT IS PROVIDED "AS IS," WITHOUT WARRANTY OF ANY KIND.
-  THE COPYRIGHT HOLDER(S) AND TOTAL PHASE DISCLAIM ANY AND ALL
-  WARRANTIES, WHETHER EXPRESSED OR IMPLIED, INCLUDING BUT NOT
-  LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
-  PARTICULAR PURPOSE AND NON-INFRINGEMENT.
-
-  IN NO EVENT SHALL THE COPYRIGHT HOLDER(S), TOTAL PHASE, ITS
-  OFFICERS, EMPLOYEES, AFFILIATES, AND DISTRIBUTORS BE LIABLE FOR
-  ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
-  CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT
-  OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR
-  BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
-  LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
-  (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE
-  USE OF THE PRODUCT, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH
-  DAMAGE.
+  THE PRODUCT IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND.
+  TOTAL PHASE DISCLAIMS ANY AND ALL WARRANTIES, WHETHER EXPRESSED OR
+  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
+  MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE, AND
+  NON-INFRINGEMENT.
+
+
+LIMITATION OF LIABILITY:
+  IN NO EVENT WILL TOTAL PHASE, ITS OFFICERS, EMPLOYEES, OR
+  AFFILIATES BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
+  SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING BUT NOT
+  LIMITED TO PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF
+  USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED
+  AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT
+  LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN
+  ANY WAY OUT OF THE USE OF THE PRODUCT, EVEN IF ADVISED OF THE
+  POSSIBILITY OF SUCH DAMAGE.
+
+
+GENERAL:
+  The failure of either party to enforce its rights under this
+  Agreement at any time for any period will not be construed as a
+  waiver of such rights.
+
+  This Agreement will be governed by and construed pursuant to the
+  laws of the State of California, without regard to conflict of
+  laws principles.
```

### Comparing `pyaardvark-0.7.1/pyaardvark.egg-info/PKG-INFO` & `pyaardvark-0.8.1/pyaardvark.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,116 +1,103 @@
 Metadata-Version: 2.1
 Name: pyaardvark
-Version: 0.7.1
+Version: 0.8.1
 Summary: Total Phase Aardvark library
 Home-page: http://github.com/kontron/python-aardvark
 Author: Michael Walle
 Author-email: michael.walle@kontron.com
 License: LGPLv2+
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Description-Content-Type: text/markdown
 License-File: COPYING
 License-File: AUTHORS
+Requires-Dist: future
 
-Python binding for Total Phase Aardvark
-=======================================
+# Python binding for Total Phase Aardvark
 
-|BuildStatus| |PyPiVersion| |PyPiPythonVersions|
+![BuildStatus](https://github.com/kontron/python-aardvark/actions/workflows/python-package.yml/badge.svg)
+![PyPiVersion](https://badge.fury.io/py/pyaardvark.svg)
+![Python versions](https://img.shields.io/pypi/pyversions/pyaardvark.svg)
 
-The `Total Phase`_ Aardvark is an USB |I2C|/SPI host adapter.
+The [Total Phase](http://www.totalphase.com) Aardvark is an USB I²C/SPI
+host adapter.
 
+## Rationale
 
-Rationale
----------
-
-The manufacturer already provides an python binding. So why a new one? This
-is correct, but the python binding you can find in the
-``aardvark-linux-api`` package is very C oriented. Eg. you need to pass
+The manufacturer already provides an python binding. So why a new one?
+This is correct, but the python binding you can find in the
+`aardvark-linux-api` package is very C oriented. Eg. you need to pass
 arrays as method parameters, which are then modified by the binding.
 Instead, this binding tries to be more pythonic.
 
+## Features
 
-Features
---------
-
-* simple interface
-* CLI tool for easy testing
-* |I2C| and SPI support
-* support for control signals like target power and internal |I2C| pullups
-* rudimental |I2C| slave support
-* Support for Linux, Windows and OSX
-
-
-(Still) Missing Features
-------------------------
+- simple interface
+- CLI tool for easy testing
+- I²C and SPI support
+- support for control signals like target power and internal I²C
+  pullups
+- rudimental I²C slave support
+- Support for Linux, Windows and OSX
 
-* more documentation (please bear with me)
-* GPIO support
+## (Still) Missing Features
 
+- more documentation (please bear with me)
+- GPIO support
 
-Documentation
--------------
+## Documentation
 
 You can find the most up to date documentation at:
-http://pyaardvark.rtfd.org
+<http://pyaardvark.rtfd.org>
 
+## Requirements
 
-Requirements
-------------
+You need an either an x86, an amd64, an aarch64, an arm32 or a M1 machine. This
+is because the binding uses a binary-only module supplied by the manufacturer,
+Total Phase. Linux, Windows, and OSX are supported.
 
-You need an either a x86 or an amd64 machine. This is because the binding
-uses a binary-only module supplied by the manufacturer, Total Phase.
-Linux, Windows, and OSX is supported.
+### Python 2.7 support
 
+The last version with python 2.7 support is 0.7.1.
 
-Contributing
-------------
+### Monitor support
 
-Contributions are always welcome. You may send patches directly (eg. ``git
-send-email``), do a github pull request or just file an issue.
+Total Phase removed the monitor support in their binary modules in version 6.00.
+The last pyaardvark version which use the old binaries and thus still support
+montoring is 0.7.x.
 
-If you are doing code changes or additions please:
+## Contributing
 
-* respect the coding style (eg. PEP8),
-* provide well-formed commit message (see `this blog post
-  <http://tbaggery.com/2008/04/19/a-note-about-git-commit-messages.html>`_.)
-* add a Signed-off-by line (eg. ``git commit -s``)
+Contributions are always welcome. You may send patches directly (eg. `git
+send-email`), do a github pull request or just file an issue.
 
+If you are doing code changes or additions please:
+- respect the coding style (eg. PEP8),
+- provide well-formed commit message (see [this blog
+  post](http://tbaggery.com/2008/04/19/a-note-about-git-commit-messages.html).)
+- add a Signed-off-by line (eg. `git commit -s`)
 
-License
--------
+## License
 
 This library is free software; you can redistribute it and/or modify it
 under the terms of the GNU Lesser General Public License as published by
 the Free Software Foundation; either version 2.1 of the License, or (at
 your option) any later version.
 
 This library is distributed in the hope that it will be useful, but WITHOUT
 ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or
-FITNESS FOR A PARTICULAR PURPOSE.  See the GNU Lesser General Public
-License for more details.
+FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General Public License
+for more details.
 
 You should have received a copy of the GNU Lesser General Public License
 along with this library; if not, write to the Free Software Foundation,
-Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301  USA
-
-.. _Total Phase: http://www.totalphase.com
-.. |I2C| replace:: I\ :sup:`2`\ C
-.. |BuildStatus| image:: https://travis-ci.org/kontron/python-aardvark.png?branch=master
-                 :target: https://travis-ci.org/kontron/python-aardvark
-.. |PyPiVersion| image:: https://badge.fury.io/py/pyaardvark.svg
-                 :target: http://badge.fury.io/py/pyaardvark
-.. |PyPiPythonVersions| image:: https://img.shields.io/pypi/pyversions/pyaardvark.svg
-                        :alt: Python versions
-                        :target: http://badge.fury.io/py/pyaardvark
+Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyaardvark-0.7.1/pyaardvark.egg-info/SOURCES.txt` & `pyaardvark-0.8.1/pyaardvark.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 AUTHORS
 COPYING
 MANIFEST.in
-README.rst
+README.md
 setup.py
 docs/api.rst
 docs/conf.py
-docs/conf.py~
 docs/defines.rst.inc
 docs/index.rst
 docs/intro.rst
-docs/intro.rst~
 pyaardvark/__init__.py
 pyaardvark/aardvark.py
 pyaardvark/cli_tool.py
 pyaardvark/constants.py
 pyaardvark/version.py
 pyaardvark.egg-info/PKG-INFO
 pyaardvark.egg-info/SOURCES.txt
@@ -23,18 +21,24 @@
 pyaardvark.egg-info/top_level.txt
 pyaardvark/ext/LICENSE.txt
 pyaardvark/ext/__init__.py
 pyaardvark/ext/linux32/__init__.py
 pyaardvark/ext/linux32/aardvark.so
 pyaardvark/ext/linux64/__init__.py
 pyaardvark/ext/linux64/aardvark.so
+pyaardvark/ext/linuxarm32/__init__.py
+pyaardvark/ext/linuxarm32/aardvark.so
+pyaardvark/ext/linuxarm64/__init__.py
+pyaardvark/ext/linuxarm64/aardvark.so
 pyaardvark/ext/osx64/__init__.py
 pyaardvark/ext/osx64/aardvark.so
 pyaardvark/ext/osxarm/__init__.py
 pyaardvark/ext/osxarm/aardvark.so
 pyaardvark/ext/win32/__init__.py
 pyaardvark/ext/win32/aardvark.pyd
 pyaardvark/ext/win64/__init__.py
 pyaardvark/ext/win64/aardvark.pyd
+pyaardvark/ext/winarm/__init__.py
+pyaardvark/ext/winarm/aardvark.pyd
 tests/__init__.py
 tests/test_aardvark.py
 tests/test_ext.py
```

### Comparing `pyaardvark-0.7.1/setup.py` & `pyaardvark-0.8.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -27,44 +27,41 @@
         with open(version_py, 'r') as f:
             d = dict()
             exec(f.read(), d)
             version = d['__version__']
     except IOError:
         version = 'unknown'
 
-with open('README.rst') as f:
+with open('README.md') as f:
     readme = f.read()
 
 setup(name = name,
         version = version,
         description = 'Total Phase Aardvark library',
+        long_description_content_type = 'text/markdown',
         long_description = readme,
         author = 'Michael Walle',
         author_email = 'michael.walle@kontron.com',
         packages = find_packages(),
         url = 'http://github.com/kontron/python-aardvark',
         license = 'LGPLv2+',
         classifiers = [
             'Development Status :: 3 - Alpha',
             'Environment :: Console',
             'License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)',
             'Natural Language :: English',
             'Operating System :: OS Independent',
-            'Programming Language :: Python :: 2',
-            'Programming Language :: Python :: 2.7',
             'Programming Language :: Python :: 3',
-            'Programming Language :: Python :: 3.4',
-            'Programming Language :: Python :: 3.5',
-            'Programming Language :: Python :: 3.6',
-            'Programming Language :: Python :: 3.7',
-            'Programming Language :: Python :: 3.8',
+            'Programming Language :: Python :: 3.9',
+            'Programming Language :: Python :: 3.10',
+            'Programming Language :: Python :: 3.11',
+            'Programming Language :: Python :: 3.12',
             'Topic :: Software Development :: Libraries :: Python Modules',
         ],
         entry_points = {
             'console_scripts': [
                 'aardvark = pyaardvark.cli_tool:main',
             ]
         },
-        test_suite = 'tests',
         include_package_data = True,
         install_requires = ['future'],
 )
```

### Comparing `pyaardvark-0.7.1/tests/test_aardvark.py` & `pyaardvark-0.8.1/tests/test_aardvark.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 #!/usr/bin/env python
 
-import nose
 import array
 from mock import patch, call, ANY
 import pyaardvark
 from pyaardvark.constants import *
-from nose.tools import eq_, raises, assert_raises
+import pytest
 
 
 @patch('pyaardvark.aardvark.api', autospec=True)
 def test_api_version(api):
     api.py_version.return_value = 83887390
     v = pyaardvark.api_version()
     api.py_version.assert_called_once_with()
-    eq_(v, "5.30")
+    assert v == "5.30"
 
 @patch('pyaardvark.aardvark.api', autospec=True)
 def test_open_default(api):
     api.py_aa_open_ext.return_value = (42, (0,) * 6)
     a = pyaardvark.open()
     api.py_aa_open_ext.assert_called_once_with(0)
-    eq_(a.handle, api.py_aa_open_ext.return_value[0])
+    assert a.handle == api.py_aa_open_ext.return_value[0]
 
 @patch('pyaardvark.aardvark.api', autospec=True)
 def test_find_devices_valid_devices(api):
     def f(num, devices):
         return 2
 
     def f_ext(num, num_ids, devices, ids):
@@ -41,28 +40,28 @@
     devs = pyaardvark.find_devices()
     api.py_aa_find_devices.assert_has_calls([
         call(0, array.array('H')),
     ])
     api.py_aa_find_devices_ext.assert_has_calls([
         call(2, 2, ANY, ANY),
     ])
-    eq_(len(devs), 2)
-    eq_(devs[0]['port'], 42)
-    eq_(devs[0]['serial_number'], '1234-567890')
-    eq_(devs[0]['in_use'], True)
-    eq_(devs[1]['port'], 4711)
-    eq_(devs[1]['serial_number'], '1111-222222')
-    eq_(devs[1]['in_use'], False)
+    assert len(devs) == 2
+    assert devs[0]['port'] == 42
+    assert devs[0]['serial_number'] == '1234-567890'
+    assert devs[0]['in_use']
+    assert devs[1]['port'] == 4711
+    assert devs[1]['serial_number'] == '1111-222222'
+    assert not devs[1]['in_use']
 
 @patch('pyaardvark.aardvark.api', autospec=True)
 def test_open_port(api):
     api.py_aa_open_ext.return_value = (42, (0,) * 6)
     a = pyaardvark.open(4711)
     api.py_aa_open_ext.assert_called_once_with(4711)
-    eq_(a.handle, api.py_aa_open_ext.return_value[0])
+    assert a.handle == api.py_aa_open_ext.return_value[0]
 
 @patch('pyaardvark.aardvark.api', autospec=True)
 def test_open_serial_number(api):
     devices = {
             42: 1234567890,
             4711: 1111222222,
             5: 3333444444,
@@ -87,188 +86,189 @@
 
     api.py_aa_find_devices.side_effect = f
     api.py_aa_find_devices_ext.side_effect = f_ext
     api.py_aa_open_ext.side_effect = open
     api.py_aa_unique_id.side_effect = unique_id
 
     a = pyaardvark.open(serial_number='1234-567890')
-    eq_(a.handle, 42)
+    assert a.handle == 42
 
     a = pyaardvark.open(serial_number='1111-222222')
-    eq_(a.handle, 4711)
+    assert a.handle == 4711
 
-    assert_raises(IOError, pyaardvark.open, serial_number='7777-888888')
+    with pytest.raises(IOError):
+        pyaardvark.open(serial_number='7777-888888')
 
 @patch('pyaardvark.aardvark.api', autospec=True)
 def test_open_versions(api):
     api.py_aa_open_ext.return_value = (1, (0x101, 0x202, 0x303, 0, 0, 0))
     a = pyaardvark.open()
-    eq_(a.api_version, '1.01')
-    eq_(a.firmware_version, '2.02')
-    eq_(a.hardware_revision, '3.03')
+    assert a.api_version == '1.01'
+    assert a.firmware_version == '2.02'
+    assert a.hardware_revision == '3.03'
 
 @patch('pyaardvark.aardvark.api', autospec=True)
-@raises(IOError)
 def test_open_error(api):
-    api.py_aa_open_ext.return_value = (-1, (0,) * 6)
-    pyaardvark.open()
+    with pytest.raises(IOError):
+        api.py_aa_open_ext.return_value = (-1, (0,) * 6)
+        pyaardvark.open()
 
 @patch('pyaardvark.aardvark.api', autospec=True)
-@raises(IOError)
 def test_open_version_check_firmware(api):
-    api.py_aa_open_ext.return_value = (1, (0, 100, 0, 0, 200, 0))
-    pyaardvark.open()
+    with pytest.raises(IOError):
+        api.py_aa_open_ext.return_value = (1, (0, 100, 0, 0, 200, 0))
+        pyaardvark.open()
 
 @patch('pyaardvark.aardvark.api', autospec=True)
-@raises(IOError)
 def test_open_version_check_api(api):
-    api.py_aa_open_ext.return_value = (1, (100, 0, 0, 200, 0, 0))
-    pyaardvark.open()
+    with pytest.raises(IOError):
+        api.py_aa_open_ext.return_value = (1, (100, 0, 0, 200, 0, 0))
+        pyaardvark.open()
 
 @patch('pyaardvark.aardvark.api', autospec=True)
 class TestAardvark(object):
     @patch('pyaardvark.aardvark.api', autospec=True)
-    def setup(self, api):
+    def setup_method(self, method, api):
         api.py_aa_open_ext.return_value = (1, (0,) * 6)
         self.a = pyaardvark.open()
 
     def test_close(self, api):
         handle = self.a.handle
         self.a.close()
         api.py_aa_close.assert_called_once_with(handle)
 
     def test_context_manager(self, api):
         api.py_aa_open_ext.return_value = (1, (0,) * 6)
         with pyaardvark.open() as a:
-            eq_(a.handle, api.py_aa_open_ext.return_value[0])
+            assert a.handle == api.py_aa_open_ext.return_value[0]
             api.py_aa_open_ext.assert_called_once_with(0)
         api.py_aa_close.assert_called_once_with(
                 api.py_aa_open_ext.return_value[0])
 
     def test_unique_id(self, api):
         api.py_aa_unique_id.return_value = 3627028473
         unique_id = self.a.unique_id()
         api.py_aa_unique_id.assert_called_once_with(self.a.handle)
-        eq_(unique_id, api.py_aa_unique_id.return_value)
+        assert unique_id == api.py_aa_unique_id.return_value
 
     def test_unique_id_str(self, api):
         api.py_aa_unique_id.return_value = 627008473
         unique_id_str = self.a.unique_id_str()
         api.py_aa_unique_id.assert_called_once_with(self.a.handle)
-        eq_(unique_id_str, '0627-008473')
+        assert unique_id_str == '0627-008473'
 
     def test_enable_i2c_1(self, api):
         api.py_aa_configure.return_value = CONFIG_SPI_GPIO
-        eq_(self.a.enable_i2c, False)
+        assert not self.a.enable_i2c
         self.a.enable_i2c = True
         api.py_aa_configure.assert_called_with(self.a.handle, CONFIG_SPI_I2C)
 
     def test_enable_i2c_2(self, api):
         api.py_aa_configure.return_value = CONFIG_GPIO_ONLY
-        eq_(self.a.enable_i2c, False)
+        assert not self.a.enable_i2c
         self.a.enable_i2c = True
         api.py_aa_configure.assert_called_with(self.a.handle, CONFIG_GPIO_I2C)
 
     def test_enable_i2c_3(self, api):
         api.py_aa_configure.return_value = CONFIG_GPIO_I2C
-        eq_(self.a.enable_i2c, True)
+        assert self.a.enable_i2c
         self.a.enable_i2c = False
         api.py_aa_configure.assert_called_with(self.a.handle, CONFIG_GPIO_ONLY)
 
     def test_enable_i2c_4(self, api):
         api.py_aa_configure.return_value = CONFIG_SPI_I2C
-        eq_(self.a.enable_i2c, True)
+        assert self.a.enable_i2c
         self.a.enable_i2c = False
         api.py_aa_configure.assert_called_with(self.a.handle, CONFIG_SPI_GPIO)
 
-    @raises(IOError)
     def test_enable_i2c_error(self, api):
-        api.py_aa_configure.return_value = -1
-        self.a.enable_i2c = True
+        with pytest.raises(IOError):
+            api.py_aa_configure.return_value = -1
+            self.a.enable_i2c = True
 
     def test_enable_spi_1(self, api):
         api.py_aa_configure.return_value = CONFIG_GPIO_I2C
-        eq_(self.a.enable_spi, False)
+        assert not self.a.enable_spi
         self.a.enable_spi = True
         api.py_aa_configure.assert_called_with(self.a.handle, CONFIG_SPI_I2C)
 
     def test_enable_spi_2(self, api):
         api.py_aa_configure.return_value = CONFIG_GPIO_ONLY
-        eq_(self.a.enable_spi, False)
+        assert not self.a.enable_spi
         self.a.enable_spi = True
         api.py_aa_configure.assert_called_with(self.a.handle, CONFIG_SPI_GPIO)
 
     def test_enable_spi_3(self, api):
         api.py_aa_configure.return_value = CONFIG_SPI_GPIO
-        eq_(self.a.enable_spi, True)
+        assert self.a.enable_spi
         self.a.enable_spi = False
         api.py_aa_configure.assert_called_with(self.a.handle, CONFIG_GPIO_ONLY)
 
     def test_enable_spi_4(self, api):
         api.py_aa_configure.return_value = CONFIG_SPI_I2C
-        eq_(self.a.enable_spi, True)
+        assert self.a.enable_spi
         self.a.enable_spi = False
         api.py_aa_configure.assert_called_with(self.a.handle, CONFIG_GPIO_I2C)
 
-    @raises(IOError)
     def test_enable_spi_error(self, api):
-        api.py_aa_configure.return_value = -1
-        self.a.enable_spi = True
+        with pytest.raises(IOError):
+            api.py_aa_configure.return_value = -1
+            self.a.enable_spi = True
 
     def test_i2c_bitrate(self, api):
         api.py_aa_i2c_bitrate.return_value = 100
         self.a.i2c_bitrate = 4711
-        eq_(self.a.i2c_bitrate, 100)
+        assert self.a.i2c_bitrate == 100
 
         api.py_aa_i2c_bitrate.assert_has_calls([
                 call(self.a.handle, 4711),
                 call(self.a.handle, 0),
         ])
 
-    @raises(IOError)
     def test_i2c_bitrate_error(self, api):
-        api.py_aa_i2c_bitrate.return_value = -1
-        self.a.i2c_bitrate = 0
+        with pytest.raises(IOError):
+            api.py_aa_i2c_bitrate.return_value = -1
+            self.a.i2c_bitrate = 0
 
     def test_i2c_pullups(self, api):
         api.py_aa_i2c_pullup.return_value = 0
         self.a.i2c_pullups = False
         self.a.i2c_pullups = True
         pullup = self.a.i2c_pullups
         api.py_aa_i2c_pullup.assert_has_calls([
             call(self.a.handle, pyaardvark.I2C_PULLUP_NONE),
             call(self.a.handle, pyaardvark.I2C_PULLUP_BOTH),
             call(self.a.handle, pyaardvark.I2C_PULLUP_QUERY),
         ])
 
-    @raises(IOError)
     def test_i2c_pullups_error(self, api):
-        api.py_aa_i2c_pullup.return_value = -1
-        _ = self.a.i2c_pullups
+        with pytest.raises(IOError):
+            api.py_aa_i2c_pullup.return_value = -1
+            _ = self.a.i2c_pullups
 
     def test_enable_target_power(self, api):
         api.py_aa_target_power.return_value = 0
         self.a.target_power = False
         self.a.target_power = True
         _ = self.a.target_power
         api.py_aa_target_power.assert_has_calls([
             call(self.a.handle, pyaardvark.TARGET_POWER_NONE),
             call(self.a.handle, pyaardvark.TARGET_POWER_BOTH),
             call(self.a.handle, pyaardvark.TARGET_POWER_QUERY),
         ])
 
-    @raises(IOError)
     def test_enable_target_power_error(self, api):
-        api.py_aa_target_power.return_value = -1
-        self.a.target_power = 0
+        with pytest.raises(IOError):
+            api.py_aa_target_power.return_value = -1
+            self.a.target_power = 0
 
     def test_i2c_bus_timeout(self, api):
         api.py_aa_i2c_bus_timeout.return_value = 10
         self.a.i2c_bus_timeout = 300
-        eq_(self.a.i2c_bus_timeout, 10)
+        assert self.a.i2c_bus_timeout == 10
 
         api.py_aa_i2c_bus_timeout.assert_has_calls([
                 call(self.a.handle, 300),
                 call(self.a.handle, 0),
         ])
 
     def test_i2c_master_write(self, api):
@@ -282,268 +282,226 @@
 
     def test_i2c_master_write_default_flags(self, api):
         api.py_aa_i2c_write_ext.return_value = (I2C_STATUS_OK, 0)
         self.a.i2c_master_write(0, b'')
         api.py_aa_i2c_write_ext.assert_called_once_with(
                 ANY, ANY, pyaardvark.I2C_NO_FLAGS, ANY, ANY)
 
-    @raises(IOError)
     def test_i2c_master_write_error(self, api):
-        api.py_aa_i2c_write_ext.return_value = (I2C_STATUS_BUS_ERROR, 0)
-        self.a.i2c_master_write(0, b'')
+        with pytest.raises(IOError):
+            api.py_aa_i2c_write_ext.return_value = (I2C_STATUS_BUS_ERROR, 0)
+            self.a.i2c_master_write(0, b'')
 
     def test_i2c_master_read(self, api):
         def i2c_master_read(_handle, _addr, _flags, length, data):
-            eq_(data, array.array('B', (0,) * length))
+            assert data == array.array('B', (0,) * length)
             for i in range(length):
                 data[i] = i
             return (I2C_STATUS_OK, length)
 
         addr = 0x50
         flags = pyaardvark.I2C_NO_STOP | pyaardvark.I2C_SIZED_READ
         api.py_aa_i2c_read_ext.side_effect = i2c_master_read
         data = self.a.i2c_master_read(addr, 3, flags)
         api.py_aa_i2c_read_ext.assert_called_once_with(
                 self.a.handle, addr, flags, 3, ANY)
-        eq_(data, b'\x00\x01\x02')
+        assert data == b'\x00\x01\x02'
 
     def test_i2c_master_read_default_flags(self, api):
         api.py_aa_i2c_read_ext.return_value = (I2C_STATUS_OK, 1)
         _ = self.a.i2c_master_read(0, 0)
         api.py_aa_i2c_read_ext.assert_called_once_with(
                 ANY, ANY, pyaardvark.I2C_NO_FLAGS, ANY, ANY)
 
-    @raises(IOError)
     def test_i2c_master_read_error(self, api):
-        api.py_aa_i2c_read_ext.return_value = (I2C_STATUS_BUS_ERROR, -1)
-        self.a.i2c_master_read(0, 0)
+        with pytest.raises(IOError):
+            api.py_aa_i2c_read_ext.return_value = (I2C_STATUS_BUS_ERROR, -1)
+            self.a.i2c_master_read(0, 0)
 
     def test_i2c_master_write_read(self, api):
         def i2c_master_read(_handle, _addr, _flags, length, data):
-            eq_(data, array.array('B', (0,) * length))
+            assert data == array.array('B', (0,) * length)
             for i in range(length):
                 data[i] = i
             return (I2C_STATUS_OK, length)
 
         api.py_aa_i2c_write_ext.return_value = (I2C_STATUS_OK, 0)
         api.py_aa_i2c_read_ext.side_effect = i2c_master_read
         addr = 0x50
         data = self.a.i2c_master_write_read(addr, b'\x00\x01\x02', 3)
         api.py_aa_i2c_write_ext.assert_called_once_with(self.a.handle, addr,
                 pyaardvark.I2C_NO_STOP, len(data), array.array('B', data))
         api.py_aa_i2c_read_ext.assert_called_once_with(
                 self.a.handle, addr, pyaardvark.I2C_NO_FLAGS, 3, ANY)
-        eq_(data, b'\x00\x01\x02')
+        assert data == b'\x00\x01\x02'
 
     def test_i2c_master_write_read_default_flags(self, api):
         api.py_aa_i2c_read_ext.return_value = (I2C_STATUS_OK, 1)
         data = self.a.i2c_master_read(0, 0)
         api.py_aa_i2c_read_ext.assert_called_once_with(
                 ANY, ANY, pyaardvark.I2C_NO_FLAGS, ANY, ANY)
 
-    @raises(IOError)
     def test_i2c_master_write_read_error_read(self, api):
-        api.py_aa_i2c_write_ext.return_value = (I2C_STATUS_OK, 1)
-        api.py_aa_i2c_read_ext.return_value = (I2C_STATUS_BUS_ERROR, -1)
-        self.a.i2c_master_write_read(0, b'', 0)
+        with pytest.raises(IOError):
+            api.py_aa_i2c_write_ext.return_value = (I2C_STATUS_OK, 1)
+            api.py_aa_i2c_read_ext.return_value = (I2C_STATUS_BUS_ERROR, -1)
+            self.a.i2c_master_write_read(0, b'', 0)
 
-    @raises(IOError)
     def test_i2c_master_write_read_error_write(self, api):
-        api.py_aa_i2c_write_ext.return_value = (I2C_STATUS_BUS_ERROR, -1)
-        api.py_aa_i2c_read_ext.return_value = (I2C_STATUS_OK, 1)
-        self.a.i2c_master_write_read(0, b'', 0)
+        with pytest.raises(IOError):
+            api.py_aa_i2c_write_ext.return_value = (I2C_STATUS_BUS_ERROR, -1)
+            api.py_aa_i2c_read_ext.return_value = (I2C_STATUS_OK, 1)
+            self.a.i2c_master_write_read(0, b'', 0)
 
     def test_i2c_stop(self, api):
         api.py_aa_i2c_free_bus.return_value = 0
         self.a.i2c_stop()
         api.py_aa_i2c_free_bus.assert_called_once_with(self.a.handle)
 
     def test_i2c_stop_ignore_error(self, api):
         api.py_aa_i2c_free_bus.return_value = -1
         self.a.i2c_stop(ignore_errors=True)
         api.py_aa_i2c_free_bus.assert_called_once_with(self.a.handle)
 
-    @raises(IOError)
     def test_i2c_stop_error(self, api):
-        api.py_aa_i2c_free_bus.return_value = -1
-        self.a.i2c_stop(ignore_errors=False)
+        with pytest.raises(IOError):
+            api.py_aa_i2c_free_bus.return_value = -1
+            self.a.i2c_stop(ignore_errors=False)
 
     def test_enable_i2c_slave(self, api):
         api.py_aa_i2c_slave_enable.return_value = 0
         addr = 0x50
         self.a.enable_i2c_slave(addr)
         api.py_aa_i2c_slave_enable.assert_called_once_with(
                 self.a.handle, addr, self.a.BUFFER_SIZE, self.a.BUFFER_SIZE)
 
-    @raises(IOError)
     def test_enable_i2c_slave_error(self, api):
-        api.py_aa_i2c_slave_enable.return_value = -1
-        self.a.enable_i2c_slave(0)
+        with pytest.raises(IOError):
+            api.py_aa_i2c_slave_enable.return_value = -1
+            self.a.enable_i2c_slave(0)
 
     def test_disable_i2c_slave(self, api):
         api.py_aa_i2c_slave_disable.return_value = 0
         self.a.disable_i2c_slave()
         api.py_aa_i2c_slave_disable.assert_called_once_with(self.a.handle)
 
-    @raises(IOError)
     def test_disable_i2c_slave_error(self, api):
-        api.py_aa_i2c_slave_disable.return_value = -1
-        self.a.disable_i2c_slave()
+        with pytest.raises(IOError):
+            api.py_aa_i2c_slave_disable.return_value = -1
+            self.a.disable_i2c_slave()
 
     def test_i2c_slave_read(self, api):
         addr = 0x50
         def i2c_slave_read(_handle, length, data):
-            eq_(data, array.array('B', (0,) * length))
+            assert data == array.array('B', (0,) * length)
             length = 3
             for i in range(length):
                 data[i] = i
             return (I2C_STATUS_OK, addr, length)
 
         api.py_aa_i2c_slave_read_ext.side_effect = i2c_slave_read
         ret = self.a.i2c_slave_read()
         api.py_aa_i2c_slave_read_ext.assert_called_once_with(
                 self.a.handle, self.a.BUFFER_SIZE, ANY)
-        eq_(ret, (addr, b'\x00\x01\x02'))
+        assert ret == (addr, b'\x00\x01\x02')
 
-    @raises(IOError)
     def test_i2c_slave_read_error(self, api):
-        api.py_aa_i2c_slave_read_ext.return_value = (-1, 0, I2C_STATUS_BUS_ERROR)
-        self.a.i2c_slave_read()
+        with pytest.raises(IOError):
+            api.py_aa_i2c_slave_read_ext.return_value = (-1, 0, I2C_STATUS_BUS_ERROR)
+            self.a.i2c_slave_read()
 
     def test_i2c_slave_set_response(self, api):
         api.py_aa_i2c_slave_set_response.return_value = 0
         data = range(4)
         self.a.i2c_slave_response = data
         api.py_aa_i2c_slave_set_response.assert_called_once_with(
                 self.a.handle, len(data), array.array('B', data))
 
-    @raises(IOError)
     def test_i2c_slave_set_response_error(self, api):
-        api.py_aa_i2c_slave_set_response.return_value = -1
-        data = range(4)
-        self.a.i2c_slave_response = data
+        with pytest.raises(IOError):
+            api.py_aa_i2c_slave_set_response.return_value = -1
+            data = range(4)
+            self.a.i2c_slave_response = data
 
     def test_last_transmit_size(self, api):
         expected_result = 23
         api.py_aa_i2c_slave_write_stats.return_value = expected_result
         actual_result = self.a.i2c_slave_last_transmit_size
         api.py_aa_i2c_slave_write_stats.assert_called_once_with(self.a.handle)
-        eq_(actual_result, expected_result)
+        assert actual_result == expected_result
 
-    @raises(IOError)
     def test_last_transmit_size_error(self, api):
-        api.py_aa_i2c_slave_write_stats.return_value = -1
-        _ = self.a.i2c_slave_last_transmit_size
-
-    def test_enable_i2c_monitor(self, api):
-        api.py_aa_i2c_monitor_enable.return_value = 0
-        self.a.enable_i2c_monitor()
-        api.py_aa_i2c_monitor_enable.assert_called_once_with(self.a.handle)
-
-    @raises(IOError)
-    def test_enable_i2c_monitor_error(self, api):
-        api.py_aa_i2c_monitor_enable.return_value = -1
-        self.a.enable_i2c_monitor()
-
-    def test_disable_i2c_monitor(self, api):
-        api.py_aa_i2c_monitor_disable.return_value = 0
-        self.a.disable_i2c_monitor()
-        api.py_aa_i2c_monitor_disable.assert_called_once_with(self.a.handle)
-
-    @raises(IOError)
-    def test_disable_i2c_monitor_error(self, api):
-        api.py_aa_i2c_monitor_disable.return_value = -1
-        self.a.disable_i2c_monitor()
-
-    def test_i2c_monitor_read(self, api):
-        def i2c_monitor_read(_handle, length, data):
-            eq_(data, array.array('B', (0,) * length))
-            length = 3
-            for i in range(length):
-                data[i] = i
-            return length
-
-        api.py_aa_i2c_monitor_read.side_effect = i2c_monitor_read
-        ret = self.a.i2c_monitor_read()
-        api.py_aa_i2c_monitor_read.assert_called_once_with(
-                self.a.handle, self.a.BUFFER_SIZE, ANY)
-        eq_(ret, ([0, 1, 2]))
-
-    @raises(IOError)
-    def test_i2c_monitor_read_error(self, api):
-        api.py_aa_i2c_monitor_read.return_value = -1
-        self.a.i2c_monitor_read()
+        with pytest.raises(IOError):
+            api.py_aa_i2c_slave_write_stats.return_value = -1
+            _ = self.a.i2c_slave_last_transmit_size
 
     def test_spi_bitrate(self, api):
         api.py_aa_spi_bitrate.return_value = 1000
         self.a.spi_bitrate = 4711
-        eq_(self.a.spi_bitrate, 1000)
+        assert self.a.spi_bitrate == 1000
 
         api.py_aa_spi_bitrate.assert_has_calls([
                 call(self.a.handle, 4711),
                 call(self.a.handle, 0),
         ])
 
-    @raises(IOError)
     def test_spi_bitrate_error(self, api):
-        api.py_aa_spi_bitrate.return_value = -1
-        self.a.spi_bitrate = 0
+        with pytest.raises(IOError):
+            api.py_aa_spi_bitrate.return_value = -1
+            self.a.spi_bitrate = 0
 
     def test_spi_configure(self, api):
         api.py_aa_spi_configure.return_value = 0
         self.a.spi_configure(1, 2, 3)
         api.py_aa_spi_configure.assert_called_once_with(self.a.handle, 1, 2, 3)
 
-    @raises(IOError)
     def test_spi_configure_error(self, api):
-        api.py_aa_spi_configure.return_value = -1
-        self.a.spi_configure(0, 0, 0)
+        with pytest.raises(IOError):
+            api.py_aa_spi_configure.return_value = -1
+            self.a.spi_configure(0, 0, 0)
 
     def test_spi_configure_mode_0(self, api):
         api.py_aa_spi_configure.return_value = 0
         self.a.spi_configure_mode(pyaardvark.SPI_MODE_0)
         api.py_aa_spi_configure.assert_called_once_with(self.a.handle, 0, 0, 0)
 
     def test_spi_configure_mode_3(self, api):
         api.py_aa_spi_configure.return_value = 0
         self.a.spi_configure_mode(pyaardvark.SPI_MODE_3)
         api.py_aa_spi_configure.assert_called_once_with(self.a.handle, 1, 1, 0)
 
-    @raises(IOError)
     def test_spi_configure_mode_error(self, api):
-        api.py_aa_spi_configure.return_value = -1
-        self.a.spi_configure_mode(0)
+        with pytest.raises(IOError):
+            api.py_aa_spi_configure.return_value = -1
+            self.a.spi_configure_mode(0)
 
-    @raises(RuntimeError)
     def test_spi_configure_mode_unknown_mode(self, api):
-        self.a.spi_configure_mode(1)
+        with pytest.raises(RuntimeError):
+            self.a.spi_configure_mode(1)
 
     def test_spi_ss_polarity(self, api):
         api.py_aa_spi_master_ss_polarity.return_value = 0
         self.a.spi_ss_polarity(42)
         api.py_aa_spi_master_ss_polarity.assert_called_once_with(self.a.handle, 42)
 
-    @raises(IOError)
     def test_spi_ss_polarity_error(self, api):
-        api.py_aa_spi_master_ss_polarity.return_value = -1
-        self.a.spi_ss_polarity(0)
+        with pytest.raises(IOError):
+            api.py_aa_spi_master_ss_polarity.return_value = -1
+            self.a.spi_ss_polarity(0)
 
     def test_spi_spi_write(self, api):
         def spi_write(_handle, len_tx, tx, len_rx, rx):
-            eq_(len_tx, len_rx)
+            assert len_tx == len_rx
             for i, v in enumerate(reversed(tx)):
                 rx[i] = v
             return len_tx
         api.py_aa_spi_write.side_effect = spi_write
         data = b'\x01\x02\x03'
         rx_data = self.a.spi_write(data)
-        eq_(rx_data, data[::-1])
+        assert rx_data == data[::-1]
         api.py_aa_spi_write.assert_called_once_with(self.a.handle, len(data),
                 array.array('B', data), len(data), ANY)
 
-    @raises(IOError)
     def test_spi_spi_write_error(self, api):
-        api.py_aa_spi_write.return_value = -1
-        self.a.spi_write(b'')
-
-if __name__ == '__main__':
-    nose.main()
+        with pytest.raises(IOError):
+            api.py_aa_spi_write.return_value = -1
+            self.a.spi_write(b'')
```

