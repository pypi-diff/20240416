# Comparing `tmp/composio_core-0.2.0.tar.gz` & `tmp/composio_core-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_core-0.2.0.tar", last modified: Mon Apr 15 09:07:38 2024, max compression
+gzip compressed data, was "composio_core-0.2.1.tar", last modified: Mon Apr 15 17:20:29 2024, max compression
```

## Comparing `composio_core-0.2.0.tar` & `composio_core-0.2.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-15 09:07:38.726396 composio_core-0.2.0/
--rw-r--r--   0 karanvaidya   (501) staff       (20)       48 2024-04-15 07:39:40.000000 composio_core-0.2.0/MANIFEST.in
--rw-r--r--   0 karanvaidya   (501) staff       (20)      796 2024-04-15 09:07:38.726193 composio_core-0.2.0/PKG-INFO
--rw-r--r--   0 karanvaidya   (501) staff       (20)      102 2024-04-15 07:39:40.000000 composio_core-0.2.0/README.md
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-15 09:07:38.723155 composio_core-0.2.0/composio/
--rw-r--r--   0 karanvaidya   (501) staff       (20)      159 2024-04-15 07:39:40.000000 composio_core-0.2.0/composio/__init__.py
--rwxr-xr-x   0 karanvaidya   (501) staff       (20)    21879 2024-04-15 07:39:40.000000 composio_core-0.2.0/composio/composio_cli.py
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-15 09:07:38.725077 composio_core-0.2.0/composio/sdk/
--rw-r--r--   0 karanvaidya   (501) staff       (20)       85 2024-04-15 07:39:40.000000 composio_core-0.2.0/composio/sdk/__init__.py
--rw-r--r--   0 karanvaidya   (501) staff       (20)     7042 2024-04-15 07:39:40.000000 composio_core-0.2.0/composio/sdk/core.py
--rw-r--r--   0 karanvaidya   (501) staff       (20)    10226 2024-04-15 07:39:40.000000 composio_core-0.2.0/composio/sdk/enums.py
--rw-r--r--   0 karanvaidya   (501) staff       (20)    19363 2024-04-15 07:39:40.000000 composio_core-0.2.0/composio/sdk/sdk.py
--rw-r--r--   0 karanvaidya   (501) staff       (20)        0 2024-04-15 07:39:40.000000 composio_core-0.2.0/composio/sdk/shared.py
--rw-r--r--   0 karanvaidya   (501) staff       (20)     2300 2024-04-15 07:39:40.000000 composio_core-0.2.0/composio/sdk/storage.py
--rw-r--r--   0 karanvaidya   (501) staff       (20)     3328 2024-04-15 07:39:40.000000 composio_core-0.2.0/composio/sdk/utils.py
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-15 09:07:38.725966 composio_core-0.2.0/composio_core.egg-info/
--rw-r--r--   0 karanvaidya   (501) staff       (20)      796 2024-04-15 09:07:38.000000 composio_core-0.2.0/composio_core.egg-info/PKG-INFO
--rw-r--r--   0 karanvaidya   (501) staff       (20)      489 2024-04-15 09:07:38.000000 composio_core-0.2.0/composio_core.egg-info/SOURCES.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)        1 2024-04-15 09:07:38.000000 composio_core-0.2.0/composio_core.egg-info/dependency_links.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)       60 2024-04-15 09:07:38.000000 composio_core-0.2.0/composio_core.egg-info/entry_points.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)      103 2024-04-15 09:07:38.000000 composio_core-0.2.0/composio_core.egg-info/requires.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)        9 2024-04-15 09:07:38.000000 composio_core-0.2.0/composio_core.egg-info/top_level.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)      528 2024-04-15 07:39:40.000000 composio_core-0.2.0/pyproject.toml
--rw-r--r--   0 karanvaidya   (501) staff       (20)      130 2024-04-15 07:39:40.000000 composio_core-0.2.0/requirements.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)       38 2024-04-15 09:07:38.726438 composio_core-0.2.0/setup.cfg
--rw-r--r--   0 karanvaidya   (501) staff       (20)     1127 2024-04-15 09:07:06.000000 composio_core-0.2.0/setup.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-15 17:20:29.893396 composio_core-0.2.1/
+-rw-r--r--   0 utkarsh    (501) staff       (20)       48 2024-03-15 13:37:31.000000 composio_core-0.2.1/MANIFEST.in
+-rw-r--r--   0 utkarsh    (501) staff       (20)      796 2024-04-15 17:20:29.893137 composio_core-0.2.1/PKG-INFO
+-rw-r--r--   0 utkarsh    (501) staff       (20)      102 2024-03-16 10:06:01.000000 composio_core-0.2.1/README.md
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-15 17:20:29.889912 composio_core-0.2.1/composio/
+-rw-r--r--   0 utkarsh    (501) staff       (20)      159 2024-04-12 09:34:06.000000 composio_core-0.2.1/composio/__init__.py
+-rwxr-xr-x   0 utkarsh    (501) staff       (20)    22056 2024-04-15 14:10:00.000000 composio_core-0.2.1/composio/composio_cli.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-15 17:20:29.891831 composio_core-0.2.1/composio/sdk/
+-rw-r--r--   0 utkarsh    (501) staff       (20)       85 2024-03-27 14:52:24.000000 composio_core-0.2.1/composio/sdk/__init__.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     6837 2024-04-15 14:05:59.000000 composio_core-0.2.1/composio/sdk/core.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)    10226 2024-04-12 13:08:03.000000 composio_core-0.2.1/composio/sdk/enums.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)    19264 2024-04-15 14:02:12.000000 composio_core-0.2.1/composio/sdk/sdk.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)        0 2024-04-12 13:36:37.000000 composio_core-0.2.1/composio/sdk/shared.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     1358 2024-04-15 14:06:14.000000 composio_core-0.2.1/composio/sdk/storage.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     3328 2024-04-12 09:33:50.000000 composio_core-0.2.1/composio/sdk/utils.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-15 17:20:29.892880 composio_core-0.2.1/composio_core.egg-info/
+-rw-r--r--   0 utkarsh    (501) staff       (20)      796 2024-04-15 17:20:29.000000 composio_core-0.2.1/composio_core.egg-info/PKG-INFO
+-rw-r--r--   0 utkarsh    (501) staff       (20)      489 2024-04-15 17:20:29.000000 composio_core-0.2.1/composio_core.egg-info/SOURCES.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-04-15 17:20:29.000000 composio_core-0.2.1/composio_core.egg-info/dependency_links.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       60 2024-04-15 17:20:29.000000 composio_core-0.2.1/composio_core.egg-info/entry_points.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)      103 2024-04-15 17:20:29.000000 composio_core-0.2.1/composio_core.egg-info/requires.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)        9 2024-04-15 17:20:29.000000 composio_core-0.2.1/composio_core.egg-info/top_level.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)      528 2024-04-12 15:10:44.000000 composio_core-0.2.1/pyproject.toml
+-rw-r--r--   0 utkarsh    (501) staff       (20)      130 2024-04-12 15:11:16.000000 composio_core-0.2.1/requirements.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-04-15 17:20:29.893439 composio_core-0.2.1/setup.cfg
+-rw-r--r--   0 utkarsh    (501) staff       (20)     1127 2024-04-15 12:25:07.000000 composio_core-0.2.1/setup.py
```

### Comparing `composio_core-0.2.0/PKG-INFO` & `composio_core-0.2.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composio_core
-Version: 0.2.0
+Version: 0.2.1
 Summary: Core package to act as a bridge between composio platform and other services.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Utkarsh
 Author-email: utkarsh@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `composio_core-0.2.0/composio/composio_cli.py` & `composio_core-0.2.1/composio/composio_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os
 import sys
 from beaupy.spinners import Spinner, DOTS
 from rich.console import Console
 from uuid import getnode as get_mac
 
 import termcolor
-from .sdk.storage import get_base_url, get_user_connection, save_api_key, save_user_connection
+from .sdk.storage import get_base_url, save_api_key
 from .sdk.core import ComposioCore, UnauthorizedAccessException
 from .sdk.utils import generate_enums, generate_enums_beta
 from rich.table import Table
 
 import webbrowser
 
 from importlib.metadata import version
@@ -272,22 +272,25 @@
         for field in required_fields:
             field_props = properties.get(field, {})
             field_title = field_props.get('title', field)
             field_description = field_props.get('description', '')
             user_input = input(f"{field_title} ({field_description}): ")
             user_inputs[field] = user_input
         
-        user_connection = get_user_connection(app_key)
-        if not user_connection:
-            console.print(f"[red]No connection found for {app_key}.\nUse the following command to add a connection: [green]composio-cli add {app_key}[/green][/red]")
+        app_enum = client.get_action_enum(app_key)
+        if not app_enum:
+            console.print(f"[red]No such app found for {app_key}.\nUse the following command to get list of available apps: [green]composio-cli add show-apps[/green][/red]")
             sys.exit(1)
         
-        connected_account_id = get_user_connection(app_key)
+        connected_account = client.get_connection(app_key)
+        if not connected_account:
+            console.print(f"[red]No connection found for {app_key}.\nUse the following command to add a connection: [green]composio-cli add {app_key}[/green][/red]")
+            sys.exit(1)
         # Assuming there's a function to enable the trigger with user inputs
-        resp = client.enable_trigger(trigger_name, connected_account_id, user_inputs)
+        resp = client.enable_trigger(trigger_name, connected_account.id, user_inputs)
         console.print(f"\n[green]✔ Trigger enabled successfully![/green]\n")
         if 'triggerId' in resp:
             console.print(f"[green]Trigger ID: {resp['triggerId']}[/green]")
     except Exception as e:
        try:
          error_json = json.loads(str(e))
          error_message = error_json.get("message", "Error message not found")
@@ -316,29 +319,30 @@
 
 def add_integration(args):
     global should_disable_webbrowser_open
 
     client = ComposioCore()
     integration_name = args.integration_name
 
-    existing_connection = get_user_connection(integration_name)
+    entity = client.sdk.get_entity("default")
+    existing_connection = client.get_connection(integration_name, entity_id="default")
     if existing_connection is not None:
         console.print(f"[yellow]Warning: An existing connection for {integration_name} was found.[/yellow]\n")
         replace_connection = input("> Do you want to replace the existing connection? (yes/no): ").lower()
         if replace_connection not in ['yes', 'y']:
             console.print("\n[green]Existing connection retained. No new connection added.[/green]\n")
             return
 
     console.print(f"\n[green]> Adding integration: {integration_name.capitalize()}...[/green]\n")
     try:
         app = client.sdk.get_app(args.integration_name)
         auth_schemes = app.get('auth_schemes')
         auth_schemes_arr = [auth_scheme.get('auth_mode') for auth_scheme in auth_schemes]
         if len(auth_schemes_arr) > 1 and auth_schemes_arr[0] == 'API_KEY':
-            connection = client.initiate_connection(integration_name.lower())
+            connection = entity.initiate_connection(integration_name.lower())
             fields = auth_schemes[0].get('fields')
             fields_input = {}
             for field in fields:
                 if field.get('expected_from_customer', True):
                     if field.get('required', False):
                         console.print(f"[green]> Enter {field.get('displayName', field.get('name'))}: [/green]", end="")
                         value = input() or field.get('default')
@@ -349,23 +353,22 @@
                         console.print(f"[green]> Enter {field.get('displayName', field.get('name'))} (Optional): [/green]", end="")
                         value = input() or field.get('default')
                     fields_input[field.get('name')] = value
 
             connection.save_user_access_data(fields_input)
         else: 
             # @TODO: add logic to wait and ask for API_KEY
-            connection = client.initiate_connection(integration_name.lower())
+            connection = entity.initiate_connection(integration_name.lower())
             if not should_disable_webbrowser_open:
                 webbrowser.open(connection.redirectUrl)
             print(f"Please authenticate {integration_name} in the browser and come back here. URL: {connection.redirectUrl}")
             spinner = Spinner(DOTS, f"[yellow]⚠[/yellow] Waiting for {integration_name} authentication...")
             spinner.start()
             connected_account = connection.wait_until_active()
             spinner.stop()
-        save_user_connection(connected_account.id, integration_name)
         print("")
         console.print(f"[green]✔[/green] {integration_name} added successfully!")
     except Exception as e:
         console.print(f"[red] Error occurred during adding integration: {e}[/red]")
         sys.exit(1)
 
 def show_apps(args):
```

