# Comparing `tmp/deepfacey-0.0.85.tar.gz` & `tmp/deepfacey-0.0.86.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepfacey-0.0.85.tar", last modified: Thu Feb 29 03:28:10 2024, max compression
+gzip compressed data, was "deepfacey-0.0.86.tar", last modified: Tue Apr 16 03:21:30 2024, max compression
```

## Comparing `deepfacey-0.0.85.tar` & `deepfacey-0.0.86.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxrwxr-x   0 alfazari  (1000) alfazari  (1000)        0 2024-02-29 03:28:10.173330 deepfacey-0.0.85/
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     1077 2024-02-23 05:45:27.000000 deepfacey-0.0.85/LICENSE
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)    24452 2024-02-29 03:28:10.173330 deepfacey-0.0.85/PKG-INFO
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)    23934 2024-02-23 05:45:27.000000 deepfacey-0.0.85/README.md
-drwxrwxr-x   0 alfazari  (1000) alfazari  (1000)        0 2024-02-29 03:28:10.165331 deepfacey-0.0.85/deepfacey/
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)    21008 2024-02-29 03:19:42.000000 deepfacey-0.0.85/deepfacey/DeepFace.py
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)       23 2024-02-23 05:45:27.000000 deepfacey-0.0.85/deepfacey/__init__.py
-drwxrwxr-x   0 alfazari  (1000) alfazari  (1000)        0 2024-02-29 03:28:10.165331 deepfacey-0.0.85/deepfacey/api/
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)        0 2024-02-23 05:45:27.000000 deepfacey-0.0.85/deepfacey/api/__init__.py
-drwxrwxr-x   0 alfazari  (1000) alfazari  (1000)        0 2024-02-29 03:28:10.165331 deepfacey-0.0.85/deepfacey/api/src/
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)        0 2024-02-23 05:45:27.000000 deepfacey-0.0.85/deepfacey/api/src/__init__.py
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)      306 2024-02-23 05:45:27.000000 deepfacey-0.0.85/deepfacey/api/src/api.py
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)      207 2024-02-29 03:19:42.000000 deepfacey-0.0.85/deepfacey/api/src/app.py
-drwxrwxr-x   0 alfazari  (1000) alfazari  (1000)        0 2024-02-29 03:28:10.165331 deepfacey-0.0.85/deepfacey/api/src/modules/
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)        0 2024-02-23 05:45:27.000000 deepfacey-0.0.85/deepfacey/api/src/modules/__init__.py
-drwxrwxr-x   0 alfazari  (1000) alfazari  (1000)        0 2024-02-29 03:28:10.165331 deepfacey-0.0.85/deepfacey/api/src/modules/core/
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)        0 2024-02-23 05:45:27.000000 deepfacey-0.0.85/deepfacey/api/src/modules/core/__init__.py
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     3099 2024-02-29 03:19:42.000000 deepfacey-0.0.85/deepfacey/api/src/modules/core/routes.py
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     1666 2024-02-29 03:19:42.000000 deepfacey-0.0.85/deepfacey/api/src/modules/core/service.py
-drwxrwxr-x   0 alfazari  (1000) alfazari  (1000)        0 2024-02-29 03:28:10.169330 deepfacey-0.0.85/deepfacey/basemodels/
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     5491 2024-02-29 03:19:42.000000 deepfacey-0.0.85/deepfacey/basemodels/ArcFace.py
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     3169 2024-02-29 03:19:42.000000 deepfacey-0.0.85/deepfacey/basemodels/DeepID.py
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     3071 2024-02-29 03:19:42.000000 deepfacey-0.0.85/deepfacey/basemodels/Dlib.py
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)    62034 2024-02-29 03:19:42.000000 deepfacey-0.0.85/deepfacey/basemodels/Facenet.py
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     3592 2024-02-29 03:19:42.000000 deepfacey-0.0.85/deepfacey/basemodels/FbDeepFace.py
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)    17833 2024-02-29 03:19:42.000000 deepfacey-0.0.85/deepfacey/basemodels/OpenFace.py
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     2454 2024-02-29 03:19:42.000000 deepfacey-0.0.85/deepfacey/basemodels/SFace.py
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     5481 2024-02-29 03:19:42.000000 deepfacey-0.0.85/deepfacey/basemodels/VGGFace.py
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)        0 2024-02-23 05:45:27.000000 deepfacey-0.0.85/deepfacey/basemodels/__init__.py
-drwxrwxr-x   0 alfazari  (1000) alfazari  (1000)        0 2024-02-29 03:28:10.169330 deepfacey-0.0.85/deepfacey/commons/
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)        0 2024-02-23 05:45:27.000000 deepfacey-0.0.85/deepfacey/commons/__init__.py
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)      117 2024-02-23 05:45:27.000000 deepfacey-0.0.85/deepfacey/commons/constant.py
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)      972 2024-02-29 03:19:42.000000 deepfacey-0.0.85/deepfacey/commons/folder_utils.py
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     1294 2024-02-23 05:45:27.000000 deepfacey-0.0.85/deepfacey/commons/logger.py
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)      352 2024-02-29 03:19:42.000000 deepfacey-0.0.85/deepfacey/commons/package_utils.py
-drwxrwxr-x   0 alfazari  (1000) alfazari  (1000)        0 2024-02-29 03:28:10.169330 deepfacey-0.0.85/deepfacey/detectors/
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     6449 2024-02-29 03:19:42.000000 deepfacey-0.0.85/deepfacey/detectors/DetectorWrapper.py
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     3449 2024-02-29 03:19:42.000000 deepfacey-0.0.85/deepfacey/detectors/Dlib.py
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     2649 2024-02-29 03:19:42.000000 deepfacey-0.0.85/deepfacey/detectors/FastMtCnn.py
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     2932 2024-02-29 03:19:42.000000 deepfacey-0.0.85/deepfacey/detectors/MediaPipe.py
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     1593 2024-02-29 03:19:42.000000 deepfacey-0.0.85/deepfacey/detectors/MtCnn.py
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     5605 2024-02-29 03:19:42.000000 deepfacey-0.0.85/deepfacey/detectors/OpenCv.py
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     1720 2024-02-29 03:19:42.000000 deepfacey-0.0.85/deepfacey/detectors/RetinaFace.py
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     4869 2024-02-29 03:19:42.000000 deepfacey-0.0.85/deepfacey/detectors/Ssd.py
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     4399 2024-02-29 03:19:42.000000 deepfacey-0.0.85/deepfacey/detectors/Yolo.py
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     4956 2024-02-29 03:19:42.000000 deepfacey-0.0.85/deepfacey/detectors/YuNet.py
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)        0 2024-02-23 05:45:27.000000 deepfacey-0.0.85/deepfacey/detectors/__init__.py
-drwxrwxr-x   0 alfazari  (1000) alfazari  (1000)        0 2024-02-29 03:28:10.169330 deepfacey-0.0.85/deepfacey/extendedmodels/
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     2636 2024-02-29 03:19:42.000000 deepfacey-0.0.85/deepfacey/extendedmodels/Age.py
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     3155 2024-02-29 03:19:42.000000 deepfacey-0.0.85/deepfacey/extendedmodels/Emotion.py
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     2361 2024-02-29 03:19:42.000000 deepfacey-0.0.85/deepfacey/extendedmodels/Gender.py
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     2359 2024-02-29 03:19:42.000000 deepfacey-0.0.85/deepfacey/extendedmodels/Race.py
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)        0 2024-02-23 05:45:27.000000 deepfacey-0.0.85/deepfacey/extendedmodels/__init__.py
-drwxrwxr-x   0 alfazari  (1000) alfazari  (1000)        0 2024-02-29 03:28:10.169330 deepfacey-0.0.85/deepfacey/models/
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)      578 2024-02-29 03:19:42.000000 deepfacey-0.0.85/deepfacey/models/Demography.py
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     1660 2024-02-23 05:45:27.000000 deepfacey-0.0.85/deepfacey/models/Detector.py
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)      653 2024-02-29 03:19:42.000000 deepfacey-0.0.85/deepfacey/models/FacialRecognition.py
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)        0 2024-02-23 05:45:27.000000 deepfacey-0.0.85/deepfacey/models/__init__.py
-drwxrwxr-x   0 alfazari  (1000) alfazari  (1000)        0 2024-02-29 03:28:10.173330 deepfacey-0.0.85/deepfacey/modules/
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)        0 2024-02-23 05:45:27.000000 deepfacey-0.0.85/deepfacey/modules/__init__.py
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     8170 2024-02-29 03:19:42.000000 deepfacey-0.0.85/deepfacey/modules/demography.py
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     7866 2024-02-29 03:19:42.000000 deepfacey-0.0.85/deepfacey/modules/detection.py
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     1565 2024-02-29 03:19:42.000000 deepfacey-0.0.85/deepfacey/modules/modeling.py
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     4145 2024-02-23 05:45:27.000000 deepfacey-0.0.85/deepfacey/modules/preprocessing.py
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)    33894 2024-02-29 03:19:42.000000 deepfacey-0.0.85/deepfacey/modules/realtime.py
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)    13641 2024-02-29 03:19:42.000000 deepfacey-0.0.85/deepfacey/modules/recognition.py
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     4738 2024-02-29 03:19:42.000000 deepfacey-0.0.85/deepfacey/modules/representation.py
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)    10451 2024-02-29 03:19:42.000000 deepfacey-0.0.85/deepfacey/modules/verification.py
-drwxrwxr-x   0 alfazari  (1000) alfazari  (1000)        0 2024-02-29 03:28:10.165331 deepfacey-0.0.85/deepfacey.egg-info/
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)    24452 2024-02-29 03:28:10.000000 deepfacey-0.0.85/deepfacey.egg-info/PKG-INFO
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     2138 2024-02-29 03:28:10.000000 deepfacey-0.0.85/deepfacey.egg-info/SOURCES.txt
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)        1 2024-02-29 03:28:10.000000 deepfacey-0.0.85/deepfacey.egg-info/dependency_links.txt
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)       53 2024-02-29 03:28:10.000000 deepfacey-0.0.85/deepfacey.egg-info/entry_points.txt
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)      199 2024-02-29 03:28:10.000000 deepfacey-0.0.85/deepfacey.egg-info/requires.txt
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)       10 2024-02-29 03:28:10.000000 deepfacey-0.0.85/deepfacey.egg-info/top_level.txt
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)       27 2024-02-23 05:45:27.000000 deepfacey-0.0.85/package_info.json
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)      210 2024-02-23 05:45:27.000000 deepfacey-0.0.85/requirements.txt
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)       38 2024-02-29 03:28:10.173330 deepfacey-0.0.85/setup.cfg
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     1206 2024-02-29 03:23:18.000000 deepfacey-0.0.85/setup.py
-drwxrwxr-x   0 alfazari  (1000) alfazari  (1000)        0 2024-02-29 03:28:10.173330 deepfacey-0.0.85/tests/
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     4550 2024-02-29 03:19:41.000000 deepfacey-0.0.85/tests/test_analyze.py
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     4361 2024-02-29 03:19:41.000000 deepfacey-0.0.85/tests/test_api.py
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     1781 2024-02-29 03:19:41.000000 deepfacey-0.0.85/tests/test_enforce_detection.py
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     1773 2024-02-29 03:19:41.000000 deepfacey-0.0.85/tests/test_extract_faces.py
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     2312 2024-02-29 03:19:41.000000 deepfacey-0.0.85/tests/test_find.py
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     1963 2024-02-29 03:19:41.000000 deepfacey-0.0.85/tests/test_represent.py
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     4051 2024-02-29 03:19:41.000000 deepfacey-0.0.85/tests/test_verify.py
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)      410 2024-02-29 03:19:41.000000 deepfacey-0.0.85/tests/test_version.py
+drwxrwxr-x   0 alfazari  (1000) alfazari  (1000)        0 2024-04-16 03:21:30.226312 deepfacey-0.0.86/
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     1077 2024-02-23 05:45:27.000000 deepfacey-0.0.86/LICENSE
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)    24452 2024-04-16 03:21:30.222311 deepfacey-0.0.86/PKG-INFO
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)    23934 2024-02-23 05:45:27.000000 deepfacey-0.0.86/README.md
+drwxrwxr-x   0 alfazari  (1000) alfazari  (1000)        0 2024-04-16 03:21:30.214311 deepfacey-0.0.86/deepfacey/
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)    21008 2024-02-29 03:19:42.000000 deepfacey-0.0.86/deepfacey/DeepFace.py
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)       23 2024-02-23 05:45:27.000000 deepfacey-0.0.86/deepfacey/__init__.py
+drwxrwxr-x   0 alfazari  (1000) alfazari  (1000)        0 2024-04-16 03:21:30.214311 deepfacey-0.0.86/deepfacey/api/
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)        0 2024-02-23 05:45:27.000000 deepfacey-0.0.86/deepfacey/api/__init__.py
+drwxrwxr-x   0 alfazari  (1000) alfazari  (1000)        0 2024-04-16 03:21:30.214311 deepfacey-0.0.86/deepfacey/api/src/
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)        0 2024-02-23 05:45:27.000000 deepfacey-0.0.86/deepfacey/api/src/__init__.py
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)      306 2024-02-23 05:45:27.000000 deepfacey-0.0.86/deepfacey/api/src/api.py
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)      207 2024-02-29 03:19:42.000000 deepfacey-0.0.86/deepfacey/api/src/app.py
+drwxrwxr-x   0 alfazari  (1000) alfazari  (1000)        0 2024-04-16 03:21:30.214311 deepfacey-0.0.86/deepfacey/api/src/modules/
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)        0 2024-02-23 05:45:27.000000 deepfacey-0.0.86/deepfacey/api/src/modules/__init__.py
+drwxrwxr-x   0 alfazari  (1000) alfazari  (1000)        0 2024-04-16 03:21:30.218311 deepfacey-0.0.86/deepfacey/api/src/modules/core/
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)        0 2024-02-23 05:45:27.000000 deepfacey-0.0.86/deepfacey/api/src/modules/core/__init__.py
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     3099 2024-02-29 03:19:42.000000 deepfacey-0.0.86/deepfacey/api/src/modules/core/routes.py
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     1666 2024-02-29 03:19:42.000000 deepfacey-0.0.86/deepfacey/api/src/modules/core/service.py
+drwxrwxr-x   0 alfazari  (1000) alfazari  (1000)        0 2024-04-16 03:21:30.218311 deepfacey-0.0.86/deepfacey/basemodels/
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     5491 2024-02-29 03:19:42.000000 deepfacey-0.0.86/deepfacey/basemodels/ArcFace.py
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     3169 2024-02-29 03:19:42.000000 deepfacey-0.0.86/deepfacey/basemodels/DeepID.py
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     3071 2024-02-29 03:19:42.000000 deepfacey-0.0.86/deepfacey/basemodels/Dlib.py
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)    62034 2024-02-29 03:19:42.000000 deepfacey-0.0.86/deepfacey/basemodels/Facenet.py
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     3592 2024-02-29 03:19:42.000000 deepfacey-0.0.86/deepfacey/basemodels/FbDeepFace.py
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)    17833 2024-02-29 03:19:42.000000 deepfacey-0.0.86/deepfacey/basemodels/OpenFace.py
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     2454 2024-02-29 03:19:42.000000 deepfacey-0.0.86/deepfacey/basemodels/SFace.py
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     5481 2024-02-29 03:19:42.000000 deepfacey-0.0.86/deepfacey/basemodels/VGGFace.py
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)        0 2024-02-23 05:45:27.000000 deepfacey-0.0.86/deepfacey/basemodels/__init__.py
+drwxrwxr-x   0 alfazari  (1000) alfazari  (1000)        0 2024-04-16 03:21:30.218311 deepfacey-0.0.86/deepfacey/commons/
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)        0 2024-02-23 05:45:27.000000 deepfacey-0.0.86/deepfacey/commons/__init__.py
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)      117 2024-02-23 05:45:27.000000 deepfacey-0.0.86/deepfacey/commons/constant.py
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)      972 2024-02-29 03:19:42.000000 deepfacey-0.0.86/deepfacey/commons/folder_utils.py
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     1294 2024-02-23 05:45:27.000000 deepfacey-0.0.86/deepfacey/commons/logger.py
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)      352 2024-02-29 03:19:42.000000 deepfacey-0.0.86/deepfacey/commons/package_utils.py
+drwxrwxr-x   0 alfazari  (1000) alfazari  (1000)        0 2024-04-16 03:21:30.218311 deepfacey-0.0.86/deepfacey/detectors/
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     6449 2024-02-29 03:19:42.000000 deepfacey-0.0.86/deepfacey/detectors/DetectorWrapper.py
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     3449 2024-02-29 03:19:42.000000 deepfacey-0.0.86/deepfacey/detectors/Dlib.py
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     2649 2024-02-29 03:19:42.000000 deepfacey-0.0.86/deepfacey/detectors/FastMtCnn.py
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     2932 2024-02-29 03:19:42.000000 deepfacey-0.0.86/deepfacey/detectors/MediaPipe.py
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     1593 2024-02-29 03:19:42.000000 deepfacey-0.0.86/deepfacey/detectors/MtCnn.py
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     5605 2024-02-29 03:19:42.000000 deepfacey-0.0.86/deepfacey/detectors/OpenCv.py
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     1720 2024-02-29 03:19:42.000000 deepfacey-0.0.86/deepfacey/detectors/RetinaFace.py
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     4869 2024-02-29 03:19:42.000000 deepfacey-0.0.86/deepfacey/detectors/Ssd.py
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     4399 2024-04-04 08:17:03.000000 deepfacey-0.0.86/deepfacey/detectors/Yolo.py
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     4956 2024-02-29 03:19:42.000000 deepfacey-0.0.86/deepfacey/detectors/YuNet.py
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)        0 2024-02-23 05:45:27.000000 deepfacey-0.0.86/deepfacey/detectors/__init__.py
+drwxrwxr-x   0 alfazari  (1000) alfazari  (1000)        0 2024-04-16 03:21:30.222311 deepfacey-0.0.86/deepfacey/extendedmodels/
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     2636 2024-02-29 03:19:42.000000 deepfacey-0.0.86/deepfacey/extendedmodels/Age.py
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     3155 2024-02-29 03:19:42.000000 deepfacey-0.0.86/deepfacey/extendedmodels/Emotion.py
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     2361 2024-02-29 03:19:42.000000 deepfacey-0.0.86/deepfacey/extendedmodels/Gender.py
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     2359 2024-02-29 03:19:42.000000 deepfacey-0.0.86/deepfacey/extendedmodels/Race.py
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)        0 2024-02-23 05:45:27.000000 deepfacey-0.0.86/deepfacey/extendedmodels/__init__.py
+drwxrwxr-x   0 alfazari  (1000) alfazari  (1000)        0 2024-04-16 03:21:30.222311 deepfacey-0.0.86/deepfacey/models/
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)      578 2024-02-29 03:19:42.000000 deepfacey-0.0.86/deepfacey/models/Demography.py
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     1660 2024-02-23 05:45:27.000000 deepfacey-0.0.86/deepfacey/models/Detector.py
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)      653 2024-02-29 03:19:42.000000 deepfacey-0.0.86/deepfacey/models/FacialRecognition.py
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)        0 2024-02-23 05:45:27.000000 deepfacey-0.0.86/deepfacey/models/__init__.py
+drwxrwxr-x   0 alfazari  (1000) alfazari  (1000)        0 2024-04-16 03:21:30.222311 deepfacey-0.0.86/deepfacey/modules/
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)        0 2024-02-23 05:45:27.000000 deepfacey-0.0.86/deepfacey/modules/__init__.py
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     8170 2024-02-29 03:19:42.000000 deepfacey-0.0.86/deepfacey/modules/demography.py
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     7866 2024-02-29 03:19:42.000000 deepfacey-0.0.86/deepfacey/modules/detection.py
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     1565 2024-02-29 03:19:42.000000 deepfacey-0.0.86/deepfacey/modules/modeling.py
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     4145 2024-02-23 05:45:27.000000 deepfacey-0.0.86/deepfacey/modules/preprocessing.py
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)    33894 2024-02-29 03:19:42.000000 deepfacey-0.0.86/deepfacey/modules/realtime.py
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)    13641 2024-02-29 03:19:42.000000 deepfacey-0.0.86/deepfacey/modules/recognition.py
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     4738 2024-02-29 03:19:42.000000 deepfacey-0.0.86/deepfacey/modules/representation.py
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)    10451 2024-02-29 03:19:42.000000 deepfacey-0.0.86/deepfacey/modules/verification.py
+drwxrwxr-x   0 alfazari  (1000) alfazari  (1000)        0 2024-04-16 03:21:30.214311 deepfacey-0.0.86/deepfacey.egg-info/
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)    24452 2024-04-16 03:21:30.000000 deepfacey-0.0.86/deepfacey.egg-info/PKG-INFO
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     2138 2024-04-16 03:21:30.000000 deepfacey-0.0.86/deepfacey.egg-info/SOURCES.txt
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)        1 2024-04-16 03:21:30.000000 deepfacey-0.0.86/deepfacey.egg-info/dependency_links.txt
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)       53 2024-04-16 03:21:30.000000 deepfacey-0.0.86/deepfacey.egg-info/entry_points.txt
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)      201 2024-04-16 03:21:30.000000 deepfacey-0.0.86/deepfacey.egg-info/requires.txt
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)       10 2024-04-16 03:21:30.000000 deepfacey-0.0.86/deepfacey.egg-info/top_level.txt
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)       26 2024-04-16 03:20:54.000000 deepfacey-0.0.86/package_info.json
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)      212 2024-04-16 03:19:06.000000 deepfacey-0.0.86/requirements.txt
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)       38 2024-04-16 03:21:30.226312 deepfacey-0.0.86/setup.cfg
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     1206 2024-02-29 03:23:18.000000 deepfacey-0.0.86/setup.py
+drwxrwxr-x   0 alfazari  (1000) alfazari  (1000)        0 2024-04-16 03:21:30.222311 deepfacey-0.0.86/tests/
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     4550 2024-02-29 03:19:41.000000 deepfacey-0.0.86/tests/test_analyze.py
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     4361 2024-02-29 03:19:41.000000 deepfacey-0.0.86/tests/test_api.py
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     1781 2024-02-29 03:19:41.000000 deepfacey-0.0.86/tests/test_enforce_detection.py
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     1773 2024-02-29 03:19:41.000000 deepfacey-0.0.86/tests/test_extract_faces.py
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     2312 2024-02-29 03:19:41.000000 deepfacey-0.0.86/tests/test_find.py
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     1963 2024-02-29 03:19:41.000000 deepfacey-0.0.86/tests/test_represent.py
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     4051 2024-02-29 03:19:41.000000 deepfacey-0.0.86/tests/test_verify.py
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)      410 2024-02-29 03:19:41.000000 deepfacey-0.0.86/tests/test_version.py
```

### Comparing `deepfacey-0.0.85/LICENSE` & `deepfacey-0.0.86/LICENSE`

 * *Files identical despite different names*

### Comparing `deepfacey-0.0.85/PKG-INFO` & `deepfacey-0.0.86/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepfacey
-Version: 0.0.85
+Version: 0.0.86
 Summary: A Lightweight Face Recognition and Facial Attribute Analysis Framework (Age, Gender, Emotion, Race) for Python
 Home-page: https://github.com/serengil/deepface
 Author: Sefik Ilkin Serengil
 Author-email: serengil@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `deepfacey-0.0.85/README.md` & `deepfacey-0.0.86/README.md`

 * *Files identical despite different names*

