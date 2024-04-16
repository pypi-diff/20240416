# Comparing `tmp/galileo_protect-0.5.0.tar.gz` & `tmp/galileo_protect-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galileo_protect-0.5.0.tar", max compression
+gzip compressed data, was "galileo_protect-0.5.1.tar", max compression
```

## Comparing `galileo_protect-0.5.0.tar` & `galileo_protect-0.5.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    10946 2024-04-10 23:28:22.445627 galileo_protect-0.5.0/LICENSE
--rw-r--r--   0        0        0      118 2024-04-10 23:28:22.445627 galileo_protect-0.5.0/README.md
--rw-r--r--   0        0        0     2529 2024-04-10 23:28:24.773630 galileo_protect-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      422 2024-04-10 23:28:24.773630 galileo_protect-0.5.0/src/galileo_protect/__init__.py
--rw-r--r--   0        0        0        0 2024-04-10 23:28:22.449627 galileo_protect-0.5.0/src/galileo_protect/constants/__init__.py
--rw-r--r--   0        0        0      324 2024-04-10 23:28:22.449627 galileo_protect-0.5.0/src/galileo_protect/constants/routes.py
--rw-r--r--   0        0        0        0 2024-04-10 23:28:22.449627 galileo_protect-0.5.0/src/galileo_protect/helpers/__init__.py
--rw-r--r--   0        0        0      530 2024-04-10 23:28:22.449627 galileo_protect-0.5.0/src/galileo_protect/helpers/config.py
--rw-r--r--   0        0        0     1402 2024-04-10 23:28:22.449627 galileo_protect-0.5.0/src/galileo_protect/invoke.py
--rw-r--r--   0        0        0      638 2024-04-10 23:28:22.449627 galileo_protect-0.5.0/src/galileo_protect/project.py
--rw-r--r--   0        0        0      665 2024-04-10 23:28:22.449627 galileo_protect-0.5.0/src/galileo_protect/schemas/__init__.py
--rw-r--r--   0        0        0      212 2024-04-10 23:28:22.449627 galileo_protect-0.5.0/src/galileo_protect/schemas/invoke.py
--rw-r--r--   0        0        0      308 2024-04-10 23:28:22.449627 galileo_protect-0.5.0/src/galileo_protect/schemas/rule.py
--rw-r--r--   0        0        0      124 2024-04-10 23:28:22.449627 galileo_protect-0.5.0/src/galileo_protect/schemas/stage.py
--rw-r--r--   0        0        0     3503 2024-04-10 23:28:22.449627 galileo_protect-0.5.0/src/galileo_protect/stage.py
--rw-r--r--   0        0        0      693 1970-01-01 00:00:00.000000 galileo_protect-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    10946 2024-04-16 14:57:26.216746 galileo_protect-0.5.1/LICENSE
+-rw-r--r--   0        0        0      118 2024-04-16 14:57:26.216746 galileo_protect-0.5.1/README.md
+-rw-r--r--   0        0        0     2529 2024-04-16 14:57:27.108759 galileo_protect-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0      422 2024-04-16 14:57:27.108759 galileo_protect-0.5.1/src/galileo_protect/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:57:26.220747 galileo_protect-0.5.1/src/galileo_protect/constants/__init__.py
+-rw-r--r--   0        0        0      324 2024-04-16 14:57:26.220747 galileo_protect-0.5.1/src/galileo_protect/constants/routes.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:57:26.220747 galileo_protect-0.5.1/src/galileo_protect/helpers/__init__.py
+-rw-r--r--   0        0        0      530 2024-04-16 14:57:26.220747 galileo_protect-0.5.1/src/galileo_protect/helpers/config.py
+-rw-r--r--   0        0        0     1403 2024-04-16 14:57:26.220747 galileo_protect-0.5.1/src/galileo_protect/invoke.py
+-rw-r--r--   0        0        0      638 2024-04-16 14:57:26.220747 galileo_protect-0.5.1/src/galileo_protect/project.py
+-rw-r--r--   0        0        0      665 2024-04-16 14:57:26.220747 galileo_protect-0.5.1/src/galileo_protect/schemas/__init__.py
+-rw-r--r--   0        0        0      212 2024-04-16 14:57:26.220747 galileo_protect-0.5.1/src/galileo_protect/schemas/invoke.py
+-rw-r--r--   0        0        0      308 2024-04-16 14:57:26.220747 galileo_protect-0.5.1/src/galileo_protect/schemas/rule.py
+-rw-r--r--   0        0        0      124 2024-04-16 14:57:26.220747 galileo_protect-0.5.1/src/galileo_protect/schemas/stage.py
+-rw-r--r--   0        0        0     3529 2024-04-16 14:57:26.220747 galileo_protect-0.5.1/src/galileo_protect/stage.py
+-rw-r--r--   0        0        0      693 1970-01-01 00:00:00.000000 galileo_protect-0.5.1/PKG-INFO
```

### Comparing `galileo_protect-0.5.0/LICENSE` & `galileo_protect-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `galileo_protect-0.5.0/pyproject.toml` & `galileo_protect-0.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "galileo-protect"
-version = "0.5.0"
+version = "0.5.1"
 description = "🛡️ Secure your Generative AI applications with Galileo Protect!"
 authors = ["Galileo Technologies Inc. <team@rungalileo.io>"]
 readme = "README.md"
 packages = [{include = "galileo_protect", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.8.1,<3.13"
```

