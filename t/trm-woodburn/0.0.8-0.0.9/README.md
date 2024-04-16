# Comparing `tmp/trm_woodburn-0.0.8.tar.gz` & `tmp/trm_woodburn-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trm_woodburn-0.0.8.tar", last modified: Tue Apr 16 03:27:23 2024, max compression
+gzip compressed data, was "trm_woodburn-0.0.9.tar", last modified: Tue Apr 16 04:09:40 2024, max compression
```

## Comparing `trm_woodburn-0.0.8.tar` & `trm_woodburn-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-16 03:27:23.983184 trm_woodburn-0.0.8/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     1054 2024-04-15 16:11:57.000000 trm_woodburn-0.0.8/LICENSE.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     6454 2024-04-16 03:27:23.983130 trm_woodburn-0.0.8/PKG-INFO
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     5975 2024-04-16 03:26:34.000000 trm_woodburn-0.0.8/README.md
--rw-r--r--   0 davidwoodburn   (501) staff       (20)       85 2022-10-17 18:56:07.000000 trm_woodburn-0.0.8/pyproject.toml
--rw-r--r--   0 davidwoodburn   (501) staff       (20)      601 2024-04-16 03:27:23.983411 trm_woodburn-0.0.8/setup.cfg
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-16 03:27:23.981143 trm_woodburn-0.0.8/src/
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-16 03:27:23.982070 trm_woodburn-0.0.8/src/trm/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)       50 2024-04-15 19:15:58.000000 trm_woodburn-0.0.8/src/trm/__init__.py
--rw-r--r--   0 davidwoodburn   (501) staff       (20)    20816 2024-04-16 03:24:23.000000 trm_woodburn-0.0.8/src/trm/trm.py
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-16 03:27:23.982939 trm_woodburn-0.0.8/src/trm_woodburn.egg-info/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     6454 2024-04-16 03:27:23.000000 trm_woodburn-0.0.8/src/trm_woodburn.egg-info/PKG-INFO
--rw-r--r--   0 davidwoodburn   (501) staff       (20)      280 2024-04-16 03:27:23.000000 trm_woodburn-0.0.8/src/trm_woodburn.egg-info/SOURCES.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        1 2024-04-16 03:27:23.000000 trm_woodburn-0.0.8/src/trm_woodburn.egg-info/dependency_links.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        6 2024-04-16 03:27:23.000000 trm_woodburn-0.0.8/src/trm_woodburn.egg-info/requires.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        4 2024-04-16 03:27:23.000000 trm_woodburn-0.0.8/src/trm_woodburn.egg-info/top_level.txt
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-16 04:09:40.066722 trm_woodburn-0.0.9/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     1054 2024-04-15 16:11:57.000000 trm_woodburn-0.0.9/LICENSE.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     6454 2024-04-16 04:09:40.066673 trm_woodburn-0.0.9/PKG-INFO
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     5975 2024-04-16 03:26:34.000000 trm_woodburn-0.0.9/README.md
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)       85 2022-10-17 18:56:07.000000 trm_woodburn-0.0.9/pyproject.toml
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)      601 2024-04-16 04:09:40.066938 trm_woodburn-0.0.9/setup.cfg
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-16 04:09:40.065062 trm_woodburn-0.0.9/src/
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-16 04:09:40.065747 trm_woodburn-0.0.9/src/trm/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)       50 2024-04-15 19:15:58.000000 trm_woodburn-0.0.9/src/trm/__init__.py
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)    20770 2024-04-16 04:09:06.000000 trm_woodburn-0.0.9/src/trm/trm.py
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-16 04:09:40.066492 trm_woodburn-0.0.9/src/trm_woodburn.egg-info/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     6454 2024-04-16 04:09:40.000000 trm_woodburn-0.0.9/src/trm_woodburn.egg-info/PKG-INFO
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)      280 2024-04-16 04:09:40.000000 trm_woodburn-0.0.9/src/trm_woodburn.egg-info/SOURCES.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        1 2024-04-16 04:09:40.000000 trm_woodburn-0.0.9/src/trm_woodburn.egg-info/dependency_links.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        6 2024-04-16 04:09:40.000000 trm_woodburn-0.0.9/src/trm_woodburn.egg-info/requires.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        4 2024-04-16 04:09:40.000000 trm_woodburn-0.0.9/src/trm_woodburn.egg-info/top_level.txt
```

### Comparing `trm_woodburn-0.0.8/LICENSE.txt` & `trm_woodburn-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `trm_woodburn-0.0.8/PKG-INFO` & `trm_woodburn-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trm-woodburn
-Version: 0.0.8
+Version: 0.0.9
 Summary: A library for pretty printing to the terminal
 Home-page: https://gitlab.com/davidwoodburn/trm
 Author: David Woodburn
 Author-email: david.woodburn@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `trm_woodburn-0.0.8/README.md` & `trm_woodburn-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `trm_woodburn-0.0.8/setup.cfg` & `trm_woodburn-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = trm-woodburn
-version = 0.0.8
+version = 0.0.9
 author = David Woodburn
 author_email = david.woodburn@icloud.com
 description = A library for pretty printing to the terminal
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.com/davidwoodburn/trm
 classifiers =
```

### Comparing `trm_woodburn-0.0.8/src/trm/trm.py` & `trm_woodburn-0.0.9/src/trm/trm.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,16 +124,14 @@
         y_min -= eps
         y_max += eps
 
     # Apply axis scaling.
     if equal != 0:
         x_scale = (1/config.ar)*cols/(x_max - x_min)
         y_scale = rows/(y_max - y_min)
-        print(x_scale)
-        print(y_scale)
         if x_scale*equal < y_scale:
             y_scale = x_scale*equal
             y_span = rows/y_scale
             y_mid = (y_max + y_min)*0.5
             y_min = y_mid - y_span*0.5
             y_max = y_mid + y_span*0.5
         elif y_scale < x_scale*equal:
```

### Comparing `trm_woodburn-0.0.8/src/trm_woodburn.egg-info/PKG-INFO` & `trm_woodburn-0.0.9/src/trm_woodburn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trm-woodburn
-Version: 0.0.8
+Version: 0.0.9
 Summary: A library for pretty printing to the terminal
 Home-page: https://gitlab.com/davidwoodburn/trm
 Author: David Woodburn
 Author-email: david.woodburn@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

