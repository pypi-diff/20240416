# Comparing `tmp/eptr2-0.3.0.tar.gz` & `tmp/eptr2-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eptr2-0.3.0.tar", max compression
+gzip compressed data, was "eptr2-0.4.0.tar", max compression
```

## Comparing `eptr2-0.3.0.tar` & `eptr2-0.4.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    11357 2023-11-15 12:19:13.028669 eptr2-0.3.0/LICENSE
--rw-r--r--   0        0        0     3132 2024-04-01 16:49:22.653196 eptr2-0.3.0/README.md
--rw-r--r--   0        0        0       48 2023-11-24 09:44:59.967784 eptr2-0.3.0/eptr2/__init__.py
--rw-r--r--   0        0        0     5846 2024-04-01 16:46:11.719108 eptr2-0.3.0/eptr2/main.py
--rw-r--r--   0        0        0      248 2024-04-01 16:47:02.813358 eptr2-0.3.0/eptr2/mapping/__init__.py
--rw-r--r--   0        0        0    74878 2024-04-01 16:19:34.773267 eptr2-0.3.0/eptr2/mapping/help.py
--rw-r--r--   0        0        0     7683 2024-04-01 16:36:27.545931 eptr2-0.3.0/eptr2/mapping/parameters.py
--rw-r--r--   0        0        0    24542 2024-04-01 16:41:59.019233 eptr2-0.3.0/eptr2/mapping/path.py
--rw-r--r--   0        0        0     3240 2024-04-01 16:35:34.003858 eptr2-0.3.0/eptr2/mapping/processing.py
--rw-r--r--   0        0        0      183 2024-04-01 16:47:13.041852 eptr2-0.3.0/eptr2/processing/__init__.py
--rw-r--r--   0        0        0        0 2023-12-08 13:25:19.644898 eptr2-0.3.0/eptr2/processing/postprocess/__init__.py
--rw-r--r--   0        0        0      829 2024-01-31 13:55:19.162404 eptr2-0.3.0/eptr2/processing/postprocess/items.py
--rw-r--r--   0        0        0        0 2023-11-24 09:44:59.970042 eptr2-0.3.0/eptr2/processing/preprocess/__init__.py
--rw-r--r--   0        0        0     1502 2024-02-23 09:41:05.037560 eptr2-0.3.0/eptr2/processing/preprocess/params.py
--rw-r--r--   0        0        0        0 2023-11-24 09:44:59.970736 eptr2-0.3.0/eptr2/util/__init__.py
--rw-r--r--   0        0        0     3161 2023-12-05 12:02:08.460583 eptr2-0.3.0/eptr2/util/certificate.py
--rw-r--r--   0        0        0     6527 2024-03-21 10:11:19.451330 eptr2-0.3.0/eptr2/util/costs.py
--rw-r--r--   0        0        0     1207 2024-01-10 14:14:00.769596 eptr2-0.3.0/eptr2/util/evaluation.py
--rw-r--r--   0        0        0     3759 2023-11-27 07:59:15.415246 eptr2-0.3.0/eptr2/util/time.py
--rw-r--r--   0        0        0      513 2024-04-01 16:50:03.100488 eptr2-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     3770 1970-01-01 00:00:00.000000 eptr2-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-11-15 12:19:13.028669 eptr2-0.4.0/LICENSE
+-rw-r--r--   0        0        0     3734 2024-04-16 15:49:05.109126 eptr2-0.4.0/README.md
+-rw-r--r--   0        0        0       48 2023-11-24 09:44:59.967784 eptr2-0.4.0/eptr2/__init__.py
+-rw-r--r--   0        0        0     6735 2024-04-16 15:39:13.034284 eptr2-0.4.0/eptr2/main.py
+-rw-r--r--   0        0        0      186 2024-04-16 15:00:23.436797 eptr2-0.4.0/eptr2/mapping/__init__.py
+-rw-r--r--   0        0        0    74878 2024-04-01 16:52:19.990559 eptr2-0.4.0/eptr2/mapping/help.py
+-rw-r--r--   0        0        0     7683 2024-04-01 16:52:19.990901 eptr2-0.4.0/eptr2/mapping/parameters.py
+-rw-r--r--   0        0        0    24542 2024-04-01 16:52:19.991139 eptr2-0.4.0/eptr2/mapping/path.py
+-rw-r--r--   0        0        0     3240 2024-04-01 16:52:19.991491 eptr2-0.4.0/eptr2/mapping/processing.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:51:58.000666 eptr2-0.4.0/eptr2/processing/__init__.py
+-rw-r--r--   0        0        0        0 2023-12-08 13:25:19.644898 eptr2-0.4.0/eptr2/processing/postprocess/__init__.py
+-rw-r--r--   0        0        0      806 2024-04-16 15:25:10.198499 eptr2-0.4.0/eptr2/processing/postprocess/items.py
+-rw-r--r--   0        0        0        0 2023-11-24 09:44:59.970042 eptr2-0.4.0/eptr2/processing/preprocess/__init__.py
+-rw-r--r--   0        0        0     1502 2024-02-23 09:41:05.037560 eptr2-0.4.0/eptr2/processing/preprocess/params.py
+-rw-r--r--   0        0        0        0 2023-11-24 09:44:59.970736 eptr2-0.4.0/eptr2/util/__init__.py
+-rw-r--r--   0        0        0     3161 2023-12-05 12:02:08.460583 eptr2-0.4.0/eptr2/util/certificate.py
+-rw-r--r--   0        0        0     6527 2024-03-21 10:11:19.451330 eptr2-0.4.0/eptr2/util/costs.py
+-rw-r--r--   0        0        0     1207 2024-01-10 14:14:00.769596 eptr2-0.4.0/eptr2/util/evaluation.py
+-rw-r--r--   0        0        0     3759 2023-11-27 07:59:15.415246 eptr2-0.4.0/eptr2/util/time.py
+-rw-r--r--   0        0        0      489 2024-04-16 15:44:52.324823 eptr2-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     4337 1970-01-01 00:00:00.000000 eptr2-0.4.0/PKG-INFO
```

### Comparing `eptr2-0.3.0/LICENSE` & `eptr2-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `eptr2-0.3.0/README.md` & `eptr2-0.4.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -10,38 +10,42 @@
 `eptr2` (**EP**IAS **Tr**ansparency **2**.0) package is a thin wrapper around [EPIAS Transparency Platform v2.0](https://seffaflik.epias.com.tr/home) API brought to you by [Robokami](https://robokami.com). It is an unofficial package with Apache License 2.0 (free and permissable use for commercial applications, [see details](https://www.tldrlegal.com/license/apache-license-2-0-apache-2-0)).
 
 
 `eptr2` currently more than 100 services with convenience methods. You can also use `transparency_call` function to call any service with any method and body.
 
 ## Installation
 
-You can simply use PyPI to install `eptr2` package or directly through GitHub. See [eptr2demo](https://eptr2demo.streamlit.io) page for available calls and examples.
+You can simply use PyPI to install `eptr2` package or directly through GitHub. See [eptr2demo](https://eptr2demo.streamlit.app) page for available calls and examples.
 
 ```bash
 pip install eptr2
 ```
 
-NOTE: In future versions, data frame returns will be optional. If pandas is not installed, data frames will not be returned. You can install "dataframe" version with the following command. _(Not implemented yet)_
+NOTE: Starting from v0.4.0, data frame returns will be optional. If pandas is not installed, data frames will not be returned. You can install "dataframe" version with the following command. _(Not implemented yet)_
 
 ```bash
 pip install "eptr2[dataframe]"
 ```
 
 ```bash
 pip install git+https://github.com/Tideseed/eptr2.git
 ```
 
 ## Usage
 
-You can simply use `EPTR2` class to call services with convenience methods. 
+You can simply use `EPTR2` class to call services with convenience methods. Main object call has some parameters to control the behavior of the package. You can set `ssl_verify` to `False` if you have SSL verification problems. You can set `postprocess` to `False` if you don't want to get data frames as response. You can set `get_raw_response` to `True` if you want to get raw urllib3 response object.
 
 ```python
 from eptr2 import EPTR2
 
