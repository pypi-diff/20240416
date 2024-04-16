# Comparing `tmp/tenzir_platform-0.3.0.tar.gz` & `tmp/tenzir_platform-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tenzir_platform-0.3.0.tar", max compression
+gzip compressed data, was "tenzir_platform-0.3.1.tar", max compression
```

## Comparing `tenzir_platform-0.3.0.tar` & `tenzir_platform-0.3.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      436 2024-04-05 14:04:00.532799 tenzir_platform-0.3.0/README.md
--rw-r--r--   0        0        0      878 2024-04-09 11:30:34.933121 tenzir_platform-0.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-05 14:04:00.532799 tenzir_platform-0.3.0/tenzir_platform/__init__.py
--rw-r--r--   0        0        0        0 2024-04-05 14:04:00.532799 tenzir_platform-0.3.0/tenzir_platform/helpers/__init__.py
--rw-r--r--   0        0        0     1195 2024-04-05 14:04:00.532799 tenzir_platform-0.3.0/tenzir_platform/helpers/auth_rule.py
--rw-r--r--   0        0        0     1196 2024-04-05 14:04:00.532799 tenzir_platform-0.3.0/tenzir_platform/helpers/cache.py
--rw-r--r--   0        0        0     3216 2024-04-05 14:04:00.532799 tenzir_platform-0.3.0/tenzir_platform/helpers/client.py
--rw-r--r--   0        0        0      887 2024-04-05 16:27:40.856682 tenzir_platform-0.3.0/tenzir_platform/helpers/environment.py
--rw-r--r--   0        0        0     5630 2024-04-09 11:36:58.813286 tenzir_platform-0.3.0/tenzir_platform/helpers/oidc.py
--rw-r--r--   0        0        0     6232 2024-04-09 11:27:53.189086 tenzir_platform-0.3.0/tenzir_platform/subcommand_admin.py
--rw-r--r--   0        0        0      585 2024-04-05 14:04:00.532799 tenzir_platform-0.3.0/tenzir_platform/subcommand_auth.py
--rw-r--r--   0        0        0     5632 2024-04-09 11:36:58.813286 tenzir_platform-0.3.0/tenzir_platform/subcommand_node.py
--rw-r--r--   0        0        0     1741 2024-04-05 14:04:00.536799 tenzir_platform-0.3.0/tenzir_platform/subcommand_workspace.py
--rw-r--r--   0        0        0     1787 2024-04-09 11:36:58.813286 tenzir_platform-0.3.0/tenzir_platform/tenzir_platform.py
--rw-r--r--   0        0        0     1110 1970-01-01 00:00:00.000000 tenzir_platform-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      436 2024-04-05 14:04:00.532799 tenzir_platform-0.3.1/README.md
+-rw-r--r--   0        0        0      878 2024-04-16 08:17:04.609817 tenzir_platform-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-05 14:04:00.532799 tenzir_platform-0.3.1/tenzir_platform/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-05 14:04:00.532799 tenzir_platform-0.3.1/tenzir_platform/helpers/__init__.py
+-rw-r--r--   0        0        0     1195 2024-04-05 14:04:00.532799 tenzir_platform-0.3.1/tenzir_platform/helpers/auth_rule.py
+-rw-r--r--   0        0        0     1196 2024-04-05 14:04:00.532799 tenzir_platform-0.3.1/tenzir_platform/helpers/cache.py
+-rw-r--r--   0        0        0     3216 2024-04-05 14:04:00.532799 tenzir_platform-0.3.1/tenzir_platform/helpers/client.py
+-rw-r--r--   0        0        0      817 2024-04-16 08:17:04.609817 tenzir_platform-0.3.1/tenzir_platform/helpers/environment.py
+-rw-r--r--   0        0        0     5908 2024-04-16 08:17:07.433819 tenzir_platform-0.3.1/tenzir_platform/helpers/oidc.py
+-rw-r--r--   0        0        0     6232 2024-04-15 11:26:22.401320 tenzir_platform-0.3.1/tenzir_platform/subcommand_admin.py
+-rw-r--r--   0        0        0      585 2024-04-05 14:04:00.532799 tenzir_platform-0.3.1/tenzir_platform/subcommand_auth.py
+-rw-r--r--   0        0        0     5654 2024-04-15 11:26:22.401320 tenzir_platform-0.3.1/tenzir_platform/subcommand_node.py
+-rw-r--r--   0        0        0     1741 2024-04-05 14:04:00.536799 tenzir_platform-0.3.1/tenzir_platform/subcommand_workspace.py
+-rw-r--r--   0        0        0     1787 2024-04-15 11:26:22.401320 tenzir_platform-0.3.1/tenzir_platform/tenzir_platform.py
+-rw-r--r--   0        0        0     1110 1970-01-01 00:00:00.000000 tenzir_platform-0.3.1/PKG-INFO
```

### Comparing `tenzir_platform-0.3.0/pyproject.toml` & `tenzir_platform-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tenzir-platform"
-version = "0.3.0"
+version = "0.3.1"
 description = "Tenzir CLI"
 authors = ["Tenzir <engineering@tenzir.com>"]
 readme = "README.md"
 packages = [{ include = "tenzir_platform" }]
 
 [tool.poetry.scripts]
 tenzir-platform = "tenzir_platform.tenzir_platform:main"
