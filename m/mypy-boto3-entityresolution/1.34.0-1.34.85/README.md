# Comparing `tmp/mypy-boto3-entityresolution-1.34.0.tar.gz` & `tmp/mypy_boto3_entityresolution-1.34.85.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-entityresolution-1.34.0.tar", last modified: Wed Dec 13 21:22:38 2023, max compression
+gzip compressed data, was "mypy_boto3_entityresolution-1.34.85.tar", last modified: Tue Apr 16 19:33:15 2024, max compression
```

## Comparing `mypy-boto3-entityresolution-1.34.0.tar` & `mypy_boto3_entityresolution-1.34.85.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:22:38.143211 mypy-boto3-entityresolution-1.34.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 21:10:13.000000 mypy-boto3-entityresolution-1.34.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14016 2023-12-13 21:22:38.143211 mypy-boto3-entityresolution-1.34.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12447 2023-12-13 21:10:13.000000 mypy-boto3-entityresolution-1.34.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:22:38.143211 mypy-boto3-entityresolution-1.34.0/mypy_boto3_entityresolution/
--rw-r--r--   0 runner    (1001) docker     (127)     1821 2023-12-13 21:10:13.000000 mypy-boto3-entityresolution-1.34.0/mypy_boto3_entityresolution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2023-12-13 21:10:13.000000 mypy-boto3-entityresolution-1.34.0/mypy_boto3_entityresolution/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      941 2023-12-13 21:10:13.000000 mypy-boto3-entityresolution-1.34.0/mypy_boto3_entityresolution/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24014 2023-12-13 21:10:13.000000 mypy-boto3-entityresolution-1.34.0/mypy_boto3_entityresolution/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    24010 2023-12-13 21:10:13.000000 mypy-boto3-entityresolution-1.34.0/mypy_boto3_entityresolution/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9973 2023-12-13 21:10:13.000000 mypy-boto3-entityresolution-1.34.0/mypy_boto3_entityresolution/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9971 2023-12-13 21:10:13.000000 mypy-boto3-entityresolution-1.34.0/mypy_boto3_entityresolution/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7701 2023-12-13 21:10:13.000000 mypy-boto3-entityresolution-1.34.0/mypy_boto3_entityresolution/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7693 2023-12-13 21:10:13.000000 mypy-boto3-entityresolution-1.34.0/mypy_boto3_entityresolution/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 21:10:13.000000 mypy-boto3-entityresolution-1.34.0/mypy_boto3_entityresolution/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    25422 2023-12-13 21:10:13.000000 mypy-boto3-entityresolution-1.34.0/mypy_boto3_entityresolution/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    25421 2023-12-13 21:10:13.000000 mypy-boto3-entityresolution-1.34.0/mypy_boto3_entityresolution/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-12-13 21:10:13.000000 mypy-boto3-entityresolution-1.34.0/mypy_boto3_entityresolution/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:22:38.143211 mypy-boto3-entityresolution-1.34.0/mypy_boto3_entityresolution.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14016 2023-12-13 21:22:38.000000 mypy-boto3-entityresolution-1.34.0/mypy_boto3_entityresolution.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      851 2023-12-13 21:22:38.000000 mypy-boto3-entityresolution-1.34.0/mypy_boto3_entityresolution.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:22:38.000000 mypy-boto3-entityresolution-1.34.0/mypy_boto3_entityresolution.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:22:38.000000 mypy-boto3-entityresolution-1.34.0/mypy_boto3_entityresolution.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 21:22:38.000000 mypy-boto3-entityresolution-1.34.0/mypy_boto3_entityresolution.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-12-13 21:22:38.000000 mypy-boto3-entityresolution-1.34.0/mypy_boto3_entityresolution.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 21:22:38.143211 mypy-boto3-entityresolution-1.34.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2023-12-13 21:10:13.000000 mypy-boto3-entityresolution-1.34.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:33:15.084309 mypy_boto3_entityresolution-1.34.85/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-16 19:32:50.000000 mypy_boto3_entityresolution-1.34.85/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14175 2024-04-16 19:33:15.084309 mypy_boto3_entityresolution-1.34.85/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12584 2024-04-16 19:32:50.000000 mypy_boto3_entityresolution-1.34.85/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:33:15.084309 mypy_boto3_entityresolution-1.34.85/mypy_boto3_entityresolution/
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-04-16 19:32:50.000000 mypy_boto3_entityresolution-1.34.85/mypy_boto3_entityresolution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-04-16 19:32:50.000000 mypy_boto3_entityresolution-1.34.85/mypy_boto3_entityresolution/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-16 19:32:50.000000 mypy_boto3_entityresolution-1.34.85/mypy_boto3_entityresolution/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30395 2024-04-16 19:32:50.000000 mypy_boto3_entityresolution-1.34.85/mypy_boto3_entityresolution/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30392 2024-04-16 19:32:50.000000 mypy_boto3_entityresolution-1.34.85/mypy_boto3_entityresolution/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10406 2024-04-16 19:32:50.000000 mypy_boto3_entityresolution-1.34.85/mypy_boto3_entityresolution/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10406 2024-04-16 19:32:50.000000 mypy_boto3_entityresolution-1.34.85/mypy_boto3_entityresolution/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8789 2024-04-16 19:32:50.000000 mypy_boto3_entityresolution-1.34.85/mypy_boto3_entityresolution/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8781 2024-04-16 19:32:50.000000 mypy_boto3_entityresolution-1.34.85/mypy_boto3_entityresolution/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 19:32:50.000000 mypy_boto3_entityresolution-1.34.85/mypy_boto3_entityresolution/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    34558 2024-04-16 19:32:51.000000 mypy_boto3_entityresolution-1.34.85/mypy_boto3_entityresolution/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34558 2024-04-16 19:32:51.000000 mypy_boto3_entityresolution-1.34.85/mypy_boto3_entityresolution/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-16 19:32:50.000000 mypy_boto3_entityresolution-1.34.85/mypy_boto3_entityresolution/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:33:15.084309 mypy_boto3_entityresolution-1.34.85/mypy_boto3_entityresolution.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14175 2024-04-16 19:33:15.000000 mypy_boto3_entityresolution-1.34.85/mypy_boto3_entityresolution.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-16 19:33:15.000000 mypy_boto3_entityresolution-1.34.85/mypy_boto3_entityresolution.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 19:33:15.000000 mypy_boto3_entityresolution-1.34.85/mypy_boto3_entityresolution.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 19:33:15.000000 mypy_boto3_entityresolution-1.34.85/mypy_boto3_entityresolution.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-16 19:33:15.000000 mypy_boto3_entityresolution-1.34.85/mypy_boto3_entityresolution.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-16 19:33:15.000000 mypy_boto3_entityresolution-1.34.85/mypy_boto3_entityresolution.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 19:33:15.084309 mypy_boto3_entityresolution-1.34.85/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-16 19:32:50.000000 mypy_boto3_entityresolution-1.34.85/setup.py
```

### Comparing `mypy-boto3-entityresolution-1.34.0/LICENSE` & `mypy_boto3_entityresolution-1.34.85/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Vlad Emelianov
+Copyright (c) 2024 Vlad Emelianov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mypy-boto3-entityresolution-1.34.0/PKG-INFO` & `mypy_boto3_entityresolution-1.34.85/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-entityresolution
-Version: 1.34.0
-Summary: Type annotations for boto3.EntityResolution 1.34.0 service generated with mypy-boto3-builder 7.21.0
+Version: 1.34.85
+Summary: Type annotations for boto3.EntityResolution 1.34.85 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -13,50 +13,50 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Classifier: Typing :: Stubs Only
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: typing-extensions>=4.1.0; python_version < "3.12"
 
 <a id="mypy-boto3-entityresolution"></a>
 
 # mypy-boto3-entityresolution
 
 [![PyPI - mypy-boto3-entityresolution](https://img.shields.io/pypi/v/mypy-boto3-entityresolution.svg?color=blue)](https://pypi.org/project/mypy-boto3-entityresolution)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-entityresolution.svg?color=blue)](https://pypi.org/project/mypy-boto3-entityresolution)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-entityresolution)](https://pepy.tech/project/mypy-boto3-entityresolution)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EntityResolution 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution)
+[boto3.EntityResolution 1.34.85](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-entityresolution docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/).
 
 See how it helps to find and fix potential bugs:
 
@@ -284,14 +284,15 @@
 ```python
 from boto3.session import Session
 
 from mypy_boto3_entityresolution import EntityResolutionClient
 from mypy_boto3_entityresolution.paginator import (
     ListIdMappingJobsPaginator,
     ListIdMappingWorkflowsPaginator,
+    ListIdNamespacesPaginator,
     ListMatchingJobsPaginator,
     ListMatchingWorkflowsPaginator,
     ListProviderServicesPaginator,
     ListSchemaMappingsPaginator,
 )
 
 client: EntityResolutionClient = Session().client("entityresolution")
@@ -300,14 +301,15 @@
 # Types should be correctly discovered by mypy and IDEs
 list_id_mapping_jobs_paginator: ListIdMappingJobsPaginator = client.get_paginator(
     "list_id_mapping_jobs"
 )
 list_id_mapping_workflows_paginator: ListIdMappingWorkflowsPaginator = client.get_paginator(
     "list_id_mapping_workflows"
 )
+list_id_namespaces_paginator: ListIdNamespacesPaginator = client.get_paginator("list_id_namespaces")
 list_matching_jobs_paginator: ListMatchingJobsPaginator = client.get_paginator("list_matching_jobs")
 list_matching_workflows_paginator: ListMatchingWorkflowsPaginator = client.get_paginator(
     "list_matching_workflows"
 )
 list_provider_services_paginator: ListProviderServicesPaginator = client.get_paginator(
     "list_provider_services"
 )
@@ -340,18 +342,18 @@
 `mypy_boto3_entityresolution.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
 Full list of `EntityResolution` TypeDefs can be found in
 [docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/type_defs/).
 
 ```python
-from mypy_boto3_entityresolution.type_defs import IdMappingWorkflowInputSourceTypeDef
+from mypy_boto3_entityresolution.type_defs import AddPolicyStatementInputRequestTypeDef
 
 
-def get_value() -> IdMappingWorkflowInputSourceTypeDef:
+def get_value() -> AddPolicyStatementInputRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-entityresolution-1.34.0/README.md` & `mypy_boto3_entityresolution-1.34.85/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-entityresolution.svg?color=blue)](https://pypi.org/project/mypy-boto3-entityresolution)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-entityresolution)](https://pepy.tech/project/mypy-boto3-entityresolution)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EntityResolution 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution)
+[boto3.EntityResolution 1.34.85](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-entityresolution docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/).
 
 See how it helps to find and fix potential bugs:
 
@@ -251,14 +251,15 @@
 ```python
 from boto3.session import Session
 
 from mypy_boto3_entityresolution import EntityResolutionClient
 from mypy_boto3_entityresolution.paginator import (
     ListIdMappingJobsPaginator,
     ListIdMappingWorkflowsPaginator,
+    ListIdNamespacesPaginator,
     ListMatchingJobsPaginator,
     ListMatchingWorkflowsPaginator,
     ListProviderServicesPaginator,
     ListSchemaMappingsPaginator,
 )
 
 client: EntityResolutionClient = Session().client("entityresolution")
@@ -267,14 +268,15 @@
 # Types should be correctly discovered by mypy and IDEs
 list_id_mapping_jobs_paginator: ListIdMappingJobsPaginator = client.get_paginator(
     "list_id_mapping_jobs"
 )
 list_id_mapping_workflows_paginator: ListIdMappingWorkflowsPaginator = client.get_paginator(
     "list_id_mapping_workflows"
 )
+list_id_namespaces_paginator: ListIdNamespacesPaginator = client.get_paginator("list_id_namespaces")
 list_matching_jobs_paginator: ListMatchingJobsPaginator = client.get_paginator("list_matching_jobs")
 list_matching_workflows_paginator: ListMatchingWorkflowsPaginator = client.get_paginator(
     "list_matching_workflows"
 )
 list_provider_services_paginator: ListProviderServicesPaginator = client.get_paginator(
     "list_provider_services"
 )
@@ -307,18 +309,18 @@
 `mypy_boto3_entityresolution.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
 Full list of `EntityResolution` TypeDefs can be found in
 [docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/type_defs/).
 
 ```python
-from mypy_boto3_entityresolution.type_defs import IdMappingWorkflowInputSourceTypeDef
+from mypy_boto3_entityresolution.type_defs import AddPolicyStatementInputRequestTypeDef
 
 
-def get_value() -> IdMappingWorkflowInputSourceTypeDef:
+def get_value() -> AddPolicyStatementInputRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-entityresolution-1.34.0/mypy_boto3_entityresolution/__init__.py` & `mypy_boto3_entityresolution-1.34.85/mypy_boto3_entityresolution/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,48 +6,51 @@
     ```python
     from boto3.session import Session
     from mypy_boto3_entityresolution import (
         Client,
         EntityResolutionClient,
         ListIdMappingJobsPaginator,
         ListIdMappingWorkflowsPaginator,
+        ListIdNamespacesPaginator,
         ListMatchingJobsPaginator,
         ListMatchingWorkflowsPaginator,
         ListProviderServicesPaginator,
         ListSchemaMappingsPaginator,
     )
 
     session = Session()
     client: EntityResolutionClient = session.client("entityresolution")
 
     list_id_mapping_jobs_paginator: ListIdMappingJobsPaginator = client.get_paginator("list_id_mapping_jobs")
     list_id_mapping_workflows_paginator: ListIdMappingWorkflowsPaginator = client.get_paginator("list_id_mapping_workflows")
+    list_id_namespaces_paginator: ListIdNamespacesPaginator = client.get_paginator("list_id_namespaces")
     list_matching_jobs_paginator: ListMatchingJobsPaginator = client.get_paginator("list_matching_jobs")
     list_matching_workflows_paginator: ListMatchingWorkflowsPaginator = client.get_paginator("list_matching_workflows")
     list_provider_services_paginator: ListProviderServicesPaginator = client.get_paginator("list_provider_services")
     list_schema_mappings_paginator: ListSchemaMappingsPaginator = client.get_paginator("list_schema_mappings")
     ```
 """
 
 from .client import EntityResolutionClient
 from .paginator import (
     ListIdMappingJobsPaginator,
     ListIdMappingWorkflowsPaginator,
+    ListIdNamespacesPaginator,
     ListMatchingJobsPaginator,
     ListMatchingWorkflowsPaginator,
     ListProviderServicesPaginator,
     ListSchemaMappingsPaginator,
 )
 
 Client = EntityResolutionClient
 
-
 __all__ = (
     "Client",
     "EntityResolutionClient",
     "ListIdMappingJobsPaginator",
     "ListIdMappingWorkflowsPaginator",
+    "ListIdNamespacesPaginator",
     "ListMatchingJobsPaginator",
     "ListMatchingWorkflowsPaginator",
     "ListProviderServicesPaginator",
     "ListSchemaMappingsPaginator",
 )
```

### Comparing `mypy-boto3-entityresolution-1.34.0/mypy_boto3_entityresolution/__init__.pyi` & `mypy_boto3_entityresolution-1.34.85/mypy_boto3_entityresolution/__init__.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -6,47 +6,51 @@
     ```python
     from boto3.session import Session
     from mypy_boto3_entityresolution import (
         Client,
         EntityResolutionClient,
         ListIdMappingJobsPaginator,
         ListIdMappingWorkflowsPaginator,
+        ListIdNamespacesPaginator,
         ListMatchingJobsPaginator,
         ListMatchingWorkflowsPaginator,
         ListProviderServicesPaginator,
         ListSchemaMappingsPaginator,
     )
 
     session = Session()
     client: EntityResolutionClient = session.client("entityresolution")
 
     list_id_mapping_jobs_paginator: ListIdMappingJobsPaginator = client.get_paginator("list_id_mapping_jobs")
     list_id_mapping_workflows_paginator: ListIdMappingWorkflowsPaginator = client.get_paginator("list_id_mapping_workflows")
+    list_id_namespaces_paginator: ListIdNamespacesPaginator = client.get_paginator("list_id_namespaces")
     list_matching_jobs_paginator: ListMatchingJobsPaginator = client.get_paginator("list_matching_jobs")
     list_matching_workflows_paginator: ListMatchingWorkflowsPaginator = client.get_paginator("list_matching_workflows")
     list_provider_services_paginator: ListProviderServicesPaginator = client.get_paginator("list_provider_services")
     list_schema_mappings_paginator: ListSchemaMappingsPaginator = client.get_paginator("list_schema_mappings")
     ```
 """
 
 from .client import EntityResolutionClient
 from .paginator import (
     ListIdMappingJobsPaginator,
     ListIdMappingWorkflowsPaginator,
+    ListIdNamespacesPaginator,
     ListMatchingJobsPaginator,
     ListMatchingWorkflowsPaginator,
     ListProviderServicesPaginator,
     ListSchemaMappingsPaginator,
 )
 
 Client = EntityResolutionClient
 
 __all__ = (
     "Client",
     "EntityResolutionClient",
     "ListIdMappingJobsPaginator",
     "ListIdMappingWorkflowsPaginator",
+    "ListIdNamespacesPaginator",
     "ListMatchingJobsPaginator",
     "ListMatchingWorkflowsPaginator",
     "ListProviderServicesPaginator",
     "ListSchemaMappingsPaginator",
 )
```

### Comparing `mypy-boto3-entityresolution-1.34.0/mypy_boto3_entityresolution/__main__.py` & `mypy_boto3_entityresolution-1.34.85/mypy_boto3_entityresolution/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,28 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.EntityResolution 1.34.0\nVersion:         1.34.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
-        " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution//\nBoto3 docs:    "
-        "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution\nOther"
-        " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
-        " https://github.com/youtype/mypy_boto3_builder/releases"
+        "Type annotations for boto3.EntityResolution 1.34.85\n"
+        "Version:         1.34.85\n"
+        "Builder version: 7.23.2\n"
+        "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution//\n"
+        "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution\n"
+        "Other services:  https://pypi.org/project/boto3-stubs/\n"
+        "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.0")
+    print("1.34.85")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-entityresolution-1.34.0/mypy_boto3_entityresolution/client.py` & `mypy_boto3_entityresolution-1.34.85/mypy_boto3_entityresolution/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,64 +15,77 @@
 """
 
 import sys
 from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
+from .literals import IdNamespaceTypeType, StatementEffectType
 from .paginator import (
     ListIdMappingJobsPaginator,
     ListIdMappingWorkflowsPaginator,
+    ListIdNamespacesPaginator,
     ListMatchingJobsPaginator,
     ListMatchingWorkflowsPaginator,
     ListProviderServicesPaginator,
     ListSchemaMappingsPaginator,
 )
 from .type_defs import (
+    AddPolicyStatementOutputTypeDef,
     CreateIdMappingWorkflowOutputTypeDef,
+    CreateIdNamespaceOutputTypeDef,
     CreateMatchingWorkflowOutputTypeDef,
     CreateSchemaMappingOutputTypeDef,
     DeleteIdMappingWorkflowOutputTypeDef,
+    DeleteIdNamespaceOutputTypeDef,
     DeleteMatchingWorkflowOutputTypeDef,
+    DeletePolicyStatementOutputTypeDef,
     DeleteSchemaMappingOutputTypeDef,
     GetIdMappingJobOutputTypeDef,
     GetIdMappingWorkflowOutputTypeDef,
+    GetIdNamespaceOutputTypeDef,
     GetMatchIdOutputTypeDef,
     GetMatchingJobOutputTypeDef,
     GetMatchingWorkflowOutputTypeDef,
+    GetPolicyOutputTypeDef,
     GetProviderServiceOutputTypeDef,
     GetSchemaMappingOutputTypeDef,
+    IdMappingJobOutputSourceTypeDef,
     IdMappingTechniquesTypeDef,
     IdMappingWorkflowInputSourceTypeDef,
     IdMappingWorkflowOutputSourceTypeDef,
+    IdNamespaceIdMappingWorkflowPropertiesTypeDef,
+    IdNamespaceInputSourceTypeDef,
     IncrementalRunConfigTypeDef,
     InputSourceTypeDef,
     ListIdMappingJobsOutputTypeDef,
     ListIdMappingWorkflowsOutputTypeDef,
+    ListIdNamespacesOutputTypeDef,
     ListMatchingJobsOutputTypeDef,
     ListMatchingWorkflowsOutputTypeDef,
     ListProviderServicesOutputTypeDef,
     ListSchemaMappingsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     OutputSourceTypeDef,
+    PutPolicyOutputTypeDef,
     ResolutionTechniquesTypeDef,
     SchemaInputAttributeTypeDef,
     StartIdMappingJobOutputTypeDef,
     StartMatchingJobOutputTypeDef,
     UpdateIdMappingWorkflowOutputTypeDef,
+    UpdateIdNamespaceOutputTypeDef,
     UpdateMatchingWorkflowOutputTypeDef,
     UpdateSchemaMappingOutputTypeDef,
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("EntityResolutionClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -104,14 +117,31 @@
         """
         EntityResolutionClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/client/#exceptions)
         """
 
+    def add_policy_statement(
+        self,
+        *,
+        action: Sequence[str],
+        arn: str,
+        effect: StatementEffectType,
+        principal: Sequence[str],
+        statementId: str,
+        condition: str = ...,
+    ) -> AddPolicyStatementOutputTypeDef:
+        """
+        Adds a policy statement object.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.add_policy_statement)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/client/#add_policy_statement)
+        """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/client/#can_paginate)
         """
