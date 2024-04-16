# Comparing `tmp/eyepop-0.15.3.tar.gz` & `tmp/eyepop-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eyepop-0.15.3.tar", last modified: Tue Apr 16 00:49:09 2024, max compression
+gzip compressed data, was "eyepop-0.9.2.tar", last modified: Mon Jan 15 21:11:17 2024, max compression
```

## Comparing `eyepop-0.15.3.tar` & `eyepop-0.9.2.tar`

### file list

```diff
@@ -1,46 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 00:49:09.690672 eyepop-0.15.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 00:49:09.682672 eyepop-0.15.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 00:49:09.682672 eyepop-0.15.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-16 00:48:59.000000 eyepop-0.15.3/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-04-16 00:48:59.000000 eyepop-0.15.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-16 00:48:59.000000 eyepop-0.15.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10850 2024-04-16 00:49:09.690672 eyepop-0.15.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8365 2024-04-16 00:48:59.000000 eyepop-0.15.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 00:49:09.686672 eyepop-0.15.3/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-16 00:48:59.000000 eyepop-0.15.3/examples/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 00:48:59.000000 eyepop-0.15.3/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   109060 2024-04-16 00:48:59.000000 eyepop-0.15.3/examples/example.jpg
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-16 00:48:59.000000 eyepop-0.15.3/examples/live_rtmp_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-16 00:48:59.000000 eyepop-0.15.3/examples/load_video_from_http.py
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-04-16 00:48:59.000000 eyepop-0.15.3/examples/upload_image_timing.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-16 00:48:59.000000 eyepop-0.15.3/examples/upload_video.py
--rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-04-16 00:48:59.000000 eyepop-0.15.3/examples/viewer.html
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-16 00:48:59.000000 eyepop-0.15.3/examples/visualize_on_image.py
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-16 00:48:59.000000 eyepop-0.15.3/examples/visualize_with_webui2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 00:49:09.686672 eyepop-0.15.3/eyepop/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-16 00:48:59.000000 eyepop-0.15.3/eyepop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23747 2024-04-16 00:48:59.000000 eyepop-0.15.3/eyepop/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-16 00:48:59.000000 eyepop-0.15.3/eyepop/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-16 00:48:59.000000 eyepop-0.15.3/eyepop/eyepopsdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     9394 2024-04-16 00:48:59.000000 eyepop-0.15.3/eyepop/jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-04-16 00:48:59.000000 eyepop-0.15.3/eyepop/syncify.py
--rw-r--r--   0 runner    (1001) docker     (127)     4787 2024-04-16 00:48:59.000000 eyepop-0.15.3/eyepop/visualize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 00:49:09.690672 eyepop-0.15.3/eyepop.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10850 2024-04-16 00:49:09.000000 eyepop-0.15.3/eyepop.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-16 00:49:09.000000 eyepop-0.15.3/eyepop.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 00:49:09.000000 eyepop-0.15.3/eyepop.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-16 00:49:09.000000 eyepop-0.15.3/eyepop.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-16 00:49:09.000000 eyepop-0.15.3/eyepop.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-16 00:48:59.000000 eyepop-0.15.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 00:49:09.690672 eyepop-0.15.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 00:49:09.690672 eyepop-0.15.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 00:48:59.000000 eyepop-0.15.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4872 2024-04-16 00:48:59.000000 eyepop-0.15.3/tests/base_endpoint_test.py
--rw-r--r--   0 runner    (1001) docker     (127)   109060 2024-04-16 00:48:59.000000 eyepop-0.15.3/tests/test.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     7322 2024-04-16 00:48:59.000000 eyepop-0.15.3/tests/test_endpoint_connect.py
--rw-r--r--   0 runner    (1001) docker     (127)     6010 2024-04-16 00:48:59.000000 eyepop-0.15.3/tests/test_endpoint_load.py
--rw-r--r--   0 runner    (1001) docker     (127)     6455 2024-04-16 00:48:59.000000 eyepop-0.15.3/tests/test_endpoint_pop_comp.py
--rw-r--r--   0 runner    (1001) docker     (127)     5618 2024-04-16 00:48:59.000000 eyepop-0.15.3/tests/test_endpoint_retry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-04-16 00:48:59.000000 eyepop-0.15.3/tests/test_endpoint_sandbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     5611 2024-04-16 00:48:59.000000 eyepop-0.15.3/tests/test_endpoint_upload.py
--rw-r--r--   0 runner    (1001) docker     (127)     5690 2024-04-16 00:48:59.000000 eyepop-0.15.3/tests/test_endpoint_upload_stream.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 21:11:17.175971 eyepop-0.9.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 21:11:17.171971 eyepop-0.9.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 21:11:17.171971 eyepop-0.9.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-01-15 21:11:06.000000 eyepop-0.9.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-01-15 21:11:06.000000 eyepop-0.9.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-01-15 21:11:06.000000 eyepop-0.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9925 2024-01-15 21:11:17.175971 eyepop-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7591 2024-01-15 21:11:06.000000 eyepop-0.9.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 21:11:17.171971 eyepop-0.9.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-15 21:11:06.000000 eyepop-0.9.2/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   109060 2024-01-15 21:11:06.000000 eyepop-0.9.2/examples/example.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-01-15 21:11:06.000000 eyepop-0.9.2/examples/live_rtmp_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-01-15 21:11:06.000000 eyepop-0.9.2/examples/load_video_from_http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-01-15 21:11:06.000000 eyepop-0.9.2/examples/upload_image_timing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-01-15 21:11:06.000000 eyepop-0.9.2/examples/visualize_on_image.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 21:11:17.175971 eyepop-0.9.2/eyepop/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-01-15 21:11:06.000000 eyepop-0.9.2/eyepop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11201 2024-01-15 21:11:06.000000 eyepop-0.9.2/eyepop/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-01-15 21:11:06.000000 eyepop-0.9.2/eyepop/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-01-15 21:11:06.000000 eyepop-0.9.2/eyepop/eyepopsdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5938 2024-01-15 21:11:06.000000 eyepop-0.9.2/eyepop/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-01-15 21:11:06.000000 eyepop-0.9.2/eyepop/syncify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4787 2024-01-15 21:11:06.000000 eyepop-0.9.2/eyepop/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 21:11:17.175971 eyepop-0.9.2/eyepop.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9925 2024-01-15 21:11:17.000000 eyepop-0.9.2/eyepop.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-01-15 21:11:17.000000 eyepop-0.9.2/eyepop.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-15 21:11:17.000000 eyepop-0.9.2/eyepop.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-01-15 21:11:17.000000 eyepop-0.9.2/eyepop.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-15 21:11:17.000000 eyepop-0.9.2/eyepop.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-01-15 21:11:06.000000 eyepop-0.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-15 21:11:17.175971 eyepop-0.9.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 21:11:17.175971 eyepop-0.9.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-15 21:11:06.000000 eyepop-0.9.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-01-15 21:11:06.000000 eyepop-0.9.2/tests/base_endpoint_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)   109060 2024-01-15 21:11:06.000000 eyepop-0.9.2/tests/test.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-01-15 21:11:06.000000 eyepop-0.9.2/tests/test_endpoint_connect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4727 2024-01-15 21:11:06.000000 eyepop-0.9.2/tests/test_endpoint_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4561 2024-01-15 21:11:06.000000 eyepop-0.9.2/tests/test_endpoint_upload.py
```

### Comparing `eyepop-0.15.3/.github/workflows/python-publish.yml` & `eyepop-0.9.2/.github/workflows/python-publish.yml`

 * *Files 6% similar despite different names*

```diff
@@ -28,16 +28,12 @@
         python-version: '3.x'
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install build
     - name: Build package
       run: python -m build
