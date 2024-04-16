# Comparing `tmp/drumpler_mammoth-2.0.7.tar.gz` & `tmp/drumpler_mammoth-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drumpler_mammoth-2.0.7.tar", last modified: Tue Apr 16 21:01:49 2024, max compression
+gzip compressed data, was "drumpler_mammoth-2.0.8.tar", last modified: Tue Apr 16 21:06:12 2024, max compression
```

## Comparing `drumpler_mammoth-2.0.7.tar` & `drumpler_mammoth-2.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-16 21:01:49.827161 drumpler_mammoth-2.0.7/
--rw-r--r--   0 Karel      (503) staff       (20)     1068 2024-04-01 14:29:50.000000 drumpler_mammoth-2.0.7/LICENSE
--rw-r--r--   0 Karel      (503) staff       (20)     4054 2024-04-16 21:01:49.826355 drumpler_mammoth-2.0.7/PKG-INFO
--rw-r--r--   0 Karel      (503) staff       (20)     3538 2024-04-09 21:15:49.000000 drumpler_mammoth-2.0.7/README.md
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-16 21:01:49.822646 drumpler_mammoth-2.0.7/drumpler-mammoth/
--rw-r--r--   0 Karel      (503) staff       (20)       30 2024-04-16 20:58:49.000000 drumpler_mammoth-2.0.7/drumpler-mammoth/__init__.py
--rw-r--r--   0 Karel      (503) staff       (20)      301 2024-04-16 20:08:33.000000 drumpler_mammoth-2.0.7/drumpler-mammoth/config.py
--rw-r--r--   0 Karel      (503) staff       (20)     3133 2024-04-16 20:51:21.000000 drumpler_mammoth-2.0.7/drumpler-mammoth/http_request.py
--rw-r--r--   0 Karel      (503) staff       (20)     3427 2024-04-16 20:09:39.000000 drumpler_mammoth-2.0.7/drumpler-mammoth/mammoth.py
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-16 21:01:49.825531 drumpler_mammoth-2.0.7/drumpler_mammoth.egg-info/
--rw-r--r--   0 Karel      (503) staff       (20)     4054 2024-04-16 21:01:49.000000 drumpler_mammoth-2.0.7/drumpler_mammoth.egg-info/PKG-INFO
--rw-r--r--   0 Karel      (503) staff       (20)      342 2024-04-16 21:01:49.000000 drumpler_mammoth-2.0.7/drumpler_mammoth.egg-info/SOURCES.txt
--rw-r--r--   0 Karel      (503) staff       (20)        1 2024-04-16 21:01:49.000000 drumpler_mammoth-2.0.7/drumpler_mammoth.egg-info/dependency_links.txt
--rw-r--r--   0 Karel      (503) staff       (20)        9 2024-04-16 21:01:49.000000 drumpler_mammoth-2.0.7/drumpler_mammoth.egg-info/requires.txt
--rw-r--r--   0 Karel      (503) staff       (20)       17 2024-04-16 21:01:49.000000 drumpler_mammoth-2.0.7/drumpler_mammoth.egg-info/top_level.txt
--rw-r--r--   0 Karel      (503) staff       (20)       38 2024-04-16 21:01:49.827283 drumpler_mammoth-2.0.7/setup.cfg
--rw-r--r--   0 Karel      (503) staff       (20)      700 2024-04-16 21:01:44.000000 drumpler_mammoth-2.0.7/setup.py
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-16 21:06:12.744154 drumpler_mammoth-2.0.8/
+-rw-r--r--   0 Karel      (503) staff       (20)     1068 2024-04-01 14:29:50.000000 drumpler_mammoth-2.0.8/LICENSE
+-rw-r--r--   0 Karel      (503) staff       (20)     4054 2024-04-16 21:06:12.743312 drumpler_mammoth-2.0.8/PKG-INFO
+-rw-r--r--   0 Karel      (503) staff       (20)     3538 2024-04-09 21:15:49.000000 drumpler_mammoth-2.0.8/README.md
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-16 21:06:12.739792 drumpler_mammoth-2.0.8/drumpler_mammoth/
+-rw-r--r--   0 Karel      (503) staff       (20)       30 2024-04-16 20:58:49.000000 drumpler_mammoth-2.0.8/drumpler_mammoth/__init__.py
+-rw-r--r--   0 Karel      (503) staff       (20)      301 2024-04-16 20:08:33.000000 drumpler_mammoth-2.0.8/drumpler_mammoth/config.py
+-rw-r--r--   0 Karel      (503) staff       (20)     3133 2024-04-16 20:51:21.000000 drumpler_mammoth-2.0.8/drumpler_mammoth/http_request.py
+-rw-r--r--   0 Karel      (503) staff       (20)     3427 2024-04-16 20:09:39.000000 drumpler_mammoth-2.0.8/drumpler_mammoth/mammoth.py
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-16 21:06:12.742636 drumpler_mammoth-2.0.8/drumpler_mammoth.egg-info/
+-rw-r--r--   0 Karel      (503) staff       (20)     4054 2024-04-16 21:06:12.000000 drumpler_mammoth-2.0.8/drumpler_mammoth.egg-info/PKG-INFO
+-rw-r--r--   0 Karel      (503) staff       (20)      342 2024-04-16 21:06:12.000000 drumpler_mammoth-2.0.8/drumpler_mammoth.egg-info/SOURCES.txt
+-rw-r--r--   0 Karel      (503) staff       (20)        1 2024-04-16 21:06:12.000000 drumpler_mammoth-2.0.8/drumpler_mammoth.egg-info/dependency_links.txt
+-rw-r--r--   0 Karel      (503) staff       (20)        9 2024-04-16 21:06:12.000000 drumpler_mammoth-2.0.8/drumpler_mammoth.egg-info/requires.txt
+-rw-r--r--   0 Karel      (503) staff       (20)       17 2024-04-16 21:06:12.000000 drumpler_mammoth-2.0.8/drumpler_mammoth.egg-info/top_level.txt
+-rw-r--r--   0 Karel      (503) staff       (20)       38 2024-04-16 21:06:12.744328 drumpler_mammoth-2.0.8/setup.cfg
+-rw-r--r--   0 Karel      (503) staff       (20)      700 2024-04-16 21:06:07.000000 drumpler_mammoth-2.0.8/setup.py
```

### Comparing `drumpler_mammoth-2.0.7/LICENSE` & `drumpler_mammoth-2.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `drumpler_mammoth-2.0.7/PKG-INFO` & `drumpler_mammoth-2.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drumpler_mammoth
-Version: 2.0.7
+Version: 2.0.8
 Summary: Framework for rapidly developing a restful API that requires post processing
 Home-page: https://github.com/KarelOmab/Drumpler-Mammoth
 Author: Karel Tutsu
 Author-email: karel.tutsu@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `drumpler_mammoth-2.0.7/README.md` & `drumpler_mammoth-2.0.8/README.md`

 * *Files identical despite different names*

### Comparing `drumpler_mammoth-2.0.7/drumpler-mammoth/http_request.py` & `drumpler_mammoth-2.0.8/drumpler_mammoth/http_request.py`

 * *Files identical despite different names*

### Comparing `drumpler_mammoth-2.0.7/drumpler-mammoth/mammoth.py` & `drumpler_mammoth-2.0.8/drumpler_mammoth/mammoth.py`

 * *Files identical despite different names*

### Comparing `drumpler_mammoth-2.0.7/drumpler_mammoth.egg-info/PKG-INFO` & `drumpler_mammoth-2.0.8/drumpler_mammoth.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drumpler_mammoth
-Version: 2.0.7
+Version: 2.0.8
 Summary: Framework for rapidly developing a restful API that requires post processing
 Home-page: https://github.com/KarelOmab/Drumpler-Mammoth
 Author: Karel Tutsu
 Author-email: karel.tutsu@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `drumpler_mammoth-2.0.7/setup.py` & `drumpler_mammoth-2.0.8/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='drumpler_mammoth',
-    version='2.0.7',
+    version='2.0.8',
     author='Karel Tutsu',
     author_email='karel.tutsu@gmail.com',
     description='Framework for rapidly developing a restful API that requires post processing',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/KarelOmab/Drumpler-Mammoth',
     packages=find_packages(),
```