@@ -125,40 +155,60 @@
         """
 
     def create_id_mapping_workflow(
         self,
         *,
         idMappingTechniques: IdMappingTechniquesTypeDef,
         inputSourceConfig: Sequence[IdMappingWorkflowInputSourceTypeDef],
-        outputSourceConfig: Sequence[IdMappingWorkflowOutputSourceTypeDef],
         roleArn: str,
         workflowName: str,
         description: str = ...,
-        tags: Mapping[str, str] = ...
+        outputSourceConfig: Sequence[IdMappingWorkflowOutputSourceTypeDef] = ...,
+        tags: Mapping[str, str] = ...,
     ) -> CreateIdMappingWorkflowOutputTypeDef:
         """
         Creates an `IdMappingWorkflow` object which stores the configuration of the
         data processing job to be
         run.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.create_id_mapping_workflow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/client/#create_id_mapping_workflow)
         """
 
+    def create_id_namespace(
+        self,
+        *,
+        idNamespaceName: str,
+        type: IdNamespaceTypeType,
+        description: str = ...,
+        idMappingWorkflowProperties: Sequence[IdNamespaceIdMappingWorkflowPropertiesTypeDef] = ...,
+        inputSourceConfig: Sequence[IdNamespaceInputSourceTypeDef] = ...,
+        roleArn: str = ...,
+        tags: Mapping[str, str] = ...,
+    ) -> CreateIdNamespaceOutputTypeDef:
+        """
+        Creates an ID namespace object which will help customers provide metadata
+        explaining their dataset and how to use
+        it.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.create_id_namespace)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/client/#create_id_namespace)
+        """
+
     def create_matching_workflow(
         self,
         *,
         inputSourceConfig: Sequence[InputSourceTypeDef],
         outputSourceConfig: Sequence[OutputSourceTypeDef],
         resolutionTechniques: ResolutionTechniquesTypeDef,
         roleArn: str,
         workflowName: str,
         description: str = ...,
         incrementalRunConfig: IncrementalRunConfigTypeDef = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateMatchingWorkflowOutputTypeDef:
         """
         Creates a `MatchingWorkflow` object which stores the configuration of the data
         processing job to be
         run.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.create_matching_workflow)
@@ -167,15 +217,15 @@
 
     def create_schema_mapping(
         self,
         *,
         mappedInputFields: Sequence[SchemaInputAttributeTypeDef],
         schemaName: str,
         description: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateSchemaMappingOutputTypeDef:
         """
         Creates a schema mapping, which defines the schema of the input customer
         records
         table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.create_schema_mapping)
@@ -188,22 +238,40 @@
         """
         Deletes the `IdMappingWorkflow` with a given name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.delete_id_mapping_workflow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/client/#delete_id_mapping_workflow)
         """
 
+    def delete_id_namespace(self, *, idNamespaceName: str) -> DeleteIdNamespaceOutputTypeDef:
+        """
+        Deletes the `IdNamespace` with a given name.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.delete_id_namespace)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/client/#delete_id_namespace)
+        """
+
     def delete_matching_workflow(self, *, workflowName: str) -> DeleteMatchingWorkflowOutputTypeDef:
         """
         Deletes the `MatchingWorkflow` with a given name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.delete_matching_workflow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/client/#delete_matching_workflow)
         """
 
+    def delete_policy_statement(
+        self, *, arn: str, statementId: str
+    ) -> DeletePolicyStatementOutputTypeDef:
+        """
+        Deletes the policy statement.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.delete_policy_statement)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/client/#delete_policy_statement)
+        """
+
     def delete_schema_mapping(self, *, schemaName: str) -> DeleteSchemaMappingOutputTypeDef:
         """
         Deletes the `SchemaMapping` with a given name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.delete_schema_mapping)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/client/#delete_schema_mapping)
         """
@@ -236,16 +304,24 @@
         """
         Returns the `IdMappingWorkflow` with a given name, if it exists.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.get_id_mapping_workflow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/client/#get_id_mapping_workflow)
         """
 
+    def get_id_namespace(self, *, idNamespaceName: str) -> GetIdNamespaceOutputTypeDef:
+        """
+        Returns the `IdNamespace` with a given name, if it exists.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.get_id_namespace)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/client/#get_id_namespace)
+        """
+
     def get_match_id(
-        self, *, record: Mapping[str, str], workflowName: str
+        self, *, record: Mapping[str, str], workflowName: str, applyNormalization: bool = ...
     ) -> GetMatchIdOutputTypeDef:
         """
         Returns the corresponding Match ID of a customer record if the record has been
         processed.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.get_match_id)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/client/#get_match_id)
@@ -265,14 +341,22 @@
         """
         Returns the `MatchingWorkflow` with a given name, if it exists.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.get_matching_workflow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/client/#get_matching_workflow)
         """
 
+    def get_policy(self, *, arn: str) -> GetPolicyOutputTypeDef:
+        """
+        Returns the resource-based policy.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.get_policy)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/client/#get_policy)
+        """
+
     def get_provider_service(
         self, *, providerName: str, providerServiceName: str
     ) -> GetProviderServiceOutputTypeDef:
         """
         Returns the `ProviderService` of a given name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.get_provider_service)
@@ -305,14 +389,24 @@
         Amazon Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.list_id_mapping_workflows)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/client/#list_id_mapping_workflows)
         """
 
+    def list_id_namespaces(
+        self, *, maxResults: int = ..., nextToken: str = ...
+    ) -> ListIdNamespacesOutputTypeDef:
+        """
+        Returns a list of all ID namespaces.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.list_id_namespaces)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/client/#list_id_namespaces)
+        """
+
     def list_matching_jobs(
         self, *, workflowName: str, maxResults: int = ..., nextToken: str = ...
     ) -> ListMatchingJobsOutputTypeDef:
         """
         Lists all jobs for a given workflow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.list_matching_jobs)
@@ -359,15 +453,28 @@
         """
         Displays the tags associated with an Entity Resolution resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/client/#list_tags_for_resource)
         """
 
-    def start_id_mapping_job(self, *, workflowName: str) -> StartIdMappingJobOutputTypeDef:
+    def put_policy(self, *, arn: str, policy: str, token: str = ...) -> PutPolicyOutputTypeDef:
+        """
+        Updates the resource-based policy.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.put_policy)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/client/#put_policy)
+        """
+
+    def start_id_mapping_job(
+        self,
+        *,
+        workflowName: str,
+        outputSourceConfig: Sequence[IdMappingJobOutputSourceTypeDef] = ...,
+    ) -> StartIdMappingJobOutputTypeDef:
         """
         Starts the `IdMappingJob` of a workflow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.start_id_mapping_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/client/#start_id_mapping_job)
         """
 
@@ -397,50 +504,66 @@
         """
 
     def update_id_mapping_workflow(
         self,
         *,
         idMappingTechniques: IdMappingTechniquesTypeDef,
         inputSourceConfig: Sequence[IdMappingWorkflowInputSourceTypeDef],
-        outputSourceConfig: Sequence[IdMappingWorkflowOutputSourceTypeDef],
         roleArn: str,
         workflowName: str,
-        description: str = ...
+        description: str = ...,
+        outputSourceConfig: Sequence[IdMappingWorkflowOutputSourceTypeDef] = ...,
     ) -> UpdateIdMappingWorkflowOutputTypeDef:
         """
         Updates an existing `IdMappingWorkflow`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.update_id_mapping_workflow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/client/#update_id_mapping_workflow)
         """
 
