# Comparing `tmp/mypy-boto3-emr-serverless-1.34.0.tar.gz` & `tmp/mypy_boto3_emr_serverless-1.34.85.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-emr-serverless-1.34.0.tar", last modified: Wed Dec 13 21:22:37 2023, max compression
+gzip compressed data, was "mypy_boto3_emr_serverless-1.34.85.tar", last modified: Tue Apr 16 19:33:14 2024, max compression
```

## Comparing `mypy-boto3-emr-serverless-1.34.0.tar` & `mypy_boto3_emr_serverless-1.34.85.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:22:37.775210 mypy-boto3-emr-serverless-1.34.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 21:10:12.000000 mypy-boto3-emr-serverless-1.34.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13183 2023-12-13 21:22:37.775210 mypy-boto3-emr-serverless-1.34.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11623 2023-12-13 21:10:12.000000 mypy-boto3-emr-serverless-1.34.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:22:37.771210 mypy-boto3-emr-serverless-1.34.0/mypy_boto3_emr_serverless/
--rw-r--r--   0 runner    (1001) docker     (127)      808 2023-12-13 21:10:12.000000 mypy-boto3-emr-serverless-1.34.0/mypy_boto3_emr_serverless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      807 2023-12-13 21:10:12.000000 mypy-boto3-emr-serverless-1.34.0/mypy_boto3_emr_serverless/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      931 2023-12-13 21:10:12.000000 mypy-boto3-emr-serverless-1.34.0/mypy_boto3_emr_serverless/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14553 2023-12-13 21:10:12.000000 mypy-boto3-emr-serverless-1.34.0/mypy_boto3_emr_serverless/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    14549 2023-12-13 21:10:12.000000 mypy-boto3-emr-serverless-1.34.0/mypy_boto3_emr_serverless/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9223 2023-12-13 21:10:12.000000 mypy-boto3-emr-serverless-1.34.0/mypy_boto3_emr_serverless/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9221 2023-12-13 21:10:12.000000 mypy-boto3-emr-serverless-1.34.0/mypy_boto3_emr_serverless/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3305 2023-12-13 21:10:12.000000 mypy-boto3-emr-serverless-1.34.0/mypy_boto3_emr_serverless/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3301 2023-12-13 21:10:12.000000 mypy-boto3-emr-serverless-1.34.0/mypy_boto3_emr_serverless/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 21:10:12.000000 mypy-boto3-emr-serverless-1.34.0/mypy_boto3_emr_serverless/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    17747 2023-12-13 21:10:12.000000 mypy-boto3-emr-serverless-1.34.0/mypy_boto3_emr_serverless/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    17746 2023-12-13 21:10:12.000000 mypy-boto3-emr-serverless-1.34.0/mypy_boto3_emr_serverless/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-12-13 21:10:12.000000 mypy-boto3-emr-serverless-1.34.0/mypy_boto3_emr_serverless/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:22:37.771210 mypy-boto3-emr-serverless-1.34.0/mypy_boto3_emr_serverless.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13183 2023-12-13 21:22:37.000000 mypy-boto3-emr-serverless-1.34.0/mypy_boto3_emr_serverless.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      813 2023-12-13 21:22:37.000000 mypy-boto3-emr-serverless-1.34.0/mypy_boto3_emr_serverless.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:22:37.000000 mypy-boto3-emr-serverless-1.34.0/mypy_boto3_emr_serverless.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:22:37.000000 mypy-boto3-emr-serverless-1.34.0/mypy_boto3_emr_serverless.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 21:22:37.000000 mypy-boto3-emr-serverless-1.34.0/mypy_boto3_emr_serverless.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-12-13 21:22:37.000000 mypy-boto3-emr-serverless-1.34.0/mypy_boto3_emr_serverless.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 21:22:37.775210 mypy-boto3-emr-serverless-1.34.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2023-12-13 21:10:12.000000 mypy-boto3-emr-serverless-1.34.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:33:14.752305 mypy_boto3_emr_serverless-1.34.85/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-16 19:32:49.000000 mypy_boto3_emr_serverless-1.34.85/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13206 2024-04-16 19:33:14.752305 mypy_boto3_emr_serverless-1.34.85/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11624 2024-04-16 19:32:49.000000 mypy_boto3_emr_serverless-1.34.85/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:33:14.748305 mypy_boto3_emr_serverless-1.34.85/mypy_boto3_emr_serverless/
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-16 19:32:49.000000 mypy_boto3_emr_serverless-1.34.85/mypy_boto3_emr_serverless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-16 19:32:49.000000 mypy_boto3_emr_serverless-1.34.85/mypy_boto3_emr_serverless/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-16 19:32:49.000000 mypy_boto3_emr_serverless-1.34.85/mypy_boto3_emr_serverless/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14557 2024-04-16 19:32:49.000000 mypy_boto3_emr_serverless-1.34.85/mypy_boto3_emr_serverless/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14554 2024-04-16 19:32:49.000000 mypy_boto3_emr_serverless-1.34.85/mypy_boto3_emr_serverless/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9398 2024-04-16 19:32:49.000000 mypy_boto3_emr_serverless-1.34.85/mypy_boto3_emr_serverless/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9398 2024-04-16 19:32:49.000000 mypy_boto3_emr_serverless-1.34.85/mypy_boto3_emr_serverless/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-04-16 19:32:49.000000 mypy_boto3_emr_serverless-1.34.85/mypy_boto3_emr_serverless/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3303 2024-04-16 19:32:49.000000 mypy_boto3_emr_serverless-1.34.85/mypy_boto3_emr_serverless/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 19:32:49.000000 mypy_boto3_emr_serverless-1.34.85/mypy_boto3_emr_serverless/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    17797 2024-04-16 19:32:49.000000 mypy_boto3_emr_serverless-1.34.85/mypy_boto3_emr_serverless/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17797 2024-04-16 19:32:49.000000 mypy_boto3_emr_serverless-1.34.85/mypy_boto3_emr_serverless/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-16 19:32:49.000000 mypy_boto3_emr_serverless-1.34.85/mypy_boto3_emr_serverless/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:33:14.752305 mypy_boto3_emr_serverless-1.34.85/mypy_boto3_emr_serverless.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13206 2024-04-16 19:33:14.000000 mypy_boto3_emr_serverless-1.34.85/mypy_boto3_emr_serverless.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-16 19:33:14.000000 mypy_boto3_emr_serverless-1.34.85/mypy_boto3_emr_serverless.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 19:33:14.000000 mypy_boto3_emr_serverless-1.34.85/mypy_boto3_emr_serverless.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 19:33:14.000000 mypy_boto3_emr_serverless-1.34.85/mypy_boto3_emr_serverless.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-16 19:33:14.000000 mypy_boto3_emr_serverless-1.34.85/mypy_boto3_emr_serverless.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-16 19:33:14.000000 mypy_boto3_emr_serverless-1.34.85/mypy_boto3_emr_serverless.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 19:33:14.752305 mypy_boto3_emr_serverless-1.34.85/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-16 19:32:48.000000 mypy_boto3_emr_serverless-1.34.85/setup.py
```

### Comparing `mypy-boto3-emr-serverless-1.34.0/LICENSE` & `mypy_boto3_emr_serverless-1.34.85/LICENSE`

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

### Comparing `mypy-boto3-emr-serverless-1.34.0/PKG-INFO` & `mypy_boto3_emr_serverless-1.34.85/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-emr-serverless
-Version: 1.34.0
-Summary: Type annotations for boto3.EMRServerless 1.34.0 service generated with mypy-boto3-builder 7.21.0
+Version: 1.34.85
+Summary: Type annotations for boto3.EMRServerless 1.34.85 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/
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
 
 <a id="mypy-boto3-emr-serverless"></a>
 
 # mypy-boto3-emr-serverless
 
 [![PyPI - mypy-boto3-emr-serverless](https://img.shields.io/pypi/v/mypy-boto3-emr-serverless.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr-serverless)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-emr-serverless.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr-serverless)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-emr-serverless)](https://pepy.tech/project/mypy-boto3-emr-serverless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EMRServerless 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless)
+[boto3.EMRServerless 1.34.85](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless)
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
 [mypy-boto3-emr-serverless docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-emr-serverless-1.34.0/README.md` & `mypy_boto3_emr_serverless-1.34.85/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-emr-serverless.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr-serverless)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-emr-serverless)](https://pepy.tech/project/mypy-boto3-emr-serverless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EMRServerless 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless)
+[boto3.EMRServerless 1.34.85](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless)
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
 [mypy-boto3-emr-serverless docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-emr-serverless-1.34.0/mypy_boto3_emr_serverless/__init__.py` & `mypy_boto3_emr_serverless-1.34.85/mypy_boto3_emr_serverless/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,9 +21,8 @@
 """
 
 from .client import EMRServerlessClient
 from .paginator import ListApplicationsPaginator, ListJobRunsPaginator
 
 Client = EMRServerlessClient
 
-
 __all__ = ("Client", "EMRServerlessClient", "ListApplicationsPaginator", "ListJobRunsPaginator")
```

### Comparing `mypy-boto3-emr-serverless-1.34.0/mypy_boto3_emr_serverless/__init__.pyi` & `mypy_boto3_emr_serverless-1.34.85/mypy_boto3_emr_serverless/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-serverless-1.34.0/mypy_boto3_emr_serverless/__main__.py` & `mypy_boto3_emr_serverless-1.34.85/mypy_boto3_emr_serverless/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,28 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.EMRServerless 1.34.0\nVersion:         1.34.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
-        " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless//\nBoto3 docs:     "
-        " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless\nOther"
-        " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
-        " https://github.com/youtype/mypy_boto3_builder/releases"
+        "Type annotations for boto3.EMRServerless 1.34.85\n"
+        "Version:         1.34.85\n"
+        "Builder version: 7.23.2\n"
+        "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless//\n"
+        "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless\n"
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

### Comparing `mypy-boto3-emr-serverless-1.34.0/mypy_boto3_emr_serverless/client.py` & `mypy_boto3_emr_serverless-1.34.85/mypy_boto3_emr_serverless/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("EMRServerlessClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -126,15 +125,15 @@
         autoStartConfiguration: AutoStartConfigTypeDef = ...,
         autoStopConfiguration: AutoStopConfigTypeDef = ...,
         networkConfiguration: NetworkConfigurationTypeDef = ...,
         architecture: ArchitectureType = ...,
         imageConfiguration: ImageConfigurationInputTypeDef = ...,
         workerTypeSpecifications: Mapping[str, WorkerTypeSpecificationInputTypeDef] = ...,
         runtimeConfiguration: Sequence["ConfigurationTypeDef"] = ...,
-        monitoringConfiguration: MonitoringConfigurationTypeDef = ...
+        monitoringConfiguration: MonitoringConfigurationTypeDef = ...,
     ) -> CreateApplicationResponseTypeDef:
         """
         Creates an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client.create_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/client/#create_application)
         """
@@ -190,15 +189,15 @@
         """
 
     def list_applications(
         self,
         *,
         nextToken: str = ...,
         maxResults: int = ...,
-        states: Sequence[ApplicationStateType] = ...
+        states: Sequence[ApplicationStateType] = ...,
     ) -> ListApplicationsResponseTypeDef:
         """
         Lists applications based on a set of parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client.list_applications)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/client/#list_applications)
         """
@@ -207,15 +206,15 @@
         self,
         *,
         applicationId: str,
         nextToken: str = ...,
         maxResults: int = ...,
         createdAtAfter: TimestampTypeDef = ...,
         createdAtBefore: TimestampTypeDef = ...,
-        states: Sequence[JobRunStateType] = ...
+        states: Sequence[JobRunStateType] = ...,
     ) -> ListJobRunsResponseTypeDef:
         """
         Lists job runs based on a set of parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client.list_job_runs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/client/#list_job_runs)
         """
@@ -242,15 +241,15 @@
         applicationId: str,
         clientToken: str,
         executionRoleArn: str,
         jobDriver: JobDriverTypeDef = ...,
         configurationOverrides: ConfigurationOverridesTypeDef = ...,
         tags: Mapping[str, str] = ...,
         executionTimeoutMinutes: int = ...,
-        name: str = ...
+        name: str = ...,
     ) -> StartJobRunResponseTypeDef:
         """
         Starts a job run.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client.start_job_run)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/client/#start_job_run)
         """