### Comparing `composio_core-0.2.0/composio/sdk/core.py` & `composio_core-0.2.1/composio/sdk/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from typing import Union
 import requests
 
 from .utils import get_git_user_info
 from .sdk import ConnectionRequest, ConnectedAccount
-from .storage import delete_user_connections, get_base_url, get_user_connection, get_api_key, load_user_data, save_api_key, save_user_data, set_base_url
+from .storage import get_base_url, get_api_key, load_user_data, save_user_data, set_base_url
 from .sdk import Composio
 from .enums import Action, App
 from enum import Enum
+import os
 
 class FrameworkEnum(Enum):
     AUTOGEN = "autogen"
     LANGCHAIN = "langchain"
     LYZR = "lyzr"
 
 __IS_FIRST_TIME__ = True
@@ -18,33 +19,33 @@
 class UnauthorizedAccessException(Exception):
     pass
 
 class ComposioCore:
     sdk: Composio = None
     framework: FrameworkEnum = None
 
-    def __init__(self, base_url = get_base_url(), manage_auth = True, framework: FrameworkEnum = None):
+    def __init__(self, base_url = get_base_url(), manage_auth = True, framework: FrameworkEnum = None, api_key: str = None):
         global __IS_FIRST_TIME__
 
         self.base_url = base_url
         self.manage_auth = manage_auth
         self.http_client = requests.Session()
         self.framework = framework
         self.http_client.headers.update({
             'Content-Type': 'application/json'
         })
 
         if manage_auth:
