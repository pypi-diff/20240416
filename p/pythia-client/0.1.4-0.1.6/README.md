# Comparing `tmp/pythia_client-0.1.4.tar.gz` & `tmp/pythia_client-0.1.6.tar.gz`

## Comparing `pythia_client-0.1.4.tar` & `pythia_client-0.1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 pythia_client-0.1.4/.python-version
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 pythia_client-0.1.4/CHANGELOG.md
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 pythia_client-0.1.4/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pythia_client-0.1.4/src/pythia_client/__init__.py
--rw-r--r--   0        0        0    17079 2020-02-02 00:00:00.000000 pythia_client-0.1.4/src/pythia_client/client.py
--rw-r--r--   0        0        0     5943 2020-02-02 00:00:00.000000 pythia_client-0.1.4/src/pythia_client/schema.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pythia_client-0.1.4/test/__init__.py
--rw-r--r--   0        0        0     7033 2020-02-02 00:00:00.000000 pythia_client-0.1.4/test/test_client.py
--rw-r--r--   0        0        0    26093 2020-02-02 00:00:00.000000 pythia_client-0.1.4/test/samples/sample1.pdf
--rw-r--r--   0        0        0   217237 2020-02-02 00:00:00.000000 pythia_client-0.1.4/test/samples/sample2.pdf
--rw-r--r--   0        0        0    21457 2020-02-02 00:00:00.000000 pythia_client-0.1.4/test/samples/sample3.pdf
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 pythia_client-0.1.4/.gitignore
--rw-r--r--   0        0        0    11343 2020-02-02 00:00:00.000000 pythia_client-0.1.4/LICENSE
--rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 pythia_client-0.1.4/README.md
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 pythia_client-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     3046 2020-02-02 00:00:00.000000 pythia_client-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 pythia_client-0.1.6/.python-version
+-rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 pythia_client-0.1.6/CHANGELOG.md
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 pythia_client-0.1.6/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pythia_client-0.1.6/src/pythia_client/__init__.py
+-rw-r--r--   0        0        0    20766 2020-02-02 00:00:00.000000 pythia_client-0.1.6/src/pythia_client/client.py
+-rw-r--r--   0        0        0     6153 2020-02-02 00:00:00.000000 pythia_client-0.1.6/src/pythia_client/schema.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pythia_client-0.1.6/test/__init__.py
+-rw-r--r--   0        0        0     8795 2020-02-02 00:00:00.000000 pythia_client-0.1.6/test/test_client.py
+-rw-r--r--   0        0        0    26093 2020-02-02 00:00:00.000000 pythia_client-0.1.6/test/samples/sample1.pdf
+-rw-r--r--   0        0        0   217237 2020-02-02 00:00:00.000000 pythia_client-0.1.6/test/samples/sample2.pdf
+-rw-r--r--   0        0        0    21457 2020-02-02 00:00:00.000000 pythia_client-0.1.6/test/samples/sample3.pdf
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 pythia_client-0.1.6/.gitignore
+-rw-r--r--   0        0        0    11343 2020-02-02 00:00:00.000000 pythia_client-0.1.6/LICENSE
+-rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 pythia_client-0.1.6/README.md
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 pythia_client-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     3046 2020-02-02 00:00:00.000000 pythia_client-0.1.6/PKG-INFO
```

### Comparing `pythia_client-0.1.4/CHANGELOG.md` & `pythia_client-0.1.6/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+#### v0.1.6
+- New intent functions: add_intent, predict_intent, delete_intent. Compatible with `haystack-api` v0.2.1
+
 #### v0.1.4
 - Minor ESR Ticket schema fix
 
 #### v0.1.3
 - Minor modification of Schema for structured data extraction.  Compatible with `haystack-api` v0.2.0
 
 #### v0.1.0
```

### Comparing `pythia_client-0.1.4/src/pythia_client/client.py` & `pythia_client-0.1.6/src/pythia_client/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 Classes:
     APIClient: Client for interacting with the API.
 """
 
 import os
 import json
 import io
-from typing import List, Optional, Literal, Tuple, Union
+from typing import List, Optional, Literal, Tuple, Union, Dict
 from urllib.parse import urljoin
 import requests
 
 from .schema import (
     UploadFileResponse,
     GetFileS3Reponse,
     FilterRequest,
@@ -23,14 +23,17 @@
     DeleteDocResponse,
     QueryRequest,
     QueryResponse,
     DataExtractRequest,
     DataExtractResponse,
     ChatMessage,
     LogIndexingTable,
+    AddIntentResponse,
+    PredictIntentResponse,
+    DeleteIntentResponse,
 )
 
 
 class APIClient:
     """Client for interacting with the API.
 
     This class provides methods for interacting with the API, including
@@ -67,14 +70,17 @@
         self.indexing_tasks_endpoint = urljoin(str(self.url), "files/indexing-tasks")
         self.documents_by_filter_endpoint = urljoin(str(self.url), "documents/filters")
         self.documents_by_s3_key_endpoint = urljoin(str(self.url), "documents/s3-key")
         self.search_endpoint = urljoin(str(self.url), "search/query")
         self.data_extraction_endpoint = urljoin(
             str(self.url), "/data_extraction/extract-structured-data"
         )
+        self.add_intent_endpoint = urljoin(str(self.url), "alie/intent")
+        self.predict_intent_endpoint = urljoin(str(self.url), "alie/intent/predict")
+        self.delete_intent_endpoint = urljoin(str(self.url), "alie/intent")
 
     def query(
         self,
         query: str,
         chat_history: Optional[List[ChatMessage]] = None,
         filters: Optional[FilterRequest] = None,
         group_id: str = None,
@@ -441,7 +447,101 @@
                 self.data_extraction_endpoint, headers=headers, json=payload
             ) as response:
                 if response.status_code == 200:
                     response = DataExtractResponse(**response.json())
                 else:
                     response = None
         return response
