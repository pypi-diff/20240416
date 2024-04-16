# Comparing `tmp/mypy_boto3_outposts-1.34.84.tar.gz` & `tmp/mypy_boto3_outposts-1.34.85.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy_boto3_outposts-1.34.84.tar", last modified: Fri Apr 12 19:32:37 2024, max compression
+gzip compressed data, was "mypy_boto3_outposts-1.34.85.tar", last modified: Tue Apr 16 19:33:16 2024, max compression
```

## Comparing `mypy_boto3_outposts-1.34.84.tar` & `mypy_boto3_outposts-1.34.85.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:32:37.957303 mypy_boto3_outposts-1.34.84/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-12 19:32:13.000000 mypy_boto3_outposts-1.34.84/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13323 2024-04-12 19:32:37.957303 mypy_boto3_outposts-1.34.84/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11764 2024-04-12 19:32:13.000000 mypy_boto3_outposts-1.34.84/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:32:37.957303 mypy_boto3_outposts-1.34.84/mypy_boto3_outposts/
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-12 19:32:13.000000 mypy_boto3_outposts-1.34.84/mypy_boto3_outposts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-12 19:32:13.000000 mypy_boto3_outposts-1.34.84/mypy_boto3_outposts/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-12 19:32:13.000000 mypy_boto3_outposts-1.34.84/mypy_boto3_outposts/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21432 2024-04-12 19:32:13.000000 mypy_boto3_outposts-1.34.84/mypy_boto3_outposts/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    21429 2024-04-12 19:32:13.000000 mypy_boto3_outposts-1.34.84/mypy_boto3_outposts/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12283 2024-04-12 19:32:13.000000 mypy_boto3_outposts-1.34.84/mypy_boto3_outposts/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    12283 2024-04-12 19:32:13.000000 mypy_boto3_outposts-1.34.84/mypy_boto3_outposts/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7749 2024-04-12 19:32:13.000000 mypy_boto3_outposts-1.34.84/mypy_boto3_outposts/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7742 2024-04-12 19:32:13.000000 mypy_boto3_outposts-1.34.84/mypy_boto3_outposts/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 19:32:13.000000 mypy_boto3_outposts-1.34.84/mypy_boto3_outposts/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    22928 2024-04-12 19:32:14.000000 mypy_boto3_outposts-1.34.84/mypy_boto3_outposts/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    22928 2024-04-12 19:32:14.000000 mypy_boto3_outposts-1.34.84/mypy_boto3_outposts/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-12 19:32:13.000000 mypy_boto3_outposts-1.34.84/mypy_boto3_outposts/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:32:37.957303 mypy_boto3_outposts-1.34.84/mypy_boto3_outposts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13323 2024-04-12 19:32:37.000000 mypy_boto3_outposts-1.34.84/mypy_boto3_outposts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-12 19:32:37.000000 mypy_boto3_outposts-1.34.84/mypy_boto3_outposts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 19:32:37.000000 mypy_boto3_outposts-1.34.84/mypy_boto3_outposts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 19:32:37.000000 mypy_boto3_outposts-1.34.84/mypy_boto3_outposts.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-12 19:32:37.000000 mypy_boto3_outposts-1.34.84/mypy_boto3_outposts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-12 19:32:37.000000 mypy_boto3_outposts-1.34.84/mypy_boto3_outposts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 19:32:37.957303 mypy_boto3_outposts-1.34.84/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-12 19:32:13.000000 mypy_boto3_outposts-1.34.84/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:33:16.820333 mypy_boto3_outposts-1.34.85/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-16 19:33:00.000000 mypy_boto3_outposts-1.34.85/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13673 2024-04-16 19:33:16.820333 mypy_boto3_outposts-1.34.85/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12114 2024-04-16 19:33:00.000000 mypy_boto3_outposts-1.34.85/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:33:16.816333 mypy_boto3_outposts-1.34.85/mypy_boto3_outposts/
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-16 19:33:00.000000 mypy_boto3_outposts-1.34.85/mypy_boto3_outposts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-16 19:33:00.000000 mypy_boto3_outposts-1.34.85/mypy_boto3_outposts/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-16 19:33:00.000000 mypy_boto3_outposts-1.34.85/mypy_boto3_outposts/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25524 2024-04-16 19:33:00.000000 mypy_boto3_outposts-1.34.85/mypy_boto3_outposts/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25521 2024-04-16 19:33:00.000000 mypy_boto3_outposts-1.34.85/mypy_boto3_outposts/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12843 2024-04-16 19:33:00.000000 mypy_boto3_outposts-1.34.85/mypy_boto3_outposts/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12843 2024-04-16 19:33:00.000000 mypy_boto3_outposts-1.34.85/mypy_boto3_outposts/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10290 2024-04-16 19:33:00.000000 mypy_boto3_outposts-1.34.85/mypy_boto3_outposts/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10281 2024-04-16 19:33:00.000000 mypy_boto3_outposts-1.34.85/mypy_boto3_outposts/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 19:33:00.000000 mypy_boto3_outposts-1.34.85/mypy_boto3_outposts/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    27810 2024-04-16 19:33:01.000000 mypy_boto3_outposts-1.34.85/mypy_boto3_outposts/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27810 2024-04-16 19:33:00.000000 mypy_boto3_outposts-1.34.85/mypy_boto3_outposts/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-16 19:33:00.000000 mypy_boto3_outposts-1.34.85/mypy_boto3_outposts/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:33:16.820333 mypy_boto3_outposts-1.34.85/mypy_boto3_outposts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13673 2024-04-16 19:33:16.000000 mypy_boto3_outposts-1.34.85/mypy_boto3_outposts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-16 19:33:16.000000 mypy_boto3_outposts-1.34.85/mypy_boto3_outposts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 19:33:16.000000 mypy_boto3_outposts-1.34.85/mypy_boto3_outposts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 19:33:16.000000 mypy_boto3_outposts-1.34.85/mypy_boto3_outposts.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-16 19:33:16.000000 mypy_boto3_outposts-1.34.85/mypy_boto3_outposts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-16 19:33:16.000000 mypy_boto3_outposts-1.34.85/mypy_boto3_outposts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 19:33:16.820333 mypy_boto3_outposts-1.34.85/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-16 19:33:00.000000 mypy_boto3_outposts-1.34.85/setup.py
```

### Comparing `mypy_boto3_outposts-1.34.84/LICENSE` & `mypy_boto3_outposts-1.34.85/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy_boto3_outposts-1.34.84/PKG-INFO` & `mypy_boto3_outposts-1.34.85/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-outposts
-Version: 1.34.84
-Summary: Type annotations for boto3.Outposts 1.34.84 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.85
+Summary: Type annotations for boto3.Outposts 1.34.85 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-outposts.svg?color=blue)](https://pypi.org/project/mypy-boto3-outposts)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-outposts)](https://pepy.tech/project/mypy-boto3-outposts)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Outposts 1.34.84](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts)
+[boto3.Outposts 1.34.85](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -281,29 +281,37 @@
 
 ```python
 from boto3.session import Session
 
 from mypy_boto3_outposts import OutpostsClient
 from mypy_boto3_outposts.paginator import (
     GetOutpostInstanceTypesPaginator,
+    GetOutpostSupportedInstanceTypesPaginator,
     ListAssetsPaginator,
+    ListCapacityTasksPaginator,
     ListCatalogItemsPaginator,
     ListOrdersPaginator,
     ListOutpostsPaginator,
     ListSitesPaginator,
 )
 
 client: OutpostsClient = Session().client("outposts")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
 get_outpost_instance_types_paginator: GetOutpostInstanceTypesPaginator = client.get_paginator(
     "get_outpost_instance_types"
 )
+get_outpost_supported_instance_types_paginator: GetOutpostSupportedInstanceTypesPaginator = (
+    client.get_paginator("get_outpost_supported_instance_types")
+)
 list_assets_paginator: ListAssetsPaginator = client.get_paginator("list_assets")
+list_capacity_tasks_paginator: ListCapacityTasksPaginator = client.get_paginator(
+    "list_capacity_tasks"
+)
 list_catalog_items_paginator: ListCatalogItemsPaginator = client.get_paginator("list_catalog_items")
 list_orders_paginator: ListOrdersPaginator = client.get_paginator("list_orders")
 list_outposts_paginator: ListOutpostsPaginator = client.get_paginator("list_outposts")
 list_sites_paginator: ListSitesPaginator = client.get_paginator("list_sites")
 ```
 
 <a id="literals"></a>
```

### Comparing `mypy_boto3_outposts-1.34.84/README.md` & `mypy_boto3_outposts-1.34.85/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-outposts.svg?color=blue)](https://pypi.org/project/mypy-boto3-outposts)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-outposts)](https://pepy.tech/project/mypy-boto3-outposts)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Outposts 1.34.84](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts)
+[boto3.Outposts 1.34.85](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -248,29 +248,37 @@
 
 ```python
 from boto3.session import Session
 
 from mypy_boto3_outposts import OutpostsClient
 from mypy_boto3_outposts.paginator import (
     GetOutpostInstanceTypesPaginator,
+    GetOutpostSupportedInstanceTypesPaginator,
     ListAssetsPaginator,
+    ListCapacityTasksPaginator,
     ListCatalogItemsPaginator,
     ListOrdersPaginator,
     ListOutpostsPaginator,
     ListSitesPaginator,
 )
 
 client: OutpostsClient = Session().client("outposts")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
 get_outpost_instance_types_paginator: GetOutpostInstanceTypesPaginator = client.get_paginator(
     "get_outpost_instance_types"
 )
+get_outpost_supported_instance_types_paginator: GetOutpostSupportedInstanceTypesPaginator = (
+    client.get_paginator("get_outpost_supported_instance_types")
+)
 list_assets_paginator: ListAssetsPaginator = client.get_paginator("list_assets")
+list_capacity_tasks_paginator: ListCapacityTasksPaginator = client.get_paginator(
+    "list_capacity_tasks"
+)
 list_catalog_items_paginator: ListCatalogItemsPaginator = client.get_paginator("list_catalog_items")
 list_orders_paginator: ListOrdersPaginator = client.get_paginator("list_orders")
 list_outposts_paginator: ListOutpostsPaginator = client.get_paginator("list_outposts")
 list_sites_paginator: ListSitesPaginator = client.get_paginator("list_sites")
 ```
 
 <a id="literals"></a>
```

### Comparing `mypy_boto3_outposts-1.34.84/mypy_boto3_outposts/__init__.py` & `mypy_boto3_outposts-1.34.85/mypy_boto3_outposts/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,49 +4,57 @@
 Usage::
 
     ```python
     from boto3.session import Session
     from mypy_boto3_outposts import (
         Client,
         GetOutpostInstanceTypesPaginator,
+        GetOutpostSupportedInstanceTypesPaginator,
         ListAssetsPaginator,
+        ListCapacityTasksPaginator,
         ListCatalogItemsPaginator,
         ListOrdersPaginator,
         ListOutpostsPaginator,
         ListSitesPaginator,
         OutpostsClient,
     )
 
     session = Session()
     client: OutpostsClient = session.client("outposts")
 
     get_outpost_instance_types_paginator: GetOutpostInstanceTypesPaginator = client.get_paginator("get_outpost_instance_types")
+    get_outpost_supported_instance_types_paginator: GetOutpostSupportedInstanceTypesPaginator = client.get_paginator("get_outpost_supported_instance_types")
     list_assets_paginator: ListAssetsPaginator = client.get_paginator("list_assets")
+    list_capacity_tasks_paginator: ListCapacityTasksPaginator = client.get_paginator("list_capacity_tasks")
     list_catalog_items_paginator: ListCatalogItemsPaginator = client.get_paginator("list_catalog_items")
     list_orders_paginator: ListOrdersPaginator = client.get_paginator("list_orders")
     list_outposts_paginator: ListOutpostsPaginator = client.get_paginator("list_outposts")
     list_sites_paginator: ListSitesPaginator = client.get_paginator("list_sites")
     ```
 """
 
 from .client import OutpostsClient
 from .paginator import (
     GetOutpostInstanceTypesPaginator,
+    GetOutpostSupportedInstanceTypesPaginator,
     ListAssetsPaginator,
+    ListCapacityTasksPaginator,
     ListCatalogItemsPaginator,
     ListOrdersPaginator,
     ListOutpostsPaginator,
     ListSitesPaginator,
 )
 
 Client = OutpostsClient
 
 __all__ = (
     "Client",
     "GetOutpostInstanceTypesPaginator",
+    "GetOutpostSupportedInstanceTypesPaginator",
     "ListAssetsPaginator",
+    "ListCapacityTasksPaginator",
     "ListCatalogItemsPaginator",
     "ListOrdersPaginator",
     "ListOutpostsPaginator",
     "ListSitesPaginator",
     "OutpostsClient",
 )
```

### Comparing `mypy_boto3_outposts-1.34.84/mypy_boto3_outposts/__init__.pyi` & `mypy_boto3_outposts-1.34.85/mypy_boto3_outposts/__init__.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -4,49 +4,57 @@
 Usage::
 
     ```python
     from boto3.session import Session
     from mypy_boto3_outposts import (
         Client,
         GetOutpostInstanceTypesPaginator,
+        GetOutpostSupportedInstanceTypesPaginator,
         ListAssetsPaginator,
+        ListCapacityTasksPaginator,
         ListCatalogItemsPaginator,
         ListOrdersPaginator,
         ListOutpostsPaginator,
         ListSitesPaginator,
         OutpostsClient,
     )
 
     session = Session()
     client: OutpostsClient = session.client("outposts")
 
     get_outpost_instance_types_paginator: GetOutpostInstanceTypesPaginator = client.get_paginator("get_outpost_instance_types")
+    get_outpost_supported_instance_types_paginator: GetOutpostSupportedInstanceTypesPaginator = client.get_paginator("get_outpost_supported_instance_types")
     list_assets_paginator: ListAssetsPaginator = client.get_paginator("list_assets")
+    list_capacity_tasks_paginator: ListCapacityTasksPaginator = client.get_paginator("list_capacity_tasks")
     list_catalog_items_paginator: ListCatalogItemsPaginator = client.get_paginator("list_catalog_items")
     list_orders_paginator: ListOrdersPaginator = client.get_paginator("list_orders")
     list_outposts_paginator: ListOutpostsPaginator = client.get_paginator("list_outposts")
     list_sites_paginator: ListSitesPaginator = client.get_paginator("list_sites")
     ```
 """
 
 from .client import OutpostsClient
 from .paginator import (
     GetOutpostInstanceTypesPaginator,
+    GetOutpostSupportedInstanceTypesPaginator,
     ListAssetsPaginator,
+    ListCapacityTasksPaginator,
     ListCatalogItemsPaginator,
     ListOrdersPaginator,
     ListOutpostsPaginator,
     ListSitesPaginator,
 )
 
 Client = OutpostsClient
 
 __all__ = (
     "Client",
     "GetOutpostInstanceTypesPaginator",
+    "GetOutpostSupportedInstanceTypesPaginator",
     "ListAssetsPaginator",
+    "ListCapacityTasksPaginator",
     "ListCatalogItemsPaginator",
     "ListOrdersPaginator",
     "ListOutpostsPaginator",
     "ListSitesPaginator",
     "OutpostsClient",
 )
```

### Comparing `mypy_boto3_outposts-1.34.84/mypy_boto3_outposts/__main__.py` & `mypy_boto3_outposts-1.34.85/mypy_boto3_outposts/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Outposts 1.34.84\n"
-        "Version:         1.34.84\n"
+        "Type annotations for boto3.Outposts 1.34.85\n"
+        "Version:         1.34.85\n"
         "Builder version: 7.23.2\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.84")
+    print("1.34.85")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy_boto3_outposts-1.34.84/mypy_boto3_outposts/client.py` & `mypy_boto3_outposts-1.34.85/mypy_boto3_outposts/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AddressTypeType,
     AssetStateType,
+    CapacityTaskStatusType,
     CatalogItemClassType,
     FiberOpticCableTypeType,
     MaximumSupportedWeightLbsType,
     OpticalStandardType,
     PaymentOptionType,
     PaymentTermType,
     PowerConnectorType,
@@ -35,40 +36,47 @@
     SupportedHardwareTypeType,
     SupportedStorageEnumType,
     UplinkCountType,
     UplinkGbpsType,
 )
 from .paginator import (
     GetOutpostInstanceTypesPaginator,
+    GetOutpostSupportedInstanceTypesPaginator,
     ListAssetsPaginator,
+    ListCapacityTasksPaginator,
     ListCatalogItemsPaginator,
     ListOrdersPaginator,
     ListOutpostsPaginator,
     ListSitesPaginator,
 )
 from .type_defs import (
     AddressTypeDef,
     CreateOrderOutputTypeDef,
     CreateOutpostOutputTypeDef,
     CreateSiteOutputTypeDef,
+    GetCapacityTaskOutputTypeDef,
     GetCatalogItemOutputTypeDef,
     GetConnectionResponseTypeDef,
     GetOrderOutputTypeDef,
     GetOutpostInstanceTypesOutputTypeDef,
     GetOutpostOutputTypeDef,
+    GetOutpostSupportedInstanceTypesOutputTypeDef,
     GetSiteAddressOutputTypeDef,
     GetSiteOutputTypeDef,
+    InstanceTypeCapacityTypeDef,
     LineItemRequestTypeDef,
     ListAssetsOutputTypeDef,
+    ListCapacityTasksOutputTypeDef,
     ListCatalogItemsOutputTypeDef,
     ListOrdersOutputTypeDef,
     ListOutpostsOutputTypeDef,
     ListSitesOutputTypeDef,
     ListTagsForResourceResponseTypeDef,
     RackPhysicalPropertiesTypeDef,
+    StartCapacityTaskOutputTypeDef,
     StartConnectionResponseTypeDef,
     UpdateOutpostOutputTypeDef,
     UpdateSiteAddressOutputTypeDef,
     UpdateSiteOutputTypeDef,
     UpdateSiteRackPhysicalPropertiesOutputTypeDef,
 )
 
