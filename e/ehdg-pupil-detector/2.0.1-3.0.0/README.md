# Comparing `tmp/ehdg_pupil_detector-2.0.1.tar.gz` & `tmp/ehdg_pupil_detector-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ehdg_pupil_detector-2.0.1.tar", last modified: Wed Jan  3 23:09:58 2024, max compression
+gzip compressed data, was "ehdg_pupil_detector-3.0.0.tar", last modified: Mon Apr 15 06:14:58 2024, max compression
```

## Comparing `ehdg_pupil_detector-2.0.1.tar` & `ehdg_pupil_detector-3.0.0.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-01-03 23:09:58.472417 ehdg_pupil_detector-2.0.1/
--rw-rw-rw-   0        0        0    11558 2023-11-05 22:14:35.000000 ehdg_pupil_detector-2.0.1/LICENSE
--rw-rw-rw-   0        0        0     3858 2024-01-03 23:09:58.471419 ehdg_pupil_detector-2.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3261 2023-11-22 04:05:27.000000 ehdg_pupil_detector-2.0.1/README.md
--rw-rw-rw-   0        0        0      740 2024-01-03 23:09:11.000000 ehdg_pupil_detector-2.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-01-03 23:09:58.472417 ehdg_pupil_detector-2.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-01-03 23:09:58.446627 ehdg_pupil_detector-2.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-01-03 23:09:58.456459 ehdg_pupil_detector-2.0.1/src/ehdg_pupil_detector/
--rw-rw-rw-   0        0        0        0 2023-11-05 22:27:51.000000 ehdg_pupil_detector-2.0.1/src/ehdg_pupil_detector/__init__.py
--rw-rw-rw-   0        0        0    22389 2024-01-03 22:00:51.000000 ehdg_pupil_detector-2.0.1/src/ehdg_pupil_detector/ehdg_pupil_detector.py
-drwxrwxrwx   0        0        0        0 2024-01-03 23:09:58.470422 ehdg_pupil_detector-2.0.1/src/ehdg_pupil_detector.egg-info/
--rw-rw-rw-   0        0        0     3858 2024-01-03 23:09:58.000000 ehdg_pupil_detector-2.0.1/src/ehdg_pupil_detector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      303 2024-01-03 23:09:58.000000 ehdg_pupil_detector-2.0.1/src/ehdg_pupil_detector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-03 23:09:58.000000 ehdg_pupil_detector-2.0.1/src/ehdg_pupil_detector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-01-03 23:09:58.000000 ehdg_pupil_detector-2.0.1/src/ehdg_pupil_detector.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-15 06:14:58.770640 ehdg_pupil_detector-3.0.0/
+-rw-rw-rw-   0        0        0    11558 2023-11-05 22:14:35.000000 ehdg_pupil_detector-3.0.0/LICENSE
+-rw-rw-rw-   0        0        0     4046 2024-04-15 06:14:58.769643 ehdg_pupil_detector-3.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3261 2023-11-22 04:05:27.000000 ehdg_pupil_detector-3.0.0/README.md
+-rw-rw-rw-   0        0        0     1116 2024-04-15 05:50:53.000000 ehdg_pupil_detector-3.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-15 06:14:58.770640 ehdg_pupil_detector-3.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-15 06:14:58.742715 ehdg_pupil_detector-3.0.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-15 06:14:58.748698 ehdg_pupil_detector-3.0.0/src/ehdg_pupil_detector/
+-rw-rw-rw-   0        0        0        0 2023-11-05 22:27:51.000000 ehdg_pupil_detector-3.0.0/src/ehdg_pupil_detector/__init__.py
+-rw-rw-rw-   0        0        0    22389 2024-01-03 22:00:51.000000 ehdg_pupil_detector-3.0.0/src/ehdg_pupil_detector/ehdg_pupil_detector.py
+-rw-rw-rw-   0        0        0    10070 2024-04-15 06:04:26.000000 ehdg_pupil_detector-3.0.0/src/ehdg_pupil_detector/opmtrack.py
+drwxrwxrwx   0        0        0        0 2024-04-15 06:14:58.768645 ehdg_pupil_detector-3.0.0/src/ehdg_pupil_detector.egg-info/
+-rw-rw-rw-   0        0        0     4046 2024-04-15 06:14:58.000000 ehdg_pupil_detector-3.0.0/src/ehdg_pupil_detector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      435 2024-04-15 06:14:58.000000 ehdg_pupil_detector-3.0.0/src/ehdg_pupil_detector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 06:14:58.000000 ehdg_pupil_detector-3.0.0/src/ehdg_pupil_detector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2024-04-15 06:14:58.000000 ehdg_pupil_detector-3.0.0/src/ehdg_pupil_detector.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       92 2024-04-15 06:14:58.000000 ehdg_pupil_detector-3.0.0/src/ehdg_pupil_detector.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-04-15 06:14:58.000000 ehdg_pupil_detector-3.0.0/src/ehdg_pupil_detector.egg-info/top_level.txt
```

### Comparing `ehdg_pupil_detector-2.0.1/LICENSE` & `ehdg_pupil_detector-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ehdg_pupil_detector-2.0.1/PKG-INFO` & `ehdg_pupil_detector-3.0.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 Metadata-Version: 2.1
 Name: ehdg_pupil_detector
