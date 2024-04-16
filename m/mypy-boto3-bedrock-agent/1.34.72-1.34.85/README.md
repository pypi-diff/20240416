# Comparing `tmp/mypy-boto3-bedrock-agent-1.34.72.tar.gz` & `tmp/mypy_boto3_bedrock_agent-1.34.85.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-bedrock-agent-1.34.72.tar", last modified: Wed Mar 27 19:47:05 2024, max compression
+gzip compressed data, was "mypy_boto3_bedrock_agent-1.34.85.tar", last modified: Tue Apr 16 19:33:14 2024, max compression
```

## Comparing `mypy-boto3-bedrock-agent-1.34.72.tar` & `mypy_boto3_bedrock_agent-1.34.85.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:47:05.378890 mypy-boto3-bedrock-agent-1.34.72/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-27 19:46:46.000000 mypy-boto3-bedrock-agent-1.34.72/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14085 2024-03-27 19:47:05.378890 mypy-boto3-bedrock-agent-1.34.72/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12503 2024-03-27 19:46:46.000000 mypy-boto3-bedrock-agent-1.34.72/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:47:05.374890 mypy-boto3-bedrock-agent-1.34.72/mypy_boto3_bedrock_agent/
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-03-27 19:46:46.000000 mypy-boto3-bedrock-agent-1.34.72/mypy_boto3_bedrock_agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-03-27 19:46:46.000000 mypy-boto3-bedrock-agent-1.34.72/mypy_boto3_bedrock_agent/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-03-27 19:46:46.000000 mypy-boto3-bedrock-agent-1.34.72/mypy_boto3_bedrock_agent/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34116 2024-03-27 19:46:47.000000 mypy-boto3-bedrock-agent-1.34.72/mypy_boto3_bedrock_agent/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    34113 2024-03-27 19:46:47.000000 mypy-boto3-bedrock-agent-1.34.72/mypy_boto3_bedrock_agent/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11197 2024-03-27 19:46:47.000000 mypy-boto3-bedrock-agent-1.34.72/mypy_boto3_bedrock_agent/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    11197 2024-03-27 19:46:47.000000 mypy-boto3-bedrock-agent-1.34.72/mypy_boto3_bedrock_agent/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9997 2024-03-27 19:46:47.000000 mypy-boto3-bedrock-agent-1.34.72/mypy_boto3_bedrock_agent/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     9988 2024-03-27 19:46:47.000000 mypy-boto3-bedrock-agent-1.34.72/mypy_boto3_bedrock_agent/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 19:46:46.000000 mypy-boto3-bedrock-agent-1.34.72/mypy_boto3_bedrock_agent/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    41147 2024-03-27 19:46:48.000000 mypy-boto3-bedrock-agent-1.34.72/mypy_boto3_bedrock_agent/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    41147 2024-03-27 19:46:47.000000 mypy-boto3-bedrock-agent-1.34.72/mypy_boto3_bedrock_agent/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-27 19:46:46.000000 mypy-boto3-bedrock-agent-1.34.72/mypy_boto3_bedrock_agent/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:47:05.378890 mypy-boto3-bedrock-agent-1.34.72/mypy_boto3_bedrock_agent.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14085 2024-03-27 19:47:05.000000 mypy-boto3-bedrock-agent-1.34.72/mypy_boto3_bedrock_agent.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-03-27 19:47:05.000000 mypy-boto3-bedrock-agent-1.34.72/mypy_boto3_bedrock_agent.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 19:47:05.000000 mypy-boto3-bedrock-agent-1.34.72/mypy_boto3_bedrock_agent.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 19:47:05.000000 mypy-boto3-bedrock-agent-1.34.72/mypy_boto3_bedrock_agent.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-27 19:47:05.000000 mypy-boto3-bedrock-agent-1.34.72/mypy_boto3_bedrock_agent.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-27 19:47:05.000000 mypy-boto3-bedrock-agent-1.34.72/mypy_boto3_bedrock_agent.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 19:47:05.378890 mypy-boto3-bedrock-agent-1.34.72/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-03-27 19:46:46.000000 mypy-boto3-bedrock-agent-1.34.72/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:33:14.412300 mypy_boto3_bedrock_agent-1.34.85/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-16 19:32:47.000000 mypy_boto3_bedrock_agent-1.34.85/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14085 2024-04-16 19:33:14.408300 mypy_boto3_bedrock_agent-1.34.85/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12503 2024-04-16 19:32:47.000000 mypy_boto3_bedrock_agent-1.34.85/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:33:14.408300 mypy_boto3_bedrock_agent-1.34.85/mypy_boto3_bedrock_agent/
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-16 19:32:47.000000 mypy_boto3_bedrock_agent-1.34.85/mypy_boto3_bedrock_agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-16 19:32:47.000000 mypy_boto3_bedrock_agent-1.34.85/mypy_boto3_bedrock_agent/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-16 19:32:47.000000 mypy_boto3_bedrock_agent-1.34.85/mypy_boto3_bedrock_agent/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34122 2024-04-16 19:32:48.000000 mypy_boto3_bedrock_agent-1.34.85/mypy_boto3_bedrock_agent/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34119 2024-04-16 19:32:47.000000 mypy_boto3_bedrock_agent-1.34.85/mypy_boto3_bedrock_agent/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11258 2024-04-16 19:32:48.000000 mypy_boto3_bedrock_agent-1.34.85/mypy_boto3_bedrock_agent/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11258 2024-04-16 19:32:48.000000 mypy_boto3_bedrock_agent-1.34.85/mypy_boto3_bedrock_agent/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9997 2024-04-16 19:32:48.000000 mypy_boto3_bedrock_agent-1.34.85/mypy_boto3_bedrock_agent/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9988 2024-04-16 19:32:48.000000 mypy_boto3_bedrock_agent-1.34.85/mypy_boto3_bedrock_agent/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 19:32:47.000000 mypy_boto3_bedrock_agent-1.34.85/mypy_boto3_bedrock_agent/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    41160 2024-04-16 19:32:48.000000 mypy_boto3_bedrock_agent-1.34.85/mypy_boto3_bedrock_agent/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41160 2024-04-16 19:32:48.000000 mypy_boto3_bedrock_agent-1.34.85/mypy_boto3_bedrock_agent/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-16 19:32:47.000000 mypy_boto3_bedrock_agent-1.34.85/mypy_boto3_bedrock_agent/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:33:14.408300 mypy_boto3_bedrock_agent-1.34.85/mypy_boto3_bedrock_agent.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14085 2024-04-16 19:33:14.000000 mypy_boto3_bedrock_agent-1.34.85/mypy_boto3_bedrock_agent.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-16 19:33:14.000000 mypy_boto3_bedrock_agent-1.34.85/mypy_boto3_bedrock_agent.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 19:33:14.000000 mypy_boto3_bedrock_agent-1.34.85/mypy_boto3_bedrock_agent.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 19:33:14.000000 mypy_boto3_bedrock_agent-1.34.85/mypy_boto3_bedrock_agent.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-16 19:33:14.000000 mypy_boto3_bedrock_agent-1.34.85/mypy_boto3_bedrock_agent.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-16 19:33:14.000000 mypy_boto3_bedrock_agent-1.34.85/mypy_boto3_bedrock_agent.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 19:33:14.412300 mypy_boto3_bedrock_agent-1.34.85/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-16 19:32:47.000000 mypy_boto3_bedrock_agent-1.34.85/setup.py
```

### Comparing `mypy-boto3-bedrock-agent-1.34.72/LICENSE` & `mypy_boto3_bedrock_agent-1.34.85/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-bedrock-agent-1.34.72/PKG-INFO` & `mypy_boto3_bedrock_agent-1.34.85/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-bedrock-agent
-Version: 1.34.72
-Summary: Type annotations for boto3.AgentsforBedrock 1.34.72 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.85
+Summary: Type annotations for boto3.AgentsforBedrock 1.34.85 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_agent/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-bedrock-agent.svg?color=blue)](https://pypi.org/project/mypy-boto3-bedrock-agent)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_agent/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-bedrock-agent)](https://pepy.tech/project/mypy-boto3-bedrock-agent)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AgentsforBedrock 1.34.72](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock)
+[boto3.AgentsforBedrock 1.34.85](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-bedrock-agent-1.34.72/README.md` & `mypy_boto3_bedrock_agent-1.34.85/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-bedrock-agent.svg?color=blue)](https://pypi.org/project/mypy-boto3-bedrock-agent)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_agent/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-bedrock-agent)](https://pepy.tech/project/mypy-boto3-bedrock-agent)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AgentsforBedrock 1.34.72](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock)
+[boto3.AgentsforBedrock 1.34.85](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-bedrock-agent-1.34.72/mypy_boto3_bedrock_agent/__init__.py` & `mypy_boto3_bedrock_agent-1.34.85/mypy_boto3_bedrock_agent/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-bedrock-agent-1.34.72/mypy_boto3_bedrock_agent/__init__.pyi` & `mypy_boto3_bedrock_agent-1.34.85/mypy_boto3_bedrock_agent/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-bedrock-agent-1.34.72/mypy_boto3_bedrock_agent/__main__.py` & `mypy_boto3_bedrock_agent-1.34.85/mypy_boto3_bedrock_agent/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.AgentsforBedrock 1.34.72\n"
-        "Version:         1.34.72\n"
+        "Type annotations for boto3.AgentsforBedrock 1.34.85\n"
+        "Version:         1.34.85\n"
         "Builder version: 7.23.2\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_agent//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.72")
+    print("1.34.85")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-bedrock-agent-1.34.72/mypy_boto3_bedrock_agent/client.py` & `mypy_boto3_bedrock_agent-1.34.85/mypy_boto3_bedrock_agent/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -156,15 +156,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_agent/client/#close)
         """
 
     def create_agent(
         self,
         *,
         agentName: str,
-        agentResourceRoleArn: str,
+        agentResourceRoleArn: str = ...,
         clientToken: str = ...,
         customerEncryptionKeyArn: str = ...,
         description: str = ...,
         foundationModel: str = ...,
         idleSessionTTLInSeconds: int = ...,
         instruction: str = ...,
         promptOverrideConfiguration: PromptOverrideConfigurationTypeDef = ...,
```

### Comparing `mypy-boto3-bedrock-agent-1.34.72/mypy_boto3_bedrock_agent/client.pyi` & `mypy_boto3_bedrock_agent-1.34.85/mypy_boto3_bedrock_agent/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -153,15 +153,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_agent/client/#close)
         """
 
     def create_agent(
         self,
         *,
         agentName: str,
-        agentResourceRoleArn: str,
+        agentResourceRoleArn: str = ...,
         clientToken: str = ...,
         customerEncryptionKeyArn: str = ...,
         description: str = ...,
         foundationModel: str = ...,
         idleSessionTTLInSeconds: int = ...,
         instruction: str = ...,
         promptOverrideConfiguration: PromptOverrideConfigurationTypeDef = ...,
```

### Comparing `mypy-boto3-bedrock-agent-1.34.72/mypy_boto3_bedrock_agent/literals.py` & `mypy_boto3_bedrock_agent-1.34.85/mypy_boto3_bedrock_agent/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,14 +161,15 @@
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
@@ -181,24 +182,26 @@
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

### Comparing `mypy-boto3-bedrock-agent-1.34.72/mypy_boto3_bedrock_agent/literals.pyi` & `mypy_boto3_bedrock_agent-1.34.85/mypy_boto3_bedrock_agent/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -161,14 +161,15 @@
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
@@ -181,24 +182,26 @@
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

### Comparing `mypy-boto3-bedrock-agent-1.34.72/mypy_boto3_bedrock_agent/paginator.py` & `mypy_boto3_bedrock_agent-1.34.85/mypy_boto3_bedrock_agent/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-bedrock-agent-1.34.72/mypy_boto3_bedrock_agent/paginator.pyi` & `mypy_boto3_bedrock_agent-1.34.85/mypy_boto3_bedrock_agent/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-bedrock-agent-1.34.72/mypy_boto3_bedrock_agent/type_defs.py` & `mypy_boto3_bedrock_agent-1.34.85/mypy_boto3_bedrock_agent/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1190,15 +1190,15 @@
         "recommendedActions": NotRequired[List[str]],
     },
 )
 CreateAgentRequestRequestTypeDef = TypedDict(
     "CreateAgentRequestRequestTypeDef",
     {
         "agentName": str,
-        "agentResourceRoleArn": str,
+        "agentResourceRoleArn": NotRequired[str],
         "clientToken": NotRequired[str],
         "customerEncryptionKeyArn": NotRequired[str],
         "description": NotRequired[str],
         "foundationModel": NotRequired[str],
         "idleSessionTTLInSeconds": NotRequired[int],
         "instruction": NotRequired[str],
         "promptOverrideConfiguration": NotRequired[PromptOverrideConfigurationTypeDef],
```

### Comparing `mypy-boto3-bedrock-agent-1.34.72/mypy_boto3_bedrock_agent/type_defs.pyi` & `mypy_boto3_bedrock_agent-1.34.85/mypy_boto3_bedrock_agent/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1190,15 +1190,15 @@
         "recommendedActions": NotRequired[List[str]],
     },
 )
 CreateAgentRequestRequestTypeDef = TypedDict(
     "CreateAgentRequestRequestTypeDef",
     {
         "agentName": str,
-        "agentResourceRoleArn": str,
+        "agentResourceRoleArn": NotRequired[str],
         "clientToken": NotRequired[str],
         "customerEncryptionKeyArn": NotRequired[str],
         "description": NotRequired[str],
         "foundationModel": NotRequired[str],
         "idleSessionTTLInSeconds": NotRequired[int],
         "instruction": NotRequired[str],
         "promptOverrideConfiguration": NotRequired[PromptOverrideConfigurationTypeDef],
```

### Comparing `mypy-boto3-bedrock-agent-1.34.72/mypy_boto3_bedrock_agent.egg-info/PKG-INFO` & `mypy_boto3_bedrock_agent-1.34.85/mypy_boto3_bedrock_agent.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-bedrock-agent
-Version: 1.34.72
-Summary: Type annotations for boto3.AgentsforBedrock 1.34.72 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.85
+Summary: Type annotations for boto3.AgentsforBedrock 1.34.85 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_agent/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-bedrock-agent.svg?color=blue)](https://pypi.org/project/mypy-boto3-bedrock-agent)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_agent/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-bedrock-agent)](https://pepy.tech/project/mypy-boto3-bedrock-agent)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AgentsforBedrock 1.34.72](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock)
+[boto3.AgentsforBedrock 1.34.85](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-bedrock-agent-1.34.72/mypy_boto3_bedrock_agent.egg-info/SOURCES.txt` & `mypy_boto3_bedrock_agent-1.34.85/mypy_boto3_bedrock_agent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-bedrock-agent-1.34.72/setup.py` & `mypy_boto3_bedrock_agent-1.34.85/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-bedrock-agent",
-    version="1.34.72",
+    version="1.34.85",
     packages=["mypy_boto3_bedrock_agent"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.AgentsforBedrock 1.34.72 service generated with mypy-boto3-builder 7.23.2",
+    description="Type annotations for boto3.AgentsforBedrock 1.34.85 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

