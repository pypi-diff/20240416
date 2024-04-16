# Comparing `tmp/mypy-boto3-wellarchitected-1.34.0.tar.gz` & `tmp/mypy_boto3_wellarchitected-1.34.85.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-wellarchitected-1.34.0.tar", last modified: Wed Dec 13 21:24:06 2023, max compression
+gzip compressed data, was "mypy_boto3_wellarchitected-1.34.85.tar", last modified: Tue Apr 16 19:33:17 2024, max compression
```

## Comparing `mypy-boto3-wellarchitected-1.34.0.tar` & `mypy_boto3_wellarchitected-1.34.85.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:24:06.327415 mypy-boto3-wellarchitected-1.34.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 21:21:12.000000 mypy-boto3-wellarchitected-1.34.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12478 2023-12-13 21:24:06.327415 mypy-boto3-wellarchitected-1.34.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10913 2023-12-13 21:21:12.000000 mypy-boto3-wellarchitected-1.34.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:24:06.323415 mypy-boto3-wellarchitected-1.34.0/mypy_boto3_wellarchitected/
--rw-r--r--   0 runner    (1001) docker     (127)      438 2023-12-13 21:21:12.000000 mypy-boto3-wellarchitected-1.34.0/mypy_boto3_wellarchitected/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2023-12-13 21:21:12.000000 mypy-boto3-wellarchitected-1.34.0/mypy_boto3_wellarchitected/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      937 2023-12-13 21:21:12.000000 mypy-boto3-wellarchitected-1.34.0/mypy_boto3_wellarchitected/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    47019 2023-12-13 21:21:12.000000 mypy-boto3-wellarchitected-1.34.0/mypy_boto3_wellarchitected/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    47016 2023-12-13 21:21:12.000000 mypy-boto3-wellarchitected-1.34.0/mypy_boto3_wellarchitected/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11876 2023-12-13 21:21:12.000000 mypy-boto3-wellarchitected-1.34.0/mypy_boto3_wellarchitected/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    11874 2023-12-13 21:21:12.000000 mypy-boto3-wellarchitected-1.34.0/mypy_boto3_wellarchitected/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 21:21:12.000000 mypy-boto3-wellarchitected-1.34.0/mypy_boto3_wellarchitected/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    60414 2023-12-13 21:21:13.000000 mypy-boto3-wellarchitected-1.34.0/mypy_boto3_wellarchitected/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    60413 2023-12-13 21:21:13.000000 mypy-boto3-wellarchitected-1.34.0/mypy_boto3_wellarchitected/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-12-13 21:21:12.000000 mypy-boto3-wellarchitected-1.34.0/mypy_boto3_wellarchitected/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:24:06.327415 mypy-boto3-wellarchitected-1.34.0/mypy_boto3_wellarchitected.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12478 2023-12-13 21:24:06.000000 mypy-boto3-wellarchitected-1.34.0/mypy_boto3_wellarchitected.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      751 2023-12-13 21:24:06.000000 mypy-boto3-wellarchitected-1.34.0/mypy_boto3_wellarchitected.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:24:06.000000 mypy-boto3-wellarchitected-1.34.0/mypy_boto3_wellarchitected.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:24:06.000000 mypy-boto3-wellarchitected-1.34.0/mypy_boto3_wellarchitected.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 21:24:06.000000 mypy-boto3-wellarchitected-1.34.0/mypy_boto3_wellarchitected.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-12-13 21:24:06.000000 mypy-boto3-wellarchitected-1.34.0/mypy_boto3_wellarchitected.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 21:24:06.327415 mypy-boto3-wellarchitected-1.34.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2023-12-13 21:21:12.000000 mypy-boto3-wellarchitected-1.34.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:33:17.156337 mypy_boto3_wellarchitected-1.34.85/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-16 19:33:02.000000 mypy_boto3_wellarchitected-1.34.85/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12553 2024-04-16 19:33:17.156337 mypy_boto3_wellarchitected-1.34.85/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10966 2024-04-16 19:33:02.000000 mypy_boto3_wellarchitected-1.34.85/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:33:17.156337 mypy_boto3_wellarchitected-1.34.85/mypy_boto3_wellarchitected/
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-16 19:33:02.000000 mypy_boto3_wellarchitected-1.34.85/mypy_boto3_wellarchitected/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-16 19:33:02.000000 mypy_boto3_wellarchitected-1.34.85/mypy_boto3_wellarchitected/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-16 19:33:02.000000 mypy_boto3_wellarchitected-1.34.85/mypy_boto3_wellarchitected/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48639 2024-04-16 19:33:02.000000 mypy_boto3_wellarchitected-1.34.85/mypy_boto3_wellarchitected/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48636 2024-04-16 19:33:02.000000 mypy_boto3_wellarchitected-1.34.85/mypy_boto3_wellarchitected/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12614 2024-04-16 19:33:02.000000 mypy_boto3_wellarchitected-1.34.85/mypy_boto3_wellarchitected/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12614 2024-04-16 19:33:02.000000 mypy_boto3_wellarchitected-1.34.85/mypy_boto3_wellarchitected/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 19:33:02.000000 mypy_boto3_wellarchitected-1.34.85/mypy_boto3_wellarchitected/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    64255 2024-04-16 19:33:03.000000 mypy_boto3_wellarchitected-1.34.85/mypy_boto3_wellarchitected/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64255 2024-04-16 19:33:03.000000 mypy_boto3_wellarchitected-1.34.85/mypy_boto3_wellarchitected/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-16 19:33:02.000000 mypy_boto3_wellarchitected-1.34.85/mypy_boto3_wellarchitected/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:33:17.156337 mypy_boto3_wellarchitected-1.34.85/mypy_boto3_wellarchitected.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12553 2024-04-16 19:33:17.000000 mypy_boto3_wellarchitected-1.34.85/mypy_boto3_wellarchitected.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-16 19:33:17.000000 mypy_boto3_wellarchitected-1.34.85/mypy_boto3_wellarchitected.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 19:33:17.000000 mypy_boto3_wellarchitected-1.34.85/mypy_boto3_wellarchitected.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 19:33:17.000000 mypy_boto3_wellarchitected-1.34.85/mypy_boto3_wellarchitected.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-16 19:33:17.000000 mypy_boto3_wellarchitected-1.34.85/mypy_boto3_wellarchitected.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-16 19:33:17.000000 mypy_boto3_wellarchitected-1.34.85/mypy_boto3_wellarchitected.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 19:33:17.156337 mypy_boto3_wellarchitected-1.34.85/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-04-16 19:33:02.000000 mypy_boto3_wellarchitected-1.34.85/setup.py
```

### Comparing `mypy-boto3-wellarchitected-1.34.0/LICENSE` & `mypy_boto3_wellarchitected-1.34.85/LICENSE`

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

### Comparing `mypy-boto3-wellarchitected-1.34.0/PKG-INFO` & `mypy_boto3_wellarchitected-1.34.85/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-wellarchitected
-Version: 1.34.0
-Summary: Type annotations for boto3.WellArchitected 1.34.0 service generated with mypy-boto3-builder 7.21.0
+Version: 1.34.85
+Summary: Type annotations for boto3.WellArchitected 1.34.85 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/
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
 
 <a id="mypy-boto3-wellarchitected"></a>
 
 # mypy-boto3-wellarchitected
 
 [![PyPI - mypy-boto3-wellarchitected](https://img.shields.io/pypi/v/mypy-boto3-wellarchitected.svg?color=blue)](https://pypi.org/project/mypy-boto3-wellarchitected)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-wellarchitected.svg?color=blue)](https://pypi.org/project/mypy-boto3-wellarchitected)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-wellarchitected)](https://pepy.tech/project/mypy-boto3-wellarchitected)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WellArchitected 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected)
+[boto3.WellArchitected 1.34.85](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected)
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
 [mypy-boto3-wellarchitected docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/).
 
 See how it helps to find and fix potential bugs:
 
@@ -280,35 +280,35 @@
 `mypy_boto3_wellarchitected.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
 Full list of `WellArchitected` Literals can be found in
 [docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/literals/).
 
 ```python
-from mypy_boto3_wellarchitected.literals import AdditionalResourceTypeType
+from mypy_boto3_wellarchitected.literals import AccountJiraIssueManagementStatusType
 
 
-def check_value(value: AdditionalResourceTypeType) -> bool: ...
+def check_value(value: AccountJiraIssueManagementStatusType) -> bool: ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `mypy_boto3_wellarchitected.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
 Full list of `WellArchitected` TypeDefs can be found in
 [docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/type_defs/).
 
 ```python
-from mypy_boto3_wellarchitected.type_defs import ChoiceContentTypeDef
+from mypy_boto3_wellarchitected.type_defs import AccountJiraConfigurationInputTypeDef
 
 
-def get_value() -> ChoiceContentTypeDef:
+def get_value() -> AccountJiraConfigurationInputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-wellarchitected-1.34.0/README.md` & `mypy_boto3_wellarchitected-1.34.85/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-wellarchitected.svg?color=blue)](https://pypi.org/project/mypy-boto3-wellarchitected)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-wellarchitected)](https://pepy.tech/project/mypy-boto3-wellarchitected)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WellArchitected 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected)
+[boto3.WellArchitected 1.34.85](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected)
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
 [mypy-boto3-wellarchitected docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/).
 
 See how it helps to find and fix potential bugs:
 
@@ -247,35 +247,35 @@
 `mypy_boto3_wellarchitected.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
 Full list of `WellArchitected` Literals can be found in
 [docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/literals/).
 
 ```python
-from mypy_boto3_wellarchitected.literals import AdditionalResourceTypeType
+from mypy_boto3_wellarchitected.literals import AccountJiraIssueManagementStatusType
 
 
-def check_value(value: AdditionalResourceTypeType) -> bool: ...
+def check_value(value: AccountJiraIssueManagementStatusType) -> bool: ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `mypy_boto3_wellarchitected.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
 Full list of `WellArchitected` TypeDefs can be found in
 [docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/type_defs/).
 
 ```python
-from mypy_boto3_wellarchitected.type_defs import ChoiceContentTypeDef
+from mypy_boto3_wellarchitected.type_defs import AccountJiraConfigurationInputTypeDef
 
 
-def get_value() -> ChoiceContentTypeDef:
+def get_value() -> AccountJiraConfigurationInputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-wellarchitected-1.34.0/mypy_boto3_wellarchitected/client.py` & `mypy_boto3_wellarchitected-1.34.85/mypy_boto3_wellarchitected/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     from mypy_boto3_wellarchitected.client import WellArchitectedClient
 
     session = Session()
     client: WellArchitectedClient = session.client("wellarchitected")
     ```
 """
 
+import sys
 from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AnswerReasonType,
     DiscoveryIntegrationStatusType,
@@ -31,40 +32,43 @@
     ShareInvitationActionType,
     ShareResourceTypeType,
     ShareStatusType,
     WorkloadEnvironmentType,
     WorkloadImprovementStatusType,
 )
 from .type_defs import (
+    AccountJiraConfigurationInputTypeDef,
     ChoiceUpdateTypeDef,
     CreateLensShareOutputTypeDef,
     CreateLensVersionOutputTypeDef,
     CreateMilestoneOutputTypeDef,
     CreateProfileOutputTypeDef,
     CreateProfileShareOutputTypeDef,
     CreateReviewTemplateOutputTypeDef,
     CreateTemplateShareOutputTypeDef,
     CreateWorkloadOutputTypeDef,
     CreateWorkloadShareOutputTypeDef,
     EmptyResponseMetadataTypeDef,
     ExportLensOutputTypeDef,
     GetAnswerOutputTypeDef,
     GetConsolidatedReportOutputTypeDef,
+    GetGlobalSettingsOutputTypeDef,
     GetLensOutputTypeDef,
     GetLensReviewOutputTypeDef,
     GetLensReviewReportOutputTypeDef,
     GetLensVersionDifferenceOutputTypeDef,
     GetMilestoneOutputTypeDef,
     GetProfileOutputTypeDef,
     GetProfileTemplateOutputTypeDef,
     GetReviewTemplateAnswerOutputTypeDef,
     GetReviewTemplateLensReviewOutputTypeDef,
     GetReviewTemplateOutputTypeDef,
     GetWorkloadOutputTypeDef,
     ImportLensOutputTypeDef,
+    JiraSelectedQuestionConfigurationTypeDef,
     ListAnswersOutputTypeDef,
     ListCheckDetailsOutputTypeDef,
     ListCheckSummariesOutputTypeDef,
     ListLensesOutputTypeDef,
     ListLensReviewImprovementsOutputTypeDef,
     ListLensReviewsOutputTypeDef,
     ListLensSharesOutputTypeDef,
@@ -87,16 +91,22 @@
     UpdateReviewTemplateAnswerOutputTypeDef,
     UpdateReviewTemplateLensReviewOutputTypeDef,
     UpdateReviewTemplateOutputTypeDef,
     UpdateShareInvitationOutputTypeDef,
     UpdateWorkloadOutputTypeDef,
     UpdateWorkloadShareOutputTypeDef,
     WorkloadDiscoveryConfigTypeDef,
+    WorkloadJiraConfigurationInputTypeDef,
 )
 
+if sys.version_info >= (3, 12):
+    from typing import Literal
+else:
+    from typing_extensions import Literal
+
 __all__ = ("WellArchitectedClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -180,15 +190,15 @@
 
     def create_lens_version(
         self,
         *,
         LensAlias: str,
         LensVersion: str,
         ClientRequestToken: str,
-        IsMajorVersion: bool = ...
+        IsMajorVersion: bool = ...,
     ) -> CreateLensVersionOutputTypeDef:
         """
         Create a new lens version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.create_lens_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#create_lens_version)
         """
@@ -206,15 +216,15 @@
     def create_profile(
         self,
         *,
         ProfileName: str,
         ProfileDescription: str,
         ProfileQuestions: Sequence[ProfileQuestionUpdateTypeDef],
         ClientRequestToken: str,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateProfileOutputTypeDef:
         """
         Create a profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.create_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#create_profile)
         """
@@ -233,15 +243,15 @@
         self,
         *,
         TemplateName: str,
         Description: str,
         Lenses: Sequence[str],
         ClientRequestToken: str,
         Notes: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateReviewTemplateOutputTypeDef:
         """
         Create a review template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.create_review_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#create_review_template)
         """
@@ -273,30 +283,31 @@
         IndustryType: str = ...,
         Industry: str = ...,
         Notes: str = ...,
         Tags: Mapping[str, str] = ...,
         DiscoveryConfig: WorkloadDiscoveryConfigTypeDef = ...,
         Applications: Sequence[str] = ...,
         ProfileArns: Sequence[str] = ...,
-        ReviewTemplateArns: Sequence[str] = ...
+        ReviewTemplateArns: Sequence[str] = ...,
+        JiraConfiguration: WorkloadJiraConfigurationInputTypeDef = ...,
     ) -> CreateWorkloadOutputTypeDef:
         """
         Create a new workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.create_workload)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#create_workload)
         """
 
     def create_workload_share(
         self,
         *,
         WorkloadId: str,
         SharedWith: str,
         PermissionType: PermissionTypeType,
-        ClientRequestToken: str
+        ClientRequestToken: str,
     ) -> CreateWorkloadShareOutputTypeDef:
         """
         Create a workload share.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.create_workload_share)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#create_workload_share)
         """
@@ -435,23 +446,31 @@
 
     def get_consolidated_report(
         self,
         *,
         Format: ReportFormatType,
         IncludeSharedResources: bool = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> GetConsolidatedReportOutputTypeDef:
         """
         Get a consolidated report of your workloads.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.get_consolidated_report)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#get_consolidated_report)
         """
 
+    def get_global_settings(self) -> GetGlobalSettingsOutputTypeDef:
+        """
+        Global settings for all workloads.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.get_global_settings)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#get_global_settings)
+        """
+
     def get_lens(self, *, LensAlias: str, LensVersion: str = ...) -> GetLensOutputTypeDef:
         """
         Get an existing lens.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.get_lens)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#get_lens)
         """
@@ -548,15 +567,15 @@
 
     def import_lens(
         self,
         *,
         JSONString: str,
         ClientRequestToken: str,
         LensAlias: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> ImportLensOutputTypeDef:
         """
         Import a new custom lens or update an existing custom lens.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.import_lens)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#import_lens)
         """
@@ -566,15 +585,15 @@
         *,
         WorkloadId: str,
         LensAlias: str,
         PillarId: str = ...,
         MilestoneNumber: int = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
-        QuestionPriority: QuestionPriorityType = ...
+        QuestionPriority: QuestionPriorityType = ...,
     ) -> ListAnswersOutputTypeDef:
         """
         List of answers for a particular workload and lens.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_answers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#list_answers)
         """
@@ -584,15 +603,15 @@
         *,
         WorkloadId: str,
         LensArn: str,
         PillarId: str,
         QuestionId: str,
         ChoiceId: str,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListCheckDetailsOutputTypeDef:
         """
         List of Trusted Advisor check details by account related to the workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_check_details)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#list_check_details)
         """
@@ -602,15 +621,15 @@
         *,
         WorkloadId: str,
         LensArn: str,
         PillarId: str,
         QuestionId: str,
         ChoiceId: str,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListCheckSummariesOutputTypeDef:
         """
         List of Trusted Advisor checks summarized for all accounts related to the
         workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_check_summaries)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#list_check_summaries)
@@ -621,30 +640,30 @@
         *,
         WorkloadId: str,
         LensAlias: str,
         PillarId: str = ...,
         MilestoneNumber: int = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
-        QuestionPriority: QuestionPriorityType = ...
+        QuestionPriority: QuestionPriorityType = ...,
     ) -> ListLensReviewImprovementsOutputTypeDef:
         """
-        List lens review improvements.
+        List the improvements of a particular lens review.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_lens_review_improvements)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#list_lens_review_improvements)
         """
 
     def list_lens_reviews(
         self,
         *,
         WorkloadId: str,
         MilestoneNumber: int = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListLensReviewsOutputTypeDef:
         """
         List lens reviews for a particular workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_lens_reviews)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#list_lens_reviews)
         """
@@ -652,15 +671,15 @@
     def list_lens_shares(
         self,
         *,
         LensAlias: str,
         SharedWithPrefix: str = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
-        Status: ShareStatusType = ...
+        Status: ShareStatusType = ...,
     ) -> ListLensSharesOutputTypeDef:
         """
         List the lens shares associated with the lens.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_lens_shares)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#list_lens_shares)
         """
@@ -668,15 +687,15 @@
     def list_lenses(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         LensType: LensTypeType = ...,
         LensStatus: LensStatusTypeType = ...,
-        LensName: str = ...
+        LensName: str = ...,
     ) -> ListLensesOutputTypeDef:
         """
         List the available lenses.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_lenses)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#list_lenses)
         """
@@ -693,15 +712,15 @@
 
     def list_notifications(
         self,
         *,
         WorkloadId: str = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
-        ResourceArn: str = ...
+        ResourceArn: str = ...,
     ) -> ListNotificationsOutputTypeDef:
         """
         List lens notifications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_notifications)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#list_notifications)
         """
@@ -719,30 +738,30 @@
     def list_profile_shares(
         self,
         *,
         ProfileArn: str,
         SharedWithPrefix: str = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
-        Status: ShareStatusType = ...
+        Status: ShareStatusType = ...,
     ) -> ListProfileSharesOutputTypeDef:
         """
         List profile shares.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_profile_shares)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#list_profile_shares)
         """
 
     def list_profiles(
         self,
         *,
         ProfileNamePrefix: str = ...,
         ProfileOwnerType: ProfileOwnerTypeType = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListProfilesOutputTypeDef:
         """
         List profiles.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_profiles)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#list_profiles)
         """
@@ -750,15 +769,15 @@
     def list_review_template_answers(
         self,
         *,
         TemplateArn: str,
         LensAlias: str,
         PillarId: str = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListReviewTemplateAnswersOutputTypeDef:
         """
         List the answers of a review template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_review_template_answers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#list_review_template_answers)
         """
@@ -778,15 +797,15 @@
         *,
         WorkloadNamePrefix: str = ...,
         LensNamePrefix: str = ...,
         ShareResourceType: ShareResourceTypeType = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
         ProfileNamePrefix: str = ...,
-        TemplateNamePrefix: str = ...
+        TemplateNamePrefix: str = ...,
     ) -> ListShareInvitationsOutputTypeDef:
         """
         List the share invitations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_share_invitations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#list_share_invitations)
         """
@@ -802,15 +821,15 @@
     def list_template_shares(
         self,
         *,
         TemplateArn: str,
         SharedWithPrefix: str = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
-        Status: ShareStatusType = ...
+        Status: ShareStatusType = ...,
     ) -> ListTemplateSharesOutputTypeDef:
         """
         List review template shares.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_template_shares)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#list_template_shares)
         """
@@ -818,15 +837,15 @@
     def list_workload_shares(
         self,
         *,
         WorkloadId: str,
         SharedWithPrefix: str = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
-        Status: ShareStatusType = ...
+        Status: ShareStatusType = ...,
     ) -> ListWorkloadSharesOutputTypeDef:
         """
         List the workload shares associated with the workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_workload_shares)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#list_workload_shares)
         """
@@ -863,59 +882,71 @@
         WorkloadId: str,
         LensAlias: str,
         QuestionId: str,
         SelectedChoices: Sequence[str] = ...,
         ChoiceUpdates: Mapping[str, ChoiceUpdateTypeDef] = ...,
         Notes: str = ...,
         IsApplicable: bool = ...,
-        Reason: AnswerReasonType = ...
+        Reason: AnswerReasonType = ...,
     ) -> UpdateAnswerOutputTypeDef:
         """
         Update the answer to a specific question in a workload review.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.update_answer)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#update_answer)
         """
 
     def update_global_settings(
         self,
         *,
         OrganizationSharingStatus: OrganizationSharingStatusType = ...,
-        DiscoveryIntegrationStatus: DiscoveryIntegrationStatusType = ...
+        DiscoveryIntegrationStatus: DiscoveryIntegrationStatusType = ...,
+        JiraConfiguration: AccountJiraConfigurationInputTypeDef = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
-        Updates whether the Amazon Web Services account is opted into organization
+        Update whether the Amazon Web Services account is opted into organization
         sharing and discovery integration
         features.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.update_global_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#update_global_settings)
         """
 
+    def update_integration(
+        self, *, WorkloadId: str, ClientRequestToken: str, IntegratingService: Literal["JIRA"]
+    ) -> EmptyResponseMetadataTypeDef:
+        """
+        Update integration features.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.update_integration)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#update_integration)
+        """
+
     def update_lens_review(
         self,
         *,
         WorkloadId: str,
         LensAlias: str,
         LensNotes: str = ...,
-        PillarNotes: Mapping[str, str] = ...
+        PillarNotes: Mapping[str, str] = ...,
+        JiraConfiguration: JiraSelectedQuestionConfigurationTypeDef = ...,
     ) -> UpdateLensReviewOutputTypeDef:
         """
         Update lens review for a particular workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.update_lens_review)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#update_lens_review)
         """
 
     def update_profile(
         self,
         *,
         ProfileArn: str,
         ProfileDescription: str = ...,
-        ProfileQuestions: Sequence[ProfileQuestionUpdateTypeDef] = ...
+        ProfileQuestions: Sequence[ProfileQuestionUpdateTypeDef] = ...,
     ) -> UpdateProfileOutputTypeDef:
         """
         Update a profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.update_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#update_profile)
         """
@@ -924,15 +955,15 @@
         self,
         *,
         TemplateArn: str,
         TemplateName: str = ...,
         Description: str = ...,
         Notes: str = ...,
         LensesToAssociate: Sequence[str] = ...,
-        LensesToDisassociate: Sequence[str] = ...
+        LensesToDisassociate: Sequence[str] = ...,
     ) -> UpdateReviewTemplateOutputTypeDef:
         """
         Update a review template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.update_review_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#update_review_template)
         """
@@ -943,30 +974,30 @@
         TemplateArn: str,
         LensAlias: str,
         QuestionId: str,
         SelectedChoices: Sequence[str] = ...,
         ChoiceUpdates: Mapping[str, ChoiceUpdateTypeDef] = ...,
         Notes: str = ...,
         IsApplicable: bool = ...,
-        Reason: AnswerReasonType = ...
+        Reason: AnswerReasonType = ...,
     ) -> UpdateReviewTemplateAnswerOutputTypeDef:
         """
         Update a review template answer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.update_review_template_answer)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#update_review_template_answer)
         """
 
     def update_review_template_lens_review(
         self,
         *,
         TemplateArn: str,
         LensAlias: str,
         LensNotes: str = ...,
-        PillarNotes: Mapping[str, str] = ...
+        PillarNotes: Mapping[str, str] = ...,
     ) -> UpdateReviewTemplateLensReviewOutputTypeDef:
         """
         Update a lens review associated with a review template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.update_review_template_lens_review)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#update_review_template_lens_review)
         """
@@ -996,15 +1027,16 @@
         ReviewOwner: str = ...,
         IsReviewOwnerUpdateAcknowledged: bool = ...,
         IndustryType: str = ...,
         Industry: str = ...,
         Notes: str = ...,
         ImprovementStatus: WorkloadImprovementStatusType = ...,
         DiscoveryConfig: WorkloadDiscoveryConfigTypeDef = ...,
-        Applications: Sequence[str] = ...
+        Applications: Sequence[str] = ...,
+        JiraConfiguration: WorkloadJiraConfigurationInputTypeDef = ...,
     ) -> UpdateWorkloadOutputTypeDef:
         """
         Update an existing workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.update_workload)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#update_workload)
         """
@@ -1031,15 +1063,15 @@
 
     def upgrade_profile_version(
         self,
         *,
         WorkloadId: str,
         ProfileArn: str,
         MilestoneName: str = ...,
-        ClientRequestToken: str = ...
+        ClientRequestToken: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Upgrade a profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.upgrade_profile_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#upgrade_profile_version)
         """
```

### Comparing `mypy-boto3-wellarchitected-1.34.0/mypy_boto3_wellarchitected/client.pyi` & `mypy_boto3_wellarchitected-1.34.85/mypy_boto3_wellarchitected/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     from mypy_boto3_wellarchitected.client import WellArchitectedClient
 
     session = Session()
     client: WellArchitectedClient = session.client("wellarchitected")
     ```
 """
 
+import sys
 from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AnswerReasonType,
     DiscoveryIntegrationStatusType,
@@ -31,40 +32,43 @@
     ShareInvitationActionType,
     ShareResourceTypeType,
     ShareStatusType,
     WorkloadEnvironmentType,
     WorkloadImprovementStatusType,
 )
 from .type_defs import (
+    AccountJiraConfigurationInputTypeDef,
     ChoiceUpdateTypeDef,
     CreateLensShareOutputTypeDef,
     CreateLensVersionOutputTypeDef,
     CreateMilestoneOutputTypeDef,
     CreateProfileOutputTypeDef,
     CreateProfileShareOutputTypeDef,
     CreateReviewTemplateOutputTypeDef,
     CreateTemplateShareOutputTypeDef,
     CreateWorkloadOutputTypeDef,
     CreateWorkloadShareOutputTypeDef,
     EmptyResponseMetadataTypeDef,
     ExportLensOutputTypeDef,
     GetAnswerOutputTypeDef,
     GetConsolidatedReportOutputTypeDef,
+    GetGlobalSettingsOutputTypeDef,
     GetLensOutputTypeDef,
     GetLensReviewOutputTypeDef,
     GetLensReviewReportOutputTypeDef,
     GetLensVersionDifferenceOutputTypeDef,
     GetMilestoneOutputTypeDef,
     GetProfileOutputTypeDef,
     GetProfileTemplateOutputTypeDef,
     GetReviewTemplateAnswerOutputTypeDef,
     GetReviewTemplateLensReviewOutputTypeDef,
     GetReviewTemplateOutputTypeDef,
     GetWorkloadOutputTypeDef,
     ImportLensOutputTypeDef,
+    JiraSelectedQuestionConfigurationTypeDef,
     ListAnswersOutputTypeDef,
     ListCheckDetailsOutputTypeDef,
     ListCheckSummariesOutputTypeDef,
     ListLensesOutputTypeDef,
     ListLensReviewImprovementsOutputTypeDef,
     ListLensReviewsOutputTypeDef,
     ListLensSharesOutputTypeDef,
@@ -87,16 +91,22 @@
     UpdateReviewTemplateAnswerOutputTypeDef,
     UpdateReviewTemplateLensReviewOutputTypeDef,
     UpdateReviewTemplateOutputTypeDef,
     UpdateShareInvitationOutputTypeDef,
     UpdateWorkloadOutputTypeDef,
     UpdateWorkloadShareOutputTypeDef,
     WorkloadDiscoveryConfigTypeDef,
+    WorkloadJiraConfigurationInputTypeDef,
 )
 
+if sys.version_info >= (3, 12):
+    from typing import Literal
+else:
+    from typing_extensions import Literal
+
 __all__ = ("WellArchitectedClient",)
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
@@ -177,15 +187,15 @@
 
     def create_lens_version(
         self,
         *,
         LensAlias: str,
         LensVersion: str,
         ClientRequestToken: str,
-        IsMajorVersion: bool = ...
+        IsMajorVersion: bool = ...,
     ) -> CreateLensVersionOutputTypeDef:
         """
         Create a new lens version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.create_lens_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#create_lens_version)
         """
@@ -203,15 +213,15 @@
     def create_profile(
         self,
         *,
         ProfileName: str,
         ProfileDescription: str,
         ProfileQuestions: Sequence[ProfileQuestionUpdateTypeDef],
         ClientRequestToken: str,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateProfileOutputTypeDef:
         """
         Create a profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.create_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#create_profile)
         """
@@ -230,15 +240,15 @@
         self,
         *,
         TemplateName: str,
         Description: str,
         Lenses: Sequence[str],
         ClientRequestToken: str,
         Notes: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateReviewTemplateOutputTypeDef:
         """
         Create a review template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.create_review_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#create_review_template)
         """
@@ -270,30 +280,31 @@
         IndustryType: str = ...,
         Industry: str = ...,
         Notes: str = ...,
         Tags: Mapping[str, str] = ...,
         DiscoveryConfig: WorkloadDiscoveryConfigTypeDef = ...,
         Applications: Sequence[str] = ...,
         ProfileArns: Sequence[str] = ...,
-        ReviewTemplateArns: Sequence[str] = ...
+        ReviewTemplateArns: Sequence[str] = ...,
+        JiraConfiguration: WorkloadJiraConfigurationInputTypeDef = ...,
     ) -> CreateWorkloadOutputTypeDef:
         """
         Create a new workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.create_workload)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#create_workload)
         """
 
     def create_workload_share(
         self,
         *,
         WorkloadId: str,
         SharedWith: str,
         PermissionType: PermissionTypeType,
-        ClientRequestToken: str
+        ClientRequestToken: str,
     ) -> CreateWorkloadShareOutputTypeDef:
         """
         Create a workload share.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.create_workload_share)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#create_workload_share)
         """
@@ -432,23 +443,31 @@
 
     def get_consolidated_report(
         self,
         *,
         Format: ReportFormatType,
         IncludeSharedResources: bool = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> GetConsolidatedReportOutputTypeDef:
         """
         Get a consolidated report of your workloads.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.get_consolidated_report)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#get_consolidated_report)
         """
 
+    def get_global_settings(self) -> GetGlobalSettingsOutputTypeDef:
+        """
+        Global settings for all workloads.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.get_global_settings)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#get_global_settings)
+        """
+
     def get_lens(self, *, LensAlias: str, LensVersion: str = ...) -> GetLensOutputTypeDef:
         """
         Get an existing lens.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.get_lens)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#get_lens)
         """
@@ -545,15 +564,15 @@
 
     def import_lens(
         self,
         *,
         JSONString: str,
         ClientRequestToken: str,
         LensAlias: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> ImportLensOutputTypeDef:
         """
         Import a new custom lens or update an existing custom lens.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.import_lens)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#import_lens)
         """
@@ -563,15 +582,15 @@
         *,
         WorkloadId: str,
         LensAlias: str,
         PillarId: str = ...,
         MilestoneNumber: int = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
-        QuestionPriority: QuestionPriorityType = ...
+        QuestionPriority: QuestionPriorityType = ...,
     ) -> ListAnswersOutputTypeDef:
         """
         List of answers for a particular workload and lens.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_answers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#list_answers)
         """
@@ -581,15 +600,15 @@
         *,
         WorkloadId: str,
         LensArn: str,
         PillarId: str,
         QuestionId: str,
         ChoiceId: str,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListCheckDetailsOutputTypeDef:
         """
         List of Trusted Advisor check details by account related to the workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_check_details)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#list_check_details)
         """
@@ -599,15 +618,15 @@
         *,
         WorkloadId: str,
         LensArn: str,
         PillarId: str,
         QuestionId: str,
         ChoiceId: str,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListCheckSummariesOutputTypeDef:
         """
         List of Trusted Advisor checks summarized for all accounts related to the
         workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_check_summaries)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#list_check_summaries)
@@ -618,30 +637,30 @@
         *,
         WorkloadId: str,
         LensAlias: str,
         PillarId: str = ...,
         MilestoneNumber: int = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
-        QuestionPriority: QuestionPriorityType = ...
+        QuestionPriority: QuestionPriorityType = ...,
     ) -> ListLensReviewImprovementsOutputTypeDef:
         """
-        List lens review improvements.
+        List the improvements of a particular lens review.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_lens_review_improvements)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#list_lens_review_improvements)
         """
 
     def list_lens_reviews(
         self,
         *,
         WorkloadId: str,
         MilestoneNumber: int = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListLensReviewsOutputTypeDef:
         """
         List lens reviews for a particular workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_lens_reviews)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#list_lens_reviews)
         """
@@ -649,15 +668,15 @@
     def list_lens_shares(
         self,
         *,
         LensAlias: str,
         SharedWithPrefix: str = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
-        Status: ShareStatusType = ...
+        Status: ShareStatusType = ...,
     ) -> ListLensSharesOutputTypeDef:
         """
         List the lens shares associated with the lens.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_lens_shares)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#list_lens_shares)
         """
@@ -665,15 +684,15 @@
     def list_lenses(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         LensType: LensTypeType = ...,
         LensStatus: LensStatusTypeType = ...,
-        LensName: str = ...
+        LensName: str = ...,
     ) -> ListLensesOutputTypeDef:
         """
         List the available lenses.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_lenses)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#list_lenses)
         """
@@ -690,15 +709,15 @@
 
     def list_notifications(
         self,
         *,
         WorkloadId: str = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
-        ResourceArn: str = ...
+        ResourceArn: str = ...,
     ) -> ListNotificationsOutputTypeDef:
         """
         List lens notifications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_notifications)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#list_notifications)
         """
@@ -716,30 +735,30 @@
     def list_profile_shares(
         self,
         *,
         ProfileArn: str,
         SharedWithPrefix: str = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
-        Status: ShareStatusType = ...
+        Status: ShareStatusType = ...,
     ) -> ListProfileSharesOutputTypeDef:
         """
         List profile shares.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_profile_shares)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#list_profile_shares)
         """
 
     def list_profiles(
         self,
         *,
         ProfileNamePrefix: str = ...,
         ProfileOwnerType: ProfileOwnerTypeType = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListProfilesOutputTypeDef:
         """
         List profiles.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_profiles)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#list_profiles)
         """
@@ -747,15 +766,15 @@
     def list_review_template_answers(
         self,
         *,
         TemplateArn: str,
         LensAlias: str,
         PillarId: str = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListReviewTemplateAnswersOutputTypeDef:
         """
         List the answers of a review template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_review_template_answers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#list_review_template_answers)
         """
@@ -775,15 +794,15 @@
         *,
         WorkloadNamePrefix: str = ...,
         LensNamePrefix: str = ...,
         ShareResourceType: ShareResourceTypeType = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
         ProfileNamePrefix: str = ...,
-        TemplateNamePrefix: str = ...
+        TemplateNamePrefix: str = ...,
     ) -> ListShareInvitationsOutputTypeDef:
         """
         List the share invitations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_share_invitations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#list_share_invitations)
         """
@@ -799,15 +818,15 @@
     def list_template_shares(
         self,
         *,
         TemplateArn: str,
         SharedWithPrefix: str = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
-        Status: ShareStatusType = ...
+        Status: ShareStatusType = ...,
     ) -> ListTemplateSharesOutputTypeDef:
         """
         List review template shares.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_template_shares)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#list_template_shares)
         """
@@ -815,15 +834,15 @@
     def list_workload_shares(
         self,
         *,
         WorkloadId: str,
         SharedWithPrefix: str = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
-        Status: ShareStatusType = ...
+        Status: ShareStatusType = ...,
     ) -> ListWorkloadSharesOutputTypeDef:
         """
         List the workload shares associated with the workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_workload_shares)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#list_workload_shares)
         """
@@ -860,59 +879,71 @@
         WorkloadId: str,
         LensAlias: str,
         QuestionId: str,
         SelectedChoices: Sequence[str] = ...,
         ChoiceUpdates: Mapping[str, ChoiceUpdateTypeDef] = ...,
         Notes: str = ...,
         IsApplicable: bool = ...,
-        Reason: AnswerReasonType = ...
+        Reason: AnswerReasonType = ...,
     ) -> UpdateAnswerOutputTypeDef:
         """
         Update the answer to a specific question in a workload review.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.update_answer)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#update_answer)
         """
 
     def update_global_settings(
         self,
         *,
         OrganizationSharingStatus: OrganizationSharingStatusType = ...,
-        DiscoveryIntegrationStatus: DiscoveryIntegrationStatusType = ...
+        DiscoveryIntegrationStatus: DiscoveryIntegrationStatusType = ...,
+        JiraConfiguration: AccountJiraConfigurationInputTypeDef = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
-        Updates whether the Amazon Web Services account is opted into organization
+        Update whether the Amazon Web Services account is opted into organization
         sharing and discovery integration
         features.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.update_global_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#update_global_settings)
         """
 
+    def update_integration(
+        self, *, WorkloadId: str, ClientRequestToken: str, IntegratingService: Literal["JIRA"]
+    ) -> EmptyResponseMetadataTypeDef:
+        """
+        Update integration features.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.update_integration)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#update_integration)
+        """
+
     def update_lens_review(
         self,
         *,
         WorkloadId: str,
         LensAlias: str,
         LensNotes: str = ...,
-        PillarNotes: Mapping[str, str] = ...
+        PillarNotes: Mapping[str, str] = ...,
+        JiraConfiguration: JiraSelectedQuestionConfigurationTypeDef = ...,
     ) -> UpdateLensReviewOutputTypeDef:
         """
         Update lens review for a particular workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.update_lens_review)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#update_lens_review)
         """
 
     def update_profile(
         self,
         *,
         ProfileArn: str,
         ProfileDescription: str = ...,
-        ProfileQuestions: Sequence[ProfileQuestionUpdateTypeDef] = ...
+        ProfileQuestions: Sequence[ProfileQuestionUpdateTypeDef] = ...,
     ) -> UpdateProfileOutputTypeDef:
         """
         Update a profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.update_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#update_profile)
         """
@@ -921,15 +952,15 @@
         self,
         *,
         TemplateArn: str,
         TemplateName: str = ...,
         Description: str = ...,
         Notes: str = ...,
         LensesToAssociate: Sequence[str] = ...,
-        LensesToDisassociate: Sequence[str] = ...
+        LensesToDisassociate: Sequence[str] = ...,
     ) -> UpdateReviewTemplateOutputTypeDef:
         """
         Update a review template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.update_review_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#update_review_template)
         """
@@ -940,30 +971,30 @@
         TemplateArn: str,
         LensAlias: str,
         QuestionId: str,
         SelectedChoices: Sequence[str] = ...,
         ChoiceUpdates: Mapping[str, ChoiceUpdateTypeDef] = ...,
         Notes: str = ...,
         IsApplicable: bool = ...,
-        Reason: AnswerReasonType = ...
+        Reason: AnswerReasonType = ...,
     ) -> UpdateReviewTemplateAnswerOutputTypeDef:
         """
         Update a review template answer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.update_review_template_answer)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#update_review_template_answer)
         """
 
     def update_review_template_lens_review(
         self,
         *,
         TemplateArn: str,
         LensAlias: str,
         LensNotes: str = ...,
-        PillarNotes: Mapping[str, str] = ...
+        PillarNotes: Mapping[str, str] = ...,
     ) -> UpdateReviewTemplateLensReviewOutputTypeDef:
         """
         Update a lens review associated with a review template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.update_review_template_lens_review)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#update_review_template_lens_review)
         """
@@ -993,15 +1024,16 @@
         ReviewOwner: str = ...,
         IsReviewOwnerUpdateAcknowledged: bool = ...,
         IndustryType: str = ...,
         Industry: str = ...,
         Notes: str = ...,
         ImprovementStatus: WorkloadImprovementStatusType = ...,
         DiscoveryConfig: WorkloadDiscoveryConfigTypeDef = ...,
-        Applications: Sequence[str] = ...
+        Applications: Sequence[str] = ...,
+        JiraConfiguration: WorkloadJiraConfigurationInputTypeDef = ...,
     ) -> UpdateWorkloadOutputTypeDef:
         """
         Update an existing workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.update_workload)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#update_workload)
         """
@@ -1028,15 +1060,15 @@
 
     def upgrade_profile_version(
         self,
         *,
         WorkloadId: str,
         ProfileArn: str,
         MilestoneName: str = ...,
-        ClientRequestToken: str = ...
+        ClientRequestToken: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Upgrade a profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.upgrade_profile_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#upgrade_profile_version)
         """
```

### Comparing `mypy-boto3-wellarchitected-1.34.0/mypy_boto3_wellarchitected/literals.py` & `mypy_boto3_wellarchitected-1.34.85/mypy_boto3_wellarchitected/literals.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,40 +2,44 @@
 Type annotations for wellarchitected service literal definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/literals/)
 
 Usage::
 
     ```python
-    from mypy_boto3_wellarchitected.literals import AdditionalResourceTypeType
+    from mypy_boto3_wellarchitected.literals import AccountJiraIssueManagementStatusType
 
-    data: AdditionalResourceTypeType = "HELPFUL_RESOURCE"
+    data: AccountJiraIssueManagementStatusType = "DISABLED"
     ```
 """
 
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
+    "AccountJiraIssueManagementStatusType",
     "AdditionalResourceTypeType",
     "AnswerReasonType",
     "CheckFailureReasonType",
     "CheckProviderType",
     "CheckStatusType",
     "ChoiceReasonType",
     "ChoiceStatusType",
     "DefinitionTypeType",
     "DifferenceStatusType",
     "DiscoveryIntegrationStatusType",
     "ImportLensStatusType",
+    "IntegratingServiceType",
+    "IntegrationStatusInputType",
+    "IntegrationStatusType",
+    "IssueManagementTypeType",
     "LensStatusType",
     "LensStatusTypeType",
     "LensTypeType",
     "MetricTypeType",
     "NotificationTypeType",
     "OrganizationSharingStatusType",
     "PermissionTypeType",
@@ -50,21 +54,22 @@
     "RiskType",
     "ShareInvitationActionType",
     "ShareResourceTypeType",
     "ShareStatusType",
     "TrustedAdvisorIntegrationStatusType",
     "WorkloadEnvironmentType",
     "WorkloadImprovementStatusType",
+    "WorkloadIssueManagementStatusType",
     "WellArchitectedServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
+AccountJiraIssueManagementStatusType = Literal["DISABLED", "ENABLED"]
 AdditionalResourceTypeType = Literal["HELPFUL_RESOURCE", "IMPROVEMENT_PLAN"]
 AnswerReasonType = Literal[
     "ARCHITECTURE_CONSTRAINTS", "BUSINESS_PRIORITIES", "NONE", "OTHER", "OUT_OF_SCOPE"
 ]
 CheckFailureReasonType = Literal[
     "ACCESS_DENIED", "ASSUME_ROLE_ERROR", "PREMIUM_SUPPORT_REQUIRED", "UNKNOWN_ERROR"
 ]
@@ -74,14 +79,18 @@
     "ARCHITECTURE_CONSTRAINTS", "BUSINESS_PRIORITIES", "NONE", "OTHER", "OUT_OF_SCOPE"
 ]
 ChoiceStatusType = Literal["NOT_APPLICABLE", "SELECTED", "UNSELECTED"]
 DefinitionTypeType = Literal["APP_REGISTRY", "WORKLOAD_METADATA"]
 DifferenceStatusType = Literal["DELETED", "NEW", "UPDATED"]
 DiscoveryIntegrationStatusType = Literal["DISABLED", "ENABLED"]
 ImportLensStatusType = Literal["COMPLETE", "ERROR", "IN_PROGRESS"]
+IntegratingServiceType = Literal["JIRA"]
+IntegrationStatusInputType = Literal["NOT_CONFIGURED"]
+IntegrationStatusType = Literal["CONFIGURED", "NOT_CONFIGURED"]
+IssueManagementTypeType = Literal["AUTO", "MANUAL"]
 LensStatusType = Literal["CURRENT", "DELETED", "DEPRECATED", "NOT_CURRENT", "UNSHARED"]
 LensStatusTypeType = Literal["ALL", "DRAFT", "PUBLISHED"]
 LensTypeType = Literal["AWS_OFFICIAL", "CUSTOM_SELF", "CUSTOM_SHARED"]
 MetricTypeType = Literal["WORKLOAD"]
 NotificationTypeType = Literal["LENS_VERSION_DEPRECATED", "LENS_VERSION_UPGRADED"]
 OrganizationSharingStatusType = Literal["DISABLED", "ENABLED"]
 PermissionTypeType = Literal["CONTRIBUTOR", "READONLY"]
@@ -100,14 +109,15 @@
     "ACCEPTED", "ASSOCIATED", "ASSOCIATING", "EXPIRED", "FAILED", "PENDING", "REJECTED", "REVOKED"
 ]
 TrustedAdvisorIntegrationStatusType = Literal["DISABLED", "ENABLED"]
 WorkloadEnvironmentType = Literal["PREPRODUCTION", "PRODUCTION"]
 WorkloadImprovementStatusType = Literal[
     "COMPLETE", "IN_PROGRESS", "NOT_APPLICABLE", "NOT_STARTED", "RISK_ACKNOWLEDGED"
 ]
+WorkloadIssueManagementStatusType = Literal["DISABLED", "ENABLED", "INHERIT"]
 WellArchitectedServiceName = Literal["wellarchitected"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
@@ -127,14 +137,15 @@
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
@@ -145,14 +156,15 @@
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
@@ -170,14 +182,15 @@
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
@@ -190,24 +203,26 @@
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
@@ -268,15 +283,14 @@
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
@@ -348,17 +362,19 @@
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
@@ -448,19 +464,21 @@
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
```

### Comparing `mypy-boto3-wellarchitected-1.34.0/mypy_boto3_wellarchitected/literals.pyi` & `mypy_boto3_wellarchitected-1.34.85/mypy_boto3_wellarchitected/literals.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -2,39 +2,44 @@
 Type annotations for wellarchitected service literal definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/literals/)
 
 Usage::
 
     ```python
-    from mypy_boto3_wellarchitected.literals import AdditionalResourceTypeType
+    from mypy_boto3_wellarchitected.literals import AccountJiraIssueManagementStatusType
 
-    data: AdditionalResourceTypeType = "HELPFUL_RESOURCE"
+    data: AccountJiraIssueManagementStatusType = "DISABLED"
     ```
 """
 
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = (
+    "AccountJiraIssueManagementStatusType",
     "AdditionalResourceTypeType",
     "AnswerReasonType",
     "CheckFailureReasonType",
     "CheckProviderType",
     "CheckStatusType",
     "ChoiceReasonType",
     "ChoiceStatusType",
     "DefinitionTypeType",
     "DifferenceStatusType",
     "DiscoveryIntegrationStatusType",
     "ImportLensStatusType",
+    "IntegratingServiceType",
+    "IntegrationStatusInputType",
+    "IntegrationStatusType",
+    "IssueManagementTypeType",
     "LensStatusType",
     "LensStatusTypeType",
     "LensTypeType",
     "MetricTypeType",
     "NotificationTypeType",
     "OrganizationSharingStatusType",
     "PermissionTypeType",
@@ -49,20 +54,22 @@
     "RiskType",
     "ShareInvitationActionType",
     "ShareResourceTypeType",
     "ShareStatusType",
     "TrustedAdvisorIntegrationStatusType",
     "WorkloadEnvironmentType",
     "WorkloadImprovementStatusType",
+    "WorkloadIssueManagementStatusType",
     "WellArchitectedServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
+AccountJiraIssueManagementStatusType = Literal["DISABLED", "ENABLED"]
 AdditionalResourceTypeType = Literal["HELPFUL_RESOURCE", "IMPROVEMENT_PLAN"]
 AnswerReasonType = Literal[
     "ARCHITECTURE_CONSTRAINTS", "BUSINESS_PRIORITIES", "NONE", "OTHER", "OUT_OF_SCOPE"
 ]
 CheckFailureReasonType = Literal[
     "ACCESS_DENIED", "ASSUME_ROLE_ERROR", "PREMIUM_SUPPORT_REQUIRED", "UNKNOWN_ERROR"
 ]
@@ -72,14 +79,18 @@
     "ARCHITECTURE_CONSTRAINTS", "BUSINESS_PRIORITIES", "NONE", "OTHER", "OUT_OF_SCOPE"
 ]
 ChoiceStatusType = Literal["NOT_APPLICABLE", "SELECTED", "UNSELECTED"]
 DefinitionTypeType = Literal["APP_REGISTRY", "WORKLOAD_METADATA"]
 DifferenceStatusType = Literal["DELETED", "NEW", "UPDATED"]
 DiscoveryIntegrationStatusType = Literal["DISABLED", "ENABLED"]
 ImportLensStatusType = Literal["COMPLETE", "ERROR", "IN_PROGRESS"]
