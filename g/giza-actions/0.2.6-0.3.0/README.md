# Comparing `tmp/giza_actions-0.2.6.tar.gz` & `tmp/giza_actions-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "giza_actions-0.2.6.tar", max compression
+gzip compressed data, was "giza_actions-0.3.0.tar", max compression
```

## Comparing `giza_actions-0.2.6.tar` & `giza_actions-0.3.0.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     1074 2024-04-03 15:29:00.127403 giza_actions-0.2.6/LICENSE
--rw-r--r--   0        0        0     3529 2024-04-03 15:29:00.127403 giza_actions-0.2.6/README.md
--rw-r--r--   0        0        0      243 2024-04-03 15:29:00.135403 giza_actions-0.2.6/giza_actions/__init__.py
--rw-r--r--   0        0        0     5915 2024-04-03 15:29:00.135403 giza_actions-0.2.6/giza_actions/action.py
--rw-r--r--   0        0        0      542 2024-04-03 15:29:00.135403 giza_actions-0.2.6/giza_actions/deployments.py
--rw-r--r--   0        0        0      225 2024-04-03 15:29:00.135403 giza_actions-0.2.6/giza_actions/logger.py
--rw-r--r--   0        0        0     3051 2024-04-03 15:29:00.135403 giza_actions-0.2.6/giza_actions/logging.yaml
--rw-r--r--   0        0        0    14203 2024-04-03 15:29:00.135403 giza_actions-0.2.6/giza_actions/model.py
--rw-r--r--   0        0        0      519 2024-04-03 15:29:00.135403 giza_actions-0.2.6/giza_actions/task.py
--rw-r--r--   0        0        0     1597 2024-04-03 15:29:00.135403 giza_actions-0.2.6/giza_actions/utils.py
--rw-r--r--   0        0        0     1077 2024-04-03 15:29:00.139403 giza_actions-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     4419 1970-01-01 00:00:00.000000 giza_actions-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-04-16 09:59:57.087231 giza_actions-0.3.0/LICENSE
+-rw-r--r--   0        0        0     6338 2024-04-16 09:59:57.087231 giza_actions-0.3.0/README.md
+-rw-r--r--   0        0        0      243 2024-04-16 09:59:57.099231 giza_actions-0.3.0/giza_actions/__init__.py
+-rw-r--r--   0        0        0     5906 2024-04-16 09:59:57.099231 giza_actions-0.3.0/giza_actions/action.py
+-rw-r--r--   0        0        0    17714 2024-04-16 09:59:57.099231 giza_actions-0.3.0/giza_actions/agent.py
+-rw-r--r--   0        0        0      601 2024-04-16 09:59:57.099231 giza_actions-0.3.0/giza_actions/deployments.py
+-rw-r--r--   0        0        0      225 2024-04-16 09:59:57.099231 giza_actions-0.3.0/giza_actions/logger.py
+-rw-r--r--   0        0        0     3051 2024-04-16 09:59:57.099231 giza_actions-0.3.0/giza_actions/logging.yaml
+-rw-r--r--   0        0        0    15596 2024-04-16 09:59:57.099231 giza_actions-0.3.0/giza_actions/model.py
+-rw-r--r--   0        0        0      519 2024-04-16 09:59:57.099231 giza_actions-0.3.0/giza_actions/task.py
+-rw-r--r--   0        0        0     1906 2024-04-16 09:59:57.099231 giza_actions-0.3.0/giza_actions/utils.py
+-rw-r--r--   0        0        0     1282 2024-04-16 09:59:57.103231 giza_actions-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     7417 1970-01-01 00:00:00.000000 giza_actions-0.3.0/PKG-INFO
```

### Comparing `giza_actions-0.2.6/LICENSE` & `giza_actions-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `giza_actions-0.2.6/giza_actions/action.py` & `giza_actions-0.3.0/giza_actions/action.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     PREFECT_UI_URL,
     update_current_profile,
 )
 from prefect.utilities.asyncutils import sync_compatible  # noqa: E402
 from rich.console import Console  # noqa: E402
 from rich.panel import Panel  # noqa: E402
 
-from giza_actions.__init__ import __module_path__  # noqa: E402
+from giza_actions import __module_path__  # noqa: E402
 
 
 class Action:
     """
     A class to represent an Action.
 
     Attributes:
```

