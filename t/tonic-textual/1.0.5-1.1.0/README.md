# Comparing `tmp/tonic_textual-1.0.5.tar.gz` & `tmp/tonic_textual-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tonic_textual-1.0.5.tar", max compression
+gzip compressed data, was "tonic_textual-1.1.0.tar", max compression
```

## Comparing `tonic_textual-1.0.5.tar` & `tonic_textual-1.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1084 2023-08-21 15:18:32.578537 tonic_textual-1.0.5/LICENSE
--rw-r--r--   0        0        0      598 2024-02-29 20:48:49.919277 tonic_textual-1.0.5/pyproject.toml
--rw-r--r--   0        0        0      972 2023-11-03 19:05:54.671774 tonic_textual-1.0.5/README.md
--rw-r--r--   0        0        0       19 2024-02-28 13:39:57.538020 tonic_textual-1.0.5/tonic_textual/__init__.py
--rw-r--r--   0        0        0     9937 2024-02-29 18:54:52.195478 tonic_textual-1.0.5/tonic_textual/api.py
--rw-r--r--   0        0        0        0 2023-11-03 19:05:54.674583 tonic_textual-1.0.5/tonic_textual/classes/__init__.py
--rw-r--r--   0        0        0      789 2023-11-15 15:30:22.056092 tonic_textual-1.0.5/tonic_textual/classes/api_responses/redaction_response.py
--rw-r--r--   0        0        0      668 2024-02-28 13:39:57.539026 tonic_textual-1.0.5/tonic_textual/classes/api_responses/single_detection_result.py
--rw-r--r--   0        0        0      348 2023-11-03 19:05:54.674583 tonic_textual-1.0.5/tonic_textual/classes/custom_model.py
--rw-r--r--   0        0        0     8219 2023-11-15 15:30:22.057087 tonic_textual-1.0.5/tonic_textual/classes/dataset.py
--rw-r--r--   0        0        0     1633 2023-11-14 22:48:18.528603 tonic_textual-1.0.5/tonic_textual/classes/datasetfile.py
--rw-r--r--   0        0        0       95 2023-11-03 19:05:54.674583 tonic_textual-1.0.5/tonic_textual/classes/generator_config.py
--rw-r--r--   0        0        0     3099 2024-02-29 12:29:23.701386 tonic_textual-1.0.5/tonic_textual/classes/httpclient.py
--rw-r--r--   0        0        0     1084 2024-02-29 12:29:23.701386 tonic_textual-1.0.5/tonic_textual/classes/tonic_exception.py
--rw-r--r--   0        0        0       92 2023-11-03 19:05:54.674583 tonic_textual-1.0.5/tonic_textual/enums/pii_state.py
--rw-r--r--   0        0        0        0 2023-11-03 19:05:54.674583 tonic_textual-1.0.5/tonic_textual/services/__init__.py
--rw-r--r--   0        0        0      610 2023-11-03 19:05:54.674583 tonic_textual-1.0.5/tonic_textual/services/dataset.py
--rw-r--r--   0        0        0      552 2023-11-03 19:05:54.674583 tonic_textual-1.0.5/tonic_textual/services/datasetfile.py
--rw-r--r--   0        0        0     1885 1970-01-01 00:00:00.000000 tonic_textual-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-08-21 15:18:32.578537 tonic_textual-1.1.0/LICENSE
+-rw-r--r--   0        0        0      598 2024-04-16 13:46:53.564799 tonic_textual-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      972 2023-11-03 19:05:54.671774 tonic_textual-1.1.0/README.md
+-rw-r--r--   0        0        0       19 2024-02-28 13:39:57.538020 tonic_textual-1.1.0/tonic_textual/__init__.py
+-rw-r--r--   0        0        0    10966 2024-04-16 13:46:35.575964 tonic_textual-1.1.0/tonic_textual/api.py
+-rw-r--r--   0        0        0        0 2023-11-03 19:05:54.674583 tonic_textual-1.1.0/tonic_textual/classes/__init__.py
+-rw-r--r--   0        0        0      789 2023-11-15 15:30:22.056092 tonic_textual-1.1.0/tonic_textual/classes/api_responses/redaction_response.py
+-rw-r--r--   0        0        0      668 2024-02-28 13:39:57.539026 tonic_textual-1.1.0/tonic_textual/classes/api_responses/single_detection_result.py
+-rw-r--r--   0        0        0      348 2023-11-03 19:05:54.674583 tonic_textual-1.1.0/tonic_textual/classes/custom_model.py
+-rw-r--r--   0        0        0     8219 2024-04-16 13:46:35.576966 tonic_textual-1.1.0/tonic_textual/classes/dataset.py
+-rw-r--r--   0        0        0     1633 2023-11-14 22:48:18.528603 tonic_textual-1.1.0/tonic_textual/classes/datasetfile.py
+-rw-r--r--   0        0        0       95 2023-11-03 19:05:54.674583 tonic_textual-1.1.0/tonic_textual/classes/generator_config.py
+-rw-r--r--   0        0        0     3442 2024-04-16 13:46:35.577964 tonic_textual-1.1.0/tonic_textual/classes/httpclient.py
+-rw-r--r--   0        0        0     1342 2024-04-16 13:46:35.578966 tonic_textual-1.1.0/tonic_textual/classes/tonic_exception.py
+-rw-r--r--   0        0        0       92 2023-11-03 19:05:54.674583 tonic_textual-1.1.0/tonic_textual/enums/pii_state.py
+-rw-r--r--   0        0        0        0 2023-11-03 19:05:54.674583 tonic_textual-1.1.0/tonic_textual/services/__init__.py
+-rw-r--r--   0        0        0      610 2023-11-03 19:05:54.674583 tonic_textual-1.1.0/tonic_textual/services/dataset.py
+-rw-r--r--   0        0        0      552 2023-11-03 19:05:54.674583 tonic_textual-1.1.0/tonic_textual/services/datasetfile.py
+-rw-r--r--   0        0        0     1885 1970-01-01 00:00:00.000000 tonic_textual-1.1.0/PKG-INFO
```

### Comparing `tonic_textual-1.0.5/LICENSE` & `tonic_textual-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tonic_textual-1.0.5/pyproject.toml` & `tonic_textual-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tonic-textual"
-version = "1.0.5"
+version = "1.1.0"
 description = "Wrappers around the Tonic Textual API"
 authors = ["Adam Kamor <adam@tonic.ai>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://www.tonic.ai/"
 keywords = ["tonic.ai", "tonic", "tonic textual"]
```

### Comparing `tonic_textual-1.0.5/README.md` & `tonic_textual-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `tonic_textual-1.0.5/tonic_textual/api.py` & `tonic_textual-1.1.0/tonic_textual/api.py`

 * *Files 14% similar despite different names*

```diff
@@ -137,59 +137,69 @@
             str
                 The string with the redaction removed.
             """
             
             response = self.client.http_post("/api/unredact", data=[redacted_string])            
             return response
     
-    def redact(self, string: str, generatorConfig: GeneratorConfig = dict(), customModels: List[str] = []) -> RedactionResponse:
+    def redact(self, string: str, generatorConfig: GeneratorConfig = dict(), customModels: List[str] = [], random_seed: Optional[int] = None) -> RedactionResponse:
             """Redacts a string. Depending on the configured handling for each sensitive data type, values can be either redacted, synthesized, or ignored.
             
             Parameters
             ----------
             string : str
                 The string to redact.
             
             generatorConfig: GeneratorConfig
                 A dictionary of sensitive data entities. For each entity, indicates whether to redact, synthesize, or ignore it.
     
             customModels: List[str]
                 A list of custom model names to use to identify values to redact. To see the list of custom models that you have access to, use the get_custom_models function.
-
+            
+            random_seed: Optional[int]
+                An optional value to use to override Textual's default random number seeding.  Can be used to ensure that different API calls use the same or different random seeds.
+                
             Returns
             -------
             RedactionResponse
                 The redacted string along with ancillary information.
             """
             
             invalid_pii_states = [v for v in list(generatorConfig.values()) if v not in PiiState._member_names_]
             if(len(invalid_pii_states)>0):
                  raise Exception("Invalid configuration for generatorConfig. The allowed values are Off, Synthesis, and Redaction.")                 
 
             endpoint = "/api/redact"
-            response = self.client.http_post(endpoint, data={"text": string, "generatorConfig": generatorConfig, "customModels": customModels})
+
+            if random_seed is not None:                 
+                response = self.client.http_post(endpoint, data={"text": string, "generatorConfig": generatorConfig, "customModels": customModels}, additionalHeaders={'textual-random-seed':str(random_seed)})
+            else:
+                response = self.client.http_post(endpoint, data={"text": string, "generatorConfig": generatorConfig, "customModels": customModels})
             
             de_id_results = [SingleDetectionResult(x["start"], x["end"], x["label"], x["text"], x["score"]) for x in list(response["deIdentifyResults"])]
 
             return RedactionResponse(response["originalText"], response["redactedText"], response["usage"], de_id_results)
     
-    def redact_json(self, json_data: Union[str, dict], generatorConfig: GeneratorConfig = dict(), customModels: List[str] = []) -> RedactionResponse:   
+    def redact_json(self, json_data: Union[str, dict], generatorConfig: GeneratorConfig = dict(), customModels: List[str] = [], random_seed: Optional[int] = None) -> RedactionResponse:   
         """Redacts the values in a JSON blob. Depending on the configured handling for each sensitive data type, values can be either redacted, synthesized, or ignored.
         
         Parameters
         ----------
         json_string : Union[str, dict]
             The JSON whose values will be redacted.  This can be either a JSON string or a Python dictionary
         
         generatorConfig: GeneratorConfig
             A dictionary of sensitive data entities. For each entity, indicates whether to redact, synthesize, or ignore it.
 
         customModels: List[str]
             A list of custom model names to use to identify values to redact. To see the list of custom models that you have access to, use the get_custom_models function.
 
+        random_seed: Optional[int]
+            An optional value to use to override Textual's default random number seeding.  Can be used to ensure that different API calls use the same or different random seeds.            
+
         Returns
         -------
         RedactionResponse
             The redacted string along with ancillary information.
         """
         
         invalid_pii_states = [v for v in list(generatorConfig.values()) if v not in PiiState._member_names_]
@@ -202,15 +212,18 @@
              payload = {"jsonText": json_data, "generatorConfig": generatorConfig, "customModels": customModels}
         elif isinstance(json_data, dict):
              payload = {"jsonText": json.dumps(json_data), "generatorConfig": generatorConfig, "customModels": customModels}
         else:
             raise Exception(f'redact_json must receive either a JSON blob as a string or dict().  You passed in type {type(json_data)} which is not supported')
         
         try:
-            response = self.client.http_post(endpoint, data=payload)
+            if random_seed is not None:
+                response = self.client.http_post(endpoint, data=payload, additionalHeaders={'textual-random-seed':str(random_seed)})
+            else:
+                response = self.client.http_post(endpoint, data=payload)
         except requests.exceptions.HTTPError as e:
              if e.response.status_code==400:                  
                   raise InvalidJsonForRedactionRequest(e.response.text)
              raise e
         
         de_id_results = [SingleDetectionResult(x["start"], x["end"], x["label"], x["text"], x["score"], x["jsonPath"]) for x in list(response["deIdentifyResults"])]
```

### Comparing `tonic_textual-1.0.5/tonic_textual/classes/api_responses/redaction_response.py` & `tonic_textual-1.1.0/tonic_textual/classes/api_responses/redaction_response.py`

 * *Files identical despite different names*

### Comparing `tonic_textual-1.0.5/tonic_textual/classes/api_responses/single_detection_result.py` & `tonic_textual-1.1.0/tonic_textual/classes/api_responses/single_detection_result.py`

 * *Files identical despite different names*

### Comparing `tonic_textual-1.0.5/tonic_textual/classes/dataset.py` & `tonic_textual-1.1.0/tonic_textual/classes/dataset.py`

 * *Files identical despite different names*

### Comparing `tonic_textual-1.0.5/tonic_textual/classes/datasetfile.py` & `tonic_textual-1.1.0/tonic_textual/classes/datasetfile.py`

 * *Files identical despite different names*

### Comparing `tonic_textual-1.0.5/tonic_textual/classes/httpclient.py` & `tonic_textual-1.1.0/tonic_textual/classes/httpclient.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import requests
 from urllib3.exceptions import InsecureRequestWarning
 
+from tonic_textual.classes.tonic_exception import LicenseInvalid
+
 requests.packages.urllib3.disable_warnings(category=InsecureRequestWarning)
 
 class HttpClient:
     """Client used to handle requests to the Tonic Textual instance.
 
     Parameters
     ----------
@@ -44,30 +46,38 @@
             Passed as the params parameter of the requests.get request.
 
         """
         res = session.get(self.base_url + url, params=params, headers=self.headers, verify=False)
         res.raise_for_status()
         return res.json()
 
-    def http_post(self, url, params={}, data={}, files={}):
+    def http_post(self, url, params={}, data={}, files={}, additionalHeaders={}):
         """Make a post request.
 
         Parameters
         ----------
         url : str
             URL to make the post request. The URL is appended to self.base_url.
         params: dict
             Passed as the params parameter of the requests.post request.
         data: dict
             Passed as the data parameter of the requests.post request.
-        """
+        """           
+
         res = requests.post(
-            self.base_url + url, params=params, json=data, headers=self.headers, verify=False, files=files
+            self.base_url + url, params=params, json=data, headers=self.headers | additionalHeaders, verify=False, files=files
         )
-        res.raise_for_status()
+        try:
+            res.raise_for_status()
+        except requests.exceptions.HTTPError as err:
+            if err.response.status_code==422:
+                raise LicenseInvalid(err)
+            else:
+                raise err            
+        
         return res.json()
 
     def http_put(self, url, params={}, data={}, files={}):
         """Makes a put request.
 
         Parameters
         ----------
```

### Comparing `tonic_textual-1.0.5/tonic_textual/classes/tonic_exception.py` & `tonic_textual-1.1.0/tonic_textual/classes/tonic_exception.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,9 +18,16 @@
         self.errors = errors
 
 class InvalidJsonForRedactionRequest(Exception):
     """
         Raised when the JSON redaction request contains invalid JSON
     """
     def __init__(self, msg):
-        # Call the base class constructor with the parameters it needs
-        super().__init__(msg)
+        super().__init__(msg)
+
+class LicenseInvalid(HTTPError):
+    """
+        Raised when either your license has expired OR you've exceeded your allowed word limit
+    """
+    def __init__(self, errors):
+        super().__init__(str(errors.response.content) or "Invalid Textual license. Please reach out to textual@tonic.ai.")
+        self.errors = errors
```

### Comparing `tonic_textual-1.0.5/tonic_textual/services/dataset.py` & `tonic_textual-1.1.0/tonic_textual/services/dataset.py`

 * *Files identical despite different names*

### Comparing `tonic_textual-1.0.5/tonic_textual/services/datasetfile.py` & `tonic_textual-1.1.0/tonic_textual/services/datasetfile.py`

 * *Files identical despite different names*

### Comparing `tonic_textual-1.0.5/PKG-INFO` & `tonic_textual-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tonic-textual
-Version: 1.0.5
+Version: 1.1.0
 Summary: Wrappers around the Tonic Textual API
 Home-page: https://www.tonic.ai/
 License: MIT
 Keywords: tonic.ai,tonic,tonic textual
 Author: Adam Kamor
 Author-email: adam@tonic.ai
 Requires-Python: >=3.7,<4.0
```

