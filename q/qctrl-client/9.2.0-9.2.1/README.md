# Comparing `tmp/qctrl_client-9.2.0.tar.gz` & `tmp/qctrl_client-9.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qctrl_client-9.2.0.tar", max compression
+gzip compressed data, was "qctrl_client-9.2.1.tar", max compression
```

## Comparing `qctrl_client-9.2.0.tar` & `qctrl_client-9.2.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0    36587 2024-02-20 02:39:50.941439 qctrl_client-9.2.0/LICENSE
--rw-r--r--   0        0        0      214 2024-02-20 02:39:50.941439 qctrl_client-9.2.0/README.md
--rw-r--r--   0        0        0     2567 2024-02-20 02:40:13.609325 qctrl_client-9.2.0/pyproject.toml
--rw-r--r--   0        0        0      683 2024-02-20 02:40:13.617325 qctrl_client-9.2.0/qctrlclient/__init__.py
--rw-r--r--   0        0        0      764 2024-02-20 02:40:13.617325 qctrl_client-9.2.0/qctrlclient/auth/__init__.py
--rw-r--r--   0        0        0     2294 2024-02-20 02:39:50.941439 qctrl_client-9.2.0/qctrlclient/auth/api_key.py
--rw-r--r--   0        0        0     1831 2024-02-20 02:39:50.941439 qctrl_client-9.2.0/qctrlclient/auth/base.py
--rw-r--r--   0        0        0     4982 2024-02-20 02:39:50.941439 qctrl_client-9.2.0/qctrlclient/auth/cli.py
--rw-r--r--   0        0        0      585 2024-02-20 02:39:50.941439 qctrl_client-9.2.0/qctrlclient/auth/constants.py
--rw-r--r--   0        0        0      718 2024-02-20 02:39:50.941439 qctrl_client-9.2.0/qctrlclient/auth/helpers.py
--rw-r--r--   0        0        0     1042 2024-02-20 02:39:50.941439 qctrl_client-9.2.0/qctrlclient/auth/keycloak.py
--rw-r--r--   0        0        0     2131 2024-02-20 02:39:50.941439 qctrl_client-9.2.0/qctrlclient/auth/mixins.py
--rw-r--r--   0        0        0     3824 2024-02-20 02:39:50.941439 qctrl_client-9.2.0/qctrlclient/auth/oidc.py
--rw-r--r--   0        0        0     1801 2024-02-20 02:39:50.941439 qctrl_client-9.2.0/qctrlclient/auth/password.py
--rw-r--r--   0        0        0     3096 2024-02-20 02:39:50.941439 qctrl_client-9.2.0/qctrlclient/auth/redirect_listener.py
--rw-r--r--   0        0        0     1516 2024-02-20 02:39:50.941439 qctrl_client-9.2.0/qctrlclient/auth/service_account.py
--rw-r--r--   0        0        0     2439 2024-02-20 02:39:50.941439 qctrl_client-9.2.0/qctrlclient/auth/token_exchange.py
--rw-r--r--   0        0        0     7747 2024-02-20 02:39:50.941439 qctrl_client-9.2.0/qctrlclient/client.py
--rw-r--r--   0        0        0     2172 2024-02-20 02:39:50.941439 qctrl_client-9.2.0/qctrlclient/exceptions.py
--rw-r--r--   0        0        0     1424 2024-02-20 02:39:50.945438 qctrl_client-9.2.0/qctrlclient/pytest_plugin.py
--rw-r--r--   0        0        0      601 2024-02-20 02:40:13.617325 qctrl_client-9.2.0/qctrlclient/transports/__init__.py
--rw-r--r--   0        0        0     4628 2024-02-20 02:39:50.945438 qctrl_client-9.2.0/qctrlclient/transports/requests_transport.py
--rw-r--r--   0        0        0     2290 1970-01-01 00:00:00.000000 qctrl_client-9.2.0/PKG-INFO
+-rw-r--r--   0        0        0    36587 2024-04-16 06:13:19.915022 qctrl_client-9.2.1/LICENSE
+-rw-r--r--   0        0        0      214 2024-04-16 06:13:19.915022 qctrl_client-9.2.1/README.md
+-rw-r--r--   0        0        0     2566 2024-04-16 06:13:43.879356 qctrl_client-9.2.1/pyproject.toml
+-rw-r--r--   0        0        0      683 2024-04-16 06:13:43.887356 qctrl_client-9.2.1/qctrlclient/__init__.py
+-rw-r--r--   0        0        0      764 2024-04-16 06:13:43.883356 qctrl_client-9.2.1/qctrlclient/auth/__init__.py
+-rw-r--r--   0        0        0     2294 2024-04-16 06:13:19.915022 qctrl_client-9.2.1/qctrlclient/auth/api_key.py
+-rw-r--r--   0        0        0     1831 2024-04-16 06:13:19.915022 qctrl_client-9.2.1/qctrlclient/auth/base.py
+-rw-r--r--   0        0        0     4982 2024-04-16 06:13:19.915022 qctrl_client-9.2.1/qctrlclient/auth/cli.py
+-rw-r--r--   0        0        0      585 2024-04-16 06:13:19.915022 qctrl_client-9.2.1/qctrlclient/auth/constants.py
+-rw-r--r--   0        0        0      718 2024-04-16 06:13:19.915022 qctrl_client-9.2.1/qctrlclient/auth/helpers.py
+-rw-r--r--   0        0        0     1042 2024-04-16 06:13:19.915022 qctrl_client-9.2.1/qctrlclient/auth/keycloak.py
+-rw-r--r--   0        0        0     2131 2024-04-16 06:13:19.915022 qctrl_client-9.2.1/qctrlclient/auth/mixins.py
+-rw-r--r--   0        0        0     3824 2024-04-16 06:13:19.915022 qctrl_client-9.2.1/qctrlclient/auth/oidc.py
+-rw-r--r--   0        0        0     1973 2024-04-16 06:13:19.915022 qctrl_client-9.2.1/qctrlclient/auth/password.py
+-rw-r--r--   0        0        0     3096 2024-04-16 06:13:19.915022 qctrl_client-9.2.1/qctrlclient/auth/redirect_listener.py
+-rw-r--r--   0        0        0     1516 2024-04-16 06:13:19.915022 qctrl_client-9.2.1/qctrlclient/auth/service_account.py
+-rw-r--r--   0        0        0     2439 2024-04-16 06:13:19.915022 qctrl_client-9.2.1/qctrlclient/auth/token_exchange.py
+-rw-r--r--   0        0        0     7747 2024-04-16 06:13:19.915022 qctrl_client-9.2.1/qctrlclient/client.py
+-rw-r--r--   0        0        0     2172 2024-04-16 06:13:19.915022 qctrl_client-9.2.1/qctrlclient/exceptions.py
+-rw-r--r--   0        0        0     1424 2024-04-16 06:13:19.915022 qctrl_client-9.2.1/qctrlclient/pytest_plugin.py
+-rw-r--r--   0        0        0      601 2024-04-16 06:13:43.887356 qctrl_client-9.2.1/qctrlclient/transports/__init__.py
+-rw-r--r--   0        0        0     4628 2024-04-16 06:13:19.915022 qctrl_client-9.2.1/qctrlclient/transports/requests_transport.py
+-rw-r--r--   0        0        0     2290 1970-01-01 00:00:00.000000 qctrl_client-9.2.1/PKG-INFO
```

### Comparing `qctrl_client-9.2.0/LICENSE` & `qctrl_client-9.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qctrl_client-9.2.0/pyproject.toml` & `qctrl_client-9.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qctrl-client"
-version = "9.2.0"
+version = "9.2.1"
 description = "Q-CTRL Client"
 license = "https://q-ctrl.com/terms"
 authors = ["Q-CTRL <support@q-ctrl.com>"]
 maintainers = ["Q-CTRL <support@q-ctrl.com>"]
 readme = "README.md"
 homepage = "https://q-ctrl.com"
 documentation = "https://docs.q-ctrl.com"
