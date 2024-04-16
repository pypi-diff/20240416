# Comparing `tmp/mypy-boto3-lakeformation-1.34.7.tar.gz` & `tmp/mypy_boto3_lakeformation-1.34.85.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-lakeformation-1.34.7.tar", last modified: Fri Dec 22 20:32:30 2023, max compression
+gzip compressed data, was "mypy_boto3_lakeformation-1.34.85.tar", last modified: Tue Apr 16 19:33:15 2024, max compression
```

## Comparing `mypy-boto3-lakeformation-1.34.7.tar` & `mypy_boto3_lakeformation-1.34.85.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 20:32:30.660719 mypy-boto3-lakeformation-1.34.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-22 20:32:09.000000 mypy-boto3-lakeformation-1.34.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13549 2023-12-22 20:32:30.660719 mypy-boto3-lakeformation-1.34.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12037 2023-12-22 20:32:09.000000 mypy-boto3-lakeformation-1.34.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 20:32:30.660719 mypy-boto3-lakeformation-1.34.7/mypy_boto3_lakeformation/
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2023-12-22 20:32:09.000000 mypy-boto3-lakeformation-1.34.7/mypy_boto3_lakeformation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2023-12-22 20:32:09.000000 mypy-boto3-lakeformation-1.34.7/mypy_boto3_lakeformation/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      929 2023-12-22 20:32:09.000000 mypy-boto3-lakeformation-1.34.7/mypy_boto3_lakeformation/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    42494 2023-12-22 20:32:10.000000 mypy-boto3-lakeformation-1.34.7/mypy_boto3_lakeformation/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    42491 2023-12-22 20:32:09.000000 mypy-boto3-lakeformation-1.34.7/mypy_boto3_lakeformation/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11226 2023-12-22 20:32:10.000000 mypy-boto3-lakeformation-1.34.7/mypy_boto3_lakeformation/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    11226 2023-12-22 20:32:10.000000 mypy-boto3-lakeformation-1.34.7/mypy_boto3_lakeformation/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6799 2023-12-22 20:32:10.000000 mypy-boto3-lakeformation-1.34.7/mypy_boto3_lakeformation/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6793 2023-12-22 20:32:10.000000 mypy-boto3-lakeformation-1.34.7/mypy_boto3_lakeformation/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 20:32:09.000000 mypy-boto3-lakeformation-1.34.7/mypy_boto3_lakeformation/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    44684 2023-12-22 20:32:11.000000 mypy-boto3-lakeformation-1.34.7/mypy_boto3_lakeformation/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    44684 2023-12-22 20:32:10.000000 mypy-boto3-lakeformation-1.34.7/mypy_boto3_lakeformation/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-12-22 20:32:09.000000 mypy-boto3-lakeformation-1.34.7/mypy_boto3_lakeformation/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 20:32:30.660719 mypy-boto3-lakeformation-1.34.7/mypy_boto3_lakeformation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13549 2023-12-22 20:32:30.000000 mypy-boto3-lakeformation-1.34.7/mypy_boto3_lakeformation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      794 2023-12-22 20:32:30.000000 mypy-boto3-lakeformation-1.34.7/mypy_boto3_lakeformation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-22 20:32:30.000000 mypy-boto3-lakeformation-1.34.7/mypy_boto3_lakeformation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-22 20:32:30.000000 mypy-boto3-lakeformation-1.34.7/mypy_boto3_lakeformation.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-22 20:32:30.000000 mypy-boto3-lakeformation-1.34.7/mypy_boto3_lakeformation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2023-12-22 20:32:30.000000 mypy-boto3-lakeformation-1.34.7/mypy_boto3_lakeformation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-22 20:32:30.660719 mypy-boto3-lakeformation-1.34.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2023-12-22 20:32:09.000000 mypy-boto3-lakeformation-1.34.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:33:15.784319 mypy_boto3_lakeformation-1.34.85/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-16 19:32:55.000000 mypy_boto3_lakeformation-1.34.85/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13617 2024-04-16 19:33:15.784319 mypy_boto3_lakeformation-1.34.85/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12038 2024-04-16 19:32:55.000000 mypy_boto3_lakeformation-1.34.85/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:33:15.784319 mypy_boto3_lakeformation-1.34.85/mypy_boto3_lakeformation/
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-16 19:32:55.000000 mypy_boto3_lakeformation-1.34.85/mypy_boto3_lakeformation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-16 19:32:55.000000 mypy_boto3_lakeformation-1.34.85/mypy_boto3_lakeformation/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-16 19:32:55.000000 mypy_boto3_lakeformation-1.34.85/mypy_boto3_lakeformation/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42628 2024-04-16 19:32:56.000000 mypy_boto3_lakeformation-1.34.85/mypy_boto3_lakeformation/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42625 2024-04-16 19:32:55.000000 mypy_boto3_lakeformation-1.34.85/mypy_boto3_lakeformation/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11359 2024-04-16 19:32:56.000000 mypy_boto3_lakeformation-1.34.85/mypy_boto3_lakeformation/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11359 2024-04-16 19:32:56.000000 mypy_boto3_lakeformation-1.34.85/mypy_boto3_lakeformation/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6799 2024-04-16 19:32:56.000000 mypy_boto3_lakeformation-1.34.85/mypy_boto3_lakeformation/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6793 2024-04-16 19:32:56.000000 mypy_boto3_lakeformation-1.34.85/mypy_boto3_lakeformation/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 19:32:55.000000 mypy_boto3_lakeformation-1.34.85/mypy_boto3_lakeformation/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    44938 2024-04-16 19:32:56.000000 mypy_boto3_lakeformation-1.34.85/mypy_boto3_lakeformation/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44938 2024-04-16 19:32:56.000000 mypy_boto3_lakeformation-1.34.85/mypy_boto3_lakeformation/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-16 19:32:55.000000 mypy_boto3_lakeformation-1.34.85/mypy_boto3_lakeformation/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:33:15.784319 mypy_boto3_lakeformation-1.34.85/mypy_boto3_lakeformation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13617 2024-04-16 19:33:15.000000 mypy_boto3_lakeformation-1.34.85/mypy_boto3_lakeformation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-16 19:33:15.000000 mypy_boto3_lakeformation-1.34.85/mypy_boto3_lakeformation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 19:33:15.000000 mypy_boto3_lakeformation-1.34.85/mypy_boto3_lakeformation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 19:33:15.000000 mypy_boto3_lakeformation-1.34.85/mypy_boto3_lakeformation.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-16 19:33:15.000000 mypy_boto3_lakeformation-1.34.85/mypy_boto3_lakeformation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-16 19:33:15.000000 mypy_boto3_lakeformation-1.34.85/mypy_boto3_lakeformation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 19:33:15.784319 mypy_boto3_lakeformation-1.34.85/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-04-16 19:32:55.000000 mypy_boto3_lakeformation-1.34.85/setup.py
```

### Comparing `mypy-boto3-lakeformation-1.34.7/LICENSE` & `mypy_boto3_lakeformation-1.34.85/LICENSE`

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

### Comparing `mypy-boto3-lakeformation-1.34.7/PKG-INFO` & `mypy_boto3_lakeformation-1.34.85/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lakeformation
-Version: 1.34.7
-Summary: Type annotations for boto3.LakeFormation 1.34.7 service generated with mypy-boto3-builder 7.23.0
+Version: 1.34.85
+Summary: Type annotations for boto3.LakeFormation 1.34.85 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -25,37 +25,38 @@
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Stubs Only
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: typing-extensions>=4.1.0; python_version < "3.12"
 
 <a id="mypy-boto3-lakeformation"></a>
 
 # mypy-boto3-lakeformation
 
 [![PyPI - mypy-boto3-lakeformation](https://img.shields.io/pypi/v/mypy-boto3-lakeformation.svg?color=blue)](https://pypi.org/project/mypy-boto3-lakeformation)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lakeformation.svg?color=blue)](https://pypi.org/project/mypy-boto3-lakeformation)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lakeformation)](https://pepy.tech/project/mypy-boto3-lakeformation)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LakeFormation 1.34.7](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation)
+[boto3.LakeFormation 1.34.85](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-lakeformation docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-lakeformation-1.34.7/README.md` & `mypy_boto3_lakeformation-1.34.85/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lakeformation.svg?color=blue)](https://pypi.org/project/mypy-boto3-lakeformation)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lakeformation)](https://pepy.tech/project/mypy-boto3-lakeformation)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LakeFormation 1.34.7](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation)
+[boto3.LakeFormation 1.34.85](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-lakeformation docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-lakeformation-1.34.7/mypy_boto3_lakeformation/__init__.py` & `mypy_boto3_lakeformation-1.34.85/mypy_boto3_lakeformation/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lakeformation-1.34.7/mypy_boto3_lakeformation/__init__.pyi` & `mypy_boto3_lakeformation-1.34.85/mypy_boto3_lakeformation/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lakeformation-1.34.7/mypy_boto3_lakeformation/client.py` & `mypy_boto3_lakeformation-1.34.85/mypy_boto3_lakeformation/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -231,14 +231,15 @@
 
     def create_lake_formation_identity_center_configuration(
         self,
         *,
         CatalogId: str = ...,
         InstanceArn: str = ...,
         ExternalFiltering: ExternalFilteringConfigurationTypeDef = ...,
+        ShareRecipients: Sequence[DataLakePrincipalTypeDef] = ...,
     ) -> CreateLakeFormationIdentityCenterConfigurationResponseTypeDef:
         """
         Creates an IAM Identity Center connection with Lake Formation to allow IAM
         Identity Center users and groups to access Data Catalog
         resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.create_lake_formation_identity_center_configuration)
@@ -775,14 +776,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#update_data_cells_filter)
         """
 
     def update_lake_formation_identity_center_configuration(
         self,
         *,
         CatalogId: str = ...,
+        ShareRecipients: Sequence[DataLakePrincipalTypeDef] = ...,
         ApplicationStatus: ApplicationStatusType = ...,
         ExternalFiltering: ExternalFilteringConfigurationTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Updates the IAM Identity Center connection parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.update_lake_formation_identity_center_configuration)
```

### Comparing `mypy-boto3-lakeformation-1.34.7/mypy_boto3_lakeformation/client.pyi` & `mypy_boto3_lakeformation-1.34.85/mypy_boto3_lakeformation/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -228,14 +228,15 @@
 
     def create_lake_formation_identity_center_configuration(
         self,
         *,
         CatalogId: str = ...,
         InstanceArn: str = ...,
         ExternalFiltering: ExternalFilteringConfigurationTypeDef = ...,
+        ShareRecipients: Sequence[DataLakePrincipalTypeDef] = ...,
     ) -> CreateLakeFormationIdentityCenterConfigurationResponseTypeDef:
         """
         Creates an IAM Identity Center connection with Lake Formation to allow IAM
         Identity Center users and groups to access Data Catalog
         resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.create_lake_formation_identity_center_configuration)
@@ -772,14 +773,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#update_data_cells_filter)
         """
 
     def update_lake_formation_identity_center_configuration(
         self,
         *,
         CatalogId: str = ...,
+        ShareRecipients: Sequence[DataLakePrincipalTypeDef] = ...,
         ApplicationStatus: ApplicationStatusType = ...,
         ExternalFiltering: ExternalFilteringConfigurationTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Updates the IAM Identity Center connection parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.update_lake_formation_identity_center_configuration)
```

### Comparing `mypy-boto3-lakeformation-1.34.7/mypy_boto3_lakeformation/literals.py` & `mypy_boto3_lakeformation-1.34.85/mypy_boto3_lakeformation/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,14 +115,15 @@
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
@@ -133,14 +134,15 @@
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
@@ -158,14 +160,15 @@
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
@@ -178,24 +181,26 @@
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
@@ -256,15 +261,14 @@
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
@@ -438,19 +442,21 @@
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
@@ -499,14 +505,15 @@
     "ap-south-1",
     "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
     "ap-southeast-4",
     "ca-central-1",
+    "ca-west-1",
     "eu-central-1",
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
     "eu-west-2",
```

### Comparing `mypy-boto3-lakeformation-1.34.7/mypy_boto3_lakeformation/literals.pyi` & `mypy_boto3_lakeformation-1.34.85/mypy_boto3_lakeformation/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -115,14 +115,15 @@
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
@@ -133,14 +134,15 @@
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
@@ -158,14 +160,15 @@
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
@@ -178,24 +181,26 @@
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
@@ -256,15 +261,14 @@
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
@@ -438,19 +442,21 @@
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
@@ -499,14 +505,15 @@
     "ap-south-1",
     "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
     "ap-southeast-4",
     "ca-central-1",
+    "ca-west-1",
     "eu-central-1",
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
     "eu-west-2",
```

### Comparing `mypy-boto3-lakeformation-1.34.7/mypy_boto3_lakeformation/paginator.py` & `mypy_boto3_lakeformation-1.34.85/mypy_boto3_lakeformation/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lakeformation-1.34.7/mypy_boto3_lakeformation/paginator.pyi` & `mypy_boto3_lakeformation-1.34.85/mypy_boto3_lakeformation/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lakeformation-1.34.7/mypy_boto3_lakeformation/type_defs.py` & `mypy_boto3_lakeformation-1.34.85/mypy_boto3_lakeformation/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,18 +206,18 @@
         "CatalogId": NotRequired[str],
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
 AddObjectInputTypeDef = TypedDict(
     "AddObjectInputTypeDef",
     {
         "Uri": str,
         "ETag": str,
@@ -796,30 +796,34 @@
 )
 CreateLakeFormationIdentityCenterConfigurationRequestRequestTypeDef = TypedDict(
     "CreateLakeFormationIdentityCenterConfigurationRequestRequestTypeDef",
     {
         "CatalogId": NotRequired[str],
         "InstanceArn": NotRequired[str],
         "ExternalFiltering": NotRequired[ExternalFilteringConfigurationTypeDef],
+        "ShareRecipients": NotRequired[Sequence[DataLakePrincipalTypeDef]],
     },
 )
 DescribeLakeFormationIdentityCenterConfigurationResponseTypeDef = TypedDict(
     "DescribeLakeFormationIdentityCenterConfigurationResponseTypeDef",
     {
         "CatalogId": str,
         "InstanceArn": str,
         "ApplicationArn": str,
         "ExternalFiltering": ExternalFilteringConfigurationTypeDef,
+        "ShareRecipients": List[DataLakePrincipalTypeDef],
+        "ResourceShare": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 UpdateLakeFormationIdentityCenterConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateLakeFormationIdentityCenterConfigurationRequestRequestTypeDef",
     {
         "CatalogId": NotRequired[str],
+        "ShareRecipients": NotRequired[Sequence[DataLakePrincipalTypeDef]],
         "ApplicationStatus": NotRequired[ApplicationStatusType],
         "ExternalFiltering": NotRequired[ExternalFilteringConfigurationTypeDef],
     },
 )
 DataCellsFilterPaginatorTypeDef = TypedDict(
     "DataCellsFilterPaginatorTypeDef",
     {
```

### Comparing `mypy-boto3-lakeformation-1.34.7/mypy_boto3_lakeformation/type_defs.pyi` & `mypy_boto3_lakeformation-1.34.85/mypy_boto3_lakeformation/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -206,18 +206,18 @@
         "CatalogId": NotRequired[str],
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
 AddObjectInputTypeDef = TypedDict(
     "AddObjectInputTypeDef",
     {
         "Uri": str,
         "ETag": str,
@@ -796,30 +796,34 @@
 )
 CreateLakeFormationIdentityCenterConfigurationRequestRequestTypeDef = TypedDict(
     "CreateLakeFormationIdentityCenterConfigurationRequestRequestTypeDef",
     {
         "CatalogId": NotRequired[str],
         "InstanceArn": NotRequired[str],
         "ExternalFiltering": NotRequired[ExternalFilteringConfigurationTypeDef],
+        "ShareRecipients": NotRequired[Sequence[DataLakePrincipalTypeDef]],
     },
 )
 DescribeLakeFormationIdentityCenterConfigurationResponseTypeDef = TypedDict(
     "DescribeLakeFormationIdentityCenterConfigurationResponseTypeDef",
     {
         "CatalogId": str,
         "InstanceArn": str,
         "ApplicationArn": str,
         "ExternalFiltering": ExternalFilteringConfigurationTypeDef,
+        "ShareRecipients": List[DataLakePrincipalTypeDef],
+        "ResourceShare": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 UpdateLakeFormationIdentityCenterConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateLakeFormationIdentityCenterConfigurationRequestRequestTypeDef",
     {
         "CatalogId": NotRequired[str],
+        "ShareRecipients": NotRequired[Sequence[DataLakePrincipalTypeDef]],
         "ApplicationStatus": NotRequired[ApplicationStatusType],
         "ExternalFiltering": NotRequired[ExternalFilteringConfigurationTypeDef],
     },
 )
 DataCellsFilterPaginatorTypeDef = TypedDict(
     "DataCellsFilterPaginatorTypeDef",
     {
```

### Comparing `mypy-boto3-lakeformation-1.34.7/mypy_boto3_lakeformation.egg-info/PKG-INFO` & `mypy_boto3_lakeformation-1.34.85/mypy_boto3_lakeformation.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lakeformation
-Version: 1.34.7
-Summary: Type annotations for boto3.LakeFormation 1.34.7 service generated with mypy-boto3-builder 7.23.0
+Version: 1.34.85
+Summary: Type annotations for boto3.LakeFormation 1.34.85 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -25,37 +25,38 @@
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Stubs Only
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: typing-extensions>=4.1.0; python_version < "3.12"
 
 <a id="mypy-boto3-lakeformation"></a>
 
 # mypy-boto3-lakeformation
 
 [![PyPI - mypy-boto3-lakeformation](https://img.shields.io/pypi/v/mypy-boto3-lakeformation.svg?color=blue)](https://pypi.org/project/mypy-boto3-lakeformation)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lakeformation.svg?color=blue)](https://pypi.org/project/mypy-boto3-lakeformation)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lakeformation)](https://pepy.tech/project/mypy-boto3-lakeformation)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LakeFormation 1.34.7](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation)
+[boto3.LakeFormation 1.34.85](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-lakeformation docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-lakeformation-1.34.7/mypy_boto3_lakeformation.egg-info/SOURCES.txt` & `mypy_boto3_lakeformation-1.34.85/mypy_boto3_lakeformation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lakeformation-1.34.7/setup.py` & `mypy_boto3_lakeformation-1.34.85/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,24 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-lakeformation",
-    version="1.34.7",
+    version="1.34.85",
     packages=["mypy_boto3_lakeformation"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description=(
-        "Type annotations for boto3.LakeFormation 1.34.7 service generated with mypy-boto3-builder"
-        " 7.23.0"
-    ),
+    description="Type annotations for boto3.LakeFormation 1.34.85 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