@@ -119,14 +127,24 @@
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/client/#can_paginate)
         """
 
+    def cancel_capacity_task(
+        self, *, CapacityTaskId: str, OutpostIdentifier: str
+    ) -> Dict[str, Any]:
+        """
+        Cancels the capacity task.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.cancel_capacity_task)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/client/#cancel_capacity_task)
+        """
+
     def cancel_order(self, *, OrderId: str) -> Dict[str, Any]:
         """
         Cancels the specified order for an Outpost.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.cancel_order)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/client/#cancel_order)
         """
@@ -216,14 +234,24 @@
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/client/#generate_presigned_url)
         """
 
+    def get_capacity_task(
+        self, *, CapacityTaskId: str, OutpostIdentifier: str
+    ) -> GetCapacityTaskOutputTypeDef:
+        """
+        Gets details of the specified capacity task.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.get_capacity_task)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/client/#get_capacity_task)
+        """
+
     def get_catalog_item(self, *, CatalogItemId: str) -> GetCatalogItemOutputTypeDef:
         """
         Gets information about the specified catalog item.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.get_catalog_item)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/client/#get_catalog_item)
         """
@@ -258,14 +286,24 @@
         """
         Gets the instance types for the specified Outpost.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.get_outpost_instance_types)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/client/#get_outpost_instance_types)
         """
 
