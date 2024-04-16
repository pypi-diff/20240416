# Comparing `tmp/nuvolos-cli-1.0.0.tar.gz` & `tmp/nuvolos_cli-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nuvolos-cli-1.0.0.tar", last modified: Fri Feb  9 16:26:47 2024, max compression
+gzip compressed data, was "nuvolos_cli-1.0.1.tar", last modified: Tue Apr 16 10:08:46 2024, max compression
```

## Comparing `nuvolos-cli-1.0.0.tar` & `nuvolos_cli-1.0.1.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:26:47.516229 nuvolos-cli-1.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:26:47.508229 nuvolos-cli-1.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:26:47.512229 nuvolos-cli-1.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-02-09 16:26:10.000000 nuvolos-cli-1.0.0/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-02-09 16:26:10.000000 nuvolos-cli-1.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-02-09 16:26:10.000000 nuvolos-cli-1.0.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-02-09 16:26:10.000000 nuvolos-cli-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-02-09 16:26:47.516229 nuvolos-cli-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-02-09 16:26:10.000000 nuvolos-cli-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-09 16:26:10.000000 nuvolos-cli-1.0.0/_config.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:26:47.512229 nuvolos-cli-1.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-02-09 16:26:10.000000 nuvolos-cli-1.0.0/docs/commands.md
--rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-02-09 16:26:10.000000 nuvolos-cli-1.0.0/docs/execute_commands.md
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-02-09 16:26:10.000000 nuvolos-cli-1.0.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-02-09 16:26:10.000000 nuvolos-cli-1.0.0/docs/install.md
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-02-09 16:26:10.000000 nuvolos-cli-1.0.0/docs/launch_scaled_apps.md
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-02-09 16:26:10.000000 nuvolos-cli-1.0.0/docs/list_running_applications.md
--rw-r--r--   0 runner    (1001) docker     (127)     5383 2024-02-09 16:26:10.000000 nuvolos-cli-1.0.0/docs/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-02-09 16:26:10.000000 nuvolos-cli-1.0.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-02-09 16:26:10.000000 nuvolos-cli-1.0.0/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:26:47.512229 nuvolos-cli-1.0.0/nuvolos_cli/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-02-09 16:26:10.000000 nuvolos-cli-1.0.0/nuvolos_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-02-09 16:26:10.000000 nuvolos-cli-1.0.0/nuvolos_cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10142 2024-02-09 16:26:10.000000 nuvolos-cli-1.0.0/nuvolos_cli/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4363 2024-02-09 16:26:10.000000 nuvolos-cli-1.0.0/nuvolos_cli/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    11712 2024-02-09 16:26:10.000000 nuvolos-cli-1.0.0/nuvolos_cli/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-02-09 16:26:10.000000 nuvolos-cli-1.0.0/nuvolos_cli/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     4495 2024-02-09 16:26:10.000000 nuvolos-cli-1.0.0/nuvolos_cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-02-09 16:26:10.000000 nuvolos-cli-1.0.0/nuvolos_cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:26:47.516229 nuvolos-cli-1.0.0/nuvolos_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-02-09 16:26:47.000000 nuvolos-cli-1.0.0/nuvolos_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-02-09 16:26:47.000000 nuvolos-cli-1.0.0/nuvolos_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-09 16:26:47.000000 nuvolos-cli-1.0.0/nuvolos_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-02-09 16:26:47.000000 nuvolos-cli-1.0.0/nuvolos_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-02-09 16:26:47.000000 nuvolos-cli-1.0.0/nuvolos_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-09 16:26:47.000000 nuvolos-cli-1.0.0/nuvolos_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-02-09 16:26:10.000000 nuvolos-cli-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-09 16:26:47.516229 nuvolos-cli-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:26:47.516229 nuvolos-cli-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-09 16:26:10.000000 nuvolos-cli-1.0.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:08:46.311403 nuvolos_cli-1.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:08:46.303403 nuvolos_cli-1.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:08:46.307403 nuvolos_cli-1.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-16 10:08:16.000000 nuvolos_cli-1.0.1/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-16 10:08:16.000000 nuvolos_cli-1.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-16 10:08:16.000000 nuvolos_cli-1.0.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-16 10:08:16.000000 nuvolos_cli-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-04-16 10:08:46.311403 nuvolos_cli-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-16 10:08:16.000000 nuvolos_cli-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-16 10:08:16.000000 nuvolos_cli-1.0.1/_config.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:08:46.307403 nuvolos_cli-1.0.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-16 10:08:16.000000 nuvolos_cli-1.0.1/docs/commands.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-04-16 10:08:16.000000 nuvolos_cli-1.0.1/docs/execute_commands.md
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-16 10:08:16.000000 nuvolos_cli-1.0.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-16 10:08:16.000000 nuvolos_cli-1.0.1/docs/install.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-16 10:08:16.000000 nuvolos_cli-1.0.1/docs/launch_scaled_apps.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-16 10:08:16.000000 nuvolos_cli-1.0.1/docs/list_running_applications.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5383 2024-04-16 10:08:16.000000 nuvolos_cli-1.0.1/docs/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-16 10:08:16.000000 nuvolos_cli-1.0.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-16 10:08:16.000000 nuvolos_cli-1.0.1/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:08:46.307403 nuvolos_cli-1.0.1/nuvolos_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-16 10:08:16.000000 nuvolos_cli-1.0.1/nuvolos_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-16 10:08:16.000000 nuvolos_cli-1.0.1/nuvolos_cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10821 2024-04-16 10:08:16.000000 nuvolos_cli-1.0.1/nuvolos_cli/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4357 2024-04-16 10:08:16.000000 nuvolos_cli-1.0.1/nuvolos_cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11712 2024-04-16 10:08:16.000000 nuvolos_cli-1.0.1/nuvolos_cli/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-16 10:08:16.000000 nuvolos_cli-1.0.1/nuvolos_cli/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4495 2024-04-16 10:08:16.000000 nuvolos_cli-1.0.1/nuvolos_cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-16 10:08:16.000000 nuvolos_cli-1.0.1/nuvolos_cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:08:46.311403 nuvolos_cli-1.0.1/nuvolos_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-04-16 10:08:46.000000 nuvolos_cli-1.0.1/nuvolos_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-16 10:08:46.000000 nuvolos_cli-1.0.1/nuvolos_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 10:08:46.000000 nuvolos_cli-1.0.1/nuvolos_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-16 10:08:46.000000 nuvolos_cli-1.0.1/nuvolos_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-16 10:08:46.000000 nuvolos_cli-1.0.1/nuvolos_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-16 10:08:46.000000 nuvolos_cli-1.0.1/nuvolos_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-16 10:08:16.000000 nuvolos_cli-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 10:08:46.311403 nuvolos_cli-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:08:46.311403 nuvolos_cli-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 10:08:16.000000 nuvolos_cli-1.0.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4942 2024-04-16 10:08:16.000000 nuvolos_cli-1.0.1/tests/test_interface.py
```

### Comparing `nuvolos-cli-1.0.0/.github/workflows/release.yaml` & `nuvolos_cli-1.0.1/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `nuvolos-cli-1.0.0/LICENSE` & `nuvolos_cli-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nuvolos-cli-1.0.0/PKG-INFO` & `nuvolos_cli-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nuvolos-cli
-Version: 1.0.0
+Version: 1.0.1
 Summary: Command-line interface for Nuvolos
 Author-email: Alphacruncher <support@nuvolos.cloud>
 Project-URL: Repository, https://github.com/nuvolos-cloud/nuvolos-cli
 Project-URL: Documentation, https://nuvolos-cli.readthedocs.io/en/latest
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
@@ -22,14 +22,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click>=8.1.7
 Requires-Dist: click-log>=0.4.0
 Requires-Dist: tabulate>=0.9.0
 Requires-Dist: pyyaml>=6.0.1
 Requires-Dist: nuvolos-client-api>=1.0.0
+Requires-Dist: humanize>=4.9.0
 
 <!-- [![PyPI version](https://img.shields.io/pypi/v/nuvolos-cli)](https://pypi.org/project/nuvolos-cli/)  -->
 [![Docs](https://readthedocs.org/projects/nuvolos-cli/badge/)](https://nuvolos-cli.readthedocs.io/en/latest/)
 <!-- [![Integration tests](https://github.com/nuvolos-cloud/nuvolos-cli/actions/workflows/integration-test.yaml/badge.svg)](https://github.com/nuvolos-cloud/nuvolos-cli/actions/workflows/integration-test.yaml) -->
 
 
 ```