-            api_key = get_api_key()
-            if api_key:
+            api_key_to_use = api_key if api_key else get_api_key()
+            if api_key_to_use:
                 self.http_client.headers.update({
                     'Content-Type': 'application/json',
-                    'x-api-key': api_key
+                    'x-api-key': api_key_to_use
                 });
-                self.sdk = Composio(api_key, base_url)
+                self.sdk = Composio(api_key=api_key_to_use, base_url=base_url)
                 if framework is not None and __IS_FIRST_TIME__ == True:
                     try: 
                         git_info = get_git_user_info()
                         self.http_client.post(f"{self.base_url}/v1/client/auth/track", json={
                             "framework": self.framework.value,
                             "user_git_user_info": {
                                 "name": git_info.name,
@@ -52,15 +53,16 @@
                             } if git_info.name and git_info.email else None
                         });
                         __IS_FIRST_TIME__ = False
                     except:
                         pass
     
     def get_authenticated_user(self):
-        api_key = get_api_key()
+        composio_api_key = os.environ.get("COMPOSIO_API_KEY", None)
+        api_key = composio_api_key if composio_api_key else get_api_key()
         return {
             "api_key": api_key,
         }
 
     def is_authenticated(self):
         if self.sdk is None:
             return False
@@ -73,15 +75,14 @@
             'Content-Type': 'application/json'
         })
     
     def logout(self):
         self.http_client.headers.pop('x-api-key')
         user_data = load_user_data()
         user_data.pop('api_key')
