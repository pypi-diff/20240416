# Comparing `tmp/mypy-boto3-mediapackagev2-1.34.60.tar.gz` & `tmp/mypy_boto3_mediapackagev2-1.34.85.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-mediapackagev2-1.34.60.tar", last modified: Mon Mar 11 19:47:10 2024, max compression
+gzip compressed data, was "mypy_boto3_mediapackagev2-1.34.85.tar", last modified: Tue Apr 16 19:33:16 2024, max compression
```

## Comparing `mypy-boto3-mediapackagev2-1.34.60.tar` & `mypy_boto3_mediapackagev2-1.34.85.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 19:47:10.182888 mypy-boto3-mediapackagev2-1.34.60/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-11 19:46:58.000000 mypy-boto3-mediapackagev2-1.34.60/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13407 2024-03-11 19:47:10.182888 mypy-boto3-mediapackagev2-1.34.60/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11824 2024-03-11 19:46:58.000000 mypy-boto3-mediapackagev2-1.34.60/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 19:47:10.182888 mypy-boto3-mediapackagev2-1.34.60/mypy_boto3_mediapackagev2/
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-03-11 19:46:58.000000 mypy-boto3-mediapackagev2-1.34.60/mypy_boto3_mediapackagev2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-03-11 19:46:58.000000 mypy-boto3-mediapackagev2-1.34.60/mypy_boto3_mediapackagev2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-03-11 19:46:58.000000 mypy-boto3-mediapackagev2-1.34.60/mypy_boto3_mediapackagev2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20387 2024-03-11 19:46:58.000000 mypy-boto3-mediapackagev2-1.34.60/mypy_boto3_mediapackagev2/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    20384 2024-03-11 19:46:58.000000 mypy-boto3-mediapackagev2-1.34.60/mypy_boto3_mediapackagev2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10151 2024-03-11 19:46:58.000000 mypy-boto3-mediapackagev2-1.34.60/mypy_boto3_mediapackagev2/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10151 2024-03-11 19:46:58.000000 mypy-boto3-mediapackagev2-1.34.60/mypy_boto3_mediapackagev2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-03-11 19:46:58.000000 mypy-boto3-mediapackagev2-1.34.60/mypy_boto3_mediapackagev2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4188 2024-03-11 19:46:58.000000 mypy-boto3-mediapackagev2-1.34.60/mypy_boto3_mediapackagev2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 19:46:58.000000 mypy-boto3-mediapackagev2-1.34.60/mypy_boto3_mediapackagev2/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    22179 2024-03-11 19:46:59.000000 mypy-boto3-mediapackagev2-1.34.60/mypy_boto3_mediapackagev2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    22179 2024-03-11 19:46:58.000000 mypy-boto3-mediapackagev2-1.34.60/mypy_boto3_mediapackagev2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-11 19:46:58.000000 mypy-boto3-mediapackagev2-1.34.60/mypy_boto3_mediapackagev2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 19:47:10.182888 mypy-boto3-mediapackagev2-1.34.60/mypy_boto3_mediapackagev2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13407 2024-03-11 19:47:10.000000 mypy-boto3-mediapackagev2-1.34.60/mypy_boto3_mediapackagev2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-03-11 19:47:10.000000 mypy-boto3-mediapackagev2-1.34.60/mypy_boto3_mediapackagev2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 19:47:10.000000 mypy-boto3-mediapackagev2-1.34.60/mypy_boto3_mediapackagev2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 19:47:10.000000 mypy-boto3-mediapackagev2-1.34.60/mypy_boto3_mediapackagev2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-11 19:47:10.000000 mypy-boto3-mediapackagev2-1.34.60/mypy_boto3_mediapackagev2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-11 19:47:10.000000 mypy-boto3-mediapackagev2-1.34.60/mypy_boto3_mediapackagev2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-11 19:47:10.182888 mypy-boto3-mediapackagev2-1.34.60/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-03-11 19:46:58.000000 mypy-boto3-mediapackagev2-1.34.60/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:33:16.484328 mypy_boto3_mediapackagev2-1.34.85/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-16 19:32:59.000000 mypy_boto3_mediapackagev2-1.34.85/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13409 2024-04-16 19:33:16.484328 mypy_boto3_mediapackagev2-1.34.85/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11826 2024-04-16 19:32:59.000000 mypy_boto3_mediapackagev2-1.34.85/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:33:16.480328 mypy_boto3_mediapackagev2-1.34.85/mypy_boto3_mediapackagev2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-16 19:32:59.000000 mypy_boto3_mediapackagev2-1.34.85/mypy_boto3_mediapackagev2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-16 19:32:59.000000 mypy_boto3_mediapackagev2-1.34.85/mypy_boto3_mediapackagev2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-16 19:32:59.000000 mypy_boto3_mediapackagev2-1.34.85/mypy_boto3_mediapackagev2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20589 2024-04-16 19:32:59.000000 mypy_boto3_mediapackagev2-1.34.85/mypy_boto3_mediapackagev2/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20586 2024-04-16 19:32:59.000000 mypy_boto3_mediapackagev2-1.34.85/mypy_boto3_mediapackagev2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10732 2024-04-16 19:32:59.000000 mypy_boto3_mediapackagev2-1.34.85/mypy_boto3_mediapackagev2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10732 2024-04-16 19:32:59.000000 mypy_boto3_mediapackagev2-1.34.85/mypy_boto3_mediapackagev2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-04-16 19:32:59.000000 mypy_boto3_mediapackagev2-1.34.85/mypy_boto3_mediapackagev2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4188 2024-04-16 19:32:59.000000 mypy_boto3_mediapackagev2-1.34.85/mypy_boto3_mediapackagev2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 19:32:59.000000 mypy_boto3_mediapackagev2-1.34.85/mypy_boto3_mediapackagev2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    24899 2024-04-16 19:32:59.000000 mypy_boto3_mediapackagev2-1.34.85/mypy_boto3_mediapackagev2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24899 2024-04-16 19:32:59.000000 mypy_boto3_mediapackagev2-1.34.85/mypy_boto3_mediapackagev2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-16 19:32:59.000000 mypy_boto3_mediapackagev2-1.34.85/mypy_boto3_mediapackagev2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:33:16.484328 mypy_boto3_mediapackagev2-1.34.85/mypy_boto3_mediapackagev2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13409 2024-04-16 19:33:16.000000 mypy_boto3_mediapackagev2-1.34.85/mypy_boto3_mediapackagev2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-16 19:33:16.000000 mypy_boto3_mediapackagev2-1.34.85/mypy_boto3_mediapackagev2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 19:33:16.000000 mypy_boto3_mediapackagev2-1.34.85/mypy_boto3_mediapackagev2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 19:33:16.000000 mypy_boto3_mediapackagev2-1.34.85/mypy_boto3_mediapackagev2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-16 19:33:16.000000 mypy_boto3_mediapackagev2-1.34.85/mypy_boto3_mediapackagev2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-16 19:33:16.000000 mypy_boto3_mediapackagev2-1.34.85/mypy_boto3_mediapackagev2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 19:33:16.484328 mypy_boto3_mediapackagev2-1.34.85/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-04-16 19:32:59.000000 mypy_boto3_mediapackagev2-1.34.85/setup.py
```

### Comparing `mypy-boto3-mediapackagev2-1.34.60/LICENSE` & `mypy_boto3_mediapackagev2-1.34.85/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackagev2-1.34.60/PKG-INFO` & `mypy_boto3_mediapackagev2-1.34.85/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mediapackagev2
-Version: 1.34.60
-Summary: Type annotations for boto3.mediapackagev2 1.34.60 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.85
+Summary: Type annotations for boto3.mediapackagev2 1.34.85 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediapackagev2.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediapackagev2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mediapackagev2)](https://pepy.tech/project/mypy-boto3-mediapackagev2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.mediapackagev2 1.34.60](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2)
+[boto3.mediapackagev2 1.34.85](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -311,18 +311,18 @@
 `mypy_boto3_mediapackagev2.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
 Full list of `mediapackagev2` Literals can be found in
 [docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2/literals/).
 
 ```python
-from mypy_boto3_mediapackagev2.literals import AdMarkerHlsType
+from mypy_boto3_mediapackagev2.literals import AdMarkerDashType
 
 
-def check_value(value: AdMarkerHlsType) -> bool: ...
+def check_value(value: AdMarkerDashType) -> bool: ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `mypy_boto3_mediapackagev2.type_defs` module contains structures and shapes
```

### Comparing `mypy-boto3-mediapackagev2-1.34.60/README.md` & `mypy_boto3_mediapackagev2-1.34.85/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediapackagev2.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediapackagev2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mediapackagev2)](https://pepy.tech/project/mypy-boto3-mediapackagev2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.mediapackagev2 1.34.60](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2)
+[boto3.mediapackagev2 1.34.85](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -278,18 +278,18 @@
 `mypy_boto3_mediapackagev2.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
 Full list of `mediapackagev2` Literals can be found in
 [docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2/literals/).
 
 ```python
-from mypy_boto3_mediapackagev2.literals import AdMarkerHlsType
+from mypy_boto3_mediapackagev2.literals import AdMarkerDashType
 
 
-def check_value(value: AdMarkerHlsType) -> bool: ...
+def check_value(value: AdMarkerDashType) -> bool: ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `mypy_boto3_mediapackagev2.type_defs` module contains structures and shapes
```

### Comparing `mypy-boto3-mediapackagev2-1.34.60/mypy_boto3_mediapackagev2/__init__.py` & `mypy_boto3_mediapackagev2-1.34.85/mypy_boto3_mediapackagev2/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackagev2-1.34.60/mypy_boto3_mediapackagev2/__init__.pyi` & `mypy_boto3_mediapackagev2-1.34.85/mypy_boto3_mediapackagev2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackagev2-1.34.60/mypy_boto3_mediapackagev2/__main__.py` & `mypy_boto3_mediapackagev2-1.34.85/mypy_boto3_mediapackagev2/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.mediapackagev2 1.34.60\n"
-        "Version:         1.34.60\n"
+        "Type annotations for boto3.mediapackagev2 1.34.85\n"
+        "Version:         1.34.85\n"
         "Builder version: 7.23.2\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.60")
+    print("1.34.85")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-mediapackagev2-1.34.60/mypy_boto3_mediapackagev2/client.py` & `mypy_boto3_mediapackagev2-1.34.85/mypy_boto3_mediapackagev2/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     ListChannelGroupsPaginator,
     ListChannelsPaginator,
     ListOriginEndpointsPaginator,
 )
 from .type_defs import (
     CreateChannelGroupResponseTypeDef,
     CreateChannelResponseTypeDef,
+    CreateDashManifestConfigurationTypeDef,
     CreateHlsManifestConfigurationTypeDef,
     CreateLowLatencyHlsManifestConfigurationTypeDef,
     CreateOriginEndpointResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetChannelGroupResponseTypeDef,
     GetChannelPolicyResponseTypeDef,
     GetChannelResponseTypeDef,
@@ -147,14 +148,15 @@
         ContainerType: ContainerTypeType,
         Segment: SegmentTypeDef = ...,
         ClientToken: str = ...,
         Description: str = ...,
         StartoverWindowSeconds: int = ...,
         HlsManifests: Sequence[CreateHlsManifestConfigurationTypeDef] = ...,
         LowLatencyHlsManifests: Sequence[CreateLowLatencyHlsManifestConfigurationTypeDef] = ...,
+        DashManifests: Sequence[CreateDashManifestConfigurationTypeDef] = ...,
         Tags: Mapping[str, str] = ...,
     ) -> CreateOriginEndpointResponseTypeDef:
         """
         The endpoint is attached to a channel, and represents the output of the live
         content.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2.Client.create_origin_endpoint)
@@ -395,14 +397,15 @@
         OriginEndpointName: str,
         ContainerType: ContainerTypeType,
         Segment: SegmentTypeDef = ...,
         Description: str = ...,
         StartoverWindowSeconds: int = ...,
         HlsManifests: Sequence[CreateHlsManifestConfigurationTypeDef] = ...,
         LowLatencyHlsManifests: Sequence[CreateLowLatencyHlsManifestConfigurationTypeDef] = ...,
+        DashManifests: Sequence[CreateDashManifestConfigurationTypeDef] = ...,
         ETag: str = ...,
     ) -> UpdateOriginEndpointResponseTypeDef:
         """
         Update the specified origin endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2.Client.update_origin_endpoint)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2/client/#update_origin_endpoint)