+    def update_id_namespace(
+        self,
+        *,
+        idNamespaceName: str,
+        description: str = ...,
+        idMappingWorkflowProperties: Sequence[IdNamespaceIdMappingWorkflowPropertiesTypeDef] = ...,
+        inputSourceConfig: Sequence[IdNamespaceInputSourceTypeDef] = ...,
+        roleArn: str = ...,
+    ) -> UpdateIdNamespaceOutputTypeDef:
+        """
+        Updates an existing ID namespace.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.update_id_namespace)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/client/#update_id_namespace)
+        """
+
     def update_matching_workflow(
         self,
         *,
         inputSourceConfig: Sequence[InputSourceTypeDef],
         outputSourceConfig: Sequence[OutputSourceTypeDef],
         resolutionTechniques: ResolutionTechniquesTypeDef,
         roleArn: str,
         workflowName: str,
         description: str = ...,
-        incrementalRunConfig: IncrementalRunConfigTypeDef = ...
+        incrementalRunConfig: IncrementalRunConfigTypeDef = ...,
     ) -> UpdateMatchingWorkflowOutputTypeDef:
         """
         Updates an existing `MatchingWorkflow`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.update_matching_workflow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/client/#update_matching_workflow)
         """
 
     def update_schema_mapping(
         self,
         *,
         mappedInputFields: Sequence[SchemaInputAttributeTypeDef],
         schemaName: str,
-        description: str = ...
+        description: str = ...,
     ) -> UpdateSchemaMappingOutputTypeDef:
         """
         Updates a schema mapping.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.update_schema_mapping)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/client/#update_schema_mapping)
         """
@@ -461,14 +584,23 @@
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/client/#get_paginator)
         """
 
     @overload
     def get_paginator(
+        self, operation_name: Literal["list_id_namespaces"]
+    ) -> ListIdNamespacesPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/client/#get_paginator)
+        """
+
+    @overload
+    def get_paginator(
         self, operation_name: Literal["list_matching_jobs"]
     ) -> ListMatchingJobsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/client/#get_paginator)
         """
```

### Comparing `mypy-boto3-entityresolution-1.34.0/mypy_boto3_entityresolution/client.pyi` & `mypy_boto3_entityresolution-1.34.85/mypy_boto3_entityresolution/client.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -15,54 +15,68 @@
 """
 
 import sys
 from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
+from .literals import IdNamespaceTypeType, StatementEffectType
 from .paginator import (
     ListIdMappingJobsPaginator,
     ListIdMappingWorkflowsPaginator,
+    ListIdNamespacesPaginator,
     ListMatchingJobsPaginator,
     ListMatchingWorkflowsPaginator,
     ListProviderServicesPaginator,
     ListSchemaMappingsPaginator,
 )
 from .type_defs import (
+    AddPolicyStatementOutputTypeDef,
     CreateIdMappingWorkflowOutputTypeDef,
+    CreateIdNamespaceOutputTypeDef,
     CreateMatchingWorkflowOutputTypeDef,
     CreateSchemaMappingOutputTypeDef,
     DeleteIdMappingWorkflowOutputTypeDef,
+    DeleteIdNamespaceOutputTypeDef,
     DeleteMatchingWorkflowOutputTypeDef,
+    DeletePolicyStatementOutputTypeDef,
     DeleteSchemaMappingOutputTypeDef,
     GetIdMappingJobOutputTypeDef,
     GetIdMappingWorkflowOutputTypeDef,
+    GetIdNamespaceOutputTypeDef,
     GetMatchIdOutputTypeDef,
     GetMatchingJobOutputTypeDef,
     GetMatchingWorkflowOutputTypeDef,
+    GetPolicyOutputTypeDef,
     GetProviderServiceOutputTypeDef,
     GetSchemaMappingOutputTypeDef,
+    IdMappingJobOutputSourceTypeDef,
     IdMappingTechniquesTypeDef,
     IdMappingWorkflowInputSourceTypeDef,
     IdMappingWorkflowOutputSourceTypeDef,
+    IdNamespaceIdMappingWorkflowPropertiesTypeDef,
+    IdNamespaceInputSourceTypeDef,
     IncrementalRunConfigTypeDef,
     InputSourceTypeDef,
     ListIdMappingJobsOutputTypeDef,
     ListIdMappingWorkflowsOutputTypeDef,
+    ListIdNamespacesOutputTypeDef,
     ListMatchingJobsOutputTypeDef,
     ListMatchingWorkflowsOutputTypeDef,
     ListProviderServicesOutputTypeDef,
     ListSchemaMappingsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     OutputSourceTypeDef,
+    PutPolicyOutputTypeDef,
     ResolutionTechniquesTypeDef,
     SchemaInputAttributeTypeDef,
     StartIdMappingJobOutputTypeDef,
     StartMatchingJobOutputTypeDef,
     UpdateIdMappingWorkflowOutputTypeDef,
+    UpdateIdNamespaceOutputTypeDef,
     UpdateMatchingWorkflowOutputTypeDef,
     UpdateSchemaMappingOutputTypeDef,
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
@@ -100,14 +114,31 @@
         """
         EntityResolutionClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/client/#exceptions)
         """
 
+    def add_policy_statement(
+        self,
+        *,
+        action: Sequence[str],
+        arn: str,
+        effect: StatementEffectType,
+        principal: Sequence[str],
+        statementId: str,
+        condition: str = ...,
+    ) -> AddPolicyStatementOutputTypeDef:
+        """
+        Adds a policy statement object.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.add_policy_statement)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/client/#add_policy_statement)
+        """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/client/#can_paginate)
         """
@@ -121,40 +152,60 @@
         """
 
     def create_id_mapping_workflow(
         self,
         *,
         idMappingTechniques: IdMappingTechniquesTypeDef,
         inputSourceConfig: Sequence[IdMappingWorkflowInputSourceTypeDef],
-        outputSourceConfig: Sequence[IdMappingWorkflowOutputSourceTypeDef],
         roleArn: str,
         workflowName: str,
         description: str = ...,
-        tags: Mapping[str, str] = ...
+        outputSourceConfig: Sequence[IdMappingWorkflowOutputSourceTypeDef] = ...,
+        tags: Mapping[str, str] = ...,
     ) -> CreateIdMappingWorkflowOutputTypeDef:
         """
         Creates an `IdMappingWorkflow` object which stores the configuration of the
         data processing job to be
         run.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.create_id_mapping_workflow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/client/#create_id_mapping_workflow)
         """
 
+    def create_id_namespace(
+        self,
+        *,
+        idNamespaceName: str,
+        type: IdNamespaceTypeType,
+        description: str = ...,
+        idMappingWorkflowProperties: Sequence[IdNamespaceIdMappingWorkflowPropertiesTypeDef] = ...,
+        inputSourceConfig: Sequence[IdNamespaceInputSourceTypeDef] = ...,
+        roleArn: str = ...,
+        tags: Mapping[str, str] = ...,
+    ) -> CreateIdNamespaceOutputTypeDef:
+        """
+        Creates an ID namespace object which will help customers provide metadata
+        explaining their dataset and how to use
+        it.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.create_id_namespace)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/client/#create_id_namespace)
+        """
+
     def create_matching_workflow(
         self,
         *,
         inputSourceConfig: Sequence[InputSourceTypeDef],
         outputSourceConfig: Sequence[OutputSourceTypeDef],
         resolutionTechniques: ResolutionTechniquesTypeDef,
         roleArn: str,
         workflowName: str,
         description: str = ...,
         incrementalRunConfig: IncrementalRunConfigTypeDef = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateMatchingWorkflowOutputTypeDef:
         """
         Creates a `MatchingWorkflow` object which stores the configuration of the data
         processing job to be
         run.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.create_matching_workflow)
@@ -163,15 +214,15 @@
 
     def create_schema_mapping(
         self,
         *,
         mappedInputFields: Sequence[SchemaInputAttributeTypeDef],
         schemaName: str,
         description: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateSchemaMappingOutputTypeDef:
         """
         Creates a schema mapping, which defines the schema of the input customer
         records
         table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.create_schema_mapping)
@@ -184,22 +235,40 @@
         """
         Deletes the `IdMappingWorkflow` with a given name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.delete_id_mapping_workflow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/client/#delete_id_mapping_workflow)
         """
 
+    def delete_id_namespace(self, *, idNamespaceName: str) -> DeleteIdNamespaceOutputTypeDef:
+        """
+        Deletes the `IdNamespace` with a given name.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.delete_id_namespace)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/client/#delete_id_namespace)
+        """
+
     def delete_matching_workflow(self, *, workflowName: str) -> DeleteMatchingWorkflowOutputTypeDef:
         """
         Deletes the `MatchingWorkflow` with a given name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.delete_matching_workflow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/client/#delete_matching_workflow)
         """
 
+    def delete_policy_statement(
+        self, *, arn: str, statementId: str
+    ) -> DeletePolicyStatementOutputTypeDef:
+        """
+        Deletes the policy statement.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.delete_policy_statement)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/client/#delete_policy_statement)
+        """
+
     def delete_schema_mapping(self, *, schemaName: str) -> DeleteSchemaMappingOutputTypeDef:
         """
         Deletes the `SchemaMapping` with a given name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.delete_schema_mapping)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/client/#delete_schema_mapping)
         """
@@ -232,16 +301,24 @@
         """
         Returns the `IdMappingWorkflow` with a given name, if it exists.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.get_id_mapping_workflow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/client/#get_id_mapping_workflow)
         """
 
+    def get_id_namespace(self, *, idNamespaceName: str) -> GetIdNamespaceOutputTypeDef:
+        """
+        Returns the `IdNamespace` with a given name, if it exists.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.get_id_namespace)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/client/#get_id_namespace)
+        """
+
     def get_match_id(
-        self, *, record: Mapping[str, str], workflowName: str
+        self, *, record: Mapping[str, str], workflowName: str, applyNormalization: bool = ...
     ) -> GetMatchIdOutputTypeDef:
         """
         Returns the corresponding Match ID of a customer record if the record has been
         processed.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.get_match_id)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/client/#get_match_id)
@@ -261,14 +338,22 @@
         """
         Returns the `MatchingWorkflow` with a given name, if it exists.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.get_matching_workflow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/client/#get_matching_workflow)
         """
 
+    def get_policy(self, *, arn: str) -> GetPolicyOutputTypeDef:
+        """
+        Returns the resource-based policy.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.get_policy)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/client/#get_policy)
+        """
+
     def get_provider_service(
         self, *, providerName: str, providerServiceName: str
     ) -> GetProviderServiceOutputTypeDef:
         """
         Returns the `ProviderService` of a given name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.get_provider_service)
@@ -301,14 +386,24 @@
         Amazon Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.list_id_mapping_workflows)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/client/#list_id_mapping_workflows)
         """
 
+    def list_id_namespaces(
+        self, *, maxResults: int = ..., nextToken: str = ...
+    ) -> ListIdNamespacesOutputTypeDef:
+        """
+        Returns a list of all ID namespaces.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.list_id_namespaces)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/client/#list_id_namespaces)
+        """
+
     def list_matching_jobs(
         self, *, workflowName: str, maxResults: int = ..., nextToken: str = ...
     ) -> ListMatchingJobsOutputTypeDef:
         """
         Lists all jobs for a given workflow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.list_matching_jobs)
@@ -355,15 +450,28 @@
         """
         Displays the tags associated with an Entity Resolution resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/client/#list_tags_for_resource)
         """
 
-    def start_id_mapping_job(self, *, workflowName: str) -> StartIdMappingJobOutputTypeDef:
+    def put_policy(self, *, arn: str, policy: str, token: str = ...) -> PutPolicyOutputTypeDef:
+        """
+        Updates the resource-based policy.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.put_policy)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/client/#put_policy)
+        """
+
+    def start_id_mapping_job(
+        self,
+        *,
+        workflowName: str,
+        outputSourceConfig: Sequence[IdMappingJobOutputSourceTypeDef] = ...,
+    ) -> StartIdMappingJobOutputTypeDef:
         """
         Starts the `IdMappingJob` of a workflow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.start_id_mapping_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/client/#start_id_mapping_job)
         """
 
@@ -393,50 +501,66 @@
         """
 
     def update_id_mapping_workflow(
         self,
         *,
         idMappingTechniques: IdMappingTechniquesTypeDef,
         inputSourceConfig: Sequence[IdMappingWorkflowInputSourceTypeDef],
-        outputSourceConfig: Sequence[IdMappingWorkflowOutputSourceTypeDef],
         roleArn: str,
         workflowName: str,
-        description: str = ...
+        description: str = ...,
+        outputSourceConfig: Sequence[IdMappingWorkflowOutputSourceTypeDef] = ...,
     ) -> UpdateIdMappingWorkflowOutputTypeDef:
         """
         Updates an existing `IdMappingWorkflow`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.update_id_mapping_workflow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/client/#update_id_mapping_workflow)
         """
 
+    def update_id_namespace(
+        self,
+        *,
+        idNamespaceName: str,
+        description: str = ...,
+        idMappingWorkflowProperties: Sequence[IdNamespaceIdMappingWorkflowPropertiesTypeDef] = ...,
+        inputSourceConfig: Sequence[IdNamespaceInputSourceTypeDef] = ...,
+        roleArn: str = ...,
+    ) -> UpdateIdNamespaceOutputTypeDef:
+        """
+        Updates an existing ID namespace.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.update_id_namespace)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/client/#update_id_namespace)
+        """
+
     def update_matching_workflow(
         self,
         *,
         inputSourceConfig: Sequence[InputSourceTypeDef],
         outputSourceConfig: Sequence[OutputSourceTypeDef],
         resolutionTechniques: ResolutionTechniquesTypeDef,
         roleArn: str,
         workflowName: str,
         description: str = ...,
-        incrementalRunConfig: IncrementalRunConfigTypeDef = ...
+        incrementalRunConfig: IncrementalRunConfigTypeDef = ...,
     ) -> UpdateMatchingWorkflowOutputTypeDef:
         """
         Updates an existing `MatchingWorkflow`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.update_matching_workflow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/client/#update_matching_workflow)
         """
 
     def update_schema_mapping(
         self,
         *,
         mappedInputFields: Sequence[SchemaInputAttributeTypeDef],
         schemaName: str,
-        description: str = ...
+        description: str = ...,
     ) -> UpdateSchemaMappingOutputTypeDef:
         """
         Updates a schema mapping.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.update_schema_mapping)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/client/#update_schema_mapping)
         """
@@ -457,14 +581,23 @@
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/client/#get_paginator)
         """
 
     @overload
     def get_paginator(
+        self, operation_name: Literal["list_id_namespaces"]
+    ) -> ListIdNamespacesPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/client/#get_paginator)
+        """
+
+    @overload
+    def get_paginator(
         self, operation_name: Literal["list_matching_jobs"]
     ) -> ListMatchingJobsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/client/#get_paginator)
         """