+
+    def add_intent(
+        self,
+        intent_data: Dict[str, List[str]],
+    ) -> AddIntentResponse:
+        """Add intent data to the intent prediction engine.
+
+        Args:
+            intent_data: Dict containing intent data.
+
+        Returns:
+            The response from the API as a Pydantic model. You can use reponse.model_dump() to get a Dict. Returns None if the status code is not 200.
+
+        Usage:
+        ```python
+        intent_data = {"greet": ["Hey", "Hello", "Bonjour"], "help": ["I need help", "Show help"]}
+        add_intent_response = client.add_intent(intent_data)
+        add_intent_response.model_dump()
+        ```
+        """
+        with requests.Session() as session:
+            headers = {
+                "X-API-Key": self.api_key,
+            }
+            with session.post(
+                self.add_intent_endpoint, headers=headers, data=json.dumps(intent_data)
+            ) as response:
+                if response.status_code == 200:
+                    response = AddIntentResponse(**response.json())
+                else:
+                    response = None
+        return response
+
+    def predict_intent(
+        self,
+        user_msg: str,
+    ) -> PredictIntentResponse:
+        """Query the API to predict the intent of a user message.
+
+        Args:
+            user_msg: The content of the user message.
+
+        Returns:
+            The response from the API as a Pydantic model. You can use reponse.model_dump() to get a Dict. Returns None if the status code is not 200.
+
+        Usage:
+        ```python
+        intent = client.predict_intent("Hello I want to modify the delivery date of order FR73681920")
+        intent.model_dump()
+        ```
+        """
+        with requests.Session() as session:
+            headers = {
+                "X-API-Key": self.api_key,
+            }
+            with session.get(
+                self.predict_intent_endpoint, headers=headers, params={"user_message": user_msg}
+            ) as response:
+                if response.status_code == 200:
+                    response = PredictIntentResponse(**response.json())
+                else:
+                    response = None
+        return response
+
+    def delete_intent(
+        self,
+        intent_name: str,
+    ) -> DeleteIntentResponse:
+        """Delete the specified intent from the database. Use "*" to delete all intents from the databse (clear the DB).
+
+        Args:
+            intent_name: The name of the intent to delete. Use "*" to delete all intents from the databse (clear the DB).
+
+        Returns:
+            The response from the API as a Pydantic model. You can use reponse.model_dump() to get a Dict. Returns None if the status code is not 200.
+
+        Usage:
+        ```python
+        delete_intent_response = client.delete_intent("greet")
+        delete_intent_response.model_dump()
+        ```
+        """
+        with requests.Session() as session:
+            headers = {
+                "X-API-Key": self.api_key,
+            }
+            with session.delete(
+                self.delete_intent_endpoint, headers=headers, params={"intent_name": intent_name}
+            ) as response:
+                if response.status_code == 200:
+                    response = DeleteIntentResponse(**response.json())
+                else:
+                    response = None
+        return response
```

### Comparing `pythia_client-0.1.4/src/pythia_client/schema.py` & `pythia_client-0.1.6/src/pythia_client/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -255,7 +255,19 @@
     total_tokens: Optional[int] = None
     status: StatusEnum
     timestamp: str
     time_taken: Optional[float] = None
     sk: str
     models: Optional[List[str]] = None
     pk: Optional[str]
+
+
+class PredictIntentResponse(BaseModel):
+    intent: str
+
+
+class AddIntentResponse(BaseModel):
+    Writter: Writer
+
+class DeleteIntentResponse(BaseModel):
+    deleted_intent: str
+    n_deleted_intent_data: int
```

### Comparing `pythia_client-0.1.4/test/samples/sample1.pdf` & `pythia_client-0.1.6/test/samples/sample1.pdf`

 * *Files identical despite different names*

### Comparing `pythia_client-0.1.4/test/samples/sample2.pdf` & `pythia_client-0.1.6/test/samples/sample2.pdf`

 * *Files identical despite different names*

### Comparing `pythia_client-0.1.4/test/samples/sample3.pdf` & `pythia_client-0.1.6/test/samples/sample3.pdf`

 * *Files identical despite different names*

### Comparing `pythia_client-0.1.4/LICENSE` & `pythia_client-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pythia_client-0.1.4/README.md` & `pythia_client-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `pythia_client-0.1.4/pyproject.toml` & `pythia_client-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pythia-client"
-version = "0.1.4"
+version = "0.1.6"
 dependencies = [
     "requests>=2.31",
     "pydantic>=2.6",
 ]
 requires-python = ">=3.11"
 authors = [
   {name = "Corentin Meyer", email = "contact@cmeyer.fr"},
```

### Comparing `pythia_client-0.1.4/PKG-INFO` & `pythia_client-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pythia-client
-Version: 0.1.4
+Version: 0.1.6
 Summary: Client to interact with the Pythia API
 Project-URL: Homepage, https://gitlab.com/ale-gitlab/dto/data-science/cip-bot/project-pythia
 Project-URL: Documentation, https://gitlab.com/ale-gitlab/dto/data-science/cip-bot/project-pythia
 Project-URL: Repository, https://gitlab.com/ale-gitlab/dto/data-science/cip-bot/project-pythia
 Project-URL: Issues, https://gitlab.com/ale-gitlab/dto/data-science/cip-bot/project-pythia/-/issues
 Author-email: Corentin Meyer <contact@cmeyer.fr>
 Maintainer-email: Corentin Meyer <contact@cmeyer.fr>
```

