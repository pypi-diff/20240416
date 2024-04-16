# Comparing `tmp/toolforge-weld-1.4.0.tar.gz` & `tmp/toolforge_weld-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toolforge-weld-1.4.0.tar", last modified: Mon Oct  9 08:42:39 2023, max compression
+gzip compressed data, was "toolforge_weld-1.5.0.tar", last modified: Tue Apr 16 08:40:05 2024, max compression
```

## Comparing `toolforge-weld-1.4.0.tar` & `toolforge_weld-1.5.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-09 08:42:39.971706 toolforge-weld-1.4.0/
--rw-rw-rw-   0 root         (0) root         (0)    34524 2023-10-09 08:42:34.000000 toolforge-weld-1.4.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      788 2023-10-09 08:42:39.971706 toolforge-weld-1.4.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       78 2023-10-09 08:42:34.000000 toolforge-weld-1.4.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      449 2023-10-09 08:42:34.000000 toolforge-weld-1.4.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-10-09 08:42:39.971706 toolforge-weld-1.4.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      982 2023-10-09 08:42:34.000000 toolforge-weld-1.4.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-09 08:42:39.967706 toolforge-weld-1.4.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)     2276 2023-10-09 08:42:34.000000 toolforge-weld-1.4.0/tests/test_api_client.py
--rw-rw-rw-   0 root         (0) root         (0)     2642 2023-10-09 08:42:34.000000 toolforge-weld-1.4.0/tests/test_config.py
--rw-rw-rw-   0 root         (0) root         (0)      385 2023-10-09 08:42:34.000000 toolforge-weld-1.4.0/tests/test_kubernetes.py
--rw-rw-rw-   0 root         (0) root         (0)     4816 2023-10-09 08:42:34.000000 toolforge-weld-1.4.0/tests/test_kubernetes_config.py
--rw-rw-rw-   0 root         (0) root         (0)      330 2023-10-09 08:42:34.000000 toolforge-weld-1.4.0/tests/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-09 08:42:39.971706 toolforge-weld-1.4.0/toolforge_weld/
--rw-rw-rw-   0 root         (0) root         (0)      176 2023-10-09 08:42:34.000000 toolforge-weld-1.4.0/toolforge_weld/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6312 2023-10-09 08:42:34.000000 toolforge-weld-1.4.0/toolforge_weld/api_client.py
--rw-rw-rw-   0 root         (0) root         (0)     3435 2023-10-09 08:42:34.000000 toolforge-weld-1.4.0/toolforge_weld/config.py
--rw-rw-rw-   0 root         (0) root         (0)     1598 2023-10-09 08:42:34.000000 toolforge-weld-1.4.0/toolforge_weld/errors.py
--rw-rw-rw-   0 root         (0) root         (0)     9083 2023-10-09 08:42:34.000000 toolforge-weld-1.4.0/toolforge_weld/kubernetes.py
--rw-rw-rw-   0 root         (0) root         (0)     4935 2023-10-09 08:42:34.000000 toolforge-weld-1.4.0/toolforge_weld/kubernetes_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-09 08:42:39.971706 toolforge-weld-1.4.0/toolforge_weld/logs/
--rw-rw-rw-   0 root         (0) root         (0)      583 2023-10-09 08:42:34.000000 toolforge-weld-1.4.0/toolforge_weld/logs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2154 2023-10-09 08:42:34.000000 toolforge-weld-1.4.0/toolforge_weld/logs/kubernetes.py
--rw-rw-rw-   0 root         (0) root         (0)      544 2023-10-09 08:42:34.000000 toolforge-weld-1.4.0/toolforge_weld/logs/source.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-10-09 08:42:34.000000 toolforge-weld-1.4.0/toolforge_weld/py.typed
--rw-rw-rw-   0 root         (0) root         (0)      462 2023-10-09 08:42:34.000000 toolforge-weld-1.4.0/toolforge_weld/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-09 08:42:39.971706 toolforge-weld-1.4.0/toolforge_weld.egg-info/
--rw-r--r--   0 root         (0) root         (0)      788 2023-10-09 08:42:39.000000 toolforge-weld-1.4.0/toolforge_weld.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      668 2023-10-09 08:42:39.000000 toolforge-weld-1.4.0/toolforge_weld.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-09 08:42:39.000000 toolforge-weld-1.4.0/toolforge_weld.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       42 2023-10-09 08:42:39.000000 toolforge-weld-1.4.0/toolforge_weld.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-10-09 08:42:39.000000 toolforge-weld-1.4.0/toolforge_weld.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 08:40:05.290944 toolforge_weld-1.5.0/
+-rw-rw-rw-   0 root         (0) root         (0)    34524 2024-04-16 08:40:02.000000 toolforge_weld-1.5.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      789 2024-04-16 08:40:05.290944 toolforge_weld-1.5.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       78 2024-04-16 08:40:02.000000 toolforge_weld-1.5.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      270 2024-04-16 08:40:02.000000 toolforge_weld-1.5.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-16 08:40:05.290944 toolforge_weld-1.5.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      983 2024-04-16 08:40:02.000000 toolforge_weld-1.5.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 08:40:05.290944 toolforge_weld-1.5.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2276 2024-04-16 08:40:02.000000 toolforge_weld-1.5.0/tests/test_api_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     2642 2024-04-16 08:40:02.000000 toolforge_weld-1.5.0/tests/test_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     1643 2024-04-16 08:40:02.000000 toolforge_weld-1.5.0/tests/test_kubernetes.py
+-rw-rw-rw-   0 root         (0) root         (0)     4816 2024-04-16 08:40:02.000000 toolforge_weld-1.5.0/tests/test_kubernetes_config.py
+-rw-rw-rw-   0 root         (0) root         (0)      330 2024-04-16 08:40:02.000000 toolforge_weld-1.5.0/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 08:40:05.290944 toolforge_weld-1.5.0/toolforge_weld/
+-rw-rw-rw-   0 root         (0) root         (0)      174 2024-04-16 08:40:02.000000 toolforge_weld-1.5.0/toolforge_weld/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6405 2024-04-16 08:40:02.000000 toolforge_weld-1.5.0/toolforge_weld/api_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     3435 2024-04-16 08:40:02.000000 toolforge_weld-1.5.0/toolforge_weld/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     1598 2024-04-16 08:40:02.000000 toolforge_weld-1.5.0/toolforge_weld/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     9816 2024-04-16 08:40:02.000000 toolforge_weld-1.5.0/toolforge_weld/kubernetes.py
+-rw-rw-rw-   0 root         (0) root         (0)     4935 2024-04-16 08:40:02.000000 toolforge_weld-1.5.0/toolforge_weld/kubernetes_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 08:40:05.290944 toolforge_weld-1.5.0/toolforge_weld/logs/
+-rw-rw-rw-   0 root         (0) root         (0)      584 2024-04-16 08:40:02.000000 toolforge_weld-1.5.0/toolforge_weld/logs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2154 2024-04-16 08:40:02.000000 toolforge_weld-1.5.0/toolforge_weld/logs/kubernetes.py
+-rw-rw-rw-   0 root         (0) root         (0)      544 2024-04-16 08:40:02.000000 toolforge_weld-1.5.0/toolforge_weld/logs/source.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-16 08:40:02.000000 toolforge_weld-1.5.0/toolforge_weld/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)      462 2024-04-16 08:40:02.000000 toolforge_weld-1.5.0/toolforge_weld/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 08:40:05.290944 toolforge_weld-1.5.0/toolforge_weld.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      789 2024-04-16 08:40:05.000000 toolforge_weld-1.5.0/toolforge_weld.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      668 2024-04-16 08:40:05.000000 toolforge_weld-1.5.0/toolforge_weld.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 08:40:05.000000 toolforge_weld-1.5.0/toolforge_weld.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2024-04-16 08:40:05.000000 toolforge_weld-1.5.0/toolforge_weld.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-04-16 08:40:05.000000 toolforge_weld-1.5.0/toolforge_weld.egg-info/top_level.txt
```

### Comparing `toolforge-weld-1.4.0/LICENSE` & `toolforge_weld-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `toolforge-weld-1.4.0/PKG-INFO` & `toolforge_weld-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: toolforge-weld
-Version: 1.4.0
+Version: 1.5.0
 Summary: Shared Python code for Toolforge infrastructure components
 Author: Taavi Väänänen
 Author-email: hi@taavi.wtf
 License: AGPL-3.0-or-later
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: python-dateutil
 Requires-Dist: PyYAML
 Requires-Dist: requests
 Requires-Dist: pyOpenSSL
```