```

### Comparing `mypy-boto3-entityresolution-1.34.0/mypy_boto3_entityresolution/literals.py` & `mypy_boto3_entityresolution-1.34.85/mypy_boto3_entityresolution/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,42 +15,45 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AttributeMatchingModelType",
     "IdMappingTypeType",
+    "IdNamespaceTypeType",
     "IncrementalRunTypeType",
     "JobStatusType",
     "ListIdMappingJobsPaginatorName",
     "ListIdMappingWorkflowsPaginatorName",
+    "ListIdNamespacesPaginatorName",
     "ListMatchingJobsPaginatorName",
     "ListMatchingWorkflowsPaginatorName",
     "ListProviderServicesPaginatorName",
     "ListSchemaMappingsPaginatorName",
     "ResolutionTypeType",
     "SchemaAttributeTypeType",
     "ServiceTypeType",
+    "StatementEffectType",
     "EntityResolutionServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
-
 AttributeMatchingModelType = Literal["MANY_TO_MANY", "ONE_TO_ONE"]
 IdMappingTypeType = Literal["PROVIDER"]
+IdNamespaceTypeType = Literal["SOURCE", "TARGET"]
 IncrementalRunTypeType = Literal["IMMEDIATE"]
 JobStatusType = Literal["FAILED", "QUEUED", "RUNNING", "SUCCEEDED"]
 ListIdMappingJobsPaginatorName = Literal["list_id_mapping_jobs"]
 ListIdMappingWorkflowsPaginatorName = Literal["list_id_mapping_workflows"]
+ListIdNamespacesPaginatorName = Literal["list_id_namespaces"]
 ListMatchingJobsPaginatorName = Literal["list_matching_jobs"]
 ListMatchingWorkflowsPaginatorName = Literal["list_matching_workflows"]
 ListProviderServicesPaginatorName = Literal["list_provider_services"]
 ListSchemaMappingsPaginatorName = Literal["list_schema_mappings"]
 ResolutionTypeType = Literal["ML_MATCHING", "PROVIDER", "RULE_MATCHING"]
 SchemaAttributeTypeType = Literal[
     "ADDRESS",
@@ -71,14 +74,15 @@
     "PHONE_COUNTRYCODE",
     "PHONE_NUMBER",
     "PROVIDER_ID",
     "STRING",
     "UNIQUE_ID",
 ]
 ServiceTypeType = Literal["ASSIGNMENT", "ID_MAPPING"]
+StatementEffectType = Literal["Allow", "Deny"]
 EntityResolutionServiceName = Literal["entityresolution"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
@@ -98,14 +102,15 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
+    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -116,14 +121,15 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
+    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -141,14 +147,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -161,24 +168,26 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
+    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -239,15 +248,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -319,17 +327,19 @@
     "migrationhuborchestrator",
     "migrationhubstrategy",
     "mobile",
     "mq",
     "mturk",
     "mwaa",
     "neptune",
+    "neptune-graph",
     "neptunedata",
     "network-firewall",
     "networkmanager",
+    "networkmonitor",
     "nimble",
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
@@ -419,19 +429,21 @@
     "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
+    "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
@@ -463,12 +475,13 @@
     "s3",
     "sns",
     "sqs",
 ]
 PaginatorName = Literal[
     "list_id_mapping_jobs",
     "list_id_mapping_workflows",
+    "list_id_namespaces",
     "list_matching_jobs",
     "list_matching_workflows",
     "list_provider_services",
     "list_schema_mappings",
 ]
```

### Comparing `mypy-boto3-entityresolution-1.34.0/mypy_boto3_entityresolution/literals.pyi` & `mypy_boto3_entityresolution-1.34.85/mypy_boto3_entityresolution/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -18,37 +18,42 @@
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = (
     "AttributeMatchingModelType",
     "IdMappingTypeType",
+    "IdNamespaceTypeType",
     "IncrementalRunTypeType",
     "JobStatusType",
     "ListIdMappingJobsPaginatorName",
     "ListIdMappingWorkflowsPaginatorName",
+    "ListIdNamespacesPaginatorName",
     "ListMatchingJobsPaginatorName",
     "ListMatchingWorkflowsPaginatorName",
     "ListProviderServicesPaginatorName",
     "ListSchemaMappingsPaginatorName",
     "ResolutionTypeType",
     "SchemaAttributeTypeType",
     "ServiceTypeType",
+    "StatementEffectType",
     "EntityResolutionServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
 AttributeMatchingModelType = Literal["MANY_TO_MANY", "ONE_TO_ONE"]
 IdMappingTypeType = Literal["PROVIDER"]
+IdNamespaceTypeType = Literal["SOURCE", "TARGET"]
 IncrementalRunTypeType = Literal["IMMEDIATE"]
 JobStatusType = Literal["FAILED", "QUEUED", "RUNNING", "SUCCEEDED"]
 ListIdMappingJobsPaginatorName = Literal["list_id_mapping_jobs"]
 ListIdMappingWorkflowsPaginatorName = Literal["list_id_mapping_workflows"]
+ListIdNamespacesPaginatorName = Literal["list_id_namespaces"]
 ListMatchingJobsPaginatorName = Literal["list_matching_jobs"]
 ListMatchingWorkflowsPaginatorName = Literal["list_matching_workflows"]
 ListProviderServicesPaginatorName = Literal["list_provider_services"]
 ListSchemaMappingsPaginatorName = Literal["list_schema_mappings"]
 ResolutionTypeType = Literal["ML_MATCHING", "PROVIDER", "RULE_MATCHING"]
 SchemaAttributeTypeType = Literal[
     "ADDRESS",
@@ -69,14 +74,15 @@
     "PHONE_COUNTRYCODE",
     "PHONE_NUMBER",
     "PROVIDER_ID",
     "STRING",
     "UNIQUE_ID",
 ]
 ServiceTypeType = Literal["ASSIGNMENT", "ID_MAPPING"]
+StatementEffectType = Literal["Allow", "Deny"]
 EntityResolutionServiceName = Literal["entityresolution"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
@@ -96,14 +102,15 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
+    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -114,14 +121,15 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
+    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -139,14 +147,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -159,24 +168,26 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
+    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -237,15 +248,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -317,17 +327,19 @@
     "migrationhuborchestrator",
     "migrationhubstrategy",
     "mobile",
     "mq",
     "mturk",
     "mwaa",
     "neptune",
+    "neptune-graph",
     "neptunedata",
     "network-firewall",
     "networkmanager",
+    "networkmonitor",
     "nimble",
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
@@ -417,19 +429,21 @@
     "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
+    "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
@@ -461,12 +475,13 @@
     "s3",
     "sns",
     "sqs",
 ]
 PaginatorName = Literal[
     "list_id_mapping_jobs",
     "list_id_mapping_workflows",
+    "list_id_namespaces",
     "list_matching_jobs",
     "list_matching_workflows",
     "list_provider_services",
     "list_schema_mappings",
 ]
```

### Comparing `mypy-boto3-entityresolution-1.34.0/mypy_boto3_entityresolution/paginator.py` & `mypy_boto3_entityresolution-1.34.85/mypy_boto3_entityresolution/paginator.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,56 +8,59 @@
     ```python
     from boto3.session import Session
 
     from mypy_boto3_entityresolution.client import EntityResolutionClient
     from mypy_boto3_entityresolution.paginator import (
         ListIdMappingJobsPaginator,
         ListIdMappingWorkflowsPaginator,
+        ListIdNamespacesPaginator,
         ListMatchingJobsPaginator,
         ListMatchingWorkflowsPaginator,
         ListProviderServicesPaginator,
         ListSchemaMappingsPaginator,
     )
 
     session = Session()
     client: EntityResolutionClient = session.client("entityresolution")
 
     list_id_mapping_jobs_paginator: ListIdMappingJobsPaginator = client.get_paginator("list_id_mapping_jobs")
     list_id_mapping_workflows_paginator: ListIdMappingWorkflowsPaginator = client.get_paginator("list_id_mapping_workflows")
+    list_id_namespaces_paginator: ListIdNamespacesPaginator = client.get_paginator("list_id_namespaces")
     list_matching_jobs_paginator: ListMatchingJobsPaginator = client.get_paginator("list_matching_jobs")
     list_matching_workflows_paginator: ListMatchingWorkflowsPaginator = client.get_paginator("list_matching_workflows")
     list_provider_services_paginator: ListProviderServicesPaginator = client.get_paginator("list_provider_services")
     list_schema_mappings_paginator: ListSchemaMappingsPaginator = client.get_paginator("list_schema_mappings")
     ```
 """
 
 from typing import Generic, Iterator, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
     ListIdMappingJobsOutputTypeDef,
     ListIdMappingWorkflowsOutputTypeDef,
+    ListIdNamespacesOutputTypeDef,
     ListMatchingJobsOutputTypeDef,
     ListMatchingWorkflowsOutputTypeDef,
     ListProviderServicesOutputTypeDef,
     ListSchemaMappingsOutputTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = (
     "ListIdMappingJobsPaginator",
     "ListIdMappingWorkflowsPaginator",
+    "ListIdNamespacesPaginator",
     "ListMatchingJobsPaginator",
     "ListMatchingWorkflowsPaginator",
     "ListProviderServicesPaginator",
     "ListSchemaMappingsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -90,14 +93,29 @@
     ) -> _PageIterator[ListIdMappingWorkflowsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Paginator.ListIdMappingWorkflows.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/paginators/#listidmappingworkflowspaginator)
         """
 
 
+class ListIdNamespacesPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Paginator.ListIdNamespaces)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/paginators/#listidnamespacespaginator)
+    """
+
+    def paginate(
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+    ) -> _PageIterator[ListIdNamespacesOutputTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Paginator.ListIdNamespaces.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/paginators/#listidnamespacespaginator)
+        """
+
+
 class ListMatchingJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Paginator.ListMatchingJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/paginators/#listmatchingjobspaginator)
     """
 
     def paginate(
```

### Comparing `mypy-boto3-entityresolution-1.34.0/mypy_boto3_entityresolution/paginator.pyi` & `mypy_boto3_entityresolution-1.34.85/mypy_boto3_entityresolution/paginator.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -8,49 +8,53 @@
     ```python
     from boto3.session import Session
 
     from mypy_boto3_entityresolution.client import EntityResolutionClient
     from mypy_boto3_entityresolution.paginator import (
         ListIdMappingJobsPaginator,
         ListIdMappingWorkflowsPaginator,
+        ListIdNamespacesPaginator,
         ListMatchingJobsPaginator,
         ListMatchingWorkflowsPaginator,
         ListProviderServicesPaginator,
         ListSchemaMappingsPaginator,
     )
 
     session = Session()
     client: EntityResolutionClient = session.client("entityresolution")
 
     list_id_mapping_jobs_paginator: ListIdMappingJobsPaginator = client.get_paginator("list_id_mapping_jobs")
     list_id_mapping_workflows_paginator: ListIdMappingWorkflowsPaginator = client.get_paginator("list_id_mapping_workflows")
+    list_id_namespaces_paginator: ListIdNamespacesPaginator = client.get_paginator("list_id_namespaces")
     list_matching_jobs_paginator: ListMatchingJobsPaginator = client.get_paginator("list_matching_jobs")
     list_matching_workflows_paginator: ListMatchingWorkflowsPaginator = client.get_paginator("list_matching_workflows")
     list_provider_services_paginator: ListProviderServicesPaginator = client.get_paginator("list_provider_services")
     list_schema_mappings_paginator: ListSchemaMappingsPaginator = client.get_paginator("list_schema_mappings")
     ```
 """
 
 from typing import Generic, Iterator, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
     ListIdMappingJobsOutputTypeDef,
     ListIdMappingWorkflowsOutputTypeDef,
