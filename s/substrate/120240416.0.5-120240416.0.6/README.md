# Comparing `tmp/substrate-120240416.0.5.tar.gz` & `tmp/substrate-120240416.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "substrate-120240416.0.5.tar", max compression
+gzip compressed data, was "substrate-120240416.0.6.tar", max compression
```

## Comparing `substrate-120240416.0.5.tar` & `substrate-120240416.0.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1066 2024-03-19 21:46:08.735767 substrate-120240416.0.5/LICENSE
--rw-r--r--   0        0        0       45 2024-03-19 21:55:57.200047 substrate-120240416.0.5/README.md
--rw-r--r--   0        0        0     2023 2024-04-16 21:23:44.744816 substrate-120240416.0.5/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-11 19:17:25.000000 substrate-120240416.0.5/substrate/.keep
--rw-r--r--   0        0        0       17 2024-04-16 21:23:08.000000 substrate-120240416.0.5/substrate/GEN_VERSION
--rw-r--r--   0        0        0     2048 2024-04-16 21:23:09.000000 substrate-120240416.0.5/substrate/__init__.py
--rw-r--r--   0        0        0     6010 2024-04-16 20:07:00.739333 substrate-120240416.0.5/substrate/_client.py
--rw-r--r--   0        0        0       30 2024-03-13 14:46:31.829473 substrate-120240416.0.5/substrate/_version.py
--rw-r--r--   0        0        0        1 2024-04-16 21:23:27.826516 substrate-120240416.0.5/substrate/core/__init__.py
--rw-r--r--   0        0        0       27 2024-04-16 21:23:27.826379 substrate-120240416.0.5/substrate/core/_version.py
--rw-r--r--   0        0        0     1535 2024-04-16 21:23:27.826967 substrate-120240416.0.5/substrate/core/base_future.py
--rw-r--r--   0        0        0        0 2024-04-16 21:23:27.827571 substrate-120240416.0.5/substrate/core/client/__init__.py
--rw-r--r--   0        0        0     1750 2024-04-16 21:23:27.827722 substrate-120240416.0.5/substrate/core/client/find_futures_client.py
--rw-r--r--   0        0        0     2697 2024-04-16 21:23:27.827901 substrate-120240416.0.5/substrate/core/client/future.py
--rw-r--r--   0        0        0     1212 2024-04-16 21:23:27.827319 substrate-120240416.0.5/substrate/core/client/graph.py
--rw-r--r--   0        0        0     1149 2024-04-16 21:23:27.826777 substrate-120240416.0.5/substrate/core/coregraph.py
--rw-r--r--   0        0        0     2186 2024-04-16 21:23:27.825560 substrate-120240416.0.5/substrate/core/corenode.py
--rw-r--r--   0        0        0     1227 2024-04-16 21:23:27.827149 substrate-120240416.0.5/substrate/core/future_directive.py
--rw-r--r--   0        0        0      894 2024-04-16 21:23:27.825332 substrate-120240416.0.5/substrate/core/id_generator.py
--rw-r--r--   0        0        0    38450 2024-04-16 21:23:27.825854 substrate-120240416.0.5/substrate/core/models.py
--rw-r--r--   0        0        0     2332 2024-04-16 21:23:27.825185 substrate-120240416.0.5/substrate/core/sb.py
--rw-r--r--   0        0        0    32587 2024-04-16 21:23:06.000000 substrate-120240416.0.5/substrate/dataclass_models.py
--rw-r--r--   0        0        0    43578 2024-04-16 21:23:08.000000 substrate-120240416.0.5/substrate/future_dataclass_models.py
--rw-r--r--   0        0        0    40555 2024-04-16 21:23:09.000000 substrate-120240416.0.5/substrate/nodes.py
--rw-r--r--   0        0        0        0 2024-02-07 23:39:17.000078 substrate-120240416.0.5/substrate/py.typed
--rw-r--r--   0        0        0     1490 2024-04-16 20:07:00.739577 substrate-120240416.0.5/substrate/substrate.py
--rw-r--r--   0        0        0     1041 2024-04-16 20:45:00.388800 substrate-120240416.0.5/substrate/substrate_response.py
--rw-r--r--   0        0        0    35749 2024-04-16 21:23:05.000000 substrate-120240416.0.5/substrate/typeddict_models.py
--rw-r--r--   0        0        0      648 1970-01-01 00:00:00.000000 substrate-120240416.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-03-19 21:46:08.735767 substrate-120240416.0.6/LICENSE
+-rw-r--r--   0        0        0       45 2024-03-19 21:55:57.200047 substrate-120240416.0.6/README.md
+-rw-r--r--   0        0        0     2023 2024-04-16 21:54:24.375133 substrate-120240416.0.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-11 19:17:25.000000 substrate-120240416.0.6/substrate/.keep
+-rw-r--r--   0        0        0       17 2024-04-16 21:25:37.772233 substrate-120240416.0.6/substrate/GEN_VERSION
+-rw-r--r--   0        0        0     2010 2024-04-16 21:54:10.814592 substrate-120240416.0.6/substrate/__init__.py
+-rw-r--r--   0        0        0     6010 2024-04-16 20:07:00.739333 substrate-120240416.0.6/substrate/_client.py
+-rw-r--r--   0        0        0       30 2024-03-13 14:46:31.829473 substrate-120240416.0.6/substrate/_version.py
+-rw-r--r--   0        0        0        1 2024-04-16 21:23:27.826516 substrate-120240416.0.6/substrate/core/__init__.py
+-rw-r--r--   0        0        0       27 2024-04-16 21:23:27.826379 substrate-120240416.0.6/substrate/core/_version.py
+-rw-r--r--   0        0        0     1535 2024-04-16 21:23:27.826967 substrate-120240416.0.6/substrate/core/base_future.py
+-rw-r--r--   0        0        0        0 2024-04-16 21:23:27.827571 substrate-120240416.0.6/substrate/core/client/__init__.py
+-rw-r--r--   0        0        0     1750 2024-04-16 21:23:27.827722 substrate-120240416.0.6/substrate/core/client/find_futures_client.py
+-rw-r--r--   0        0        0     2697 2024-04-16 21:23:27.827901 substrate-120240416.0.6/substrate/core/client/future.py
+-rw-r--r--   0        0        0     1212 2024-04-16 21:23:27.827319 substrate-120240416.0.6/substrate/core/client/graph.py
+-rw-r--r--   0        0        0     1149 2024-04-16 21:23:27.826777 substrate-120240416.0.6/substrate/core/coregraph.py
+-rw-r--r--   0        0        0     2186 2024-04-16 21:25:37.773256 substrate-120240416.0.6/substrate/core/corenode.py
+-rw-r--r--   0        0        0     1227 2024-04-16 21:23:27.827149 substrate-120240416.0.6/substrate/core/future_directive.py
+-rw-r--r--   0        0        0      894 2024-04-16 21:23:27.825332 substrate-120240416.0.6/substrate/core/id_generator.py
+-rw-r--r--   0        0        0    38450 2024-04-16 21:25:37.773637 substrate-120240416.0.6/substrate/core/models.py
+-rw-r--r--   0        0        0     2332 2024-04-16 21:23:27.825185 substrate-120240416.0.6/substrate/core/sb.py
+-rw-r--r--   0        0        0    32587 2024-04-16 21:25:37.774019 substrate-120240416.0.6/substrate/dataclass_models.py
+-rw-r--r--   0        0        0    43578 2024-04-16 21:25:37.774619 substrate-120240416.0.6/substrate/future_dataclass_models.py
+-rw-r--r--   0        0        0    40555 2024-04-16 21:25:37.774957 substrate-120240416.0.6/substrate/nodes.py
+-rw-r--r--   0        0        0        0 2024-02-07 23:39:17.000078 substrate-120240416.0.6/substrate/py.typed
+-rw-r--r--   0        0        0     1490 2024-04-16 20:07:00.739577 substrate-120240416.0.6/substrate/substrate.py
+-rw-r--r--   0        0        0     1034 2024-04-16 21:25:37.775283 substrate-120240416.0.6/substrate/substrate_response.py
+-rw-r--r--   0        0        0    35749 2024-04-16 21:25:37.775828 substrate-120240416.0.6/substrate/typeddict_models.py
+-rw-r--r--   0        0        0      648 1970-01-01 00:00:00.000000 substrate-120240416.0.6/PKG-INFO
```

### Comparing `substrate-120240416.0.5/LICENSE` & `substrate-120240416.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `substrate-120240416.0.5/pyproject.toml` & `substrate-120240416.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "substrate"
-version = "120240416.0.5"
+version = "120240416.0.6"
 description = "Substrate Python SDK"
 readme = "README.md"
 authors = [ "vprtwn <ben@substrate.run>", "liamgriffiths <liam@substrate.run>",]
 [[tool.poetry.packages]]
 include = "substrate"
 
 [tool.pyright]
```