+    def get_outpost_supported_instance_types(
+        self, *, OutpostIdentifier: str, OrderId: str, MaxResults: int = ..., NextToken: str = ...
+    ) -> GetOutpostSupportedInstanceTypesOutputTypeDef:
+        """
+        Gets the instance types that an Outpost can support in `InstanceTypeCapacity`.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.get_outpost_supported_instance_types)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/client/#get_outpost_supported_instance_types)
+        """
+
     def get_site(self, *, SiteId: str) -> GetSiteOutputTypeDef:
         """
         Gets information about the specified Outpost site.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.get_site)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/client/#get_site)
         """
@@ -292,14 +330,29 @@
         """
         Lists the hardware assets for the specified Outpost.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.list_assets)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/client/#list_assets)
         """
 
+    def list_capacity_tasks(
+        self,
+        *,
+        OutpostIdentifierFilter: str = ...,
+        MaxResults: int = ...,
+        NextToken: str = ...,
+        CapacityTaskStatusFilter: Sequence[CapacityTaskStatusType] = ...,
+    ) -> ListCapacityTasksOutputTypeDef:
+        """
+        Lists the capacity tasks for your Amazon Web Services account.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.list_capacity_tasks)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/client/#list_capacity_tasks)
+        """
+
     def list_catalog_items(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         ItemClassFilter: Sequence[CatalogItemClassType] = ...,
         SupportedStorageFilter: Sequence[SupportedStorageEnumType] = ...,
@@ -358,14 +411,29 @@
         """
         Lists the tags for the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/client/#list_tags_for_resource)
         """
 
+    def start_capacity_task(
+        self,
+        *,
+        OutpostIdentifier: str,
+        OrderId: str,
+        InstancePools: Sequence[InstanceTypeCapacityTypeDef],
+        DryRun: bool = ...,
+    ) -> StartCapacityTaskOutputTypeDef:
+        """
+        Starts the specified capacity task.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.start_capacity_task)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/client/#start_capacity_task)
+        """
+
     def start_connection(
         self,
         *,
         AssetId: str,
         ClientPublicKey: str,
         NetworkInterfaceDeviceIndex: int,
         DeviceSerialNumber: str = ...,
@@ -455,22 +523,40 @@
     ) -> GetOutpostInstanceTypesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/client/#get_paginator)
         """
 
     @overload
+    def get_paginator(
+        self, operation_name: Literal["get_outpost_supported_instance_types"]
+    ) -> GetOutpostSupportedInstanceTypesPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/client/#get_paginator)
+        """
+
+    @overload
     def get_paginator(self, operation_name: Literal["list_assets"]) -> ListAssetsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/client/#get_paginator)
         """
 
     @overload
     def get_paginator(
+        self, operation_name: Literal["list_capacity_tasks"]
+    ) -> ListCapacityTasksPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/client/#get_paginator)
+        """
+
+    @overload
+    def get_paginator(
         self, operation_name: Literal["list_catalog_items"]
     ) -> ListCatalogItemsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/client/#get_paginator)
         """
```

### Comparing `mypy_boto3_outposts-1.34.84/mypy_boto3_outposts/client.pyi` & `mypy_boto3_outposts-1.34.85/mypy_boto3_outposts/client.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AddressTypeType,
     AssetStateType,
+    CapacityTaskStatusType,
     CatalogItemClassType,
     FiberOpticCableTypeType,
     MaximumSupportedWeightLbsType,
     OpticalStandardType,
     PaymentOptionType,
     PaymentTermType,
     PowerConnectorType,
@@ -35,40 +36,47 @@
     SupportedHardwareTypeType,
     SupportedStorageEnumType,
     UplinkCountType,
     UplinkGbpsType,
 )
 from .paginator import (
     GetOutpostInstanceTypesPaginator,
+    GetOutpostSupportedInstanceTypesPaginator,
     ListAssetsPaginator,
+    ListCapacityTasksPaginator,
     ListCatalogItemsPaginator,
     ListOrdersPaginator,
     ListOutpostsPaginator,
     ListSitesPaginator,
 )
 from .type_defs import (
     AddressTypeDef,
     CreateOrderOutputTypeDef,
     CreateOutpostOutputTypeDef,
     CreateSiteOutputTypeDef,
+    GetCapacityTaskOutputTypeDef,
     GetCatalogItemOutputTypeDef,
     GetConnectionResponseTypeDef,
     GetOrderOutputTypeDef,
     GetOutpostInstanceTypesOutputTypeDef,
     GetOutpostOutputTypeDef,
+    GetOutpostSupportedInstanceTypesOutputTypeDef,
     GetSiteAddressOutputTypeDef,
     GetSiteOutputTypeDef,
+    InstanceTypeCapacityTypeDef,
     LineItemRequestTypeDef,
     ListAssetsOutputTypeDef,
+    ListCapacityTasksOutputTypeDef,
     ListCatalogItemsOutputTypeDef,
     ListOrdersOutputTypeDef,
     ListOutpostsOutputTypeDef,
     ListSitesOutputTypeDef,
     ListTagsForResourceResponseTypeDef,
     RackPhysicalPropertiesTypeDef,
+    StartCapacityTaskOutputTypeDef,
     StartConnectionResponseTypeDef,
     UpdateOutpostOutputTypeDef,
     UpdateSiteAddressOutputTypeDef,
     UpdateSiteOutputTypeDef,
     UpdateSiteRackPhysicalPropertiesOutputTypeDef,
 )
 
@@ -116,14 +124,24 @@
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/client/#can_paginate)
         """
 
+    def cancel_capacity_task(
+        self, *, CapacityTaskId: str, OutpostIdentifier: str
+    ) -> Dict[str, Any]:
+        """
+        Cancels the capacity task.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.cancel_capacity_task)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/client/#cancel_capacity_task)
+        """
+
     def cancel_order(self, *, OrderId: str) -> Dict[str, Any]:
         """
         Cancels the specified order for an Outpost.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.cancel_order)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/client/#cancel_order)
         """
@@ -213,14 +231,24 @@
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/client/#generate_presigned_url)
         """
 
+    def get_capacity_task(
+        self, *, CapacityTaskId: str, OutpostIdentifier: str
+    ) -> GetCapacityTaskOutputTypeDef:
+        """
+        Gets details of the specified capacity task.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.get_capacity_task)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/client/#get_capacity_task)
+        """
+
     def get_catalog_item(self, *, CatalogItemId: str) -> GetCatalogItemOutputTypeDef:
         """
         Gets information about the specified catalog item.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.get_catalog_item)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/client/#get_catalog_item)
         """
@@ -255,14 +283,24 @@
         """
         Gets the instance types for the specified Outpost.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.get_outpost_instance_types)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/client/#get_outpost_instance_types)
         """
 
+    def get_outpost_supported_instance_types(
+        self, *, OutpostIdentifier: str, OrderId: str, MaxResults: int = ..., NextToken: str = ...
+    ) -> GetOutpostSupportedInstanceTypesOutputTypeDef:
+        """
+        Gets the instance types that an Outpost can support in `InstanceTypeCapacity`.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.get_outpost_supported_instance_types)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/client/#get_outpost_supported_instance_types)
+        """
+
     def get_site(self, *, SiteId: str) -> GetSiteOutputTypeDef:
         """
         Gets information about the specified Outpost site.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.get_site)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/client/#get_site)
         """
@@ -289,14 +327,29 @@
         """
         Lists the hardware assets for the specified Outpost.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.list_assets)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/client/#list_assets)
         """
 
+    def list_capacity_tasks(
+        self,
+        *,
+        OutpostIdentifierFilter: str = ...,
+        MaxResults: int = ...,
+        NextToken: str = ...,
+        CapacityTaskStatusFilter: Sequence[CapacityTaskStatusType] = ...,
+    ) -> ListCapacityTasksOutputTypeDef:
+        """
+        Lists the capacity tasks for your Amazon Web Services account.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.list_capacity_tasks)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/client/#list_capacity_tasks)
+        """
+
     def list_catalog_items(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         ItemClassFilter: Sequence[CatalogItemClassType] = ...,
         SupportedStorageFilter: Sequence[SupportedStorageEnumType] = ...,
@@ -355,14 +408,29 @@
         """
         Lists the tags for the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/client/#list_tags_for_resource)
         """
 
+    def start_capacity_task(
+        self,
+        *,
+        OutpostIdentifier: str,
+        OrderId: str,
+        InstancePools: Sequence[InstanceTypeCapacityTypeDef],
+        DryRun: bool = ...,
+    ) -> StartCapacityTaskOutputTypeDef:
+        """
+        Starts the specified capacity task.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.start_capacity_task)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/client/#start_capacity_task)
+        """
+
     def start_connection(
         self,
         *,
         AssetId: str,
         ClientPublicKey: str,
         NetworkInterfaceDeviceIndex: int,
         DeviceSerialNumber: str = ...,
@@ -452,22 +520,40 @@
     ) -> GetOutpostInstanceTypesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/client/#get_paginator)
         """
 
     @overload
