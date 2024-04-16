# Comparing `tmp/retina-face-0.0.8.tar.gz` & `tmp/retina-face-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/retina-face-0.0.8.tar", last modified: Wed Jan 12 07:56:40 2022, max compression
+gzip compressed data, was "dist/retina-face-0.0.9.tar", last modified: Wed Jan 12 10:41:32 2022, max compression
```

## Comparing `retina-face-0.0.8.tar` & `retina-face-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 sefik      (501) staff       (20)        0 2022-01-12 07:56:40.228431 retina-face-0.0.8/
--rw-r--r--   0 sefik      (501) staff       (20)     1077 2021-12-02 08:54:59.000000 retina-face-0.0.8/LICENSE
--rw-r--r--   0 sefik      (501) staff       (20)     8743 2022-01-12 07:56:40.228041 retina-face-0.0.8/PKG-INFO
--rw-r--r--   0 sefik      (501) staff       (20)     7272 2022-01-12 07:51:58.000000 retina-face-0.0.8/README.md
-drwxr-xr-x   0 sefik      (501) staff       (20)        0 2022-01-12 07:56:40.223629 retina-face-0.0.8/retina_face.egg-info/
--rw-r--r--   0 sefik      (501) staff       (20)     8743 2022-01-12 07:56:40.000000 retina-face-0.0.8/retina_face.egg-info/PKG-INFO
--rw-r--r--   0 sefik      (501) staff       (20)      412 2022-01-12 07:56:40.000000 retina-face-0.0.8/retina_face.egg-info/SOURCES.txt
--rw-r--r--   0 sefik      (501) staff       (20)        1 2022-01-12 07:56:40.000000 retina-face-0.0.8/retina_face.egg-info/dependency_links.txt
--rw-r--r--   0 sefik      (501) staff       (20)       81 2022-01-12 07:56:40.000000 retina-face-0.0.8/retina_face.egg-info/requires.txt
--rw-r--r--   0 sefik      (501) staff       (20)       11 2022-01-12 07:56:40.000000 retina-face-0.0.8/retina_face.egg-info/top_level.txt
-drwxr-xr-x   0 sefik      (501) staff       (20)        0 2022-01-12 07:56:40.224876 retina-face-0.0.8/retinaface/
--rw-r--r--   0 sefik      (501) staff       (20)     6824 2021-12-02 08:54:59.000000 retina-face-0.0.8/retinaface/RetinaFace.py
--rw-r--r--   0 sefik      (501) staff       (20)        0 2021-12-02 08:54:59.000000 retina-face-0.0.8/retinaface/__init__.py
-drwxr-xr-x   0 sefik      (501) staff       (20)        0 2022-01-12 07:56:40.226156 retina-face-0.0.8/retinaface/commons/
--rw-r--r--   0 sefik      (501) staff       (20)        0 2021-12-02 08:54:59.000000 retina-face-0.0.8/retinaface/commons/__init__.py
--rw-r--r--   0 sefik      (501) staff       (20)     6746 2021-12-02 08:54:59.000000 retina-face-0.0.8/retinaface/commons/postprocess.py
--rw-r--r--   0 sefik      (501) staff       (20)     1782 2021-12-02 08:54:59.000000 retina-face-0.0.8/retinaface/commons/preprocess.py
-drwxr-xr-x   0 sefik      (501) staff       (20)        0 2022-01-12 07:56:40.226940 retina-face-0.0.8/retinaface/model/
--rw-r--r--   0 sefik      (501) staff       (20)        0 2021-12-02 08:54:59.000000 retina-face-0.0.8/retinaface/model/__init__.py
--rw-r--r--   0 sefik      (501) staff       (20)    40910 2021-12-02 08:54:59.000000 retina-face-0.0.8/retinaface/model/retinaface_model.py
--rw-r--r--   0 sefik      (501) staff       (20)       38 2022-01-12 07:56:40.228562 retina-face-0.0.8/setup.cfg
--rw-r--r--   0 sefik      (501) staff       (20)      853 2022-01-12 07:51:58.000000 retina-face-0.0.8/setup.py
+drwxr-xr-x   0 sefik      (501) staff       (20)        0 2022-01-12 10:41:32.284001 retina-face-0.0.9/
+-rw-r--r--   0 sefik      (501) staff       (20)     1077 2021-12-02 08:54:59.000000 retina-face-0.0.9/LICENSE
+-rw-r--r--   0 sefik      (501) staff       (20)     8795 2022-01-12 10:41:32.283695 retina-face-0.0.9/PKG-INFO
+-rw-r--r--   0 sefik      (501) staff       (20)     7332 2022-01-12 10:38:07.000000 retina-face-0.0.9/README.md
+drwxr-xr-x   0 sefik      (501) staff       (20)        0 2022-01-12 10:41:32.280193 retina-face-0.0.9/retina_face.egg-info/
+-rw-r--r--   0 sefik      (501) staff       (20)     8795 2022-01-12 10:41:32.000000 retina-face-0.0.9/retina_face.egg-info/PKG-INFO
+-rw-r--r--   0 sefik      (501) staff       (20)      412 2022-01-12 10:41:32.000000 retina-face-0.0.9/retina_face.egg-info/SOURCES.txt
+-rw-r--r--   0 sefik      (501) staff       (20)        1 2022-01-12 10:41:32.000000 retina-face-0.0.9/retina_face.egg-info/dependency_links.txt
+-rw-r--r--   0 sefik      (501) staff       (20)       81 2022-01-12 10:41:32.000000 retina-face-0.0.9/retina_face.egg-info/requires.txt
+-rw-r--r--   0 sefik      (501) staff       (20)       11 2022-01-12 10:41:32.000000 retina-face-0.0.9/retina_face.egg-info/top_level.txt
+drwxr-xr-x   0 sefik      (501) staff       (20)        0 2022-01-12 10:41:32.281116 retina-face-0.0.9/retinaface/
+-rw-r--r--   0 sefik      (501) staff       (20)     6824 2021-12-02 08:54:59.000000 retina-face-0.0.9/retinaface/RetinaFace.py
+-rw-r--r--   0 sefik      (501) staff       (20)        0 2021-12-02 08:54:59.000000 retina-face-0.0.9/retinaface/__init__.py
+drwxr-xr-x   0 sefik      (501) staff       (20)        0 2022-01-12 10:41:32.281937 retina-face-0.0.9/retinaface/commons/
+-rw-r--r--   0 sefik      (501) staff       (20)        0 2021-12-02 08:54:59.000000 retina-face-0.0.9/retinaface/commons/__init__.py
+-rw-r--r--   0 sefik      (501) staff       (20)     6746 2021-12-02 08:54:59.000000 retina-face-0.0.9/retinaface/commons/postprocess.py
+-rw-r--r--   0 sefik      (501) staff       (20)     1782 2021-12-02 08:54:59.000000 retina-face-0.0.9/retinaface/commons/preprocess.py
+drwxr-xr-x   0 sefik      (501) staff       (20)        0 2022-01-12 10:41:32.282792 retina-face-0.0.9/retinaface/model/
+-rw-r--r--   0 sefik      (501) staff       (20)        0 2021-12-02 08:54:59.000000 retina-face-0.0.9/retinaface/model/__init__.py
+-rw-r--r--   0 sefik      (501) staff       (20)    40910 2021-12-02 08:54:59.000000 retina-face-0.0.9/retinaface/model/retinaface_model.py
+-rw-r--r--   0 sefik      (501) staff       (20)       38 2022-01-12 10:41:32.284115 retina-face-0.0.9/setup.cfg
+-rw-r--r--   0 sefik      (501) staff       (20)      853 2022-01-12 10:38:07.000000 retina-face-0.0.9/setup.py
```

### Comparing `retina-face-0.0.8/LICENSE` & `retina-face-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `retina-face-0.0.8/PKG-INFO` & `retina-face-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: retina-face
-Version: 0.0.8
+Version: 0.0.9
 Summary: RetinaFace: Deep Face Detection Framework in TensorFlow for Python
 Home-page: https://github.com/serengil/retinaface
 Author: Sefik Ilkin Serengil
 Author-email: serengil@gmail.com
 License: UNKNOWN
 Description: # RetinaFace
         
         [![Downloads](https://pepy.tech/badge/retina-face)](https://pepy.tech/project/retina-face)
         [![Stars](https://img.shields.io/github/stars/serengil/retinaface?color=yellow)](https://github.com/serengil/retinaface)
         [![License](http://img.shields.io/:license-MIT-green.svg?style=flat)](https://github.com/serengil/retinaface/blob/master/LICENSE)
         [![Support me on Patreon](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Fshieldsio-patreon.vercel.app%2Fapi%3Fusername%3Dserengil%26type%3Dpatrons&style=flat)](https://www.patreon.com/bePatron?u=31795557&redirect_uri=https%3A%2F%2Fgithub.com%2Fserengil%2Fretinaface%2F)
-        [![Twitter](https://badgen.net/twitter/follow/serengil?icon=twitter)](https://twitter.com/serengil)
         [![DOI](http://img.shields.io/:DOI-10.1109/ICEET53442.2021.9659697-blue.svg?style=flat)](https://doi.org/10.1109/ICEET53442.2021.9659697)
         
         RetinaFace is a deep learning based cutting-edge facial detector for Python coming with facial landmarks. Its detection performance is amazing even in the crowd as shown in the following illustration.
         
         RetinaFace is the face detection module of [insightface](https://github.com/deepinsight/insightface) project. The original implementation is mainly based on mxnet. Then, its tensorflow based [re-implementation](https://github.com/StanislasBertrand/RetinaFace-tf2) is published by [Stanislas Bertrand](https://github.com/StanislasBertrand). So, this repo is heavily inspired from the study of Stanislas Bertrand. Its source code is simplified and it is transformed to pip compatible but the main structure of the reference model and its pre-trained weights are same.
         
         <p align="center"><img src="https://raw.githubusercontent.com/serengil/retinaface/master/tests/outputs/img3.jpg" width="90%" height="90%"></p>
@@ -91,17 +90,17 @@
         
         Notice that ArcFace got 99.40% accuracy on [LFW data set](https://sefiks.com/2020/08/27/labeled-faces-in-the-wild-for-face-recognition/) whereas human beings just have 97.53% confidence.
         
         ## Support
         
         There are many ways to support a project. Starring⭐️ the repo is just one 🙏
         
-        You can also support this work on [Patreon](https://patreon.com/serengil)
+        You can also support this work on [Patreon](https://www.patreon.com/bePatron?u=31795557&redirect_uri=https%3A%2F%2Fgithub.com%2Fserengil%2Fretinaface%2F)
         
-        <a href="https://patreon.com/serengil">
+        <a href="https://www.patreon.com/bePatron?u=31795557&redirect_uri=https%3A%2F%2Fgithub.com%2Fserengil%2Fretinaface%2F">
         <img src="https://raw.githubusercontent.com/serengil/retinaface/master/icons/patreon.png" width="30%" height="30%">
         </a>
         
         ## Acknowledgements
         
         This work is mainly based on the [insightface](https://github.com/deepinsight/insightface) project and [retinaface](https://arxiv.org/pdf/1905.00641.pdf) paper; and it is heavily inspired from the re-implementation of [retinaface-tf2](https://github.com/StanislasBertrand/RetinaFace-tf2) by [Stanislas Bertrand](https://github.com/StanislasBertrand). Finally, Bertrand's [implemenation](https://github.com/StanislasBertrand/RetinaFace-tf2/blob/master/rcnn/cython/cpu_nms.pyx) uses [Fast R-CNN](https://arxiv.org/abs/1504.08083) written by [Ross Girshick](https://github.com/rbgirshick/fast-rcnn) in the background. All of those reference studies are licensed under MIT license.
```