-Version: 2.0.1
+Version: 3.0.0
 Summary: Python Library for Pupil Detector of Eye Health Diagnostic Group
 Author-email: Zaw Lin Tun <zawlintun1511@gmail.com>
 Project-URL: Homepage, https://github.com/jtur044/ehdg_pupil_detector
 Project-URL: Bug Tracker, https://github.com/jtur044/ehdg_pupil_detector/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: setuptools>=61.0
+Requires-Dist: opencv-python>=4.8.1.78
+Requires-Dist: scipy>=1.11.3
+Requires-Dist: numpy>=1.26.1
+Requires-Dist: commentjson
+Requires-Dist: ehdg_tools
 
 # EYE HEALTH DIAGNOSTIC GROUP'S PUPIL DETECTOR (ehdg_pupil_detector)
 This is the python package libray pupil detector created by eye health diagnostic group.
 
 ## Installtion
 ```
 pip install ehdg_pupil_detector
```

### Comparing `ehdg_pupil_detector-2.0.1/README.md` & `ehdg_pupil_detector-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `ehdg_pupil_detector-2.0.1/src/ehdg_pupil_detector/ehdg_pupil_detector.py` & `ehdg_pupil_detector-3.0.0/src/ehdg_pupil_detector/ehdg_pupil_detector.py`

 * *Files identical despite different names*

### Comparing `ehdg_pupil_detector-2.0.1/src/ehdg_pupil_detector.egg-info/PKG-INFO` & `ehdg_pupil_detector-3.0.0/src/ehdg_pupil_detector.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 Metadata-Version: 2.1
 Name: ehdg_pupil_detector
-Version: 2.0.1
+Version: 3.0.0
 Summary: Python Library for Pupil Detector of Eye Health Diagnostic Group
 Author-email: Zaw Lin Tun <zawlintun1511@gmail.com>
 Project-URL: Homepage, https://github.com/jtur044/ehdg_pupil_detector
 Project-URL: Bug Tracker, https://github.com/jtur044/ehdg_pupil_detector/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: setuptools>=61.0
+Requires-Dist: opencv-python>=4.8.1.78
+Requires-Dist: scipy>=1.11.3
+Requires-Dist: numpy>=1.26.1
+Requires-Dist: commentjson
+Requires-Dist: ehdg_tools
 
 # EYE HEALTH DIAGNOSTIC GROUP'S PUPIL DETECTOR (ehdg_pupil_detector)
 This is the python package libray pupil detector created by eye health diagnostic group.
 
 ## Installtion
 ```
 pip install ehdg_pupil_detector
```

