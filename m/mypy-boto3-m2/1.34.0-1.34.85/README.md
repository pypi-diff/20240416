# Comparing `tmp/mypy-boto3-m2-1.34.0.tar.gz` & `tmp/mypy_boto3_m2-1.34.85.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-m2-1.34.0.tar", last modified: Wed Dec 13 21:23:09 2023, max compression
+gzip compressed data, was "mypy_boto3_m2-1.34.85.tar", last modified: Tue Apr 16 19:33:16 2024, max compression
```

## Comparing `mypy-boto3-m2-1.34.0.tar` & `mypy_boto3_m2-1.34.85.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:23:09.803276 mypy-boto3-m2-1.34.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 21:13:26.000000 mypy-boto3-m2-1.34.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13820 2023-12-13 21:23:09.803276 mypy-boto3-m2-1.34.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12287 2023-12-13 21:13:26.000000 mypy-boto3-m2-1.34.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:23:09.803276 mypy-boto3-m2-1.34.0/mypy_boto3_m2/
--rw-r--r--   0 runner    (1001) docker     (127)     2461 2023-12-13 21:13:26.000000 mypy-boto3-m2-1.34.0/mypy_boto3_m2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2460 2023-12-13 21:13:26.000000 mypy-boto3-m2-1.34.0/mypy_boto3_m2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      925 2023-12-13 21:13:26.000000 mypy-boto3-m2-1.34.0/mypy_boto3_m2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28137 2023-12-13 21:13:26.000000 mypy-boto3-m2-1.34.0/mypy_boto3_m2/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    28133 2023-12-13 21:13:26.000000 mypy-boto3-m2-1.34.0/mypy_boto3_m2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10941 2023-12-13 21:13:26.000000 mypy-boto3-m2-1.34.0/mypy_boto3_m2/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10939 2023-12-13 21:13:26.000000 mypy-boto3-m2-1.34.0/mypy_boto3_m2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11373 2023-12-13 21:13:26.000000 mypy-boto3-m2-1.34.0/mypy_boto3_m2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    11362 2023-12-13 21:13:26.000000 mypy-boto3-m2-1.34.0/mypy_boto3_m2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 21:13:26.000000 mypy-boto3-m2-1.34.0/mypy_boto3_m2/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    33865 2023-12-13 21:13:28.000000 mypy-boto3-m2-1.34.0/mypy_boto3_m2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    33864 2023-12-13 21:13:26.000000 mypy-boto3-m2-1.34.0/mypy_boto3_m2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-12-13 21:13:26.000000 mypy-boto3-m2-1.34.0/mypy_boto3_m2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:23:09.803276 mypy-boto3-m2-1.34.0/mypy_boto3_m2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13820 2023-12-13 21:23:09.000000 mypy-boto3-m2-1.34.0/mypy_boto3_m2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      585 2023-12-13 21:23:09.000000 mypy-boto3-m2-1.34.0/mypy_boto3_m2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:23:09.000000 mypy-boto3-m2-1.34.0/mypy_boto3_m2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:23:09.000000 mypy-boto3-m2-1.34.0/mypy_boto3_m2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 21:23:09.000000 mypy-boto3-m2-1.34.0/mypy_boto3_m2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2023-12-13 21:23:09.000000 mypy-boto3-m2-1.34.0/mypy_boto3_m2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 21:23:09.803276 mypy-boto3-m2-1.34.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2028 2023-12-13 21:13:26.000000 mypy-boto3-m2-1.34.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:33:16.140323 mypy_boto3_m2-1.34.85/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-16 19:32:57.000000 mypy_boto3_m2-1.34.85/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13843 2024-04-16 19:33:16.140323 mypy_boto3_m2-1.34.85/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12288 2024-04-16 19:32:57.000000 mypy_boto3_m2-1.34.85/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:33:16.140323 mypy_boto3_m2-1.34.85/mypy_boto3_m2/
+-rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-04-16 19:32:57.000000 mypy_boto3_m2-1.34.85/mypy_boto3_m2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-04-16 19:32:57.000000 mypy_boto3_m2-1.34.85/mypy_boto3_m2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-16 19:32:57.000000 mypy_boto3_m2-1.34.85/mypy_boto3_m2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28749 2024-04-16 19:32:57.000000 mypy_boto3_m2-1.34.85/mypy_boto3_m2/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28746 2024-04-16 19:32:57.000000 mypy_boto3_m2-1.34.85/mypy_boto3_m2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11226 2024-04-16 19:32:57.000000 mypy_boto3_m2-1.34.85/mypy_boto3_m2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11226 2024-04-16 19:32:57.000000 mypy_boto3_m2-1.34.85/mypy_boto3_m2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11377 2024-04-16 19:32:57.000000 mypy_boto3_m2-1.34.85/mypy_boto3_m2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11367 2024-04-16 19:32:57.000000 mypy_boto3_m2-1.34.85/mypy_boto3_m2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 19:32:57.000000 mypy_boto3_m2-1.34.85/mypy_boto3_m2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    35366 2024-04-16 19:32:58.000000 mypy_boto3_m2-1.34.85/mypy_boto3_m2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35366 2024-04-16 19:32:58.000000 mypy_boto3_m2-1.34.85/mypy_boto3_m2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-16 19:32:57.000000 mypy_boto3_m2-1.34.85/mypy_boto3_m2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:33:16.140323 mypy_boto3_m2-1.34.85/mypy_boto3_m2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13843 2024-04-16 19:33:16.000000 mypy_boto3_m2-1.34.85/mypy_boto3_m2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-16 19:33:16.000000 mypy_boto3_m2-1.34.85/mypy_boto3_m2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 19:33:16.000000 mypy_boto3_m2-1.34.85/mypy_boto3_m2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 19:33:16.000000 mypy_boto3_m2-1.34.85/mypy_boto3_m2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-16 19:33:16.000000 mypy_boto3_m2-1.34.85/mypy_boto3_m2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-16 19:33:16.000000 mypy_boto3_m2-1.34.85/mypy_boto3_m2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 19:33:16.140323 mypy_boto3_m2-1.34.85/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-16 19:32:57.000000 mypy_boto3_m2-1.34.85/setup.py
```

### Comparing `mypy-boto3-m2-1.34.0/LICENSE` & `mypy_boto3_m2-1.34.85/LICENSE`

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

### Comparing `mypy-boto3-m2-1.34.0/PKG-INFO` & `mypy_boto3_m2-1.34.85/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-m2
-Version: 1.34.0
-Summary: Type annotations for boto3.MainframeModernization 1.34.0 service generated with mypy-boto3-builder 7.21.0
+Version: 1.34.85
+Summary: Type annotations for boto3.MainframeModernization 1.34.85 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/
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
 
 <a id="mypy-boto3-m2"></a>
 
 # mypy-boto3-m2
 
 [![PyPI - mypy-boto3-m2](https://img.shields.io/pypi/v/mypy-boto3-m2.svg?color=blue)](https://pypi.org/project/mypy-boto3-m2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-m2.svg?color=blue)](https://pypi.org/project/mypy-boto3-m2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-m2)](https://pepy.tech/project/mypy-boto3-m2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MainframeModernization 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization)
+[boto3.MainframeModernization 1.34.85](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization)
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
 [mypy-boto3-m2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-m2-1.34.0/README.md` & `mypy_boto3_m2-1.34.85/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-m2.svg?color=blue)](https://pypi.org/project/mypy-boto3-m2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-m2)](https://pepy.tech/project/mypy-boto3-m2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MainframeModernization 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization)
+[boto3.MainframeModernization 1.34.85](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization)
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
 [mypy-boto3-m2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-m2-1.34.0/mypy_boto3_m2/__init__.py` & `mypy_boto3_m2-1.34.85/mypy_boto3_m2/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,14 @@
     ListDeploymentsPaginator,
     ListEngineVersionsPaginator,
     ListEnvironmentsPaginator,
 )
 
 Client = MainframeModernizationClient
 
-
 __all__ = (
     "Client",
     "ListApplicationVersionsPaginator",
     "ListApplicationsPaginator",
     "ListBatchJobDefinitionsPaginator",
     "ListBatchJobExecutionsPaginator",
     "ListDataSetImportHistoryPaginator",
```

### Comparing `mypy-boto3-m2-1.34.0/mypy_boto3_m2/__init__.pyi` & `mypy_boto3_m2-1.34.85/mypy_boto3_m2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-m2-1.34.0/mypy_boto3_m2/__main__.py` & `mypy_boto3_m2-1.34.85/mypy_boto3_m2/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,28 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MainframeModernization 1.34.0\nVersion:         1.34.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
-        " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2//\nBoto3 docs:     "
-        " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization\nOther"
-        " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
-        " https://github.com/youtype/mypy_boto3_builder/releases"
+        "Type annotations for boto3.MainframeModernization 1.34.85\n"
+        "Version:         1.34.85\n"
+        "Builder version: 7.23.2\n"
+        "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2//\n"
+        "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization\n"
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

### Comparing `mypy-boto3-m2-1.34.0/mypy_boto3_m2/client.py` & `mypy_boto3_m2-1.34.85/mypy_boto3_m2/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,15 @@
     GetEnvironmentResponseTypeDef,
     GetSignedBluinsightsUrlResponseTypeDef,
     HighAvailabilityConfigTypeDef,
     ListApplicationsResponseTypeDef,
     ListApplicationVersionsResponseTypeDef,
     ListBatchJobDefinitionsResponseTypeDef,
     ListBatchJobExecutionsResponseTypeDef,
+    ListBatchJobRestartPointsResponseTypeDef,
     ListDataSetImportHistoryResponseTypeDef,
     ListDataSetsResponseTypeDef,
     ListDeploymentsResponseTypeDef,
     ListEngineVersionsResponseTypeDef,
     ListEnvironmentsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     StartBatchJobResponseTypeDef,
@@ -66,39 +67,35 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("MainframeModernizationClient",)
 
-
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     ExecutionTimeoutException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
     ServiceUnavailableException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
-
 class MainframeModernizationClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/client/)
     """
 
     meta: ClientMeta
@@ -142,44 +139,44 @@
         definition: DefinitionTypeDef,
         engineType: EngineTypeType,
         name: str,
         clientToken: str = ...,
         description: str = ...,
         kmsKeyId: str = ...,
         roleArn: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateApplicationResponseTypeDef:
         """
         Creates a new application with given parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.create_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/client/#create_application)
         """
 
     def create_data_set_import_task(
         self,
         *,
         applicationId: str,
         importConfig: DataSetImportConfigTypeDef,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> CreateDataSetImportTaskResponseTypeDef:
         """
         Starts a data set import task for a specific application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.create_data_set_import_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/client/#create_data_set_import_task)
         """
 
     def create_deployment(
         self,
         *,
         applicationId: str,
         applicationVersion: int,
         environmentId: str,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> CreateDeploymentResponseTypeDef:
         """
         Creates and starts a deployment to deploy an application into a runtime
         environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.create_deployment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/client/#create_deployment)
@@ -197,15 +194,15 @@
         highAvailabilityConfig: HighAvailabilityConfigTypeDef = ...,
         kmsKeyId: str = ...,
         preferredMaintenanceWindow: str = ...,
         publiclyAccessible: bool = ...,
         securityGroupIds: Sequence[str] = ...,
         storageConfigurations: Sequence[StorageConfigurationTypeDef] = ...,
         subnetIds: Sequence[str] = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateEnvironmentResponseTypeDef:
         """
         Creates a runtime environment for a given runtime engine.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.create_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/client/#create_environment)
         """
@@ -340,15 +337,15 @@
 
     def list_applications(
         self,
         *,
         environmentId: str = ...,
         maxResults: int = ...,
         names: Sequence[str] = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListApplicationsResponseTypeDef:
         """
         Lists the applications associated with a specific Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.list_applications)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/client/#list_applications)
         """
@@ -371,24 +368,34 @@
         applicationId: str,
         executionIds: Sequence[str] = ...,
         jobName: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         startedAfter: TimestampTypeDef = ...,
         startedBefore: TimestampTypeDef = ...,
-        status: BatchJobExecutionStatusType = ...
+        status: BatchJobExecutionStatusType = ...,
     ) -> ListBatchJobExecutionsResponseTypeDef:
         """
         Lists historical, current, and scheduled batch job executions for a specific
         application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.list_batch_job_executions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/client/#list_batch_job_executions)
         """
 
+    def list_batch_job_restart_points(
+        self, *, applicationId: str, executionId: str
+    ) -> ListBatchJobRestartPointsResponseTypeDef:
+        """
+        Lists all the job steps for JCL files to restart a batch job.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.list_batch_job_restart_points)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/client/#list_batch_job_restart_points)
+        """
+
     def list_data_set_import_history(
         self, *, applicationId: str, maxResults: int = ..., nextToken: str = ...
     ) -> ListDataSetImportHistoryResponseTypeDef:
         """
         Lists the data set imports for the specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.list_data_set_import_history)
@@ -398,15 +405,15 @@
     def list_data_sets(
         self,
         *,
         applicationId: str,
         maxResults: int = ...,
         nameFilter: str = ...,
         nextToken: str = ...,
-        prefix: str = ...
+        prefix: str = ...,
     ) -> ListDataSetsResponseTypeDef:
         """
         Lists the data sets imported for a specific application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.list_data_sets)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/client/#list_data_sets)
         """
@@ -433,15 +440,15 @@
 
     def list_environments(
         self,
         *,
         engineType: EngineTypeType = ...,
         maxResults: int = ...,
         names: Sequence[str] = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListEnvironmentsResponseTypeDef:
         """
         Lists the runtime environments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.list_environments)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/client/#list_environments)
         """
@@ -463,15 +470,15 @@
         """
 
     def start_batch_job(
         self,
         *,
         applicationId: str,
         batchJobIdentifier: BatchJobIdentifierTypeDef,
-        jobParams: Mapping[str, str] = ...
+        jobParams: Mapping[str, str] = ...,
     ) -> StartBatchJobResponseTypeDef:
         """
         Starts a batch job and returns the unique identifier of this execution of the
         batch
         job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.start_batch_job)
@@ -504,15 +511,15 @@
 
     def update_application(
         self,
         *,
         applicationId: str,
         currentApplicationVersion: int,
         definition: DefinitionTypeDef = ...,
-        description: str = ...
+        description: str = ...,
     ) -> UpdateApplicationResponseTypeDef:
         """
         Updates an application and creates a new version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.update_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/client/#update_application)
         """
@@ -522,15 +529,15 @@
         *,
         environmentId: str,
         applyDuringMaintenanceWindow: bool = ...,
         desiredCapacity: int = ...,
         engineVersion: str = ...,
         forceUpdate: bool = ...,
         instanceType: str = ...,
-        preferredMaintenanceWindow: str = ...
+        preferredMaintenanceWindow: str = ...,
     ) -> UpdateEnvironmentResponseTypeDef:
         """
         Updates the configuration details for a specific runtime environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.update_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/client/#update_environment)
         """
```

### Comparing `mypy-boto3-m2-1.34.0/mypy_boto3_m2/client.pyi` & `mypy_boto3_m2-1.34.85/mypy_boto3_m2/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,15 @@
     GetEnvironmentResponseTypeDef,
     GetSignedBluinsightsUrlResponseTypeDef,
     HighAvailabilityConfigTypeDef,
     ListApplicationsResponseTypeDef,
     ListApplicationVersionsResponseTypeDef,
     ListBatchJobDefinitionsResponseTypeDef,
     ListBatchJobExecutionsResponseTypeDef,
+    ListBatchJobRestartPointsResponseTypeDef,
     ListDataSetImportHistoryResponseTypeDef,
     ListDataSetsResponseTypeDef,
     ListDeploymentsResponseTypeDef,
     ListEngineVersionsResponseTypeDef,
     ListEnvironmentsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     StartBatchJobResponseTypeDef,
@@ -68,33 +69,36 @@
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = ("MainframeModernizationClient",)
 
+
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     ExecutionTimeoutException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
     ServiceUnavailableException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
+
 class MainframeModernizationClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/client/)
     """
 
     meta: ClientMeta