+    def get_paginator(
+        self, operation_name: Literal["get_outpost_supported_instance_types"]
+    ) -> GetOutpostSupportedInstanceTypesPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/client/#get_paginator)
+        """
+
+    @overload
     def get_paginator(self, operation_name: Literal["list_assets"]) -> ListAssetsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/client/#get_paginator)
         """
 
     @overload
     def get_paginator(
+        self, operation_name: Literal["list_capacity_tasks"]
+    ) -> ListCapacityTasksPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/client/#get_paginator)
+        """
+
+    @overload
+    def get_paginator(
         self, operation_name: Literal["list_catalog_items"]
     ) -> ListCatalogItemsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/client/#get_paginator)
         """
```

### Comparing `mypy_boto3_outposts-1.34.84/mypy_boto3_outposts/literals.py` & `mypy_boto3_outposts-1.34.85/mypy_boto3_outposts/literals.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,21 +19,25 @@
 else:
     from typing_extensions import Literal
 
 __all__ = (
     "AddressTypeType",
     "AssetStateType",
     "AssetTypeType",
+    "CapacityTaskFailureTypeType",
+    "CapacityTaskStatusType",
     "CatalogItemClassType",
     "CatalogItemStatusType",
     "ComputeAssetStateType",
     "FiberOpticCableTypeType",
     "GetOutpostInstanceTypesPaginatorName",
+    "GetOutpostSupportedInstanceTypesPaginatorName",
     "LineItemStatusType",
     "ListAssetsPaginatorName",
+    "ListCapacityTasksPaginatorName",
     "ListCatalogItemsPaginatorName",
     "ListOrdersPaginatorName",
     "ListOutpostsPaginatorName",
     "ListSitesPaginatorName",
     "MaximumSupportedWeightLbsType",
     "OpticalStandardType",
     "OrderStatusType",
@@ -55,31 +59,35 @@
     "PaginatorName",
     "RegionName",
 )
 
 AddressTypeType = Literal["OPERATING_ADDRESS", "SHIPPING_ADDRESS"]
 AssetStateType = Literal["ACTIVE", "ISOLATED", "RETIRING"]
 AssetTypeType = Literal["COMPUTE"]
+CapacityTaskFailureTypeType = Literal["UNSUPPORTED_CAPACITY_CONFIGURATION"]
+CapacityTaskStatusType = Literal["CANCELLED", "COMPLETED", "FAILED", "IN_PROGRESS", "REQUESTED"]
 CatalogItemClassType = Literal["RACK", "SERVER"]
 CatalogItemStatusType = Literal["AVAILABLE", "DISCONTINUED"]
 ComputeAssetStateType = Literal["ACTIVE", "ISOLATED", "RETIRING"]
 FiberOpticCableTypeType = Literal["MULTI_MODE", "SINGLE_MODE"]
 GetOutpostInstanceTypesPaginatorName = Literal["get_outpost_instance_types"]
+GetOutpostSupportedInstanceTypesPaginatorName = Literal["get_outpost_supported_instance_types"]
 LineItemStatusType = Literal[
     "BUILDING",
     "CANCELLED",
     "DELIVERED",
     "ERROR",
     "INSTALLED",
     "INSTALLING",
     "PREPARING",
     "REPLACED",
     "SHIPPED",
 ]
 ListAssetsPaginatorName = Literal["list_assets"]
+ListCapacityTasksPaginatorName = Literal["list_capacity_tasks"]
 ListCatalogItemsPaginatorName = Literal["list_catalog_items"]
 ListOrdersPaginatorName = Literal["list_orders"]
 ListOutpostsPaginatorName = Literal["list_outposts"]
 ListSitesPaginatorName = Literal["list_sites"]
 MaximumSupportedWeightLbsType = Literal[
     "MAX_1400_LBS", "MAX_1600_LBS", "MAX_1800_LBS", "MAX_2000_LBS", "NO_LIMIT"
 ]
