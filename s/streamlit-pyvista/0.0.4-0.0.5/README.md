# Comparing `tmp/streamlit_pyvista-0.0.4.tar.gz` & `tmp/streamlit_pyvista-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit_pyvista-0.0.4.tar", max compression
+gzip compressed data, was "streamlit_pyvista-0.0.5.tar", max compression
```

## Comparing `streamlit_pyvista-0.0.4.tar` & `streamlit_pyvista-0.0.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      104 2024-04-05 09:02:25.101594 streamlit_pyvista-0.0.4/README.md
--rw-r--r--   0        0        0      650 2024-04-05 09:02:30.255535 streamlit_pyvista-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     5972 2024-04-05 09:02:25.102594 streamlit_pyvista-0.0.4/streamlit_pyvista/MeshViewerComponent.py
--rw-r--r--   0        0        0       89 2024-04-05 09:02:25.102594 streamlit_pyvista-0.0.4/streamlit_pyvista/__init__.py
--rw-r--r--   0        0        0    17989 2024-04-05 09:02:25.102594 streamlit_pyvista-0.0.4/streamlit_pyvista/trame_viewer.py
--rw-r--r--   0        0        0      208 2024-04-05 09:02:25.102594 streamlit_pyvista-0.0.4/streamlit_pyvista/utils.py
--rw-r--r--   0        0        0      941 1970-01-01 00:00:00.000000 streamlit_pyvista-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      104 2024-04-16 16:04:25.476831 streamlit_pyvista-0.0.5/README.md
+-rw-r--r--   0        0        0      659 2024-04-16 16:04:31.117806 streamlit_pyvista-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     6070 2024-04-16 16:04:25.478831 streamlit_pyvista-0.0.5/streamlit_pyvista/MeshViewerComponent.py
+-rw-r--r--   0        0        0       89 2024-04-16 16:04:25.478831 streamlit_pyvista-0.0.5/streamlit_pyvista/__init__.py
+-rw-r--r--   0        0        0    24891 2024-04-16 16:04:25.478831 streamlit_pyvista-0.0.5/streamlit_pyvista/trame_viewer.py
+-rw-r--r--   0        0        0      208 2024-04-16 16:04:25.478831 streamlit_pyvista-0.0.5/streamlit_pyvista/utils.py
+-rw-r--r--   0        0        0     1005 1970-01-01 00:00:00.000000 streamlit_pyvista-0.0.5/PKG-INFO
```

### Comparing `streamlit_pyvista-0.0.4/pyproject.toml` & `streamlit_pyvista-0.0.5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [tool.poetry]
 name = "streamlit-pyvista"
-version = "0.0.4"
+version = "0.0.5"
 description = ""
 authors = ["Maxime Rochat <rochat.max@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9.12"
-aiohttp = "3.9.3"
-pyvista = "0.43.3"
+aiohttp = "^3.9.3"
+pyvista = "^0.43.3"
 streamlit = "^1.17.0"
-trame = "3.5.2"
-trame-client = "2.16.1"
-trame-plotly = "3.0.2"
-trame-server = "2.17.2"
-trame-vtk = "2.8.5"
-trame-vuetify = "2.4.2"
+trame = "^3.5.2"
+trame-client = "^2.16.1"
+trame-plotly = "^3.0.2"
+trame-server = "^2.17.2"
+trame-vtk = "^2.8.5"
+trame-vuetify = "^2.4.2"
 protobuf="<=4.25.3"
 pytest = ">=7.2.1"
-requests = "2.29.0"
+requests = "^2.29.0"
 
 
 [build-system]
 requires = ["poetry-core", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
```

### Comparing `streamlit_pyvista-0.0.4/streamlit_pyvista/MeshViewerComponent.py` & `streamlit_pyvista-0.0.5/streamlit_pyvista/MeshViewerComponent.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 import streamlit.components.v1 as components
 import requests
 import json
 import subprocess
 import threading
 
+
+
 from .utils import is_localhost
 
 root_logger = logging.getLogger("solidipes")
 root_logger.propagate = True
 root_logger.setLevel(logging.DEBUG)
 if "FULL_SOLIDIPES_LOG" not in os.environ:
     root_logger.setLevel(logging.INFO)
@@ -135,14 +137,17 @@
             "width": self.width,
             "height": self.height
         }
         headers = {"Content-Type": "application/json"}
 
         # Check in the response if any action is necessary such as make the iframe bigger
         response = requests.get(url, data=json.dumps(data), headers=headers, timeout=2000)
-        resp_body = response.json()
-        if "request_space" in resp_body:
-            self.height = resp_body["request_space"]
+        try:
+            resp_body = response.json()
+            if "request_space" in resp_body:
+                self.height = resp_body["request_space"]
+        except requests.exceptions.JSONDecodeError:
+            return
 
     def show(self):
         """ Render the streamlit component """
         components.iframe("http://127.0.0.1:8080/index.html", height=self.height)  # , scrolling=True
```

### Comparing `streamlit_pyvista-0.0.4/PKG-INFO` & `streamlit_pyvista-0.0.5/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: streamlit-pyvista
-Version: 0.0.4
+Version: 0.0.5
 Summary: 
 Author: Maxime Rochat
 Author-email: rochat.max@gmail.com
 Requires-Python: >=3.9.12,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: aiohttp (==3.9.3)
+Requires-Dist: aiohttp (>=3.9.3,<4.0.0)
 Requires-Dist: protobuf (<=4.25.3)
 Requires-Dist: pytest (>=7.2.1)
-Requires-Dist: pyvista (==0.43.3)
-Requires-Dist: requests (==2.29.0)
+Requires-Dist: pyvista (>=0.43.3,<0.44.0)
+Requires-Dist: requests (>=2.29.0,<3.0.0)
 Requires-Dist: streamlit (>=1.17.0,<2.0.0)
-Requires-Dist: trame (==3.5.2)
-Requires-Dist: trame-client (==2.16.1)
-Requires-Dist: trame-plotly (==3.0.2)
-Requires-Dist: trame-server (==2.17.2)
-Requires-Dist: trame-vtk (==2.8.5)
-Requires-Dist: trame-vuetify (==2.4.2)
+Requires-Dist: trame (>=3.5.2,<4.0.0)
+Requires-Dist: trame-client (>=2.16.1,<3.0.0)
+Requires-Dist: trame-plotly (>=3.0.2,<4.0.0)
+Requires-Dist: trame-server (>=2.17.2,<3.0.0)
+Requires-Dist: trame-vtk (>=2.8.5,<3.0.0)
+Requires-Dist: trame-vuetify (>=2.4.2,<3.0.0)
 Description-Content-Type: text/markdown
 
 # streamlit-pyvista
 A Streamlit component that allow support for new pyvista viewer backend : Trame.
```