```

### Comparing `mypy-boto3-mediapackagev2-1.34.60/mypy_boto3_mediapackagev2/client.pyi` & `mypy_boto3_mediapackagev2-1.34.85/mypy_boto3_mediapackagev2/client.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     ListChannelGroupsPaginator,
     ListChannelsPaginator,
     ListOriginEndpointsPaginator,
 )
 from .type_defs import (
     CreateChannelGroupResponseTypeDef,
     CreateChannelResponseTypeDef,
+    CreateDashManifestConfigurationTypeDef,
     CreateHlsManifestConfigurationTypeDef,
     CreateLowLatencyHlsManifestConfigurationTypeDef,
     CreateOriginEndpointResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetChannelGroupResponseTypeDef,
     GetChannelPolicyResponseTypeDef,
     GetChannelResponseTypeDef,
@@ -144,14 +145,15 @@
         ContainerType: ContainerTypeType,
         Segment: SegmentTypeDef = ...,
         ClientToken: str = ...,
         Description: str = ...,
         StartoverWindowSeconds: int = ...,
         HlsManifests: Sequence[CreateHlsManifestConfigurationTypeDef] = ...,
         LowLatencyHlsManifests: Sequence[CreateLowLatencyHlsManifestConfigurationTypeDef] = ...,
+        DashManifests: Sequence[CreateDashManifestConfigurationTypeDef] = ...,
         Tags: Mapping[str, str] = ...,
     ) -> CreateOriginEndpointResponseTypeDef:
         """
         The endpoint is attached to a channel, and represents the output of the live
         content.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2.Client.create_origin_endpoint)
@@ -392,14 +394,15 @@
         OriginEndpointName: str,
         ContainerType: ContainerTypeType,
         Segment: SegmentTypeDef = ...,
         Description: str = ...,
         StartoverWindowSeconds: int = ...,
         HlsManifests: Sequence[CreateHlsManifestConfigurationTypeDef] = ...,
         LowLatencyHlsManifests: Sequence[CreateLowLatencyHlsManifestConfigurationTypeDef] = ...,
+        DashManifests: Sequence[CreateDashManifestConfigurationTypeDef] = ...,
         ETag: str = ...,
     ) -> UpdateOriginEndpointResponseTypeDef:
         """
         Update the specified origin endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2.Client.update_origin_endpoint)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2/client/#update_origin_endpoint)