-    - name: Test package
-      run: |
-        pip install -e .[test]
-        python -m pytest
     - name: Publish package
       uses: pypa/gh-action-pypi-publish@27b31702a0e7fc50959f5ad993c78deac1bdfc29
       with:
         user: __token__
         password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `eyepop-0.15.3/.gitignore` & `eyepop-0.9.2/.gitignore`

 * *Files identical despite different names*

### Comparing `eyepop-0.15.3/LICENSE` & `eyepop-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `eyepop-0.15.3/PKG-INFO` & `eyepop-0.9.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eyepop
-Version: 0.15.3
+Version: 0.9.2
 Summary: EyePop.ai Python SDK
 Author-email: "EyePop.ai" <support@eyepop.ai>
 License: MIT License
         
         Copyright (c) 2023 EyePop.ai
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -43,18 +43,14 @@
 Requires-Dist: aioresponses; extra == "test"
 Provides-Extra: doc
 Requires-Dist: mkdocs; extra == "doc"
 Requires-Dist: mkdocstrings; extra == "doc"
 Requires-Dist: mkdocstrings[python]; extra == "doc"
 Requires-Dist: mkdocs-material; extra == "doc"
 Requires-Dist: Pygments; extra == "doc"
-Provides-Extra: example
-Requires-Dist: pyqt5; extra == "example"
-Requires-Dist: webui2; extra == "example"
-Requires-Dist: pybars3; extra == "example"
 Provides-Extra: all
 Requires-Dist: eyepop[doc,test]; extra == "all"
 
 # EyePop.ai Python SDK
 The EyePop.ai Python SDK provides convenient access to the EyePop.ai's inference API from applications written in the 
 Python language. 
 
@@ -107,49 +103,31 @@
 the context and releasing all underlying resources upon exiting the context. Alternatively your code can call 
 endpoint.connect() before any job is submitted and endpoint.disconnect() to release all resources.
 2. `endpoint.upload('examples/example.jpg')` initiates the upload to the local file to the worker service. The image will
 be queued and processed immediately when the worker becomes available.
 3. `predict()` waits for the first prediction result as reports it as a dict. In case of a single image, there will be 
 one single prediction result and subsequent calls to predict() will return None. If the uploaded file is a video
 e.g. 'video/mp4' or image container format e.g. 'image/gif', subsequent calls to predict() will return a prediction 
-for each individual frame and None when the entire file has been processed.
-
-To upload a binary stream, i.e. a file-like object, you can use the method `upload_stream()` and pass the file-like 
-object and the mime-type:
-```python
-from eyepop import EyePopSdk
-
-def upload_photo_from_stream(file_path: str, mime_type: str):
-    with EyePopSdk.endpoint() as endpoint:
-        with open(file_path, 'rb') as file:
-            result = endpoint.upload_stream(file, mime_type).predict()
-            print(result)
-
-upload_photo_from_stream('examples/example.jpg', 'image/jpeg')
-```
-
+for each individual frame and None when the entire file has been processed. 
 ### Visualizing Results
-The EyePop SDK includes helper classes to to visualize bounding boxes `matplotlib.pyplot`.
+The EyePop SDK includes helper classes to visualize the predictions for images using `matplotlib.pyplot`.
 ```python
 from PIL import Image
 import matplotlib.pyplot as plt
 from eyepop import EyePopSdk
 
 with EyePopSdk.endpoint() as endpoint:
     result = endpoint.upload('examples/example.jpg').predict()
 with Image.open('examples/example.jpg') as image:
     plt.imshow(image)
 plot = EyePopSdk.plot(plt.gca())
 plot.prediction(result)    
 plt.show()
 ```
-Depending on the environment, you might need to install an interactive backend, e.g. with `pip3 install pyqt5`. 
-EyePop's Python Sdk does not include visualization helpers for any other prediction types than object bounding boxes.
-Check out [visualize_with_webui2.py](examples/visualize_with_webui2.py) for an example how to use the comprehensive visualization support provided by the EyePop Node Sdk.
-
+Depending on the environment, you might need to install an interactive backend, e.g. with `pip3 install pyqt5`.
 ### Uploading and processing batches of images
 For batches of images, instead of waiting for each result `predict()` _before_ submitting the next job, you can queue 
 all jobs first, let them process in parallel and collect the results later. This avoids the sequential accumulation of 
 the HTTP roundtrip time.
 
 ```python
 from eyepop import EyePopSdk
```