```

### Comparing `nuvolos-cli-1.0.0/README.md` & `nuvolos_cli-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `nuvolos-cli-1.0.0/docs/execute_commands.md` & `nuvolos_cli-1.0.1/docs/execute_commands.md`

 * *Files identical despite different names*

### Comparing `nuvolos-cli-1.0.0/docs/index.md` & `nuvolos_cli-1.0.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `nuvolos-cli-1.0.0/docs/launch_scaled_apps.md` & `nuvolos_cli-1.0.1/docs/launch_scaled_apps.md`

 * *Files identical despite different names*

### Comparing `nuvolos-cli-1.0.0/docs/list_running_applications.md` & `nuvolos_cli-1.0.1/docs/list_running_applications.md`

 * *Files identical despite different names*

### Comparing `nuvolos-cli-1.0.0/docs/quickstart.md` & `nuvolos_cli-1.0.1/docs/quickstart.md`

 * *Files identical despite different names*

### Comparing `nuvolos-cli-1.0.0/nuvolos_cli/api_client.py` & `nuvolos_cli-1.0.1/nuvolos_cli/api_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 from click import ClickException
 from datetime import datetime
 from time import sleep
+
+from humanize import naturalsize
 from .logging import clog
 from .config import get_api_config, from_variable
 from .utils import exit_on_timeout
 
 import nuvolos_client_api
 from nuvolos_client_api.models import StartApp, ExecuteCommand