```

### Comparing `mypy-boto3-mediapackagev2-1.34.60/mypy_boto3_mediapackagev2/literals.py` & `mypy_boto3_mediapackagev2-1.34.85/mypy_boto3_mediapackagev2/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,31 +2,36 @@
 Type annotations for mediapackagev2 service literal definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2/literals/)
 
 Usage::
 
     ```python
-    from mypy_boto3_mediapackagev2.literals import AdMarkerHlsType
+    from mypy_boto3_mediapackagev2.literals import AdMarkerDashType
 
-    data: AdMarkerHlsType = "DATERANGE"
+    data: AdMarkerDashType = "BINARY"
     ```
 """
 
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = (
+    "AdMarkerDashType",
     "AdMarkerHlsType",
     "CmafEncryptionMethodType",
     "ContainerTypeType",
+    "DashDrmSignalingType",
+    "DashPeriodTriggerType",
+    "DashSegmentTemplateFormatType",
+    "DashUtcTimingModeType",
     "DrmSystemType",
     "ListChannelGroupsPaginatorName",
     "ListChannelsPaginatorName",
     "ListOriginEndpointsPaginatorName",
     "PresetSpeke20AudioType",
     "PresetSpeke20VideoType",
     "ScteFilterType",
@@ -34,17 +39,24 @@
     "mediapackagev2ServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+AdMarkerDashType = Literal["BINARY", "XML"]
 AdMarkerHlsType = Literal["DATERANGE"]
 CmafEncryptionMethodType = Literal["CBCS", "CENC"]
 ContainerTypeType = Literal["CMAF", "TS"]
+DashDrmSignalingType = Literal["INDIVIDUAL", "REFERENCED"]
+DashPeriodTriggerType = Literal[
+    "AVAILS", "DRM_KEY_ROTATION", "NONE", "SOURCE_CHANGES", "SOURCE_DISRUPTIONS"
+]
+DashSegmentTemplateFormatType = Literal["NUMBER_WITH_TIMELINE"]
+DashUtcTimingModeType = Literal["HTTP_HEAD", "HTTP_ISO", "HTTP_XSDATE", "UTC_DIRECT"]
 DrmSystemType = Literal["CLEAR_KEY_AES_128", "FAIRPLAY", "PLAYREADY", "WIDEVINE"]
 ListChannelGroupsPaginatorName = Literal["list_channel_groups"]
 ListChannelsPaginatorName = Literal["list_channels"]
 ListOriginEndpointsPaginatorName = Literal["list_origin_endpoints"]
 PresetSpeke20AudioType = Literal[
     "PRESET_AUDIO_1", "PRESET_AUDIO_2", "PRESET_AUDIO_3", "SHARED", "UNENCRYPTED"
 ]
@@ -140,14 +152,15 @@
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
@@ -160,24 +173,26 @@
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
@@ -238,15 +253,14 @@
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
@@ -426,14 +440,15 @@
     "sts",
     "supplychain",
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
```

### Comparing `mypy-boto3-mediapackagev2-1.34.60/mypy_boto3_mediapackagev2/literals.pyi` & `mypy_boto3_mediapackagev2-1.34.85/mypy_boto3_mediapackagev2/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -2,31 +2,36 @@
 Type annotations for mediapackagev2 service literal definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2/literals/)
 
 Usage::
 
     ```python
-    from mypy_boto3_mediapackagev2.literals import AdMarkerHlsType
+    from mypy_boto3_mediapackagev2.literals import AdMarkerDashType
 
-    data: AdMarkerHlsType = "DATERANGE"
+    data: AdMarkerDashType = "BINARY"
     ```
 """
 
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = (
+    "AdMarkerDashType",
     "AdMarkerHlsType",
     "CmafEncryptionMethodType",
     "ContainerTypeType",
+    "DashDrmSignalingType",
+    "DashPeriodTriggerType",
+    "DashSegmentTemplateFormatType",
+    "DashUtcTimingModeType",
     "DrmSystemType",
     "ListChannelGroupsPaginatorName",
     "ListChannelsPaginatorName",
     "ListOriginEndpointsPaginatorName",
     "PresetSpeke20AudioType",
     "PresetSpeke20VideoType",
     "ScteFilterType",
@@ -34,17 +39,24 @@
     "mediapackagev2ServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+AdMarkerDashType = Literal["BINARY", "XML"]
 AdMarkerHlsType = Literal["DATERANGE"]
 CmafEncryptionMethodType = Literal["CBCS", "CENC"]
 ContainerTypeType = Literal["CMAF", "TS"]
+DashDrmSignalingType = Literal["INDIVIDUAL", "REFERENCED"]
+DashPeriodTriggerType = Literal[
+    "AVAILS", "DRM_KEY_ROTATION", "NONE", "SOURCE_CHANGES", "SOURCE_DISRUPTIONS"
+]
+DashSegmentTemplateFormatType = Literal["NUMBER_WITH_TIMELINE"]
+DashUtcTimingModeType = Literal["HTTP_HEAD", "HTTP_ISO", "HTTP_XSDATE", "UTC_DIRECT"]
 DrmSystemType = Literal["CLEAR_KEY_AES_128", "FAIRPLAY", "PLAYREADY", "WIDEVINE"]
 ListChannelGroupsPaginatorName = Literal["list_channel_groups"]
 ListChannelsPaginatorName = Literal["list_channels"]
 ListOriginEndpointsPaginatorName = Literal["list_origin_endpoints"]
 PresetSpeke20AudioType = Literal[
     "PRESET_AUDIO_1", "PRESET_AUDIO_2", "PRESET_AUDIO_3", "SHARED", "UNENCRYPTED"
 ]
@@ -140,14 +152,15 @@
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
@@ -160,24 +173,26 @@
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
@@ -238,15 +253,14 @@
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
@@ -426,14 +440,15 @@
     "sts",
     "supplychain",
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
```

### Comparing `mypy-boto3-mediapackagev2-1.34.60/mypy_boto3_mediapackagev2/paginator.py` & `mypy_boto3_mediapackagev2-1.34.85/mypy_boto3_mediapackagev2/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackagev2-1.34.60/mypy_boto3_mediapackagev2/paginator.pyi` & `mypy_boto3_mediapackagev2-1.34.85/mypy_boto3_mediapackagev2/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackagev2-1.34.60/mypy_boto3_mediapackagev2/type_defs.py` & `mypy_boto3_mediapackagev2-1.34.85/mypy_boto3_mediapackagev2/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,16 +13,20 @@
 """
 
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
+    AdMarkerDashType,
     CmafEncryptionMethodType,
     ContainerTypeType,
+    DashDrmSignalingType,
+    DashPeriodTriggerType,
+    DashUtcTimingModeType,
     DrmSystemType,
     PresetSpeke20AudioType,
     PresetSpeke20VideoType,
     ScteFilterType,
     TsEncryptionMethodType,
 )
 
@@ -42,14 +46,16 @@
 __all__ = (
     "ChannelGroupListConfigurationTypeDef",
     "ChannelListConfigurationTypeDef",
     "CreateChannelGroupRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "CreateChannelRequestRequestTypeDef",
     "IngestEndpointTypeDef",
+    "DashUtcTimingTypeDef",
+    "ScteDashTypeDef",
     "ScteHlsTypeDef",
     "DeleteChannelGroupRequestRequestTypeDef",
     "DeleteChannelPolicyRequestRequestTypeDef",
     "DeleteChannelRequestRequestTypeDef",
     "DeleteOriginEndpointPolicyRequestRequestTypeDef",
     "DeleteOriginEndpointRequestRequestTypeDef",
     "EncryptionContractConfigurationTypeDef",
@@ -59,14 +65,15 @@
     "GetChannelPolicyRequestRequestTypeDef",
     "GetChannelRequestRequestTypeDef",
     "GetOriginEndpointPolicyRequestRequestTypeDef",
     "GetOriginEndpointRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "ListChannelGroupsRequestRequestTypeDef",
     "ListChannelsRequestRequestTypeDef",
+    "ListDashManifestConfigurationTypeDef",
     "ListHlsManifestConfigurationTypeDef",
     "ListLowLatencyHlsManifestConfigurationTypeDef",
     "ListOriginEndpointsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "PutChannelPolicyRequestRequestTypeDef",
     "PutOriginEndpointPolicyRequestRequestTypeDef",
     "ScteTypeDef",
@@ -89,16 +96,18 @@
     "SpekeKeyProviderTypeDef",
     "FilterConfigurationTypeDef",
     "ListChannelGroupsRequestListChannelGroupsPaginateTypeDef",
     "ListChannelsRequestListChannelsPaginateTypeDef",
     "ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef",
     "OriginEndpointListConfigurationTypeDef",
     "EncryptionTypeDef",
+    "CreateDashManifestConfigurationTypeDef",
     "CreateHlsManifestConfigurationTypeDef",
     "CreateLowLatencyHlsManifestConfigurationTypeDef",
+    "GetDashManifestConfigurationTypeDef",
     "GetHlsManifestConfigurationTypeDef",
     "GetLowLatencyHlsManifestConfigurationTypeDef",
     "ListOriginEndpointsResponseTypeDef",
     "SegmentTypeDef",
     "CreateOriginEndpointRequestRequestTypeDef",
     "CreateOriginEndpointResponseTypeDef",
     "GetOriginEndpointResponseTypeDef",
@@ -159,14 +168,27 @@
 IngestEndpointTypeDef = TypedDict(
     "IngestEndpointTypeDef",
     {
         "Id": NotRequired[str],
         "Url": NotRequired[str],
     },
 )
+DashUtcTimingTypeDef = TypedDict(
+    "DashUtcTimingTypeDef",
+    {
+        "TimingMode": NotRequired[DashUtcTimingModeType],
+        "TimingSource": NotRequired[str],
+    },
+)
+ScteDashTypeDef = TypedDict(
+    "ScteDashTypeDef",
+    {
+        "AdMarkerDash": NotRequired[AdMarkerDashType],
+    },
+)
 ScteHlsTypeDef = TypedDict(
     "ScteHlsTypeDef",
     {
         "AdMarkerHls": NotRequired[Literal["DATERANGE"]],
     },
 )
 DeleteChannelGroupRequestRequestTypeDef = TypedDict(
@@ -275,14 +297,21 @@
     "ListChannelsRequestRequestTypeDef",
     {
         "ChannelGroupName": str,
         "MaxResults": NotRequired[int],
         "NextToken": NotRequired[str],
     },
 )
+ListDashManifestConfigurationTypeDef = TypedDict(
+    "ListDashManifestConfigurationTypeDef",
+    {
+        "ManifestName": str,
+        "Url": NotRequired[str],
+    },
+)
 ListHlsManifestConfigurationTypeDef = TypedDict(
     "ListHlsManifestConfigurationTypeDef",
     {
         "ManifestName": str,
         "ChildManifestName": NotRequired[str],
         "Url": NotRequired[str],
     },
@@ -548,25 +577,42 @@
         "OriginEndpointName": str,
         "ContainerType": ContainerTypeType,
         "Description": NotRequired[str],
         "CreatedAt": NotRequired[datetime],
         "ModifiedAt": NotRequired[datetime],
         "HlsManifests": NotRequired[List[ListHlsManifestConfigurationTypeDef]],
         "LowLatencyHlsManifests": NotRequired[List[ListLowLatencyHlsManifestConfigurationTypeDef]],
+        "DashManifests": NotRequired[List[ListDashManifestConfigurationTypeDef]],
     },
 )
 EncryptionTypeDef = TypedDict(
     "EncryptionTypeDef",
     {
         "EncryptionMethod": EncryptionMethodTypeDef,
         "SpekeKeyProvider": SpekeKeyProviderTypeDef,
         "ConstantInitializationVector": NotRequired[str],
         "KeyRotationIntervalSeconds": NotRequired[int],
     },
 )
+CreateDashManifestConfigurationTypeDef = TypedDict(
+    "CreateDashManifestConfigurationTypeDef",
+    {
+        "ManifestName": str,
+        "ManifestWindowSeconds": NotRequired[int],
+        "FilterConfiguration": NotRequired[FilterConfigurationTypeDef],
+        "MinUpdatePeriodSeconds": NotRequired[int],
+        "MinBufferTimeSeconds": NotRequired[int],
+        "SuggestedPresentationDelaySeconds": NotRequired[int],
+        "SegmentTemplateFormat": NotRequired[Literal["NUMBER_WITH_TIMELINE"]],
+        "PeriodTriggers": NotRequired[Sequence[DashPeriodTriggerType]],
+        "ScteDash": NotRequired[ScteDashTypeDef],
+        "DrmSignaling": NotRequired[DashDrmSignalingType],
+        "UtcTiming": NotRequired[DashUtcTimingTypeDef],
+    },
+)
 CreateHlsManifestConfigurationTypeDef = TypedDict(
     "CreateHlsManifestConfigurationTypeDef",
     {
         "ManifestName": str,
         "ChildManifestName": NotRequired[str],
         "ScteHls": NotRequired[ScteHlsTypeDef],
         "ManifestWindowSeconds": NotRequired[int],
@@ -581,14 +627,31 @@
         "ChildManifestName": NotRequired[str],
         "ScteHls": NotRequired[ScteHlsTypeDef],
         "ManifestWindowSeconds": NotRequired[int],
         "ProgramDateTimeIntervalSeconds": NotRequired[int],
         "FilterConfiguration": NotRequired[FilterConfigurationTypeDef],
     },
 )
+GetDashManifestConfigurationTypeDef = TypedDict(
+    "GetDashManifestConfigurationTypeDef",
+    {
+        "ManifestName": str,
+        "Url": str,
+        "ManifestWindowSeconds": NotRequired[int],
+        "FilterConfiguration": NotRequired[FilterConfigurationTypeDef],
+        "MinUpdatePeriodSeconds": NotRequired[int],
+        "MinBufferTimeSeconds": NotRequired[int],
+        "SuggestedPresentationDelaySeconds": NotRequired[int],
+        "SegmentTemplateFormat": NotRequired[Literal["NUMBER_WITH_TIMELINE"]],
+        "PeriodTriggers": NotRequired[List[DashPeriodTriggerType]],
+        "ScteDash": NotRequired[ScteDashTypeDef],
+        "DrmSignaling": NotRequired[DashDrmSignalingType],
+        "UtcTiming": NotRequired[DashUtcTimingTypeDef],
+    },
+)
 GetHlsManifestConfigurationTypeDef = TypedDict(
     "GetHlsManifestConfigurationTypeDef",
     {
         "ManifestName": str,
         "Url": str,
         "ChildManifestName": NotRequired[str],
         "ManifestWindowSeconds": NotRequired[int],
@@ -640,14 +703,15 @@
         "ClientToken": NotRequired[str],
         "Description": NotRequired[str],
         "StartoverWindowSeconds": NotRequired[int],
         "HlsManifests": NotRequired[Sequence[CreateHlsManifestConfigurationTypeDef]],
         "LowLatencyHlsManifests": NotRequired[
             Sequence[CreateLowLatencyHlsManifestConfigurationTypeDef]
         ],
+        "DashManifests": NotRequired[Sequence[CreateDashManifestConfigurationTypeDef]],
         "Tags": NotRequired[Mapping[str, str]],
     },
 )
 CreateOriginEndpointResponseTypeDef = TypedDict(
     "CreateOriginEndpointResponseTypeDef",
     {
         "Arn": str,
@@ -658,14 +722,15 @@
         "Segment": SegmentTypeDef,
         "CreatedAt": datetime,
         "ModifiedAt": datetime,
         "Description": str,
         "StartoverWindowSeconds": int,
         "HlsManifests": List[GetHlsManifestConfigurationTypeDef],
         "LowLatencyHlsManifests": List[GetLowLatencyHlsManifestConfigurationTypeDef],
+        "DashManifests": List[GetDashManifestConfigurationTypeDef],
         "ETag": str,
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 GetOriginEndpointResponseTypeDef = TypedDict(
     "GetOriginEndpointResponseTypeDef",
@@ -680,14 +745,15 @@
         "ModifiedAt": datetime,
         "Description": str,
         "StartoverWindowSeconds": int,
         "HlsManifests": List[GetHlsManifestConfigurationTypeDef],
         "LowLatencyHlsManifests": List[GetLowLatencyHlsManifestConfigurationTypeDef],
         "ETag": str,
         "Tags": Dict[str, str],
+        "DashManifests": List[GetDashManifestConfigurationTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 UpdateOriginEndpointRequestRequestTypeDef = TypedDict(
     "UpdateOriginEndpointRequestRequestTypeDef",
     {
         "ChannelGroupName": str,
@@ -697,14 +763,15 @@
         "Segment": NotRequired[SegmentTypeDef],
         "Description": NotRequired[str],
         "StartoverWindowSeconds": NotRequired[int],
         "HlsManifests": NotRequired[Sequence[CreateHlsManifestConfigurationTypeDef]],
         "LowLatencyHlsManifests": NotRequired[
             Sequence[CreateLowLatencyHlsManifestConfigurationTypeDef]
         ],
+        "DashManifests": NotRequired[Sequence[CreateDashManifestConfigurationTypeDef]],
         "ETag": NotRequired[str],
     },
 )
 UpdateOriginEndpointResponseTypeDef = TypedDict(
     "UpdateOriginEndpointResponseTypeDef",
     {
         "Arn": str,
@@ -717,10 +784,11 @@
         "ModifiedAt": datetime,
         "Description": str,
         "StartoverWindowSeconds": int,
         "HlsManifests": List[GetHlsManifestConfigurationTypeDef],
         "LowLatencyHlsManifests": List[GetLowLatencyHlsManifestConfigurationTypeDef],
         "ETag": str,
         "Tags": Dict[str, str],
+        "DashManifests": List[GetDashManifestConfigurationTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-mediapackagev2-1.34.60/mypy_boto3_mediapackagev2/type_defs.pyi` & `mypy_boto3_mediapackagev2-1.34.85/mypy_boto3_mediapackagev2/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -13,16 +13,20 @@
 """
 
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
+    AdMarkerDashType,
     CmafEncryptionMethodType,
     ContainerTypeType,
+    DashDrmSignalingType,
+    DashPeriodTriggerType,
+    DashUtcTimingModeType,
     DrmSystemType,
     PresetSpeke20AudioType,
     PresetSpeke20VideoType,
     ScteFilterType,
     TsEncryptionMethodType,
 )
 