@@ -290,15 +289,15 @@
         autoStopConfiguration: AutoStopConfigTypeDef = ...,
         networkConfiguration: NetworkConfigurationTypeDef = ...,
         architecture: ArchitectureType = ...,
         imageConfiguration: ImageConfigurationInputTypeDef = ...,
         workerTypeSpecifications: Mapping[str, WorkerTypeSpecificationInputTypeDef] = ...,
         releaseLabel: str = ...,
         runtimeConfiguration: Sequence["ConfigurationTypeDef"] = ...,
-        monitoringConfiguration: MonitoringConfigurationTypeDef = ...
+        monitoringConfiguration: MonitoringConfigurationTypeDef = ...,
     ) -> UpdateApplicationResponseTypeDef:
         """
         Updates a specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client.update_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/client/#update_application)
         """
```

### Comparing `mypy-boto3-emr-serverless-1.34.0/mypy_boto3_emr_serverless/client.pyi` & `mypy_boto3_emr_serverless-1.34.85/mypy_boto3_emr_serverless/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -122,15 +122,15 @@
         autoStartConfiguration: AutoStartConfigTypeDef = ...,
         autoStopConfiguration: AutoStopConfigTypeDef = ...,
         networkConfiguration: NetworkConfigurationTypeDef = ...,
         architecture: ArchitectureType = ...,
         imageConfiguration: ImageConfigurationInputTypeDef = ...,
         workerTypeSpecifications: Mapping[str, WorkerTypeSpecificationInputTypeDef] = ...,
         runtimeConfiguration: Sequence["ConfigurationTypeDef"] = ...,
