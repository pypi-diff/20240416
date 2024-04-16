# Comparing `tmp/tonic_textual-1.1.0.tar.gz` & `tmp/tonic_textual-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tonic_textual-1.1.0.tar", max compression
+gzip compressed data, was "tonic_textual-1.2.0.tar", max compression
```

## Comparing `tonic_textual-1.1.0.tar` & `tonic_textual-1.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1084 2023-08-21 15:18:32.578537 tonic_textual-1.1.0/LICENSE
--rw-r--r--   0        0        0      598 2024-04-16 13:46:53.564799 tonic_textual-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      972 2023-11-03 19:05:54.671774 tonic_textual-1.1.0/README.md
--rw-r--r--   0        0        0       19 2024-02-28 13:39:57.538020 tonic_textual-1.1.0/tonic_textual/__init__.py
--rw-r--r--   0        0        0    10966 2024-04-16 13:46:35.575964 tonic_textual-1.1.0/tonic_textual/api.py
--rw-r--r--   0        0        0        0 2023-11-03 19:05:54.674583 tonic_textual-1.1.0/tonic_textual/classes/__init__.py
--rw-r--r--   0        0        0      789 2023-11-15 15:30:22.056092 tonic_textual-1.1.0/tonic_textual/classes/api_responses/redaction_response.py
--rw-r--r--   0        0        0      668 2024-02-28 13:39:57.539026 tonic_textual-1.1.0/tonic_textual/classes/api_responses/single_detection_result.py
--rw-r--r--   0        0        0      348 2023-11-03 19:05:54.674583 tonic_textual-1.1.0/tonic_textual/classes/custom_model.py
--rw-r--r--   0        0        0     8219 2024-04-16 13:46:35.576966 tonic_textual-1.1.0/tonic_textual/classes/dataset.py
--rw-r--r--   0        0        0     1633 2023-11-14 22:48:18.528603 tonic_textual-1.1.0/tonic_textual/classes/datasetfile.py
--rw-r--r--   0        0        0       95 2023-11-03 19:05:54.674583 tonic_textual-1.1.0/tonic_textual/classes/generator_config.py
--rw-r--r--   0        0        0     3442 2024-04-16 13:46:35.577964 tonic_textual-1.1.0/tonic_textual/classes/httpclient.py
--rw-r--r--   0        0        0     1342 2024-04-16 13:46:35.578966 tonic_textual-1.1.0/tonic_textual/classes/tonic_exception.py
--rw-r--r--   0        0        0       92 2023-11-03 19:05:54.674583 tonic_textual-1.1.0/tonic_textual/enums/pii_state.py
--rw-r--r--   0        0        0        0 2023-11-03 19:05:54.674583 tonic_textual-1.1.0/tonic_textual/services/__init__.py
--rw-r--r--   0        0        0      610 2023-11-03 19:05:54.674583 tonic_textual-1.1.0/tonic_textual/services/dataset.py
--rw-r--r--   0        0        0      552 2023-11-03 19:05:54.674583 tonic_textual-1.1.0/tonic_textual/services/datasetfile.py
--rw-r--r--   0        0        0     1885 1970-01-01 00:00:00.000000 tonic_textual-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-08-21 15:18:32.578537 tonic_textual-1.2.0/LICENSE
+-rw-r--r--   0        0        0      598 2024-04-16 14:27:41.277226 tonic_textual-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      972 2023-11-03 19:05:54.671774 tonic_textual-1.2.0/README.md
+-rw-r--r--   0        0        0       19 2024-04-16 14:54:12.778627 tonic_textual-1.2.0/tonic_textual/__init__.py
+-rw-r--r--   0        0        0    14228 2024-04-16 14:31:27.775440 tonic_textual-1.2.0/tonic_textual/api.py
+-rw-r--r--   0        0        0        0 2023-11-03 19:05:54.674583 tonic_textual-1.2.0/tonic_textual/classes/__init__.py
+-rw-r--r--   0        0        0      789 2023-11-15 15:30:22.056092 tonic_textual-1.2.0/tonic_textual/classes/api_responses/redaction_response.py
+-rw-r--r--   0        0        0      668 2024-02-28 13:39:57.539026 tonic_textual-1.2.0/tonic_textual/classes/api_responses/single_detection_result.py
+-rw-r--r--   0        0        0      348 2024-04-16 14:31:52.343889 tonic_textual-1.2.0/tonic_textual/classes/custom_model.py
+-rw-r--r--   0        0        0     8183 2024-04-16 14:27:25.096645 tonic_textual-1.2.0/tonic_textual/classes/dataset.py
+-rw-r--r--   0        0        0     1633 2023-11-14 22:48:18.528603 tonic_textual-1.2.0/tonic_textual/classes/datasetfile.py
+-rw-r--r--   0        0        0       95 2023-11-03 19:05:54.674583 tonic_textual-1.2.0/tonic_textual/classes/generator_config.py
+-rw-r--r--   0        0        0     4668 2024-04-16 14:27:25.097640 tonic_textual-1.2.0/tonic_textual/classes/httpclient.py
+-rw-r--r--   0        0        0     1864 2024-04-16 14:27:25.098640 tonic_textual-1.2.0/tonic_textual/classes/tonic_exception.py
+-rw-r--r--   0        0        0       92 2023-11-03 19:05:54.674583 tonic_textual-1.2.0/tonic_textual/enums/pii_state.py
+-rw-r--r--   0        0        0        0 2023-11-03 19:05:54.674583 tonic_textual-1.2.0/tonic_textual/services/__init__.py
+-rw-r--r--   0        0        0      610 2023-11-03 19:05:54.674583 tonic_textual-1.2.0/tonic_textual/services/dataset.py
+-rw-r--r--   0        0        0      552 2023-11-03 19:05:54.674583 tonic_textual-1.2.0/tonic_textual/services/datasetfile.py
+-rw-r--r--   0        0        0     1885 1970-01-01 00:00:00.000000 tonic_textual-1.2.0/PKG-INFO
```

### Comparing `tonic_textual-1.1.0/LICENSE` & `tonic_textual-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tonic_textual-1.1.0/pyproject.toml` & `tonic_textual-1.2.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tonic-textual"
-version = "1.1.0"
+version = "1.2.0"
 description = "Wrappers around the Tonic Textual API"
 authors = ["Adam Kamor <adam@tonic.ai>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://www.tonic.ai/"
 keywords = ["tonic.ai", "tonic", "tonic textual"]
```

### Comparing `tonic_textual-1.1.0/README.md` & `tonic_textual-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `tonic_textual-1.1.0/tonic_textual/api.py` & `tonic_textual-1.2.0/tonic_textual/api.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,29 @@
+import io
 import json
 import os
 import requests
 
+from time import sleep
 from typing import List, Optional, Union
 from urllib.parse import urlencode
 
+from tqdm.utils import CallbackIOWrapper
+from tqdm import tqdm
 from tonic_textual.classes.api_responses.single_detection_result import SingleDetectionResult
 from tonic_textual.classes.custom_model import CustomModel
 from tonic_textual.classes.generator_config import GeneratorConfig
 from tonic_textual.classes.httpclient import HttpClient
 from tonic_textual.classes.api_responses.redaction_response import RedactionResponse
 from tonic_textual.enums.pii_state import PiiState
 from tonic_textual.services.dataset import DatasetService
 from tonic_textual.services.datasetfile import DatasetFileService
 from tonic_textual.classes.dataset import Dataset
 from tonic_textual.classes.datasetfile import DatasetFile
-from tonic_textual.classes.tonic_exception import DatasetNameAlreadyExists, InvalidJsonForRedactionRequest
+from tonic_textual.classes.tonic_exception import DatasetNameAlreadyExists, InvalidJsonForRedactionRequest, FileNotReadyForDownload
 
 class TonicTextual:
     '''Wrapper class for invoking Tonic Textual API
 
     Parameters
     ----------
     base_url : str
@@ -137,85 +141,85 @@
             str
                 The string with the redaction removed.
             """
             
             response = self.client.http_post("/api/unredact", data=[redacted_string])            
             return response
     
-    def redact(self, string: str, generatorConfig: GeneratorConfig = dict(), customModels: List[str] = [], random_seed: Optional[int] = None) -> RedactionResponse:
+    def redact(self, string: str, generator_config: GeneratorConfig = dict(), custom_models: List[str] = [], random_seed: Optional[int] = None) -> RedactionResponse:
             """Redacts a string. Depending on the configured handling for each sensitive data type, values can be either redacted, synthesized, or ignored.
             
             Parameters
             ----------
             string : str
                 The string to redact.
             
-            generatorConfig: GeneratorConfig
+            generator_config: GeneratorConfig
                 A dictionary of sensitive data entities. For each entity, indicates whether to redact, synthesize, or ignore it.
     
-            customModels: List[str]
+            custom_models: List[str]
                 A list of custom model names to use to identify values to redact. To see the list of custom models that you have access to, use the get_custom_models function.
             
             random_seed: Optional[int]
                 An optional value to use to override Textual's default random number seeding.  Can be used to ensure that different API calls use the same or different random seeds.
                 
             Returns
             -------
             RedactionResponse
                 The redacted string along with ancillary information.
             """
             
-            invalid_pii_states = [v for v in list(generatorConfig.values()) if v not in PiiState._member_names_]
+            invalid_pii_states = [v for v in list(generator_config.values()) if v not in PiiState._member_names_]
             if(len(invalid_pii_states)>0):
                  raise Exception("Invalid configuration for generatorConfig. The allowed values are Off, Synthesis, and Redaction.")                 
 
             endpoint = "/api/redact"
 
             if random_seed is not None:                 
-                response = self.client.http_post(endpoint, data={"text": string, "generatorConfig": generatorConfig, "customModels": customModels}, additionalHeaders={'textual-random-seed':str(random_seed)})
+                response = self.client.http_post(endpoint, data={"text": string, "generatorConfig": generator_config, "customModels": custom_models}, additionalHeaders={'textual-random-seed':str(random_seed)})
             else:
-                response = self.client.http_post(endpoint, data={"text": string, "generatorConfig": generatorConfig, "customModels": customModels})
+                response = self.client.http_post(endpoint, data={"text": string, "generatorConfig": generator_config, "customModels": custom_models})
             
             de_id_results = [SingleDetectionResult(x["start"], x["end"], x["label"], x["text"], x["score"]) for x in list(response["deIdentifyResults"])]
 
             return RedactionResponse(response["originalText"], response["redactedText"], response["usage"], de_id_results)
     
-    def redact_json(self, json_data: Union[str, dict], generatorConfig: GeneratorConfig = dict(), customModels: List[str] = [], random_seed: Optional[int] = None) -> RedactionResponse:   
+    def redact_json(self, json_data: Union[str, dict], generator_config: GeneratorConfig = dict(), custom_models: List[str] = [], random_seed: Optional[int] = None) -> RedactionResponse:   
         """Redacts the values in a JSON blob. Depending on the configured handling for each sensitive data type, values can be either redacted, synthesized, or ignored.
         
         Parameters
         ----------
         json_string : Union[str, dict]
             The JSON whose values will be redacted.  This can be either a JSON string or a Python dictionary
         
-        generatorConfig: GeneratorConfig
+        generator_config: GeneratorConfig
             A dictionary of sensitive data entities. For each entity, indicates whether to redact, synthesize, or ignore it.
 
-        customModels: List[str]
+        custom_models: List[str]
             A list of custom model names to use to identify values to redact. To see the list of custom models that you have access to, use the get_custom_models function.
 
         random_seed: Optional[int]
             An optional value to use to override Textual's default random number seeding.  Can be used to ensure that different API calls use the same or different random seeds.            
 
         Returns
         -------
         RedactionResponse
             The redacted string along with ancillary information.
         """
         
-        invalid_pii_states = [v for v in list(generatorConfig.values()) if v not in PiiState._member_names_]
+        invalid_pii_states = [v for v in list(generator_config.values()) if v not in PiiState._member_names_]
         if(len(invalid_pii_states)>0):
                 raise Exception("Invalid configuration for generatorConfig. The allowed values are Off, Synthesis, and Redaction.")                 
 
         endpoint = "/api/redact/json"
 
         if isinstance(json_data, str):
-             payload = {"jsonText": json_data, "generatorConfig": generatorConfig, "customModels": customModels}
+             payload = {"jsonText": json_data, "generatorConfig": generator_config, "customModels": custom_models}
         elif isinstance(json_data, dict):
-             payload = {"jsonText": json.dumps(json_data), "generatorConfig": generatorConfig, "customModels": customModels}
+             payload = {"jsonText": json.dumps(json_data), "generatorConfig": generator_config, "customModels": custom_models}
         else:
             raise Exception(f'redact_json must receive either a JSON blob as a string or dict().  You passed in type {type(json_data)} which is not supported')
         
         try:
             if random_seed is not None:
                 response = self.client.http_post(endpoint, data=payload, additionalHeaders={'textual-random-seed':str(random_seed)})
             else:
@@ -245,7 +249,76 @@
                 id = model['id']
                 name = model['name']
                 entities = model['entities']
                 entityNames = [entity['label'] for entity in entities]
                 models.append(CustomModel(id, name, entityNames))
             
             return models
+        
+    def start_file_redaction(self, file: io.IOBase, file_name: str) -> str:
+        """
+        Redact a provided file
+
+        Parameters
+        --------
+        file: io.IOBase
+            The opened file, available for reading, which will be uploaded and redacted
+        file_name: str
+            The name of the file
+
+        Returns
+        -------
+        str
+        The job id which can be used to download the redacted file once it is ready
+
+        """
+
+        files = {
+            'document': (None, json.dumps({"fileName": file_name, "csvConfig":{}, "datasetId":""}), 'application/json'),
+            'file': file
+        }
+
+        response = self.client.http_post("/api/unattachedfile/upload", files=files)
+
+        return response['jobId']
+
+    def download_redacted_file(self, job_id: str, generator_config: GeneratorConfig = dict(), custom_models: List[str] = [], random_seed: Optional[int] = None, num_retries: Optional[int] = 6) -> io.BufferedWriter:
+        """
+        Download a redacted file
+
+        Parameters
+        --------
+        job_id: str
+            The ID of the redaction job
+                    
+        generator_config: GeneratorConfig
+            A dictionary of sensitive data entities. For each entity, indicates whether to redact, synthesize, or ignore it.
+
+        custom_models: List[str]
+            A list of custom model names to use to identify values to redact. To see the list of custom models that you have access to, use the get_custom_models function.
+        
+        random_seed: Optional[int]
+            An optional value to use to override Textual's default random number seeding.  Can be used to ensure that different API calls use the same or different random seeds.
+
+        num_retries: Optional[int]
+            An optional value to specify how many times to attempt to download the file.  If a file is not yet ready for download, there will be a 10 second pause before retrying.  (The default value is 6)
+            
+        Returns
+        -------
+        io.BufferedWriter
+            The redacted file, ready to be written to disc as a buffered byte array
+        """
+        retries = 1
+        while(retries <= num_retries):
+            try:
+                if random_seed is not None:
+                    return self.client.http_post_download_file(f"/api/unattachedfile/{job_id}/download", data={"generatorConfig": generator_config, "customModels": custom_models}, additionalHeaders={'textual-random-seed':str(random_seed)})
+                else:
+                    return self.client.http_post_download_file(f"/api/unattachedfile/{job_id}/download", data={"generatorConfig": generator_config, "customModels": custom_models})
+            except FileNotReadyForDownload:
+                 retries = retries + 1
+                 if retries <= num_retries:
+                    sleep(10)
+
+        retryWord = "retry" if num_retries==1 else "retries"
+        raise FileNotReadyForDownload(f"After {num_retries} {retryWord} the file is not yet ready for download.  This is likely due to a high service load.  Please try again later.")
+
```

### Comparing `tonic_textual-1.1.0/tonic_textual/classes/api_responses/redaction_response.py` & `tonic_textual-1.2.0/tonic_textual/classes/api_responses/redaction_response.py`

 * *Files identical despite different names*

### Comparing `tonic_textual-1.1.0/tonic_textual/classes/api_responses/single_detection_result.py` & `tonic_textual-1.2.0/tonic_textual/classes/api_responses/single_detection_result.py`

 * *Files identical despite different names*

### Comparing `tonic_textual-1.1.0/tonic_textual/classes/dataset.py` & `tonic_textual-1.2.0/tonic_textual/classes/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from __future__ import annotations
 from typing import List, Dict, Optional
 import os
 import json
 from tqdm import tqdm
 from tqdm.utils import CallbackIOWrapper
-from urllib.parse import urlencode
-import requests.exceptions;
+import requests.exceptions
 import requests
 import pandas as pd
 from tonic_textual.classes.tonic_exception import DatasetFileMatchesExistingFile
 from tonic_textual.classes.httpclient import HttpClient
 from tonic_textual.classes.datasetfile import DatasetFile
 from tonic_textual.services.datasetfile import DatasetFileService
```

### Comparing `tonic_textual-1.1.0/tonic_textual/classes/datasetfile.py` & `tonic_textual-1.2.0/tonic_textual/classes/datasetfile.py`

 * *Files identical despite different names*

### Comparing `tonic_textual-1.1.0/tonic_textual/classes/httpclient.py` & `tonic_textual-1.2.0/tonic_textual/classes/httpclient.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import requests
 from urllib3.exceptions import InsecureRequestWarning
 
-from tonic_textual.classes.tonic_exception import LicenseInvalid
+from tonic_textual.classes.tonic_exception import ErrorWhenDownloadFile, FileNotReadyForDownload, LicenseInvalid
 
 requests.packages.urllib3.disable_warnings(category=InsecureRequestWarning)
 
 class HttpClient:
     """Client used to handle requests to the Tonic Textual instance.
 
     Parameters
@@ -16,28 +16,60 @@
         The API token associated to use for the requests.
     """
 
     def __init__(self, base_url: str, api_key: str):
         self.base_url = base_url
         self.headers = {"Authorization": api_key, "User-Agent": "tonic-textual-python-sdk"}
 
-    def http_get_file(self, url: str, session: requests.Session, params: dict={}) -> str:
+    def http_get_file(self, url: str, session: requests.Session, params: dict={}) -> bytes:
         """Makes a get request to get a file.
 
         Parameters
         ----------
         url : str
             URL to make the get request. The URL is appended to self.base_url.
         params: dict
             Passed as the params parameter of the requests.get request.
 
         """
         res = session.get(self.base_url + url, params=params, headers=self.headers, verify=False)
         res.raise_for_status()
-        return res.content.decode('utf-8')
+        return res.content
+    
+    def http_post_download_file(self, url: str, params: dict={}, data={}, additionalHeaders={}) -> bytes:
+        """Makes a POST request to download a file.
+
+        Parameters
+        ----------
+        url : str
+            URL to make the get request. The URL is appended to self.base_url.
+        params: dict
+            Passed as the params parameter of the requests.get request.
+        data: dict
+            Request body
+        additionaHeaders: dict
+            Additional HTTP request headers
+        """
+
+        res = requests.post(
+            self.base_url + url, params=params, json=data, headers=self.headers | additionalHeaders, verify=False
+        )
+        try:
+            res.raise_for_status()
+        except requests.exceptions.HTTPError as err:
+            if err.response.status_code==422:
+                raise LicenseInvalid(err)
+            if err.response.status_code==409:
+                raise FileNotReadyForDownload("File not yet ready for download")
+            if err.response.status_code==500:
+                raise ErrorWhenDownloadFile(err)            
+            else:
+                raise err            
+        
+        return res.content
 
     def http_get(self, url: str, session: requests.Session, params: dict={}):
         """Makes a get request.
 
         Parameters
         ----------
         url : str
```

### Comparing `tonic_textual-1.1.0/tonic_textual/classes/tonic_exception.py` & `tonic_textual-1.2.0/tonic_textual/classes/tonic_exception.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,8 +26,24 @@
 
 class LicenseInvalid(HTTPError):
     """
         Raised when either your license has expired OR you've exceeded your allowed word limit
     """
     def __init__(self, errors):
         super().__init__(str(errors.response.content) or "Invalid Textual license. Please reach out to textual@tonic.ai.")
-        self.errors = errors
+        self.errors = errors
+
+class FileNotReadyForDownload(Exception):
+    """
+        Raised when you make a reques to download a file that is not yet ready for download
+    """
+    def __init__(self, msg):
+        super().__init__(msg)
+
+class ErrorWhenDownloadFile(HTTPError):
+    """
+        Raised when server returns 500 when attempting to download file
+    """
+    def __init__(self, errors):
+        super().__init__("Either error occured while downloading file or the file redaction job was cancelled.")
+        self.errors = errors
+
```

### Comparing `tonic_textual-1.1.0/tonic_textual/services/dataset.py` & `tonic_textual-1.2.0/tonic_textual/services/dataset.py`

 * *Files identical despite different names*

### Comparing `tonic_textual-1.1.0/tonic_textual/services/datasetfile.py` & `tonic_textual-1.2.0/tonic_textual/services/datasetfile.py`

 * *Files identical despite different names*

### Comparing `tonic_textual-1.1.0/PKG-INFO` & `tonic_textual-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tonic-textual
-Version: 1.1.0
+Version: 1.2.0
 Summary: Wrappers around the Tonic Textual API
 Home-page: https://www.tonic.ai/
 License: MIT
 Keywords: tonic.ai,tonic,tonic textual
 Author: Adam Kamor
 Author-email: adam@tonic.ai
 Requires-Python: >=3.7,<4.0
```