### Comparing `toolforge-weld-1.4.0/setup.py` & `toolforge_weld-1.5.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import find_packages, setup
 
 this_directory = Path(__file__).parent
 
 setup(
     name="toolforge-weld",
-    version="1.4.0",
+    version="1.5.0",
     author="Taavi Väänänen",
     author_email="hi@taavi.wtf",
     license="AGPL-3.0-or-later",
     packages=find_packages(),
     package_data={"toolforge_weld": ["py.typed"]},
     description="Shared Python code for Toolforge infrastructure components",
     long_description=(this_directory / "README.md").read_text(),
@@ -20,9 +20,9 @@
         "Development Status :: 4 - Beta",
         "Intended Audience :: System Administrators",
         "License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)",
         "Operating System :: POSIX :: Linux",
         "Programming Language :: Python :: 3",
         "Typing :: Typed",
     ],
-    python_requires=">=3.7",
+    python_requires=">=3.11",
 )
```

### Comparing `toolforge-weld-1.4.0/tests/test_api_client.py` & `toolforge_weld-1.5.0/tests/test_api_client.py`

 * *Files identical despite different names*

### Comparing `toolforge-weld-1.4.0/tests/test_config.py` & `toolforge_weld-1.5.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `toolforge-weld-1.4.0/tests/test_kubernetes_config.py` & `toolforge_weld-1.5.0/tests/test_kubernetes_config.py`

 * *Files identical despite different names*