-eptr = EPTR2()
+eptr = EPTR2(
+        ssl_verify=True,  ## SSL verification (default: True)
+        postprocess=True, ## If you want to get data frames as response (default: True) install pandas
+        get_raw_response=False ## If you want to get raw urllib3 response object (default: False)
+        )
 
 mcp_call = eptr.call("mcp",start_date="2023-10-10",end_date="2023-10-10")
 print(mcp.json())
 ```
 
 You can search for available calls with `eptr.get_available_calls()` function. We plan to include all transparency services in the future.
```

### Comparing `eptr2-0.3.0/eptr2/main.py` & `eptr2-0.4.0/eptr2/main.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,47 +1,35 @@
 from typing import Any
-import requests
+import urllib3
 import re
+import json
 from urllib.parse import urljoin
 import copy
 from eptr2.mapping import (
     get_total_path,
     get_call_method,
     get_required_parameters,
     get_param_label,
     get_path_map,
     get_optional_parameters,
 )
 from warnings import warn
-from eptr2.processing import preprocess_parameter
-from eptr2.mapping import get_postprocess_function
+from eptr2.processing.preprocess.params import preprocess_parameter
 
 
 class EPTR2:
     def __init__(self, **kwargs) -> None:
         ## kwargs are
         ### map_param_labels: bool
         ### secure: bool
         ### query_parameters: dict
         ### just_call_phrase: bool
         self.ssl_verify = kwargs.get("ssl_verify", True)