```

### Comparing `tenzir_platform-0.3.0/tenzir_platform/helpers/auth_rule.py` & `tenzir_platform-0.3.1/tenzir_platform/helpers/auth_rule.py`

 * *Files identical despite different names*

### Comparing `tenzir_platform-0.3.0/tenzir_platform/helpers/cache.py` & `tenzir_platform-0.3.1/tenzir_platform/helpers/cache.py`

 * *Files identical despite different names*

### Comparing `tenzir_platform-0.3.0/tenzir_platform/helpers/client.py` & `tenzir_platform-0.3.1/tenzir_platform/helpers/client.py`

 * *Files identical despite different names*

### Comparing `tenzir_platform-0.3.0/tenzir_platform/helpers/environment.py` & `tenzir_platform-0.3.1/tenzir_platform/helpers/environment.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 from pydantic_settings import BaseSettings
 
 
-API_ENDPOINT = "https://rest.tenzir.app/production-v1/"
-OIDC_ISSUER_URL = "https://tenzir.eu.auth0.com/"
+API_ENDPOINT = "https://rest.tenzir.app/production-v1"
+OIDC_ISSUER_URL = "https://tenzir.eu.auth0.com"
 OIDC_CLIENT_ID = "vzRh8grIVu1bwutvZbbpBDCOvSzN8AXh"
-OIDC_AUDIENCE = "tenzir_cli"
 
 
 class PlatformEnvironment(BaseSettings):
     # The remote API endpoint of the platform.
     api_endpoint: str = API_ENDPOINT
 
     # An arbitrary short string to identify this environment
     # in the local cache directory.
     stage_identifier: str = "prod"
 
     # TODO: Provide a new `/oidc-config` endpoint in the public platform api
     # to load these values dynamically.
     oidc_issuer_url: str = OIDC_ISSUER_URL
     oidc_client_id: str = OIDC_CLIENT_ID
-    oidc_audience: str = OIDC_AUDIENCE
 
     @staticmethod
     def load():
         return PlatformEnvironment(
             _env_prefix="TENZIR_PLATFORM_CLI", _env_nested_delimiter="__"
         )
```

### Comparing `tenzir_platform-0.3.0/tenzir_platform/helpers/oidc.py` & `tenzir_platform-0.3.1/tenzir_platform/helpers/oidc.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,21 +48,26 @@
 
 
 class IdTokenClient:
     def __init__(self, platform: PlatformEnvironment):
         self.platform_environment = platform
         self.issuer = platform.oidc_issuer_url
         self.client_id = platform.oidc_client_id
-        self.audience = platform.oidc_audience
         self.verbose = False
+        discovery_url = f"{self.issuer.rstrip('/')}/.well-known/openid-configuration"
+        discovered_configuration = requests.get(discovery_url).json()
+        self.jwks_url = discovered_configuration["jwks_uri"]
+        self.token_endpoint = discovered_configuration["token_endpoint"]
+        self.device_authorization_endpoint = discovered_configuration[
+            "device_authorization_endpoint"
+        ]
 
     def validate_token(self, id_token: str) -> ValidOidcToken:
         """Verify the token using the audience specific to the CLI"""
