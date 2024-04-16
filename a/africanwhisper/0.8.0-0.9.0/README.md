# Comparing `tmp/africanwhisper-0.8.tar.gz` & `tmp/africanwhisper-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "africanwhisper-0.8.tar", last modified: Fri Apr 12 16:33:29 2024, max compression
+gzip compressed data, was "africanwhisper-0.9.0.tar", last modified: Tue Apr 16 13:21:46 2024, max compression
```

## Comparing `africanwhisper-0.8.tar` & `africanwhisper-0.9.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:33:29.079936 africanwhisper-0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-12 16:33:25.000000 africanwhisper-0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11255 2024-04-12 16:33:29.079936 africanwhisper-0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10050 2024-04-12 16:33:25.000000 africanwhisper-0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-12 16:33:25.000000 africanwhisper-0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-12 16:33:29.079936 africanwhisper-0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:33:29.075936 africanwhisper-0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:33:29.079936 africanwhisper-0.8/src/africanwhisper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11255 2024-04-12 16:33:29.000000 africanwhisper-0.8/src/africanwhisper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-12 16:33:29.000000 africanwhisper-0.8/src/africanwhisper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 16:33:29.000000 africanwhisper-0.8/src/africanwhisper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-12 16:33:29.000000 africanwhisper-0.8/src/africanwhisper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-12 16:33:29.000000 africanwhisper-0.8/src/africanwhisper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:33:29.079936 africanwhisper-0.8/src/deployment/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 16:33:25.000000 africanwhisper-0.8/src/deployment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-04-12 16:33:25.000000 africanwhisper-0.8/src/deployment/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-04-12 16:33:25.000000 africanwhisper-0.8/src/deployment/speech_inference.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:33:29.079936 africanwhisper-0.8/src/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 16:33:25.000000 africanwhisper-0.8/src/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-04-12 16:33:25.000000 africanwhisper-0.8/src/tests/test_load_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:33:29.079936 africanwhisper-0.8/src/training/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 16:33:25.000000 africanwhisper-0.8/src/training/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-12 16:33:25.000000 africanwhisper-0.8/src/training/audio_data_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-12 16:33:25.000000 africanwhisper-0.8/src/training/collator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4480 2024-04-12 16:33:25.000000 africanwhisper-0.8/src/training/data_prep.py
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-12 16:33:25.000000 africanwhisper-0.8/src/training/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-12 16:33:25.000000 africanwhisper-0.8/src/training/gradio_demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     6383 2024-04-12 16:33:25.000000 africanwhisper-0.8/src/training/gradio_inference.py
--rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-04-12 16:33:25.000000 africanwhisper-0.8/src/training/load_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-04-12 16:33:25.000000 africanwhisper-0.8/src/training/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     7226 2024-04-12 16:33:25.000000 africanwhisper-0.8/src/training/model_trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7942 2024-04-12 16:33:25.000000 africanwhisper-0.8/src/training/wandb_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     4410 2024-04-12 16:33:25.000000 africanwhisper-0.8/src/training/whisper_model_prep.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:21:46.667922 africanwhisper-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-16 13:21:43.000000 africanwhisper-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11255 2024-04-16 13:21:46.667922 africanwhisper-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10050 2024-04-16 13:21:43.000000 africanwhisper-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-16 13:21:43.000000 africanwhisper-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-16 13:21:46.667922 africanwhisper-0.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:21:46.663922 africanwhisper-0.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:21:46.667922 africanwhisper-0.9.0/src/africanwhisper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11255 2024-04-16 13:21:46.000000 africanwhisper-0.9.0/src/africanwhisper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-16 13:21:46.000000 africanwhisper-0.9.0/src/africanwhisper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 13:21:46.000000 africanwhisper-0.9.0/src/africanwhisper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-16 13:21:46.000000 africanwhisper-0.9.0/src/africanwhisper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-16 13:21:46.000000 africanwhisper-0.9.0/src/africanwhisper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:21:46.663922 africanwhisper-0.9.0/src/deployment/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 13:21:43.000000 africanwhisper-0.9.0/src/deployment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-04-16 13:21:43.000000 africanwhisper-0.9.0/src/deployment/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-04-16 13:21:43.000000 africanwhisper-0.9.0/src/deployment/speech_inference.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:21:46.663922 africanwhisper-0.9.0/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 13:21:43.000000 africanwhisper-0.9.0/src/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-04-16 13:21:43.000000 africanwhisper-0.9.0/src/tests/test_load_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:21:46.667922 africanwhisper-0.9.0/src/training/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 13:21:43.000000 africanwhisper-0.9.0/src/training/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-16 13:21:43.000000 africanwhisper-0.9.0/src/training/audio_data_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-16 13:21:43.000000 africanwhisper-0.9.0/src/training/collator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4480 2024-04-16 13:21:43.000000 africanwhisper-0.9.0/src/training/data_prep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-16 13:21:43.000000 africanwhisper-0.9.0/src/training/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-16 13:21:43.000000 africanwhisper-0.9.0/src/training/gradio_demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6383 2024-04-16 13:21:43.000000 africanwhisper-0.9.0/src/training/gradio_inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-04-16 13:21:43.000000 africanwhisper-0.9.0/src/training/load_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-04-16 13:21:43.000000 africanwhisper-0.9.0/src/training/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7226 2024-04-16 13:21:43.000000 africanwhisper-0.9.0/src/training/model_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7942 2024-04-16 13:21:43.000000 africanwhisper-0.9.0/src/training/wandb_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4410 2024-04-16 13:21:43.000000 africanwhisper-0.9.0/src/training/whisper_model_prep.py
```

### Comparing `africanwhisper-0.8/LICENSE` & `africanwhisper-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.8/PKG-INFO` & `africanwhisper-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: africanwhisper
-Version: 0.8.0
+Version: 0.9.0
 Summary: A package for fast fine-tuning and API endpoint deployment of Whisper model specifically developed to accelerate Automatic Speech Recognition(ASR) for African Languages.
 Home-page: https://github.com/KevKibe/African-Whisper
 Author: Kevin Kibe
 Author-email: keviinkibe@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: africanwhisper Version: 0.8.0 Summary: A package