### Comparing `substrate-120240416.0.5/substrate/__init__.py` & `substrate-120240416.0.6/substrate/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,19 +44,18 @@
     StableDiffusionXLInpaint,
     StableDiffusionXLIPAdapter,
     StableDiffusionXLLightning,
     StableDiffusionXLControlNet,
 )
 from .core.sb import sb
 from ._version import __version__
-from .substrate import Substrate, AsyncSubstrate, SubstrateResponse
+from .substrate import Substrate, SubstrateResponse
 
 __all__ = [
     "__version__",
-    "AsyncSubstrate",
     "SubstrateResponse",
     "sb",
     "Substrate",
     "GenerateText",
     "MultiGenerateText",
     "GenerateJSON",
     "MultiGenerateJSON",
```

### Comparing `substrate-120240416.0.5/substrate/_client.py` & `substrate-120240416.0.6/substrate/_client.py`

 * *Files identical despite different names*

### Comparing `substrate-120240416.0.5/substrate/core/base_future.py` & `substrate-120240416.0.6/substrate/core/base_future.py`

 * *Files identical despite different names*

### Comparing `substrate-120240416.0.5/substrate/core/client/find_futures_client.py` & `substrate-120240416.0.6/substrate/core/client/find_futures_client.py`

 * *Files identical despite different names*

### Comparing `substrate-120240416.0.5/substrate/core/client/future.py` & `substrate-120240416.0.6/substrate/core/client/future.py`

 * *Files identical despite different names*

### Comparing `substrate-120240416.0.5/substrate/core/client/graph.py` & `substrate-120240416.0.6/substrate/core/client/graph.py`

 * *Files identical despite different names*

### Comparing `substrate-120240416.0.5/substrate/core/coregraph.py` & `substrate-120240416.0.6/substrate/core/coregraph.py`

 * *Files identical despite different names*

### Comparing `substrate-120240416.0.5/substrate/core/corenode.py` & `substrate-120240416.0.6/substrate/core/corenode.py`

 * *Files identical despite different names*

### Comparing `substrate-120240416.0.5/substrate/core/future_directive.py` & `substrate-120240416.0.6/substrate/core/future_directive.py`

 * *Files identical despite different names*

### Comparing `substrate-120240416.0.5/substrate/core/id_generator.py` & `substrate-120240416.0.6/substrate/core/id_generator.py`

 * *Files identical despite different names*

### Comparing `substrate-120240416.0.5/substrate/core/models.py` & `substrate-120240416.0.6/substrate/core/models.py`

 * *Files identical despite different names*

### Comparing `substrate-120240416.0.5/substrate/core/sb.py` & `substrate-120240416.0.6/substrate/core/sb.py`

 * *Files identical despite different names*

### Comparing `substrate-120240416.0.5/substrate/dataclass_models.py` & `substrate-120240416.0.6/substrate/dataclass_models.py`

 * *Files identical despite different names*

### Comparing `substrate-120240416.0.5/substrate/future_dataclass_models.py` & `substrate-120240416.0.6/substrate/future_dataclass_models.py`

 * *Files identical despite different names*

### Comparing `substrate-120240416.0.5/substrate/nodes.py` & `substrate-120240416.0.6/substrate/nodes.py`

 * *Files identical despite different names*

### Comparing `substrate-120240416.0.5/substrate/substrate.py` & `substrate-120240416.0.6/substrate/substrate.py`

 * *Files identical despite different names*

### Comparing `substrate-120240416.0.5/substrate/substrate_response.py` & `substrate-120240416.0.6/substrate/substrate_response.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from typing import Any, Dict, Optional, TypeVar, Type, Union
-from .core.corenode import CoreNode
-from ._client import APIResponse
+from typing import Any, Dict, Type, TypeVar, Optional
 
+from ._client import APIResponse
+from .core.corenode import CoreNode
 
 T = TypeVar("T", bound=Any)
 
 
 class SubstrateResponse:
     """
     Substrate run response.
```

### Comparing `substrate-120240416.0.5/substrate/typeddict_models.py` & `substrate-120240416.0.6/substrate/typeddict_models.py`

 * *Files identical despite different names*

### Comparing `substrate-120240416.0.5/PKG-INFO` & `substrate-120240416.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: substrate
-Version: 120240416.0.5
+Version: 120240416.0.6
 Summary: Substrate Python SDK
 Author: vprtwn
 Author-email: ben@substrate.run
 Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