-        monitoringConfiguration: MonitoringConfigurationTypeDef = ...
+        monitoringConfiguration: MonitoringConfigurationTypeDef = ...,
     ) -> CreateApplicationResponseTypeDef:
         """
         Creates an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client.create_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/client/#create_application)
         """
@@ -186,15 +186,15 @@
         """
 
     def list_applications(
         self,
         *,
         nextToken: str = ...,
         maxResults: int = ...,
-        states: Sequence[ApplicationStateType] = ...
+        states: Sequence[ApplicationStateType] = ...,
     ) -> ListApplicationsResponseTypeDef:
         """
         Lists applications based on a set of parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client.list_applications)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/client/#list_applications)
         """
@@ -203,15 +203,15 @@
         self,
         *,
         applicationId: str,
         nextToken: str = ...,
         maxResults: int = ...,
         createdAtAfter: TimestampTypeDef = ...,
         createdAtBefore: TimestampTypeDef = ...,
-        states: Sequence[JobRunStateType] = ...
+        states: Sequence[JobRunStateType] = ...,
     ) -> ListJobRunsResponseTypeDef:
         """
         Lists job runs based on a set of parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client.list_job_runs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/client/#list_job_runs)
         """
@@ -238,15 +238,15 @@
         applicationId: str,
         clientToken: str,
         executionRoleArn: str,
         jobDriver: JobDriverTypeDef = ...,
         configurationOverrides: ConfigurationOverridesTypeDef = ...,
         tags: Mapping[str, str] = ...,
         executionTimeoutMinutes: int = ...,
-        name: str = ...
+        name: str = ...,
     ) -> StartJobRunResponseTypeDef:
         """
         Starts a job run.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client.start_job_run)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/client/#start_job_run)
         """
@@ -286,15 +286,15 @@
         autoStopConfiguration: AutoStopConfigTypeDef = ...,
         networkConfiguration: NetworkConfigurationTypeDef = ...,
         architecture: ArchitectureType = ...,
         imageConfiguration: ImageConfigurationInputTypeDef = ...,
         workerTypeSpecifications: Mapping[str, WorkerTypeSpecificationInputTypeDef] = ...,
         releaseLabel: str = ...,
         runtimeConfiguration: Sequence["ConfigurationTypeDef"] = ...,
-        monitoringConfiguration: MonitoringConfigurationTypeDef = ...
+        monitoringConfiguration: MonitoringConfigurationTypeDef = ...,
     ) -> UpdateApplicationResponseTypeDef:
         """
         Updates a specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client.update_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/client/#update_application)
         """
```

### Comparing `mypy-boto3-emr-serverless-1.34.0/mypy_boto3_emr_serverless/literals.py` & `mypy_boto3_emr_serverless-1.34.85/mypy_boto3_emr_serverless/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,29 +15,27 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ApplicationStateType",
     "ArchitectureType",
     "JobRunStateType",
     "ListApplicationsPaginatorName",
     "ListJobRunsPaginatorName",
     "EMRServerlessServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ApplicationStateType = Literal[
     "CREATED", "CREATING", "STARTED", "STARTING", "STOPPED", "STOPPING", "TERMINATED"
 ]
 ArchitectureType = Literal["ARM64", "X86_64"]
 JobRunStateType = Literal[
     "CANCELLED", "CANCELLING", "FAILED", "PENDING", "RUNNING", "SCHEDULED", "SUBMITTED", "SUCCESS"
 ]
@@ -66,14 +64,15 @@
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
@@ -84,14 +83,15 @@
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
@@ -109,14 +109,15 @@
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
@@ -129,24 +130,26 @@
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
@@ -207,15 +210,14 @@
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
@@ -287,17 +289,19 @@
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
@@ -387,19 +391,21 @@
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
@@ -443,14 +449,15 @@
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
     "ca-central-1",
     "eu-central-1",
     "eu-north-1",
     "eu-south-1",
+    "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
```

### Comparing `mypy-boto3-emr-serverless-1.34.0/mypy_boto3_emr_serverless/literals.pyi` & `mypy_boto3_emr_serverless-1.34.85/mypy_boto3_emr_serverless/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -64,14 +64,15 @@
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
@@ -82,14 +83,15 @@
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
@@ -107,14 +109,15 @@
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
@@ -127,24 +130,26 @@
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
@@ -205,15 +210,14 @@
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
@@ -285,17 +289,19 @@
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
@@ -385,19 +391,21 @@
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
@@ -441,14 +449,15 @@
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
     "ca-central-1",
     "eu-central-1",
     "eu-north-1",
     "eu-south-1",
+    "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
```

### Comparing `mypy-boto3-emr-serverless-1.34.0/mypy_boto3_emr_serverless/paginator.py` & `mypy_boto3_emr_serverless-1.34.85/mypy_boto3_emr_serverless/paginator.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,15 +32,14 @@
     ListJobRunsResponseTypeDef,
     PaginatorConfigTypeDef,
     TimestampTypeDef,
 )
 
 __all__ = ("ListApplicationsPaginator", "ListJobRunsPaginator")
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -53,15 +52,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/paginators/#listapplicationspaginator)
     """
 
     def paginate(
         self,
         *,
         states: Sequence[ApplicationStateType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Paginator.ListApplications.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/paginators/#listapplicationspaginator)
         """
 
 
@@ -74,13 +73,13 @@
     def paginate(
         self,
         *,
         applicationId: str,
         createdAtAfter: TimestampTypeDef = ...,
         createdAtBefore: TimestampTypeDef = ...,
         states: Sequence[JobRunStateType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListJobRunsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Paginator.ListJobRuns.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/paginators/#listjobrunspaginator)
         """
```

### Comparing `mypy-boto3-emr-serverless-1.34.0/mypy_boto3_emr_serverless/paginator.pyi` & `mypy_boto3_emr_serverless-1.34.85/mypy_boto3_emr_serverless/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/paginators/#listapplicationspaginator)
     """
 
     def paginate(
         self,
         *,
         states: Sequence[ApplicationStateType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Paginator.ListApplications.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/paginators/#listapplicationspaginator)
         """
 
 class ListJobRunsPaginator(Paginator):
@@ -70,13 +70,13 @@
     def paginate(
         self,
         *,
         applicationId: str,
         createdAtAfter: TimestampTypeDef = ...,
         createdAtBefore: TimestampTypeDef = ...,
         states: Sequence[JobRunStateType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListJobRunsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Paginator.ListJobRuns.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/paginators/#listjobrunspaginator)
         """
```

### Comparing `mypy-boto3-emr-serverless-1.34.0/mypy_boto3_emr_serverless/type_defs.py` & `mypy_boto3_emr_serverless-1.34.85/mypy_boto3_emr_serverless/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ApplicationSummaryTypeDef",
     "AutoStartConfigTypeDef",
     "AutoStopConfigTypeDef",
     "ImageConfigurationTypeDef",
     "MaximumAllowedResourcesTypeDef",
     "NetworkConfigurationTypeDef",
@@ -143,18 +142,18 @@
         "jobRunId": str,
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
 CloudWatchLoggingConfigurationTypeDef = TypedDict(
     "CloudWatchLoggingConfigurationTypeDef",
     {
         "enabled": bool,
         "logGroupName": NotRequired[str],
@@ -213,14 +212,15 @@
 )
 WorkerResourceConfigTypeDef = TypedDict(
     "WorkerResourceConfigTypeDef",
     {
         "cpu": str,
         "memory": str,
         "disk": NotRequired[str],
+        "diskType": NotRequired[str],
     },
 )
 SparkSubmitTypeDef = TypedDict(
     "SparkSubmitTypeDef",
     {
         "entryPoint": str,
         "entryPointArguments": NotRequired[List[str]],
```

### Comparing `mypy-boto3-emr-serverless-1.34.0/mypy_boto3_emr_serverless/type_defs.pyi` & `mypy_boto3_emr_serverless-1.34.85/mypy_boto3_emr_serverless/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -142,18 +142,18 @@
         "jobRunId": str,
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
 CloudWatchLoggingConfigurationTypeDef = TypedDict(
     "CloudWatchLoggingConfigurationTypeDef",
     {
         "enabled": bool,
         "logGroupName": NotRequired[str],
@@ -212,14 +212,15 @@
 )
 WorkerResourceConfigTypeDef = TypedDict(
     "WorkerResourceConfigTypeDef",
     {
         "cpu": str,
         "memory": str,
         "disk": NotRequired[str],
+        "diskType": NotRequired[str],
     },
 )
 SparkSubmitTypeDef = TypedDict(
     "SparkSubmitTypeDef",
     {
         "entryPoint": str,
         "entryPointArguments": NotRequired[List[str]],
```

### Comparing `mypy-boto3-emr-serverless-1.34.0/mypy_boto3_emr_serverless.egg-info/PKG-INFO` & `mypy_boto3_emr_serverless-1.34.85/mypy_boto3_emr_serverless.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-emr-serverless
-Version: 1.34.0
-Summary: Type annotations for boto3.EMRServerless 1.34.0 service generated with mypy-boto3-builder 7.21.0
+Version: 1.34.85
+Summary: Type annotations for boto3.EMRServerless 1.34.85 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/
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
 
 <a id="mypy-boto3-emr-serverless"></a>
 
 # mypy-boto3-emr-serverless
 
 [![PyPI - mypy-boto3-emr-serverless](https://img.shields.io/pypi/v/mypy-boto3-emr-serverless.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr-serverless)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-emr-serverless.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr-serverless)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-emr-serverless)](https://pepy.tech/project/mypy-boto3-emr-serverless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EMRServerless 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless)
+[boto3.EMRServerless 1.34.85](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless)
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
 [mypy-boto3-emr-serverless docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-emr-serverless-1.34.0/mypy_boto3_emr_serverless.egg-info/SOURCES.txt` & `mypy_boto3_emr_serverless-1.34.85/mypy_boto3_emr_serverless.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-serverless-1.34.0/setup.py` & `mypy_boto3_emr_serverless-1.34.85/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,48 +7,44 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-emr-serverless",
-    version="1.34.0",
+    version="1.34.85",
     packages=["mypy_boto3_emr_serverless"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description=(
-        "Type annotations for boto3.EMRServerless 1.34.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
-    ),
+    description="Type annotations for boto3.EMRServerless 1.34.85 service generated with mypy-boto3-builder 7.23.2",
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
     keywords="boto3 emr-serverless type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_emr_serverless": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