@@ -138,44 +142,44 @@
         definition: DefinitionTypeDef,
         engineType: EngineTypeType,
         name: str,
         clientToken: str = ...,
         description: str = ...,
         kmsKeyId: str = ...,
         roleArn: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateApplicationResponseTypeDef:
         """
         Creates a new application with given parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.create_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/client/#create_application)
         """
 
     def create_data_set_import_task(
         self,
         *,
         applicationId: str,
         importConfig: DataSetImportConfigTypeDef,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> CreateDataSetImportTaskResponseTypeDef:
         """
         Starts a data set import task for a specific application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.create_data_set_import_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/client/#create_data_set_import_task)
         """
 
     def create_deployment(
         self,
         *,
         applicationId: str,
         applicationVersion: int,
         environmentId: str,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> CreateDeploymentResponseTypeDef:
         """
         Creates and starts a deployment to deploy an application into a runtime
         environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.create_deployment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/client/#create_deployment)
@@ -193,15 +197,15 @@
         highAvailabilityConfig: HighAvailabilityConfigTypeDef = ...,
         kmsKeyId: str = ...,
         preferredMaintenanceWindow: str = ...,
         publiclyAccessible: bool = ...,
         securityGroupIds: Sequence[str] = ...,
         storageConfigurations: Sequence[StorageConfigurationTypeDef] = ...,
         subnetIds: Sequence[str] = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateEnvironmentResponseTypeDef:
         """
         Creates a runtime environment for a given runtime engine.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.create_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/client/#create_environment)
         """
@@ -336,15 +340,15 @@
 
     def list_applications(
         self,
         *,
         environmentId: str = ...,
         maxResults: int = ...,
         names: Sequence[str] = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListApplicationsResponseTypeDef:
         """
         Lists the applications associated with a specific Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.list_applications)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/client/#list_applications)
         """
@@ -367,24 +371,34 @@
         applicationId: str,
         executionIds: Sequence[str] = ...,
         jobName: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         startedAfter: TimestampTypeDef = ...,
         startedBefore: TimestampTypeDef = ...,
-        status: BatchJobExecutionStatusType = ...
+        status: BatchJobExecutionStatusType = ...,
     ) -> ListBatchJobExecutionsResponseTypeDef:
         """
         Lists historical, current, and scheduled batch job executions for a specific
         application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.list_batch_job_executions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/client/#list_batch_job_executions)
         """
 
+    def list_batch_job_restart_points(
+        self, *, applicationId: str, executionId: str
+    ) -> ListBatchJobRestartPointsResponseTypeDef:
+        """
+        Lists all the job steps for JCL files to restart a batch job.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.list_batch_job_restart_points)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/client/#list_batch_job_restart_points)
+        """
+
     def list_data_set_import_history(
         self, *, applicationId: str, maxResults: int = ..., nextToken: str = ...
     ) -> ListDataSetImportHistoryResponseTypeDef:
         """
         Lists the data set imports for the specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.list_data_set_import_history)