### Comparing `deepfacey-0.0.85/deepfacey/DeepFace.py` & `deepfacey-0.0.86/deepfacey/DeepFace.py`

 * *Files identical despite different names*

### Comparing `deepfacey-0.0.85/deepfacey/api/src/modules/core/routes.py` & `deepfacey-0.0.86/deepfacey/api/src/modules/core/routes.py`

 * *Files identical despite different names*

### Comparing `deepfacey-0.0.85/deepfacey/api/src/modules/core/service.py` & `deepfacey-0.0.86/deepfacey/api/src/modules/core/service.py`

 * *Files identical despite different names*

### Comparing `deepfacey-0.0.85/deepfacey/basemodels/ArcFace.py` & `deepfacey-0.0.86/deepfacey/basemodels/ArcFace.py`

 * *Files identical despite different names*

### Comparing `deepfacey-0.0.85/deepfacey/basemodels/DeepID.py` & `deepfacey-0.0.86/deepfacey/basemodels/DeepID.py`

 * *Files identical despite different names*

### Comparing `deepfacey-0.0.85/deepfacey/basemodels/Dlib.py` & `deepfacey-0.0.86/deepfacey/basemodels/Dlib.py`

 * *Files identical despite different names*

### Comparing `deepfacey-0.0.85/deepfacey/basemodels/Facenet.py` & `deepfacey-0.0.86/deepfacey/basemodels/Facenet.py`

 * *Files identical despite different names*