-        self.postprocess = kwargs.get("postprocess", True)
-
-        # try:
-        #     import pandas as pd
-        # except ImportError:
-        #     warn(
-        #         "pandas is not installed. Some functionalities may not work properly. Postprocessing is disabled.",
-        #         ImportWarning,
-        #         stacklevel=2,
-        #     )
-        #     self.postprocess = False
-
-        # if self.postprocess:
-        #     from eptr2.mapping import get_postprocess_function
+        self.check_postprocess(postprocess=kwargs.get("postprocess", True))
+        self.get_raw_response = kwargs.get("get_raw_response", False)
 
     ## Ref: https://stackoverflow.com/a/62303969/3608936
     def __getattr__(self, __name: str) -> Any:
         def method(*args, **kwargs):
             key_raw = __name
             key = re.sub("_", "-", key_raw)
             if key not in get_path_map(just_call_keys=True):
@@ -49,14 +37,25 @@
                     "This call is not yet defined. Call 'get_available_calls' method to see the available calls."
                 )
             # required_body_params = get_required_parameters(key)
             return getattr(self, "call")(key=key, **kwargs)
 
         return method
 
+    def check_postprocess(self, postprocess: bool = True):
+        self.postprocess = postprocess
+        if self.postprocess:
+            try:
+                from eptr2.mapping.processing import get_postprocess_function
+            except ImportError:
+                print(
+                    "pandas is not installed. Some functionalities may not work properly. Postprocessing is disabled. To disable postprocessing just set 'postprocess' parameter to False when calling EPTR2 class.",
+                )
+                self.postprocess = False
+
     def get_available_calls(self):
         return get_path_map(just_call_keys=True)
 
     def call(self, key: str, **kwargs):
         call_path = get_total_path(key)
         call_method = get_call_method(key)
         required_body_params = get_required_parameters(key)
@@ -115,14 +114,18 @@
             call_path=call_path,
             call_method=call_method,
             call_body=call_body,
             ssl_verify=self.ssl_verify,
             **kwargs,
         )
 
+        if kwargs.get("get_raw_response", self.get_raw_response):
+            return res
+
+        res = json.loads(res.data.decode("utf-8"))
         if kwargs.get("postprocess", self.postprocess):
             df = get_postprocess_function(key)(res, key=key)
             return df
 
         return res
 
 
@@ -152,21 +155,38 @@
         return call_phrase
 
     if call_body is not None and call_body != {} and call_method == "GET":
         raise Exception("GET method does not allow body parameters.")
 
     ssl_verify = kwargs.pop("ssl_verify", True)
 