+IntegratingServiceType = Literal["JIRA"]
+IntegrationStatusInputType = Literal["NOT_CONFIGURED"]
+IntegrationStatusType = Literal["CONFIGURED", "NOT_CONFIGURED"]
+IssueManagementTypeType = Literal["AUTO", "MANUAL"]
 LensStatusType = Literal["CURRENT", "DELETED", "DEPRECATED", "NOT_CURRENT", "UNSHARED"]
 LensStatusTypeType = Literal["ALL", "DRAFT", "PUBLISHED"]
 LensTypeType = Literal["AWS_OFFICIAL", "CUSTOM_SELF", "CUSTOM_SHARED"]
 MetricTypeType = Literal["WORKLOAD"]
 NotificationTypeType = Literal["LENS_VERSION_DEPRECATED", "LENS_VERSION_UPGRADED"]
 OrganizationSharingStatusType = Literal["DISABLED", "ENABLED"]
 PermissionTypeType = Literal["CONTRIBUTOR", "READONLY"]
@@ -98,14 +109,15 @@
     "ACCEPTED", "ASSOCIATED", "ASSOCIATING", "EXPIRED", "FAILED", "PENDING", "REJECTED", "REVOKED"
 ]
 TrustedAdvisorIntegrationStatusType = Literal["DISABLED", "ENABLED"]
 WorkloadEnvironmentType = Literal["PREPRODUCTION", "PRODUCTION"]
 WorkloadImprovementStatusType = Literal[
     "COMPLETE", "IN_PROGRESS", "NOT_APPLICABLE", "NOT_STARTED", "RISK_ACKNOWLEDGED"
 ]