### Comparing `eyepop-0.15.3/README.md` & `eyepop-0.9.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -51,49 +51,31 @@
 the context and releasing all underlying resources upon exiting the context. Alternatively your code can call 
 endpoint.connect() before any job is submitted and endpoint.disconnect() to release all resources.
 2. `endpoint.upload('examples/example.jpg')` initiates the upload to the local file to the worker service. The image will
 be queued and processed immediately when the worker becomes available.
 3. `predict()` waits for the first prediction result as reports it as a dict. In case of a single image, there will be 
 one single prediction result and subsequent calls to predict() will return None. If the uploaded file is a video
 e.g. 'video/mp4' or image container format e.g. 'image/gif', subsequent calls to predict() will return a prediction 
-for each individual frame and None when the entire file has been processed.
-
-To upload a binary stream, i.e. a file-like object, you can use the method `upload_stream()` and pass the file-like 
-object and the mime-type:
-```python
-from eyepop import EyePopSdk
-
-def upload_photo_from_stream(file_path: str, mime_type: str):
-    with EyePopSdk.endpoint() as endpoint:
-        with open(file_path, 'rb') as file:
-            result = endpoint.upload_stream(file, mime_type).predict()
-            print(result)
-
-upload_photo_from_stream('examples/example.jpg', 'image/jpeg')
-```
-
+for each individual frame and None when the entire file has been processed. 
 ### Visualizing Results
-The EyePop SDK includes helper classes to to visualize bounding boxes `matplotlib.pyplot`.
+The EyePop SDK includes helper classes to visualize the predictions for images using `matplotlib.pyplot`.
 ```python
 from PIL import Image
 import matplotlib.pyplot as plt
 from eyepop import EyePopSdk
 
 with EyePopSdk.endpoint() as endpoint:
     result = endpoint.upload('examples/example.jpg').predict()
 with Image.open('examples/example.jpg') as image:
     plt.imshow(image)
 plot = EyePopSdk.plot(plt.gca())
 plot.prediction(result)    
 plt.show()
 ```
-Depending on the environment, you might need to install an interactive backend, e.g. with `pip3 install pyqt5`. 
-EyePop's Python Sdk does not include visualization helpers for any other prediction types than object bounding boxes.
-Check out [visualize_with_webui2.py](examples/visualize_with_webui2.py) for an example how to use the comprehensive visualization support provided by the EyePop Node Sdk.
-
+Depending on the environment, you might need to install an interactive backend, e.g. with `pip3 install pyqt5`.
 ### Uploading and processing batches of images
 For batches of images, instead of waiting for each result `predict()` _before_ submitting the next job, you can queue 
 all jobs first, let them process in parallel and collect the results later. This avoids the sequential accumulation of 
 the HTTP roundtrip time.
 
 ```python
 from eyepop import EyePopSdk
```

### Comparing `eyepop-0.15.3/examples/example.jpg` & `eyepop-0.9.2/examples/example.jpg`

 * *Files identical despite different names*

### Comparing `eyepop-0.15.3/examples/live_rtmp_stream.py` & `eyepop-0.9.2/examples/live_rtmp_stream.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 
 logging.basicConfig(level=logging.INFO)
 logging.getLogger('eyepop').setLevel(level=logging.DEBUG)
 
 
 async def async_load_from_rtmp(url: str):
     async def on_ready(job: Job):
-        print('async_load_from_rtmp on_ready')
-        while result := await job.predict():
+        print('on_ready', job.job_type, job.location)
+        while result := job.predict():
             print(result)
 
     async with EyePopSdk.endpoint(is_async=True) as endpoint:
         await endpoint.load_from(url, on_ready)
 
 
 t1 = time.time()
```

### Comparing `eyepop-0.15.3/examples/load_video_from_http.py` & `eyepop-0.9.2/examples/load_video_from_http.py`

 * *Files identical despite different names*

### Comparing `eyepop-0.15.3/examples/upload_image_timing.py` & `eyepop-0.9.2/examples/upload_image_timing.py`

 * *Files identical despite different names*

### Comparing `eyepop-0.15.3/examples/visualize_on_image.py` & `eyepop-0.9.2/examples/visualize_on_image.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 import logging
 import sys
 from PIL import Image
-import json
 
 import matplotlib.pyplot as plt
 
 from eyepop import EyePopSdk
 
 logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(name)s - %(levelname)s - %(message)s')
 logging.getLogger('eyepop.requests').setLevel(level=logging.DEBUG)
 
 example_image_path = sys.argv[1]
 
 with EyePopSdk.endpoint() as endpoint:
     result = endpoint.upload(example_image_path).predict()
-    print(json.dumps(result))
 with Image.open(example_image_path) as image:
     plt.imshow(image)
 plot = EyePopSdk.plot(plt.gca())
 plot.prediction(result)
 plt.show()
```

### Comparing `eyepop-0.15.3/eyepop/eyepopsdk.py` & `eyepop-0.9.2/eyepop/eyepopsdk.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 class EyePopSdk:
     """
     EyePop.ai Python SDK
     """
     @staticmethod
     def endpoint(pop_id: str | None = None, secret_key: str | None = None, auto_start: bool = True,
                  stop_jobs: bool = True, eyepop_url: str | None = None, job_queue_length: int = 1024,
-                 is_async: bool = False, is_sandbox: bool = False) -> Endpoint | SyncEndpoint:
+                 is_async: bool = False) -> Endpoint | SyncEndpoint:
         if secret_key is None:
             secret_key = os.getenv('EYEPOP_SECRET_KEY')
             if secret_key is None:
                 raise Exception('parameter \'secret_key\' or environment \'EYEPOP_SECRET_KEY\' is required')
 
         if eyepop_url is None:
             eyepop_url = os.getenv('EYEPOP_URL')