@@ -394,15 +408,15 @@
     def list_data_sets(
         self,
         *,
         applicationId: str,
         maxResults: int = ...,
         nameFilter: str = ...,
         nextToken: str = ...,
-        prefix: str = ...
+        prefix: str = ...,
     ) -> ListDataSetsResponseTypeDef:
         """
         Lists the data sets imported for a specific application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.list_data_sets)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/client/#list_data_sets)
         """
@@ -429,15 +443,15 @@
 
     def list_environments(
         self,
         *,
         engineType: EngineTypeType = ...,
         maxResults: int = ...,
         names: Sequence[str] = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListEnvironmentsResponseTypeDef:
         """
         Lists the runtime environments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.list_environments)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/client/#list_environments)
         """
@@ -459,15 +473,15 @@
         """
 
     def start_batch_job(
         self,
         *,
         applicationId: str,
         batchJobIdentifier: BatchJobIdentifierTypeDef,
-        jobParams: Mapping[str, str] = ...
+        jobParams: Mapping[str, str] = ...,
     ) -> StartBatchJobResponseTypeDef:
         """
         Starts a batch job and returns the unique identifier of this execution of the
         batch
         job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.start_batch_job)
@@ -500,15 +514,15 @@
 
     def update_application(
         self,
         *,
         applicationId: str,
         currentApplicationVersion: int,
         definition: DefinitionTypeDef = ...,
-        description: str = ...
+        description: str = ...,
     ) -> UpdateApplicationResponseTypeDef:
         """
         Updates an application and creates a new version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.update_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/client/#update_application)
         """