@@ -42,14 +46,16 @@
 __all__ = (
     "ChannelGroupListConfigurationTypeDef",
     "ChannelListConfigurationTypeDef",
     "CreateChannelGroupRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "CreateChannelRequestRequestTypeDef",
     "IngestEndpointTypeDef",
+    "DashUtcTimingTypeDef",
+    "ScteDashTypeDef",
     "ScteHlsTypeDef",
     "DeleteChannelGroupRequestRequestTypeDef",
     "DeleteChannelPolicyRequestRequestTypeDef",
     "DeleteChannelRequestRequestTypeDef",
     "DeleteOriginEndpointPolicyRequestRequestTypeDef",
     "DeleteOriginEndpointRequestRequestTypeDef",
     "EncryptionContractConfigurationTypeDef",
@@ -59,14 +65,15 @@
     "GetChannelPolicyRequestRequestTypeDef",
     "GetChannelRequestRequestTypeDef",
     "GetOriginEndpointPolicyRequestRequestTypeDef",
     "GetOriginEndpointRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "ListChannelGroupsRequestRequestTypeDef",
     "ListChannelsRequestRequestTypeDef",
+    "ListDashManifestConfigurationTypeDef",
     "ListHlsManifestConfigurationTypeDef",
     "ListLowLatencyHlsManifestConfigurationTypeDef",
     "ListOriginEndpointsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "PutChannelPolicyRequestRequestTypeDef",
     "PutOriginEndpointPolicyRequestRequestTypeDef",
     "ScteTypeDef",
@@ -89,16 +96,18 @@
     "SpekeKeyProviderTypeDef",
     "FilterConfigurationTypeDef",
     "ListChannelGroupsRequestListChannelGroupsPaginateTypeDef",
     "ListChannelsRequestListChannelsPaginateTypeDef",
     "ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef",
     "OriginEndpointListConfigurationTypeDef",
     "EncryptionTypeDef",
+    "CreateDashManifestConfigurationTypeDef",
     "CreateHlsManifestConfigurationTypeDef",
     "CreateLowLatencyHlsManifestConfigurationTypeDef",
+    "GetDashManifestConfigurationTypeDef",
     "GetHlsManifestConfigurationTypeDef",
     "GetLowLatencyHlsManifestConfigurationTypeDef",
     "ListOriginEndpointsResponseTypeDef",
     "SegmentTypeDef",
     "CreateOriginEndpointRequestRequestTypeDef",
     "CreateOriginEndpointResponseTypeDef",
     "GetOriginEndpointResponseTypeDef",
@@ -159,14 +168,27 @@
 IngestEndpointTypeDef = TypedDict(
     "IngestEndpointTypeDef",
     {
         "Id": NotRequired[str],
         "Url": NotRequired[str],
     },
 )
+DashUtcTimingTypeDef = TypedDict(
+    "DashUtcTimingTypeDef",
+    {
+        "TimingMode": NotRequired[DashUtcTimingModeType],
+        "TimingSource": NotRequired[str],
+    },
+)
+ScteDashTypeDef = TypedDict(
+    "ScteDashTypeDef",
+    {
+        "AdMarkerDash": NotRequired[AdMarkerDashType],
+    },
+)
 ScteHlsTypeDef = TypedDict(
     "ScteHlsTypeDef",
     {
         "AdMarkerHls": NotRequired[Literal["DATERANGE"]],
     },
 )
 DeleteChannelGroupRequestRequestTypeDef = TypedDict(
@@ -275,14 +297,21 @@
     "ListChannelsRequestRequestTypeDef",
     {
         "ChannelGroupName": str,
         "MaxResults": NotRequired[int],
         "NextToken": NotRequired[str],
     },
 )
+ListDashManifestConfigurationTypeDef = TypedDict(
+    "ListDashManifestConfigurationTypeDef",
+    {
+        "ManifestName": str,
+        "Url": NotRequired[str],
+    },
+)
 ListHlsManifestConfigurationTypeDef = TypedDict(
     "ListHlsManifestConfigurationTypeDef",
     {
         "ManifestName": str,
         "ChildManifestName": NotRequired[str],
         "Url": NotRequired[str],
     },
@@ -548,25 +577,42 @@
         "OriginEndpointName": str,
         "ContainerType": ContainerTypeType,
         "Description": NotRequired[str],
         "CreatedAt": NotRequired[datetime],
         "ModifiedAt": NotRequired[datetime],
         "HlsManifests": NotRequired[List[ListHlsManifestConfigurationTypeDef]],
         "LowLatencyHlsManifests": NotRequired[List[ListLowLatencyHlsManifestConfigurationTypeDef]],
+        "DashManifests": NotRequired[List[ListDashManifestConfigurationTypeDef]],
     },
 )
 EncryptionTypeDef = TypedDict(
     "EncryptionTypeDef",
     {
         "EncryptionMethod": EncryptionMethodTypeDef,
         "SpekeKeyProvider": SpekeKeyProviderTypeDef,
         "ConstantInitializationVector": NotRequired[str],
         "KeyRotationIntervalSeconds": NotRequired[int],
     },
 )
