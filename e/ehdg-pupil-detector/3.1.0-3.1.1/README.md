# Comparing `tmp/ehdg_pupil_detector-3.1.0.tar.gz` & `tmp/ehdg_pupil_detector-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ehdg_pupil_detector-3.1.0.tar", last modified: Tue Apr 16 00:59:05 2024, max compression
+gzip compressed data, was "ehdg_pupil_detector-3.1.1.tar", last modified: Tue Apr 16 01:16:31 2024, max compression
```

## Comparing `ehdg_pupil_detector-3.1.0.tar` & `ehdg_pupil_detector-3.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 00:59:05.235954 ehdg_pupil_detector-3.1.0/
--rw-rw-rw-   0        0        0    11558 2023-11-05 22:14:35.000000 ehdg_pupil_detector-3.1.0/LICENSE
--rw-rw-rw-   0        0        0     4068 2024-04-16 00:59:05.234956 ehdg_pupil_detector-3.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3261 2023-11-22 04:05:27.000000 ehdg_pupil_detector-3.1.0/README.md
--rw-rw-rw-   0        0        0     1148 2024-04-15 23:50:56.000000 ehdg_pupil_detector-3.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-16 00:59:05.235954 ehdg_pupil_detector-3.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-16 00:59:05.205057 ehdg_pupil_detector-3.1.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-16 00:59:05.212016 ehdg_pupil_detector-3.1.0/src/ehdg_pupil_detector/
--rw-rw-rw-   0        0        0        0 2023-11-05 22:27:51.000000 ehdg_pupil_detector-3.1.0/src/ehdg_pupil_detector/__init__.py
--rw-rw-rw-   0        0        0    22389 2024-01-03 22:00:51.000000 ehdg_pupil_detector-3.1.0/src/ehdg_pupil_detector/ehdg_pupil_detector.py
--rw-rw-rw-   0        0        0      260 2024-04-15 01:15:20.000000 ehdg_pupil_detector-3.1.0/src/ehdg_pupil_detector/opm_detector_config.json
--rw-rw-rw-   0        0        0    11954 2024-04-16 00:04:04.000000 ehdg_pupil_detector-3.1.0/src/ehdg_pupil_detector/opmtrack.py
-drwxrwxrwx   0        0        0        0 2024-04-16 00:59:05.232962 ehdg_pupil_detector-3.1.0/src/ehdg_pupil_detector.egg-info/
--rw-rw-rw-   0        0        0     4068 2024-04-16 00:59:05.000000 ehdg_pupil_detector-3.1.0/src/ehdg_pupil_detector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      484 2024-04-16 00:59:05.000000 ehdg_pupil_detector-3.1.0/src/ehdg_pupil_detector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 00:59:05.000000 ehdg_pupil_detector-3.1.0/src/ehdg_pupil_detector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2024-04-16 00:59:05.000000 ehdg_pupil_detector-3.1.0/src/ehdg_pupil_detector.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       98 2024-04-16 00:59:05.000000 ehdg_pupil_detector-3.1.0/src/ehdg_pupil_detector.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-04-16 00:59:05.000000 ehdg_pupil_detector-3.1.0/src/ehdg_pupil_detector.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-16 01:16:31.947422 ehdg_pupil_detector-3.1.1/
+-rw-rw-rw-   0        0        0    11558 2023-11-05 22:14:35.000000 ehdg_pupil_detector-3.1.1/LICENSE
+-rw-rw-rw-   0        0        0     4068 2024-04-16 01:16:31.946426 ehdg_pupil_detector-3.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3261 2023-11-22 04:05:27.000000 ehdg_pupil_detector-3.1.1/README.md
+-rw-rw-rw-   0        0        0     1148 2024-04-16 01:15:36.000000 ehdg_pupil_detector-3.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-16 01:16:31.947422 ehdg_pupil_detector-3.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-16 01:16:31.916506 ehdg_pupil_detector-3.1.1/src/
+drwxrwxrwx   0        0        0        0 2024-04-16 01:16:31.923486 ehdg_pupil_detector-3.1.1/src/ehdg_pupil_detector/
+-rw-rw-rw-   0        0        0        0 2023-11-05 22:27:51.000000 ehdg_pupil_detector-3.1.1/src/ehdg_pupil_detector/__init__.py
+-rw-rw-rw-   0        0        0    22389 2024-01-03 22:00:51.000000 ehdg_pupil_detector-3.1.1/src/ehdg_pupil_detector/ehdg_pupil_detector.py
+-rw-rw-rw-   0        0        0      260 2024-04-15 01:15:20.000000 ehdg_pupil_detector-3.1.1/src/ehdg_pupil_detector/opm_detector_config.json
+-rw-rw-rw-   0        0        0    11990 2024-04-16 01:15:13.000000 ehdg_pupil_detector-3.1.1/src/ehdg_pupil_detector/opmtrack.py
+drwxrwxrwx   0        0        0        0 2024-04-16 01:16:31.944431 ehdg_pupil_detector-3.1.1/src/ehdg_pupil_detector.egg-info/
+-rw-rw-rw-   0        0        0     4068 2024-04-16 01:16:31.000000 ehdg_pupil_detector-3.1.1/src/ehdg_pupil_detector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      484 2024-04-16 01:16:31.000000 ehdg_pupil_detector-3.1.1/src/ehdg_pupil_detector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 01:16:31.000000 ehdg_pupil_detector-3.1.1/src/ehdg_pupil_detector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2024-04-16 01:16:31.000000 ehdg_pupil_detector-3.1.1/src/ehdg_pupil_detector.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       98 2024-04-16 01:16:31.000000 ehdg_pupil_detector-3.1.1/src/ehdg_pupil_detector.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-04-16 01:16:31.000000 ehdg_pupil_detector-3.1.1/src/ehdg_pupil_detector.egg-info/top_level.txt
```

### Comparing `ehdg_pupil_detector-3.1.0/LICENSE` & `ehdg_pupil_detector-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ehdg_pupil_detector-3.1.0/PKG-INFO` & `ehdg_pupil_detector-3.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ehdg_pupil_detector
-Version: 3.1.0
+Version: 3.1.1
 Summary: Python Library for Pupil Detector of Eye Health Diagnostic Group
 Author-email: Zaw Lin Tun <zawlintun1511@gmail.com>
 Project-URL: Homepage, https://github.com/jtur044/ehdg_pupil_detector
 Project-URL: Bug Tracker, https://github.com/jtur044/ehdg_pupil_detector/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `ehdg_pupil_detector-3.1.0/README.md` & `ehdg_pupil_detector-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ehdg_pupil_detector-3.1.0/pyproject.toml` & `ehdg_pupil_detector-3.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ehdg_pupil_detector"
