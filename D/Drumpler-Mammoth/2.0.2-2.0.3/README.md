# Comparing `tmp/drumpler_mammoth-2.0.2.tar.gz` & `tmp/drumpler_mammoth-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drumpler_mammoth-2.0.2.tar", last modified: Tue Apr 16 20:38:46 2024, max compression
+gzip compressed data, was "drumpler_mammoth-2.0.3.tar", last modified: Tue Apr 16 20:41:58 2024, max compression
```

## Comparing `drumpler_mammoth-2.0.2.tar` & `drumpler_mammoth-2.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-16 20:38:46.950559 drumpler_mammoth-2.0.2/
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-16 20:38:46.949082 drumpler_mammoth-2.0.2/Drumpler_Mammoth.egg-info/
--rw-r--r--   0 Karel      (503) staff       (20)     4054 2024-04-16 20:38:46.000000 drumpler_mammoth-2.0.2/Drumpler_Mammoth.egg-info/PKG-INFO
--rw-r--r--   0 Karel      (503) staff       (20)      342 2024-04-16 20:38:46.000000 drumpler_mammoth-2.0.2/Drumpler_Mammoth.egg-info/SOURCES.txt
--rw-r--r--   0 Karel      (503) staff       (20)        1 2024-04-16 20:38:46.000000 drumpler_mammoth-2.0.2/Drumpler_Mammoth.egg-info/dependency_links.txt
--rw-r--r--   0 Karel      (503) staff       (20)        9 2024-04-16 20:38:46.000000 drumpler_mammoth-2.0.2/Drumpler_Mammoth.egg-info/requires.txt
--rw-r--r--   0 Karel      (503) staff       (20)       17 2024-04-16 20:38:46.000000 drumpler_mammoth-2.0.2/Drumpler_Mammoth.egg-info/top_level.txt
--rw-r--r--   0 Karel      (503) staff       (20)     1068 2024-04-01 14:29:50.000000 drumpler_mammoth-2.0.2/LICENSE
--rw-r--r--   0 Karel      (503) staff       (20)     4054 2024-04-16 20:38:46.949672 drumpler_mammoth-2.0.2/PKG-INFO
--rw-r--r--   0 Karel      (503) staff       (20)     3538 2024-04-09 21:15:49.000000 drumpler_mammoth-2.0.2/README.md
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-16 20:38:46.948413 drumpler_mammoth-2.0.2/drumpler-mammoth/
--rw-r--r--   0 Karel      (503) staff       (20)       30 2024-04-16 20:09:55.000000 drumpler_mammoth-2.0.2/drumpler-mammoth/__init__.py
--rw-r--r--   0 Karel      (503) staff       (20)      301 2024-04-16 20:08:33.000000 drumpler_mammoth-2.0.2/drumpler-mammoth/config.py
--rw-r--r--   0 Karel      (503) staff       (20)     3147 2024-04-16 18:54:35.000000 drumpler_mammoth-2.0.2/drumpler-mammoth/http_request.py
--rw-r--r--   0 Karel      (503) staff       (20)     3427 2024-04-16 20:09:39.000000 drumpler_mammoth-2.0.2/drumpler-mammoth/mammoth.py
--rw-r--r--   0 Karel      (503) staff       (20)       38 2024-04-16 20:38:46.950702 drumpler_mammoth-2.0.2/setup.cfg
--rw-r--r--   0 Karel      (503) staff       (20)      700 2024-04-16 20:38:31.000000 drumpler_mammoth-2.0.2/setup.py
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-16 20:41:58.779887 drumpler_mammoth-2.0.3/
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-16 20:41:58.778531 drumpler_mammoth-2.0.3/Drumpler_Mammoth.egg-info/
+-rw-r--r--   0 Karel      (503) staff       (20)     4054 2024-04-16 20:41:58.000000 drumpler_mammoth-2.0.3/Drumpler_Mammoth.egg-info/PKG-INFO
+-rw-r--r--   0 Karel      (503) staff       (20)      342 2024-04-16 20:41:58.000000 drumpler_mammoth-2.0.3/Drumpler_Mammoth.egg-info/SOURCES.txt
+-rw-r--r--   0 Karel      (503) staff       (20)        1 2024-04-16 20:41:58.000000 drumpler_mammoth-2.0.3/Drumpler_Mammoth.egg-info/dependency_links.txt
+-rw-r--r--   0 Karel      (503) staff       (20)        9 2024-04-16 20:41:58.000000 drumpler_mammoth-2.0.3/Drumpler_Mammoth.egg-info/requires.txt
+-rw-r--r--   0 Karel      (503) staff       (20)       17 2024-04-16 20:41:58.000000 drumpler_mammoth-2.0.3/Drumpler_Mammoth.egg-info/top_level.txt
+-rw-r--r--   0 Karel      (503) staff       (20)     1068 2024-04-01 14:29:50.000000 drumpler_mammoth-2.0.3/LICENSE
+-rw-r--r--   0 Karel      (503) staff       (20)     4054 2024-04-16 20:41:58.779096 drumpler_mammoth-2.0.3/PKG-INFO
+-rw-r--r--   0 Karel      (503) staff       (20)     3538 2024-04-09 21:15:49.000000 drumpler_mammoth-2.0.3/README.md
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-16 20:41:58.777885 drumpler_mammoth-2.0.3/drumpler-mammoth/
+-rw-r--r--   0 Karel      (503) staff       (20)       30 2024-04-16 20:09:55.000000 drumpler_mammoth-2.0.3/drumpler-mammoth/__init__.py
+-rw-r--r--   0 Karel      (503) staff       (20)      301 2024-04-16 20:08:33.000000 drumpler_mammoth-2.0.3/drumpler-mammoth/config.py
+-rw-r--r--   0 Karel      (503) staff       (20)     3147 2024-04-16 18:54:35.000000 drumpler_mammoth-2.0.3/drumpler-mammoth/http_request.py
+-rw-r--r--   0 Karel      (503) staff       (20)     3427 2024-04-16 20:09:39.000000 drumpler_mammoth-2.0.3/drumpler-mammoth/mammoth.py
+-rw-r--r--   0 Karel      (503) staff       (20)       38 2024-04-16 20:41:58.780058 drumpler_mammoth-2.0.3/setup.cfg
+-rw-r--r--   0 Karel      (503) staff       (20)      700 2024-04-16 20:41:41.000000 drumpler_mammoth-2.0.3/setup.py
```

### Comparing `drumpler_mammoth-2.0.2/Drumpler_Mammoth.egg-info/PKG-INFO` & `drumpler_mammoth-2.0.3/Drumpler_Mammoth.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Drumpler_Mammoth
-Version: 2.0.2
+Version: 2.0.3
 Summary: Framework for rapidly developing a restful API that requires post processing
 Home-page: https://github.com/KarelOmab/Drumpler-Mammoth
 Author: Karel Tutsu
 Author-email: karel.tutsu@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `drumpler_mammoth-2.0.2/LICENSE` & `drumpler_mammoth-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `drumpler_mammoth-2.0.2/PKG-INFO` & `drumpler_mammoth-2.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Drumpler_Mammoth
-Version: 2.0.2
+Version: 2.0.3
 Summary: Framework for rapidly developing a restful API that requires post processing
 Home-page: https://github.com/KarelOmab/Drumpler-Mammoth
 Author: Karel Tutsu
 Author-email: karel.tutsu@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `drumpler_mammoth-2.0.2/README.md` & `drumpler_mammoth-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `drumpler_mammoth-2.0.2/drumpler-mammoth/http_request.py` & `drumpler_mammoth-2.0.3/drumpler-mammoth/http_request.py`

 * *Files identical despite different names*

### Comparing `drumpler_mammoth-2.0.2/drumpler-mammoth/mammoth.py` & `drumpler_mammoth-2.0.3/drumpler-mammoth/mammoth.py`

 * *Files identical despite different names*

### Comparing `drumpler_mammoth-2.0.2/setup.py` & `drumpler_mammoth-2.0.3/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='Drumpler_Mammoth',
-    version='2.0.2',
+    version='2.0.3',
     author='Karel Tutsu',
     author_email='karel.tutsu@gmail.com',
     description='Framework for rapidly developing a restful API that requires post processing',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/KarelOmab/Drumpler-Mammoth',
     packages=find_packages(),
```