+    ListIdNamespacesOutputTypeDef,
     ListMatchingJobsOutputTypeDef,
     ListMatchingWorkflowsOutputTypeDef,
     ListProviderServicesOutputTypeDef,
     ListSchemaMappingsOutputTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = (
     "ListIdMappingJobsPaginator",
     "ListIdMappingWorkflowsPaginator",
+    "ListIdNamespacesPaginator",
     "ListMatchingJobsPaginator",
     "ListMatchingWorkflowsPaginator",
     "ListProviderServicesPaginator",
     "ListSchemaMappingsPaginator",
 )
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
@@ -85,14 +89,28 @@
         self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListIdMappingWorkflowsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Paginator.ListIdMappingWorkflows.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/paginators/#listidmappingworkflowspaginator)
         """
 
+class ListIdNamespacesPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Paginator.ListIdNamespaces)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/paginators/#listidnamespacespaginator)
+    """
+
+    def paginate(
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+    ) -> _PageIterator[ListIdNamespacesOutputTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Paginator.ListIdNamespaces.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/paginators/#listidnamespacespaginator)
+        """
+
 class ListMatchingJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Paginator.ListMatchingJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/paginators/#listmatchingjobspaginator)
     """
 
     def paginate(
```

### Comparing `mypy-boto3-entityresolution-1.34.0/mypy_boto3_entityresolution/type_defs.py` & `mypy_boto3_entityresolution-1.34.85/mypy_boto3_entityresolution/type_defs.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,30 +2,32 @@
 Type annotations for entityresolution service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_entityresolution.type_defs import IdMappingWorkflowInputSourceTypeDef
+    from mypy_boto3_entityresolution.type_defs import AddPolicyStatementInputRequestTypeDef
 
-    data: IdMappingWorkflowInputSourceTypeDef = ...
+    data: AddPolicyStatementInputRequestTypeDef = ...
     ```
 """
 
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence
 
 from .literals import (
     AttributeMatchingModelType,
+    IdNamespaceTypeType,
     JobStatusType,
     ResolutionTypeType,
     SchemaAttributeTypeType,
     ServiceTypeType,
+    StatementEffectType,
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 12):
@@ -33,87 +35,114 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
+    "AddPolicyStatementInputRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "IdMappingWorkflowInputSourceTypeDef",
     "IdMappingWorkflowOutputSourceTypeDef",
-    "ResponseMetadataTypeDef",
+    "IdNamespaceInputSourceTypeDef",
     "IncrementalRunConfigTypeDef",
     "InputSourceTypeDef",
     "SchemaInputAttributeTypeDef",
     "DeleteIdMappingWorkflowInputRequestTypeDef",
+    "DeleteIdNamespaceInputRequestTypeDef",
     "DeleteMatchingWorkflowInputRequestTypeDef",
+    "DeletePolicyStatementInputRequestTypeDef",
     "DeleteSchemaMappingInputRequestTypeDef",
     "ErrorDetailsTypeDef",
     "GetIdMappingJobInputRequestTypeDef",
     "IdMappingJobMetricsTypeDef",
+    "IdMappingJobOutputSourceTypeDef",
     "GetIdMappingWorkflowInputRequestTypeDef",
+    "GetIdNamespaceInputRequestTypeDef",
     "GetMatchIdInputRequestTypeDef",
     "GetMatchingJobInputRequestTypeDef",
     "JobMetricsTypeDef",
+    "JobOutputSourceTypeDef",
     "GetMatchingWorkflowInputRequestTypeDef",
+    "GetPolicyInputRequestTypeDef",
     "GetProviderServiceInputRequestTypeDef",
+    "ProviderIdNameSpaceConfigurationTypeDef",
     "ProviderIntermediateDataAccessConfigurationTypeDef",
     "GetSchemaMappingInputRequestTypeDef",
     "IdMappingWorkflowSummaryTypeDef",
+    "NamespaceProviderPropertiesTypeDef",
+    "IdNamespaceSummaryTypeDef",
     "IntermediateSourceConfigurationTypeDef",
     "JobSummaryTypeDef",
     "PaginatorConfigTypeDef",
     "ListIdMappingJobsInputRequestTypeDef",
     "ListIdMappingWorkflowsInputRequestTypeDef",
+    "ListIdNamespacesInputRequestTypeDef",
     "ListMatchingJobsInputRequestTypeDef",
     "ListMatchingWorkflowsInputRequestTypeDef",
     "MatchingWorkflowSummaryTypeDef",
     "ListProviderServicesInputRequestTypeDef",
     "ProviderServiceSummaryTypeDef",
     "ListSchemaMappingsInputRequestTypeDef",
     "SchemaMappingSummaryTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
     "OutputAttributeTypeDef",
+    "ProviderSchemaAttributeTypeDef",
     "ProviderMarketplaceConfigurationTypeDef",
+    "PutPolicyInputRequestTypeDef",
     "RuleTypeDef",
-    "StartIdMappingJobInputRequestTypeDef",
     "StartMatchingJobInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
+    "AddPolicyStatementOutputTypeDef",
     "DeleteIdMappingWorkflowOutputTypeDef",
+    "DeleteIdNamespaceOutputTypeDef",
     "DeleteMatchingWorkflowOutputTypeDef",
+    "DeletePolicyStatementOutputTypeDef",
     "DeleteSchemaMappingOutputTypeDef",
     "GetMatchIdOutputTypeDef",
+    "GetPolicyOutputTypeDef",
     "ListTagsForResourceOutputTypeDef",
-    "StartIdMappingJobOutputTypeDef",
+    "PutPolicyOutputTypeDef",
     "StartMatchingJobOutputTypeDef",
     "CreateSchemaMappingInputRequestTypeDef",
     "CreateSchemaMappingOutputTypeDef",
     "GetSchemaMappingOutputTypeDef",
     "UpdateSchemaMappingInputRequestTypeDef",
     "UpdateSchemaMappingOutputTypeDef",
     "GetIdMappingJobOutputTypeDef",
+    "StartIdMappingJobInputRequestTypeDef",
+    "StartIdMappingJobOutputTypeDef",
     "GetMatchingJobOutputTypeDef",
     "ListIdMappingWorkflowsOutputTypeDef",
+    "IdNamespaceIdMappingWorkflowPropertiesTypeDef",
+    "ListIdNamespacesOutputTypeDef",
     "ProviderPropertiesTypeDef",
     "ListIdMappingJobsOutputTypeDef",
     "ListMatchingJobsOutputTypeDef",
     "ListIdMappingJobsInputListIdMappingJobsPaginateTypeDef",
     "ListIdMappingWorkflowsInputListIdMappingWorkflowsPaginateTypeDef",
+    "ListIdNamespacesInputListIdNamespacesPaginateTypeDef",
     "ListMatchingJobsInputListMatchingJobsPaginateTypeDef",
     "ListMatchingWorkflowsInputListMatchingWorkflowsPaginateTypeDef",
     "ListProviderServicesInputListProviderServicesPaginateTypeDef",
     "ListSchemaMappingsInputListSchemaMappingsPaginateTypeDef",
     "ListMatchingWorkflowsOutputTypeDef",
     "ListProviderServicesOutputTypeDef",
     "ListSchemaMappingsOutputTypeDef",
     "OutputSourceTypeDef",
+    "ProviderComponentSchemaTypeDef",
     "ProviderEndpointConfigurationTypeDef",
     "RuleBasedPropertiesTypeDef",
+    "CreateIdNamespaceInputRequestTypeDef",
+    "CreateIdNamespaceOutputTypeDef",
+    "GetIdNamespaceOutputTypeDef",
+    "UpdateIdNamespaceInputRequestTypeDef",
+    "UpdateIdNamespaceOutputTypeDef",
     "IdMappingTechniquesTypeDef",
     "GetProviderServiceOutputTypeDef",
     "ResolutionTechniquesTypeDef",
     "CreateIdMappingWorkflowInputRequestTypeDef",
     "CreateIdMappingWorkflowOutputTypeDef",
     "GetIdMappingWorkflowOutputTypeDef",
     "UpdateIdMappingWorkflowInputRequestTypeDef",
@@ -121,36 +150,55 @@
     "CreateMatchingWorkflowInputRequestTypeDef",
     "CreateMatchingWorkflowOutputTypeDef",
     "GetMatchingWorkflowOutputTypeDef",
     "UpdateMatchingWorkflowInputRequestTypeDef",
     "UpdateMatchingWorkflowOutputTypeDef",
 )
 
+AddPolicyStatementInputRequestTypeDef = TypedDict(
+    "AddPolicyStatementInputRequestTypeDef",
+    {
+        "action": Sequence[str],
+        "arn": str,
+        "effect": StatementEffectType,
+        "principal": Sequence[str],
+        "statementId": str,
+        "condition": NotRequired[str],
+    },
+)
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+        "HostId": NotRequired[str],
+    },
+)
 IdMappingWorkflowInputSourceTypeDef = TypedDict(
     "IdMappingWorkflowInputSourceTypeDef",
     {
         "inputSourceARN": str,
-        "schemaName": str,
+        "schemaName": NotRequired[str],
+        "type": NotRequired[IdNamespaceTypeType],
     },
 )
 IdMappingWorkflowOutputSourceTypeDef = TypedDict(
     "IdMappingWorkflowOutputSourceTypeDef",
     {
         "outputS3Path": str,
         "KMSArn": NotRequired[str],
     },
 )
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+IdNamespaceInputSourceTypeDef = TypedDict(
+    "IdNamespaceInputSourceTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "inputSourceARN": str,
+        "schemaName": NotRequired[str],
     },
 )
 IncrementalRunConfigTypeDef = TypedDict(
     "IncrementalRunConfigTypeDef",
     {
         "incrementalRunType": NotRequired[Literal["IMMEDIATE"]],
     },
@@ -175,20 +223,33 @@
 )
 DeleteIdMappingWorkflowInputRequestTypeDef = TypedDict(
     "DeleteIdMappingWorkflowInputRequestTypeDef",
     {
         "workflowName": str,
     },
 )
+DeleteIdNamespaceInputRequestTypeDef = TypedDict(
+    "DeleteIdNamespaceInputRequestTypeDef",
+    {
+        "idNamespaceName": str,
+    },
+)
 DeleteMatchingWorkflowInputRequestTypeDef = TypedDict(
     "DeleteMatchingWorkflowInputRequestTypeDef",
     {
         "workflowName": str,
     },
 )
+DeletePolicyStatementInputRequestTypeDef = TypedDict(
+    "DeletePolicyStatementInputRequestTypeDef",
+    {
+        "arn": str,
+        "statementId": str,
+    },
+)
 DeleteSchemaMappingInputRequestTypeDef = TypedDict(
     "DeleteSchemaMappingInputRequestTypeDef",
     {
         "schemaName": str,
     },
 )
 ErrorDetailsTypeDef = TypedDict(
@@ -208,25 +269,40 @@
     "IdMappingJobMetricsTypeDef",
     {
         "inputRecords": NotRequired[int],
         "recordsNotProcessed": NotRequired[int],
         "totalRecordsProcessed": NotRequired[int],
     },
 )
+IdMappingJobOutputSourceTypeDef = TypedDict(
+    "IdMappingJobOutputSourceTypeDef",
+    {
+        "outputS3Path": str,
+        "roleArn": str,
+        "KMSArn": NotRequired[str],
+    },
+)
 GetIdMappingWorkflowInputRequestTypeDef = TypedDict(
     "GetIdMappingWorkflowInputRequestTypeDef",
     {
         "workflowName": str,
     },
 )
+GetIdNamespaceInputRequestTypeDef = TypedDict(
+    "GetIdNamespaceInputRequestTypeDef",
+    {
+        "idNamespaceName": str,
+    },
+)
 GetMatchIdInputRequestTypeDef = TypedDict(
     "GetMatchIdInputRequestTypeDef",
     {
         "record": Mapping[str, str],
         "workflowName": str,
+        "applyNormalization": NotRequired[bool],
     },
 )
 GetMatchingJobInputRequestTypeDef = TypedDict(
     "GetMatchingJobInputRequestTypeDef",
     {
         "jobId": str,
         "workflowName": str,
@@ -237,27 +313,49 @@
     {
         "inputRecords": NotRequired[int],
         "matchIDs": NotRequired[int],
         "recordsNotProcessed": NotRequired[int],
         "totalRecordsProcessed": NotRequired[int],
     },
 )
+JobOutputSourceTypeDef = TypedDict(
+    "JobOutputSourceTypeDef",
+    {
+        "outputS3Path": str,
+        "roleArn": str,
+        "KMSArn": NotRequired[str],
+    },
+)
 GetMatchingWorkflowInputRequestTypeDef = TypedDict(
     "GetMatchingWorkflowInputRequestTypeDef",
     {
         "workflowName": str,
     },
 )
+GetPolicyInputRequestTypeDef = TypedDict(
+    "GetPolicyInputRequestTypeDef",
+    {
+        "arn": str,
+    },
+)
 GetProviderServiceInputRequestTypeDef = TypedDict(
     "GetProviderServiceInputRequestTypeDef",
     {
         "providerName": str,
         "providerServiceName": str,
     },
 )
+ProviderIdNameSpaceConfigurationTypeDef = TypedDict(
+    "ProviderIdNameSpaceConfigurationTypeDef",
+    {
+        "description": NotRequired[str],
+        "providerSourceConfigurationDefinition": NotRequired[Dict[str, Any]],
+        "providerTargetConfigurationDefinition": NotRequired[Dict[str, Any]],
+    },
+)
 ProviderIntermediateDataAccessConfigurationTypeDef = TypedDict(
     "ProviderIntermediateDataAccessConfigurationTypeDef",
     {
         "awsAccountIds": NotRequired[List[str]],
         "requiredBucketActions": NotRequired[List[str]],
     },
 )
@@ -272,14 +370,32 @@
     {
         "createdAt": datetime,
         "updatedAt": datetime,
         "workflowArn": str,
         "workflowName": str,
     },
 )
+NamespaceProviderPropertiesTypeDef = TypedDict(
+    "NamespaceProviderPropertiesTypeDef",
+    {
+        "providerServiceArn": str,
+        "providerConfiguration": NotRequired[Mapping[str, Any]],
+    },
+)
+IdNamespaceSummaryTypeDef = TypedDict(
+    "IdNamespaceSummaryTypeDef",
+    {
+        "createdAt": datetime,
+        "idNamespaceArn": str,
+        "idNamespaceName": str,
+        "type": IdNamespaceTypeType,
+        "updatedAt": datetime,
+        "description": NotRequired[str],
+    },
+)
 IntermediateSourceConfigurationTypeDef = TypedDict(
     "IntermediateSourceConfigurationTypeDef",
     {
         "intermediateS3Path": str,
     },
 )
 JobSummaryTypeDef = TypedDict(
@@ -310,14 +426,21 @@
 ListIdMappingWorkflowsInputRequestTypeDef = TypedDict(
     "ListIdMappingWorkflowsInputRequestTypeDef",
     {
         "maxResults": NotRequired[int],
         "nextToken": NotRequired[str],
     },
 )
+ListIdNamespacesInputRequestTypeDef = TypedDict(
+    "ListIdNamespacesInputRequestTypeDef",
+    {
+        "maxResults": NotRequired[int],
+        "nextToken": NotRequired[str],
+    },
+)
 ListMatchingJobsInputRequestTypeDef = TypedDict(
     "ListMatchingJobsInputRequestTypeDef",
     {
         "workflowName": str,
         "maxResults": NotRequired[int],
         "nextToken": NotRequired[str],
     },
@@ -383,36 +506,47 @@
 OutputAttributeTypeDef = TypedDict(
     "OutputAttributeTypeDef",
     {
         "name": str,
         "hashed": NotRequired[bool],
     },
 )
+ProviderSchemaAttributeTypeDef = TypedDict(
+    "ProviderSchemaAttributeTypeDef",
+    {
+        "fieldName": str,
+        "type": SchemaAttributeTypeType,
+        "hashing": NotRequired[bool],
+        "subType": NotRequired[str],
+    },
+)
 ProviderMarketplaceConfigurationTypeDef = TypedDict(
     "ProviderMarketplaceConfigurationTypeDef",
     {
         "assetId": str,
         "dataSetId": str,
         "listingId": str,
         "revisionId": str,
     },
 )
+PutPolicyInputRequestTypeDef = TypedDict(
+    "PutPolicyInputRequestTypeDef",
+    {
+        "arn": str,
+        "policy": str,
+        "token": NotRequired[str],
+    },
+)
 RuleTypeDef = TypedDict(
     "RuleTypeDef",
     {
         "matchingKeys": Sequence[str],
         "ruleName": str,
     },
 )
-StartIdMappingJobInputRequestTypeDef = TypedDict(
-    "StartIdMappingJobInputRequestTypeDef",
-    {
-        "workflowName": str,
-    },
-)
 StartMatchingJobInputRequestTypeDef = TypedDict(
     "StartMatchingJobInputRequestTypeDef",
     {
         "workflowName": str,
     },
 )
 TagResourceInputRequestTypeDef = TypedDict(
@@ -425,53 +559,90 @@
 UntagResourceInputRequestTypeDef = TypedDict(
     "UntagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
+AddPolicyStatementOutputTypeDef = TypedDict(
+    "AddPolicyStatementOutputTypeDef",
+    {
+        "arn": str,
+        "policy": str,
+        "token": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 DeleteIdMappingWorkflowOutputTypeDef = TypedDict(
     "DeleteIdMappingWorkflowOutputTypeDef",
     {
         "message": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+DeleteIdNamespaceOutputTypeDef = TypedDict(
+    "DeleteIdNamespaceOutputTypeDef",
+    {
+        "message": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 DeleteMatchingWorkflowOutputTypeDef = TypedDict(
     "DeleteMatchingWorkflowOutputTypeDef",
     {
         "message": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+DeletePolicyStatementOutputTypeDef = TypedDict(
+    "DeletePolicyStatementOutputTypeDef",
+    {
+        "arn": str,
+        "policy": str,
+        "token": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 DeleteSchemaMappingOutputTypeDef = TypedDict(
     "DeleteSchemaMappingOutputTypeDef",
     {
         "message": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 GetMatchIdOutputTypeDef = TypedDict(
     "GetMatchIdOutputTypeDef",
     {
         "matchId": str,
+        "matchRule": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+GetPolicyOutputTypeDef = TypedDict(
+    "GetPolicyOutputTypeDef",
+    {
+        "arn": str,
+        "policy": str,
+        "token": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListTagsForResourceOutputTypeDef = TypedDict(
     "ListTagsForResourceOutputTypeDef",
     {
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-StartIdMappingJobOutputTypeDef = TypedDict(
-    "StartIdMappingJobOutputTypeDef",
+PutPolicyOutputTypeDef = TypedDict(
+    "PutPolicyOutputTypeDef",
     {
-        "jobId": str,
+        "arn": str,
+        "policy": str,
+        "token": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 StartMatchingJobOutputTypeDef = TypedDict(
     "StartMatchingJobOutputTypeDef",
     {
         "jobId": str,
@@ -532,39 +703,71 @@
 GetIdMappingJobOutputTypeDef = TypedDict(
     "GetIdMappingJobOutputTypeDef",
     {
         "endTime": datetime,
         "errorDetails": ErrorDetailsTypeDef,
         "jobId": str,
         "metrics": IdMappingJobMetricsTypeDef,
+        "outputSourceConfig": List[IdMappingJobOutputSourceTypeDef],
         "startTime": datetime,
         "status": JobStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+StartIdMappingJobInputRequestTypeDef = TypedDict(
+    "StartIdMappingJobInputRequestTypeDef",
+    {
+        "workflowName": str,
+        "outputSourceConfig": NotRequired[Sequence[IdMappingJobOutputSourceTypeDef]],
+    },
+)
+StartIdMappingJobOutputTypeDef = TypedDict(
+    "StartIdMappingJobOutputTypeDef",
+    {
+        "jobId": str,
+        "outputSourceConfig": List[IdMappingJobOutputSourceTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 GetMatchingJobOutputTypeDef = TypedDict(
     "GetMatchingJobOutputTypeDef",
     {
         "endTime": datetime,
         "errorDetails": ErrorDetailsTypeDef,
         "jobId": str,
         "metrics": JobMetricsTypeDef,
+        "outputSourceConfig": List[JobOutputSourceTypeDef],
         "startTime": datetime,
         "status": JobStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListIdMappingWorkflowsOutputTypeDef = TypedDict(
     "ListIdMappingWorkflowsOutputTypeDef",
     {
         "nextToken": str,
         "workflowSummaries": List[IdMappingWorkflowSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+IdNamespaceIdMappingWorkflowPropertiesTypeDef = TypedDict(
+    "IdNamespaceIdMappingWorkflowPropertiesTypeDef",
+    {
+        "idMappingType": Literal["PROVIDER"],
+        "providerProperties": NotRequired[NamespaceProviderPropertiesTypeDef],
+    },
+)
+ListIdNamespacesOutputTypeDef = TypedDict(
+    "ListIdNamespacesOutputTypeDef",
+    {
+        "idNamespaceSummaries": List[IdNamespaceSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 ProviderPropertiesTypeDef = TypedDict(
     "ProviderPropertiesTypeDef",
     {
         "providerServiceArn": str,
         "intermediateSourceConfiguration": NotRequired[IntermediateSourceConfigurationTypeDef],
         "providerConfiguration": NotRequired[Mapping[str, Any]],
     },
@@ -594,14 +797,20 @@
 )
 ListIdMappingWorkflowsInputListIdMappingWorkflowsPaginateTypeDef = TypedDict(
     "ListIdMappingWorkflowsInputListIdMappingWorkflowsPaginateTypeDef",
     {
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
+ListIdNamespacesInputListIdNamespacesPaginateTypeDef = TypedDict(
+    "ListIdNamespacesInputListIdNamespacesPaginateTypeDef",
+    {
+        "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
+    },
+)
 ListMatchingJobsInputListMatchingJobsPaginateTypeDef = TypedDict(
     "ListMatchingJobsInputListMatchingJobsPaginateTypeDef",
     {
         "workflowName": str,
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
@@ -653,44 +862,125 @@
     {
         "output": Sequence[OutputAttributeTypeDef],
         "outputS3Path": str,
         "KMSArn": NotRequired[str],
         "applyNormalization": NotRequired[bool],
     },
 )
+ProviderComponentSchemaTypeDef = TypedDict(
+    "ProviderComponentSchemaTypeDef",
+    {
+        "providerSchemaAttributes": NotRequired[List[ProviderSchemaAttributeTypeDef]],
+        "schemas": NotRequired[List[List[str]]],
+    },
+)
 ProviderEndpointConfigurationTypeDef = TypedDict(
     "ProviderEndpointConfigurationTypeDef",
     {
         "marketplaceConfiguration": NotRequired[ProviderMarketplaceConfigurationTypeDef],
     },
 )
 RuleBasedPropertiesTypeDef = TypedDict(
     "RuleBasedPropertiesTypeDef",
     {
         "attributeMatchingModel": AttributeMatchingModelType,
         "rules": Sequence[RuleTypeDef],
     },
 )
+CreateIdNamespaceInputRequestTypeDef = TypedDict(
+    "CreateIdNamespaceInputRequestTypeDef",
+    {
+        "idNamespaceName": str,
+        "type": IdNamespaceTypeType,
+        "description": NotRequired[str],
+        "idMappingWorkflowProperties": NotRequired[
+            Sequence[IdNamespaceIdMappingWorkflowPropertiesTypeDef]
+        ],
+        "inputSourceConfig": NotRequired[Sequence[IdNamespaceInputSourceTypeDef]],
+        "roleArn": NotRequired[str],
+        "tags": NotRequired[Mapping[str, str]],
+    },
+)
+CreateIdNamespaceOutputTypeDef = TypedDict(
+    "CreateIdNamespaceOutputTypeDef",
+    {
+        "createdAt": datetime,
+        "description": str,
+        "idMappingWorkflowProperties": List[IdNamespaceIdMappingWorkflowPropertiesTypeDef],
+        "idNamespaceArn": str,
+        "idNamespaceName": str,
+        "inputSourceConfig": List[IdNamespaceInputSourceTypeDef],
+        "roleArn": str,
+        "tags": Dict[str, str],
+        "type": IdNamespaceTypeType,
+        "updatedAt": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+GetIdNamespaceOutputTypeDef = TypedDict(
+    "GetIdNamespaceOutputTypeDef",
+    {
+        "createdAt": datetime,
+        "description": str,
+        "idMappingWorkflowProperties": List[IdNamespaceIdMappingWorkflowPropertiesTypeDef],
+        "idNamespaceArn": str,
+        "idNamespaceName": str,
+        "inputSourceConfig": List[IdNamespaceInputSourceTypeDef],
+        "roleArn": str,
+        "tags": Dict[str, str],
+        "type": IdNamespaceTypeType,
+        "updatedAt": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+UpdateIdNamespaceInputRequestTypeDef = TypedDict(
+    "UpdateIdNamespaceInputRequestTypeDef",
+    {
+        "idNamespaceName": str,
+        "description": NotRequired[str],
+        "idMappingWorkflowProperties": NotRequired[
+            Sequence[IdNamespaceIdMappingWorkflowPropertiesTypeDef]
+        ],
+        "inputSourceConfig": NotRequired[Sequence[IdNamespaceInputSourceTypeDef]],
+        "roleArn": NotRequired[str],
+    },
+)
+UpdateIdNamespaceOutputTypeDef = TypedDict(
+    "UpdateIdNamespaceOutputTypeDef",
+    {
+        "createdAt": datetime,
+        "description": str,
+        "idMappingWorkflowProperties": List[IdNamespaceIdMappingWorkflowPropertiesTypeDef],
+        "idNamespaceArn": str,
+        "idNamespaceName": str,
+        "inputSourceConfig": List[IdNamespaceInputSourceTypeDef],
+        "roleArn": str,
+        "type": IdNamespaceTypeType,
+        "updatedAt": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 IdMappingTechniquesTypeDef = TypedDict(
     "IdMappingTechniquesTypeDef",
     {
         "idMappingType": Literal["PROVIDER"],
-        "providerProperties": ProviderPropertiesTypeDef,
+        "providerProperties": NotRequired[ProviderPropertiesTypeDef],
     },
 )
 GetProviderServiceOutputTypeDef = TypedDict(
     "GetProviderServiceOutputTypeDef",
     {
         "anonymizedOutput": bool,
+        "providerComponentSchema": ProviderComponentSchemaTypeDef,
         "providerConfigurationDefinition": Dict[str, Any],
         "providerEndpointConfiguration": ProviderEndpointConfigurationTypeDef,
         "providerEntityOutputDefinition": Dict[str, Any],
-        "providerIntermediateDataAccessConfiguration": (
-            ProviderIntermediateDataAccessConfigurationTypeDef
-        ),
+        "providerIdNameSpaceConfiguration": ProviderIdNameSpaceConfigurationTypeDef,
+        "providerIntermediateDataAccessConfiguration": ProviderIntermediateDataAccessConfigurationTypeDef,
+        "providerJobConfiguration": Dict[str, Any],
         "providerName": str,
         "providerServiceArn": str,
         "providerServiceDisplayName": str,
         "providerServiceName": str,
         "providerServiceType": ServiceTypeType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -704,18 +994,18 @@
     },
 )
 CreateIdMappingWorkflowInputRequestTypeDef = TypedDict(
     "CreateIdMappingWorkflowInputRequestTypeDef",
     {
         "idMappingTechniques": IdMappingTechniquesTypeDef,
         "inputSourceConfig": Sequence[IdMappingWorkflowInputSourceTypeDef],
-        "outputSourceConfig": Sequence[IdMappingWorkflowOutputSourceTypeDef],
         "roleArn": str,
         "workflowName": str,
         "description": NotRequired[str],
+        "outputSourceConfig": NotRequired[Sequence[IdMappingWorkflowOutputSourceTypeDef]],
         "tags": NotRequired[Mapping[str, str]],
     },
 )
 CreateIdMappingWorkflowOutputTypeDef = TypedDict(
     "CreateIdMappingWorkflowOutputTypeDef",
     {
         "description": str,
@@ -745,18 +1035,18 @@
     },
 )
 UpdateIdMappingWorkflowInputRequestTypeDef = TypedDict(
     "UpdateIdMappingWorkflowInputRequestTypeDef",
     {
         "idMappingTechniques": IdMappingTechniquesTypeDef,
         "inputSourceConfig": Sequence[IdMappingWorkflowInputSourceTypeDef],
-        "outputSourceConfig": Sequence[IdMappingWorkflowOutputSourceTypeDef],
         "roleArn": str,
         "workflowName": str,
         "description": NotRequired[str],
+        "outputSourceConfig": NotRequired[Sequence[IdMappingWorkflowOutputSourceTypeDef]],
     },
 )
 UpdateIdMappingWorkflowOutputTypeDef = TypedDict(
     "UpdateIdMappingWorkflowOutputTypeDef",
     {
         "description": str,
         "idMappingTechniques": IdMappingTechniquesTypeDef,
```

### Comparing `mypy-boto3-entityresolution-1.34.0/mypy_boto3_entityresolution/type_defs.pyi` & `mypy_boto3_entityresolution-1.34.85/mypy_boto3_entityresolution/type_defs.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -2,30 +2,32 @@
 Type annotations for entityresolution service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_entityresolution.type_defs import IdMappingWorkflowInputSourceTypeDef
+    from mypy_boto3_entityresolution.type_defs import AddPolicyStatementInputRequestTypeDef
 
-    data: IdMappingWorkflowInputSourceTypeDef = ...
+    data: AddPolicyStatementInputRequestTypeDef = ...
     ```
 """
 
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence
 
 from .literals import (
     AttributeMatchingModelType,
+    IdNamespaceTypeType,
     JobStatusType,
     ResolutionTypeType,
     SchemaAttributeTypeType,
     ServiceTypeType,
+    StatementEffectType,
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 12):
@@ -34,85 +36,113 @@
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "AddPolicyStatementInputRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "IdMappingWorkflowInputSourceTypeDef",
     "IdMappingWorkflowOutputSourceTypeDef",
-    "ResponseMetadataTypeDef",
+    "IdNamespaceInputSourceTypeDef",
     "IncrementalRunConfigTypeDef",
     "InputSourceTypeDef",
     "SchemaInputAttributeTypeDef",
     "DeleteIdMappingWorkflowInputRequestTypeDef",
+    "DeleteIdNamespaceInputRequestTypeDef",
     "DeleteMatchingWorkflowInputRequestTypeDef",
+    "DeletePolicyStatementInputRequestTypeDef",
     "DeleteSchemaMappingInputRequestTypeDef",
     "ErrorDetailsTypeDef",
     "GetIdMappingJobInputRequestTypeDef",
     "IdMappingJobMetricsTypeDef",
+    "IdMappingJobOutputSourceTypeDef",
     "GetIdMappingWorkflowInputRequestTypeDef",
+    "GetIdNamespaceInputRequestTypeDef",
     "GetMatchIdInputRequestTypeDef",
     "GetMatchingJobInputRequestTypeDef",
     "JobMetricsTypeDef",
+    "JobOutputSourceTypeDef",
     "GetMatchingWorkflowInputRequestTypeDef",
+    "GetPolicyInputRequestTypeDef",
     "GetProviderServiceInputRequestTypeDef",
+    "ProviderIdNameSpaceConfigurationTypeDef",
     "ProviderIntermediateDataAccessConfigurationTypeDef",
     "GetSchemaMappingInputRequestTypeDef",
     "IdMappingWorkflowSummaryTypeDef",
+    "NamespaceProviderPropertiesTypeDef",
+    "IdNamespaceSummaryTypeDef",
     "IntermediateSourceConfigurationTypeDef",
     "JobSummaryTypeDef",
     "PaginatorConfigTypeDef",
     "ListIdMappingJobsInputRequestTypeDef",
     "ListIdMappingWorkflowsInputRequestTypeDef",
+    "ListIdNamespacesInputRequestTypeDef",
     "ListMatchingJobsInputRequestTypeDef",
     "ListMatchingWorkflowsInputRequestTypeDef",
     "MatchingWorkflowSummaryTypeDef",
     "ListProviderServicesInputRequestTypeDef",
     "ProviderServiceSummaryTypeDef",
     "ListSchemaMappingsInputRequestTypeDef",
     "SchemaMappingSummaryTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
     "OutputAttributeTypeDef",
+    "ProviderSchemaAttributeTypeDef",
     "ProviderMarketplaceConfigurationTypeDef",
+    "PutPolicyInputRequestTypeDef",
     "RuleTypeDef",
-    "StartIdMappingJobInputRequestTypeDef",
     "StartMatchingJobInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
+    "AddPolicyStatementOutputTypeDef",
     "DeleteIdMappingWorkflowOutputTypeDef",
+    "DeleteIdNamespaceOutputTypeDef",
     "DeleteMatchingWorkflowOutputTypeDef",
+    "DeletePolicyStatementOutputTypeDef",
     "DeleteSchemaMappingOutputTypeDef",
     "GetMatchIdOutputTypeDef",
+    "GetPolicyOutputTypeDef",
     "ListTagsForResourceOutputTypeDef",
-    "StartIdMappingJobOutputTypeDef",
+    "PutPolicyOutputTypeDef",
     "StartMatchingJobOutputTypeDef",
     "CreateSchemaMappingInputRequestTypeDef",
     "CreateSchemaMappingOutputTypeDef",
     "GetSchemaMappingOutputTypeDef",
     "UpdateSchemaMappingInputRequestTypeDef",
     "UpdateSchemaMappingOutputTypeDef",
     "GetIdMappingJobOutputTypeDef",
+    "StartIdMappingJobInputRequestTypeDef",
+    "StartIdMappingJobOutputTypeDef",
     "GetMatchingJobOutputTypeDef",
     "ListIdMappingWorkflowsOutputTypeDef",
+    "IdNamespaceIdMappingWorkflowPropertiesTypeDef",
+    "ListIdNamespacesOutputTypeDef",
     "ProviderPropertiesTypeDef",
     "ListIdMappingJobsOutputTypeDef",
     "ListMatchingJobsOutputTypeDef",
     "ListIdMappingJobsInputListIdMappingJobsPaginateTypeDef",
     "ListIdMappingWorkflowsInputListIdMappingWorkflowsPaginateTypeDef",
+    "ListIdNamespacesInputListIdNamespacesPaginateTypeDef",
     "ListMatchingJobsInputListMatchingJobsPaginateTypeDef",
     "ListMatchingWorkflowsInputListMatchingWorkflowsPaginateTypeDef",
     "ListProviderServicesInputListProviderServicesPaginateTypeDef",
     "ListSchemaMappingsInputListSchemaMappingsPaginateTypeDef",
     "ListMatchingWorkflowsOutputTypeDef",
     "ListProviderServicesOutputTypeDef",
     "ListSchemaMappingsOutputTypeDef",
     "OutputSourceTypeDef",
+    "ProviderComponentSchemaTypeDef",
     "ProviderEndpointConfigurationTypeDef",
     "RuleBasedPropertiesTypeDef",
+    "CreateIdNamespaceInputRequestTypeDef",
+    "CreateIdNamespaceOutputTypeDef",
+    "GetIdNamespaceOutputTypeDef",
+    "UpdateIdNamespaceInputRequestTypeDef",
+    "UpdateIdNamespaceOutputTypeDef",
     "IdMappingTechniquesTypeDef",
     "GetProviderServiceOutputTypeDef",
     "ResolutionTechniquesTypeDef",
     "CreateIdMappingWorkflowInputRequestTypeDef",
     "CreateIdMappingWorkflowOutputTypeDef",
     "GetIdMappingWorkflowOutputTypeDef",
     "UpdateIdMappingWorkflowInputRequestTypeDef",
@@ -120,36 +150,55 @@
     "CreateMatchingWorkflowInputRequestTypeDef",
     "CreateMatchingWorkflowOutputTypeDef",
     "GetMatchingWorkflowOutputTypeDef",
     "UpdateMatchingWorkflowInputRequestTypeDef",
     "UpdateMatchingWorkflowOutputTypeDef",
 )
 
+AddPolicyStatementInputRequestTypeDef = TypedDict(
+    "AddPolicyStatementInputRequestTypeDef",
+    {
+        "action": Sequence[str],
+        "arn": str,
+        "effect": StatementEffectType,
+        "principal": Sequence[str],
+        "statementId": str,
+        "condition": NotRequired[str],
+    },
+)
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+        "HostId": NotRequired[str],
+    },
+)
 IdMappingWorkflowInputSourceTypeDef = TypedDict(
     "IdMappingWorkflowInputSourceTypeDef",
     {
         "inputSourceARN": str,
-        "schemaName": str,
+        "schemaName": NotRequired[str],
+        "type": NotRequired[IdNamespaceTypeType],
     },
 )
 IdMappingWorkflowOutputSourceTypeDef = TypedDict(
     "IdMappingWorkflowOutputSourceTypeDef",
     {
         "outputS3Path": str,
         "KMSArn": NotRequired[str],
     },
 )
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+IdNamespaceInputSourceTypeDef = TypedDict(
+    "IdNamespaceInputSourceTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "inputSourceARN": str,
+        "schemaName": NotRequired[str],
     },
 )
 IncrementalRunConfigTypeDef = TypedDict(
     "IncrementalRunConfigTypeDef",
     {
         "incrementalRunType": NotRequired[Literal["IMMEDIATE"]],
     },
@@ -174,20 +223,33 @@
 )
 DeleteIdMappingWorkflowInputRequestTypeDef = TypedDict(
     "DeleteIdMappingWorkflowInputRequestTypeDef",
     {
         "workflowName": str,
     },
 )
+DeleteIdNamespaceInputRequestTypeDef = TypedDict(
+    "DeleteIdNamespaceInputRequestTypeDef",
+    {
+        "idNamespaceName": str,
+    },
+)
 DeleteMatchingWorkflowInputRequestTypeDef = TypedDict(
     "DeleteMatchingWorkflowInputRequestTypeDef",
     {
         "workflowName": str,
     },
 )
+DeletePolicyStatementInputRequestTypeDef = TypedDict(
+    "DeletePolicyStatementInputRequestTypeDef",
+    {
+        "arn": str,
+        "statementId": str,
+    },
+)
 DeleteSchemaMappingInputRequestTypeDef = TypedDict(
     "DeleteSchemaMappingInputRequestTypeDef",
     {
         "schemaName": str,
     },
 )
 ErrorDetailsTypeDef = TypedDict(
@@ -207,25 +269,40 @@
     "IdMappingJobMetricsTypeDef",
     {
         "inputRecords": NotRequired[int],
         "recordsNotProcessed": NotRequired[int],
         "totalRecordsProcessed": NotRequired[int],
     },
 )
+IdMappingJobOutputSourceTypeDef = TypedDict(
+    "IdMappingJobOutputSourceTypeDef",
+    {
+        "outputS3Path": str,
+        "roleArn": str,
+        "KMSArn": NotRequired[str],
+    },
+)
 GetIdMappingWorkflowInputRequestTypeDef = TypedDict(
     "GetIdMappingWorkflowInputRequestTypeDef",
     {
         "workflowName": str,
     },
 )
+GetIdNamespaceInputRequestTypeDef = TypedDict(
+    "GetIdNamespaceInputRequestTypeDef",
+    {
+        "idNamespaceName": str,
+    },
+)
 GetMatchIdInputRequestTypeDef = TypedDict(
     "GetMatchIdInputRequestTypeDef",
     {
         "record": Mapping[str, str],
         "workflowName": str,
+        "applyNormalization": NotRequired[bool],
     },
 )
 GetMatchingJobInputRequestTypeDef = TypedDict(
     "GetMatchingJobInputRequestTypeDef",
     {
         "jobId": str,
         "workflowName": str,
@@ -236,27 +313,49 @@
     {
         "inputRecords": NotRequired[int],
         "matchIDs": NotRequired[int],
         "recordsNotProcessed": NotRequired[int],
         "totalRecordsProcessed": NotRequired[int],
     },
 )
+JobOutputSourceTypeDef = TypedDict(
+    "JobOutputSourceTypeDef",
+    {
+        "outputS3Path": str,
+        "roleArn": str,
+        "KMSArn": NotRequired[str],
+    },
+)
 GetMatchingWorkflowInputRequestTypeDef = TypedDict(
     "GetMatchingWorkflowInputRequestTypeDef",
     {
         "workflowName": str,
     },
 )
+GetPolicyInputRequestTypeDef = TypedDict(
+    "GetPolicyInputRequestTypeDef",
+    {
+        "arn": str,
+    },
+)
 GetProviderServiceInputRequestTypeDef = TypedDict(
     "GetProviderServiceInputRequestTypeDef",
     {
         "providerName": str,
         "providerServiceName": str,
     },
 )
+ProviderIdNameSpaceConfigurationTypeDef = TypedDict(
+    "ProviderIdNameSpaceConfigurationTypeDef",
+    {
+        "description": NotRequired[str],
+        "providerSourceConfigurationDefinition": NotRequired[Dict[str, Any]],
+        "providerTargetConfigurationDefinition": NotRequired[Dict[str, Any]],
+    },
+)
 ProviderIntermediateDataAccessConfigurationTypeDef = TypedDict(
     "ProviderIntermediateDataAccessConfigurationTypeDef",
     {
         "awsAccountIds": NotRequired[List[str]],
         "requiredBucketActions": NotRequired[List[str]],
     },
 )
@@ -271,14 +370,32 @@
     {
         "createdAt": datetime,
         "updatedAt": datetime,
         "workflowArn": str,
         "workflowName": str,
     },
 )
+NamespaceProviderPropertiesTypeDef = TypedDict(
+    "NamespaceProviderPropertiesTypeDef",
+    {
+        "providerServiceArn": str,
+        "providerConfiguration": NotRequired[Mapping[str, Any]],
+    },
+)
+IdNamespaceSummaryTypeDef = TypedDict(
+    "IdNamespaceSummaryTypeDef",
+    {
+        "createdAt": datetime,
+        "idNamespaceArn": str,
+        "idNamespaceName": str,
+        "type": IdNamespaceTypeType,
+        "updatedAt": datetime,
+        "description": NotRequired[str],
+    },
+)
 IntermediateSourceConfigurationTypeDef = TypedDict(
     "IntermediateSourceConfigurationTypeDef",
     {
         "intermediateS3Path": str,
     },
 )
 JobSummaryTypeDef = TypedDict(
@@ -309,14 +426,21 @@
 ListIdMappingWorkflowsInputRequestTypeDef = TypedDict(
     "ListIdMappingWorkflowsInputRequestTypeDef",
     {
         "maxResults": NotRequired[int],
         "nextToken": NotRequired[str],
     },
 )
+ListIdNamespacesInputRequestTypeDef = TypedDict(
+    "ListIdNamespacesInputRequestTypeDef",
+    {
+        "maxResults": NotRequired[int],
+        "nextToken": NotRequired[str],
+    },
+)
 ListMatchingJobsInputRequestTypeDef = TypedDict(
     "ListMatchingJobsInputRequestTypeDef",
     {
         "workflowName": str,
         "maxResults": NotRequired[int],
         "nextToken": NotRequired[str],
     },
@@ -382,36 +506,47 @@
 OutputAttributeTypeDef = TypedDict(
     "OutputAttributeTypeDef",
     {
         "name": str,
         "hashed": NotRequired[bool],
     },
 )
+ProviderSchemaAttributeTypeDef = TypedDict(
+    "ProviderSchemaAttributeTypeDef",
+    {
+        "fieldName": str,
+        "type": SchemaAttributeTypeType,
+        "hashing": NotRequired[bool],
+        "subType": NotRequired[str],
+    },
+)
 ProviderMarketplaceConfigurationTypeDef = TypedDict(
     "ProviderMarketplaceConfigurationTypeDef",
     {
         "assetId": str,
         "dataSetId": str,
         "listingId": str,
         "revisionId": str,
     },
 )
+PutPolicyInputRequestTypeDef = TypedDict(
+    "PutPolicyInputRequestTypeDef",
+    {
+        "arn": str,
+        "policy": str,
+        "token": NotRequired[str],
+    },
+)
 RuleTypeDef = TypedDict(
     "RuleTypeDef",
     {
         "matchingKeys": Sequence[str],
         "ruleName": str,
     },
 )
-StartIdMappingJobInputRequestTypeDef = TypedDict(
-    "StartIdMappingJobInputRequestTypeDef",
-    {
-        "workflowName": str,
-    },
-)
 StartMatchingJobInputRequestTypeDef = TypedDict(
     "StartMatchingJobInputRequestTypeDef",
     {
         "workflowName": str,
     },
 )
 TagResourceInputRequestTypeDef = TypedDict(
@@ -424,53 +559,90 @@
 UntagResourceInputRequestTypeDef = TypedDict(
     "UntagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
+AddPolicyStatementOutputTypeDef = TypedDict(
+    "AddPolicyStatementOutputTypeDef",
+    {
+        "arn": str,
+        "policy": str,
+        "token": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 DeleteIdMappingWorkflowOutputTypeDef = TypedDict(
     "DeleteIdMappingWorkflowOutputTypeDef",
     {
         "message": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+DeleteIdNamespaceOutputTypeDef = TypedDict(
+    "DeleteIdNamespaceOutputTypeDef",
+    {
+        "message": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 DeleteMatchingWorkflowOutputTypeDef = TypedDict(
     "DeleteMatchingWorkflowOutputTypeDef",
     {
         "message": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+DeletePolicyStatementOutputTypeDef = TypedDict(
+    "DeletePolicyStatementOutputTypeDef",
+    {
+        "arn": str,
+        "policy": str,
+        "token": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 DeleteSchemaMappingOutputTypeDef = TypedDict(
     "DeleteSchemaMappingOutputTypeDef",
     {
         "message": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 GetMatchIdOutputTypeDef = TypedDict(
     "GetMatchIdOutputTypeDef",
     {
         "matchId": str,
+        "matchRule": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+GetPolicyOutputTypeDef = TypedDict(
+    "GetPolicyOutputTypeDef",
+    {
+        "arn": str,
+        "policy": str,
+        "token": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListTagsForResourceOutputTypeDef = TypedDict(
     "ListTagsForResourceOutputTypeDef",
     {
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-StartIdMappingJobOutputTypeDef = TypedDict(
-    "StartIdMappingJobOutputTypeDef",
+PutPolicyOutputTypeDef = TypedDict(
+    "PutPolicyOutputTypeDef",
     {
-        "jobId": str,
+        "arn": str,
+        "policy": str,
+        "token": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 StartMatchingJobOutputTypeDef = TypedDict(
     "StartMatchingJobOutputTypeDef",
     {
         "jobId": str,
@@ -531,39 +703,71 @@
 GetIdMappingJobOutputTypeDef = TypedDict(
     "GetIdMappingJobOutputTypeDef",
     {
         "endTime": datetime,
         "errorDetails": ErrorDetailsTypeDef,
         "jobId": str,
         "metrics": IdMappingJobMetricsTypeDef,
+        "outputSourceConfig": List[IdMappingJobOutputSourceTypeDef],
         "startTime": datetime,
         "status": JobStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+StartIdMappingJobInputRequestTypeDef = TypedDict(
+    "StartIdMappingJobInputRequestTypeDef",
+    {
+        "workflowName": str,
+        "outputSourceConfig": NotRequired[Sequence[IdMappingJobOutputSourceTypeDef]],
+    },
+)
+StartIdMappingJobOutputTypeDef = TypedDict(
+    "StartIdMappingJobOutputTypeDef",
+    {
+        "jobId": str,
+        "outputSourceConfig": List[IdMappingJobOutputSourceTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 GetMatchingJobOutputTypeDef = TypedDict(
     "GetMatchingJobOutputTypeDef",
     {
         "endTime": datetime,
         "errorDetails": ErrorDetailsTypeDef,
         "jobId": str,
         "metrics": JobMetricsTypeDef,
+        "outputSourceConfig": List[JobOutputSourceTypeDef],
         "startTime": datetime,
         "status": JobStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListIdMappingWorkflowsOutputTypeDef = TypedDict(
     "ListIdMappingWorkflowsOutputTypeDef",
     {
         "nextToken": str,
         "workflowSummaries": List[IdMappingWorkflowSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+IdNamespaceIdMappingWorkflowPropertiesTypeDef = TypedDict(
+    "IdNamespaceIdMappingWorkflowPropertiesTypeDef",
+    {
+        "idMappingType": Literal["PROVIDER"],
+        "providerProperties": NotRequired[NamespaceProviderPropertiesTypeDef],
+    },
+)
+ListIdNamespacesOutputTypeDef = TypedDict(
+    "ListIdNamespacesOutputTypeDef",
+    {
+        "idNamespaceSummaries": List[IdNamespaceSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 ProviderPropertiesTypeDef = TypedDict(
     "ProviderPropertiesTypeDef",
     {
         "providerServiceArn": str,
         "intermediateSourceConfiguration": NotRequired[IntermediateSourceConfigurationTypeDef],
         "providerConfiguration": NotRequired[Mapping[str, Any]],
     },
@@ -593,14 +797,20 @@
 )
 ListIdMappingWorkflowsInputListIdMappingWorkflowsPaginateTypeDef = TypedDict(
     "ListIdMappingWorkflowsInputListIdMappingWorkflowsPaginateTypeDef",
     {
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
+ListIdNamespacesInputListIdNamespacesPaginateTypeDef = TypedDict(
+    "ListIdNamespacesInputListIdNamespacesPaginateTypeDef",
+    {
+        "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
+    },
+)
 ListMatchingJobsInputListMatchingJobsPaginateTypeDef = TypedDict(
     "ListMatchingJobsInputListMatchingJobsPaginateTypeDef",
     {
         "workflowName": str,
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
@@ -652,44 +862,125 @@
     {
         "output": Sequence[OutputAttributeTypeDef],
         "outputS3Path": str,
         "KMSArn": NotRequired[str],
         "applyNormalization": NotRequired[bool],
     },
 )
+ProviderComponentSchemaTypeDef = TypedDict(
+    "ProviderComponentSchemaTypeDef",
+    {
+        "providerSchemaAttributes": NotRequired[List[ProviderSchemaAttributeTypeDef]],
+        "schemas": NotRequired[List[List[str]]],
+    },
+)
 ProviderEndpointConfigurationTypeDef = TypedDict(
     "ProviderEndpointConfigurationTypeDef",
     {
         "marketplaceConfiguration": NotRequired[ProviderMarketplaceConfigurationTypeDef],
     },
 )
 RuleBasedPropertiesTypeDef = TypedDict(
     "RuleBasedPropertiesTypeDef",
     {
         "attributeMatchingModel": AttributeMatchingModelType,
         "rules": Sequence[RuleTypeDef],
     },
 )
+CreateIdNamespaceInputRequestTypeDef = TypedDict(
+    "CreateIdNamespaceInputRequestTypeDef",
+    {
+        "idNamespaceName": str,
+        "type": IdNamespaceTypeType,
+        "description": NotRequired[str],
+        "idMappingWorkflowProperties": NotRequired[
+            Sequence[IdNamespaceIdMappingWorkflowPropertiesTypeDef]
+        ],
+        "inputSourceConfig": NotRequired[Sequence[IdNamespaceInputSourceTypeDef]],
+        "roleArn": NotRequired[str],
+        "tags": NotRequired[Mapping[str, str]],
+    },
+)
+CreateIdNamespaceOutputTypeDef = TypedDict(
+    "CreateIdNamespaceOutputTypeDef",
+    {
+        "createdAt": datetime,
+        "description": str,
+        "idMappingWorkflowProperties": List[IdNamespaceIdMappingWorkflowPropertiesTypeDef],
+        "idNamespaceArn": str,
+        "idNamespaceName": str,
+        "inputSourceConfig": List[IdNamespaceInputSourceTypeDef],
+        "roleArn": str,
+        "tags": Dict[str, str],
+        "type": IdNamespaceTypeType,
+        "updatedAt": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+GetIdNamespaceOutputTypeDef = TypedDict(
+    "GetIdNamespaceOutputTypeDef",
+    {
+        "createdAt": datetime,
+        "description": str,
+        "idMappingWorkflowProperties": List[IdNamespaceIdMappingWorkflowPropertiesTypeDef],
+        "idNamespaceArn": str,
+        "idNamespaceName": str,
+        "inputSourceConfig": List[IdNamespaceInputSourceTypeDef],
+        "roleArn": str,
+        "tags": Dict[str, str],
+        "type": IdNamespaceTypeType,
+        "updatedAt": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+UpdateIdNamespaceInputRequestTypeDef = TypedDict(
+    "UpdateIdNamespaceInputRequestTypeDef",
+    {
+        "idNamespaceName": str,
+        "description": NotRequired[str],
+        "idMappingWorkflowProperties": NotRequired[
+            Sequence[IdNamespaceIdMappingWorkflowPropertiesTypeDef]
+        ],
+        "inputSourceConfig": NotRequired[Sequence[IdNamespaceInputSourceTypeDef]],
+        "roleArn": NotRequired[str],
+    },
+)
+UpdateIdNamespaceOutputTypeDef = TypedDict(
+    "UpdateIdNamespaceOutputTypeDef",
+    {
+        "createdAt": datetime,
+        "description": str,
+        "idMappingWorkflowProperties": List[IdNamespaceIdMappingWorkflowPropertiesTypeDef],
+        "idNamespaceArn": str,
+        "idNamespaceName": str,
+        "inputSourceConfig": List[IdNamespaceInputSourceTypeDef],
+        "roleArn": str,
+        "type": IdNamespaceTypeType,
+        "updatedAt": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 IdMappingTechniquesTypeDef = TypedDict(
     "IdMappingTechniquesTypeDef",
     {
         "idMappingType": Literal["PROVIDER"],
-        "providerProperties": ProviderPropertiesTypeDef,
+        "providerProperties": NotRequired[ProviderPropertiesTypeDef],
     },
 )
 GetProviderServiceOutputTypeDef = TypedDict(
     "GetProviderServiceOutputTypeDef",
     {
         "anonymizedOutput": bool,
+        "providerComponentSchema": ProviderComponentSchemaTypeDef,
         "providerConfigurationDefinition": Dict[str, Any],
         "providerEndpointConfiguration": ProviderEndpointConfigurationTypeDef,
         "providerEntityOutputDefinition": Dict[str, Any],
-        "providerIntermediateDataAccessConfiguration": (
-            ProviderIntermediateDataAccessConfigurationTypeDef
-        ),
+        "providerIdNameSpaceConfiguration": ProviderIdNameSpaceConfigurationTypeDef,
+        "providerIntermediateDataAccessConfiguration": ProviderIntermediateDataAccessConfigurationTypeDef,
+        "providerJobConfiguration": Dict[str, Any],
         "providerName": str,
         "providerServiceArn": str,
         "providerServiceDisplayName": str,
         "providerServiceName": str,
         "providerServiceType": ServiceTypeType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -703,18 +994,18 @@
     },
 )
 CreateIdMappingWorkflowInputRequestTypeDef = TypedDict(
     "CreateIdMappingWorkflowInputRequestTypeDef",
     {
         "idMappingTechniques": IdMappingTechniquesTypeDef,
         "inputSourceConfig": Sequence[IdMappingWorkflowInputSourceTypeDef],
-        "outputSourceConfig": Sequence[IdMappingWorkflowOutputSourceTypeDef],
         "roleArn": str,
         "workflowName": str,
         "description": NotRequired[str],
+        "outputSourceConfig": NotRequired[Sequence[IdMappingWorkflowOutputSourceTypeDef]],
         "tags": NotRequired[Mapping[str, str]],
     },
 )
 CreateIdMappingWorkflowOutputTypeDef = TypedDict(
     "CreateIdMappingWorkflowOutputTypeDef",
     {
         "description": str,
@@ -744,18 +1035,18 @@
     },
 )
 UpdateIdMappingWorkflowInputRequestTypeDef = TypedDict(
     "UpdateIdMappingWorkflowInputRequestTypeDef",
     {
         "idMappingTechniques": IdMappingTechniquesTypeDef,
         "inputSourceConfig": Sequence[IdMappingWorkflowInputSourceTypeDef],
-        "outputSourceConfig": Sequence[IdMappingWorkflowOutputSourceTypeDef],
         "roleArn": str,
         "workflowName": str,
         "description": NotRequired[str],
+        "outputSourceConfig": NotRequired[Sequence[IdMappingWorkflowOutputSourceTypeDef]],
     },
 )
 UpdateIdMappingWorkflowOutputTypeDef = TypedDict(
     "UpdateIdMappingWorkflowOutputTypeDef",
     {
         "description": str,
         "idMappingTechniques": IdMappingTechniquesTypeDef,
```

### Comparing `mypy-boto3-entityresolution-1.34.0/mypy_boto3_entityresolution.egg-info/PKG-INFO` & `mypy_boto3_entityresolution-1.34.85/mypy_boto3_entityresolution.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-entityresolution
-Version: 1.34.0
-Summary: Type annotations for boto3.EntityResolution 1.34.0 service generated with mypy-boto3-builder 7.21.0
+Version: 1.34.85
+Summary: Type annotations for boto3.EntityResolution 1.34.85 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -13,50 +13,50 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Classifier: Typing :: Stubs Only
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: typing-extensions>=4.1.0; python_version < "3.12"
 
 <a id="mypy-boto3-entityresolution"></a>
 
 # mypy-boto3-entityresolution
 
 [![PyPI - mypy-boto3-entityresolution](https://img.shields.io/pypi/v/mypy-boto3-entityresolution.svg?color=blue)](https://pypi.org/project/mypy-boto3-entityresolution)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-entityresolution.svg?color=blue)](https://pypi.org/project/mypy-boto3-entityresolution)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-entityresolution)](https://pepy.tech/project/mypy-boto3-entityresolution)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EntityResolution 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution)
+[boto3.EntityResolution 1.34.85](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-entityresolution docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/).
 
 See how it helps to find and fix potential bugs:
 
@@ -284,14 +284,15 @@
 ```python
 from boto3.session import Session
 
 from mypy_boto3_entityresolution import EntityResolutionClient
 from mypy_boto3_entityresolution.paginator import (
     ListIdMappingJobsPaginator,
     ListIdMappingWorkflowsPaginator,
+    ListIdNamespacesPaginator,
     ListMatchingJobsPaginator,
     ListMatchingWorkflowsPaginator,
     ListProviderServicesPaginator,
     ListSchemaMappingsPaginator,
 )
 
 client: EntityResolutionClient = Session().client("entityresolution")
@@ -300,14 +301,15 @@
 # Types should be correctly discovered by mypy and IDEs
 list_id_mapping_jobs_paginator: ListIdMappingJobsPaginator = client.get_paginator(
     "list_id_mapping_jobs"
 )
 list_id_mapping_workflows_paginator: ListIdMappingWorkflowsPaginator = client.get_paginator(
     "list_id_mapping_workflows"
 )
+list_id_namespaces_paginator: ListIdNamespacesPaginator = client.get_paginator("list_id_namespaces")
 list_matching_jobs_paginator: ListMatchingJobsPaginator = client.get_paginator("list_matching_jobs")
 list_matching_workflows_paginator: ListMatchingWorkflowsPaginator = client.get_paginator(
     "list_matching_workflows"
 )
 list_provider_services_paginator: ListProviderServicesPaginator = client.get_paginator(
     "list_provider_services"
 )
@@ -340,18 +342,18 @@
 `mypy_boto3_entityresolution.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
 Full list of `EntityResolution` TypeDefs can be found in
 [docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/type_defs/).
 
 ```python
-from mypy_boto3_entityresolution.type_defs import IdMappingWorkflowInputSourceTypeDef
+from mypy_boto3_entityresolution.type_defs import AddPolicyStatementInputRequestTypeDef
 
 
-def get_value() -> IdMappingWorkflowInputSourceTypeDef:
+def get_value() -> AddPolicyStatementInputRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-entityresolution-1.34.0/mypy_boto3_entityresolution.egg-info/SOURCES.txt` & `mypy_boto3_entityresolution-1.34.85/mypy_boto3_entityresolution.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-entityresolution-1.34.0/setup.py` & `mypy_boto3_entityresolution-1.34.85/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,48 +7,44 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-entityresolution",
-    version="1.34.0",
+    version="1.34.85",
     packages=["mypy_boto3_entityresolution"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description=(
-        "Type annotations for boto3.EntityResolution 1.34.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
-    ),
+    description="Type annotations for boto3.EntityResolution 1.34.85 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3.13",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
-        "Typing :: Typed",
+        "Typing :: Stubs Only",
     ],
     keywords="boto3 entityresolution type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_entityresolution": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

