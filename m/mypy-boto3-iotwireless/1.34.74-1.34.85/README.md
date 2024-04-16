# Comparing `tmp/mypy-boto3-iotwireless-1.34.74.tar.gz` & `tmp/mypy_boto3_iotwireless-1.34.85.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-iotwireless-1.34.74.tar", last modified: Fri Mar 29 19:18:23 2024, max compression
+gzip compressed data, was "mypy_boto3_iotwireless-1.34.85.tar", last modified: Tue Apr 16 19:33:15 2024, max compression
```

## Comparing `mypy-boto3-iotwireless-1.34.74.tar` & `mypy_boto3_iotwireless-1.34.85.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 19:18:23.976137 mypy-boto3-iotwireless-1.34.74/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-29 19:17:46.000000 mypy-boto3-iotwireless-1.34.74/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12283 2024-03-29 19:18:23.976137 mypy-boto3-iotwireless-1.34.74/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10712 2024-03-29 19:17:46.000000 mypy-boto3-iotwireless-1.34.74/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 19:18:23.972137 mypy-boto3-iotwireless-1.34.74/mypy_boto3_iotwireless/
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-03-29 19:17:46.000000 mypy-boto3-iotwireless-1.34.74/mypy_boto3_iotwireless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-03-29 19:17:46.000000 mypy-boto3-iotwireless-1.34.74/mypy_boto3_iotwireless/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-03-29 19:17:46.000000 mypy-boto3-iotwireless-1.34.74/mypy_boto3_iotwireless/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    73750 2024-03-29 19:17:47.000000 mypy-boto3-iotwireless-1.34.74/mypy_boto3_iotwireless/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    73747 2024-03-29 19:17:46.000000 mypy-boto3-iotwireless-1.34.74/mypy_boto3_iotwireless/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    14166 2024-03-29 19:17:47.000000 mypy-boto3-iotwireless-1.34.74/mypy_boto3_iotwireless/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    14166 2024-03-29 19:17:47.000000 mypy-boto3-iotwireless-1.34.74/mypy_boto3_iotwireless/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 19:17:46.000000 mypy-boto3-iotwireless-1.34.74/mypy_boto3_iotwireless/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    90188 2024-03-29 19:17:49.000000 mypy-boto3-iotwireless-1.34.74/mypy_boto3_iotwireless/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    90188 2024-03-29 19:17:48.000000 mypy-boto3-iotwireless-1.34.74/mypy_boto3_iotwireless/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-29 19:17:46.000000 mypy-boto3-iotwireless-1.34.74/mypy_boto3_iotwireless/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 19:18:23.976137 mypy-boto3-iotwireless-1.34.74/mypy_boto3_iotwireless.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12283 2024-03-29 19:18:23.000000 mypy-boto3-iotwireless-1.34.74/mypy_boto3_iotwireless.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-03-29 19:18:23.000000 mypy-boto3-iotwireless-1.34.74/mypy_boto3_iotwireless.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 19:18:23.000000 mypy-boto3-iotwireless-1.34.74/mypy_boto3_iotwireless.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 19:18:23.000000 mypy-boto3-iotwireless-1.34.74/mypy_boto3_iotwireless.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-29 19:18:23.000000 mypy-boto3-iotwireless-1.34.74/mypy_boto3_iotwireless.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-29 19:18:23.000000 mypy-boto3-iotwireless-1.34.74/mypy_boto3_iotwireless.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 19:18:23.976137 mypy-boto3-iotwireless-1.34.74/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-03-29 19:17:46.000000 mypy-boto3-iotwireless-1.34.74/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:33:15.424314 mypy_boto3_iotwireless-1.34.85/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-16 19:32:52.000000 mypy_boto3_iotwireless-1.34.85/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12283 2024-04-16 19:33:15.424314 mypy_boto3_iotwireless-1.34.85/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10712 2024-04-16 19:32:52.000000 mypy_boto3_iotwireless-1.34.85/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:33:15.424314 mypy_boto3_iotwireless-1.34.85/mypy_boto3_iotwireless/
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-16 19:32:52.000000 mypy_boto3_iotwireless-1.34.85/mypy_boto3_iotwireless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-16 19:32:52.000000 mypy_boto3_iotwireless-1.34.85/mypy_boto3_iotwireless/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-16 19:32:52.000000 mypy_boto3_iotwireless-1.34.85/mypy_boto3_iotwireless/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73795 2024-04-16 19:32:52.000000 mypy_boto3_iotwireless-1.34.85/mypy_boto3_iotwireless/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73792 2024-04-16 19:32:52.000000 mypy_boto3_iotwireless-1.34.85/mypy_boto3_iotwireless/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    14204 2024-04-16 19:32:53.000000 mypy_boto3_iotwireless-1.34.85/mypy_boto3_iotwireless/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14204 2024-04-16 19:32:53.000000 mypy_boto3_iotwireless-1.34.85/mypy_boto3_iotwireless/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 19:32:52.000000 mypy_boto3_iotwireless-1.34.85/mypy_boto3_iotwireless/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    90644 2024-04-16 19:32:54.000000 mypy_boto3_iotwireless-1.34.85/mypy_boto3_iotwireless/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    90644 2024-04-16 19:32:54.000000 mypy_boto3_iotwireless-1.34.85/mypy_boto3_iotwireless/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-16 19:32:52.000000 mypy_boto3_iotwireless-1.34.85/mypy_boto3_iotwireless/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:33:15.424314 mypy_boto3_iotwireless-1.34.85/mypy_boto3_iotwireless.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12283 2024-04-16 19:33:15.000000 mypy_boto3_iotwireless-1.34.85/mypy_boto3_iotwireless.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-16 19:33:15.000000 mypy_boto3_iotwireless-1.34.85/mypy_boto3_iotwireless.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 19:33:15.000000 mypy_boto3_iotwireless-1.34.85/mypy_boto3_iotwireless.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 19:33:15.000000 mypy_boto3_iotwireless-1.34.85/mypy_boto3_iotwireless.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-16 19:33:15.000000 mypy_boto3_iotwireless-1.34.85/mypy_boto3_iotwireless.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-16 19:33:15.000000 mypy_boto3_iotwireless-1.34.85/mypy_boto3_iotwireless.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 19:33:15.424314 mypy_boto3_iotwireless-1.34.85/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-04-16 19:32:51.000000 mypy_boto3_iotwireless-1.34.85/setup.py
```

### Comparing `mypy-boto3-iotwireless-1.34.74/LICENSE` & `mypy_boto3_iotwireless-1.34.85/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotwireless-1.34.74/PKG-INFO` & `mypy_boto3_iotwireless-1.34.85/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotwireless
-Version: 1.34.74
-Summary: Type annotations for boto3.IoTWireless 1.34.74 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.85
+Summary: Type annotations for boto3.IoTWireless 1.34.85 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotwireless.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotwireless)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotwireless)](https://pepy.tech/project/mypy-boto3-iotwireless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTWireless 1.34.74](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless)
+[boto3.IoTWireless 1.34.85](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-iotwireless-1.34.74/README.md` & `mypy_boto3_iotwireless-1.34.85/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotwireless.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotwireless)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotwireless)](https://pepy.tech/project/mypy-boto3-iotwireless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTWireless 1.34.74](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless)
+[boto3.IoTWireless 1.34.85](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-iotwireless-1.34.74/mypy_boto3_iotwireless/__main__.py` & `mypy_boto3_iotwireless-1.34.85/mypy_boto3_iotwireless/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IoTWireless 1.34.74\n"
-        "Version:         1.34.74\n"
+        "Type annotations for boto3.IoTWireless 1.34.85\n"
+        "Version:         1.34.85\n"
         "Builder version: 7.23.2\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.74")
+    print("1.34.85")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-iotwireless-1.34.74/mypy_boto3_iotwireless/client.py` & `mypy_boto3_iotwireless-1.34.85/mypy_boto3_iotwireless/client.pyi`

 * *Files identical despite different names*

```diff
@@ -142,34 +142,31 @@
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = ("IoTWirelessClient",)
 
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
     InternalServerException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     TooManyTagsException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
-
 class IoTWirelessClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/client/)
     """
 
     meta: ClientMeta
@@ -670,25 +667,25 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.get_log_levels_by_resource_types)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/client/#get_log_levels_by_resource_types)
         """
 
     def get_metric_configuration(self) -> GetMetricConfigurationResponseTypeDef:
         """
-        Get the metric configuration status for this account.
+        Get the metric configuration status for this AWS account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.get_metric_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/client/#get_metric_configuration)
         """
 
     def get_metrics(
         self, *, SummaryMetricQueries: Sequence[SummaryMetricQueryTypeDef] = ...
     ) -> GetMetricsResponseTypeDef:
         """
-        Get metrics.
+        Get the summary metrics for this AWS account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.get_metrics)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/client/#get_metrics)
         """
 
     def get_multicast_group(self, *, Id: str) -> GetMulticastGroupResponseTypeDef:
         """
@@ -1347,15 +1344,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/client/#update_log_levels_by_resource_types)
         """
 
     def update_metric_configuration(
         self, *, SummaryMetric: SummaryMetricConfigurationTypeDef = ...
     ) -> Dict[str, Any]:
         """
-        Update the metric configuration.
+        Update the summary metric configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.update_metric_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/client/#update_metric_configuration)
         """
 
     def update_multicast_group(
         self,
```

### Comparing `mypy-boto3-iotwireless-1.34.74/mypy_boto3_iotwireless/client.pyi` & `mypy_boto3_iotwireless-1.34.85/mypy_boto3_iotwireless/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,31 +142,34 @@
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = ("IoTWirelessClient",)
 
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
     InternalServerException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     TooManyTagsException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
+
 class IoTWirelessClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/client/)
     """
 
     meta: ClientMeta
@@ -667,25 +670,25 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.get_log_levels_by_resource_types)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/client/#get_log_levels_by_resource_types)
         """
 
     def get_metric_configuration(self) -> GetMetricConfigurationResponseTypeDef:
         """
-        Get the metric configuration status for this account.
+        Get the metric configuration status for this AWS account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.get_metric_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/client/#get_metric_configuration)
         """
 
     def get_metrics(
         self, *, SummaryMetricQueries: Sequence[SummaryMetricQueryTypeDef] = ...
     ) -> GetMetricsResponseTypeDef:
         """
-        Get metrics.
+        Get the summary metrics for this AWS account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.get_metrics)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/client/#get_metrics)
         """
 
     def get_multicast_group(self, *, Id: str) -> GetMulticastGroupResponseTypeDef:
         """
@@ -1344,15 +1347,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/client/#update_log_levels_by_resource_types)
         """
 
     def update_metric_configuration(
         self, *, SummaryMetric: SummaryMetricConfigurationTypeDef = ...
     ) -> Dict[str, Any]:
         """
-        Update the metric configuration.
+        Update the summary metric configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.update_metric_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/client/#update_metric_configuration)
         """
 
     def update_multicast_group(
         self,
```

### Comparing `mypy-boto3-iotwireless-1.34.74/mypy_boto3_iotwireless/literals.py` & `mypy_boto3_iotwireless-1.34.85/mypy_boto3_iotwireless/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -279,24 +279,26 @@
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
```

### Comparing `mypy-boto3-iotwireless-1.34.74/mypy_boto3_iotwireless/literals.pyi` & `mypy_boto3_iotwireless-1.34.85/mypy_boto3_iotwireless/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -279,24 +279,26 @@
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
```

### Comparing `mypy-boto3-iotwireless-1.34.74/mypy_boto3_iotwireless/type_defs.py` & `mypy_boto3_iotwireless-1.34.85/mypy_boto3_iotwireless/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -188,14 +188,15 @@
     "ServiceProfileTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListWirelessDeviceImportTasksRequestRequestTypeDef",
     "ListWirelessDevicesRequestRequestTypeDef",
     "ListWirelessGatewayTaskDefinitionsRequestRequestTypeDef",
     "ListWirelessGatewaysRequestRequestTypeDef",
     "LoRaWANGatewayMetadataTypeDef",
+    "LoRaWANPublicGatewayMetadataTypeDef",
     "OtaaV10XTypeDef",
     "OtaaV11TypeDef",
     "LoRaWANGatewayVersionTypeDef",
     "LoRaWANListDeviceTypeDef",
     "LoRaWANMulticastMetadataTypeDef",
     "UpdateAbpV10XTypeDef",
     "UpdateAbpV11TypeDef",
@@ -1236,14 +1237,25 @@
     "LoRaWANGatewayMetadataTypeDef",
     {
         "GatewayEui": NotRequired[str],
         "Snr": NotRequired[float],
         "Rssi": NotRequired[float],
     },
 )