@@ -27,15 +27,15 @@
 
         if pop_id is None:
             pop_id = os.getenv('EYEPOP_POP_ID')
             if pop_id is None:
                 raise Exception('parameter \'pop_id\' is required')
 
         endpoint = Endpoint(secret_key=secret_key, pop_id=pop_id, auto_start=auto_start, stop_jobs=stop_jobs,
-                            eyepop_url=eyepop_url, job_queue_length=job_queue_length, is_sandbox=is_sandbox)
+                            eyepop_url=eyepop_url, job_queue_length=job_queue_length)
 
         if not is_async:
             endpoint = SyncEndpoint(endpoint)
 
         return endpoint
 
     @staticmethod
```

### Comparing `eyepop-0.15.3/eyepop/visualize.py` & `eyepop-0.9.2/eyepop/visualize.py`

 * *Files identical despite different names*

### Comparing `eyepop-0.15.3/eyepop.egg-info/PKG-INFO` & `eyepop-0.9.2/eyepop.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eyepop
-Version: 0.15.3
+Version: 0.9.2
 Summary: EyePop.ai Python SDK
 Author-email: "EyePop.ai" <support@eyepop.ai>
 License: MIT License
         
         Copyright (c) 2023 EyePop.ai
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -43,18 +43,14 @@
 Requires-Dist: aioresponses; extra == "test"
 Provides-Extra: doc
 Requires-Dist: mkdocs; extra == "doc"
 Requires-Dist: mkdocstrings; extra == "doc"
 Requires-Dist: mkdocstrings[python]; extra == "doc"
 Requires-Dist: mkdocs-material; extra == "doc"
 Requires-Dist: Pygments; extra == "doc"
-Provides-Extra: example
-Requires-Dist: pyqt5; extra == "example"
-Requires-Dist: webui2; extra == "example"
-Requires-Dist: pybars3; extra == "example"
 Provides-Extra: all
 Requires-Dist: eyepop[doc,test]; extra == "all"
 
 # EyePop.ai Python SDK
 The EyePop.ai Python SDK provides convenient access to the EyePop.ai's inference API from applications written in the 
 Python language. 
 
@@ -107,49 +103,31 @@
 the context and releasing all underlying resources upon exiting the context. Alternatively your code can call 
 endpoint.connect() before any job is submitted and endpoint.disconnect() to release all resources.
 2. `endpoint.upload('examples/example.jpg')` initiates the upload to the local file to the worker service. The image will
 be queued and processed immediately when the worker becomes available.
 3. `predict()` waits for the first prediction result as reports it as a dict. In case of a single image, there will be 
 one single prediction result and subsequent calls to predict() will return None. If the uploaded file is a video
 e.g. 'video/mp4' or image container format e.g. 'image/gif', subsequent calls to predict() will return a prediction 
-for each individual frame and None when the entire file has been processed.
-
-To upload a binary stream, i.e. a file-like object, you can use the method `upload_stream()` and pass the file-like 
-object and the mime-type:
-```python
-from eyepop import EyePopSdk
-
-def upload_photo_from_stream(file_path: str, mime_type: str):
-    with EyePopSdk.endpoint() as endpoint:
-        with open(file_path, 'rb') as file:
-            result = endpoint.upload_stream(file, mime_type).predict()
-            print(result)
-
-upload_photo_from_stream('examples/example.jpg', 'image/jpeg')
-```
-
+for each individual frame and None when the entire file has been processed. 
 ### Visualizing Results
-The EyePop SDK includes helper classes to to visualize bounding boxes `matplotlib.pyplot`.
+The EyePop SDK includes helper classes to visualize the predictions for images using `matplotlib.pyplot`.
 ```python
 from PIL import Image
 import matplotlib.pyplot as plt
 from eyepop import EyePopSdk
 
 with EyePopSdk.endpoint() as endpoint:
     result = endpoint.upload('examples/example.jpg').predict()
 with Image.open('examples/example.jpg') as image:
     plt.imshow(image)
 plot = EyePopSdk.plot(plt.gca())
 plot.prediction(result)    
 plt.show()
 ```
-Depending on the environment, you might need to install an interactive backend, e.g. with `pip3 install pyqt5`. 
-EyePop's Python Sdk does not include visualization helpers for any other prediction types than object bounding boxes.
-Check out [visualize_with_webui2.py](examples/visualize_with_webui2.py) for an example how to use the comprehensive visualization support provided by the EyePop Node Sdk.
-
+Depending on the environment, you might need to install an interactive backend, e.g. with `pip3 install pyqt5`.
 ### Uploading and processing batches of images
 For batches of images, instead of waiting for each result `predict()` _before_ submitting the next job, you can queue 
 all jobs first, let them process in parallel and collect the results later. This avoids the sequential accumulation of 
 the HTTP roundtrip time.
 
 ```python
 from eyepop import EyePopSdk
```

### Comparing `eyepop-0.15.3/pyproject.toml` & `eyepop-0.9.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     "wheel",
     "importlib"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "eyepop"
-version = "0.15.3"
+version = "0.9.2"
 description="EyePop.ai Python SDK"
 readme = "README.md"
 license.file = "./LICENSE"
 authors = [
 { name = "EyePop.ai", email = "support@eyepop.ai" },
 ]
 keywords=["EyePop", "AI", "ML", "CV"]
@@ -42,23 +42,18 @@
 doc = [
     "mkdocs",
     "mkdocstrings",
     "mkdocstrings[python]",
     "mkdocs-material",
     "Pygments",
 ]
-example = [
-    "pyqt5",
-    "webui2",
-    "pybars3"
-]
 all = ["eyepop[test,doc]"]
 
 [tool.pytest.ini_options]
 addopts = [
     "--import-mode=importlib",
 ]
 testpaths = [
     "tests",
 ]
 [tool.coverage.run]