### Comparing `toolforge-weld-1.4.0/toolforge_weld/api_client.py` & `toolforge_weld-1.5.0/toolforge_weld/api_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,31 +103,35 @@
         else:
             self.session.verify = False
 
             # T253412: Disable warnings about unverifed TLS certs when talking to the
             # Kubernetes API endpoint
             urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
-        self.session.headers[
-            "User-Agent"
-        ] = f"{user_agent} toolforge_weld/{toolforge_weld.__version__} python-requests/{requests.__version__}"
+        self.session.headers["User-Agent"] = (
+            f"{user_agent} toolforge_weld/{toolforge_weld.__version__} python-requests/{requests.__version__}"
+        )
 
     def _make_request(self, method: str, url: str, **kwargs) -> requests.Response:
         try:
             response = self.session.request(method, **self.make_kwargs(url, **kwargs))
             response.raise_for_status()
             return response
         except requests.exceptions.ConnectionError as e:
             if self.connect_exception_handler:
                 raise self.connect_exception_handler(e) from e
             raise e
         except requests.exceptions.HTTPError as e:
             # Raise a connection error on proxy (= api-gateway) level
             # errors to provide more uniform error messages.
-            if e.response.status_code in (502, 503) and self.connect_exception_handler:
+            if (
+                e.response is not None
+                and e.response.status_code in (502, 503)
+                and self.connect_exception_handler
+            ):
                 raise self.connect_exception_handler(e) from e
 
             if self.exception_handler:
                 raise self.exception_handler(e) from e
             raise e
 
     def make_kwargs(self, url: str, **kwargs) -> dict[str, Any]:
```

### Comparing `toolforge-weld-1.4.0/toolforge_weld/config.py` & `toolforge_weld-1.5.0/toolforge_weld/config.py`

 * *Files identical despite different names*

### Comparing `toolforge-weld-1.4.0/toolforge_weld/errors.py` & `toolforge_weld-1.5.0/toolforge_weld/errors.py`

 * *Files identical despite different names*

### Comparing `toolforge-weld-1.4.0/toolforge_weld/kubernetes.py` & `toolforge_weld-1.5.0/toolforge_weld/kubernetes.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
+from dataclasses import dataclass
 from decimal import Decimal, InvalidOperation
 from enum import Enum
 from pathlib import Path
-from typing import Any, ClassVar, Dict, List, Optional
+from typing import Any, ClassVar, Dict, List, Optional, Union
 
 from toolforge_weld.api_client import ToolforgeClient
 from toolforge_weld.errors import ToolforgeError
 from toolforge_weld.kubernetes_config import Kubeconfig, locate_config_file
 
 
 class ToolforgeKubernetesError(ToolforgeError):
@@ -50,26 +51,36 @@
         return {"toolforge.org/mount-storage": self.value}
 
 
 def _format_labels(labels: Dict[str, str]) -> str:
     return ",".join([f"{k}={v}" for k, v in labels.items()])
 
 
+@dataclass
+class ApiData:
+    version: str
+    namespaced: bool = True
+
+
+VersionType = Union[str, ApiData]
+
+
 class K8sClient(ToolforgeClient):
     """Kubernetes API client."""
 