-        jwks_url = f"{self.issuer.rstrip('/')}/.well-known/jwks.json"
-        jwks_client = PyJWKClient(jwks_url)
+        jwks_client = PyJWKClient(self.jwks_url)
         signing_key = jwks_client.get_signing_key_from_jwt(id_token)
         validated_token = jwt.decode(
             id_token,
             signing_key.key,
             algorithms=["RS256"],
             issuer=self.issuer,
             # for id tokens, the audience is the client_id
@@ -74,25 +79,27 @@
         # TODO: Add an option to use password flow for non-interactive environments.
         token_data = self._device_code_flow()
         return self._unwrap_flow_result(token_data)
 
     def _device_code_flow(self) -> dict[str, str]:
         device_code_payload = {
             "client_id": self.client_id,
+            # Request email by default since many auth rules are checked against the email address.
             "scope": "openid email",
-            # This points to an API audience in Auth0
-            "audience": self.audience,
         }
+
         device_code_response = requests.post(
-            f"{self.issuer.rstrip('/')}/oauth/device/code",
+            self.device_authorization_endpoint,
             data=device_code_payload,
         )
 
         if device_code_response.status_code != 200:
-            raise Exception(f"Error generating the device code: {device_code_response.text}")
+            raise Exception(
+                f"Error generating the device code: {device_code_response.text}"
+            )
 
         device_code_data = device_code_response.json()
         print(
             "1. On your computer or mobile device navigate to: ",
             device_code_data["verification_uri_complete"],
         )
         print(
@@ -104,17 +111,15 @@
         token_payload = {
             "grant_type": "urn:ietf:params:oauth:grant-type:device_code",
             "device_code": device_code_data["device_code"],
             "client_id": self.client_id,
         }
         authenticated = False
         while not authenticated:
-            token_response = requests.post(
-                f"{self.issuer.rstrip('/')}/oauth/token", data=token_payload
-            )
+            token_response = requests.post(self.token_endpoint, data=token_payload)
             token_data = token_response.json()
             if token_response.status_code == 200:
                 print("Authenticated!")
                 break
             elif token_data["error"] not in ("authorization_pending", "slow_down"):
                 print(token_data["error_description"])
                 authenticated = True
```

### Comparing `tenzir_platform-0.3.0/tenzir_platform/subcommand_admin.py` & `tenzir_platform-0.3.1/tenzir_platform/subcommand_admin.py`

 * *Files identical despite different names*

### Comparing `tenzir_platform-0.3.0/tenzir_platform/subcommand_auth.py` & `tenzir_platform-0.3.1/tenzir_platform/subcommand_auth.py`

 * *Files identical despite different names*

### Comparing `tenzir_platform-0.3.0/tenzir_platform/subcommand_node.py` & `tenzir_platform-0.3.1/tenzir_platform/subcommand_node.py`

 * *Files 5% similar despite different names*

```diff
@@ -121,15 +121,17 @@
                 "node_id": node_id,
             },
         )
 
 
 def create(client: AppClient, workspace_id: str, node_name: Optional[str]):
     if node_name is None:
-        time_suffix = datetime.datetime.now(datetime.timezone.utc).strftime("%Y%m%dT%H%M%SZ")
+        time_suffix = datetime.datetime.now(datetime.timezone.utc).strftime(
+            "%Y%m%dT%H%M%SZ"
+        )
         node_name = f"node-{time_suffix}"
     resp = client.post(
         "/generate-client-config",
         json={
             "tenant_id": workspace_id,
             "config_type": "docker",
             "node_name": node_name,
```

### Comparing `tenzir_platform-0.3.0/tenzir_platform/subcommand_workspace.py` & `tenzir_platform-0.3.1/tenzir_platform/subcommand_workspace.py`

 * *Files identical despite different names*

### Comparing `tenzir_platform-0.3.0/tenzir_platform/tenzir_platform.py` & `tenzir_platform-0.3.1/tenzir_platform/tenzir_platform.py`

 * *Files identical despite different names*

### Comparing `tenzir_platform-0.3.0/PKG-INFO` & `tenzir_platform-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tenzir-platform
-Version: 0.3.0
+Version: 0.3.1
 Summary: Tenzir CLI
 Author: Tenzir
 Author-email: engineering@tenzir.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