-source = ["eyepop"]
+source = ["eyepop"]
```

### Comparing `eyepop-0.15.3/tests/base_endpoint_test.py` & `eyepop-0.9.2/tests/test_endpoint_load.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,98 +1,92 @@
 import json
-import os
-import unittest
+import time
+import aiohttp
+import pytest
 from aioresponses import aioresponses, CallbackResult
 
+from eyepop import EyePopSdk
+from tests.base_endpoint_test import BaseEndpointTest
 
-class BaseEndpointTest(unittest.IsolatedAsyncioTestCase):
 
-    test_eyepop_url = 'http://example.test'
-    test_eyepop_pop_id = 'test_pop_id'
-    test_eyepop_secret_key = 'test secret key'
-    test_expired_access_token = '... expired ...'
-    test_access_token = '... an access token ...'
-    test_worker_url = f'http://example-worker.test'
-    test_pipeline_id = 'test_pipeline_id'
-    test_pop_comp = "test_pop_comp"
-    
-    env_var = ['EYEPOP_SECRET_KEY', 'EYEPOP_POP_ID', 'EYEPOP_URL']
-    for var in env_var:
-        if var in os.environ:
-            del os.environ[var]
-
-    def setup_base_mock(self, mock: aioresponses, sandbox_id: str | None = None):
-        mock.clear()
-        def transient_config(url, **kwargs) -> CallbackResult:
-            if kwargs['headers']['Authorization'] == f'Bearer {self.test_access_token}':
-                return CallbackResult(status=200,
-                                      body=json.dumps(
-                                          {'base_url': self.test_worker_url}))
-            else:
-                return CallbackResult(status=401, reason='test auth token expired')
-
-        def config(url, **kwargs) -> CallbackResult:
-            if kwargs['headers']['Authorization'] == f'Bearer {self.test_access_token}':
-                return CallbackResult(status=200,
-                                      body=json.dumps(
-                                          {'base_url': self.test_worker_url, 'pipeline_id': self.test_pipeline_id}))
-            else:
-                return CallbackResult(status=401, reason='test auth token expired')
-
-        def start(url, **kwargs) -> CallbackResult:
-            if kwargs['headers']['Authorization'] == f'Bearer {self.test_access_token}':
-                return CallbackResult(status=200,
-                                      body=json.dumps({'id': self.test_pipeline_id}))
-            else:
-                return CallbackResult(status=401, reason='test auth token expired')
-
-        def stop(url, **kwargs) -> CallbackResult:
-            if kwargs['headers']['Authorization'] == f'Bearer {self.test_access_token}':
-                return CallbackResult(status=204)
-            else:
-                return CallbackResult(status=401, reason='test auth token expired')
-
-        mock.get(f'{self.test_eyepop_url}/workers/config', callback=transient_config,
-                 repeat=True)
-        mock.get(f'{self.test_eyepop_url}/pops/{self.test_eyepop_pop_id}/config?auto_start=True', callback=config,
-                 repeat=True)
-        if sandbox_id is None:
-            mock.post(f'{self.test_worker_url}/pipelines', callback=start, repeat=False)
-        else:
-            mock.post(f'{self.test_worker_url}/pipelines?sandboxId={sandbox_id}', callback=start, repeat=False)
-
-        mock.patch(f'{self.test_worker_url}/pipelines/{self.test_pipeline_id}/source?mode=preempt&processing=sync',
-                   callback=stop, repeat=False)
-
-    def assertBaseMock(self, mock: aioresponses, is_transient: bool = False, sandbox_id: str | None = None):
-        mock.assert_called_with(f'{self.test_eyepop_url}/authentication/token', method='POST',
-                                json={'secret_key': self.test_eyepop_secret_key})
-        if is_transient:
-            mock.assert_called_with(f'{self.test_eyepop_url}/workers/config',
-                                    method='GET',
-                                    headers={'Authorization': f'Bearer {self.test_access_token}'})
-            if sandbox_id is None:
-                start_url = f'{self.test_worker_url}/pipelines'
-            else:
-                start_url = f'{self.test_worker_url}/pipelines?sandboxId={sandbox_id}'
+class TestEndpointLoadFrom(BaseEndpointTest):
+    test_source_id = 'test_source_id'
+    test_url = 'http://examle-media.test/test.png'
+
+    @aioresponses()
+    def test_sync_load_ok(self, mock: aioresponses):
+        self.setup_base_mock(mock)
+        mock.post(f'{self.test_eyepop_url}/authentication/token', status=200, body=json.dumps(
+            {'expires_in': 1000 * 1000, 'token_type': 'Bearer', 'access_token': self.test_access_token}))
+
+        with EyePopSdk.endpoint(eyepop_url=self.test_eyepop_url, secret_key=self.test_eyepop_secret_key,
+                                pop_id=self.test_eyepop_pop_id) as endpoint:
+            self.assertBaseMock(mock)
+            test_timestamp = time.time() * 1000 * 1000 * 1000
+
+            def loadFrom(url, **kwargs) -> CallbackResult:
+                nonlocal test_timestamp
+                if kwargs['headers']['Authorization'] == f'Bearer {self.test_access_token}':
+                    return CallbackResult(status=200,
+                                          body=json.dumps(
+                                              {'source_id': self.test_source_id, 'seconds': 0,
+                                               'system_timestamp': test_timestamp}))
+                else:
+                    return CallbackResult(status=401, reason='test auth token expired')
+
+            mock.patch(f'{self.test_worker_url}/pipelines/{self.test_pipeline_id}/source?mode=queue&processing=sync',
+                       callback=loadFrom)
+
+            job = endpoint.load_from(self.test_url)
+            result = job.predict()
+            self.assertIsNotNone(result)
+            self.assertEqual(result['source_id'], self.test_source_id)
+            self.assertEqual(result['seconds'], 0)
+            self.assertEqual(result['system_timestamp'], test_timestamp)
+            self.assertIsNone(job.predict())
+
             mock.assert_called_with(
-                start_url,
-                method='POST', headers={'Authorization': f'Bearer {self.test_access_token}'}, data=None,
-                json={
-                'inferPipelineDef': {
-                    'pipeline': 'identity'
-                },
-                "source": {
-                    "sourceType": "NONE",
-                },
-                "idleTimeoutSeconds": 60,
-                "logging": ["out_meta"],
-                "videoOutput": "no_output"
-            })
-        else:
-            mock.assert_called_with(f'{self.test_eyepop_url}/pops/{self.test_eyepop_pop_id}/config?auto_start=True',
-                                    method='GET',
-                                    headers={'Authorization': f'Bearer {self.test_access_token}'})
+                f'{self.test_worker_url}/pipelines/{self.test_pipeline_id}/source?mode=queue&processing=sync',
+                method='PATCH',
+                headers={'Accept': 'application/jsonl', 'Authorization': f'Bearer {self.test_access_token}'}, data=None,
+                json={'sourceType': 'URL', 'url': self.test_url},
+                timeout=aiohttp.ClientTimeout(total=None, sock_read=60))
+
+    @aioresponses()
+    @pytest.mark.asyncio
+    async def test_async_load_ok(self, mock: aioresponses) -> None:
+        self.setup_base_mock(mock)
+        mock.post(f'{self.test_eyepop_url}/authentication/token', status=200, body=json.dumps(
+            {'expires_in': 1000 * 1000, 'token_type': 'Bearer', 'access_token': self.test_access_token}))
+
+        async with EyePopSdk.endpoint(eyepop_url=self.test_eyepop_url, secret_key=self.test_eyepop_secret_key,
+                                pop_id=self.test_eyepop_pop_id, is_async=True) as endpoint:
+            self.assertBaseMock(mock)
+            test_timestamp = time.time() * 1000 * 1000 * 1000
+
+            def loadFrom(url, **kwargs) -> CallbackResult:
+                nonlocal test_timestamp
+                if kwargs['headers']['Authorization'] == f'Bearer {self.test_access_token}':
+                    return CallbackResult(status=200,
+                                          body=json.dumps(
+                                              {'source_id': self.test_source_id, 'seconds': 0,
+                                               'system_timestamp': test_timestamp}))
+                else:
+                    return CallbackResult(status=401, reason='test auth token expired')
+
+            mock.patch(f'{self.test_worker_url}/pipelines/{self.test_pipeline_id}/source?mode=queue&processing=sync',
+                       callback=loadFrom)
+
+            job = await endpoint.load_from(self.test_url)
+            result = await job.predict()
+            self.assertIsNotNone(result)
+            self.assertEqual(result['source_id'], self.test_source_id)
+            self.assertEqual(result['seconds'], 0)
+            self.assertEqual(result['system_timestamp'], test_timestamp)
+            self.assertIsNone(await job.predict())
+
             mock.assert_called_with(
-                f'{self.test_worker_url}/pipelines/{self.test_pipeline_id}/source?mode=preempt&processing=sync',
-                method='PATCH', headers={'Authorization': f'Bearer {self.test_access_token}'}, data=None,
-                json={'sourceType': 'NONE'})
+                f'{self.test_worker_url}/pipelines/{self.test_pipeline_id}/source?mode=queue&processing=sync',
+                method='PATCH',
+                headers={'Accept': 'application/jsonl', 'Authorization': f'Bearer {self.test_access_token}'}, data=None,
+                json={'sourceType': 'URL', 'url': self.test_url},
+                timeout=aiohttp.ClientTimeout(total=None, sock_read=60))
```

### Comparing `eyepop-0.15.3/tests/test.jpg` & `eyepop-0.9.2/tests/test.jpg`

 * *Files identical despite different names*

### Comparing `eyepop-0.15.3/tests/test_endpoint_retry.py` & `eyepop-0.9.2/eyepop/jobs.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,119 +1,173 @@
+import asyncio
 import json