-    VERSIONS: ClassVar[Dict[str, str]] = {
+    VERSIONS: ClassVar[Dict[str, VersionType]] = {
         "configmaps": "v1",
         "cronjobs": "batch/v1",
         "deployments": "apps/v1",
         "endpoints": "v1",
         "events": "v1",
         "ingresses": "networking.k8s.io/v1",
         "jobs": "batch/v1",
         "limitranges": "v1",
+        "namespaces": ApiData(version="v1", namespaced=False),
         "pods": "v1",
         "replicasets": "apps/v1",
         "resourcequotas": "v1",
         "services": "v1",
     }
 
     def __init__(
@@ -98,25 +109,41 @@
     def locate_config_file() -> Path:
         """Deprecated: use Kubeconfig.load instead."""
         return locate_config_file()
 
     def make_kwargs(self, url: str, **kwargs):
         """Setup kwargs for a Requests request."""
         kwargs = super().make_kwargs(url=url, **kwargs)
-        version = kwargs.pop("version", "v1")
+        api = kwargs.pop("version", "v1")
+        if isinstance(api, str):
+            version = api
+            namespaced = True
+        elif isinstance(api, ApiData):
+            version = api.version
+            namespaced = api.namespaced
+        else:
+            raise RuntimeError("Invalid version data passed to make_kwargs")
+
         if version == "v1":
             root = "api"
         else:
             root = "apis"
 
         # use "or" syntax in case namespace is present but set as None
+        # this is not done in the if statement below as we don't want to pass it
+        # to requests either way
         namespace = kwargs.pop("namespace", None) or self.namespace
 
-        kwargs["url"] = "{}/{}/{}/namespaces/{}/{}".format(
-            self.server, root, version, namespace, url
+        if namespaced:
+            namespace_path = f"/namespaces/{namespace}"
+        else:
+            namespace_path = ""
+
+        kwargs["url"] = "{}/{}/{}{}/{}".format(
+            self.server, root, version, namespace_path, url
         )
 
         name = kwargs.pop("name", None)
         if name is not None:
             kwargs["url"] = "{}/{}".format(kwargs["url"], name)
 
         subpath = kwargs.pop("subpath", None)
@@ -141,15 +168,15 @@
         )
 
     def get_objects(
         self,
         kind: str,
         *,
         label_selector: Optional[Dict[str, str]] = None,
-        field_selector: Optional[Dict[str, Any]] = None,
+        field_selector: Optional[str] = None,
         namespace: Optional[str] = None,
     ) -> List[Dict[str, Any]]:
         """Get list of objects of the given kind in the namespace."""
         params: Dict[str, Any] = {}
 
         if label_selector:
             params["labelSelector"] = _format_labels(label_selector)
```

### Comparing `toolforge-weld-1.4.0/toolforge_weld/kubernetes_config.py` & `toolforge_weld-1.5.0/toolforge_weld/kubernetes_config.py`

 * *Files identical despite different names*

### Comparing `toolforge-weld-1.4.0/toolforge_weld/logs/__init__.py` & `toolforge_weld-1.5.0/toolforge_weld/logs/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Queries logs created by a tool."""
+
 from toolforge_weld.kubernetes import K8sClient
 from toolforge_weld.kubernetes_config import Kubeconfig
 from toolforge_weld.logs.kubernetes import KubernetesSource
 from toolforge_weld.logs.source import LogEntry, LogSource
 
 
 def get_log_source(user_agent: str) -> LogSource:
```

### Comparing `toolforge-weld-1.4.0/toolforge_weld/logs/kubernetes.py` & `toolforge_weld-1.5.0/toolforge_weld/logs/kubernetes.py`

 * *Files identical despite different names*

### Comparing `toolforge-weld-1.4.0/toolforge_weld/logs/source.py` & `toolforge_weld-1.5.0/toolforge_weld/logs/source.py`

 * *Files identical despite different names*

### Comparing `toolforge-weld-1.4.0/toolforge_weld.egg-info/PKG-INFO` & `toolforge_weld-1.5.0/toolforge_weld.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: toolforge-weld
-Version: 1.4.0
+Version: 1.5.0
 Summary: Shared Python code for Toolforge infrastructure components
 Author: Taavi Väänänen
 Author-email: hi@taavi.wtf
 License: AGPL-3.0-or-later
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: python-dateutil
 Requires-Dist: PyYAML
 Requires-Dist: requests
 Requires-Dist: pyOpenSSL
```

### Comparing `toolforge-weld-1.4.0/toolforge_weld.egg-info/SOURCES.txt` & `toolforge_weld-1.5.0/toolforge_weld.egg-info/SOURCES.txt`

 * *Files identical despite different names*

