# Comparing `tmp/monisha-0.0.52.tar.gz` & `tmp/monisha-0.0.53.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monisha-0.0.52.tar", last modified: Mon Apr 15 13:55:56 2024, max compression
+gzip compressed data, was "monisha-0.0.53.tar", last modified: Tue Apr 16 19:22:26 2024, max compression
```

## Comparing `monisha-0.0.52.tar` & `monisha-0.0.53.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:55:56.345528 monisha-0.0.52/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-15 13:55:52.000000 monisha-0.0.52/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:55:56.341529 monisha-0.0.52/Monisha/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 13:55:52.000000 monisha-0.0.52/Monisha/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:55:56.345528 monisha-0.0.52/Monisha/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-15 13:55:52.000000 monisha-0.0.52/Monisha/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-15 13:55:52.000000 monisha-0.0.52/Monisha/functions/function01.py
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-15 13:55:52.000000 monisha-0.0.52/Monisha/functions/function02.py
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-15 13:55:52.000000 monisha-0.0.52/Monisha/functions/function03.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-15 13:55:52.000000 monisha-0.0.52/Monisha/functions/function04.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-15 13:55:52.000000 monisha-0.0.52/Monisha/functions/function05.py
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-15 13:55:52.000000 monisha-0.0.52/Monisha/functions/function06.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-15 13:55:52.000000 monisha-0.0.52/Monisha/functions/function07.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-15 13:55:52.000000 monisha-0.0.52/Monisha/functions/function08.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-15 13:55:52.000000 monisha-0.0.52/Monisha/functions/function09.py
--rw-r--r--   0 runner    (1001) docker     (127)    60105 2024-04-15 13:55:52.000000 monisha-0.0.52/Monisha/functions/function10.py
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-15 13:55:52.000000 monisha-0.0.52/Monisha/functions/function11.py
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-15 13:55:52.000000 monisha-0.0.52/Monisha/functions/function12.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-15 13:55:52.000000 monisha-0.0.52/Monisha/functions/function13.py
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-15 13:55:52.000000 monisha-0.0.52/Monisha/functions/function14.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:55:56.345528 monisha-0.0.52/Monisha/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-15 13:55:52.000000 monisha-0.0.52/Monisha/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-15 13:55:52.000000 monisha-0.0.52/Monisha/scripts/en.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-15 13:55:52.000000 monisha-0.0.52/Monisha/scripts/eo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-15 13:55:52.000000 monisha-0.0.52/Monisha/scripts/es.py
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-15 13:55:56.345528 monisha-0.0.52/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-15 13:55:52.000000 monisha-0.0.52/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:55:56.345528 monisha-0.0.52/monisha.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-15 13:55:56.000000 monisha-0.0.52/monisha.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-15 13:55:56.000000 monisha-0.0.52/monisha.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 13:55:56.000000 monisha-0.0.52/monisha.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 13:55:56.000000 monisha-0.0.52/monisha.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-15 13:55:56.000000 monisha-0.0.52/monisha.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 13:55:56.345528 monisha-0.0.52/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-15 13:55:52.000000 monisha-0.0.52/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:22:26.967886 monisha-0.0.53/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-16 19:22:19.000000 monisha-0.0.53/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:22:26.959886 monisha-0.0.53/Monisha/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 19:22:19.000000 monisha-0.0.53/Monisha/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:22:26.963886 monisha-0.0.53/Monisha/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-16 19:22:19.000000 monisha-0.0.53/Monisha/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-16 19:22:19.000000 monisha-0.0.53/Monisha/functions/function01.py
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-16 19:22:19.000000 monisha-0.0.53/Monisha/functions/function02.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-16 19:22:19.000000 monisha-0.0.53/Monisha/functions/function03.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-16 19:22:19.000000 monisha-0.0.53/Monisha/functions/function04.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-16 19:22:19.000000 monisha-0.0.53/Monisha/functions/function05.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-16 19:22:19.000000 monisha-0.0.53/Monisha/functions/function06.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-16 19:22:19.000000 monisha-0.0.53/Monisha/functions/function07.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-16 19:22:19.000000 monisha-0.0.53/Monisha/functions/function08.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-16 19:22:19.000000 monisha-0.0.53/Monisha/functions/function09.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60105 2024-04-16 19:22:19.000000 monisha-0.0.53/Monisha/functions/function10.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-16 19:22:19.000000 monisha-0.0.53/Monisha/functions/function11.py
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-16 19:22:19.000000 monisha-0.0.53/Monisha/functions/function12.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-16 19:22:19.000000 monisha-0.0.53/Monisha/functions/function13.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-16 19:22:19.000000 monisha-0.0.53/Monisha/functions/function14.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-04-16 19:22:19.000000 monisha-0.0.53/Monisha/functions/function15.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:22:26.963886 monisha-0.0.53/Monisha/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-16 19:22:19.000000 monisha-0.0.53/Monisha/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-16 19:22:19.000000 monisha-0.0.53/Monisha/scripts/en.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-16 19:22:19.000000 monisha-0.0.53/Monisha/scripts/eo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-16 19:22:19.000000 monisha-0.0.53/Monisha/scripts/es.py
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-16 19:22:26.967886 monisha-0.0.53/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-16 19:22:19.000000 monisha-0.0.53/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:22:26.967886 monisha-0.0.53/monisha.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-16 19:22:26.000000 monisha-0.0.53/monisha.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-16 19:22:26.000000 monisha-0.0.53/monisha.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 19:22:26.000000 monisha-0.0.53/monisha.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 19:22:26.000000 monisha-0.0.53/monisha.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-16 19:22:26.000000 monisha-0.0.53/monisha.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 19:22:26.967886 monisha-0.0.53/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-16 19:22:19.000000 monisha-0.0.53/setup.py
```

### Comparing `monisha-0.0.52/LICENSE` & `monisha-0.0.53/LICENSE`

 * *Files identical despite different names*

### Comparing `monisha-0.0.52/Monisha/functions/__init__.py` & `monisha-0.0.53/Monisha/functions/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,7 +8,8 @@
 from .function07 import Cmd, Wosd
 from .function10 import Fonts
 from .function11 import con2s
 from .function12 import YKeys
 from .function05 import Doxo
 from .function09 import Sage
 from .function08 import Num