### Comparing `deepfacey-0.0.85/deepfacey/basemodels/FbDeepFace.py` & `deepfacey-0.0.86/deepfacey/basemodels/FbDeepFace.py`

 * *Files identical despite different names*

### Comparing `deepfacey-0.0.85/deepfacey/basemodels/OpenFace.py` & `deepfacey-0.0.86/deepfacey/basemodels/OpenFace.py`

 * *Files identical despite different names*

### Comparing `deepfacey-0.0.85/deepfacey/basemodels/SFace.py` & `deepfacey-0.0.86/deepfacey/basemodels/SFace.py`

 * *Files identical despite different names*

### Comparing `deepfacey-0.0.85/deepfacey/basemodels/VGGFace.py` & `deepfacey-0.0.86/deepfacey/basemodels/VGGFace.py`

 * *Files identical despite different names*

### Comparing `deepfacey-0.0.85/deepfacey/commons/folder_utils.py` & `deepfacey-0.0.86/deepfacey/commons/folder_utils.py`

 * *Files identical despite different names*

### Comparing `deepfacey-0.0.85/deepfacey/commons/logger.py` & `deepfacey-0.0.86/deepfacey/commons/logger.py`

 * *Files identical despite different names*

### Comparing `deepfacey-0.0.85/deepfacey/detectors/DetectorWrapper.py` & `deepfacey-0.0.86/deepfacey/detectors/DetectorWrapper.py`

 * *Files identical despite different names*

