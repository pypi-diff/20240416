# Comparing `tmp/deepface-0.0.9.tar.gz` & `tmp/deepface-0.0.90.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\deepface-0.0.9.tar", last modified: Tue Feb 25 19:13:28 2020, max compression
+gzip compressed data, was "dist/deepface-0.0.90.tar", last modified: Tue Apr 16 21:04:24 2024, max compression
```

## Comparing `deepface-0.0.9.tar` & `deepface-0.0.90.tar`

### file list

```diff
@@ -1,30 +1,82 @@
-drwxrwxrwx   0        0        0        0 2020-02-25 19:13:28.000000 deepface-0.0.9/
-drwxrwxrwx   0        0        0        0 2020-02-25 19:13:28.000000 deepface-0.0.9/deepface/
-drwxrwxrwx   0        0        0        0 2020-02-25 19:13:28.000000 deepface-0.0.9/deepface/basemodels/
--rw-rw-rw-   0        0        0    49346 2020-02-25 18:26:59.000000 deepface-0.0.9/deepface/basemodels/Facenet.py
--rw-rw-rw-   0        0        0     1980 2020-02-25 18:26:59.000000 deepface-0.0.9/deepface/basemodels/FbDeepFace.py
--rw-rw-rw-   0        0        0    15074 2020-02-25 18:26:59.000000 deepface-0.0.9/deepface/basemodels/OpenFace.py
--rw-rw-rw-   0        0        0     2793 2020-02-25 18:26:59.000000 deepface-0.0.9/deepface/basemodels/VGGFace.py
--rw-rw-rw-   0        0        0        0 2020-02-25 18:26:59.000000 deepface-0.0.9/deepface/basemodels/__init__.py
-drwxrwxrwx   0        0        0        0 2020-02-25 19:13:28.000000 deepface-0.0.9/deepface/commons/
--rw-rw-rw-   0        0        0      919 2020-02-25 18:26:59.000000 deepface-0.0.9/deepface/commons/distance.py
--rw-rw-rw-   0        0        0     7611 2020-02-25 19:02:47.000000 deepface-0.0.9/deepface/commons/functions.py
--rw-rw-rw-   0        0        0        0 2020-02-25 18:26:59.000000 deepface-0.0.9/deepface/commons/__init__.py
--rw-rw-rw-   0        0        0     7159 2020-02-25 19:11:16.000000 deepface-0.0.9/deepface/DeepFace.py
-drwxrwxrwx   0        0        0        0 2020-02-25 19:13:28.000000 deepface-0.0.9/deepface/extendedmodels/
--rw-rw-rw-   0        0        0     1411 2020-02-25 18:26:59.000000 deepface-0.0.9/deepface/extendedmodels/Age.py
--rw-rw-rw-   0        0        0     1853 2020-02-25 18:26:59.000000 deepface-0.0.9/deepface/extendedmodels/Emotion.py
--rw-rw-rw-   0        0        0     1253 2020-02-25 18:26:59.000000 deepface-0.0.9/deepface/extendedmodels/Gender.py
--rw-rw-rw-   0        0        0     1428 2020-02-25 18:26:59.000000 deepface-0.0.9/deepface/extendedmodels/Race.py
--rw-rw-rw-   0        0        0        0 2020-02-25 18:26:59.000000 deepface-0.0.9/deepface/extendedmodels/__init__.py
--rw-rw-rw-   0        0        0        0 2020-02-25 18:26:59.000000 deepface-0.0.9/deepface/__init__.py
-drwxrwxrwx   0        0        0        0 2020-02-25 19:13:28.000000 deepface-0.0.9/deepface.egg-info/
--rw-rw-rw-   0        0        0        1 2020-02-25 19:13:27.000000 deepface-0.0.9/deepface.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     9744 2020-02-25 19:13:27.000000 deepface-0.0.9/deepface.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      140 2020-02-25 19:13:27.000000 deepface-0.0.9/deepface.egg-info/requires.txt
--rw-rw-rw-   0        0        0      635 2020-02-25 19:13:28.000000 deepface-0.0.9/deepface.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        9 2020-02-25 19:13:27.000000 deepface-0.0.9/deepface.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     9744 2020-02-25 19:13:28.000000 deepface-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     7961 2020-02-25 18:26:59.000000 deepface-0.0.9/README.md
--rw-rw-rw-   0        0        0       42 2020-02-25 19:13:28.000000 deepface-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0      918 2020-02-25 19:10:58.000000 deepface-0.0.9/setup.py
+drwxr-xr-x   0 sefik      (501) staff       (20)        0 2024-04-16 21:04:24.599128 deepface-0.0.90/
+-rw-r--r--   0 sefik      (501) staff       (20)     1077 2023-10-22 18:40:56.000000 deepface-0.0.90/LICENSE
+-rw-r--r--   0 sefik      (501) staff       (20)    26049 2024-04-16 21:04:24.598521 deepface-0.0.90/PKG-INFO
+-rw-r--r--   0 sefik      (501) staff       (20)    25497 2024-04-14 08:51:12.000000 deepface-0.0.90/README.md
+drwxr-xr-x   0 sefik      (501) staff       (20)        0 2024-04-16 21:04:24.574627 deepface-0.0.90/deepface/
+-rw-r--r--   0 sefik      (501) staff       (20)    21984 2024-04-13 07:27:53.000000 deepface-0.0.90/deepface/DeepFace.py
+-rw-r--r--   0 sefik      (501) staff       (20)       23 2024-03-24 16:59:56.000000 deepface-0.0.90/deepface/__init__.py
+drwxr-xr-x   0 sefik      (501) staff       (20)        0 2024-04-16 21:04:24.577052 deepface-0.0.90/deepface/api/
+-rw-r--r--   0 sefik      (501) staff       (20)        0 2024-02-04 13:08:55.000000 deepface-0.0.90/deepface/api/__init__.py
+drwxr-xr-x   0 sefik      (501) staff       (20)        0 2024-04-16 21:04:24.577739 deepface-0.0.90/deepface/api/src/
+-rw-r--r--   0 sefik      (501) staff       (20)        0 2024-02-04 13:08:55.000000 deepface-0.0.90/deepface/api/src/__init__.py
+-rw-r--r--   0 sefik      (501) staff       (20)      306 2024-02-04 13:08:55.000000 deepface-0.0.90/deepface/api/src/api.py
+-rw-r--r--   0 sefik      (501) staff       (20)      206 2024-02-04 13:08:55.000000 deepface-0.0.90/deepface/api/src/app.py
+drwxr-xr-x   0 sefik      (501) staff       (20)        0 2024-04-16 21:04:24.578013 deepface-0.0.90/deepface/api/src/modules/
+-rw-r--r--   0 sefik      (501) staff       (20)        0 2024-02-04 13:08:55.000000 deepface-0.0.90/deepface/api/src/modules/__init__.py
+drwxr-xr-x   0 sefik      (501) staff       (20)        0 2024-04-16 21:04:24.578686 deepface-0.0.90/deepface/api/src/modules/core/
+-rw-r--r--   0 sefik      (501) staff       (20)        0 2024-02-04 13:08:55.000000 deepface-0.0.90/deepface/api/src/modules/core/__init__.py
+-rw-r--r--   0 sefik      (501) staff       (20)     3092 2024-04-12 13:50:50.000000 deepface-0.0.90/deepface/api/src/modules/core/routes.py
+-rw-r--r--   0 sefik      (501) staff       (20)     1665 2024-02-04 13:08:55.000000 deepface-0.0.90/deepface/api/src/modules/core/service.py
+drwxr-xr-x   0 sefik      (501) staff       (20)        0 2024-04-16 21:04:24.582829 deepface-0.0.90/deepface/basemodels/
+-rw-r--r--   0 sefik      (501) staff       (20)     4962 2024-04-12 13:50:50.000000 deepface-0.0.90/deepface/basemodels/ArcFace.py
+-rw-r--r--   0 sefik      (501) staff       (20)     2641 2024-04-12 13:50:50.000000 deepface-0.0.90/deepface/basemodels/DeepID.py
+-rw-r--r--   0 sefik      (501) staff       (20)     2872 2024-04-12 13:50:50.000000 deepface-0.0.90/deepface/basemodels/Dlib.py
+-rw-r--r--   0 sefik      (501) staff       (20)    61329 2024-04-12 13:50:50.000000 deepface-0.0.90/deepface/basemodels/Facenet.py
+-rw-r--r--   0 sefik      (501) staff       (20)     3712 2024-04-12 13:50:50.000000 deepface-0.0.90/deepface/basemodels/FbDeepFace.py
+-rw-r--r--   0 sefik      (501) staff       (20)     9811 2024-04-12 13:50:50.000000 deepface-0.0.90/deepface/basemodels/GhostFaceNet.py
+-rw-r--r--   0 sefik      (501) staff       (20)    17301 2024-04-12 13:50:50.000000 deepface-0.0.90/deepface/basemodels/OpenFace.py
+-rw-r--r--   0 sefik      (501) staff       (20)     2473 2024-04-12 13:50:50.000000 deepface-0.0.90/deepface/basemodels/SFace.py
+-rw-r--r--   0 sefik      (501) staff       (20)     5610 2024-04-12 13:50:50.000000 deepface-0.0.90/deepface/basemodels/VGGFace.py
+-rw-r--r--   0 sefik      (501) staff       (20)        0 2021-09-07 17:19:21.000000 deepface-0.0.90/deepface/basemodels/__init__.py
+drwxr-xr-x   0 sefik      (501) staff       (20)        0 2024-04-16 21:04:24.584800 deepface-0.0.90/deepface/commons/
+-rw-r--r--   0 sefik      (501) staff       (20)        0 2021-09-07 17:19:21.000000 deepface-0.0.90/deepface/commons/__init__.py
+-rw-r--r--   0 sefik      (501) staff       (20)      117 2024-02-02 20:17:38.000000 deepface-0.0.90/deepface/commons/constant.py
+-rw-r--r--   0 sefik      (501) staff       (20)      951 2024-04-12 13:50:50.000000 deepface-0.0.90/deepface/commons/folder_utils.py
+-rw-r--r--   0 sefik      (501) staff       (20)     4348 2024-04-13 07:27:53.000000 deepface-0.0.90/deepface/commons/image_utils.py
+-rw-r--r--   0 sefik      (501) staff       (20)     1571 2024-04-12 13:50:50.000000 deepface-0.0.90/deepface/commons/logger.py
+-rw-r--r--   0 sefik      (501) staff       (20)     1188 2024-04-13 07:27:53.000000 deepface-0.0.90/deepface/commons/package_utils.py
+drwxr-xr-x   0 sefik      (501) staff       (20)        0 2024-04-16 21:04:24.588679 deepface-0.0.90/deepface/detectors/
+-rw-r--r--   0 sefik      (501) staff       (20)     7791 2024-04-16 19:12:52.000000 deepface-0.0.90/deepface/detectors/CenterFace.py
+-rw-r--r--   0 sefik      (501) staff       (20)     7119 2024-04-16 19:12:52.000000 deepface-0.0.90/deepface/detectors/DetectorWrapper.py
+-rw-r--r--   0 sefik      (501) staff       (20)     3787 2024-04-12 13:50:50.000000 deepface-0.0.90/deepface/detectors/Dlib.py
+-rw-r--r--   0 sefik      (501) staff       (20)     2925 2024-04-12 13:50:50.000000 deepface-0.0.90/deepface/detectors/FastMtCnn.py
+-rw-r--r--   0 sefik      (501) staff       (20)     2931 2024-03-24 16:59:56.000000 deepface-0.0.90/deepface/detectors/MediaPipe.py
+-rw-r--r--   0 sefik      (501) staff       (20)     1745 2024-03-24 16:59:56.000000 deepface-0.0.90/deepface/detectors/MtCnn.py
+-rw-r--r--   0 sefik      (501) staff       (20)     6038 2024-03-24 16:59:56.000000 deepface-0.0.90/deepface/detectors/OpenCv.py
+-rw-r--r--   0 sefik      (501) staff       (20)     1733 2024-03-24 16:59:56.000000 deepface-0.0.90/deepface/detectors/RetinaFace.py
+-rw-r--r--   0 sefik      (501) staff       (20)     5229 2024-04-12 13:50:50.000000 deepface-0.0.90/deepface/detectors/Ssd.py
+-rw-r--r--   0 sefik      (501) staff       (20)     3434 2024-04-12 13:50:50.000000 deepface-0.0.90/deepface/detectors/Yolo.py
+-rw-r--r--   0 sefik      (501) staff       (20)     5130 2024-04-12 13:50:50.000000 deepface-0.0.90/deepface/detectors/YuNet.py
+-rw-r--r--   0 sefik      (501) staff       (20)        0 2021-09-07 17:19:21.000000 deepface-0.0.90/deepface/detectors/__init__.py
+drwxr-xr-x   0 sefik      (501) staff       (20)        0 2024-04-16 21:04:24.590699 deepface-0.0.90/deepface/extendedmodels/
+-rw-r--r--   0 sefik      (501) staff       (20)     2626 2024-04-12 13:50:50.000000 deepface-0.0.90/deepface/extendedmodels/Age.py
+-rw-r--r--   0 sefik      (501) staff       (20)     3216 2024-04-12 13:50:50.000000 deepface-0.0.90/deepface/extendedmodels/Emotion.py
+-rw-r--r--   0 sefik      (501) staff       (20)     2422 2024-04-12 13:50:50.000000 deepface-0.0.90/deepface/extendedmodels/Gender.py
+-rw-r--r--   0 sefik      (501) staff       (20)     2422 2024-04-12 13:50:50.000000 deepface-0.0.90/deepface/extendedmodels/Race.py
+-rw-r--r--   0 sefik      (501) staff       (20)        0 2021-09-07 17:19:21.000000 deepface-0.0.90/deepface/extendedmodels/__init__.py
+drwxr-xr-x   0 sefik      (501) staff       (20)        0 2024-04-16 21:04:24.592789 deepface-0.0.90/deepface/models/
+-rw-r--r--   0 sefik      (501) staff       (20)      577 2024-02-02 20:17:38.000000 deepface-0.0.90/deepface/models/Demography.py
+-rw-r--r--   0 sefik      (501) staff       (20)     2882 2024-03-24 16:59:56.000000 deepface-0.0.90/deepface/models/Detector.py
+-rw-r--r--   0 sefik      (501) staff       (20)     1029 2024-03-31 08:35:42.000000 deepface-0.0.90/deepface/models/FacialRecognition.py
+-rw-r--r--   0 sefik      (501) staff       (20)        0 2024-01-20 12:27:18.000000 deepface-0.0.90/deepface/models/__init__.py
+drwxr-xr-x   0 sefik      (501) staff       (20)        0 2024-04-16 21:04:24.597962 deepface-0.0.90/deepface/modules/
+-rw-r--r--   0 sefik      (501) staff       (20)        0 2024-01-13 23:12:01.000000 deepface-0.0.90/deepface/modules/__init__.py
+-rw-r--r--   0 sefik      (501) staff       (20)     8291 2024-04-12 16:09:50.000000 deepface-0.0.90/deepface/modules/demography.py
+-rw-r--r--   0 sefik      (501) staff       (20)     5820 2024-04-13 07:27:53.000000 deepface-0.0.90/deepface/modules/detection.py
+-rw-r--r--   0 sefik      (501) staff       (20)     1674 2024-03-16 10:00:17.000000 deepface-0.0.90/deepface/modules/modeling.py
+-rw-r--r--   0 sefik      (501) staff       (20)     3517 2024-04-13 07:27:53.000000 deepface-0.0.90/deepface/modules/preprocessing.py
+-rw-r--r--   0 sefik      (501) staff       (20)    14173 2024-04-13 07:27:53.000000 deepface-0.0.90/deepface/modules/recognition.py
+-rw-r--r--   0 sefik      (501) staff       (20)     4619 2024-04-13 07:27:53.000000 deepface-0.0.90/deepface/modules/representation.py
+-rw-r--r--   0 sefik      (501) staff       (20)    31376 2024-04-12 16:09:50.000000 deepface-0.0.90/deepface/modules/streaming.py
+-rw-r--r--   0 sefik      (501) staff       (20)    14303 2024-04-12 16:09:50.000000 deepface-0.0.90/deepface/modules/verification.py
+drwxr-xr-x   0 sefik      (501) staff       (20)        0 2024-04-16 21:04:24.576764 deepface-0.0.90/deepface.egg-info/
+-rw-r--r--   0 sefik      (501) staff       (20)    26049 2024-04-16 21:04:24.000000 deepface-0.0.90/deepface.egg-info/PKG-INFO
+-rw-r--r--   0 sefik      (501) staff       (20)     1995 2024-04-16 21:04:24.000000 deepface-0.0.90/deepface.egg-info/SOURCES.txt
+-rw-r--r--   0 sefik      (501) staff       (20)        1 2024-04-16 21:04:24.000000 deepface-0.0.90/deepface.egg-info/dependency_links.txt
+-rw-r--r--   0 sefik      (501) staff       (20)       51 2024-04-16 21:04:24.000000 deepface-0.0.90/deepface.egg-info/entry_points.txt
+-rw-r--r--   0 sefik      (501) staff       (20)      216 2024-04-16 21:04:24.000000 deepface-0.0.90/deepface.egg-info/requires.txt
+-rw-r--r--   0 sefik      (501) staff       (20)        9 2024-04-16 21:04:24.000000 deepface-0.0.90/deepface.egg-info/top_level.txt
+-rw-r--r--   0 sefik      (501) staff       (20)       27 2024-03-24 16:59:56.000000 deepface-0.0.90/package_info.json
+-rw-r--r--   0 sefik      (501) staff       (20)      230 2024-04-13 07:27:53.000000 deepface-0.0.90/requirements.txt
+-rw-r--r--   0 sefik      (501) staff       (20)       38 2024-04-16 21:04:24.599291 deepface-0.0.90/setup.cfg
+-rw-r--r--   0 sefik      (501) staff       (20)     1201 2024-03-10 09:13:34.000000 deepface-0.0.90/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