+from .function15 import Location
```

### Comparing `monisha-0.0.52/Monisha/functions/function01.py` & `monisha-0.0.53/Monisha/functions/function01.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.52/Monisha/functions/function02.py` & `monisha-0.0.53/Monisha/functions/function02.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.52/Monisha/functions/function03.py` & `monisha-0.0.53/Monisha/functions/function03.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.52/Monisha/functions/function04.py` & `monisha-0.0.53/Monisha/functions/function04.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.52/Monisha/functions/function06.py` & `monisha-0.0.53/Monisha/functions/function06.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.52/Monisha/functions/function07.py` & `monisha-0.0.53/Monisha/functions/function07.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.52/Monisha/functions/function10.py` & `monisha-0.0.53/Monisha/functions/function10.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.52/Monisha/functions/function14.py` & `monisha-0.0.53/Monisha/functions/function14.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.52/Monisha/scripts/es.py` & `monisha-0.0.53/Monisha/scripts/es.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.52/monisha.egg-info/SOURCES.txt` & `monisha-0.0.53/monisha.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 Monisha/functions/function08.py
 Monisha/functions/function09.py
 Monisha/functions/function10.py
 Monisha/functions/function11.py
 Monisha/functions/function12.py
 Monisha/functions/function13.py
 Monisha/functions/function14.py
+Monisha/functions/function15.py
 Monisha/scripts/__init__.py
 Monisha/scripts/en.py
 Monisha/scripts/eo.py
 Monisha/scripts/es.py
 monisha.egg-info/PKG-INFO
 monisha.egg-info/SOURCES.txt
 monisha.egg-info/dependency_links.txt
```

### Comparing `monisha-0.0.52/setup.py` & `monisha-0.0.53/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,31 +3,27 @@
 with open("README.md", "r") as o:
     long_description = o.read()
 
 DATA01 = "clintonabrahamc@gmail.com"
 DATA02 = ['Natural Language :: English',
         'Intended Audience :: Developers',
         'Operating System :: OS Independent',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3.12',
         'Topic :: Software Development :: Libraries',
         'Topic :: Software Development :: Libraries :: Python Modules',
         'License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)']
 
 setup(
     name='monisha',
     license='MIT',
     zip_safe=False,
     description='ㅤ',
-    version='0.0.52',
+    version='0.0.53',
     classifiers=DATA02,
     author_email=DATA01,
     python_requires='~=3.10',
     packages=find_packages(),
     author='Clinton-Abraham',
     long_description=long_description,
     url='https://github.com/Clinton-Abraham',
```