### Comparing `deepfacey-0.0.85/deepfacey/detectors/Dlib.py` & `deepfacey-0.0.86/deepfacey/detectors/Dlib.py`

 * *Files identical despite different names*

### Comparing `deepfacey-0.0.85/deepfacey/detectors/FastMtCnn.py` & `deepfacey-0.0.86/deepfacey/detectors/FastMtCnn.py`

 * *Files identical despite different names*

### Comparing `deepfacey-0.0.85/deepfacey/detectors/MediaPipe.py` & `deepfacey-0.0.86/deepfacey/detectors/MediaPipe.py`

 * *Files identical despite different names*

### Comparing `deepfacey-0.0.85/deepfacey/detectors/MtCnn.py` & `deepfacey-0.0.86/deepfacey/detectors/MtCnn.py`

 * *Files identical despite different names*

### Comparing `deepfacey-0.0.85/deepfacey/detectors/OpenCv.py` & `deepfacey-0.0.86/deepfacey/detectors/OpenCv.py`

 * *Files identical despite different names*

### Comparing `deepfacey-0.0.85/deepfacey/detectors/RetinaFace.py` & `deepfacey-0.0.86/deepfacey/detectors/RetinaFace.py`

 * *Files identical despite different names*

### Comparing `deepfacey-0.0.85/deepfacey/detectors/Ssd.py` & `deepfacey-0.0.86/deepfacey/detectors/Ssd.py`

 * *Files identical despite different names*