@@ -528,15 +536,17 @@
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
 PaginatorName = Literal[
     "get_outpost_instance_types",
+    "get_outpost_supported_instance_types",
     "list_assets",
+    "list_capacity_tasks",
     "list_catalog_items",
     "list_orders",
     "list_outposts",
     "list_sites",
 ]
 RegionName = Literal[
     "af-south-1",
```

### Comparing `mypy_boto3_outposts-1.34.84/mypy_boto3_outposts/literals.pyi` & `mypy_boto3_outposts-1.34.85/mypy_boto3_outposts/literals.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -19,21 +19,25 @@
 else:
     from typing_extensions import Literal
 
 __all__ = (
     "AddressTypeType",
     "AssetStateType",
     "AssetTypeType",
+    "CapacityTaskFailureTypeType",
+    "CapacityTaskStatusType",
     "CatalogItemClassType",
     "CatalogItemStatusType",
     "ComputeAssetStateType",
     "FiberOpticCableTypeType",
     "GetOutpostInstanceTypesPaginatorName",
+    "GetOutpostSupportedInstanceTypesPaginatorName",
     "LineItemStatusType",
     "ListAssetsPaginatorName",
+    "ListCapacityTasksPaginatorName",
     "ListCatalogItemsPaginatorName",
     "ListOrdersPaginatorName",
     "ListOutpostsPaginatorName",
     "ListSitesPaginatorName",
     "MaximumSupportedWeightLbsType",
     "OpticalStandardType",
     "OrderStatusType",
@@ -55,31 +59,35 @@
     "PaginatorName",
     "RegionName",
 )
 
 AddressTypeType = Literal["OPERATING_ADDRESS", "SHIPPING_ADDRESS"]
 AssetStateType = Literal["ACTIVE", "ISOLATED", "RETIRING"]
 AssetTypeType = Literal["COMPUTE"]
+CapacityTaskFailureTypeType = Literal["UNSUPPORTED_CAPACITY_CONFIGURATION"]
+CapacityTaskStatusType = Literal["CANCELLED", "COMPLETED", "FAILED", "IN_PROGRESS", "REQUESTED"]
 CatalogItemClassType = Literal["RACK", "SERVER"]
 CatalogItemStatusType = Literal["AVAILABLE", "DISCONTINUED"]
 ComputeAssetStateType = Literal["ACTIVE", "ISOLATED", "RETIRING"]
 FiberOpticCableTypeType = Literal["MULTI_MODE", "SINGLE_MODE"]
 GetOutpostInstanceTypesPaginatorName = Literal["get_outpost_instance_types"]
+GetOutpostSupportedInstanceTypesPaginatorName = Literal["get_outpost_supported_instance_types"]
 LineItemStatusType = Literal[
     "BUILDING",
     "CANCELLED",
     "DELIVERED",
     "ERROR",
     "INSTALLED",
     "INSTALLING",
     "PREPARING",
     "REPLACED",
     "SHIPPED",
 ]
 ListAssetsPaginatorName = Literal["list_assets"]
+ListCapacityTasksPaginatorName = Literal["list_capacity_tasks"]
 ListCatalogItemsPaginatorName = Literal["list_catalog_items"]
 ListOrdersPaginatorName = Literal["list_orders"]
 ListOutpostsPaginatorName = Literal["list_outposts"]
 ListSitesPaginatorName = Literal["list_sites"]
 MaximumSupportedWeightLbsType = Literal[
     "MAX_1400_LBS", "MAX_1600_LBS", "MAX_1800_LBS", "MAX_2000_LBS", "NO_LIMIT"
 ]
@@ -528,15 +536,17 @@
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
 PaginatorName = Literal[
     "get_outpost_instance_types",
+    "get_outpost_supported_instance_types",
     "list_assets",
+    "list_capacity_tasks",
     "list_catalog_items",
     "list_orders",
     "list_outposts",
     "list_sites",
 ]
 RegionName = Literal[
     "af-south-1",
```

### Comparing `mypy_boto3_outposts-1.34.84/mypy_boto3_outposts/paginator.py` & `mypy_boto3_outposts-1.34.85/mypy_boto3_outposts/paginator.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,51 +7,64 @@
 
     ```python
     from boto3.session import Session
 
     from mypy_boto3_outposts.client import OutpostsClient
     from mypy_boto3_outposts.paginator import (
         GetOutpostInstanceTypesPaginator,
+        GetOutpostSupportedInstanceTypesPaginator,
         ListAssetsPaginator,
+        ListCapacityTasksPaginator,
         ListCatalogItemsPaginator,
         ListOrdersPaginator,
         ListOutpostsPaginator,
         ListSitesPaginator,
     )
 
     session = Session()
     client: OutpostsClient = session.client("outposts")
 
     get_outpost_instance_types_paginator: GetOutpostInstanceTypesPaginator = client.get_paginator("get_outpost_instance_types")
+    get_outpost_supported_instance_types_paginator: GetOutpostSupportedInstanceTypesPaginator = client.get_paginator("get_outpost_supported_instance_types")
     list_assets_paginator: ListAssetsPaginator = client.get_paginator("list_assets")
+    list_capacity_tasks_paginator: ListCapacityTasksPaginator = client.get_paginator("list_capacity_tasks")
     list_catalog_items_paginator: ListCatalogItemsPaginator = client.get_paginator("list_catalog_items")
     list_orders_paginator: ListOrdersPaginator = client.get_paginator("list_orders")
     list_outposts_paginator: ListOutpostsPaginator = client.get_paginator("list_outposts")
     list_sites_paginator: ListSitesPaginator = client.get_paginator("list_sites")
     ```
 """
 
 from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
-from .literals import AssetStateType, CatalogItemClassType, SupportedStorageEnumType
+from .literals import (
+    AssetStateType,
+    CapacityTaskStatusType,
+    CatalogItemClassType,
+    SupportedStorageEnumType,
+)
 from .type_defs import (
     GetOutpostInstanceTypesOutputTypeDef,
+    GetOutpostSupportedInstanceTypesOutputTypeDef,
     ListAssetsOutputTypeDef,
+    ListCapacityTasksOutputTypeDef,
     ListCatalogItemsOutputTypeDef,
     ListOrdersOutputTypeDef,
     ListOutpostsOutputTypeDef,
     ListSitesOutputTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = (
     "GetOutpostInstanceTypesPaginator",
+    "GetOutpostSupportedInstanceTypesPaginator",
     "ListAssetsPaginator",
+    "ListCapacityTasksPaginator",
     "ListCatalogItemsPaginator",
     "ListOrdersPaginator",
     "ListOutpostsPaginator",
     "ListSitesPaginator",
 )
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
@@ -75,14 +88,33 @@
     ) -> _PageIterator[GetOutpostInstanceTypesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Paginator.GetOutpostInstanceTypes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/paginators/#getoutpostinstancetypespaginator)
         """
 
 
+class GetOutpostSupportedInstanceTypesPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Paginator.GetOutpostSupportedInstanceTypes)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/paginators/#getoutpostsupportedinstancetypespaginator)
+    """
+
+    def paginate(
+        self,
+        *,
+        OutpostIdentifier: str,
+        OrderId: str,
+        PaginationConfig: PaginatorConfigTypeDef = ...,
+    ) -> _PageIterator[GetOutpostSupportedInstanceTypesOutputTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Paginator.GetOutpostSupportedInstanceTypes.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/paginators/#getoutpostsupportedinstancetypespaginator)
+        """
+
+
 class ListAssetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Paginator.ListAssets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/paginators/#listassetspaginator)
     """
 
     def paginate(
@@ -95,14 +127,33 @@
     ) -> _PageIterator[ListAssetsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Paginator.ListAssets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/paginators/#listassetspaginator)
         """
 
 
+class ListCapacityTasksPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Paginator.ListCapacityTasks)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/paginators/#listcapacitytaskspaginator)
+    """
+
+    def paginate(
+        self,
+        *,
+        OutpostIdentifierFilter: str = ...,
+        CapacityTaskStatusFilter: Sequence[CapacityTaskStatusType] = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...,
+    ) -> _PageIterator[ListCapacityTasksOutputTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Paginator.ListCapacityTasks.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/paginators/#listcapacitytaskspaginator)
+        """
+
+
 class ListCatalogItemsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Paginator.ListCatalogItems)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/paginators/#listcatalogitemspaginator)
     """
 
     def paginate(
```

### Comparing `mypy_boto3_outposts-1.34.84/mypy_boto3_outposts/paginator.pyi` & `mypy_boto3_outposts-1.34.85/mypy_boto3_outposts/paginator.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -7,51 +7,64 @@
 
     ```python
     from boto3.session import Session
 
     from mypy_boto3_outposts.client import OutpostsClient
     from mypy_boto3_outposts.paginator import (
         GetOutpostInstanceTypesPaginator,
+        GetOutpostSupportedInstanceTypesPaginator,
         ListAssetsPaginator,
+        ListCapacityTasksPaginator,
         ListCatalogItemsPaginator,
         ListOrdersPaginator,
         ListOutpostsPaginator,
         ListSitesPaginator,
     )
 
     session = Session()
     client: OutpostsClient = session.client("outposts")
 
     get_outpost_instance_types_paginator: GetOutpostInstanceTypesPaginator = client.get_paginator("get_outpost_instance_types")
+    get_outpost_supported_instance_types_paginator: GetOutpostSupportedInstanceTypesPaginator = client.get_paginator("get_outpost_supported_instance_types")
     list_assets_paginator: ListAssetsPaginator = client.get_paginator("list_assets")
+    list_capacity_tasks_paginator: ListCapacityTasksPaginator = client.get_paginator("list_capacity_tasks")
     list_catalog_items_paginator: ListCatalogItemsPaginator = client.get_paginator("list_catalog_items")
     list_orders_paginator: ListOrdersPaginator = client.get_paginator("list_orders")
     list_outposts_paginator: ListOutpostsPaginator = client.get_paginator("list_outposts")
     list_sites_paginator: ListSitesPaginator = client.get_paginator("list_sites")
     ```
 """
 
 from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