-import time
+import logging
+import mimetypes
+from asyncio import Queue
+from enum import Enum
+from typing import Callable
+
 import aiohttp
-import pytest
-from aioresponses import aioresponses, CallbackResult
+from aiohttp import ClientSession
 
-from eyepop import EyePopSdk
-from tests.base_endpoint_test import BaseEndpointTest
+log_requests = logging.getLogger('eyepop.requests')
 
 
-class TestEndpointLoadFrom(BaseEndpointTest):
-    test_source_id = 'test_source_id'
-    test_url = 'http://examle-media.test/test.png'
-
-    @aioresponses()
-    def test_sync_load_auth_retry(self, mock: aioresponses):
-        self._prepare_mock(mock)
-        with EyePopSdk.endpoint(eyepop_url=self.test_eyepop_url, secret_key=self.test_eyepop_secret_key,
-                                pop_id=self.test_eyepop_pop_id) as endpoint:
-            self.assertBaseMock(mock)
-            test_timestamp = time.time() * 1000 * 1000 * 1000
-
-            self.test_access_token = '... a new access token ....'
-            self._prepare_mock(mock)
-
-            def loadFrom(url, **kwargs) -> CallbackResult:
-                nonlocal test_timestamp
-                if kwargs['headers']['Authorization'] == f'Bearer {self.test_access_token}':
-                    return CallbackResult(status=200,
-                                          body=json.dumps(
-                                              {'source_id': self.test_source_id, 'seconds': 0,
-                                               'system_timestamp': test_timestamp}))
-                else:
-                    return CallbackResult(status=401, reason='test auth token expired')
-
-            mock.patch(f'{self.test_worker_url}/pipelines/{self.test_pipeline_id}/source?mode=queue&processing=sync',
-                       callback=loadFrom, repeat=True)
-
-            job = endpoint.load_from(self.test_url)
-            result = job.predict()
-            self.assertIsNotNone(result)
-            self.assertEqual(result['source_id'], self.test_source_id)
-            self.assertEqual(result['seconds'], 0)
-            self.assertEqual(result['system_timestamp'], test_timestamp)
-            self.assertIsNone(job.predict())
-
-            mock.assert_called_with(
-                f'{self.test_worker_url}/pipelines/{self.test_pipeline_id}/source?mode=queue&processing=sync',
-                method='PATCH',
-                headers={
-                    'Accept': 'application/jsonl',
-                    'Content-Type': 'application/json',
-                    'Authorization': f'Bearer {self.test_access_token}'
-                },
-                data=json.dumps({'sourceType': 'URL', 'url': self.test_url}),
-                timeout=aiohttp.ClientTimeout(total=None, sock_read=60))
-
-    @aioresponses()
-    def test_sync_load_auth_retry(self, mock: aioresponses):
-        self._prepare_mock(mock)
-        with EyePopSdk.endpoint(eyepop_url=self.test_eyepop_url, secret_key=self.test_eyepop_secret_key,
-                                pop_id=self.test_eyepop_pop_id) as endpoint:
-            self.assertBaseMock(mock)
-            test_timestamp = time.time() * 1000 * 1000 * 1000
-
-            self.test_access_token = '... a new access token ....'
-            self._prepare_mock(mock)
-
-            def loadFrom(url, **kwargs) -> CallbackResult:
-                nonlocal test_timestamp
-                if kwargs['headers']['Authorization'] == f'Bearer {self.test_access_token}':
-                    return CallbackResult(status=200,
-                                          body=json.dumps(
-                                              {'source_id': self.test_source_id, 'seconds': 0,
-                                               'system_timestamp': test_timestamp}))
-                else:
-                    return CallbackResult(status=401, reason='test auth token expired')
-
-            mock.patch(f'{self.test_worker_url}/pipelines/{self.test_pipeline_id}/source?mode=queue&processing=sync',
-                       callback=loadFrom, repeat=True)
-
-            job = endpoint.load_from(self.test_url)
-            result = job.predict()
-            self.assertIsNotNone(result)
-            self.assertEqual(result['source_id'], self.test_source_id)
-            self.assertEqual(result['seconds'], 0)
-            self.assertEqual(result['system_timestamp'], test_timestamp)
-            self.assertIsNone(job.predict())
-
-            mock.assert_called_with(
-                f'{self.test_worker_url}/pipelines/{self.test_pipeline_id}/source?mode=queue&processing=sync',
-                method='PATCH',
-                headers={
-                    'Accept': 'application/jsonl',
-                    'Content-Type': 'application/json',
-                    'Authorization': f'Bearer {self.test_access_token}'
-                },
-                data=json.dumps({'sourceType': 'URL', 'url': self.test_url}),
-                timeout=aiohttp.ClientTimeout(total=None, sock_read=60))
-
-
-    def _prepare_mock(self, mock):
-        self.setup_base_mock(mock)
-        mock.post(f'{self.test_eyepop_url}/authentication/token',
-                  status=200,
-                  body=json.dumps({
-                      'expires_in': 1000 * 1000, 'token_type': 'Bearer', 'access_token': self.test_access_token
-                  }),
-                  repeat=True)
-
-        # automatic call to get pop comp and store
-        def get_pop_comp(url, **kwargs) -> CallbackResult:
-            if kwargs['headers']['Authorization'] != f'Bearer {self.test_access_token}':
-                return CallbackResult(status=401, reason='test auth token expired')
+class JobType(Enum):
+    UPLOAD = 1
+    FROM_URL = 2
+
+
+class _JobStateCallback:
+    def created(self, job):
+        pass
+
+    def started(self, job):
+        pass
+
+    def first_result(self, job):
+        pass
+
+    def failed(self, job):
+        pass
+
+    def finished(self, job):
+        pass
+
+    def drained(self, job):
+        pass
+
+    def finalized(self, job):
+        pass
+
+class Job:
+    """
+    Abstract Job submitted to an EyePop.ai Endpoint.
+    """
+
+    def __init__(self, job_type: JobType, location: str, session: ClientSession,
+                 on_ready: Callable[["Job"], None] | None, callback: _JobStateCallback | None = None):
+        self.on_ready = on_ready
+        self.job_type = job_type
+        self.location = location
+        self._session = session
+        self._response = None
+        self._queue = asyncio.Queue(maxsize=128)
+        if callback is not None:
+            self._callback = callback
+        else:
+            self._callback = _JobStateCallback()
+        self._callback.created(self)
+
+    def __del__(self):
+        self._callback.finalized(self)
+
+    async def predict(self) -> dict:
+        queue = self._queue
+        if queue is None:
+            return None
+        else:
+            prediction = await queue.get()
+            if prediction is None:
+                self._queue = None
+                self._callback.drained(self)
+            elif isinstance(prediction, Exception):
+                self._queue = None
+                self._callback.drained(self)
+                raise prediction
+            return prediction
+
+    async def cancel(self):
+        queue = self._queue
+        if queue is None:
+            return None
+        self._queue = None
+        if self._response is not None:
+            self._response.close()
+        await queue.put(None)
+
+    async def execute(self):
+        queue = self._queue
+        session = self._session
+
+        self._callback.started(self)
+
+        try:
+            await self._do_execute_job(queue, session)
+            await queue.put(None)
+        except Exception as e:
+            if self._queue is None:
+                # we got canceled
+                pass
             else:
-                return CallbackResult(status=200, body=json.dumps({'inferPipeline': self.test_pop_comp}))
-
-        mock.get(f'{self.test_worker_url}/pipelines/{self.test_pipeline_id}',
-                 callback=get_pop_comp)
+                self._callback.failed(self)
+                await queue.put(e)
+        finally:
+            if self._response is not None:
+                response = self._response.close()
+                if response is not None:
+                    response.release()
+            self._callback.finished(self)
+            if self.on_ready:
+                await self.on_ready(self)
+
+    async def _do_execute_job(self, queue: Queue, session: ClientSession):
+        raise NotImplementedError("can't execute abstract jobs")
+
+    async def _do_read_response(self, queue: Queue):
+        got_results = False
+        async with self._response as response:
+            self._callback.first_result(self)
+            while line := await response.content.readline():
+                if not got_results:
+                    got_results = True
+                prediction = json.loads(line)
+                await queue.put(prediction)
+
+
+class _UploadJob(Job):
+    def __init__(self, location: str, pipeline_base_url: str, authorization_header: str, session: ClientSession,
+                 on_ready: Callable[[Job], None] | None = None, callback: _JobStateCallback | None = None):
+        super().__init__(JobType.UPLOAD, location, session, on_ready, callback)
+        mime_types = mimetypes.guess_type(location)
+        if len(mime_types) > 0:
+            mime_type = mime_types[0]
+        else:
+            mime_type = 'application/octet-stream'
+        self._target_url = f'{pipeline_base_url}/source?mode=queue&processing=sync'
+        self._headers = {
+            'Content-Type': mime_type,
+            'Accept': 'application/jsonl',
+            'Authorization': authorization_header
+        }
+        self.timeouts = aiohttp.ClientTimeout(total=None, sock_read=60)
+
+    async def _do_execute_job(self, queue: Queue, session: ClientSession):
+        with open(self.location, 'rb') as file:
+            log_requests.debug("before POST %s with file %s as body", self._target_url, self.location)
+            self._response = await session.post(self._target_url, headers=self._headers, data=file,
+                                                timeout=self.timeouts)
+            await self._do_read_response(queue)
+            log_requests.debug("after POST %s with file %s as body", self._target_url, self.location)
+
+
+class _LoadFromJob(Job):
+    def __init__(self, location: str, pipeline_base_url: str, authorization_header: str, session: ClientSession,
+                 on_ready: Callable[[Job], None] | None = None, callback: _JobStateCallback | None = None):
+        super().__init__(JobType.FROM_URL, location, session, on_ready, callback)
+        self._target_url = f'{pipeline_base_url}/source?mode=queue&processing=sync'
+        self._headers = {
+            'Accept': 'application/jsonl',
+            'Authorization': authorization_header
+        }
+        self._body = {
+            "sourceType": "URL",
+            "url": self.location
+        }
+        self.timeouts = aiohttp.ClientTimeout(total=None, sock_read=60)
+
+    async def _do_execute_job(self, queue: Queue, session: ClientSession):
+        log_requests.debug("before PATCH %s with url %s as source", self._target_url, self.location)
+        self._response = await session.patch(self._target_url, headers=self._headers, json=self._body,
+                                             timeout=self.timeouts)
+        await self._do_read_response(queue)
+        log_requests.debug("after PATCH %s with url %s as source", self._target_url, self.location)
```

### Comparing `eyepop-0.15.3/tests/test_endpoint_upload.py` & `eyepop-0.9.2/tests/test_endpoint_upload.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,33 +6,26 @@
 import pytest
 from aioresponses import aioresponses, CallbackResult
 
 from eyepop import EyePopSdk
 from tests.base_endpoint_test import BaseEndpointTest
 import tests
 