+from nuvolos_client_api.models.application import Application
+from pydantic import StrictStr
 
 
 def _find_variables(tb, variables):
     to_find = list(variables)
     found = {}
     for var in to_find:
         if var in tb.tb_frame.f_locals:
@@ -35,14 +39,30 @@
 
     @classmethod
     def from_api_exception(cls, e: nuvolos_client_api.ApiException, message=None):
         url = _find_variables(e.__traceback__, ["url"]).get("url", "")
         return cls(e.status, e.reason, e.body, e.headers, url)
 
 
+class HumanizedApplication(Application):
+    storage_used: StrictStr
+
+    @classmethod
+    def from_application(cls, app: Application):
+        return cls(
+            slug=app.slug,
+            name=app.name,
+            description=app.description,
+            storage_used=naturalsize(app.storage_used, binary=False),
+            shared=app.shared,
+            exportable=app.exportable,
+            status=app.status,
+        )
+
+
 def list_orgs():
     config = get_api_config()
     with nuvolos_client_api.ApiClient(config) as api_client:
         api_instance = nuvolos_client_api.OrganizationsV1Api(api_client)
         try:
             return api_instance.get_orgs()
         except nuvolos_client_api.ApiException as e:
@@ -99,20 +119,23 @@
     instance_slug: str,
     snapshot_slug: str,
 ):
     config = get_api_config()
     with nuvolos_client_api.ApiClient(config) as api_client:
         api_instance = nuvolos_client_api.AppsV1Api(api_client)
         try:
-            return api_instance.get_apps(
-                org_slug=org_slug,
-                space_slug=space_slug,
-                instance_slug=instance_slug,
-                snapshot_slug=snapshot_slug,
-            )
+            return [
+                HumanizedApplication.from_application(a)
+                for a in api_instance.get_apps(
+                    org_slug=org_slug,
+                    space_slug=space_slug,
+                    instance_slug=instance_slug,
+                    snapshot_slug=snapshot_slug,
+                )
+            ]
         except nuvolos_client_api.ApiException as e:
             raise NuvolosCliException.from_api_exception(
                 e,
                 f"Exception when listing Nuvolos apps for org [{org_slug}], space [{space_slug}] and instance [{instance_slug}]: {e}",
             )