@@ -518,15 +532,15 @@
         *,
         environmentId: str,
         applyDuringMaintenanceWindow: bool = ...,
         desiredCapacity: int = ...,
         engineVersion: str = ...,
         forceUpdate: bool = ...,
         instanceType: str = ...,
-        preferredMaintenanceWindow: str = ...
+        preferredMaintenanceWindow: str = ...,
     ) -> UpdateEnvironmentResponseTypeDef:
         """
         Updates the configuration details for a specific runtime environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.update_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/client/#update_environment)
         """
```

### Comparing `mypy-boto3-m2-1.34.0/mypy_boto3_m2/literals.py` & `mypy_boto3_m2-1.34.85/mypy_boto3_m2/literals.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ApplicationDeploymentLifecycleType",
     "ApplicationLifecycleType",
     "ApplicationVersionLifecycleType",
     "BatchJobExecutionStatusType",
     "BatchJobTypeType",
     "DataSetTaskLifecycleType",
@@ -42,15 +41,14 @@
     "MainframeModernizationServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ApplicationDeploymentLifecycleType = Literal["Deployed", "Deploying"]
 ApplicationLifecycleType = Literal[
     "Available",
     "Created",
     "Creating",
     "Deleting",
     "Deleting From Environment",
@@ -64,14 +62,15 @@
 ApplicationVersionLifecycleType = Literal["Available", "Creating", "Failed"]
 BatchJobExecutionStatusType = Literal[
     "Cancelled",
     "Cancelling",
     "Dispatching",
     "Failed",
     "Holding",
+    "Purged",
     "Running",
     "Submitting",
     "Succeeded",
     "Succeeded With Warning",
 ]
 BatchJobTypeType = Literal["JES2", "JES3", "VSE"]
 DataSetTaskLifecycleType = Literal["Completed", "Creating", "Failed", "Running"]
@@ -110,14 +109,15 @@
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
@@ -128,14 +128,15 @@
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
@@ -153,14 +154,15 @@
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
@@ -173,24 +175,26 @@
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
@@ -251,15 +255,14 @@
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
@@ -331,17 +334,19 @@
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
@@ -431,19 +436,21 @@
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
@@ -484,23 +491,29 @@
     "list_data_set_import_history",
     "list_data_sets",
     "list_deployments",
     "list_engine_versions",
     "list_environments",
 ]
 RegionName = Literal[
+    "af-south-1",
     "ap-northeast-1",
     "ap-northeast-2",
+    "ap-northeast-3",
     "ap-south-1",
     "ap-southeast-1",
     "ap-southeast-2",
     "ca-central-1",
     "eu-central-1",
+    "eu-north-1",
+    "eu-south-1",
+    "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "il-central-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
 ]