+LoRaWANPublicGatewayMetadataTypeDef = TypedDict(
+    "LoRaWANPublicGatewayMetadataTypeDef",
+    {
+        "ProviderNetId": NotRequired[str],
+        "Id": NotRequired[str],
+        "Rssi": NotRequired[float],
+        "Snr": NotRequired[float],
+        "RfRegion": NotRequired[str],
+        "DlAllowed": NotRequired[bool],
+    },
+)
 OtaaV10XTypeDef = TypedDict(
     "OtaaV10XTypeDef",
     {
         "AppKey": NotRequired[str],
         "AppEui": NotRequired[str],
         "JoinEui": NotRequired[str],
         "GenAppKey": NotRequired[str],
@@ -2224,14 +2236,15 @@
     {
         "DevEui": NotRequired[str],
         "FPort": NotRequired[int],
         "DataRate": NotRequired[int],
         "Frequency": NotRequired[int],
         "Timestamp": NotRequired[str],
         "Gateways": NotRequired[List[LoRaWANGatewayMetadataTypeDef]],
+        "PublicGateways": NotRequired[List[LoRaWANPublicGatewayMetadataTypeDef]],
     },
 )
 LoRaWANGatewayCurrentVersionTypeDef = TypedDict(
     "LoRaWANGatewayCurrentVersionTypeDef",
     {
         "CurrentVersion": NotRequired[LoRaWANGatewayVersionTypeDef],
     },
```

### Comparing `mypy-boto3-iotwireless-1.34.74/mypy_boto3_iotwireless/type_defs.pyi` & `mypy_boto3_iotwireless-1.34.85/mypy_boto3_iotwireless/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -188,14 +188,15 @@
     "ServiceProfileTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListWirelessDeviceImportTasksRequestRequestTypeDef",
     "ListWirelessDevicesRequestRequestTypeDef",
     "ListWirelessGatewayTaskDefinitionsRequestRequestTypeDef",
     "ListWirelessGatewaysRequestRequestTypeDef",
     "LoRaWANGatewayMetadataTypeDef",
+    "LoRaWANPublicGatewayMetadataTypeDef",
     "OtaaV10XTypeDef",
     "OtaaV11TypeDef",
     "LoRaWANGatewayVersionTypeDef",
     "LoRaWANListDeviceTypeDef",
     "LoRaWANMulticastMetadataTypeDef",
     "UpdateAbpV10XTypeDef",
     "UpdateAbpV11TypeDef",
@@ -1236,14 +1237,25 @@
     "LoRaWANGatewayMetadataTypeDef",
     {
         "GatewayEui": NotRequired[str],
         "Snr": NotRequired[float],
         "Rssi": NotRequired[float],
     },
 )
+LoRaWANPublicGatewayMetadataTypeDef = TypedDict(
+    "LoRaWANPublicGatewayMetadataTypeDef",
+    {
+        "ProviderNetId": NotRequired[str],
+        "Id": NotRequired[str],
+        "Rssi": NotRequired[float],
+        "Snr": NotRequired[float],
+        "RfRegion": NotRequired[str],
+        "DlAllowed": NotRequired[bool],
+    },
+)
 OtaaV10XTypeDef = TypedDict(
     "OtaaV10XTypeDef",
     {
         "AppKey": NotRequired[str],
         "AppEui": NotRequired[str],
         "JoinEui": NotRequired[str],
         "GenAppKey": NotRequired[str],
@@ -2224,14 +2236,15 @@
     {
         "DevEui": NotRequired[str],
         "FPort": NotRequired[int],
         "DataRate": NotRequired[int],
         "Frequency": NotRequired[int],
         "Timestamp": NotRequired[str],
         "Gateways": NotRequired[List[LoRaWANGatewayMetadataTypeDef]],
+        "PublicGateways": NotRequired[List[LoRaWANPublicGatewayMetadataTypeDef]],
     },
 )
 LoRaWANGatewayCurrentVersionTypeDef = TypedDict(
     "LoRaWANGatewayCurrentVersionTypeDef",
     {
         "CurrentVersion": NotRequired[LoRaWANGatewayVersionTypeDef],
     },
```

### Comparing `mypy-boto3-iotwireless-1.34.74/mypy_boto3_iotwireless.egg-info/PKG-INFO` & `mypy_boto3_iotwireless-1.34.85/mypy_boto3_iotwireless.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotwireless
-Version: 1.34.74
-Summary: Type annotations for boto3.IoTWireless 1.34.74 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.85
+Summary: Type annotations for boto3.IoTWireless 1.34.85 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotwireless.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotwireless)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotwireless)](https://pepy.tech/project/mypy-boto3-iotwireless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTWireless 1.34.74](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless)
+[boto3.IoTWireless 1.34.85](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-iotwireless-1.34.74/mypy_boto3_iotwireless.egg-info/SOURCES.txt` & `mypy_boto3_iotwireless-1.34.85/mypy_boto3_iotwireless.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotwireless-1.34.74/setup.py` & `mypy_boto3_iotwireless-1.34.85/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-iotwireless",
-    version="1.34.74",
+    version="1.34.85",
     packages=["mypy_boto3_iotwireless"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.IoTWireless 1.34.74 service generated with mypy-boto3-builder 7.23.2",
+    description="Type annotations for boto3.IoTWireless 1.34.85 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