### Comparing `deepfacey-0.0.85/deepfacey/detectors/Yolo.py` & `deepfacey-0.0.86/deepfacey/detectors/Yolo.py`

 * *Files identical despite different names*

### Comparing `deepfacey-0.0.85/deepfacey/detectors/YuNet.py` & `deepfacey-0.0.86/deepfacey/detectors/YuNet.py`

 * *Files identical despite different names*

### Comparing `deepfacey-0.0.85/deepfacey/extendedmodels/Age.py` & `deepfacey-0.0.86/deepfacey/extendedmodels/Age.py`

 * *Files identical despite different names*

### Comparing `deepfacey-0.0.85/deepfacey/extendedmodels/Emotion.py` & `deepfacey-0.0.86/deepfacey/extendedmodels/Emotion.py`

 * *Files identical despite different names*

### Comparing `deepfacey-0.0.85/deepfacey/extendedmodels/Gender.py` & `deepfacey-0.0.86/deepfacey/extendedmodels/Gender.py`

 * *Files identical despite different names*

### Comparing `deepfacey-0.0.85/deepfacey/extendedmodels/Race.py` & `deepfacey-0.0.86/deepfacey/extendedmodels/Race.py`

 * *Files identical despite different names*

### Comparing `deepfacey-0.0.85/deepfacey/models/Demography.py` & `deepfacey-0.0.86/deepfacey/models/Demography.py`

 * *Files identical despite different names*