```

### Comparing `mypy-boto3-m2-1.34.0/mypy_boto3_m2/literals.pyi` & `mypy_boto3_m2-1.34.85/mypy_boto3_m2/literals.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -62,14 +62,15 @@
 ApplicationVersionLifecycleType = Literal["Available", "Creating", "Failed"]
 BatchJobExecutionStatusType = Literal[
     "Cancelled",
     "Cancelling",
     "Dispatching",
     "Failed",
     "Holding",
+    "Purged",
     "Running",
     "Submitting",
     "Succeeded",
     "Succeeded With Warning",
 ]
 BatchJobTypeType = Literal["JES2", "JES3", "VSE"]
 DataSetTaskLifecycleType = Literal["Completed", "Creating", "Failed", "Running"]
@@ -108,14 +109,15 @@
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
@@ -126,14 +128,15 @@
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
@@ -151,14 +154,15 @@
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
@@ -171,24 +175,26 @@
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
@@ -249,15 +255,14 @@
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
@@ -329,17 +334,19 @@
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
@@ -429,19 +436,21 @@
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
@@ -482,23 +491,29 @@
     "list_data_set_import_history",
     "list_data_sets",
     "list_deployments",
     "list_engine_versions",
     "list_environments",
 ]
 RegionName = Literal[
+    "af-south-1",
     "ap-northeast-1",
     "ap-northeast-2",
+    "ap-northeast-3",
     "ap-south-1",
     "ap-southeast-1",
     "ap-southeast-2",
     "ca-central-1",
     "eu-central-1",
+    "eu-north-1",
+    "eu-south-1",
+    "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "il-central-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
 ]
```

### Comparing `mypy-boto3-m2-1.34.0/mypy_boto3_m2/paginator.py` & `mypy_boto3_m2-1.34.85/mypy_boto3_m2/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,14 @@
     "ListDataSetImportHistoryPaginator",
     "ListDataSetsPaginator",
     "ListDeploymentsPaginator",
     "ListEngineVersionsPaginator",
     "ListEnvironmentsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -100,15 +99,15 @@
     """
 
     def paginate(
         self,
         *,
         environmentId: str = ...,
         names: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListApplications.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/paginators/#listapplicationspaginator)
         """
 
 
@@ -119,15 +118,15 @@
     """
 
     def paginate(
         self,
         *,
         applicationId: str,
         prefix: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListBatchJobDefinitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListBatchJobDefinitions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/paginators/#listbatchjobdefinitionspaginator)
         """
 
 
@@ -142,15 +141,15 @@
         *,
         applicationId: str,
         executionIds: Sequence[str] = ...,
         jobName: str = ...,
         startedAfter: TimestampTypeDef = ...,
         startedBefore: TimestampTypeDef = ...,
         status: BatchJobExecutionStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListBatchJobExecutionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListBatchJobExecutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/paginators/#listbatchjobexecutionspaginator)
         """
 
 
@@ -177,15 +176,15 @@
 
     def paginate(
         self,
         *,
         applicationId: str,
         nameFilter: str = ...,
         prefix: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListDataSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListDataSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/paginators/#listdatasetspaginator)
         """
 
 
@@ -226,13 +225,13 @@
     """
 
     def paginate(
         self,
         *,
         engineType: EngineTypeType = ...,
         names: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListEnvironmentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListEnvironments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/paginators/#listenvironmentspaginator)
         """
```

### Comparing `mypy-boto3-m2-1.34.0/mypy_boto3_m2/paginator.pyi` & `mypy_boto3_m2-1.34.85/mypy_boto3_m2/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
     """
 
     def paginate(
         self,
         *,
         environmentId: str = ...,
         names: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListApplications.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/paginators/#listapplicationspaginator)
         """
 
 class ListBatchJobDefinitionsPaginator(Paginator):
@@ -114,15 +114,15 @@
     """
 
     def paginate(
         self,
         *,
         applicationId: str,
         prefix: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListBatchJobDefinitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListBatchJobDefinitions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/paginators/#listbatchjobdefinitionspaginator)
         """
 
 class ListBatchJobExecutionsPaginator(Paginator):
@@ -136,15 +136,15 @@
         *,
         applicationId: str,
         executionIds: Sequence[str] = ...,
         jobName: str = ...,
         startedAfter: TimestampTypeDef = ...,
         startedBefore: TimestampTypeDef = ...,
         status: BatchJobExecutionStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListBatchJobExecutionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListBatchJobExecutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/paginators/#listbatchjobexecutionspaginator)
         """
 
 class ListDataSetImportHistoryPaginator(Paginator):
@@ -169,15 +169,15 @@
 
     def paginate(
         self,
         *,
         applicationId: str,
         nameFilter: str = ...,
         prefix: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListDataSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListDataSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/paginators/#listdatasetspaginator)
         """
 
 class ListDeploymentsPaginator(Paginator):