+WorkloadIssueManagementStatusType = Literal["DISABLED", "ENABLED", "INHERIT"]
 WellArchitectedServiceName = Literal["wellarchitected"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
@@ -125,14 +137,15 @@
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
@@ -143,14 +156,15 @@
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
@@ -168,14 +182,15 @@
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
@@ -188,24 +203,26 @@
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
@@ -266,15 +283,14 @@
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
@@ -346,17 +362,19 @@
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
@@ -446,19 +464,21 @@
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
```

### Comparing `mypy-boto3-wellarchitected-1.34.0/mypy_boto3_wellarchitected/type_defs.py` & `mypy_boto3_wellarchitected-1.34.85/mypy_boto3_wellarchitected/type_defs.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,35 +2,38 @@
 Type annotations for wellarchitected service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_wellarchitected.type_defs import ChoiceContentTypeDef
+    from mypy_boto3_wellarchitected.type_defs import AccountJiraConfigurationInputTypeDef
 
-    data: ChoiceContentTypeDef = ...
+    data: AccountJiraConfigurationInputTypeDef = ...
     ```
 """
 
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
+    AccountJiraIssueManagementStatusType,
     AdditionalResourceTypeType,
     AnswerReasonType,
     CheckFailureReasonType,
     CheckStatusType,
     ChoiceReasonType,
     ChoiceStatusType,
     DefinitionTypeType,
     DifferenceStatusType,
     DiscoveryIntegrationStatusType,
     ImportLensStatusType,
+    IntegrationStatusType,
+    IssueManagementTypeType,
     LensStatusType,
     LensStatusTypeType,
     LensTypeType,
     NotificationTypeType,
     OrganizationSharingStatusType,
     PermissionTypeType,
     ProfileNotificationTypeType,
@@ -44,14 +47,15 @@
     RiskType,
     ShareInvitationActionType,
     ShareResourceTypeType,
     ShareStatusType,
     TrustedAdvisorIntegrationStatusType,
     WorkloadEnvironmentType,
     WorkloadImprovementStatusType,
+    WorkloadIssueManagementStatusType,
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 12):
@@ -59,18 +63,20 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
+    "AccountJiraConfigurationInputTypeDef",
+    "AccountJiraConfigurationOutputTypeDef",
     "ChoiceContentTypeDef",
     "ChoiceAnswerSummaryTypeDef",
+    "JiraConfigurationTypeDef",
     "ChoiceAnswerTypeDef",
     "AssociateLensesInputRequestTypeDef",
     "AssociateProfilesInputRequestTypeDef",
     "BestPracticeTypeDef",
     "CheckDetailTypeDef",
     "CheckSummaryTypeDef",
     "ChoiceImprovementPlanTypeDef",
@@ -80,14 +86,15 @@
     "CreateLensVersionInputRequestTypeDef",
     "CreateMilestoneInputRequestTypeDef",
     "ProfileQuestionUpdateTypeDef",
     "CreateProfileShareInputRequestTypeDef",
     "CreateReviewTemplateInputRequestTypeDef",
     "CreateTemplateShareInputRequestTypeDef",
     "WorkloadDiscoveryConfigTypeDef",
+    "WorkloadJiraConfigurationInputTypeDef",
     "CreateWorkloadShareInputRequestTypeDef",
     "DeleteLensInputRequestTypeDef",
     "DeleteLensShareInputRequestTypeDef",
     "DeleteProfileInputRequestTypeDef",
     "DeleteProfileShareInputRequestTypeDef",
     "DeleteReviewTemplateInputRequestTypeDef",
     "DeleteTemplateShareInputRequestTypeDef",
@@ -108,14 +115,15 @@
     "GetProfileInputRequestTypeDef",
     "GetReviewTemplateAnswerInputRequestTypeDef",
     "GetReviewTemplateInputRequestTypeDef",
     "GetReviewTemplateLensReviewInputRequestTypeDef",
     "ReviewTemplateTypeDef",
     "GetWorkloadInputRequestTypeDef",
     "ImportLensInputRequestTypeDef",
+    "SelectedPillarTypeDef",
     "WorkloadProfileTypeDef",
     "PillarReviewSummaryTypeDef",
     "LensShareSummaryTypeDef",
     "LensSummaryTypeDef",
     "LensUpgradeSummaryTypeDef",
     "ListAnswersInputRequestTypeDef",
     "ListCheckDetailsInputRequestTypeDef",
@@ -146,24 +154,25 @@
     "QuestionDifferenceTypeDef",
     "ProfileChoiceTypeDef",
     "ProfileTemplateChoiceTypeDef",
     "ReviewTemplatePillarReviewSummaryTypeDef",
     "ShareInvitationTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
-    "UpdateGlobalSettingsInputRequestTypeDef",
-    "UpdateLensReviewInputRequestTypeDef",
+    "UpdateIntegrationInputRequestTypeDef",
     "UpdateReviewTemplateInputRequestTypeDef",
     "UpdateReviewTemplateLensReviewInputRequestTypeDef",
     "UpdateShareInvitationInputRequestTypeDef",
     "UpdateWorkloadShareInputRequestTypeDef",
     "WorkloadShareTypeDef",
     "UpgradeLensReviewInputRequestTypeDef",
     "UpgradeProfileVersionInputRequestTypeDef",
     "UpgradeReviewTemplateLensReviewInputRequestTypeDef",
+    "WorkloadJiraConfigurationOutputTypeDef",
+    "UpdateGlobalSettingsInputRequestTypeDef",
     "AdditionalResourcesTypeDef",
     "QuestionMetricTypeDef",
     "ImprovementSummaryTypeDef",
     "UpdateAnswerInputRequestTypeDef",
     "UpdateReviewTemplateAnswerInputRequestTypeDef",
     "CreateLensShareOutputTypeDef",
     "CreateLensVersionOutputTypeDef",
@@ -172,30 +181,30 @@
     "CreateProfileShareOutputTypeDef",
     "CreateReviewTemplateOutputTypeDef",
     "CreateTemplateShareOutputTypeDef",
     "CreateWorkloadOutputTypeDef",
     "CreateWorkloadShareOutputTypeDef",
     "EmptyResponseMetadataTypeDef",
     "ExportLensOutputTypeDef",
+    "GetGlobalSettingsOutputTypeDef",
     "ImportLensOutputTypeDef",
     "ListCheckDetailsOutputTypeDef",
     "ListCheckSummariesOutputTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "CreateProfileInputRequestTypeDef",
     "UpdateProfileInputRequestTypeDef",
     "CreateWorkloadInputRequestTypeDef",
     "UpdateWorkloadInputRequestTypeDef",
     "GetLensOutputTypeDef",
     "GetLensReviewReportOutputTypeDef",
     "GetReviewTemplateOutputTypeDef",
     "UpdateReviewTemplateOutputTypeDef",
+    "JiraSelectedQuestionConfigurationTypeDef",
     "LensReviewSummaryTypeDef",
     "WorkloadSummaryTypeDef",
-    "WorkloadTypeDef",
-    "LensReviewTypeDef",
     "ListLensSharesOutputTypeDef",
     "ListLensesOutputTypeDef",
     "NotificationSummaryTypeDef",
     "ListProfileNotificationsOutputTypeDef",
     "ListProfileSharesOutputTypeDef",
     "ListProfilesOutputTypeDef",
     "ListReviewTemplatesOutputTypeDef",
@@ -204,52 +213,75 @@
     "ListWorkloadSharesOutputTypeDef",
     "PillarDifferenceTypeDef",
     "ProfileQuestionTypeDef",
     "ProfileTemplateQuestionTypeDef",
     "ReviewTemplateLensReviewTypeDef",
     "UpdateShareInvitationOutputTypeDef",
     "UpdateWorkloadShareOutputTypeDef",
+    "WorkloadTypeDef",
     "ChoiceTypeDef",
     "PillarMetricTypeDef",
     "ListLensReviewImprovementsOutputTypeDef",
+    "LensReviewTypeDef",
+    "UpdateLensReviewInputRequestTypeDef",
     "ListLensReviewsOutputTypeDef",
     "ListWorkloadsOutputTypeDef",
     "MilestoneSummaryTypeDef",
-    "GetWorkloadOutputTypeDef",
-    "MilestoneTypeDef",
-    "UpdateWorkloadOutputTypeDef",
-    "GetLensReviewOutputTypeDef",
-    "UpdateLensReviewOutputTypeDef",
     "ListNotificationsOutputTypeDef",
     "VersionDifferencesTypeDef",
     "ProfileTypeDef",
     "ProfileTemplateTypeDef",
     "GetReviewTemplateLensReviewOutputTypeDef",
     "UpdateReviewTemplateLensReviewOutputTypeDef",
+    "GetWorkloadOutputTypeDef",
+    "MilestoneTypeDef",
+    "UpdateWorkloadOutputTypeDef",
     "AnswerSummaryTypeDef",
     "AnswerTypeDef",
     "ReviewTemplateAnswerSummaryTypeDef",
     "ReviewTemplateAnswerTypeDef",
     "LensMetricTypeDef",
+    "GetLensReviewOutputTypeDef",
+    "UpdateLensReviewOutputTypeDef",
     "ListMilestonesOutputTypeDef",
-    "GetMilestoneOutputTypeDef",
     "GetLensVersionDifferenceOutputTypeDef",
     "GetProfileOutputTypeDef",
     "UpdateProfileOutputTypeDef",
     "GetProfileTemplateOutputTypeDef",
+    "GetMilestoneOutputTypeDef",
     "ListAnswersOutputTypeDef",
     "GetAnswerOutputTypeDef",
     "UpdateAnswerOutputTypeDef",
     "ListReviewTemplateAnswersOutputTypeDef",
     "GetReviewTemplateAnswerOutputTypeDef",
     "UpdateReviewTemplateAnswerOutputTypeDef",
     "ConsolidatedReportMetricTypeDef",
     "GetConsolidatedReportOutputTypeDef",
 )
 
+AccountJiraConfigurationInputTypeDef = TypedDict(
+    "AccountJiraConfigurationInputTypeDef",
+    {
+        "IssueManagementStatus": NotRequired[AccountJiraIssueManagementStatusType],
+        "IssueManagementType": NotRequired[IssueManagementTypeType],
+        "JiraProjectKey": NotRequired[str],
+        "IntegrationStatus": NotRequired[Literal["NOT_CONFIGURED"]],
+    },
+)
+AccountJiraConfigurationOutputTypeDef = TypedDict(
+    "AccountJiraConfigurationOutputTypeDef",
+    {
+        "IntegrationStatus": NotRequired[IntegrationStatusType],
+        "IssueManagementStatus": NotRequired[AccountJiraIssueManagementStatusType],
+        "IssueManagementType": NotRequired[IssueManagementTypeType],
+        "Subdomain": NotRequired[str],
+        "JiraProjectKey": NotRequired[str],
+        "StatusMessage": NotRequired[str],
+    },
+)
 ChoiceContentTypeDef = TypedDict(
     "ChoiceContentTypeDef",
     {
         "DisplayText": NotRequired[str],
         "Url": NotRequired[str],
     },
 )
@@ -257,14 +289,21 @@
     "ChoiceAnswerSummaryTypeDef",
     {
         "ChoiceId": NotRequired[str],
         "Status": NotRequired[ChoiceStatusType],
         "Reason": NotRequired[ChoiceReasonType],
     },
 )
+JiraConfigurationTypeDef = TypedDict(
+    "JiraConfigurationTypeDef",
+    {
+        "JiraIssueUrl": NotRequired[str],
+        "LastSyncedTime": NotRequired[datetime],
+    },
+)
 ChoiceAnswerTypeDef = TypedDict(
     "ChoiceAnswerTypeDef",
     {
         "ChoiceId": NotRequired[str],
         "Status": NotRequired[ChoiceStatusType],
         "Reason": NotRequired[ChoiceReasonType],
         "Notes": NotRequired[str],
@@ -349,18 +388,18 @@
         "ClientRequestToken": str,
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
 CreateLensVersionInputRequestTypeDef = TypedDict(
     "CreateLensVersionInputRequestTypeDef",
     {
         "LensAlias": str,
         "LensVersion": str,
@@ -413,14 +452,22 @@
 WorkloadDiscoveryConfigTypeDef = TypedDict(
     "WorkloadDiscoveryConfigTypeDef",
     {
         "TrustedAdvisorIntegrationStatus": NotRequired[TrustedAdvisorIntegrationStatusType],
         "WorkloadResourceDefinition": NotRequired[Sequence[DefinitionTypeType]],
     },
 )
+WorkloadJiraConfigurationInputTypeDef = TypedDict(
+    "WorkloadJiraConfigurationInputTypeDef",
+    {
+        "IssueManagementStatus": NotRequired[WorkloadIssueManagementStatusType],
+        "IssueManagementType": NotRequired[IssueManagementTypeType],
+        "JiraProjectKey": NotRequired[str],
+    },
+)
 CreateWorkloadShareInputRequestTypeDef = TypedDict(
     "CreateWorkloadShareInputRequestTypeDef",
     {
         "WorkloadId": str,
         "SharedWith": str,
         "PermissionType": PermissionTypeType,
         "ClientRequestToken": str,
@@ -639,14 +686,21 @@
     {
         "JSONString": str,
         "ClientRequestToken": str,
         "LensAlias": NotRequired[str],
         "Tags": NotRequired[Mapping[str, str]],
     },
 )
+SelectedPillarTypeDef = TypedDict(
+    "SelectedPillarTypeDef",
+    {
+        "PillarId": NotRequired[str],
+        "SelectedQuestionIds": NotRequired[List[str]],
+    },
+)
 WorkloadProfileTypeDef = TypedDict(
     "WorkloadProfileTypeDef",
     {
         "ProfileArn": NotRequired[str],
         "ProfileVersion": NotRequired[str],
     },
 )
@@ -1018,28 +1072,20 @@
 UntagResourceInputRequestTypeDef = TypedDict(
     "UntagResourceInputRequestTypeDef",
     {
         "WorkloadArn": str,
         "TagKeys": Sequence[str],
     },
 )
-UpdateGlobalSettingsInputRequestTypeDef = TypedDict(
-    "UpdateGlobalSettingsInputRequestTypeDef",
-    {
-        "OrganizationSharingStatus": NotRequired[OrganizationSharingStatusType],
-        "DiscoveryIntegrationStatus": NotRequired[DiscoveryIntegrationStatusType],
-    },
-)
-UpdateLensReviewInputRequestTypeDef = TypedDict(
-    "UpdateLensReviewInputRequestTypeDef",
+UpdateIntegrationInputRequestTypeDef = TypedDict(
+    "UpdateIntegrationInputRequestTypeDef",
     {
         "WorkloadId": str,
-        "LensAlias": str,
-        "LensNotes": NotRequired[str],
-        "PillarNotes": NotRequired[Mapping[str, str]],
+        "ClientRequestToken": str,
+        "IntegratingService": Literal["JIRA"],
     },
 )
 UpdateReviewTemplateInputRequestTypeDef = TypedDict(
     "UpdateReviewTemplateInputRequestTypeDef",
     {
         "TemplateArn": str,
         "TemplateName": NotRequired[str],
@@ -1107,14 +1153,31 @@
     "UpgradeReviewTemplateLensReviewInputRequestTypeDef",
     {
         "TemplateArn": str,
         "LensAlias": str,
         "ClientRequestToken": NotRequired[str],
     },
 )
+WorkloadJiraConfigurationOutputTypeDef = TypedDict(
+    "WorkloadJiraConfigurationOutputTypeDef",
+    {
+        "IssueManagementStatus": NotRequired[WorkloadIssueManagementStatusType],
+        "IssueManagementType": NotRequired[IssueManagementTypeType],
+        "JiraProjectKey": NotRequired[str],
+        "StatusMessage": NotRequired[str],
+    },
+)
+UpdateGlobalSettingsInputRequestTypeDef = TypedDict(
+    "UpdateGlobalSettingsInputRequestTypeDef",
+    {
+        "OrganizationSharingStatus": NotRequired[OrganizationSharingStatusType],
+        "DiscoveryIntegrationStatus": NotRequired[DiscoveryIntegrationStatusType],
+        "JiraConfiguration": NotRequired[AccountJiraConfigurationInputTypeDef],
+    },
+)
 AdditionalResourcesTypeDef = TypedDict(
     "AdditionalResourcesTypeDef",
     {
         "Type": NotRequired[AdditionalResourceTypeType],
         "Content": NotRequired[List[ChoiceContentTypeDef]],
     },
 )
@@ -1131,14 +1194,15 @@
     {
         "QuestionId": NotRequired[str],
         "PillarId": NotRequired[str],
         "QuestionTitle": NotRequired[str],
         "Risk": NotRequired[RiskType],
         "ImprovementPlanUrl": NotRequired[str],
         "ImprovementPlans": NotRequired[List[ChoiceImprovementPlanTypeDef]],
+        "JiraConfiguration": NotRequired[JiraConfigurationTypeDef],
     },
 )
 UpdateAnswerInputRequestTypeDef = TypedDict(
     "UpdateAnswerInputRequestTypeDef",
     {
         "WorkloadId": str,
         "LensAlias": str,
@@ -1242,14 +1306,23 @@
 ExportLensOutputTypeDef = TypedDict(
     "ExportLensOutputTypeDef",
     {
         "LensJSON": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+GetGlobalSettingsOutputTypeDef = TypedDict(
+    "GetGlobalSettingsOutputTypeDef",
+    {
+        "OrganizationSharingStatus": OrganizationSharingStatusType,
+        "DiscoveryIntegrationStatus": DiscoveryIntegrationStatusType,
+        "JiraConfiguration": AccountJiraConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 ImportLensOutputTypeDef = TypedDict(
     "ImportLensOutputTypeDef",
     {
         "LensArn": str,
         "Status": ImportLensStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1313,14 +1386,15 @@
         "Industry": NotRequired[str],
         "Notes": NotRequired[str],
         "Tags": NotRequired[Mapping[str, str]],
         "DiscoveryConfig": NotRequired[WorkloadDiscoveryConfigTypeDef],
         "Applications": NotRequired[Sequence[str]],
         "ProfileArns": NotRequired[Sequence[str]],
         "ReviewTemplateArns": NotRequired[Sequence[str]],
+        "JiraConfiguration": NotRequired[WorkloadJiraConfigurationInputTypeDef],
     },
 )
 UpdateWorkloadInputRequestTypeDef = TypedDict(
     "UpdateWorkloadInputRequestTypeDef",
     {
         "WorkloadId": str,
         "WorkloadName": NotRequired[str],
@@ -1335,14 +1409,15 @@
         "IsReviewOwnerUpdateAcknowledged": NotRequired[bool],
         "IndustryType": NotRequired[str],
         "Industry": NotRequired[str],
         "Notes": NotRequired[str],
         "ImprovementStatus": NotRequired[WorkloadImprovementStatusType],
         "DiscoveryConfig": NotRequired[WorkloadDiscoveryConfigTypeDef],
         "Applications": NotRequired[Sequence[str]],
+        "JiraConfiguration": NotRequired[WorkloadJiraConfigurationInputTypeDef],
     },
 )
 GetLensOutputTypeDef = TypedDict(
     "GetLensOutputTypeDef",
     {
         "Lens": LensTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1367,14 +1442,20 @@
 UpdateReviewTemplateOutputTypeDef = TypedDict(
     "UpdateReviewTemplateOutputTypeDef",
     {
         "ReviewTemplate": ReviewTemplateTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+JiraSelectedQuestionConfigurationTypeDef = TypedDict(
+    "JiraSelectedQuestionConfigurationTypeDef",
+    {
+        "SelectedPillars": NotRequired[List[SelectedPillarTypeDef]],
+    },
+)
 LensReviewSummaryTypeDef = TypedDict(
     "LensReviewSummaryTypeDef",
     {
         "LensAlias": NotRequired[str],
         "LensArn": NotRequired[str],
         "LensVersion": NotRequired[str],
         "LensName": NotRequired[str],
@@ -1396,63 +1477,14 @@
         "Lenses": NotRequired[List[str]],
         "RiskCounts": NotRequired[Dict[RiskType, int]],
         "ImprovementStatus": NotRequired[WorkloadImprovementStatusType],
         "Profiles": NotRequired[List[WorkloadProfileTypeDef]],
         "PrioritizedRiskCounts": NotRequired[Dict[RiskType, int]],
     },
 )
-WorkloadTypeDef = TypedDict(
-    "WorkloadTypeDef",
-    {
-        "WorkloadId": NotRequired[str],
-        "WorkloadArn": NotRequired[str],
-        "WorkloadName": NotRequired[str],
-        "Description": NotRequired[str],
-        "Environment": NotRequired[WorkloadEnvironmentType],
-        "UpdatedAt": NotRequired[datetime],
-        "AccountIds": NotRequired[List[str]],
-        "AwsRegions": NotRequired[List[str]],
-        "NonAwsRegions": NotRequired[List[str]],
-        "ArchitecturalDesign": NotRequired[str],
-        "ReviewOwner": NotRequired[str],
-        "ReviewRestrictionDate": NotRequired[datetime],
-        "IsReviewOwnerUpdateAcknowledged": NotRequired[bool],
-        "IndustryType": NotRequired[str],
-        "Industry": NotRequired[str],
-        "Notes": NotRequired[str],
-        "ImprovementStatus": NotRequired[WorkloadImprovementStatusType],
-        "RiskCounts": NotRequired[Dict[RiskType, int]],
-        "PillarPriorities": NotRequired[List[str]],
-        "Lenses": NotRequired[List[str]],
-        "Owner": NotRequired[str],
-        "ShareInvitationId": NotRequired[str],
-        "Tags": NotRequired[Dict[str, str]],
-        "DiscoveryConfig": NotRequired[WorkloadDiscoveryConfigTypeDef],
-        "Applications": NotRequired[List[str]],
-        "Profiles": NotRequired[List[WorkloadProfileTypeDef]],
-        "PrioritizedRiskCounts": NotRequired[Dict[RiskType, int]],
-    },
-)
-LensReviewTypeDef = TypedDict(
-    "LensReviewTypeDef",
-    {
-        "LensAlias": NotRequired[str],
-        "LensArn": NotRequired[str],
-        "LensVersion": NotRequired[str],
-        "LensName": NotRequired[str],
-        "LensStatus": NotRequired[LensStatusType],
-        "PillarReviewSummaries": NotRequired[List[PillarReviewSummaryTypeDef]],
-        "UpdatedAt": NotRequired[datetime],
-        "Notes": NotRequired[str],
-        "RiskCounts": NotRequired[Dict[RiskType, int]],
-        "NextToken": NotRequired[str],
-        "Profiles": NotRequired[List[WorkloadProfileTypeDef]],
-        "PrioritizedRiskCounts": NotRequired[Dict[RiskType, int]],
-    },
-)
 ListLensSharesOutputTypeDef = TypedDict(
     "ListLensSharesOutputTypeDef",
     {
         "LensShareSummaries": List[LensShareSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1588,14 +1620,47 @@
     "UpdateWorkloadShareOutputTypeDef",
     {
         "WorkloadId": str,
         "WorkloadShare": WorkloadShareTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+WorkloadTypeDef = TypedDict(
+    "WorkloadTypeDef",
+    {
+        "WorkloadId": NotRequired[str],
+        "WorkloadArn": NotRequired[str],
+        "WorkloadName": NotRequired[str],
+        "Description": NotRequired[str],
+        "Environment": NotRequired[WorkloadEnvironmentType],
+        "UpdatedAt": NotRequired[datetime],
+        "AccountIds": NotRequired[List[str]],
+        "AwsRegions": NotRequired[List[str]],
+        "NonAwsRegions": NotRequired[List[str]],
+        "ArchitecturalDesign": NotRequired[str],
+        "ReviewOwner": NotRequired[str],
+        "ReviewRestrictionDate": NotRequired[datetime],
+        "IsReviewOwnerUpdateAcknowledged": NotRequired[bool],
+        "IndustryType": NotRequired[str],
+        "Industry": NotRequired[str],
+        "Notes": NotRequired[str],
+        "ImprovementStatus": NotRequired[WorkloadImprovementStatusType],
+        "RiskCounts": NotRequired[Dict[RiskType, int]],
+        "PillarPriorities": NotRequired[List[str]],
+        "Lenses": NotRequired[List[str]],
+        "Owner": NotRequired[str],
+        "ShareInvitationId": NotRequired[str],
+        "Tags": NotRequired[Dict[str, str]],
+        "DiscoveryConfig": NotRequired[WorkloadDiscoveryConfigTypeDef],
+        "Applications": NotRequired[List[str]],
+        "Profiles": NotRequired[List[WorkloadProfileTypeDef]],
+        "PrioritizedRiskCounts": NotRequired[Dict[RiskType, int]],
+        "JiraConfiguration": NotRequired[WorkloadJiraConfigurationOutputTypeDef],
+    },
+)
 ChoiceTypeDef = TypedDict(
     "ChoiceTypeDef",
     {
         "ChoiceId": NotRequired[str],
         "Title": NotRequired[str],
         "Description": NotRequired[str],
         "HelpfulResource": NotRequired[ChoiceContentTypeDef],
@@ -1619,14 +1684,42 @@
         "LensAlias": str,
         "LensArn": str,
         "ImprovementSummaries": List[ImprovementSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+LensReviewTypeDef = TypedDict(
+    "LensReviewTypeDef",
+    {
+        "LensAlias": NotRequired[str],
+        "LensArn": NotRequired[str],
+        "LensVersion": NotRequired[str],
+        "LensName": NotRequired[str],
+        "LensStatus": NotRequired[LensStatusType],
+        "PillarReviewSummaries": NotRequired[List[PillarReviewSummaryTypeDef]],
+        "JiraConfiguration": NotRequired[JiraSelectedQuestionConfigurationTypeDef],
+        "UpdatedAt": NotRequired[datetime],
+        "Notes": NotRequired[str],
+        "RiskCounts": NotRequired[Dict[RiskType, int]],
+        "NextToken": NotRequired[str],
+        "Profiles": NotRequired[List[WorkloadProfileTypeDef]],
+        "PrioritizedRiskCounts": NotRequired[Dict[RiskType, int]],
+    },
+)
+UpdateLensReviewInputRequestTypeDef = TypedDict(
+    "UpdateLensReviewInputRequestTypeDef",
+    {
+        "WorkloadId": str,
+        "LensAlias": str,
+        "LensNotes": NotRequired[str],
+        "PillarNotes": NotRequired[Mapping[str, str]],
+        "JiraConfiguration": NotRequired[JiraSelectedQuestionConfigurationTypeDef],
+    },
+)
 ListLensReviewsOutputTypeDef = TypedDict(
     "ListLensReviewsOutputTypeDef",
     {
         "WorkloadId": str,
         "MilestoneNumber": int,
         "LensReviewSummaries": List[LensReviewSummaryTypeDef],
         "NextToken": str,
@@ -1646,54 +1739,14 @@
     {
         "MilestoneNumber": NotRequired[int],
         "MilestoneName": NotRequired[str],
         "RecordedAt": NotRequired[datetime],
         "WorkloadSummary": NotRequired[WorkloadSummaryTypeDef],
     },
 )
-GetWorkloadOutputTypeDef = TypedDict(
-    "GetWorkloadOutputTypeDef",
-    {
-        "Workload": WorkloadTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-MilestoneTypeDef = TypedDict(
-    "MilestoneTypeDef",
-    {
-        "MilestoneNumber": NotRequired[int],
-        "MilestoneName": NotRequired[str],
-        "RecordedAt": NotRequired[datetime],
-        "Workload": NotRequired[WorkloadTypeDef],
-    },
-)
-UpdateWorkloadOutputTypeDef = TypedDict(
-    "UpdateWorkloadOutputTypeDef",
-    {
-        "Workload": WorkloadTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-GetLensReviewOutputTypeDef = TypedDict(
-    "GetLensReviewOutputTypeDef",
-    {
-        "WorkloadId": str,
-        "MilestoneNumber": int,
-        "LensReview": LensReviewTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-UpdateLensReviewOutputTypeDef = TypedDict(
-    "UpdateLensReviewOutputTypeDef",
-    {
-        "WorkloadId": str,
-        "LensReview": LensReviewTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 ListNotificationsOutputTypeDef = TypedDict(
     "ListNotificationsOutputTypeDef",
     {
         "NotificationSummaries": List[NotificationSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1740,27 +1793,51 @@
     "UpdateReviewTemplateLensReviewOutputTypeDef",
     {
         "TemplateArn": str,
         "LensReview": ReviewTemplateLensReviewTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+GetWorkloadOutputTypeDef = TypedDict(
+    "GetWorkloadOutputTypeDef",
+    {
+        "Workload": WorkloadTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+MilestoneTypeDef = TypedDict(
+    "MilestoneTypeDef",
+    {
+        "MilestoneNumber": NotRequired[int],
+        "MilestoneName": NotRequired[str],
+        "RecordedAt": NotRequired[datetime],
+        "Workload": NotRequired[WorkloadTypeDef],
+    },
+)
+UpdateWorkloadOutputTypeDef = TypedDict(
+    "UpdateWorkloadOutputTypeDef",
+    {
+        "Workload": WorkloadTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 AnswerSummaryTypeDef = TypedDict(
     "AnswerSummaryTypeDef",
     {
         "QuestionId": NotRequired[str],
         "PillarId": NotRequired[str],
         "QuestionTitle": NotRequired[str],
         "Choices": NotRequired[List[ChoiceTypeDef]],
         "SelectedChoices": NotRequired[List[str]],
         "ChoiceAnswerSummaries": NotRequired[List[ChoiceAnswerSummaryTypeDef]],
         "IsApplicable": NotRequired[bool],
         "Risk": NotRequired[RiskType],
         "Reason": NotRequired[AnswerReasonType],
         "QuestionType": NotRequired[QuestionTypeType],
+        "JiraConfiguration": NotRequired[JiraConfigurationTypeDef],
     },
 )
 AnswerTypeDef = TypedDict(
     "AnswerTypeDef",
     {
         "QuestionId": NotRequired[str],
         "PillarId": NotRequired[str],
@@ -1772,14 +1849,15 @@
         "Choices": NotRequired[List[ChoiceTypeDef]],
         "SelectedChoices": NotRequired[List[str]],
         "ChoiceAnswers": NotRequired[List[ChoiceAnswerTypeDef]],
         "IsApplicable": NotRequired[bool],
         "Risk": NotRequired[RiskType],
         "Notes": NotRequired[str],
         "Reason": NotRequired[AnswerReasonType],
+        "JiraConfiguration": NotRequired[JiraConfigurationTypeDef],
     },
 )
 ReviewTemplateAnswerSummaryTypeDef = TypedDict(
     "ReviewTemplateAnswerSummaryTypeDef",
     {
         "QuestionId": NotRequired[str],
         "PillarId": NotRequired[str],
@@ -1816,28 +1894,37 @@
     "LensMetricTypeDef",
     {
         "LensArn": NotRequired[str],
         "Pillars": NotRequired[List[PillarMetricTypeDef]],
         "RiskCounts": NotRequired[Dict[RiskType, int]],
     },
 )
-ListMilestonesOutputTypeDef = TypedDict(
-    "ListMilestonesOutputTypeDef",
+GetLensReviewOutputTypeDef = TypedDict(
+    "GetLensReviewOutputTypeDef",
     {
         "WorkloadId": str,
-        "MilestoneSummaries": List[MilestoneSummaryTypeDef],
-        "NextToken": str,
+        "MilestoneNumber": int,
+        "LensReview": LensReviewTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-GetMilestoneOutputTypeDef = TypedDict(
-    "GetMilestoneOutputTypeDef",
+UpdateLensReviewOutputTypeDef = TypedDict(
+    "UpdateLensReviewOutputTypeDef",
     {
         "WorkloadId": str,
-        "Milestone": MilestoneTypeDef,
+        "LensReview": LensReviewTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+ListMilestonesOutputTypeDef = TypedDict(
+    "ListMilestonesOutputTypeDef",
+    {
+        "WorkloadId": str,
+        "MilestoneSummaries": List[MilestoneSummaryTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 GetLensVersionDifferenceOutputTypeDef = TypedDict(
     "GetLensVersionDifferenceOutputTypeDef",
     {
         "LensAlias": str,
@@ -1866,14 +1953,22 @@
 GetProfileTemplateOutputTypeDef = TypedDict(
     "GetProfileTemplateOutputTypeDef",
     {
         "ProfileTemplate": ProfileTemplateTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+GetMilestoneOutputTypeDef = TypedDict(
+    "GetMilestoneOutputTypeDef",
+    {
+        "WorkloadId": str,
+        "Milestone": MilestoneTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 ListAnswersOutputTypeDef = TypedDict(
     "ListAnswersOutputTypeDef",
     {
         "WorkloadId": str,
         "MilestoneNumber": int,
         "LensAlias": str,
         "LensArn": str,
```

### Comparing `mypy-boto3-wellarchitected-1.34.0/mypy_boto3_wellarchitected/type_defs.pyi` & `mypy_boto3_wellarchitected-1.34.85/mypy_boto3_wellarchitected/type_defs.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -2,35 +2,38 @@
 Type annotations for wellarchitected service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_wellarchitected.type_defs import ChoiceContentTypeDef
+    from mypy_boto3_wellarchitected.type_defs import AccountJiraConfigurationInputTypeDef
 
-    data: ChoiceContentTypeDef = ...
+    data: AccountJiraConfigurationInputTypeDef = ...
     ```
 """
 
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
+    AccountJiraIssueManagementStatusType,
     AdditionalResourceTypeType,
     AnswerReasonType,
     CheckFailureReasonType,
     CheckStatusType,
     ChoiceReasonType,
     ChoiceStatusType,
     DefinitionTypeType,
     DifferenceStatusType,
     DiscoveryIntegrationStatusType,
     ImportLensStatusType,
+    IntegrationStatusType,
+    IssueManagementTypeType,
     LensStatusType,
     LensStatusTypeType,
     LensTypeType,
     NotificationTypeType,
     OrganizationSharingStatusType,
     PermissionTypeType,
     ProfileNotificationTypeType,
@@ -44,14 +47,15 @@
     RiskType,
     ShareInvitationActionType,
     ShareResourceTypeType,
     ShareStatusType,
     TrustedAdvisorIntegrationStatusType,
     WorkloadEnvironmentType,
     WorkloadImprovementStatusType,
+    WorkloadIssueManagementStatusType,
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 12):
@@ -60,16 +64,19 @@
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "AccountJiraConfigurationInputTypeDef",
+    "AccountJiraConfigurationOutputTypeDef",
     "ChoiceContentTypeDef",
     "ChoiceAnswerSummaryTypeDef",
+    "JiraConfigurationTypeDef",
     "ChoiceAnswerTypeDef",
     "AssociateLensesInputRequestTypeDef",
     "AssociateProfilesInputRequestTypeDef",
     "BestPracticeTypeDef",
     "CheckDetailTypeDef",
     "CheckSummaryTypeDef",
     "ChoiceImprovementPlanTypeDef",
@@ -79,14 +86,15 @@
     "CreateLensVersionInputRequestTypeDef",
     "CreateMilestoneInputRequestTypeDef",
     "ProfileQuestionUpdateTypeDef",
     "CreateProfileShareInputRequestTypeDef",
     "CreateReviewTemplateInputRequestTypeDef",
     "CreateTemplateShareInputRequestTypeDef",
     "WorkloadDiscoveryConfigTypeDef",
+    "WorkloadJiraConfigurationInputTypeDef",
     "CreateWorkloadShareInputRequestTypeDef",
     "DeleteLensInputRequestTypeDef",
     "DeleteLensShareInputRequestTypeDef",
     "DeleteProfileInputRequestTypeDef",
     "DeleteProfileShareInputRequestTypeDef",
     "DeleteReviewTemplateInputRequestTypeDef",
     "DeleteTemplateShareInputRequestTypeDef",
@@ -107,14 +115,15 @@
     "GetProfileInputRequestTypeDef",
     "GetReviewTemplateAnswerInputRequestTypeDef",
     "GetReviewTemplateInputRequestTypeDef",
     "GetReviewTemplateLensReviewInputRequestTypeDef",
     "ReviewTemplateTypeDef",
     "GetWorkloadInputRequestTypeDef",
     "ImportLensInputRequestTypeDef",
+    "SelectedPillarTypeDef",
     "WorkloadProfileTypeDef",
     "PillarReviewSummaryTypeDef",
     "LensShareSummaryTypeDef",
     "LensSummaryTypeDef",
     "LensUpgradeSummaryTypeDef",
     "ListAnswersInputRequestTypeDef",
     "ListCheckDetailsInputRequestTypeDef",
@@ -145,24 +154,25 @@
     "QuestionDifferenceTypeDef",
     "ProfileChoiceTypeDef",
     "ProfileTemplateChoiceTypeDef",
     "ReviewTemplatePillarReviewSummaryTypeDef",
     "ShareInvitationTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
-    "UpdateGlobalSettingsInputRequestTypeDef",
-    "UpdateLensReviewInputRequestTypeDef",
+    "UpdateIntegrationInputRequestTypeDef",
     "UpdateReviewTemplateInputRequestTypeDef",
     "UpdateReviewTemplateLensReviewInputRequestTypeDef",
     "UpdateShareInvitationInputRequestTypeDef",
     "UpdateWorkloadShareInputRequestTypeDef",
     "WorkloadShareTypeDef",
     "UpgradeLensReviewInputRequestTypeDef",
     "UpgradeProfileVersionInputRequestTypeDef",
     "UpgradeReviewTemplateLensReviewInputRequestTypeDef",
+    "WorkloadJiraConfigurationOutputTypeDef",
+    "UpdateGlobalSettingsInputRequestTypeDef",
     "AdditionalResourcesTypeDef",
     "QuestionMetricTypeDef",
     "ImprovementSummaryTypeDef",
     "UpdateAnswerInputRequestTypeDef",
     "UpdateReviewTemplateAnswerInputRequestTypeDef",
     "CreateLensShareOutputTypeDef",
     "CreateLensVersionOutputTypeDef",
@@ -171,30 +181,30 @@
     "CreateProfileShareOutputTypeDef",
     "CreateReviewTemplateOutputTypeDef",
     "CreateTemplateShareOutputTypeDef",
     "CreateWorkloadOutputTypeDef",
     "CreateWorkloadShareOutputTypeDef",
     "EmptyResponseMetadataTypeDef",
     "ExportLensOutputTypeDef",
+    "GetGlobalSettingsOutputTypeDef",
     "ImportLensOutputTypeDef",
     "ListCheckDetailsOutputTypeDef",
     "ListCheckSummariesOutputTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "CreateProfileInputRequestTypeDef",
     "UpdateProfileInputRequestTypeDef",
     "CreateWorkloadInputRequestTypeDef",
     "UpdateWorkloadInputRequestTypeDef",
     "GetLensOutputTypeDef",
     "GetLensReviewReportOutputTypeDef",
     "GetReviewTemplateOutputTypeDef",
     "UpdateReviewTemplateOutputTypeDef",
+    "JiraSelectedQuestionConfigurationTypeDef",
     "LensReviewSummaryTypeDef",
     "WorkloadSummaryTypeDef",
-    "WorkloadTypeDef",
-    "LensReviewTypeDef",
     "ListLensSharesOutputTypeDef",
     "ListLensesOutputTypeDef",
     "NotificationSummaryTypeDef",
     "ListProfileNotificationsOutputTypeDef",
     "ListProfileSharesOutputTypeDef",
     "ListProfilesOutputTypeDef",
     "ListReviewTemplatesOutputTypeDef",
@@ -203,52 +213,75 @@
     "ListWorkloadSharesOutputTypeDef",
     "PillarDifferenceTypeDef",
     "ProfileQuestionTypeDef",
     "ProfileTemplateQuestionTypeDef",
     "ReviewTemplateLensReviewTypeDef",
     "UpdateShareInvitationOutputTypeDef",
     "UpdateWorkloadShareOutputTypeDef",
+    "WorkloadTypeDef",
     "ChoiceTypeDef",
     "PillarMetricTypeDef",
     "ListLensReviewImprovementsOutputTypeDef",
+    "LensReviewTypeDef",
+    "UpdateLensReviewInputRequestTypeDef",
     "ListLensReviewsOutputTypeDef",
     "ListWorkloadsOutputTypeDef",
     "MilestoneSummaryTypeDef",
-    "GetWorkloadOutputTypeDef",
-    "MilestoneTypeDef",
-    "UpdateWorkloadOutputTypeDef",
-    "GetLensReviewOutputTypeDef",
-    "UpdateLensReviewOutputTypeDef",
     "ListNotificationsOutputTypeDef",
     "VersionDifferencesTypeDef",
     "ProfileTypeDef",
     "ProfileTemplateTypeDef",
     "GetReviewTemplateLensReviewOutputTypeDef",
     "UpdateReviewTemplateLensReviewOutputTypeDef",
+    "GetWorkloadOutputTypeDef",
+    "MilestoneTypeDef",
+    "UpdateWorkloadOutputTypeDef",
     "AnswerSummaryTypeDef",
     "AnswerTypeDef",
     "ReviewTemplateAnswerSummaryTypeDef",
     "ReviewTemplateAnswerTypeDef",
     "LensMetricTypeDef",
+    "GetLensReviewOutputTypeDef",
+    "UpdateLensReviewOutputTypeDef",
     "ListMilestonesOutputTypeDef",
-    "GetMilestoneOutputTypeDef",
     "GetLensVersionDifferenceOutputTypeDef",
     "GetProfileOutputTypeDef",
     "UpdateProfileOutputTypeDef",
     "GetProfileTemplateOutputTypeDef",
+    "GetMilestoneOutputTypeDef",
     "ListAnswersOutputTypeDef",
     "GetAnswerOutputTypeDef",
     "UpdateAnswerOutputTypeDef",
     "ListReviewTemplateAnswersOutputTypeDef",
     "GetReviewTemplateAnswerOutputTypeDef",
     "UpdateReviewTemplateAnswerOutputTypeDef",
     "ConsolidatedReportMetricTypeDef",
     "GetConsolidatedReportOutputTypeDef",
 )
 
+AccountJiraConfigurationInputTypeDef = TypedDict(
+    "AccountJiraConfigurationInputTypeDef",
+    {
+        "IssueManagementStatus": NotRequired[AccountJiraIssueManagementStatusType],
+        "IssueManagementType": NotRequired[IssueManagementTypeType],
+        "JiraProjectKey": NotRequired[str],
+        "IntegrationStatus": NotRequired[Literal["NOT_CONFIGURED"]],
+    },
+)
+AccountJiraConfigurationOutputTypeDef = TypedDict(
+    "AccountJiraConfigurationOutputTypeDef",
+    {
+        "IntegrationStatus": NotRequired[IntegrationStatusType],
+        "IssueManagementStatus": NotRequired[AccountJiraIssueManagementStatusType],
+        "IssueManagementType": NotRequired[IssueManagementTypeType],
+        "Subdomain": NotRequired[str],
+        "JiraProjectKey": NotRequired[str],
+        "StatusMessage": NotRequired[str],
+    },
+)
 ChoiceContentTypeDef = TypedDict(
     "ChoiceContentTypeDef",
     {
         "DisplayText": NotRequired[str],
         "Url": NotRequired[str],
     },
 )
@@ -256,14 +289,21 @@
     "ChoiceAnswerSummaryTypeDef",
     {
         "ChoiceId": NotRequired[str],
         "Status": NotRequired[ChoiceStatusType],
         "Reason": NotRequired[ChoiceReasonType],
     },
 )
+JiraConfigurationTypeDef = TypedDict(
+    "JiraConfigurationTypeDef",
+    {
+        "JiraIssueUrl": NotRequired[str],
+        "LastSyncedTime": NotRequired[datetime],
+    },
+)
 ChoiceAnswerTypeDef = TypedDict(
     "ChoiceAnswerTypeDef",
     {
         "ChoiceId": NotRequired[str],
         "Status": NotRequired[ChoiceStatusType],
         "Reason": NotRequired[ChoiceReasonType],
         "Notes": NotRequired[str],
@@ -348,18 +388,18 @@
         "ClientRequestToken": str,
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
 CreateLensVersionInputRequestTypeDef = TypedDict(
     "CreateLensVersionInputRequestTypeDef",
     {
         "LensAlias": str,
         "LensVersion": str,
@@ -412,14 +452,22 @@
 WorkloadDiscoveryConfigTypeDef = TypedDict(
     "WorkloadDiscoveryConfigTypeDef",
     {
         "TrustedAdvisorIntegrationStatus": NotRequired[TrustedAdvisorIntegrationStatusType],
         "WorkloadResourceDefinition": NotRequired[Sequence[DefinitionTypeType]],
     },
 )
+WorkloadJiraConfigurationInputTypeDef = TypedDict(
+    "WorkloadJiraConfigurationInputTypeDef",
+    {
+        "IssueManagementStatus": NotRequired[WorkloadIssueManagementStatusType],
+        "IssueManagementType": NotRequired[IssueManagementTypeType],
+        "JiraProjectKey": NotRequired[str],
+    },
+)
 CreateWorkloadShareInputRequestTypeDef = TypedDict(
     "CreateWorkloadShareInputRequestTypeDef",
     {
         "WorkloadId": str,
         "SharedWith": str,
         "PermissionType": PermissionTypeType,
         "ClientRequestToken": str,
@@ -638,14 +686,21 @@
     {
         "JSONString": str,
         "ClientRequestToken": str,
         "LensAlias": NotRequired[str],
         "Tags": NotRequired[Mapping[str, str]],
     },
 )
+SelectedPillarTypeDef = TypedDict(
+    "SelectedPillarTypeDef",
+    {
+        "PillarId": NotRequired[str],
+        "SelectedQuestionIds": NotRequired[List[str]],
+    },
+)
 WorkloadProfileTypeDef = TypedDict(
     "WorkloadProfileTypeDef",
     {
         "ProfileArn": NotRequired[str],
         "ProfileVersion": NotRequired[str],
     },
 )
@@ -1017,28 +1072,20 @@
 UntagResourceInputRequestTypeDef = TypedDict(
     "UntagResourceInputRequestTypeDef",
     {
         "WorkloadArn": str,
         "TagKeys": Sequence[str],
     },
 )
-UpdateGlobalSettingsInputRequestTypeDef = TypedDict(
-    "UpdateGlobalSettingsInputRequestTypeDef",
-    {
-        "OrganizationSharingStatus": NotRequired[OrganizationSharingStatusType],
-        "DiscoveryIntegrationStatus": NotRequired[DiscoveryIntegrationStatusType],
-    },
-)
-UpdateLensReviewInputRequestTypeDef = TypedDict(
-    "UpdateLensReviewInputRequestTypeDef",
+UpdateIntegrationInputRequestTypeDef = TypedDict(
+    "UpdateIntegrationInputRequestTypeDef",
     {
         "WorkloadId": str,
-        "LensAlias": str,
-        "LensNotes": NotRequired[str],
-        "PillarNotes": NotRequired[Mapping[str, str]],
+        "ClientRequestToken": str,
+        "IntegratingService": Literal["JIRA"],
     },
 )
 UpdateReviewTemplateInputRequestTypeDef = TypedDict(
     "UpdateReviewTemplateInputRequestTypeDef",
     {
         "TemplateArn": str,
         "TemplateName": NotRequired[str],
@@ -1106,14 +1153,31 @@
     "UpgradeReviewTemplateLensReviewInputRequestTypeDef",
     {
         "TemplateArn": str,
         "LensAlias": str,
         "ClientRequestToken": NotRequired[str],
     },
 )
+WorkloadJiraConfigurationOutputTypeDef = TypedDict(
+    "WorkloadJiraConfigurationOutputTypeDef",
+    {
+        "IssueManagementStatus": NotRequired[WorkloadIssueManagementStatusType],
+        "IssueManagementType": NotRequired[IssueManagementTypeType],
+        "JiraProjectKey": NotRequired[str],
+        "StatusMessage": NotRequired[str],
+    },
+)
+UpdateGlobalSettingsInputRequestTypeDef = TypedDict(
+    "UpdateGlobalSettingsInputRequestTypeDef",
+    {
+        "OrganizationSharingStatus": NotRequired[OrganizationSharingStatusType],
+        "DiscoveryIntegrationStatus": NotRequired[DiscoveryIntegrationStatusType],
+        "JiraConfiguration": NotRequired[AccountJiraConfigurationInputTypeDef],
+    },
+)
 AdditionalResourcesTypeDef = TypedDict(
     "AdditionalResourcesTypeDef",
     {
         "Type": NotRequired[AdditionalResourceTypeType],
         "Content": NotRequired[List[ChoiceContentTypeDef]],
     },
 )
@@ -1130,14 +1194,15 @@
     {
         "QuestionId": NotRequired[str],
         "PillarId": NotRequired[str],
         "QuestionTitle": NotRequired[str],
         "Risk": NotRequired[RiskType],
         "ImprovementPlanUrl": NotRequired[str],
         "ImprovementPlans": NotRequired[List[ChoiceImprovementPlanTypeDef]],
+        "JiraConfiguration": NotRequired[JiraConfigurationTypeDef],
     },
 )
 UpdateAnswerInputRequestTypeDef = TypedDict(
     "UpdateAnswerInputRequestTypeDef",
     {
         "WorkloadId": str,
         "LensAlias": str,
@@ -1241,14 +1306,23 @@
 ExportLensOutputTypeDef = TypedDict(
     "ExportLensOutputTypeDef",
     {
         "LensJSON": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+GetGlobalSettingsOutputTypeDef = TypedDict(
+    "GetGlobalSettingsOutputTypeDef",
+    {
+        "OrganizationSharingStatus": OrganizationSharingStatusType,
+        "DiscoveryIntegrationStatus": DiscoveryIntegrationStatusType,
+        "JiraConfiguration": AccountJiraConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 ImportLensOutputTypeDef = TypedDict(
     "ImportLensOutputTypeDef",
     {
         "LensArn": str,
         "Status": ImportLensStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1312,14 +1386,15 @@
         "Industry": NotRequired[str],
         "Notes": NotRequired[str],
         "Tags": NotRequired[Mapping[str, str]],
         "DiscoveryConfig": NotRequired[WorkloadDiscoveryConfigTypeDef],
         "Applications": NotRequired[Sequence[str]],
         "ProfileArns": NotRequired[Sequence[str]],
         "ReviewTemplateArns": NotRequired[Sequence[str]],
+        "JiraConfiguration": NotRequired[WorkloadJiraConfigurationInputTypeDef],
     },
 )
 UpdateWorkloadInputRequestTypeDef = TypedDict(
     "UpdateWorkloadInputRequestTypeDef",
     {
         "WorkloadId": str,
         "WorkloadName": NotRequired[str],
@@ -1334,14 +1409,15 @@
         "IsReviewOwnerUpdateAcknowledged": NotRequired[bool],
         "IndustryType": NotRequired[str],
         "Industry": NotRequired[str],
         "Notes": NotRequired[str],
         "ImprovementStatus": NotRequired[WorkloadImprovementStatusType],
         "DiscoveryConfig": NotRequired[WorkloadDiscoveryConfigTypeDef],
         "Applications": NotRequired[Sequence[str]],
+        "JiraConfiguration": NotRequired[WorkloadJiraConfigurationInputTypeDef],
     },
 )
 GetLensOutputTypeDef = TypedDict(
     "GetLensOutputTypeDef",
     {
         "Lens": LensTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1366,14 +1442,20 @@
 UpdateReviewTemplateOutputTypeDef = TypedDict(
     "UpdateReviewTemplateOutputTypeDef",
     {
         "ReviewTemplate": ReviewTemplateTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+JiraSelectedQuestionConfigurationTypeDef = TypedDict(
+    "JiraSelectedQuestionConfigurationTypeDef",
+    {
+        "SelectedPillars": NotRequired[List[SelectedPillarTypeDef]],
+    },
+)
 LensReviewSummaryTypeDef = TypedDict(
     "LensReviewSummaryTypeDef",
     {
         "LensAlias": NotRequired[str],
         "LensArn": NotRequired[str],
         "LensVersion": NotRequired[str],
         "LensName": NotRequired[str],
@@ -1395,63 +1477,14 @@
         "Lenses": NotRequired[List[str]],
         "RiskCounts": NotRequired[Dict[RiskType, int]],
         "ImprovementStatus": NotRequired[WorkloadImprovementStatusType],
         "Profiles": NotRequired[List[WorkloadProfileTypeDef]],
         "PrioritizedRiskCounts": NotRequired[Dict[RiskType, int]],
     },
 )
-WorkloadTypeDef = TypedDict(
-    "WorkloadTypeDef",
-    {
-        "WorkloadId": NotRequired[str],
-        "WorkloadArn": NotRequired[str],
-        "WorkloadName": NotRequired[str],
-        "Description": NotRequired[str],
-        "Environment": NotRequired[WorkloadEnvironmentType],
-        "UpdatedAt": NotRequired[datetime],
-        "AccountIds": NotRequired[List[str]],
-        "AwsRegions": NotRequired[List[str]],
-        "NonAwsRegions": NotRequired[List[str]],
-        "ArchitecturalDesign": NotRequired[str],
-        "ReviewOwner": NotRequired[str],
-        "ReviewRestrictionDate": NotRequired[datetime],
-        "IsReviewOwnerUpdateAcknowledged": NotRequired[bool],
-        "IndustryType": NotRequired[str],
-        "Industry": NotRequired[str],
-        "Notes": NotRequired[str],
-        "ImprovementStatus": NotRequired[WorkloadImprovementStatusType],
-        "RiskCounts": NotRequired[Dict[RiskType, int]],
-        "PillarPriorities": NotRequired[List[str]],
-        "Lenses": NotRequired[List[str]],
-        "Owner": NotRequired[str],
-        "ShareInvitationId": NotRequired[str],
-        "Tags": NotRequired[Dict[str, str]],
-        "DiscoveryConfig": NotRequired[WorkloadDiscoveryConfigTypeDef],
-        "Applications": NotRequired[List[str]],
-        "Profiles": NotRequired[List[WorkloadProfileTypeDef]],
-        "PrioritizedRiskCounts": NotRequired[Dict[RiskType, int]],
-    },
-)
-LensReviewTypeDef = TypedDict(
-    "LensReviewTypeDef",
-    {
-        "LensAlias": NotRequired[str],
-        "LensArn": NotRequired[str],
-        "LensVersion": NotRequired[str],
-        "LensName": NotRequired[str],
-        "LensStatus": NotRequired[LensStatusType],
-        "PillarReviewSummaries": NotRequired[List[PillarReviewSummaryTypeDef]],
-        "UpdatedAt": NotRequired[datetime],
-        "Notes": NotRequired[str],
-        "RiskCounts": NotRequired[Dict[RiskType, int]],
-        "NextToken": NotRequired[str],
-        "Profiles": NotRequired[List[WorkloadProfileTypeDef]],
-        "PrioritizedRiskCounts": NotRequired[Dict[RiskType, int]],
-    },
-)
 ListLensSharesOutputTypeDef = TypedDict(
     "ListLensSharesOutputTypeDef",
     {
         "LensShareSummaries": List[LensShareSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1587,14 +1620,47 @@
     "UpdateWorkloadShareOutputTypeDef",
     {
         "WorkloadId": str,
         "WorkloadShare": WorkloadShareTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+WorkloadTypeDef = TypedDict(
+    "WorkloadTypeDef",
+    {
+        "WorkloadId": NotRequired[str],
+        "WorkloadArn": NotRequired[str],
+        "WorkloadName": NotRequired[str],
+        "Description": NotRequired[str],
+        "Environment": NotRequired[WorkloadEnvironmentType],
+        "UpdatedAt": NotRequired[datetime],
+        "AccountIds": NotRequired[List[str]],
+        "AwsRegions": NotRequired[List[str]],
+        "NonAwsRegions": NotRequired[List[str]],
+        "ArchitecturalDesign": NotRequired[str],
+        "ReviewOwner": NotRequired[str],
+        "ReviewRestrictionDate": NotRequired[datetime],
+        "IsReviewOwnerUpdateAcknowledged": NotRequired[bool],
+        "IndustryType": NotRequired[str],
+        "Industry": NotRequired[str],
+        "Notes": NotRequired[str],
+        "ImprovementStatus": NotRequired[WorkloadImprovementStatusType],
+        "RiskCounts": NotRequired[Dict[RiskType, int]],
+        "PillarPriorities": NotRequired[List[str]],
+        "Lenses": NotRequired[List[str]],
+        "Owner": NotRequired[str],
+        "ShareInvitationId": NotRequired[str],
+        "Tags": NotRequired[Dict[str, str]],
+        "DiscoveryConfig": NotRequired[WorkloadDiscoveryConfigTypeDef],
+        "Applications": NotRequired[List[str]],
+        "Profiles": NotRequired[List[WorkloadProfileTypeDef]],
+        "PrioritizedRiskCounts": NotRequired[Dict[RiskType, int]],
+        "JiraConfiguration": NotRequired[WorkloadJiraConfigurationOutputTypeDef],
+    },
+)
 ChoiceTypeDef = TypedDict(
     "ChoiceTypeDef",
     {
         "ChoiceId": NotRequired[str],
         "Title": NotRequired[str],
         "Description": NotRequired[str],
         "HelpfulResource": NotRequired[ChoiceContentTypeDef],
@@ -1618,14 +1684,42 @@
         "LensAlias": str,
         "LensArn": str,
         "ImprovementSummaries": List[ImprovementSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+LensReviewTypeDef = TypedDict(
+    "LensReviewTypeDef",
+    {
+        "LensAlias": NotRequired[str],
+        "LensArn": NotRequired[str],
+        "LensVersion": NotRequired[str],
+        "LensName": NotRequired[str],
+        "LensStatus": NotRequired[LensStatusType],
+        "PillarReviewSummaries": NotRequired[List[PillarReviewSummaryTypeDef]],
+        "JiraConfiguration": NotRequired[JiraSelectedQuestionConfigurationTypeDef],
+        "UpdatedAt": NotRequired[datetime],
+        "Notes": NotRequired[str],
+        "RiskCounts": NotRequired[Dict[RiskType, int]],
+        "NextToken": NotRequired[str],
+        "Profiles": NotRequired[List[WorkloadProfileTypeDef]],
+        "PrioritizedRiskCounts": NotRequired[Dict[RiskType, int]],
+    },
+)
+UpdateLensReviewInputRequestTypeDef = TypedDict(
+    "UpdateLensReviewInputRequestTypeDef",
+    {
+        "WorkloadId": str,
+        "LensAlias": str,
+        "LensNotes": NotRequired[str],
+        "PillarNotes": NotRequired[Mapping[str, str]],
+        "JiraConfiguration": NotRequired[JiraSelectedQuestionConfigurationTypeDef],
+    },
+)
 ListLensReviewsOutputTypeDef = TypedDict(
     "ListLensReviewsOutputTypeDef",
     {
         "WorkloadId": str,
         "MilestoneNumber": int,
         "LensReviewSummaries": List[LensReviewSummaryTypeDef],
         "NextToken": str,
@@ -1645,54 +1739,14 @@
     {
         "MilestoneNumber": NotRequired[int],
         "MilestoneName": NotRequired[str],
         "RecordedAt": NotRequired[datetime],
         "WorkloadSummary": NotRequired[WorkloadSummaryTypeDef],
     },
 )
-GetWorkloadOutputTypeDef = TypedDict(
-    "GetWorkloadOutputTypeDef",
-    {
-        "Workload": WorkloadTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-MilestoneTypeDef = TypedDict(
-    "MilestoneTypeDef",
-    {
-        "MilestoneNumber": NotRequired[int],
-        "MilestoneName": NotRequired[str],
-        "RecordedAt": NotRequired[datetime],
-        "Workload": NotRequired[WorkloadTypeDef],
-    },
-)
-UpdateWorkloadOutputTypeDef = TypedDict(
-    "UpdateWorkloadOutputTypeDef",
-    {
-        "Workload": WorkloadTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-GetLensReviewOutputTypeDef = TypedDict(
-    "GetLensReviewOutputTypeDef",
-    {
-        "WorkloadId": str,
-        "MilestoneNumber": int,
-        "LensReview": LensReviewTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-UpdateLensReviewOutputTypeDef = TypedDict(
-    "UpdateLensReviewOutputTypeDef",
-    {
-        "WorkloadId": str,
-        "LensReview": LensReviewTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 ListNotificationsOutputTypeDef = TypedDict(
     "ListNotificationsOutputTypeDef",
     {
         "NotificationSummaries": List[NotificationSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1739,27 +1793,51 @@
     "UpdateReviewTemplateLensReviewOutputTypeDef",
     {
         "TemplateArn": str,
         "LensReview": ReviewTemplateLensReviewTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+GetWorkloadOutputTypeDef = TypedDict(
+    "GetWorkloadOutputTypeDef",
+    {
+        "Workload": WorkloadTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+MilestoneTypeDef = TypedDict(
+    "MilestoneTypeDef",
+    {
+        "MilestoneNumber": NotRequired[int],
+        "MilestoneName": NotRequired[str],
+        "RecordedAt": NotRequired[datetime],
+        "Workload": NotRequired[WorkloadTypeDef],
+    },
+)
+UpdateWorkloadOutputTypeDef = TypedDict(
+    "UpdateWorkloadOutputTypeDef",
+    {
+        "Workload": WorkloadTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 AnswerSummaryTypeDef = TypedDict(
     "AnswerSummaryTypeDef",
     {
         "QuestionId": NotRequired[str],
         "PillarId": NotRequired[str],
         "QuestionTitle": NotRequired[str],
         "Choices": NotRequired[List[ChoiceTypeDef]],
         "SelectedChoices": NotRequired[List[str]],
         "ChoiceAnswerSummaries": NotRequired[List[ChoiceAnswerSummaryTypeDef]],
         "IsApplicable": NotRequired[bool],
         "Risk": NotRequired[RiskType],
         "Reason": NotRequired[AnswerReasonType],
         "QuestionType": NotRequired[QuestionTypeType],
+        "JiraConfiguration": NotRequired[JiraConfigurationTypeDef],
     },
 )
 AnswerTypeDef = TypedDict(
     "AnswerTypeDef",
     {
         "QuestionId": NotRequired[str],
         "PillarId": NotRequired[str],
@@ -1771,14 +1849,15 @@
         "Choices": NotRequired[List[ChoiceTypeDef]],
         "SelectedChoices": NotRequired[List[str]],
         "ChoiceAnswers": NotRequired[List[ChoiceAnswerTypeDef]],
         "IsApplicable": NotRequired[bool],
         "Risk": NotRequired[RiskType],
         "Notes": NotRequired[str],
         "Reason": NotRequired[AnswerReasonType],
+        "JiraConfiguration": NotRequired[JiraConfigurationTypeDef],
     },
 )
 ReviewTemplateAnswerSummaryTypeDef = TypedDict(
     "ReviewTemplateAnswerSummaryTypeDef",
     {
         "QuestionId": NotRequired[str],
         "PillarId": NotRequired[str],
@@ -1815,28 +1894,37 @@
     "LensMetricTypeDef",
     {
         "LensArn": NotRequired[str],
         "Pillars": NotRequired[List[PillarMetricTypeDef]],
         "RiskCounts": NotRequired[Dict[RiskType, int]],
     },
 )
-ListMilestonesOutputTypeDef = TypedDict(
-    "ListMilestonesOutputTypeDef",
+GetLensReviewOutputTypeDef = TypedDict(
+    "GetLensReviewOutputTypeDef",
     {
         "WorkloadId": str,
-        "MilestoneSummaries": List[MilestoneSummaryTypeDef],
-        "NextToken": str,
+        "MilestoneNumber": int,
+        "LensReview": LensReviewTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-GetMilestoneOutputTypeDef = TypedDict(
-    "GetMilestoneOutputTypeDef",
+UpdateLensReviewOutputTypeDef = TypedDict(
+    "UpdateLensReviewOutputTypeDef",
     {
         "WorkloadId": str,
-        "Milestone": MilestoneTypeDef,
+        "LensReview": LensReviewTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+ListMilestonesOutputTypeDef = TypedDict(
+    "ListMilestonesOutputTypeDef",
+    {
+        "WorkloadId": str,
+        "MilestoneSummaries": List[MilestoneSummaryTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 GetLensVersionDifferenceOutputTypeDef = TypedDict(
     "GetLensVersionDifferenceOutputTypeDef",
     {
         "LensAlias": str,
@@ -1865,14 +1953,22 @@
 GetProfileTemplateOutputTypeDef = TypedDict(
     "GetProfileTemplateOutputTypeDef",
     {
         "ProfileTemplate": ProfileTemplateTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+GetMilestoneOutputTypeDef = TypedDict(
+    "GetMilestoneOutputTypeDef",
+    {
+        "WorkloadId": str,
+        "Milestone": MilestoneTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 ListAnswersOutputTypeDef = TypedDict(
     "ListAnswersOutputTypeDef",
     {
         "WorkloadId": str,
         "MilestoneNumber": int,
         "LensAlias": str,
         "LensArn": str,
```

### Comparing `mypy-boto3-wellarchitected-1.34.0/mypy_boto3_wellarchitected.egg-info/PKG-INFO` & `mypy_boto3_wellarchitected-1.34.85/mypy_boto3_wellarchitected.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-wellarchitected
-Version: 1.34.0
-Summary: Type annotations for boto3.WellArchitected 1.34.0 service generated with mypy-boto3-builder 7.21.0
+Version: 1.34.85
+Summary: Type annotations for boto3.WellArchitected 1.34.85 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/
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
 
 <a id="mypy-boto3-wellarchitected"></a>
 
 # mypy-boto3-wellarchitected
 
 [![PyPI - mypy-boto3-wellarchitected](https://img.shields.io/pypi/v/mypy-boto3-wellarchitected.svg?color=blue)](https://pypi.org/project/mypy-boto3-wellarchitected)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-wellarchitected.svg?color=blue)](https://pypi.org/project/mypy-boto3-wellarchitected)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-wellarchitected)](https://pepy.tech/project/mypy-boto3-wellarchitected)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WellArchitected 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected)
+[boto3.WellArchitected 1.34.85](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected)
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
 [mypy-boto3-wellarchitected docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/).
 
 See how it helps to find and fix potential bugs:
 
@@ -280,35 +280,35 @@
 `mypy_boto3_wellarchitected.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
 Full list of `WellArchitected` Literals can be found in
 [docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/literals/).
 
 ```python
-from mypy_boto3_wellarchitected.literals import AdditionalResourceTypeType
+from mypy_boto3_wellarchitected.literals import AccountJiraIssueManagementStatusType
 
 
-def check_value(value: AdditionalResourceTypeType) -> bool: ...
+def check_value(value: AccountJiraIssueManagementStatusType) -> bool: ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `mypy_boto3_wellarchitected.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
 Full list of `WellArchitected` TypeDefs can be found in
 [docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/type_defs/).
 
 ```python
-from mypy_boto3_wellarchitected.type_defs import ChoiceContentTypeDef
+from mypy_boto3_wellarchitected.type_defs import AccountJiraConfigurationInputTypeDef
 
 
-def get_value() -> ChoiceContentTypeDef:
+def get_value() -> AccountJiraConfigurationInputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-wellarchitected-1.34.0/mypy_boto3_wellarchitected.egg-info/SOURCES.txt` & `mypy_boto3_wellarchitected-1.34.85/mypy_boto3_wellarchitected.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wellarchitected-1.34.0/setup.py` & `mypy_boto3_wellarchitected-1.34.85/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,48 +7,44 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-wellarchitected",
-    version="1.34.0",
+    version="1.34.85",
     packages=["mypy_boto3_wellarchitected"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description=(
-        "Type annotations for boto3.WellArchitected 1.34.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
-    ),
+    description="Type annotations for boto3.WellArchitected 1.34.85 service generated with mypy-boto3-builder 7.23.2",
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
     keywords="boto3 wellarchitected type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_wellarchitected": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