-        delete_user_connections()
         save_user_data(user_data)
 
     def generate_cli_auth_session(self):
         resp = self.http_client.get(f"{self.base_url}/v1/cli/generate-cli-session");
         if resp.status_code == 200:
             resp = resp.json()
             if resp.get('key'):
@@ -142,31 +143,25 @@
             raise Exception(f"Failed to enable trigger: {e}")
     
     def enable_trigger(self, trigger_id: str, connected_account_id: str, user_inputs: dict):
         try:
             return self.sdk.enable_trigger(trigger_id, connected_account_id, user_inputs)
         except Exception as e:
             raise Exception(e)
+        
+    def get_connection(self, app_name: str, entity_id: str = "default"):
+        entity = self.sdk.get_entity(entity_id)
+        return entity.get_connection(app_name)
 
-    def get_saved_connections(self, app_name: str = None):
-        connectionId = get_user_connection(app_name)
-        return connectionId
-
-    def execute_action(self, action: Action, params: dict, entity_id: str = None):
+    def execute_action(self, action: Action, params: dict, entity_id: str = "default"):
         tool_name  = action.value[0]
-        if entity_id is not None:
-            entity = self.sdk.get_entity(entity_id)
-            account = entity.get_connection(tool_name)
-            if not account:
-                raise Exception(f"Entity {entity_id} does not have a connection to {tool_name}")
-        else:
-            connectionId = get_user_connection(tool_name)
-            if not connectionId:
-                raise Exception(f"User not authenticated or connection not found. Please authenticate using: composio-cli add {tool_name}")
-            account = self.sdk.get_connected_account(connectionId)
+        entity = self.sdk.get_entity(entity_id)
+        account = entity.get_connection(tool_name)
+        if not account:
+            raise Exception(f"Entity {entity_id} does not have a connection to {tool_name}")
 
         resp = account.execute_action(action, params)
         return resp
 
     def get_list_of_connections(self, app_name: list[Union[App, str]] = None) -> list[ConnectedAccount]:
         for i, item in enumerate(app_name):
             if isinstance(item, App):