### Comparing `deepfacey-0.0.85/deepfacey/models/Detector.py` & `deepfacey-0.0.86/deepfacey/models/Detector.py`

 * *Files identical despite different names*

### Comparing `deepfacey-0.0.85/deepfacey/models/FacialRecognition.py` & `deepfacey-0.0.86/deepfacey/models/FacialRecognition.py`

 * *Files identical despite different names*

### Comparing `deepfacey-0.0.85/deepfacey/modules/demography.py` & `deepfacey-0.0.86/deepfacey/modules/demography.py`

 * *Files identical despite different names*

### Comparing `deepfacey-0.0.85/deepfacey/modules/detection.py` & `deepfacey-0.0.86/deepfacey/modules/detection.py`

 * *Files identical despite different names*

### Comparing `deepfacey-0.0.85/deepfacey/modules/modeling.py` & `deepfacey-0.0.86/deepfacey/modules/modeling.py`

 * *Files identical despite different names*

### Comparing `deepfacey-0.0.85/deepfacey/modules/preprocessing.py` & `deepfacey-0.0.86/deepfacey/modules/preprocessing.py`

 * *Files identical despite different names*

### Comparing `deepfacey-0.0.85/deepfacey/modules/realtime.py` & `deepfacey-0.0.86/deepfacey/modules/realtime.py`

 * *Files identical despite different names*