-version = "3.1.0"
+version = "3.1.1"
 authors = [
   { name="Zaw Lin Tun", email="zawlintun1511@gmail.com" },
 ]
 description = "Python Library for Pupil Detector of Eye Health Diagnostic Group"
 readme = "README.md"
 dependencies = ["setuptools>=61.0", "opencv-python>=4.8.1.78", "scipy>=1.11.3", "numpy>=1.26.1", "commentjson", "ehdg_tools", "numpy"]
 requires-python = ">=3.9"
```

### Comparing `ehdg_pupil_detector-3.1.0/src/ehdg_pupil_detector/ehdg_pupil_detector.py` & `ehdg_pupil_detector-3.1.1/src/ehdg_pupil_detector/ehdg_pupil_detector.py`

 * *Files identical despite different names*

### Comparing `ehdg_pupil_detector-3.1.0/src/ehdg_pupil_detector/opmtrack.py` & `ehdg_pupil_detector-3.1.1/src/ehdg_pupil_detector/opmtrack.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,14 +152,15 @@
                 for return_data in buffer.buffer:
                     if not got_first_data:
                         got_first_data = True
                     else:
                         temp_dict = get_data_dict(return_data, frame_rate, frame_width, frame_height, direction_input)
                         csv_writer.writerow(temp_dict)
                 destination_file.close()
+                v_writer.release()
                 print(f"The opmtrack_result folder is created in {out_dir}.")
                 print(f"Result folder dir: {out_folder}.")
                 print(f"Result csv dir: {out_csv_dir}.")
                 print(f"Result video dir: {out_video_dir}.")
                 break
```

### Comparing `ehdg_pupil_detector-3.1.0/src/ehdg_pupil_detector.egg-info/PKG-INFO` & `ehdg_pupil_detector-3.1.1/src/ehdg_pupil_detector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ehdg_pupil_detector
-Version: 3.1.0
+Version: 3.1.1
 Summary: Python Library for Pupil Detector of Eye Health Diagnostic Group
 Author-email: Zaw Lin Tun <zawlintun1511@gmail.com>
 Project-URL: Homepage, https://github.com/jtur044/ehdg_pupil_detector
 Project-URL: Bug Tracker, https://github.com/jtur044/ehdg_pupil_detector/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