+Metadata-Version: 2.1 Name: africanwhisper Version: 0.9.0 Summary: A package
 for fast fine-tuning and API endpoint deployment of Whisper model specifically
 developed to accelerate Automatic Speech Recognition(ASR) for African
 Languages. Home-page: https://github.com/KevKibe/African-Whisper Author: Kevin
 Kibe Author-email: keviinkibe@gmail.com License: MIT Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 pip==24.0 Requires-Dist: transformers==4.39.2 Requires-Dist: datasets==2.17.0
 Requires-Dist: librosa==0.10.1 Requires-Dist: evaluate==0.4.1 Requires-Dist:
```

### Comparing `africanwhisper-0.8/README.md` & `africanwhisper-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.8/setup.cfg` & `africanwhisper-0.9.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = africanwhisper
 author = Kevin Kibe
-version = 0.8.0
+version = 0.9.0
 author_email = keviinkibe@gmail.com
 description = A package for fast fine-tuning and API endpoint deployment of Whisper model specifically developed to accelerate Automatic Speech Recognition(ASR) for African Languages.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/KevKibe/African-Whisper
 license = MIT
```

### Comparing `africanwhisper-0.8/src/africanwhisper.egg-info/PKG-INFO` & `africanwhisper-0.9.0/src/africanwhisper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: africanwhisper
-Version: 0.8.0
+Version: 0.9.0
 Summary: A package for fast fine-tuning and API endpoint deployment of Whisper model specifically developed to accelerate Automatic Speech Recognition(ASR) for African Languages.
 Home-page: https://github.com/KevKibe/African-Whisper
 Author: Kevin Kibe
 Author-email: keviinkibe@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: africanwhisper Version: 0.8.0 Summary: A package
+Metadata-Version: 2.1 Name: africanwhisper Version: 0.9.0 Summary: A package
 for fast fine-tuning and API endpoint deployment of Whisper model specifically
 developed to accelerate Automatic Speech Recognition(ASR) for African
 Languages. Home-page: https://github.com/KevKibe/African-Whisper Author: Kevin
 Kibe Author-email: keviinkibe@gmail.com License: MIT Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 pip==24.0 Requires-Dist: transformers==4.39.2 Requires-Dist: datasets==2.17.0
 Requires-Dist: librosa==0.10.1 Requires-Dist: evaluate==0.4.1 Requires-Dist:
```

### Comparing `africanwhisper-0.8/src/africanwhisper.egg-info/SOURCES.txt` & `africanwhisper-0.9.0/src/africanwhisper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.8/src/deployment/main.py` & `africanwhisper-0.9.0/src/deployment/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,40 @@
 import os