@@ -82,15 +82,15 @@
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.0"
 pytest-cov = "^4.1.0"
 pytest-mock = "^3.12.0"
 pylint = "^2.14.4"
 pylint_runner = "^0.6.0"
-black = "^23.10.0"
+black = "^24.3.0"
 isort = "^5.12.0"
 pre-commit = "^3.5.0"
 
 [tool.isort]
 profile = "black"
 force_grid_wrap = "2"
```

### Comparing `qctrl_client-9.2.0/qctrlclient/__init__.py` & `qctrl_client-9.2.1/qctrlclient/__init__.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-9.2.0/qctrlclient/auth/__init__.py` & `qctrl_client-9.2.1/qctrlclient/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-9.2.0/qctrlclient/auth/api_key.py` & `qctrl_client-9.2.1/qctrlclient/auth/api_key.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-9.2.0/qctrlclient/auth/base.py` & `qctrl_client-9.2.1/qctrlclient/auth/base.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-9.2.0/qctrlclient/auth/cli.py` & `qctrl_client-9.2.1/qctrlclient/auth/cli.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-9.2.0/qctrlclient/auth/constants.py` & `qctrl_client-9.2.1/qctrlclient/auth/constants.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-9.2.0/qctrlclient/auth/helpers.py` & `qctrl_client-9.2.1/qctrlclient/auth/helpers.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-9.2.0/qctrlclient/auth/keycloak.py` & `qctrl_client-9.2.1/qctrlclient/auth/keycloak.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-9.2.0/qctrlclient/auth/mixins.py` & `qctrl_client-9.2.1/qctrlclient/auth/mixins.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-9.2.0/qctrlclient/auth/oidc.py` & `qctrl_client-9.2.1/qctrlclient/auth/oidc.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-9.2.0/qctrlclient/auth/password.py` & `qctrl_client-9.2.1/qctrlclient/auth/password.py`

 * *Files 10% similar despite different names*

```diff
@@ -45,15 +45,21 @@
         super().__init__()
 
     def _get_urls(self):
         return get_keycloak_oidc_urls(self._base_url)
 
     def _create_session(self):
         client = LegacyApplicationClient(client_id=self._client_id)