-class TestEndpointUpload(BaseEndpointTest):
+class TestEndpointUploadFrom(BaseEndpointTest):
     test_source_id = 'test_source_id'
     test_file = resources.files(tests) / 'test.jpg'
     test_content_type = 'image/jpeg'
 
 
     @aioresponses()
     def test_sync_upload_ok(self, mock: aioresponses):
         self.setup_base_mock(mock)
         mock.post(f'{self.test_eyepop_url}/authentication/token', status=200, body=json.dumps(
             {'expires_in': 1000 * 1000, 'token_type': 'Bearer', 'access_token': self.test_access_token}))
-        # automatic call to get pop comp and store
-        def get_pop_comp(url, **kwargs) -> CallbackResult:
-            if kwargs['headers']['Authorization'] != f'Bearer {self.test_access_token}':
-                return CallbackResult(status=401, reason='test auth token expired')
-            else:
-                return CallbackResult(status=200, body=json.dumps({'inferPipeline': self.test_pop_comp}))
-        mock.get(f'{self.test_worker_url}/pipelines/{self.test_pipeline_id}',
-                    callback=get_pop_comp)
+
         with EyePopSdk.endpoint(eyepop_url=self.test_eyepop_url, secret_key=self.test_eyepop_secret_key,
                                 pop_id=self.test_eyepop_pop_id) as endpoint:
             self.assertBaseMock(mock)
             test_timestamp = time.time() * 1000 * 1000 * 1000
 
             upload_called = 0
 
@@ -66,22 +59,15 @@
 
     @aioresponses()
     @pytest.mark.asyncio
     async def test_async_upload_ok(self, mock: aioresponses):
         self.setup_base_mock(mock)
         mock.post(f'{self.test_eyepop_url}/authentication/token', status=200, body=json.dumps(
             {'expires_in': 1000 * 1000, 'token_type': 'Bearer', 'access_token': self.test_access_token}))
-        # automatic call to get pop comp and store
-        def get_pop_comp(url, **kwargs) -> CallbackResult:
-            if kwargs['headers']['Authorization'] != f'Bearer {self.test_access_token}':
-                return CallbackResult(status=401, reason='test auth token expired')
-            else:
-                return CallbackResult(status=200, body=json.dumps({'inferPipeline': self.test_pop_comp}))
-        mock.get(f'{self.test_worker_url}/pipelines/{self.test_pipeline_id}',
-                    callback=get_pop_comp)
+
         async with EyePopSdk.endpoint(eyepop_url=self.test_eyepop_url, secret_key=self.test_eyepop_secret_key,
                                 pop_id=self.test_eyepop_pop_id, is_async=True) as endpoint:
             self.assertBaseMock(mock)
             test_timestamp = time.time() * 1000 * 1000 * 1000
 
             upload_called = 0
```