### Comparing `giza_actions-0.2.6/giza_actions/logging.yaml` & `giza_actions-0.3.0/giza_actions/logging.yaml`

 * *Files identical despite different names*

### Comparing `giza_actions-0.2.6/giza_actions/model.py` & `giza_actions-0.3.0/giza_actions/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,40 +1,44 @@
 import logging
 from pathlib import Path
 from typing import Dict, Optional
 
 import numpy as np
-import onnxruntime as ort
 import onnx
+import onnxruntime as ort
 import requests
 from giza import API_HOST
-from giza.client import ApiClient, ModelsClient, VersionsClient
+from giza.client import ApiClient, EndpointsClient, ModelsClient, VersionsClient
 from giza.utils.enums import Framework, VersionStatus
 from osiris.app import (
     create_tensor_from_array,
     deserialize,
     load_data,
     serialize,
     serializer,
 )
 
 from giza_actions.utils import get_endpoint_uri
 
+logger = logging.getLogger(__name__)
+
 
 class GizaModel:
     """
     A class to manage the lifecycle and predictions of models using both local ONNX runtime sessions and
     remote deployments via the Giza SDK.
 
     Attributes:
         session (ort.InferenceSession | None): An ONNX runtime inference session for local model predictions.
         model_client (ModelsClient): Client to interact with the models endpoint of the Giza API.
         version_client (VersionsClient): Client to interact with the versions endpoint of the Giza API.
         api_client (ApiClient): General client for interacting with the Giza API.
         uri (str): The URI for making prediction requests to a deployed model.
+        model_id (int): The unique identifier of the model in the Giza platform.
+        version_id (int): The version number of the model in the Giza platform.
 
     Args:
         model_path (Optional[str]): The file path to a local ONNX model. Defaults to None.
         id (Optional[int]): The unique identifier of the model in the Giza platform. Defaults to None.
         version (Optional[int]): The version number of the model in the Giza platform. Defaults to None.
         output_path (Optional[str]): The file path where the downloaded model should be saved. Defaults to None.
 
@@ -46,56 +50,80 @@
         self,
         model_path: Optional[str] = None,
         id: Optional[int] = None,
         version: Optional[int] = None,
         output_path: Optional[str] = None,
     ):
         if model_path is None and id is None and version is None:
-            raise ValueError(
-                "Either model_path or id and version must be provided.")
+            raise ValueError("Either model_path or id and version must be provided.")
 
         if model_path is None and (id is None or version is None):
             raise ValueError("Both id and version must be provided.")
 
         if model_path and (id or version):
-            raise ValueError(
-                "Either model_path or id and version must be provided.")
+            raise ValueError("Either model_path or id and version must be provided.")
 
         if model_path and id and version:
             raise ValueError(
                 "Only one of model_path or id and version should be provided."
             )
 
         if model_path:
             self.session = ort.InferenceSession(model_path)
         elif id and version:
+            self.model_id = id
+            self.version_id = version
             self.model_client = ModelsClient(API_HOST)
             self.version_client = VersionsClient(API_HOST)
             self.api_client = ApiClient(API_HOST)
+            self.endpoints_client = EndpointsClient(API_HOST)
             self._get_credentials()
             self.model = self._get_model(id)
             self.version = self._get_version(version)
             self.session = self._set_session()
             self.framework = self.version.framework
-            self.uri = self._retrieve_uri(version)
+            self.uri = self._retrieve_uri()
+            self.endpoint_id = self._get_endpoint_id()
             if output_path:
                 self._download_model(output_path)
 
-    def _retrieve_uri(self, version_id: int):
+    def _get_endpoint_id(self):
+        """
+        Retrieves the endpoint id for the deployed model.
+
+        Returns:
+            The endpoint id for the deployed model.
+        """
+        deployments_list = self.endpoints_client.list(
+            params={
+                "model_id": self.model.id,
+                "version_id": self.version.version,
+                "is_active": True,
+            }
+        )
+
+        if len(deployments_list.root) == 1:
+            return deployments_list.root[0].id
+        elif len(deployments_list.root) > 1:
+            raise ValueError("Multiple versions deployed for the same model")
+        else:
+            raise ValueError("No active deployments found")
+
+    def _retrieve_uri(self):
         """
         Retrieves the URI for making prediction requests to a deployed model.
 
         Args:
             version_id (int): The version number of the model.
 
         Returns:
             The URI for making prediction requests to the deployed model.
         """
         # Different URI per framework
-        uri = get_endpoint_uri(self.model.id, version_id)
+        uri = get_endpoint_uri(self.model.id, self.version.version)
         if self.framework == Framework.CAIRO:
             return f"{uri}/cairo_run"
         else:
             return f"{uri}/predict"
 
     def _get_model(self, model_id: int):
         """