-from fastapi import FastAPI, UploadFile, HTTPException
+from fastapi import FastAPI, UploadFile, HTTPException, Response
 from pydantic import BaseModel
 import tempfile
 from speech_inference import SpeechInference
 import logging
-import time
 from dotenv import load_dotenv
+import uvicorn
+import time
+import prometheus_client
+from prometheus_client import Histogram, Counter
 load_dotenv()
 
-app = FastAPI()
+app = FastAPI(debug=True)
 
+request_time = Histogram('request_processing_seconds', 'Time spent processing request')
+request_count = prometheus_client.Counter("request_count", "number_of_requests")
+errors_counter = Counter('app_errors_total', 'Total number of errors in the application')
+successful_requests_counter = Counter('app_successful_requests_total', 'Total number of successful requests in the application')
 
 model_name = os.getenv("MODEL_NAME")
 huggingface_read_token = os.getenv("HUGGINGFACE_READ_TOKEN")
 inference = SpeechInference(model_name, huggingface_read_token)
 pipeline = inference.pipe_initialization()
 
 
 class AudioTranscriptionRequest(BaseModel):
     file: UploadFile
     task: str
 
-
-
 @app.post("/speech_inference")
 async def speechinference(file: UploadFile, task: str):
+    request_count.inc()
     logger = logging.getLogger(__name__)
     logging.basicConfig(format='%(asctime)s %(levelname)-8s %(message)s', filename='app.log', level=logging.INFO, datefmt='%Y-%m-%d %H:%M:%S')
     if file is None:
         logger.error("No file provided")
         raise HTTPException(status_code=400, detail="No file provided")
 
     try:
@@ -37,22 +43,33 @@
             tmp_file_path = tmp_file.name
 
         if file.filename.endswith(".mp3"):
             logger.info("Processing mp3 file")
             start_time = time.time()
             result = inference.output(pipeline, tmp_file_path, task)
             end_time = time.time()
-            logger.info(f"Time taken for inference: {end_time - start_time} seconds")
+            duration = end_time - start_time
+            request_time.observe(duration)
+            logger.info(f"Time taken for inference: {duration} seconds")
         elif file.filename.endswith(".wav"):
             logger.info("Processing wav file")
             pass
         else:
             logger.error("Unsupported file format")
             raise HTTPException(status_code=400, detail="Unsupported file format")
 
         logger.info("File processed successfully")
+        successful_requests_counter.inc()
         return result
     except Exception as e:
         logger.error(f"Error processing file: {str(e)}")
+        errors_counter.inc()
         raise HTTPException(status_code=500, detail=f"Error processing file: {str(e)}")
 
 
+@app.get("/metrics")
+def metrics():
+    return Response(
+        content = prometheus_client.generate_latest())
+
+if __name__ == "__main__":
+    uvicorn.run(app, host = "0.0.0.0", port = 8000)
```

### Comparing `africanwhisper-0.8/src/deployment/speech_inference.py` & `africanwhisper-0.9.0/src/deployment/speech_inference.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.8/src/tests/test_load_dataset.py` & `africanwhisper-0.9.0/src/tests/test_load_dataset.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.8/src/training/audio_data_processor.py` & `africanwhisper-0.9.0/src/training/audio_data_processor.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.8/src/training/collator.py` & `africanwhisper-0.9.0/src/training/collator.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.8/src/training/data_prep.py` & `africanwhisper-0.9.0/src/training/data_prep.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.8/src/training/evaluation.py` & `africanwhisper-0.9.0/src/training/evaluation.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.8/src/training/gradio_demo.py` & `africanwhisper-0.9.0/src/training/gradio_demo.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.8/src/training/gradio_inference.py` & `africanwhisper-0.9.0/src/training/gradio_inference.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.8/src/training/load_data.py` & `africanwhisper-0.9.0/src/training/load_data.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.8/src/training/main.py` & `africanwhisper-0.9.0/src/training/main.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.8/src/training/model_trainer.py` & `africanwhisper-0.9.0/src/training/model_trainer.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.8/src/training/wandb_callback.py` & `africanwhisper-0.9.0/src/training/wandb_callback.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.8/src/training/whisper_model_prep.py` & `africanwhisper-0.9.0/src/training/whisper_model_prep.py`

 * *Files identical despite different names*