```

### Comparing `composio_core-0.2.0/composio/sdk/enums.py` & `composio_core-0.2.1/composio/sdk/enums.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.2.0/composio/sdk/sdk.py` & `composio_core-0.2.1/composio/sdk/sdk.py`

 * *Files 2% similar despite different names*

```diff
@@ -350,27 +350,28 @@
         )
         if resp.status_code == 200:
             return ConnectedAccount(self, **resp.json())
 
         raise Exception("Failed to get connection")
 
     def get_connected_accounts(
-        self, entity_id: Union[list[str], str], status: str = None
+        self, entity_id: Union[list[str], str] = None, status: str = None
     ) -> list[ConnectedAccount]:
-        user_uuid_str = entity_id if isinstance(entity_id, str) else ",".join(entity_id)
-        resp = self.http_client.get(
-            f"{self.base_url}/v1/connectedAccounts?user_uuid={user_uuid_str}{'&status=' + status if status else ''}"
-        )
-        if resp.status_code == 200:
-            return [ConnectedAccount(self, **item) for item in resp.json()["items"]]
-
-        raise Exception("Failed to get connected accounts")
+        query_params = {}
+        if entity_id is not None:
+            query_params['user_uuid'] = entity_id if isinstance(entity_id, str) else ",".join(entity_id)
+        if status:
+            query_params['status'] = status
+
+        query_string = "&".join([f"{key}={value}" for key, value in query_params.items()])
+        url = f"{self.base_url}/v1/connectedAccounts"
+        if query_string:
+            url += f"?{query_string}"
 
-    def get_list_of_connected_accounts(self) -> list[ConnectedAccount]:
-        resp = self.http_client.get(f"{self.base_url}/v1/connectedAccounts")
+        resp = self.http_client.get(url)
         if resp.status_code == 200:
             return [ConnectedAccount(self, **item) for item in resp.json()["items"]]
 
         raise Exception("Failed to get connected accounts")
 
     def get_action_enum(self, action_name: str, tool_name: str) -> Action:
         for action in Action:
```

### Comparing `composio_core-0.2.0/composio/sdk/utils.py` & `composio_core-0.2.1/composio/sdk/utils.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.2.0/composio_core.egg-info/PKG-INFO` & `composio_core-0.2.1/composio_core.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composio_core
-Version: 0.2.0
+Version: 0.2.1
 Summary: Core package to act as a bridge between composio platform and other services.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Utkarsh
 Author-email: utkarsh@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `composio_core-0.2.0/pyproject.toml` & `composio_core-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `composio_core-0.2.0/setup.py` & `composio_core-0.2.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     """Customized setuptools install command."""
 
     def run(self):
         install.run(self)
 
 setup(
     name="composio_core",
-    version="0.2.0",
+    version="0.2.1",
     author="Utkarsh",
     author_email="utkarsh@composio.dev",
     description="Core package to act as a bridge between composio platform and other services.",
     long_description=open(readme_path).read(),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
```