@@ -215,13 +215,13 @@
     """
 
     def paginate(
         self,
         *,
         engineType: EngineTypeType = ...,
         names: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListEnvironmentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListEnvironments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/paginators/#listenvironmentspaginator)
         """
```

### Comparing `mypy-boto3-m2-1.34.0/mypy_boto3_m2/type_defs.py` & `mypy_boto3_m2-1.34.85/mypy_boto3_m2/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AlternateKeyTypeDef",
     "ApplicationSummaryTypeDef",
     "ApplicationVersionSummaryTypeDef",
     "FileBatchJobDefinitionTypeDef",
     "ScriptBatchJobDefinitionTypeDef",
     "FileBatchJobIdentifierTypeDef",
@@ -70,24 +69,27 @@
     "EngineVersionsSummaryTypeDef",
     "EnvironmentSummaryTypeDef",
     "FsxStorageConfigurationTypeDef",
     "GetApplicationRequestRequestTypeDef",
     "LogGroupSummaryTypeDef",
     "GetApplicationVersionRequestRequestTypeDef",
     "GetBatchJobExecutionRequestRequestTypeDef",
+    "JobStepRestartMarkerTypeDef",
     "GetDataSetDetailsRequestRequestTypeDef",
     "GetDataSetImportTaskRequestRequestTypeDef",
     "GetDeploymentRequestRequestTypeDef",
     "GetEnvironmentRequestRequestTypeDef",
     "JobIdentifierTypeDef",
+    "JobStepTypeDef",
     "PaginatorConfigTypeDef",
     "ListApplicationVersionsRequestRequestTypeDef",
     "ListApplicationsRequestRequestTypeDef",
     "ListBatchJobDefinitionsRequestRequestTypeDef",
     "TimestampTypeDef",
+    "ListBatchJobRestartPointsRequestRequestTypeDef",
     "ListDataSetImportHistoryRequestRequestTypeDef",
     "ListDataSetsRequestRequestTypeDef",
     "ListDeploymentsRequestRequestTypeDef",
     "ListEngineVersionsRequestRequestTypeDef",
     "ListEnvironmentsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "MaintenanceScheduleTypeDef",
@@ -117,15 +119,17 @@
     "GetDataSetImportTaskResponseTypeDef",
     "ListDataSetsResponseTypeDef",
     "ListDeploymentsResponseTypeDef",
     "ListEngineVersionsResponseTypeDef",
     "ListEnvironmentsResponseTypeDef",
     "StorageConfigurationTypeDef",
     "GetApplicationResponseTypeDef",
+    "RestartBatchJobIdentifierTypeDef",
     "S3BatchJobIdentifierTypeDef",
+    "ListBatchJobRestartPointsResponseTypeDef",
     "ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
     "ListApplicationsRequestListApplicationsPaginateTypeDef",
     "ListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef",
     "ListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef",
     "ListDataSetsRequestListDataSetsPaginateTypeDef",
     "ListDeploymentsRequestListDeploymentsPaginateTypeDef",
     "ListEngineVersionsRequestListEngineVersionsPaginateTypeDef",
@@ -229,18 +233,18 @@
         "s3Location": NotRequired[str],
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
-        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
+        "HostId": NotRequired[str],
     },
 )
 CreateDeploymentRequestRequestTypeDef = TypedDict(
     "CreateDeploymentRequestRequestTypeDef",
     {
         "applicationId": str,
         "applicationVersion": int,
@@ -427,14 +431,23 @@
 GetBatchJobExecutionRequestRequestTypeDef = TypedDict(
     "GetBatchJobExecutionRequestRequestTypeDef",
     {
         "applicationId": str,
         "executionId": str,
     },
 )
+JobStepRestartMarkerTypeDef = TypedDict(
+    "JobStepRestartMarkerTypeDef",
+    {
+        "fromStep": str,
+        "fromProcStep": NotRequired[str],
+        "toProcStep": NotRequired[str],
+        "toStep": NotRequired[str],
+    },
+)
 GetDataSetDetailsRequestRequestTypeDef = TypedDict(
     "GetDataSetDetailsRequestRequestTypeDef",
     {
         "applicationId": str,
         "dataSetName": str,
     },
 )
@@ -461,14 +474,25 @@
 JobIdentifierTypeDef = TypedDict(
     "JobIdentifierTypeDef",
     {
         "fileName": NotRequired[str],
         "scriptName": NotRequired[str],
     },
 )
+JobStepTypeDef = TypedDict(
+    "JobStepTypeDef",
+    {
+        "procStepName": NotRequired[str],
+        "procStepNumber": NotRequired[int],
+        "stepCondCode": NotRequired[str],
+        "stepName": NotRequired[str],
+        "stepNumber": NotRequired[int],
+        "stepRestartable": NotRequired[bool],
+    },
+)
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": NotRequired[int],
         "PageSize": NotRequired[int],
         "StartingToken": NotRequired[str],
     },
@@ -496,14 +520,21 @@
         "applicationId": str,
         "maxResults": NotRequired[int],
         "nextToken": NotRequired[str],
         "prefix": NotRequired[str],
     },
 )
 TimestampTypeDef = Union[datetime, str]