@@ -132,20 +160,21 @@
         if self.version.status != VersionStatus.COMPLETED:
             raise ValueError(
                 f"Model version status is not completed {self.version.status}"
             )
 
         try:
             onnx_model = self.version_client.download_original(
-                self.model.id, self.version.version)
+                self.model.id, self.version.version
+            )
 
             return ort.InferenceSession(onnx_model)
 
         except Exception as e:
-            print(f"Could not download model: {e}")
+            logger.info(f"Could not download model: {e}")
             return None
 
     def _download_model(self, output_path: str):
         """
         Downloads the model specified by model id and version id to the given output_path.
 
         Args:
@@ -157,27 +186,28 @@
 
         if self.version.status != VersionStatus.COMPLETED:
             raise ValueError(
                 f"Model version status is not completed {self.version.status}"
             )
 
         onnx_model = self.version_client.download_original(
-            self.model.id, self.version.version)
+            self.model.id, self.version.version
+        )
 
-        print("ONNX model is ready, downloading! ✅")
+        logger.info("ONNX model is ready, downloading! ✅")
 
         if ".onnx" in output_path:
             save_path = Path(output_path)
         else:
             save_path = Path(f"{output_path}/{self.model.name}.onnx")
 
         with open(save_path, "wb") as f:
             f.write(onnx_model)
 
-        print(f"ONNX model saved at: {save_path} ✅")
+        logger.info(f"ONNX model saved at: {save_path} ✅")
 
     def _get_credentials(self):
         """
         Retrieves and sets the necessary credentials for API access.
         """
         self.api_client.retrieve_token()
         self.api_client.retrieve_api_key()
@@ -186,14 +216,15 @@
         self,
         input_file: Optional[str] = None,
         input_feed: Optional[Dict] = None,
         verifiable: bool = False,
         fp_impl="FP16x16",
         custom_output_dtype: Optional[str] = None,
         job_size: str = "M",
+        dry_run: bool = False,
     ):
         """
         Makes a prediction using either a local ONNX session or a remote deployed model, depending on the
         instance configuration.
 
         Args:
             input_file (Optional[str]): The path to the input file for prediction. Defaults to None.