+CreateDashManifestConfigurationTypeDef = TypedDict(
+    "CreateDashManifestConfigurationTypeDef",
+    {
+        "ManifestName": str,
+        "ManifestWindowSeconds": NotRequired[int],
+        "FilterConfiguration": NotRequired[FilterConfigurationTypeDef],
+        "MinUpdatePeriodSeconds": NotRequired[int],
+        "MinBufferTimeSeconds": NotRequired[int],
+        "SuggestedPresentationDelaySeconds": NotRequired[int],
+        "SegmentTemplateFormat": NotRequired[Literal["NUMBER_WITH_TIMELINE"]],
+        "PeriodTriggers": NotRequired[Sequence[DashPeriodTriggerType]],
+        "ScteDash": NotRequired[ScteDashTypeDef],
+        "DrmSignaling": NotRequired[DashDrmSignalingType],
+        "UtcTiming": NotRequired[DashUtcTimingTypeDef],
+    },
+)
 CreateHlsManifestConfigurationTypeDef = TypedDict(
     "CreateHlsManifestConfigurationTypeDef",
     {
         "ManifestName": str,
         "ChildManifestName": NotRequired[str],
         "ScteHls": NotRequired[ScteHlsTypeDef],
         "ManifestWindowSeconds": NotRequired[int],
@@ -581,14 +627,31 @@
         "ChildManifestName": NotRequired[str],
         "ScteHls": NotRequired[ScteHlsTypeDef],
         "ManifestWindowSeconds": NotRequired[int],
         "ProgramDateTimeIntervalSeconds": NotRequired[int],
         "FilterConfiguration": NotRequired[FilterConfigurationTypeDef],
     },
 )