+ListBatchJobRestartPointsRequestRequestTypeDef = TypedDict(
+    "ListBatchJobRestartPointsRequestRequestTypeDef",
+    {
+        "applicationId": str,
+        "executionId": str,
+    },
+)
 ListDataSetImportHistoryRequestRequestTypeDef = TypedDict(
     "ListDataSetImportHistoryRequestRequestTypeDef",
     {
         "applicationId": str,
         "maxResults": NotRequired[int],
         "nextToken": NotRequired[str],
     },
@@ -818,22 +849,36 @@
         "status": ApplicationLifecycleType,
         "statusReason": str,
         "tags": Dict[str, str],
         "targetGroupArns": List[str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+RestartBatchJobIdentifierTypeDef = TypedDict(
+    "RestartBatchJobIdentifierTypeDef",
+    {
+        "executionId": str,
+        "jobStepRestartMarker": JobStepRestartMarkerTypeDef,
+    },
+)
 S3BatchJobIdentifierTypeDef = TypedDict(
     "S3BatchJobIdentifierTypeDef",
     {
         "bucket": str,
         "identifier": JobIdentifierTypeDef,
         "keyPrefix": NotRequired[str],
     },
 )
+ListBatchJobRestartPointsResponseTypeDef = TypedDict(
+    "ListBatchJobRestartPointsResponseTypeDef",
+    {
+        "batchJobSteps": List[JobStepTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef = TypedDict(
     "ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
     {
         "applicationId": str,
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
@@ -979,14 +1024,15 @@
         "tags": NotRequired[Mapping[str, str]],
     },
 )
 BatchJobIdentifierTypeDef = TypedDict(
     "BatchJobIdentifierTypeDef",
     {
         "fileBatchJobIdentifier": NotRequired[FileBatchJobIdentifierTypeDef],
+        "restartBatchJobIdentifier": NotRequired[RestartBatchJobIdentifierTypeDef],
         "s3BatchJobIdentifier": NotRequired[S3BatchJobIdentifierTypeDef],
         "scriptBatchJobIdentifier": NotRequired[ScriptBatchJobIdentifierTypeDef],
     },
 )
 GetEnvironmentResponseTypeDef = TypedDict(
     "GetEnvironmentResponseTypeDef",
     {
@@ -1053,14 +1099,15 @@
     {
         "applicationId": str,
         "batchJobIdentifier": BatchJobIdentifierTypeDef,
         "endTime": datetime,
         "executionId": str,
         "jobId": str,
         "jobName": str,
+        "jobStepRestartMarker": JobStepRestartMarkerTypeDef,
         "jobType": BatchJobTypeType,
         "jobUser": str,
         "returnCode": str,
         "startTime": datetime,
         "status": BatchJobExecutionStatusType,
         "statusReason": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
```

### Comparing `mypy-boto3-m2-1.34.0/mypy_boto3_m2/type_defs.pyi` & `mypy_boto3_m2-1.34.85/mypy_boto3_m2/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -69,24 +69,27 @@
     "EngineVersionsSummaryTypeDef",
     "EnvironmentSummaryTypeDef",
     "FsxStorageConfigurationTypeDef",
     "GetApplicationRequestRequestTypeDef",
     "LogGroupSummaryTypeDef",
     "GetApplicationVersionRequestRequestTypeDef",
     "GetBatchJobExecutionRequestRequestTypeDef",
+    "JobStepRestartMarkerTypeDef",
     "GetDataSetDetailsRequestRequestTypeDef",
     "GetDataSetImportTaskRequestRequestTypeDef",
     "GetDeploymentRequestRequestTypeDef",
     "GetEnvironmentRequestRequestTypeDef",
     "JobIdentifierTypeDef",
+    "JobStepTypeDef",
     "PaginatorConfigTypeDef",
     "ListApplicationVersionsRequestRequestTypeDef",
     "ListApplicationsRequestRequestTypeDef",
     "ListBatchJobDefinitionsRequestRequestTypeDef",
     "TimestampTypeDef",
+    "ListBatchJobRestartPointsRequestRequestTypeDef",
     "ListDataSetImportHistoryRequestRequestTypeDef",
     "ListDataSetsRequestRequestTypeDef",
     "ListDeploymentsRequestRequestTypeDef",
     "ListEngineVersionsRequestRequestTypeDef",
     "ListEnvironmentsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "MaintenanceScheduleTypeDef",
@@ -116,15 +119,17 @@
     "GetDataSetImportTaskResponseTypeDef",
     "ListDataSetsResponseTypeDef",
     "ListDeploymentsResponseTypeDef",
     "ListEngineVersionsResponseTypeDef",
     "ListEnvironmentsResponseTypeDef",
     "StorageConfigurationTypeDef",
     "GetApplicationResponseTypeDef",
+    "RestartBatchJobIdentifierTypeDef",
     "S3BatchJobIdentifierTypeDef",
+    "ListBatchJobRestartPointsResponseTypeDef",
     "ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
     "ListApplicationsRequestListApplicationsPaginateTypeDef",
     "ListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef",
     "ListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef",
     "ListDataSetsRequestListDataSetsPaginateTypeDef",
     "ListDeploymentsRequestListDeploymentsPaginateTypeDef",
     "ListEngineVersionsRequestListEngineVersionsPaginateTypeDef",
@@ -228,18 +233,18 @@
         "s3Location": NotRequired[str],
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
-        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
+        "HostId": NotRequired[str],
     },
 )
 CreateDeploymentRequestRequestTypeDef = TypedDict(
     "CreateDeploymentRequestRequestTypeDef",
     {
         "applicationId": str,
         "applicationVersion": int,
@@ -426,14 +431,23 @@
 GetBatchJobExecutionRequestRequestTypeDef = TypedDict(
     "GetBatchJobExecutionRequestRequestTypeDef",
     {
         "applicationId": str,
         "executionId": str,
     },
 )
+JobStepRestartMarkerTypeDef = TypedDict(
+    "JobStepRestartMarkerTypeDef",
+    {
+        "fromStep": str,
+        "fromProcStep": NotRequired[str],
+        "toProcStep": NotRequired[str],
+        "toStep": NotRequired[str],
+    },
+)
 GetDataSetDetailsRequestRequestTypeDef = TypedDict(
     "GetDataSetDetailsRequestRequestTypeDef",
     {
         "applicationId": str,
         "dataSetName": str,
     },
 )
@@ -460,14 +474,25 @@
 JobIdentifierTypeDef = TypedDict(
     "JobIdentifierTypeDef",
     {
         "fileName": NotRequired[str],
         "scriptName": NotRequired[str],
     },
 )
+JobStepTypeDef = TypedDict(
+    "JobStepTypeDef",
+    {
+        "procStepName": NotRequired[str],
+        "procStepNumber": NotRequired[int],
+        "stepCondCode": NotRequired[str],
+        "stepName": NotRequired[str],
+        "stepNumber": NotRequired[int],
+        "stepRestartable": NotRequired[bool],
+    },
+)
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": NotRequired[int],
         "PageSize": NotRequired[int],
         "StartingToken": NotRequired[str],
     },
@@ -495,14 +520,21 @@
         "applicationId": str,
         "maxResults": NotRequired[int],
         "nextToken": NotRequired[str],
         "prefix": NotRequired[str],
     },
 )
 TimestampTypeDef = Union[datetime, str]
+ListBatchJobRestartPointsRequestRequestTypeDef = TypedDict(
+    "ListBatchJobRestartPointsRequestRequestTypeDef",
+    {
+        "applicationId": str,
+        "executionId": str,
+    },
+)
 ListDataSetImportHistoryRequestRequestTypeDef = TypedDict(
     "ListDataSetImportHistoryRequestRequestTypeDef",
     {
         "applicationId": str,
         "maxResults": NotRequired[int],
         "nextToken": NotRequired[str],
     },
@@ -817,22 +849,36 @@
         "status": ApplicationLifecycleType,
         "statusReason": str,
         "tags": Dict[str, str],
         "targetGroupArns": List[str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+RestartBatchJobIdentifierTypeDef = TypedDict(
+    "RestartBatchJobIdentifierTypeDef",
+    {
+        "executionId": str,
+        "jobStepRestartMarker": JobStepRestartMarkerTypeDef,
+    },
+)
 S3BatchJobIdentifierTypeDef = TypedDict(
     "S3BatchJobIdentifierTypeDef",
     {
         "bucket": str,
         "identifier": JobIdentifierTypeDef,
         "keyPrefix": NotRequired[str],
     },
 )
+ListBatchJobRestartPointsResponseTypeDef = TypedDict(
+    "ListBatchJobRestartPointsResponseTypeDef",
+    {
+        "batchJobSteps": List[JobStepTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef = TypedDict(
     "ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
     {
         "applicationId": str,
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
@@ -978,14 +1024,15 @@
         "tags": NotRequired[Mapping[str, str]],
     },
 )
 BatchJobIdentifierTypeDef = TypedDict(
     "BatchJobIdentifierTypeDef",
     {
         "fileBatchJobIdentifier": NotRequired[FileBatchJobIdentifierTypeDef],
+        "restartBatchJobIdentifier": NotRequired[RestartBatchJobIdentifierTypeDef],
         "s3BatchJobIdentifier": NotRequired[S3BatchJobIdentifierTypeDef],
         "scriptBatchJobIdentifier": NotRequired[ScriptBatchJobIdentifierTypeDef],
     },
 )
 GetEnvironmentResponseTypeDef = TypedDict(
     "GetEnvironmentResponseTypeDef",
     {
@@ -1052,14 +1099,15 @@
     {
         "applicationId": str,
         "batchJobIdentifier": BatchJobIdentifierTypeDef,
         "endTime": datetime,
         "executionId": str,
         "jobId": str,
         "jobName": str,
+        "jobStepRestartMarker": JobStepRestartMarkerTypeDef,
         "jobType": BatchJobTypeType,
         "jobUser": str,
         "returnCode": str,
         "startTime": datetime,
         "status": BatchJobExecutionStatusType,
         "statusReason": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
```

### Comparing `mypy-boto3-m2-1.34.0/mypy_boto3_m2.egg-info/PKG-INFO` & `mypy_boto3_m2-1.34.85/mypy_boto3_m2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-m2
-Version: 1.34.0
-Summary: Type annotations for boto3.MainframeModernization 1.34.0 service generated with mypy-boto3-builder 7.21.0
+Version: 1.34.85
+Summary: Type annotations for boto3.MainframeModernization 1.34.85 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/
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
 
 <a id="mypy-boto3-m2"></a>
 
 # mypy-boto3-m2
 
 [![PyPI - mypy-boto3-m2](https://img.shields.io/pypi/v/mypy-boto3-m2.svg?color=blue)](https://pypi.org/project/mypy-boto3-m2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-m2.svg?color=blue)](https://pypi.org/project/mypy-boto3-m2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-m2)](https://pepy.tech/project/mypy-boto3-m2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MainframeModernization 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization)
+[boto3.MainframeModernization 1.34.85](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization)
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
 [mypy-boto3-m2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-m2-1.34.0/mypy_boto3_m2.egg-info/SOURCES.txt` & `mypy_boto3_m2-1.34.85/mypy_boto3_m2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-m2-1.34.0/setup.py` & `mypy_boto3_m2-1.34.85/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,48 +7,44 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-m2",
-    version="1.34.0",
+    version="1.34.85",
     packages=["mypy_boto3_m2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description=(
-        "Type annotations for boto3.MainframeModernization 1.34.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
-    ),
+    description="Type annotations for boto3.MainframeModernization 1.34.85 service generated with mypy-boto3-builder 7.23.2",
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
     keywords="boto3 m2 type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_m2": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