-        return OAuth2Session(client=client)
+        return OAuth2Session(
+            client=client,
+            auto_refresh_kwargs={
+                "client_id": self._client_id,
+                "client_secret": self._client_secret,
+            },
+        )
 
     def _authenticate(self):
         self._oidc_session.fetch_token(
             self._urls.token_url,
             client_secret=self._client_secret,
             username=self._username,
             password=self._password,
```

### Comparing `qctrl_client-9.2.0/qctrlclient/auth/redirect_listener.py` & `qctrl_client-9.2.1/qctrlclient/auth/redirect_listener.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-9.2.0/qctrlclient/auth/service_account.py` & `qctrl_client-9.2.1/qctrlclient/auth/service_account.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-9.2.0/qctrlclient/auth/token_exchange.py` & `qctrl_client-9.2.1/qctrlclient/auth/token_exchange.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-9.2.0/qctrlclient/client.py` & `qctrl_client-9.2.1/qctrlclient/client.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-9.2.0/qctrlclient/exceptions.py` & `qctrl_client-9.2.1/qctrlclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-9.2.0/qctrlclient/pytest_plugin.py` & `qctrl_client-9.2.1/qctrlclient/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-9.2.0/qctrlclient/transports/__init__.py` & `qctrl_client-9.2.1/qctrlclient/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-9.2.0/qctrlclient/transports/requests_transport.py` & `qctrl_client-9.2.1/qctrlclient/transports/requests_transport.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-9.2.0/PKG-INFO` & `qctrl_client-9.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qctrl-client
-Version: 9.2.0
+Version: 9.2.1
 Summary: Q-CTRL Client
 Home-page: https://q-ctrl.com
 License: https://q-ctrl.com/terms
 Keywords: black opal,boulder opal,fire opal,nisq,open controls,q control,q ctrl,q-control,q-ctrl,qcontrol,qctrl,quantum,quantum algorithms,quantum circuits,quantum coding,quantum coding software,quantum computing,quantum control,quantum control software,quantum control theory,quantum engineering,quantum error correction,quantum firmware,quantum fundamentals,quantum sensing,qubit,qudit
 Author: Q-CTRL
 Author-email: support@q-ctrl.com
 Maintainer: Q-CTRL
```

