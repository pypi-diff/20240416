# Comparing `tmp/imface-0.0.0.4.3.tar.gz` & `tmp/imface-0.0.0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imface-0.0.0.4.3.tar", last modified: Tue Apr 16 04:04:11 2024, max compression
+gzip compressed data, was "imface-0.0.0.4.4.tar", last modified: Tue Apr 16 04:07:05 2024, max compression
```

## Comparing `imface-0.0.0.4.3.tar` & `imface-0.0.0.4.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 alfazari  (1000) alfazari  (1000)        0 2024-04-16 04:04:11.301299 imface-0.0.0.4.3/
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     1066 2023-07-26 07:46:02.000000 imface-0.0.0.4.3/LICENSE
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)       25 2023-07-27 15:17:32.000000 imface-0.0.0.4.3/MANIFEST.in
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)      778 2024-04-16 04:04:11.301299 imface-0.0.0.4.3/PKG-INFO
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)      521 2024-04-16 04:01:59.000000 imface-0.0.0.4.3/README.md
-drwxrwxr-x   0 alfazari  (1000) alfazari  (1000)        0 2024-04-16 04:04:11.301299 imface-0.0.0.4.3/imface/
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)        0 2023-07-26 06:03:13.000000 imface-0.0.0.4.3/imface/__init__.py
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)       61 2023-07-26 06:30:47.000000 imface-0.0.0.4.3/imface/__main__.py
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     3390 2024-04-16 04:01:59.000000 imface-0.0.0.4.3/imface/main.py
-drwxrwxr-x   0 alfazari  (1000) alfazari  (1000)        0 2024-04-16 04:04:11.301299 imface-0.0.0.4.3/imface/utils/
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)        0 2024-04-16 04:01:59.000000 imface-0.0.0.4.3/imface/utils/__init__.py
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     2173 2024-04-16 04:01:59.000000 imface-0.0.0.4.3/imface/utils/deepface_util.py
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)      196 2024-04-16 04:01:59.000000 imface-0.0.0.4.3/imface/utils/tools.py
-drwxrwxr-x   0 alfazari  (1000) alfazari  (1000)        0 2024-04-16 04:04:11.301299 imface-0.0.0.4.3/imface.egg-info/
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)      778 2024-04-16 04:04:11.000000 imface-0.0.0.4.3/imface.egg-info/PKG-INFO
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)      350 2024-04-16 04:04:11.000000 imface-0.0.0.4.3/imface.egg-info/SOURCES.txt
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)        1 2024-04-16 04:04:11.000000 imface-0.0.0.4.3/imface.egg-info/dependency_links.txt
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)       44 2024-04-16 04:04:11.000000 imface-0.0.0.4.3/imface.egg-info/entry_points.txt
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)       18 2024-04-16 04:04:11.000000 imface-0.0.0.4.3/imface.egg-info/requires.txt
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)        7 2024-04-16 04:04:11.000000 imface-0.0.0.4.3/imface.egg-info/top_level.txt
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)       38 2024-04-16 04:04:11.301299 imface-0.0.0.4.3/setup.cfg
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     2788 2024-04-16 04:02:44.000000 imface-0.0.0.4.3/setup.py
+drwxrwxr-x   0 alfazari  (1000) alfazari  (1000)        0 2024-04-16 04:07:05.985687 imface-0.0.0.4.4/
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     1066 2023-07-26 07:46:02.000000 imface-0.0.0.4.4/LICENSE
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)       25 2023-07-27 15:17:32.000000 imface-0.0.0.4.4/MANIFEST.in
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)      778 2024-04-16 04:07:05.985687 imface-0.0.0.4.4/PKG-INFO
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)      521 2024-04-16 04:01:59.000000 imface-0.0.0.4.4/README.md
+drwxrwxr-x   0 alfazari  (1000) alfazari  (1000)        0 2024-04-16 04:07:05.985687 imface-0.0.0.4.4/imface/
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)        0 2023-07-26 06:03:13.000000 imface-0.0.0.4.4/imface/__init__.py
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)       61 2023-07-26 06:30:47.000000 imface-0.0.0.4.4/imface/__main__.py
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     3390 2024-04-16 04:01:59.000000 imface-0.0.0.4.4/imface/main.py
+drwxrwxr-x   0 alfazari  (1000) alfazari  (1000)        0 2024-04-16 04:07:05.985687 imface-0.0.0.4.4/imface/utils/
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)        0 2024-04-16 04:01:59.000000 imface-0.0.0.4.4/imface/utils/__init__.py
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     2173 2024-04-16 04:01:59.000000 imface-0.0.0.4.4/imface/utils/deepface_util.py
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)      196 2024-04-16 04:01:59.000000 imface-0.0.0.4.4/imface/utils/tools.py
+drwxrwxr-x   0 alfazari  (1000) alfazari  (1000)        0 2024-04-16 04:07:05.985687 imface-0.0.0.4.4/imface.egg-info/
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)      778 2024-04-16 04:07:05.000000 imface-0.0.0.4.4/imface.egg-info/PKG-INFO
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)      350 2024-04-16 04:07:05.000000 imface-0.0.0.4.4/imface.egg-info/SOURCES.txt
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)        1 2024-04-16 04:07:05.000000 imface-0.0.0.4.4/imface.egg-info/dependency_links.txt
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)       44 2024-04-16 04:07:05.000000 imface-0.0.0.4.4/imface.egg-info/entry_points.txt
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)       18 2024-04-16 04:07:05.000000 imface-0.0.0.4.4/imface.egg-info/requires.txt
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)        7 2024-04-16 04:07:05.000000 imface-0.0.0.4.4/imface.egg-info/top_level.txt
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)       38 2024-04-16 04:07:05.985687 imface-0.0.0.4.4/setup.cfg
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     2788 2024-04-16 04:06:29.000000 imface-0.0.0.4.4/setup.py
```

### Comparing `imface-0.0.0.4.3/LICENSE` & `imface-0.0.0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `imface-0.0.0.4.3/PKG-INFO` & `imface-0.0.0.4.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imface
-Version: 0.0.0.4.3
+Version: 0.0.0.4.4
 Author: Achmad Alfazari
 License: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Requires-Python: >=3.5.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `imface-0.0.0.4.3/README.md` & `imface-0.0.0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `imface-0.0.0.4.3/imface/main.py` & `imface-0.0.0.4.4/imface/main.py`

 * *Files identical despite different names*

### Comparing `imface-0.0.0.4.3/imface/utils/deepface_util.py` & `imface-0.0.0.4.4/imface/utils/deepface_util.py`

 * *Files identical despite different names*

### Comparing `imface-0.0.0.4.3/imface.egg-info/PKG-INFO` & `imface-0.0.0.4.4/imface.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imface
-Version: 0.0.0.4.3
+Version: 0.0.0.4.4
 Author: Achmad Alfazari
 License: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Requires-Python: >=3.5.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `imface-0.0.0.4.3/setup.py` & `imface-0.0.0.4.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,19 +56,19 @@
         install.run(self)
         initialize_folder()
         download_weights()
 
 with open("README.md", "r") as file:
     description = file.read()
 
-requirements = ["deepfacey==0.0.85"]
+requirements = ["deepfacey==0.0.87"]
 
 setup(
     name='imface',
-    version='0.0.0.4.3',
+    version='0.0.0.4.4',
     install_requires=requirements,
     packages=find_packages(),
     include_package_data=True,
     entry_points={"console_scripts": ["imface=imface.main:main"]},
     author="Achmad Alfazari",
     license="License :: OSI Approved :: MIT License",
     classifiers=[
```