@@ -206,60 +237,65 @@
             A tuple (predictions, request_id) where predictions is the result of the prediction and request_id
             is the identifier of the prediction request if verifiable computation is used, otherwise None.
 
         Raises:
             ValueError: If required parameters are not provided or the session is not initialized.
         """
         try:
+            logger.info("Predicting")
             if verifiable:
                 if not self.uri:
                     raise ValueError("Model has not been deployed")
 
                 # Non common arguments should be named parameters
                 payload = self._format_inputs_for_framework(
                     input_file, input_feed, fp_impl=fp_impl, job_size=job_size
                 )
 
+                if dry_run:
+                    payload["dry_run"] = True
+
                 response = requests.post(self.uri, json=payload)
 
                 try:
                     response.raise_for_status()
                 except requests.exceptions.HTTPError as e:
-                    logging.error(f"An error occurred in predict: {e}")
+                    logger.error(f"An error occurred in predict: {e}")
                     error_message = f"Deployment predict error: {response.text}"
-                    logging.error(error_message)
+                    logger.error(error_message)
                     raise e
 
                 body = response.json()
                 serialized_output = body["result"]
-                request_id =  body["request_id"]
+                request_id = body["request_id"]
 
                 if self.framework == Framework.CAIRO:
-                    logging.info("Serialized: ", serialized_output)
+                    logger.info("Serialized: %s", serialized_output)
 
                     if custom_output_dtype is None:
                         output_dtype = self._get_output_dtype()
                     else:
                         output_dtype = custom_output_dtype
 
-                    preds = self._parse_cairo_response(
-                        serialized_output, output_dtype)
+                    logger.debug("Output dtype: %s", output_dtype)
+                    preds = self._parse_cairo_response(serialized_output, output_dtype)
                 elif self.framework == Framework.EZKL:
                     preds = np.array(serialized_output[0])
                 return (preds, request_id)
-
+            # Here we are returning different things, Tuple vs np.ndarray
+            # TODO: make it consistent
             else:
                 if self.session is None:
                     raise ValueError("Session is not initialized.")
                 if input_feed is None:
                     raise ValueError("Input feed is none")
                 preds = self.session.run(None, input_feed)[0]
                 return preds
         except Exception as e:
-            logging.error(f"An error occurred in predict: {e}")
+            logger.error(f"An error occurred in predict: {e}")
             raise e
 
     def _format_inputs_for_framework(self, *args, **kwargs):
         """
         Formats the inputs for a prediction request for a specific framework.
 
         Args:
```

### Comparing `giza_actions-0.2.6/giza_actions/task.py` & `giza_actions-0.3.0/giza_actions/task.py`

 * *Files identical despite different names*

### Comparing `giza_actions-0.2.6/giza_actions/utils.py` & `giza_actions-0.3.0/giza_actions/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 import logging
 
 import requests
 from giza import API_HOST
 from giza.client import EndpointsClient, WorkspaceClient
 
 logger = logging.getLogger(__name__)
@@ -50,7 +51,22 @@
         params={"model_id": model_id, "version_id": version_id, "is_active": True}
     )
 
     if len(deployments_list.root) == 1:
         return deployments_list.root[0].uri
     else:
         return None
+
+
+def read_json(file_path: str):
+    """
+    Read the JSON file from the specified path and return the
+    JSON data.
+
+    Args:
+        file_path (str): The path to the JSON file.
+
+    Returns:
+        dict: The JSON data.
+    """
+    with open(file_path) as file:
+        return json.load(file)
```

### Comparing `giza_actions-0.2.6/pyproject.toml` & `giza_actions-0.3.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "giza-actions"
-version = "0.2.6"
+version = "0.3.0"
 
 description = "A Python SDK for Giza platform"
 authors = [
     "Francisco Algaba <fran@gizatech.xyz>",
     "Raphael Doukhan <raphael@gizatech.xyz>",
     "Gonzalo Mellizo-Soto <gonzalo@gizatech.xyz>"]
 readme = "README.md"
@@ -18,16 +18,22 @@
 onnx = "^1.15.0"
 httpx = "^0.25.1"
 onnxruntime = "^1.16.3"
 prefect-gcp = "^0.5.4"
 pyyaml = "^6.0.1"
 prefect-docker = "^0.4.1"
 distlib = "^0.3.8"
-giza-cli = ">=0.13.0,<1.0.0"
+giza-cli = ">=0.15.0,<1.0.0"
 giza-osiris = ">=0.2.6,<1.0.0"
+loguru = "^0.7.2"
+eth-ape = {version = "^0.7.10", optional = true }
+ape-etherscan = {version = "^0.7.2", optional = true }
+
+[tool.poetry.extras]
+agents = ["eth-ape", "ape-etherscan"]
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.5"
 
 [tool.poetry.group.dev.dependencies]
 pillow = "^10.1.0"
 opencv-python = "^4.8.1.78"
@@ -37,14 +43,15 @@
 mypy = "^1.7.1"
 ruff = "^0.1.6"
 lazydocs = "^0.4.8"
 pre-commit = "^3.5.0"
 torch = "^2.1.2"
 torchvision = "^0.16.2"
 matplotlib = "^3.8.2"
+ipykernel = "^6.29.4"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
```