### Comparing `retina-face-0.0.8/README.md` & `retina-face-0.0.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # RetinaFace
 
 [![Downloads](https://pepy.tech/badge/retina-face)](https://pepy.tech/project/retina-face)
 [![Stars](https://img.shields.io/github/stars/serengil/retinaface?color=yellow)](https://github.com/serengil/retinaface)
 [![License](http://img.shields.io/:license-MIT-green.svg?style=flat)](https://github.com/serengil/retinaface/blob/master/LICENSE)
 [![Support me on Patreon](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Fshieldsio-patreon.vercel.app%2Fapi%3Fusername%3Dserengil%26type%3Dpatrons&style=flat)](https://www.patreon.com/bePatron?u=31795557&redirect_uri=https%3A%2F%2Fgithub.com%2Fserengil%2Fretinaface%2F)
-[![Twitter](https://badgen.net/twitter/follow/serengil?icon=twitter)](https://twitter.com/serengil)
 [![DOI](http://img.shields.io/:DOI-10.1109/ICEET53442.2021.9659697-blue.svg?style=flat)](https://doi.org/10.1109/ICEET53442.2021.9659697)
 
 RetinaFace is a deep learning based cutting-edge facial detector for Python coming with facial landmarks. Its detection performance is amazing even in the crowd as shown in the following illustration.
 
 RetinaFace is the face detection module of [insightface](https://github.com/deepinsight/insightface) project. The original implementation is mainly based on mxnet. Then, its tensorflow based [re-implementation](https://github.com/StanislasBertrand/RetinaFace-tf2) is published by [Stanislas Bertrand](https://github.com/StanislasBertrand). So, this repo is heavily inspired from the study of Stanislas Bertrand. Its source code is simplified and it is transformed to pip compatible but the main structure of the reference model and its pre-trained weights are same.
 
 <p align="center"><img src="https://raw.githubusercontent.com/serengil/retinaface/master/tests/outputs/img3.jpg" width="90%" height="90%"></p>
@@ -83,17 +82,17 @@
 
 Notice that ArcFace got 99.40% accuracy on [LFW data set](https://sefiks.com/2020/08/27/labeled-faces-in-the-wild-for-face-recognition/) whereas human beings just have 97.53% confidence.
 
 ## Support
 
 There are many ways to support a project. Starring⭐️ the repo is just one 🙏
 
-You can also support this work on [Patreon](https://patreon.com/serengil)
+You can also support this work on [Patreon](https://www.patreon.com/bePatron?u=31795557&redirect_uri=https%3A%2F%2Fgithub.com%2Fserengil%2Fretinaface%2F)
 
-<a href="https://patreon.com/serengil">
+<a href="https://www.patreon.com/bePatron?u=31795557&redirect_uri=https%3A%2F%2Fgithub.com%2Fserengil%2Fretinaface%2F">
 <img src="https://raw.githubusercontent.com/serengil/retinaface/master/icons/patreon.png" width="30%" height="30%">
 </a>
 
 ## Acknowledgements
 
 This work is mainly based on the [insightface](https://github.com/deepinsight/insightface) project and [retinaface](https://arxiv.org/pdf/1905.00641.pdf) paper; and it is heavily inspired from the re-implementation of [retinaface-tf2](https://github.com/StanislasBertrand/RetinaFace-tf2) by [Stanislas Bertrand](https://github.com/StanislasBertrand). Finally, Bertrand's [implemenation](https://github.com/StanislasBertrand/RetinaFace-tf2/blob/master/rcnn/cython/cpu_nms.pyx) uses [Fast R-CNN](https://arxiv.org/abs/1504.08083) written by [Ross Girshick](https://github.com/rbgirshick/fast-rcnn) in the background. All of those reference studies are licensed under MIT license.
```

### Comparing `retina-face-0.0.8/retina_face.egg-info/PKG-INFO` & `retina-face-0.0.9/retina_face.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: retina-face
-Version: 0.0.8
+Version: 0.0.9
 Summary: RetinaFace: Deep Face Detection Framework in TensorFlow for Python
 Home-page: https://github.com/serengil/retinaface
 Author: Sefik Ilkin Serengil
 Author-email: serengil@gmail.com
 License: UNKNOWN
 Description: # RetinaFace
         
         [![Downloads](https://pepy.tech/badge/retina-face)](https://pepy.tech/project/retina-face)
         [![Stars](https://img.shields.io/github/stars/serengil/retinaface?color=yellow)](https://github.com/serengil/retinaface)
         [![License](http://img.shields.io/:license-MIT-green.svg?style=flat)](https://github.com/serengil/retinaface/blob/master/LICENSE)
         [![Support me on Patreon](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Fshieldsio-patreon.vercel.app%2Fapi%3Fusername%3Dserengil%26type%3Dpatrons&style=flat)](https://www.patreon.com/bePatron?u=31795557&redirect_uri=https%3A%2F%2Fgithub.com%2Fserengil%2Fretinaface%2F)
-        [![Twitter](https://badgen.net/twitter/follow/serengil?icon=twitter)](https://twitter.com/serengil)
         [![DOI](http://img.shields.io/:DOI-10.1109/ICEET53442.2021.9659697-blue.svg?style=flat)](https://doi.org/10.1109/ICEET53442.2021.9659697)
         
         RetinaFace is a deep learning based cutting-edge facial detector for Python coming with facial landmarks. Its detection performance is amazing even in the crowd as shown in the following illustration.
         
         RetinaFace is the face detection module of [insightface](https://github.com/deepinsight/insightface) project. The original implementation is mainly based on mxnet. Then, its tensorflow based [re-implementation](https://github.com/StanislasBertrand/RetinaFace-tf2) is published by [Stanislas Bertrand](https://github.com/StanislasBertrand). So, this repo is heavily inspired from the study of Stanislas Bertrand. Its source code is simplified and it is transformed to pip compatible but the main structure of the reference model and its pre-trained weights are same.
         
         <p align="center"><img src="https://raw.githubusercontent.com/serengil/retinaface/master/tests/outputs/img3.jpg" width="90%" height="90%"></p>
@@ -91,17 +90,17 @@
         
         Notice that ArcFace got 99.40% accuracy on [LFW data set](https://sefiks.com/2020/08/27/labeled-faces-in-the-wild-for-face-recognition/) whereas human beings just have 97.53% confidence.
         
         ## Support
         
         There are many ways to support a project. Starring⭐️ the repo is just one 🙏
         
-        You can also support this work on [Patreon](https://patreon.com/serengil)
+        You can also support this work on [Patreon](https://www.patreon.com/bePatron?u=31795557&redirect_uri=https%3A%2F%2Fgithub.com%2Fserengil%2Fretinaface%2F)
         
-        <a href="https://patreon.com/serengil">
+        <a href="https://www.patreon.com/bePatron?u=31795557&redirect_uri=https%3A%2F%2Fgithub.com%2Fserengil%2Fretinaface%2F">
         <img src="https://raw.githubusercontent.com/serengil/retinaface/master/icons/patreon.png" width="30%" height="30%">
         </a>
         
         ## Acknowledgements
         
         This work is mainly based on the [insightface](https://github.com/deepinsight/insightface) project and [retinaface](https://arxiv.org/pdf/1905.00641.pdf) paper; and it is heavily inspired from the re-implementation of [retinaface-tf2](https://github.com/StanislasBertrand/RetinaFace-tf2) by [Stanislas Bertrand](https://github.com/StanislasBertrand). Finally, Bertrand's [implemenation](https://github.com/StanislasBertrand/RetinaFace-tf2/blob/master/rcnn/cython/cpu_nms.pyx) uses [Fast R-CNN](https://arxiv.org/abs/1504.08083) written by [Ross Girshick](https://github.com/rbgirshick/fast-rcnn) in the background. All of those reference studies are licensed under MIT license.
```

### Comparing `retina-face-0.0.8/retinaface/RetinaFace.py` & `retina-face-0.0.9/retinaface/RetinaFace.py`

 * *Files identical despite different names*

### Comparing `retina-face-0.0.8/retinaface/commons/postprocess.py` & `retina-face-0.0.9/retinaface/commons/postprocess.py`

 * *Files identical despite different names*

### Comparing `retina-face-0.0.8/retinaface/commons/preprocess.py` & `retina-face-0.0.9/retinaface/commons/preprocess.py`

 * *Files identical despite different names*

### Comparing `retina-face-0.0.8/retinaface/model/retinaface_model.py` & `retina-face-0.0.9/retinaface/model/retinaface_model.py`

 * *Files identical despite different names*

### Comparing `retina-face-0.0.8/setup.py` & `retina-face-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="retina-face", #pip install retina-face
-    version="0.0.8",
+    version="0.0.9",
     author="Sefik Ilkin Serengil",
     author_email="serengil@gmail.com",
     description="RetinaFace: Deep Face Detection Framework in TensorFlow for Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/serengil/retinaface",
     packages=setuptools.find_packages(),
```