-    res = requests.request(
+    http = urllib3.PoolManager(cert_reqs="CERT_REQUIRED" if ssl_verify else "CERT_NONE")
+    res = http.request(
         method=call_method,
         url=urljoin(call_phrase, ""),
-        json=call_body,
-        verify=ssl_verify,
+        body=json.dumps(call_body),
+        headers={"Content-Type": "application/json"},
         **kwargs.get("request_kwargs", {}),
     )
-
-    if res.status_code not in [200, 201]:
+    if res.status not in [200, 201]:
         raise Exception(
-            "Request failed with status code: " + str(res.status_code) + "\n" + res.text
+            "Request failed with status code: "
+            + str(res.status)
+            + "\n"
+            + res.data.decode("utf-8")
         )
-
     return res
+
+    # res = requests.request(
+    #     method=call_method,
+    #     url=urljoin(call_phrase, ""),
+    #     json=call_body,
+    #     verify=ssl_verify,
+    #     **kwargs.get("request_kwargs", {}),
+    # )
+
+    # if res.status_code not in [200, 201]:
+    #     raise Exception(
+    #         "Request failed with status code: " + str(res.status_code) + "\n" + res.text
+    #     )
+
+    # return res
```

### Comparing `eptr2-0.3.0/eptr2/mapping/help.py` & `eptr2-0.4.0/eptr2/mapping/help.py`

 * *Files identical despite different names*

### Comparing `eptr2-0.3.0/eptr2/mapping/parameters.py` & `eptr2-0.4.0/eptr2/mapping/parameters.py`

 * *Files identical despite different names*

### Comparing `eptr2-0.3.0/eptr2/mapping/path.py` & `eptr2-0.4.0/eptr2/mapping/path.py`

 * *Files identical despite different names*

### Comparing `eptr2-0.3.0/eptr2/mapping/processing.py` & `eptr2-0.4.0/eptr2/mapping/processing.py`

 * *Files identical despite different names*

### Comparing `eptr2-0.3.0/eptr2/processing/preprocess/params.py` & `eptr2-0.4.0/eptr2/processing/preprocess/params.py`

 * *Files identical despite different names*

### Comparing `eptr2-0.3.0/eptr2/util/certificate.py` & `eptr2-0.4.0/eptr2/util/certificate.py`

 * *Files identical despite different names*

### Comparing `eptr2-0.3.0/eptr2/util/costs.py` & `eptr2-0.4.0/eptr2/util/costs.py`

 * *Files identical despite different names*

### Comparing `eptr2-0.3.0/eptr2/util/evaluation.py` & `eptr2-0.4.0/eptr2/util/evaluation.py`

 * *Files identical despite different names*

### Comparing `eptr2-0.3.0/eptr2/util/time.py` & `eptr2-0.4.0/eptr2/util/time.py`

 * *Files identical despite different names*

### Comparing `eptr2-0.3.0/PKG-INFO` & `eptr2-0.4.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: eptr2
-Version: 0.3.0
+Version: 0.4.0
 Summary: EPIAS Transparency Platform v2.0 Python client by Robokami Data
 License: Apache-2.0
 Author: Tideseed
 Author-email: info@tideseed.com
 Requires-Python: >=3.9.6
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: dataframe
 Requires-Dist: pandas (>=2.1.3) ; extra == "dataframe"
-Requires-Dist: requests (>=2.31.0)
 Description-Content-Type: text/markdown
 
 ![PyPI - Version](https://img.shields.io/pypi/v/eptr2) ![PyPI - Downloads](https://img.shields.io/pypi/dm/eptr2) 
 
 _🇹🇷 Türkçe açıklama için aşağıya bakınız._
 
 > [!IMPORTANT]  
@@ -28,38 +27,42 @@
 `eptr2` (**EP**IAS **Tr**ansparency **2**.0) package is a thin wrapper around [EPIAS Transparency Platform v2.0](https://seffaflik.epias.com.tr/home) API brought to you by [Robokami](https://robokami.com). It is an unofficial package with Apache License 2.0 (free and permissable use for commercial applications, [see details](https://www.tldrlegal.com/license/apache-license-2-0-apache-2-0)).
 
 
 `eptr2` currently more than 100 services with convenience methods. You can also use `transparency_call` function to call any service with any method and body.
 
 ## Installation
 
-You can simply use PyPI to install `eptr2` package or directly through GitHub. See [eptr2demo](https://eptr2demo.streamlit.io) page for available calls and examples.
+You can simply use PyPI to install `eptr2` package or directly through GitHub. See [eptr2demo](https://eptr2demo.streamlit.app) page for available calls and examples.
 
 ```bash
 pip install eptr2
 ```
 
-NOTE: In future versions, data frame returns will be optional. If pandas is not installed, data frames will not be returned. You can install "dataframe" version with the following command. _(Not implemented yet)_
+NOTE: Starting from v0.4.0, data frame returns will be optional. If pandas is not installed, data frames will not be returned. You can install "dataframe" version with the following command. _(Not implemented yet)_
 
 ```bash
 pip install "eptr2[dataframe]"
 ```
 
 ```bash
 pip install git+https://github.com/Tideseed/eptr2.git
 ```
 
 ## Usage
 
-You can simply use `EPTR2` class to call services with convenience methods. 
+You can simply use `EPTR2` class to call services with convenience methods. Main object call has some parameters to control the behavior of the package. You can set `ssl_verify` to `False` if you have SSL verification problems. You can set `postprocess` to `False` if you don't want to get data frames as response. You can set `get_raw_response` to `True` if you want to get raw urllib3 response object.
 
 ```python
 from eptr2 import EPTR2
 
-eptr = EPTR2()
+eptr = EPTR2(
+        ssl_verify=True,  ## SSL verification (default: True)
+        postprocess=True, ## If you want to get data frames as response (default: True) install pandas
+        get_raw_response=False ## If you want to get raw urllib3 response object (default: False)
+        )
 
 mcp_call = eptr.call("mcp",start_date="2023-10-10",end_date="2023-10-10")
 print(mcp.json())
 ```
 
 You can search for available calls with `eptr.get_available_calls()` function. We plan to include all transparency services in the future.
```