```

### Comparing `nuvolos-cli-1.0.0/nuvolos_cli/config.py` & `nuvolos_cli-1.0.1/nuvolos_cli/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,21 +98,21 @@
 
 
 def check_api_key_configured():
     api_key = from_variable("NUVOLOS_API_KEY")
     if api_key is None:
         if not get_default_config_path().exists():
             raise ClickException(
-                "The Nuvolos API key must be set either as the NUVOLOS_API_KEY environment variable or with the `nuvolos configure --api-key` command."
+                "The Nuvolos API key must be set either as the NUVOLOS_API_KEY environment variable or with the `nuvolos config --api-key` command."
             )
         gdc = get_global_dict_config().read()
         api_key = gdc["api_key"]
         if api_key is None:
             raise ClickException(
-                "The Nuvolos API key must be set either as the NUVOLOS_API_KEY environment variable or with the `nuvolos configure --api-key` command."
+                "The Nuvolos API key must be set either as the NUVOLOS_API_KEY environment variable or with the `nuvolos config --api-key` command."
             )
     return api_key
 
 
 def info(nuvolos_ctx=None):
     clog.info(
         r"""
```

### Comparing `nuvolos-cli-1.0.0/nuvolos_cli/interface.py` & `nuvolos_cli-1.0.1/nuvolos_cli/interface.py`

 * *Files identical despite different names*

### Comparing `nuvolos-cli-1.0.0/nuvolos_cli/logging.py` & `nuvolos_cli-1.0.1/nuvolos_cli/logging.py`

 * *Files identical despite different names*

### Comparing `nuvolos-cli-1.0.0/nuvolos_cli/utils.py` & `nuvolos_cli-1.0.1/nuvolos_cli/utils.py`

 * *Files identical despite different names*

### Comparing `nuvolos-cli-1.0.0/nuvolos_cli.egg-info/PKG-INFO` & `nuvolos_cli-1.0.1/nuvolos_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nuvolos-cli
-Version: 1.0.0
+Version: 1.0.1
 Summary: Command-line interface for Nuvolos
 Author-email: Alphacruncher <support@nuvolos.cloud>
 Project-URL: Repository, https://github.com/nuvolos-cloud/nuvolos-cli
 Project-URL: Documentation, https://nuvolos-cli.readthedocs.io/en/latest
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
@@ -22,14 +22,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click>=8.1.7
 Requires-Dist: click-log>=0.4.0
 Requires-Dist: tabulate>=0.9.0
 Requires-Dist: pyyaml>=6.0.1
 Requires-Dist: nuvolos-client-api>=1.0.0
+Requires-Dist: humanize>=4.9.0
 
 <!-- [![PyPI version](https://img.shields.io/pypi/v/nuvolos-cli)](https://pypi.org/project/nuvolos-cli/)  -->
 [![Docs](https://readthedocs.org/projects/nuvolos-cli/badge/)](https://nuvolos-cli.readthedocs.io/en/latest/)
 <!-- [![Integration tests](https://github.com/nuvolos-cloud/nuvolos-cli/actions/workflows/integration-test.yaml/badge.svg)](https://github.com/nuvolos-cloud/nuvolos-cli/actions/workflows/integration-test.yaml) -->
 
 
 ```
```

### Comparing `nuvolos-cli-1.0.0/nuvolos_cli.egg-info/SOURCES.txt` & `nuvolos_cli-1.0.1/nuvolos_cli.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -24,8 +24,9 @@
 nuvolos_cli/version.py
 nuvolos_cli.egg-info/PKG-INFO
 nuvolos_cli.egg-info/SOURCES.txt
 nuvolos_cli.egg-info/dependency_links.txt
 nuvolos_cli.egg-info/entry_points.txt
 nuvolos_cli.egg-info/requires.txt
 nuvolos_cli.egg-info/top_level.txt
-tests/__init__.py
+tests/__init__.py
+tests/test_interface.py
```

### Comparing `nuvolos-cli-1.0.0/pyproject.toml` & `nuvolos_cli-1.0.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -28,15 +28,16 @@
     "Topic :: Scientific/Engineering :: Artificial Intelligence"
 ]
 dependencies = [
     "click>=8.1.7",
     "click-log>=0.4.0",
     "tabulate>=0.9.0",
     "pyyaml>=6.0.1",
-    "nuvolos-client-api>=1.0.0"
+    "nuvolos-client-api>=1.0.0",
+    "humanize>=4.9.0",
 ]
 
 [tool.setuptools_scm]
 
 
 [project.urls]
 Repository = "https://github.com/nuvolos-cloud/nuvolos-cli"
```

