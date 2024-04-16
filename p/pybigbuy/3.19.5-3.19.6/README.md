# Comparing `tmp/pybigbuy-3.19.5.tar.gz` & `tmp/pybigbuy-3.19.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybigbuy-3.19.5.tar", max compression
+gzip compressed data, was "pybigbuy-3.19.6.tar", max compression
```

## Comparing `pybigbuy-3.19.5.tar` & `pybigbuy-3.19.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1062 2023-11-17 09:08:35.459830 pybigbuy-3.19.5/LICENSE
--rw-r--r--   0        0        0      531 2023-11-17 09:08:35.459830 pybigbuy-3.19.5/README.md
--rw-r--r--   0        0        0      665 2023-11-17 09:08:35.459830 pybigbuy-3.19.5/bigbuy/__init__.py
--rw-r--r--   0        0        0    26371 2023-11-17 09:08:35.459830 pybigbuy-3.19.5/bigbuy/api.py
--rw-r--r--   0        0        0    13271 2023-11-17 09:08:35.459830 pybigbuy-3.19.5/bigbuy/exceptions.py
--rw-r--r--   0        0        0        0 2023-11-17 09:08:35.459830 pybigbuy-3.19.5/bigbuy/py.typed
--rw-r--r--   0        0        0     1403 2023-11-17 09:08:35.459830 pybigbuy-3.19.5/bigbuy/rate_limit.py
--rw-r--r--   0        0        0      952 2023-11-17 09:08:35.459830 pybigbuy-3.19.5/pyproject.toml
--rw-r--r--   0        0        0     1243 1970-01-01 00:00:00.000000 pybigbuy-3.19.5/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-04-16 09:46:56.017069 pybigbuy-3.19.6/LICENSE
+-rw-r--r--   0        0        0      531 2024-04-16 09:46:56.017069 pybigbuy-3.19.6/README.md
+-rw-r--r--   0        0        0      665 2024-04-16 09:46:56.017069 pybigbuy-3.19.6/bigbuy/__init__.py
+-rw-r--r--   0        0        0    26371 2024-04-16 09:46:56.017069 pybigbuy-3.19.6/bigbuy/api.py
+-rw-r--r--   0        0        0    13466 2024-04-16 09:46:56.017069 pybigbuy-3.19.6/bigbuy/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-16 09:46:56.017069 pybigbuy-3.19.6/bigbuy/py.typed
+-rw-r--r--   0        0        0     1403 2024-04-16 09:46:56.017069 pybigbuy-3.19.6/bigbuy/rate_limit.py
+-rw-r--r--   0        0        0      952 2024-04-16 09:46:56.017069 pybigbuy-3.19.6/pyproject.toml
+-rw-r--r--   0        0        0     1243 1970-01-01 00:00:00.000000 pybigbuy-3.19.6/PKG-INFO
```

### Comparing `pybigbuy-3.19.5/LICENSE` & `pybigbuy-3.19.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pybigbuy-3.19.5/README.md` & `pybigbuy-3.19.6/README.md`

 * *Files identical despite different names*

### Comparing `pybigbuy-3.19.5/bigbuy/__init__.py` & `pybigbuy-3.19.6/bigbuy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Bigbuy
 -------
 
 Bigbuy is a library for Python that wraps the BigBuy API.
 """
 
 __author__ = 'Bixoto <tech@bixoto.com>'
-__version__ = '3.19.5'
+__version__ = '3.19.6'
 
 from .api import BigBuy
 from .exceptions import (
     BBError, BBResponseError, BBPackError, BBExportError, BBProductError, BBStockError,
     BBNoCarrierError, BBBankWireTooLowError, BBMoneyBoxTooLowError, BBTemporaryOrderError, BBOrderAlreadyExistsError,
     BBOrderTooLowError, BBIncorrectRefError, BBInvalidPaymentError, BBZipcodeFormatError, BBProductNotFoundError,
     BBServerError, BBRateLimitError, BBValidationError, BBWarehouseSplitError, BBShippingError, BBTimeoutError,
```

### Comparing `pybigbuy-3.19.5/bigbuy/api.py` & `pybigbuy-3.19.6/bigbuy/api.py`

 * *Files identical despite different names*

### Comparing `pybigbuy-3.19.5/bigbuy/exceptions.py` & `pybigbuy-3.19.6/bigbuy/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,17 +8,16 @@
 """
 import json
 import re
 import time
 from datetime import datetime, timedelta
 from typing import Optional, Union, Dict, Any, List, Type, cast, Sequence
 
-from requests import Response
-
 from bigbuy.rate_limit import RateLimit
+from requests import Response
 
 
 class BBError(Exception):
     """Generic error class."""
 
 
 class BBResponseError(BBError):
@@ -366,14 +365,18 @@
                 message = error.get("message", message)
 
     # {"code": "ER003", "message": "..."}
     elif "code" in content and "message" in content:
         bb_code = content["code"]
         message = content["message"]
 
+        # {"code": "Bad request", "message": 400}
+        if isinstance(message, int) and 400 <= message <= 599 and isinstance(bb_code, str):
+            bb_code, message = str(message), bb_code
+
     if "error_detail" in content and "different warehouses" in message:
         error_detail = content["error_detail"]
         if isinstance(error_detail, dict) and "warehouses" in error_detail:
             raise BBWarehouseSplitError(message, response, bb_code=bb_code, warehouses=error_detail["warehouses"])
 
     try:
         if int(bb_code) // 100 == 5:
```

### Comparing `pybigbuy-3.19.5/bigbuy/rate_limit.py` & `pybigbuy-3.19.6/bigbuy/rate_limit.py`

 * *Files identical despite different names*

### Comparing `pybigbuy-3.19.5/pyproject.toml` & `pybigbuy-3.19.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pybigbuy"
-version = "3.19.5"
+version = "3.19.6"
 description = "BigBuy API client in Python"
 authors = ["Bixoto <tech@bixoto.com>"]
 license = "MIT"
 include = ["bigbuy/py.typed"]
 readme = "README.md"
 # https://github.com/python-poetry/poetry/issues/705#issuecomment-444742697
 packages = [
```

### Comparing `pybigbuy-3.19.5/PKG-INFO` & `pybigbuy-3.19.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybigbuy
-Version: 3.19.5
+Version: 3.19.6
 Summary: BigBuy API client in Python
 License: MIT
 Author: Bixoto
 Author-email: tech@bixoto.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