### Comparing `deepfacey-0.0.85/deepfacey/modules/recognition.py` & `deepfacey-0.0.86/deepfacey/modules/recognition.py`

 * *Files identical despite different names*

### Comparing `deepfacey-0.0.85/deepfacey/modules/representation.py` & `deepfacey-0.0.86/deepfacey/modules/representation.py`

 * *Files identical despite different names*

### Comparing `deepfacey-0.0.85/deepfacey/modules/verification.py` & `deepfacey-0.0.86/deepfacey/modules/verification.py`

 * *Files identical despite different names*

### Comparing `deepfacey-0.0.85/deepfacey.egg-info/PKG-INFO` & `deepfacey-0.0.86/deepfacey.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepfacey
-Version: 0.0.85
+Version: 0.0.86
 Summary: A Lightweight Face Recognition and Facial Attribute Analysis Framework (Age, Gender, Emotion, Race) for Python
 Home-page: https://github.com/serengil/deepface
 Author: Sefik Ilkin Serengil
 Author-email: serengil@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `deepfacey-0.0.85/deepfacey.egg-info/SOURCES.txt` & `deepfacey-0.0.86/deepfacey.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deepfacey-0.0.85/setup.py` & `deepfacey-0.0.86/setup.py`

 * *Files identical despite different names*

### Comparing `deepfacey-0.0.85/tests/test_analyze.py` & `deepfacey-0.0.86/tests/test_analyze.py`

 * *Files identical despite different names*

### Comparing `deepfacey-0.0.85/tests/test_api.py` & `deepfacey-0.0.86/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `deepfacey-0.0.85/tests/test_enforce_detection.py` & `deepfacey-0.0.86/tests/test_enforce_detection.py`

 * *Files identical despite different names*

### Comparing `deepfacey-0.0.85/tests/test_extract_faces.py` & `deepfacey-0.0.86/tests/test_extract_faces.py`

 * *Files identical despite different names*

### Comparing `deepfacey-0.0.85/tests/test_find.py` & `deepfacey-0.0.86/tests/test_find.py`

 * *Files identical despite different names*

### Comparing `deepfacey-0.0.85/tests/test_represent.py` & `deepfacey-0.0.86/tests/test_represent.py`

 * *Files identical despite different names*

### Comparing `deepfacey-0.0.85/tests/test_verify.py` & `deepfacey-0.0.86/tests/test_verify.py`

 * *Files identical despite different names*