-from .literals import AssetStateType, CatalogItemClassType, SupportedStorageEnumType
+from .literals import (
+    AssetStateType,
+    CapacityTaskStatusType,
+    CatalogItemClassType,
+    SupportedStorageEnumType,
+)
 from .type_defs import (
     GetOutpostInstanceTypesOutputTypeDef,
+    GetOutpostSupportedInstanceTypesOutputTypeDef,
     ListAssetsOutputTypeDef,
+    ListCapacityTasksOutputTypeDef,
     ListCatalogItemsOutputTypeDef,
     ListOrdersOutputTypeDef,
     ListOutpostsOutputTypeDef,
     ListSitesOutputTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = (
     "GetOutpostInstanceTypesPaginator",
+    "GetOutpostSupportedInstanceTypesPaginator",
     "ListAssetsPaginator",
+    "ListCapacityTasksPaginator",
     "ListCatalogItemsPaginator",
     "ListOrdersPaginator",
     "ListOutpostsPaginator",
     "ListSitesPaginator",
 )
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
@@ -72,14 +85,32 @@
         self, *, OutpostId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetOutpostInstanceTypesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Paginator.GetOutpostInstanceTypes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/paginators/#getoutpostinstancetypespaginator)
         """
 
+class GetOutpostSupportedInstanceTypesPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Paginator.GetOutpostSupportedInstanceTypes)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/paginators/#getoutpostsupportedinstancetypespaginator)
+    """
+
+    def paginate(
+        self,
+        *,
+        OutpostIdentifier: str,
+        OrderId: str,
+        PaginationConfig: PaginatorConfigTypeDef = ...,
+    ) -> _PageIterator[GetOutpostSupportedInstanceTypesOutputTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Paginator.GetOutpostSupportedInstanceTypes.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/paginators/#getoutpostsupportedinstancetypespaginator)
+        """
+
 class ListAssetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Paginator.ListAssets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/paginators/#listassetspaginator)
     """
 
     def paginate(
@@ -91,14 +122,32 @@
         PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListAssetsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Paginator.ListAssets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/paginators/#listassetspaginator)
         """
 
+class ListCapacityTasksPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Paginator.ListCapacityTasks)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/paginators/#listcapacitytaskspaginator)
+    """
+
+    def paginate(
+        self,
+        *,
+        OutpostIdentifierFilter: str = ...,
+        CapacityTaskStatusFilter: Sequence[CapacityTaskStatusType] = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...,
+    ) -> _PageIterator[ListCapacityTasksOutputTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Paginator.ListCapacityTasks.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/paginators/#listcapacitytaskspaginator)
+        """
+
 class ListCatalogItemsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Paginator.ListCatalogItems)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/paginators/#listcatalogitemspaginator)
     """
 
     def paginate(
```

### Comparing `mypy_boto3_outposts-1.34.84/mypy_boto3_outposts/type_defs.py` & `mypy_boto3_outposts-1.34.85/mypy_boto3_outposts/type_defs.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AddressTypeType,
     AssetStateType,
+    CapacityTaskStatusType,
     CatalogItemClassType,
     CatalogItemStatusType,
     ComputeAssetStateType,
     FiberOpticCableTypeType,
     LineItemStatusType,
     MaximumSupportedWeightLbsType,
     OpticalStandardType,
@@ -54,36 +55,43 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AddressTypeDef",
     "AssetLocationTypeDef",
     "ComputeAttributesTypeDef",
+    "CancelCapacityTaskInputRequestTypeDef",
     "CancelOrderInputRequestTypeDef",
+    "CapacityTaskFailureTypeDef",
+    "CapacityTaskSummaryTypeDef",
     "EC2CapacityTypeDef",
     "ConnectionDetailsTypeDef",
     "LineItemRequestTypeDef",
     "ResponseMetadataTypeDef",
     "CreateOutpostInputRequestTypeDef",
     "OutpostTypeDef",
     "RackPhysicalPropertiesTypeDef",
     "DeleteOutpostInputRequestTypeDef",
     "DeleteSiteInputRequestTypeDef",
+    "GetCapacityTaskInputRequestTypeDef",
+    "InstanceTypeCapacityTypeDef",
     "GetCatalogItemInputRequestTypeDef",
     "GetConnectionRequestRequestTypeDef",
     "GetOrderInputRequestTypeDef",
     "GetOutpostInputRequestTypeDef",
     "PaginatorConfigTypeDef",
     "GetOutpostInstanceTypesInputRequestTypeDef",
     "InstanceTypeItemTypeDef",
+    "GetOutpostSupportedInstanceTypesInputRequestTypeDef",
     "GetSiteAddressInputRequestTypeDef",
     "GetSiteInputRequestTypeDef",
     "LineItemAssetInformationTypeDef",
     "ShipmentInformationTypeDef",
     "ListAssetsInputRequestTypeDef",
+    "ListCapacityTasksInputRequestTypeDef",
     "ListCatalogItemsInputRequestTypeDef",
     "ListOrdersInputRequestTypeDef",
     "OrderSummaryTypeDef",
     "ListOutpostsInputRequestTypeDef",
     "ListSitesInputRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "StartConnectionRequestRequestTypeDef",
@@ -94,30 +102,37 @@
     "UpdateSiteRackPhysicalPropertiesInputRequestTypeDef",
     "UpdateSiteAddressInputRequestTypeDef",
     "AssetInfoTypeDef",
     "CatalogItemTypeDef",
     "CreateOrderInputRequestTypeDef",
     "GetConnectionResponseTypeDef",
     "GetSiteAddressOutputTypeDef",
+    "ListCapacityTasksOutputTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "StartConnectionResponseTypeDef",
     "UpdateSiteAddressOutputTypeDef",
     "CreateOutpostOutputTypeDef",
     "GetOutpostOutputTypeDef",
     "ListOutpostsOutputTypeDef",
     "UpdateOutpostOutputTypeDef",
     "CreateSiteInputRequestTypeDef",
     "SiteTypeDef",
+    "GetCapacityTaskOutputTypeDef",
+    "StartCapacityTaskInputRequestTypeDef",
+    "StartCapacityTaskOutputTypeDef",
     "GetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef",
+    "GetOutpostSupportedInstanceTypesInputGetOutpostSupportedInstanceTypesPaginateTypeDef",
     "ListAssetsInputListAssetsPaginateTypeDef",
+    "ListCapacityTasksInputListCapacityTasksPaginateTypeDef",
     "ListCatalogItemsInputListCatalogItemsPaginateTypeDef",
     "ListOrdersInputListOrdersPaginateTypeDef",
     "ListOutpostsInputListOutpostsPaginateTypeDef",
     "ListSitesInputListSitesPaginateTypeDef",
     "GetOutpostInstanceTypesOutputTypeDef",
+    "GetOutpostSupportedInstanceTypesOutputTypeDef",
     "LineItemTypeDef",
     "ListOrdersOutputTypeDef",
     "ListAssetsOutputTypeDef",
     "GetCatalogItemOutputTypeDef",
     "ListCatalogItemsOutputTypeDef",
     "CreateSiteOutputTypeDef",
     "GetSiteOutputTypeDef",
@@ -155,20 +170,46 @@
     "ComputeAttributesTypeDef",
     {
         "HostId": NotRequired[str],
         "State": NotRequired[ComputeAssetStateType],
         "InstanceFamilies": NotRequired[List[str]],
     },
 )
+CancelCapacityTaskInputRequestTypeDef = TypedDict(
+    "CancelCapacityTaskInputRequestTypeDef",
+    {
+        "CapacityTaskId": str,
+        "OutpostIdentifier": str,
+    },
+)
 CancelOrderInputRequestTypeDef = TypedDict(
     "CancelOrderInputRequestTypeDef",
     {
         "OrderId": str,
     },
 )
+CapacityTaskFailureTypeDef = TypedDict(
+    "CapacityTaskFailureTypeDef",
+    {
+        "Reason": str,
+        "Type": NotRequired[Literal["UNSUPPORTED_CAPACITY_CONFIGURATION"]],
+    },
+)
+CapacityTaskSummaryTypeDef = TypedDict(
+    "CapacityTaskSummaryTypeDef",
+    {
+        "CapacityTaskId": NotRequired[str],
+        "OutpostId": NotRequired[str],
+        "OrderId": NotRequired[str],
+        "CapacityTaskStatus": NotRequired[CapacityTaskStatusType],
+        "CreationDate": NotRequired[datetime],
+        "CompletionDate": NotRequired[datetime],
+        "LastModifiedDate": NotRequired[datetime],
+    },
+)
 EC2CapacityTypeDef = TypedDict(
     "EC2CapacityTypeDef",
     {
         "Family": NotRequired[str],
         "MaxSize": NotRequired[str],
         "Quantity": NotRequired[str],
     },
@@ -252,14 +293,28 @@
 )
 DeleteSiteInputRequestTypeDef = TypedDict(
     "DeleteSiteInputRequestTypeDef",
     {
         "SiteId": str,
     },
 )
+GetCapacityTaskInputRequestTypeDef = TypedDict(
+    "GetCapacityTaskInputRequestTypeDef",
+    {
+        "CapacityTaskId": str,
+        "OutpostIdentifier": str,
+    },
+)
+InstanceTypeCapacityTypeDef = TypedDict(
+    "InstanceTypeCapacityTypeDef",
+    {
+        "InstanceType": str,
+        "Count": int,
+    },
+)
 GetCatalogItemInputRequestTypeDef = TypedDict(
     "GetCatalogItemInputRequestTypeDef",
     {
         "CatalogItemId": str,
     },
 )
 GetConnectionRequestRequestTypeDef = TypedDict(
@@ -298,14 +353,23 @@
 )
 InstanceTypeItemTypeDef = TypedDict(
     "InstanceTypeItemTypeDef",
     {
         "InstanceType": NotRequired[str],
     },
 )
+GetOutpostSupportedInstanceTypesInputRequestTypeDef = TypedDict(
+    "GetOutpostSupportedInstanceTypesInputRequestTypeDef",
+    {
+        "OutpostIdentifier": str,
+        "OrderId": str,
+        "MaxResults": NotRequired[int],
+        "NextToken": NotRequired[str],
+    },
+)
 GetSiteAddressInputRequestTypeDef = TypedDict(
     "GetSiteAddressInputRequestTypeDef",
     {
         "SiteId": str,
         "AddressType": AddressTypeType,
     },
 )
@@ -335,14 +399,23 @@
         "OutpostIdentifier": str,
         "HostIdFilter": NotRequired[Sequence[str]],
         "MaxResults": NotRequired[int],
         "NextToken": NotRequired[str],
         "StatusFilter": NotRequired[Sequence[AssetStateType]],
     },
 )
+ListCapacityTasksInputRequestTypeDef = TypedDict(
+    "ListCapacityTasksInputRequestTypeDef",
+    {
+        "OutpostIdentifierFilter": NotRequired[str],
+        "MaxResults": NotRequired[int],
+        "NextToken": NotRequired[str],
+        "CapacityTaskStatusFilter": NotRequired[Sequence[CapacityTaskStatusType]],
+    },
+)
 ListCatalogItemsInputRequestTypeDef = TypedDict(
     "ListCatalogItemsInputRequestTypeDef",
     {
         "NextToken": NotRequired[str],
         "MaxResults": NotRequired[int],
         "ItemClassFilter": NotRequired[Sequence[CatalogItemClassType]],
         "SupportedStorageFilter": NotRequired[Sequence[SupportedStorageEnumType]],
@@ -503,14 +576,22 @@
     {
         "SiteId": str,
         "AddressType": AddressTypeType,
         "Address": AddressTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+ListCapacityTasksOutputTypeDef = TypedDict(
+    "ListCapacityTasksOutputTypeDef",
+    {
+        "CapacityTasks": List[CapacityTaskSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -583,30 +664,87 @@
         "Notes": NotRequired[str],
         "OperatingAddressCountryCode": NotRequired[str],
         "OperatingAddressStateOrRegion": NotRequired[str],
         "OperatingAddressCity": NotRequired[str],
         "RackPhysicalProperties": NotRequired[RackPhysicalPropertiesTypeDef],
     },
 )
+GetCapacityTaskOutputTypeDef = TypedDict(
+    "GetCapacityTaskOutputTypeDef",
+    {
+        "CapacityTaskId": str,
+        "OutpostId": str,
+        "OrderId": str,
+        "RequestedInstancePools": List[InstanceTypeCapacityTypeDef],
+        "DryRun": bool,
+        "CapacityTaskStatus": CapacityTaskStatusType,
+        "Failed": CapacityTaskFailureTypeDef,
+        "CreationDate": datetime,
+        "CompletionDate": datetime,
+        "LastModifiedDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+StartCapacityTaskInputRequestTypeDef = TypedDict(
+    "StartCapacityTaskInputRequestTypeDef",
+    {
+        "OutpostIdentifier": str,
+        "OrderId": str,
+        "InstancePools": Sequence[InstanceTypeCapacityTypeDef],
+        "DryRun": NotRequired[bool],
+    },
+)
+StartCapacityTaskOutputTypeDef = TypedDict(
+    "StartCapacityTaskOutputTypeDef",
+    {
+        "CapacityTaskId": str,
+        "OutpostId": str,
+        "OrderId": str,
+        "RequestedInstancePools": List[InstanceTypeCapacityTypeDef],
+        "DryRun": bool,
+        "CapacityTaskStatus": CapacityTaskStatusType,
+        "Failed": CapacityTaskFailureTypeDef,
+        "CreationDate": datetime,
+        "CompletionDate": datetime,
+        "LastModifiedDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 GetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef = TypedDict(
     "GetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef",
     {
         "OutpostId": str,
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
+GetOutpostSupportedInstanceTypesInputGetOutpostSupportedInstanceTypesPaginateTypeDef = TypedDict(
+    "GetOutpostSupportedInstanceTypesInputGetOutpostSupportedInstanceTypesPaginateTypeDef",
+    {
+        "OutpostIdentifier": str,
+        "OrderId": str,
+        "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
+    },
+)
 ListAssetsInputListAssetsPaginateTypeDef = TypedDict(
     "ListAssetsInputListAssetsPaginateTypeDef",
     {
         "OutpostIdentifier": str,
         "HostIdFilter": NotRequired[Sequence[str]],
         "StatusFilter": NotRequired[Sequence[AssetStateType]],
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
+ListCapacityTasksInputListCapacityTasksPaginateTypeDef = TypedDict(
+    "ListCapacityTasksInputListCapacityTasksPaginateTypeDef",
+    {
+        "OutpostIdentifierFilter": NotRequired[str],
+        "CapacityTaskStatusFilter": NotRequired[Sequence[CapacityTaskStatusType]],
+        "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
+    },
+)
 ListCatalogItemsInputListCatalogItemsPaginateTypeDef = TypedDict(
     "ListCatalogItemsInputListCatalogItemsPaginateTypeDef",
     {
         "ItemClassFilter": NotRequired[Sequence[CatalogItemClassType]],
         "SupportedStorageFilter": NotRequired[Sequence[SupportedStorageEnumType]],
         "EC2FamilyFilter": NotRequired[Sequence[str]],
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
@@ -643,14 +781,22 @@
         "InstanceTypes": List[InstanceTypeItemTypeDef],
         "NextToken": str,
         "OutpostId": str,
         "OutpostArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+GetOutpostSupportedInstanceTypesOutputTypeDef = TypedDict(
+    "GetOutpostSupportedInstanceTypesOutputTypeDef",
+    {
+        "InstanceTypes": List[InstanceTypeItemTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 LineItemTypeDef = TypedDict(
     "LineItemTypeDef",
     {
         "CatalogItemId": NotRequired[str],
         "LineItemId": NotRequired[str],
         "Quantity": NotRequired[int],
         "Status": NotRequired[LineItemStatusType],
```

### Comparing `mypy_boto3_outposts-1.34.84/mypy_boto3_outposts/type_defs.pyi` & `mypy_boto3_outposts-1.34.85/mypy_boto3_outposts/type_defs.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AddressTypeType,
     AssetStateType,
+    CapacityTaskStatusType,
     CatalogItemClassType,
     CatalogItemStatusType,
     ComputeAssetStateType,
     FiberOpticCableTypeType,
     LineItemStatusType,
     MaximumSupportedWeightLbsType,
     OpticalStandardType,
@@ -54,36 +55,43 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AddressTypeDef",
     "AssetLocationTypeDef",
     "ComputeAttributesTypeDef",
+    "CancelCapacityTaskInputRequestTypeDef",
     "CancelOrderInputRequestTypeDef",
+    "CapacityTaskFailureTypeDef",
+    "CapacityTaskSummaryTypeDef",
     "EC2CapacityTypeDef",
     "ConnectionDetailsTypeDef",
     "LineItemRequestTypeDef",
     "ResponseMetadataTypeDef",
     "CreateOutpostInputRequestTypeDef",
     "OutpostTypeDef",
     "RackPhysicalPropertiesTypeDef",
     "DeleteOutpostInputRequestTypeDef",
     "DeleteSiteInputRequestTypeDef",
+    "GetCapacityTaskInputRequestTypeDef",
+    "InstanceTypeCapacityTypeDef",
     "GetCatalogItemInputRequestTypeDef",
     "GetConnectionRequestRequestTypeDef",
     "GetOrderInputRequestTypeDef",
     "GetOutpostInputRequestTypeDef",
     "PaginatorConfigTypeDef",
     "GetOutpostInstanceTypesInputRequestTypeDef",
     "InstanceTypeItemTypeDef",
+    "GetOutpostSupportedInstanceTypesInputRequestTypeDef",
     "GetSiteAddressInputRequestTypeDef",
     "GetSiteInputRequestTypeDef",
     "LineItemAssetInformationTypeDef",
     "ShipmentInformationTypeDef",
     "ListAssetsInputRequestTypeDef",
+    "ListCapacityTasksInputRequestTypeDef",
     "ListCatalogItemsInputRequestTypeDef",
     "ListOrdersInputRequestTypeDef",
     "OrderSummaryTypeDef",
     "ListOutpostsInputRequestTypeDef",
     "ListSitesInputRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "StartConnectionRequestRequestTypeDef",
@@ -94,30 +102,37 @@
     "UpdateSiteRackPhysicalPropertiesInputRequestTypeDef",
     "UpdateSiteAddressInputRequestTypeDef",
     "AssetInfoTypeDef",
     "CatalogItemTypeDef",
     "CreateOrderInputRequestTypeDef",
     "GetConnectionResponseTypeDef",
     "GetSiteAddressOutputTypeDef",
+    "ListCapacityTasksOutputTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "StartConnectionResponseTypeDef",
     "UpdateSiteAddressOutputTypeDef",
     "CreateOutpostOutputTypeDef",
     "GetOutpostOutputTypeDef",
     "ListOutpostsOutputTypeDef",
     "UpdateOutpostOutputTypeDef",
     "CreateSiteInputRequestTypeDef",
     "SiteTypeDef",
+    "GetCapacityTaskOutputTypeDef",
+    "StartCapacityTaskInputRequestTypeDef",
+    "StartCapacityTaskOutputTypeDef",
     "GetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef",
+    "GetOutpostSupportedInstanceTypesInputGetOutpostSupportedInstanceTypesPaginateTypeDef",
     "ListAssetsInputListAssetsPaginateTypeDef",
+    "ListCapacityTasksInputListCapacityTasksPaginateTypeDef",
     "ListCatalogItemsInputListCatalogItemsPaginateTypeDef",
     "ListOrdersInputListOrdersPaginateTypeDef",
     "ListOutpostsInputListOutpostsPaginateTypeDef",
     "ListSitesInputListSitesPaginateTypeDef",
     "GetOutpostInstanceTypesOutputTypeDef",
+    "GetOutpostSupportedInstanceTypesOutputTypeDef",
     "LineItemTypeDef",
     "ListOrdersOutputTypeDef",
     "ListAssetsOutputTypeDef",
     "GetCatalogItemOutputTypeDef",
     "ListCatalogItemsOutputTypeDef",
     "CreateSiteOutputTypeDef",
     "GetSiteOutputTypeDef",
@@ -155,20 +170,46 @@
     "ComputeAttributesTypeDef",
     {
         "HostId": NotRequired[str],
         "State": NotRequired[ComputeAssetStateType],
         "InstanceFamilies": NotRequired[List[str]],
     },
 )
+CancelCapacityTaskInputRequestTypeDef = TypedDict(
+    "CancelCapacityTaskInputRequestTypeDef",
+    {
+        "CapacityTaskId": str,
+        "OutpostIdentifier": str,
+    },
+)
 CancelOrderInputRequestTypeDef = TypedDict(
     "CancelOrderInputRequestTypeDef",
     {
         "OrderId": str,
     },
 )
+CapacityTaskFailureTypeDef = TypedDict(
+    "CapacityTaskFailureTypeDef",
+    {
+        "Reason": str,
+        "Type": NotRequired[Literal["UNSUPPORTED_CAPACITY_CONFIGURATION"]],
+    },
+)
+CapacityTaskSummaryTypeDef = TypedDict(
+    "CapacityTaskSummaryTypeDef",
+    {
+        "CapacityTaskId": NotRequired[str],
+        "OutpostId": NotRequired[str],
+        "OrderId": NotRequired[str],
+        "CapacityTaskStatus": NotRequired[CapacityTaskStatusType],
+        "CreationDate": NotRequired[datetime],
+        "CompletionDate": NotRequired[datetime],
+        "LastModifiedDate": NotRequired[datetime],
+    },
+)
 EC2CapacityTypeDef = TypedDict(
     "EC2CapacityTypeDef",
     {
         "Family": NotRequired[str],
         "MaxSize": NotRequired[str],
         "Quantity": NotRequired[str],
     },
@@ -252,14 +293,28 @@
 )
 DeleteSiteInputRequestTypeDef = TypedDict(
     "DeleteSiteInputRequestTypeDef",
     {
         "SiteId": str,
     },
 )
+GetCapacityTaskInputRequestTypeDef = TypedDict(
+    "GetCapacityTaskInputRequestTypeDef",
+    {
+        "CapacityTaskId": str,
+        "OutpostIdentifier": str,
+    },
+)
+InstanceTypeCapacityTypeDef = TypedDict(
+    "InstanceTypeCapacityTypeDef",
+    {
+        "InstanceType": str,
+        "Count": int,
+    },
+)
 GetCatalogItemInputRequestTypeDef = TypedDict(
     "GetCatalogItemInputRequestTypeDef",
     {
         "CatalogItemId": str,
     },
 )
 GetConnectionRequestRequestTypeDef = TypedDict(
@@ -298,14 +353,23 @@
 )
 InstanceTypeItemTypeDef = TypedDict(
     "InstanceTypeItemTypeDef",
     {
         "InstanceType": NotRequired[str],
     },
 )
+GetOutpostSupportedInstanceTypesInputRequestTypeDef = TypedDict(
+    "GetOutpostSupportedInstanceTypesInputRequestTypeDef",
+    {
+        "OutpostIdentifier": str,
+        "OrderId": str,
+        "MaxResults": NotRequired[int],
+        "NextToken": NotRequired[str],
+    },
+)
 GetSiteAddressInputRequestTypeDef = TypedDict(
     "GetSiteAddressInputRequestTypeDef",
     {
         "SiteId": str,
         "AddressType": AddressTypeType,
     },
 )
@@ -335,14 +399,23 @@
         "OutpostIdentifier": str,
         "HostIdFilter": NotRequired[Sequence[str]],
         "MaxResults": NotRequired[int],
         "NextToken": NotRequired[str],
         "StatusFilter": NotRequired[Sequence[AssetStateType]],
     },
 )
+ListCapacityTasksInputRequestTypeDef = TypedDict(
+    "ListCapacityTasksInputRequestTypeDef",
+    {
+        "OutpostIdentifierFilter": NotRequired[str],
+        "MaxResults": NotRequired[int],
+        "NextToken": NotRequired[str],
+        "CapacityTaskStatusFilter": NotRequired[Sequence[CapacityTaskStatusType]],
+    },
+)
 ListCatalogItemsInputRequestTypeDef = TypedDict(
     "ListCatalogItemsInputRequestTypeDef",
     {
         "NextToken": NotRequired[str],
         "MaxResults": NotRequired[int],
         "ItemClassFilter": NotRequired[Sequence[CatalogItemClassType]],
         "SupportedStorageFilter": NotRequired[Sequence[SupportedStorageEnumType]],
@@ -503,14 +576,22 @@
     {
         "SiteId": str,
         "AddressType": AddressTypeType,
         "Address": AddressTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+ListCapacityTasksOutputTypeDef = TypedDict(
+    "ListCapacityTasksOutputTypeDef",
+    {
+        "CapacityTasks": List[CapacityTaskSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -583,30 +664,87 @@
         "Notes": NotRequired[str],
         "OperatingAddressCountryCode": NotRequired[str],
         "OperatingAddressStateOrRegion": NotRequired[str],
         "OperatingAddressCity": NotRequired[str],
         "RackPhysicalProperties": NotRequired[RackPhysicalPropertiesTypeDef],
     },
 )
+GetCapacityTaskOutputTypeDef = TypedDict(
+    "GetCapacityTaskOutputTypeDef",
+    {
+        "CapacityTaskId": str,
+        "OutpostId": str,
+        "OrderId": str,
+        "RequestedInstancePools": List[InstanceTypeCapacityTypeDef],
+        "DryRun": bool,
+        "CapacityTaskStatus": CapacityTaskStatusType,
+        "Failed": CapacityTaskFailureTypeDef,
+        "CreationDate": datetime,
+        "CompletionDate": datetime,
+        "LastModifiedDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+StartCapacityTaskInputRequestTypeDef = TypedDict(
+    "StartCapacityTaskInputRequestTypeDef",
+    {
+        "OutpostIdentifier": str,
+        "OrderId": str,
+        "InstancePools": Sequence[InstanceTypeCapacityTypeDef],
+        "DryRun": NotRequired[bool],
+    },
+)
+StartCapacityTaskOutputTypeDef = TypedDict(
+    "StartCapacityTaskOutputTypeDef",
+    {
+        "CapacityTaskId": str,
+        "OutpostId": str,
+        "OrderId": str,
+        "RequestedInstancePools": List[InstanceTypeCapacityTypeDef],
+        "DryRun": bool,
+        "CapacityTaskStatus": CapacityTaskStatusType,
+        "Failed": CapacityTaskFailureTypeDef,
+        "CreationDate": datetime,
+        "CompletionDate": datetime,
+        "LastModifiedDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 GetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef = TypedDict(
     "GetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef",
     {
         "OutpostId": str,
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
+GetOutpostSupportedInstanceTypesInputGetOutpostSupportedInstanceTypesPaginateTypeDef = TypedDict(
+    "GetOutpostSupportedInstanceTypesInputGetOutpostSupportedInstanceTypesPaginateTypeDef",
+    {
+        "OutpostIdentifier": str,
+        "OrderId": str,
+        "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
+    },
+)
 ListAssetsInputListAssetsPaginateTypeDef = TypedDict(
     "ListAssetsInputListAssetsPaginateTypeDef",
     {
         "OutpostIdentifier": str,
         "HostIdFilter": NotRequired[Sequence[str]],
         "StatusFilter": NotRequired[Sequence[AssetStateType]],
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
+ListCapacityTasksInputListCapacityTasksPaginateTypeDef = TypedDict(
+    "ListCapacityTasksInputListCapacityTasksPaginateTypeDef",
+    {
+        "OutpostIdentifierFilter": NotRequired[str],
+        "CapacityTaskStatusFilter": NotRequired[Sequence[CapacityTaskStatusType]],
+        "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
+    },
+)
 ListCatalogItemsInputListCatalogItemsPaginateTypeDef = TypedDict(
     "ListCatalogItemsInputListCatalogItemsPaginateTypeDef",
     {
         "ItemClassFilter": NotRequired[Sequence[CatalogItemClassType]],
         "SupportedStorageFilter": NotRequired[Sequence[SupportedStorageEnumType]],
         "EC2FamilyFilter": NotRequired[Sequence[str]],
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
@@ -643,14 +781,22 @@
         "InstanceTypes": List[InstanceTypeItemTypeDef],
         "NextToken": str,
         "OutpostId": str,
         "OutpostArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+GetOutpostSupportedInstanceTypesOutputTypeDef = TypedDict(
+    "GetOutpostSupportedInstanceTypesOutputTypeDef",
+    {
+        "InstanceTypes": List[InstanceTypeItemTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 LineItemTypeDef = TypedDict(
     "LineItemTypeDef",
     {
         "CatalogItemId": NotRequired[str],
         "LineItemId": NotRequired[str],
         "Quantity": NotRequired[int],
         "Status": NotRequired[LineItemStatusType],
```

### Comparing `mypy_boto3_outposts-1.34.84/mypy_boto3_outposts.egg-info/PKG-INFO` & `mypy_boto3_outposts-1.34.85/mypy_boto3_outposts.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-outposts
-Version: 1.34.84
-Summary: Type annotations for boto3.Outposts 1.34.84 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.85
+Summary: Type annotations for boto3.Outposts 1.34.85 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-outposts.svg?color=blue)](https://pypi.org/project/mypy-boto3-outposts)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-outposts)](https://pepy.tech/project/mypy-boto3-outposts)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Outposts 1.34.84](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts)
+[boto3.Outposts 1.34.85](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -281,29 +281,37 @@
 
 ```python
 from boto3.session import Session
 
 from mypy_boto3_outposts import OutpostsClient
 from mypy_boto3_outposts.paginator import (
     GetOutpostInstanceTypesPaginator,
+    GetOutpostSupportedInstanceTypesPaginator,
     ListAssetsPaginator,
+    ListCapacityTasksPaginator,
     ListCatalogItemsPaginator,
     ListOrdersPaginator,
     ListOutpostsPaginator,
     ListSitesPaginator,
 )
 
 client: OutpostsClient = Session().client("outposts")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
 get_outpost_instance_types_paginator: GetOutpostInstanceTypesPaginator = client.get_paginator(
     "get_outpost_instance_types"
 )
+get_outpost_supported_instance_types_paginator: GetOutpostSupportedInstanceTypesPaginator = (
+    client.get_paginator("get_outpost_supported_instance_types")
+)
 list_assets_paginator: ListAssetsPaginator = client.get_paginator("list_assets")
+list_capacity_tasks_paginator: ListCapacityTasksPaginator = client.get_paginator(
+    "list_capacity_tasks"
+)
 list_catalog_items_paginator: ListCatalogItemsPaginator = client.get_paginator("list_catalog_items")
 list_orders_paginator: ListOrdersPaginator = client.get_paginator("list_orders")
 list_outposts_paginator: ListOutpostsPaginator = client.get_paginator("list_outposts")
 list_sites_paginator: ListSitesPaginator = client.get_paginator("list_sites")
 ```
 
 <a id="literals"></a>
```

### Comparing `mypy_boto3_outposts-1.34.84/mypy_boto3_outposts.egg-info/SOURCES.txt` & `mypy_boto3_outposts-1.34.85/mypy_boto3_outposts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy_boto3_outposts-1.34.84/setup.py` & `mypy_boto3_outposts-1.34.85/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-outposts",
-    version="1.34.84",
+    version="1.34.85",
     packages=["mypy_boto3_outposts"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.Outposts 1.34.84 service generated with mypy-boto3-builder 7.23.2",
+    description="Type annotations for boto3.Outposts 1.34.85 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