+GetDashManifestConfigurationTypeDef = TypedDict(
+    "GetDashManifestConfigurationTypeDef",
+    {
+        "ManifestName": str,
+        "Url": str,
+        "ManifestWindowSeconds": NotRequired[int],
+        "FilterConfiguration": NotRequired[FilterConfigurationTypeDef],
+        "MinUpdatePeriodSeconds": NotRequired[int],
+        "MinBufferTimeSeconds": NotRequired[int],
+        "SuggestedPresentationDelaySeconds": NotRequired[int],
+        "SegmentTemplateFormat": NotRequired[Literal["NUMBER_WITH_TIMELINE"]],
+        "PeriodTriggers": NotRequired[List[DashPeriodTriggerType]],
+        "ScteDash": NotRequired[ScteDashTypeDef],
+        "DrmSignaling": NotRequired[DashDrmSignalingType],
+        "UtcTiming": NotRequired[DashUtcTimingTypeDef],
+    },
+)
 GetHlsManifestConfigurationTypeDef = TypedDict(
     "GetHlsManifestConfigurationTypeDef",
     {
         "ManifestName": str,
         "Url": str,
         "ChildManifestName": NotRequired[str],
         "ManifestWindowSeconds": NotRequired[int],
@@ -640,14 +703,15 @@
         "ClientToken": NotRequired[str],
         "Description": NotRequired[str],
         "StartoverWindowSeconds": NotRequired[int],
         "HlsManifests": NotRequired[Sequence[CreateHlsManifestConfigurationTypeDef]],
         "LowLatencyHlsManifests": NotRequired[
             Sequence[CreateLowLatencyHlsManifestConfigurationTypeDef]
         ],
+        "DashManifests": NotRequired[Sequence[CreateDashManifestConfigurationTypeDef]],
         "Tags": NotRequired[Mapping[str, str]],
     },
 )
 CreateOriginEndpointResponseTypeDef = TypedDict(
     "CreateOriginEndpointResponseTypeDef",
     {
         "Arn": str,
@@ -658,14 +722,15 @@
         "Segment": SegmentTypeDef,
         "CreatedAt": datetime,
         "ModifiedAt": datetime,
         "Description": str,
         "StartoverWindowSeconds": int,
         "HlsManifests": List[GetHlsManifestConfigurationTypeDef],
         "LowLatencyHlsManifests": List[GetLowLatencyHlsManifestConfigurationTypeDef],
+        "DashManifests": List[GetDashManifestConfigurationTypeDef],
         "ETag": str,
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 GetOriginEndpointResponseTypeDef = TypedDict(
     "GetOriginEndpointResponseTypeDef",
@@ -680,14 +745,15 @@
         "ModifiedAt": datetime,
         "Description": str,
         "StartoverWindowSeconds": int,
         "HlsManifests": List[GetHlsManifestConfigurationTypeDef],
         "LowLatencyHlsManifests": List[GetLowLatencyHlsManifestConfigurationTypeDef],
         "ETag": str,
         "Tags": Dict[str, str],
+        "DashManifests": List[GetDashManifestConfigurationTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 UpdateOriginEndpointRequestRequestTypeDef = TypedDict(
     "UpdateOriginEndpointRequestRequestTypeDef",
     {
         "ChannelGroupName": str,
@@ -697,14 +763,15 @@
         "Segment": NotRequired[SegmentTypeDef],
         "Description": NotRequired[str],
         "StartoverWindowSeconds": NotRequired[int],
         "HlsManifests": NotRequired[Sequence[CreateHlsManifestConfigurationTypeDef]],
         "LowLatencyHlsManifests": NotRequired[
             Sequence[CreateLowLatencyHlsManifestConfigurationTypeDef]
         ],
+        "DashManifests": NotRequired[Sequence[CreateDashManifestConfigurationTypeDef]],
         "ETag": NotRequired[str],
     },
 )
 UpdateOriginEndpointResponseTypeDef = TypedDict(
     "UpdateOriginEndpointResponseTypeDef",
     {
         "Arn": str,
@@ -717,10 +784,11 @@
         "ModifiedAt": datetime,
         "Description": str,
         "StartoverWindowSeconds": int,
         "HlsManifests": List[GetHlsManifestConfigurationTypeDef],
         "LowLatencyHlsManifests": List[GetLowLatencyHlsManifestConfigurationTypeDef],
         "ETag": str,
         "Tags": Dict[str, str],
+        "DashManifests": List[GetDashManifestConfigurationTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-mediapackagev2-1.34.60/mypy_boto3_mediapackagev2.egg-info/PKG-INFO` & `mypy_boto3_mediapackagev2-1.34.85/mypy_boto3_mediapackagev2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mediapackagev2
-Version: 1.34.60
-Summary: Type annotations for boto3.mediapackagev2 1.34.60 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.85
+Summary: Type annotations for boto3.mediapackagev2 1.34.85 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediapackagev2.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediapackagev2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mediapackagev2)](https://pepy.tech/project/mypy-boto3-mediapackagev2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.mediapackagev2 1.34.60](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2)
+[boto3.mediapackagev2 1.34.85](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -311,18 +311,18 @@
 `mypy_boto3_mediapackagev2.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
 Full list of `mediapackagev2` Literals can be found in
 [docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2/literals/).
 
 ```python
-from mypy_boto3_mediapackagev2.literals import AdMarkerHlsType
+from mypy_boto3_mediapackagev2.literals import AdMarkerDashType
 
 
-def check_value(value: AdMarkerHlsType) -> bool: ...
+def check_value(value: AdMarkerDashType) -> bool: ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `mypy_boto3_mediapackagev2.type_defs` module contains structures and shapes
```

### Comparing `mypy-boto3-mediapackagev2-1.34.60/mypy_boto3_mediapackagev2.egg-info/SOURCES.txt` & `mypy_boto3_mediapackagev2-1.34.85/mypy_boto3_mediapackagev2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackagev2-1.34.60/setup.py` & `mypy_boto3_mediapackagev2-1.34.85/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-mediapackagev2",
-    version="1.34.60",
+    version="1.34.85",
     packages=["mypy_boto3_mediapackagev2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.mediapackagev2 1.34.60 service generated with mypy-boto3-builder 7.23.2",
+    description="Type annotations for boto3.mediapackagev2 1.34.85 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