### Comparing `galileo_protect-0.5.0/src/galileo_protect/helpers/config.py` & `galileo_protect-0.5.1/src/galileo_protect/helpers/config.py`

 * *Files identical despite different names*

### Comparing `galileo_protect-0.5.0/src/galileo_protect/invoke.py` & `galileo_protect-0.5.1/src/galileo_protect/invoke.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 def invoke(
     payload: Payload,
     prioritized_rulesets: Optional[Sequence[Ruleset]] = None,
     project_id: Optional[UUID4] = None,
     stage_name: Optional[str] = None,
     stage_id: Optional[UUID4] = None,
-    timeout: float = timedelta(minutes=5).total_seconds(),
+    timeout: float = timedelta(seconds=10).total_seconds(),
     metadata: Optional[Dict[str, str]] = None,
     headers: Optional[Dict[str, str]] = None,
     config: Optional[ProtectConfig] = None,
 ) -> Response:
     protect_config: ProtectConfig = config or ProtectConfig.get()
     response_json = protect_config.api_client.request(
         post,
```

### Comparing `galileo_protect-0.5.0/src/galileo_protect/project.py` & `galileo_protect-0.5.1/src/galileo_protect/project.py`

 * *Files identical despite different names*

### Comparing `galileo_protect-0.5.0/src/galileo_protect/schemas/__init__.py` & `galileo_protect-0.5.1/src/galileo_protect/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `galileo_protect-0.5.0/src/galileo_protect/stage.py` & `galileo_protect-0.5.1/src/galileo_protect/stage.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,37 +2,37 @@
 
 from galileo_core.utils.name import ts_name
 from pydantic import UUID4
 from requests import post, put
 
 from galileo_protect.constants.routes import Routes
 from galileo_protect.helpers.config import ProtectConfig
-from galileo_protect.schemas import Action, Stage
+from galileo_protect.schemas import Action, PassthroughAction, Stage
 from galileo_protect.schemas.stage import StageResponse
 
 
 def create_stage(
     project_id: Optional[UUID4] = None,
     name: Optional[str] = None,
     description: Optional[str] = None,
-    action: Optional[Action] = None,
-    action_elabed: bool = False,
+    action: Action = PassthroughAction(),
+    action_enabled: bool = False,
     config: Optional[ProtectConfig] = None,
 ) -> StageResponse:
     config = config or ProtectConfig.get()
     project_id = project_id or config.project_id
     if project_id is None:
         raise ValueError("Project ID must be provided to create a stage.")
     name = name or ts_name("stage")
     stage = StageResponse.model_validate(
         config.api_client.request(
             post,
             Routes.stages.format(project_id=project_id),
             json=Stage(
-                name=name, project_id=project_id, description=description, action=action, action_enabled=action_elabed
+                name=name, project_id=project_id, description=description, action=action, action_enabled=action_enabled
             ).model_dump(mode="json"),
         )
     )
     config.project_id = project_id
     config.stage_id = stage.id
     config.stage_name = stage.name
     config.write()
```

### Comparing `galileo_protect-0.5.0/PKG-INFO` & `galileo_protect-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galileo-protect
-Version: 0.5.0
+Version: 0.5.1
 Summary: 🛡️ Secure your Generative AI applications with Galileo Protect!
 Author: Galileo Technologies Inc.
 Author-email: team@rungalileo.io
 Requires-Python: >=3.8.1,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

