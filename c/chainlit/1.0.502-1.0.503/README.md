# Comparing `tmp/chainlit-1.0.502.tar.gz` & `tmp/chainlit-1.0.503.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chainlit-1.0.502.tar", max compression
+gzip compressed data, was "chainlit-1.0.503.tar", max compression
```

## Comparing `chainlit-1.0.502.tar` & `chainlit-1.0.503.tar`

### file list

```diff
@@ -1,65 +1,67 @@
--rw-r--r--   0        0        0     3884 2024-04-08 16:42:56.058701 chainlit-1.0.502/README.md
--rw-r--r--   0        0        0     9667 2024-04-08 16:42:17.718612 chainlit-1.0.502/chainlit/__init__.py
--rw-r--r--   0        0        0       87 2024-04-08 16:42:17.718612 chainlit-1.0.502/chainlit/__main__.py
--rw-r--r--   0        0        0     1410 2024-04-08 16:42:17.718612 chainlit-1.0.502/chainlit/action.py
--rw-r--r--   0        0        0     2681 2024-04-08 16:42:17.718612 chainlit-1.0.502/chainlit/auth.py
--rw-r--r--   0        0        0     1361 2024-04-08 16:42:17.718612 chainlit-1.0.502/chainlit/cache.py
--rw-r--r--   0        0        0      877 2024-04-08 16:42:17.718612 chainlit-1.0.502/chainlit/chat_settings.py
--rw-r--r--   0        0        0     4949 2024-04-08 16:42:17.718612 chainlit-1.0.502/chainlit/cli/__init__.py
--rw-r--r--   0        0        0      717 2024-04-08 16:42:17.718612 chainlit-1.0.502/chainlit/cli/utils.py
--rw-r--r--   0        0        0    15066 2024-04-08 16:42:17.718612 chainlit-1.0.502/chainlit/config.py
--rw-r--r--   0        0        0     2476 2024-04-08 16:42:17.718612 chainlit-1.0.502/chainlit/context.py
--rw-r--r--   0        0        0     8887 2024-04-08 16:45:18.735901 chainlit-1.0.502/chainlit/copilot/dist/assets/logo_dark-2a3cf740.svg
--rw-r--r--   0        0        0     8889 2024-04-08 16:45:18.735901 chainlit-1.0.502/chainlit/copilot/dist/assets/logo_light-b078e7bc.svg
--rw-r--r--   0        0        0  7015695 2024-04-08 16:45:18.735901 chainlit-1.0.502/chainlit/copilot/dist/index.js
--rw-r--r--   0        0        0    15588 2024-04-08 16:42:17.718612 chainlit-1.0.502/chainlit/data/__init__.py
--rw-r--r--   0        0        0      461 2024-04-08 16:42:17.718612 chainlit-1.0.502/chainlit/data/acl.py
--rw-r--r--   0        0        0    10162 2024-04-08 16:42:17.718612 chainlit-1.0.502/chainlit/element.py
--rw-r--r--   0        0        0    12178 2024-04-08 16:42:17.718612 chainlit-1.0.502/chainlit/emitter.py
--rw-r--r--   0        0        0     6605 2024-04-08 16:45:18.723901 chainlit-1.0.502/chainlit/frontend/dist/assets/index-d088547c.css
--rw-r--r--   0        0        0  3072941 2024-04-08 16:45:18.723901 chainlit-1.0.502/chainlit/frontend/dist/assets/index-e306c2e5.js
--rw-r--r--   0        0        0     8887 2024-04-08 16:45:18.719901 chainlit-1.0.502/chainlit/frontend/dist/assets/logo_dark-2a3cf740.svg
--rw-r--r--   0        0        0     8889 2024-04-08 16:45:18.719901 chainlit-1.0.502/chainlit/frontend/dist/assets/logo_light-b078e7bc.svg
--rw-r--r--   0        0        0  3763471 2024-04-08 16:45:18.727901 chainlit-1.0.502/chainlit/frontend/dist/assets/react-plotly-cc656f1c.js
--rw-r--r--   0        0        0     6455 2024-04-08 16:45:18.719901 chainlit-1.0.502/chainlit/frontend/dist/favicon.svg
--rw-r--r--   0        0        0     1005 2024-04-08 16:45:18.719901 chainlit-1.0.502/chainlit/frontend/dist/index.html
--rw-r--r--   0        0        0      217 2024-04-08 16:42:17.718612 chainlit-1.0.502/chainlit/haystack/__init__.py
--rw-r--r--   0        0        0     5209 2024-04-08 16:42:17.718612 chainlit-1.0.502/chainlit/haystack/callbacks.py
--rw-r--r--   0        0        0      416 2024-04-08 16:42:17.718612 chainlit-1.0.502/chainlit/hello.py
--rw-r--r--   0        0        0     4880 2024-04-08 16:42:17.718612 chainlit-1.0.502/chainlit/input_widget.py
--rw-r--r--   0        0        0      217 2024-04-08 16:42:17.718612 chainlit-1.0.502/chainlit/langchain/__init__.py
--rw-r--r--   0        0        0    20484 2024-04-08 16:42:17.718612 chainlit-1.0.502/chainlit/langchain/callbacks.py
--rw-r--r--   0        0        0      817 2024-04-08 16:42:17.718612 chainlit-1.0.502/chainlit/langflow/__init__.py
--rw-r--r--   0        0        0      227 2024-04-08 16:42:17.718612 chainlit-1.0.502/chainlit/llama_index/__init__.py
--rw-r--r--   0        0        0     7225 2024-04-08 16:42:17.718612 chainlit-1.0.502/chainlit/llama_index/callbacks.py
--rw-r--r--   0        0        0      373 2024-04-08 16:42:17.718612 chainlit-1.0.502/chainlit/logger.py
--rw-r--r--   0        0        0     2025 2024-04-08 16:42:17.718612 chainlit-1.0.502/chainlit/markdown.py
--rw-r--r--   0        0        0    17974 2024-04-08 16:42:17.718612 chainlit-1.0.502/chainlit/message.py
--rw-r--r--   0        0        0    17459 2024-04-08 16:42:17.718612 chainlit-1.0.502/chainlit/oauth_providers.py
--rw-r--r--   0        0        0     1993 2024-04-08 16:42:17.718612 chainlit-1.0.502/chainlit/openai/__init__.py
--rw-r--r--   0        0        0       80 2024-04-08 16:42:17.722612 chainlit-1.0.502/chainlit/playground/__init__.py
--rw-r--r--   0        0        0      948 2024-04-08 16:42:17.722612 chainlit-1.0.502/chainlit/playground/config.py
--rw-r--r--   0        0        0     3858 2024-04-08 16:42:17.722612 chainlit-1.0.502/chainlit/playground/provider.py
--rw-r--r--   0        0        0      207 2024-04-08 16:42:17.722612 chainlit-1.0.502/chainlit/playground/providers/__init__.py
--rw-r--r--   0        0        0     3495 2024-04-08 16:42:17.722612 chainlit-1.0.502/chainlit/playground/providers/anthropic.py
--rw-r--r--   0        0        0     2130 2024-04-08 16:42:17.722612 chainlit-1.0.502/chainlit/playground/providers/huggingface.py
--rw-r--r--   0        0        0     3103 2024-04-08 16:42:17.722612 chainlit-1.0.502/chainlit/playground/providers/langchain.py
--rw-r--r--   0        0        0    11956 2024-04-08 16:42:17.722612 chainlit-1.0.502/chainlit/playground/providers/openai.py
--rw-r--r--   0        0        0     5084 2024-04-08 16:42:17.722612 chainlit-1.0.502/chainlit/playground/providers/vertexai.py
--rw-r--r--   0        0        0        0 2024-04-08 16:42:17.722612 chainlit-1.0.502/chainlit/py.typed
--rw-r--r--   0        0        0      295 2024-04-08 16:42:17.722612 chainlit-1.0.502/chainlit/secret.py
--rw-r--r--   0        0        0    23716 2024-04-08 16:42:17.722612 chainlit-1.0.502/chainlit/server.py
--rw-r--r--   0        0        0     8844 2024-04-08 16:42:17.722612 chainlit-1.0.502/chainlit/session.py
--rw-r--r--   0        0        0     9995 2024-04-08 16:42:17.722612 chainlit-1.0.502/chainlit/socket.py
--rw-r--r--   0        0        0    13102 2024-04-08 16:42:17.722612 chainlit-1.0.502/chainlit/step.py
--rw-r--r--   0        0        0     1235 2024-04-08 16:42:17.722612 chainlit-1.0.502/chainlit/sync.py
--rw-r--r--   0        0        0     3060 2024-04-08 16:42:17.722612 chainlit-1.0.502/chainlit/telemetry.py
--rw-r--r--   0        0        0     7835 2024-04-08 16:42:17.722612 chainlit-1.0.502/chainlit/translations/en-US.json
--rw-r--r--   0        0        0     2034 2024-04-08 16:42:17.722612 chainlit-1.0.502/chainlit/translations.py
--rw-r--r--   0        0        0     3375 2024-04-08 16:42:17.722612 chainlit-1.0.502/chainlit/types.py
--rw-r--r--   0        0        0      619 2024-04-08 16:42:17.722612 chainlit-1.0.502/chainlit/user.py
--rw-r--r--   0        0        0     1368 2024-04-08 16:42:17.722612 chainlit-1.0.502/chainlit/user_session.py
--rw-r--r--   0        0        0     2571 2024-04-08 16:42:17.722612 chainlit-1.0.502/chainlit/utils.py
--rw-r--r--   0        0        0      196 2024-04-08 16:42:17.722612 chainlit-1.0.502/chainlit/version.py
--rw-r--r--   0        0        0     2141 2024-04-08 16:42:17.722612 chainlit-1.0.502/pyproject.toml
--rw-r--r--   0        0        0     5560 1970-01-01 00:00:00.000000 chainlit-1.0.502/PKG-INFO
+-rw-r--r--   0        0        0     3884 2024-04-15 14:32:47.386217 chainlit-1.0.503/README.md
+-rw-r--r--   0        0        0     9667 2024-04-15 14:32:22.638272 chainlit-1.0.503/chainlit/__init__.py
+-rw-r--r--   0        0        0       87 2024-04-15 14:32:22.638272 chainlit-1.0.503/chainlit/__main__.py
+-rw-r--r--   0        0        0     1410 2024-04-15 14:32:22.638272 chainlit-1.0.503/chainlit/action.py
+-rw-r--r--   0        0        0     2681 2024-04-15 14:32:22.638272 chainlit-1.0.503/chainlit/auth.py
+-rw-r--r--   0        0        0     1361 2024-04-15 14:32:22.638272 chainlit-1.0.503/chainlit/cache.py
+-rw-r--r--   0        0        0      877 2024-04-15 14:32:22.638272 chainlit-1.0.503/chainlit/chat_settings.py
+-rw-r--r--   0        0        0     4951 2024-04-15 14:32:22.638272 chainlit-1.0.503/chainlit/cli/__init__.py
+-rw-r--r--   0        0        0      717 2024-04-15 14:32:22.638272 chainlit-1.0.503/chainlit/cli/utils.py
+-rw-r--r--   0        0        0    15066 2024-04-15 14:32:22.638272 chainlit-1.0.503/chainlit/config.py
+-rw-r--r--   0        0        0     2476 2024-04-15 14:32:22.638272 chainlit-1.0.503/chainlit/context.py
+-rw-r--r--   0        0        0     8887 2024-04-15 14:35:04.821836 chainlit-1.0.503/chainlit/copilot/dist/assets/logo_dark-2a3cf740.svg
+-rw-r--r--   0        0        0     8889 2024-04-15 14:35:04.821836 chainlit-1.0.503/chainlit/copilot/dist/assets/logo_light-b078e7bc.svg
+-rw-r--r--   0        0        0  7015707 2024-04-15 14:35:04.821836 chainlit-1.0.503/chainlit/copilot/dist/index.js
+-rw-r--r--   0        0        0    16321 2024-04-15 14:32:22.638272 chainlit-1.0.503/chainlit/data/__init__.py
+-rw-r--r--   0        0        0      461 2024-04-15 14:32:22.638272 chainlit-1.0.503/chainlit/data/acl.py
+-rw-r--r--   0        0        0    24600 2024-04-15 14:32:22.638272 chainlit-1.0.503/chainlit/data/sql_alchemy.py
+-rw-r--r--   0        0        0     3007 2024-04-15 14:32:22.638272 chainlit-1.0.503/chainlit/data/storage_clients.py
+-rw-r--r--   0        0        0    10162 2024-04-15 14:32:22.638272 chainlit-1.0.503/chainlit/element.py
+-rw-r--r--   0        0        0    12339 2024-04-15 14:32:22.638272 chainlit-1.0.503/chainlit/emitter.py
+-rw-r--r--   0        0        0  3072953 2024-04-15 14:35:04.813836 chainlit-1.0.503/chainlit/frontend/dist/assets/index-a8e1b559.js
+-rw-r--r--   0        0        0     6605 2024-04-15 14:35:04.809836 chainlit-1.0.503/chainlit/frontend/dist/assets/index-d088547c.css
+-rw-r--r--   0        0        0     8887 2024-04-15 14:35:04.805836 chainlit-1.0.503/chainlit/frontend/dist/assets/logo_dark-2a3cf740.svg
+-rw-r--r--   0        0        0     8889 2024-04-15 14:35:04.809836 chainlit-1.0.503/chainlit/frontend/dist/assets/logo_light-b078e7bc.svg
+-rw-r--r--   0        0        0  3763471 2024-04-15 14:35:04.809836 chainlit-1.0.503/chainlit/frontend/dist/assets/react-plotly-b225b63c.js
+-rw-r--r--   0        0        0     6455 2024-04-15 14:35:04.805836 chainlit-1.0.503/chainlit/frontend/dist/favicon.svg
+-rw-r--r--   0        0        0     1005 2024-04-15 14:35:04.805836 chainlit-1.0.503/chainlit/frontend/dist/index.html
+-rw-r--r--   0        0        0      217 2024-04-15 14:32:22.638272 chainlit-1.0.503/chainlit/haystack/__init__.py
+-rw-r--r--   0        0        0     5209 2024-04-15 14:32:22.638272 chainlit-1.0.503/chainlit/haystack/callbacks.py
+-rw-r--r--   0        0        0      416 2024-04-15 14:32:22.638272 chainlit-1.0.503/chainlit/hello.py
+-rw-r--r--   0        0        0     4880 2024-04-15 14:32:22.638272 chainlit-1.0.503/chainlit/input_widget.py
+-rw-r--r--   0        0        0      217 2024-04-15 14:32:22.638272 chainlit-1.0.503/chainlit/langchain/__init__.py
+-rw-r--r--   0        0        0    20484 2024-04-15 14:32:22.638272 chainlit-1.0.503/chainlit/langchain/callbacks.py
+-rw-r--r--   0        0        0      817 2024-04-15 14:32:22.638272 chainlit-1.0.503/chainlit/langflow/__init__.py
+-rw-r--r--   0        0        0      227 2024-04-15 14:32:22.638272 chainlit-1.0.503/chainlit/llama_index/__init__.py
+-rw-r--r--   0        0        0     7225 2024-04-15 14:32:22.638272 chainlit-1.0.503/chainlit/llama_index/callbacks.py
+-rw-r--r--   0        0        0      373 2024-04-15 14:32:22.638272 chainlit-1.0.503/chainlit/logger.py
+-rw-r--r--   0        0        0     2025 2024-04-15 14:32:22.638272 chainlit-1.0.503/chainlit/markdown.py
+-rw-r--r--   0        0        0    17974 2024-04-15 14:32:22.638272 chainlit-1.0.503/chainlit/message.py
+-rw-r--r--   0        0        0    17459 2024-04-15 14:32:22.638272 chainlit-1.0.503/chainlit/oauth_providers.py
+-rw-r--r--   0        0        0     1993 2024-04-15 14:32:22.638272 chainlit-1.0.503/chainlit/openai/__init__.py
+-rw-r--r--   0        0        0       80 2024-04-15 14:32:22.642272 chainlit-1.0.503/chainlit/playground/__init__.py
+-rw-r--r--   0        0        0      948 2024-04-15 14:32:22.642272 chainlit-1.0.503/chainlit/playground/config.py
+-rw-r--r--   0        0        0     3858 2024-04-15 14:32:22.642272 chainlit-1.0.503/chainlit/playground/provider.py
+-rw-r--r--   0        0        0      207 2024-04-15 14:32:22.642272 chainlit-1.0.503/chainlit/playground/providers/__init__.py
+-rw-r--r--   0        0        0     3495 2024-04-15 14:32:22.642272 chainlit-1.0.503/chainlit/playground/providers/anthropic.py
+-rw-r--r--   0        0        0     2130 2024-04-15 14:32:22.642272 chainlit-1.0.503/chainlit/playground/providers/huggingface.py
+-rw-r--r--   0        0        0     3103 2024-04-15 14:32:22.642272 chainlit-1.0.503/chainlit/playground/providers/langchain.py
+-rw-r--r--   0        0        0    11956 2024-04-15 14:32:22.642272 chainlit-1.0.503/chainlit/playground/providers/openai.py
+-rw-r--r--   0        0        0     5084 2024-04-15 14:32:22.642272 chainlit-1.0.503/chainlit/playground/providers/vertexai.py
+-rw-r--r--   0        0        0        0 2024-04-15 14:32:22.642272 chainlit-1.0.503/chainlit/py.typed
+-rw-r--r--   0        0        0      295 2024-04-15 14:32:22.642272 chainlit-1.0.503/chainlit/secret.py
+-rw-r--r--   0        0        0    23716 2024-04-15 14:32:22.642272 chainlit-1.0.503/chainlit/server.py
+-rw-r--r--   0        0        0     8844 2024-04-15 14:32:22.642272 chainlit-1.0.503/chainlit/session.py
+-rw-r--r--   0        0        0     9995 2024-04-15 14:32:22.642272 chainlit-1.0.503/chainlit/socket.py
+-rw-r--r--   0        0        0    13102 2024-04-15 14:32:22.642272 chainlit-1.0.503/chainlit/step.py
+-rw-r--r--   0        0        0     1235 2024-04-15 14:32:22.642272 chainlit-1.0.503/chainlit/sync.py
+-rw-r--r--   0        0        0     3060 2024-04-15 14:32:22.642272 chainlit-1.0.503/chainlit/telemetry.py
+-rw-r--r--   0        0        0     7835 2024-04-15 14:32:22.642272 chainlit-1.0.503/chainlit/translations/en-US.json
+-rw-r--r--   0        0        0     2034 2024-04-15 14:32:22.642272 chainlit-1.0.503/chainlit/translations.py
+-rw-r--r--   0        0        0     4947 2024-04-15 14:32:22.642272 chainlit-1.0.503/chainlit/types.py
+-rw-r--r--   0        0        0      619 2024-04-15 14:32:22.642272 chainlit-1.0.503/chainlit/user.py
+-rw-r--r--   0        0        0     1368 2024-04-15 14:32:22.642272 chainlit-1.0.503/chainlit/user_session.py
+-rw-r--r--   0        0        0     2571 2024-04-15 14:32:22.642272 chainlit-1.0.503/chainlit/utils.py
+-rw-r--r--   0        0        0      196 2024-04-15 14:32:22.642272 chainlit-1.0.503/chainlit/version.py
+-rw-r--r--   0        0        0     2366 2024-04-15 14:32:22.642272 chainlit-1.0.503/pyproject.toml
+-rw-r--r--   0        0        0     5560 1970-01-01 00:00:00.000000 chainlit-1.0.503/PKG-INFO
```

### Comparing `chainlit-1.0.502/README.md` & `chainlit-1.0.503/README.md`

 * *Files identical despite different names*

### Comparing `chainlit-1.0.502/chainlit/__init__.py` & `chainlit-1.0.503/chainlit/__init__.py`

 * *Files identical despite different names*

### Comparing `chainlit-1.0.502/chainlit/action.py` & `chainlit-1.0.503/chainlit/action.py`

 * *Files identical despite different names*

### Comparing `chainlit-1.0.502/chainlit/auth.py` & `chainlit-1.0.503/chainlit/auth.py`

 * *Files identical despite different names*

### Comparing `chainlit-1.0.502/chainlit/cache.py` & `chainlit-1.0.503/chainlit/cache.py`

 * *Files identical despite different names*

### Comparing `chainlit-1.0.502/chainlit/chat_settings.py` & `chainlit-1.0.503/chainlit/chat_settings.py`

 * *Files identical despite different names*

### Comparing `chainlit-1.0.502/chainlit/cli/__init__.py` & `chainlit-1.0.503/chainlit/cli/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,15 +171,15 @@
 
 @cli.command("create-secret")
 @click.argument("args", nargs=-1)
 def chainlit_create_secret(args=None, **kwargs):
     trace_event("chainlit secret")
 
     print(
-        f"Copy the following secret into your .env file. Once it is set, changing it will logout all users with active sessions.\nCHAINLIT_AUTH_SECRET={random_secret()}"
+        f'Copy the following secret into your .env file. Once it is set, changing it will logout all users with active sessions.\nCHAINLIT_AUTH_SECRET="{random_secret()}"'
     )
 
 
 @cli.command("lint-translations")
 @click.argument("args", nargs=-1)
 def chainlit_lint_translations(args=None, **kwargs):
     trace_event("chainlit lint-translation")
```

### Comparing `chainlit-1.0.502/chainlit/cli/utils.py` & `chainlit-1.0.503/chainlit/cli/utils.py`

 * *Files identical despite different names*

### Comparing `chainlit-1.0.502/chainlit/config.py` & `chainlit-1.0.503/chainlit/config.py`

 * *Files identical despite different names*

### Comparing `chainlit-1.0.502/chainlit/context.py` & `chainlit-1.0.503/chainlit/context.py`

 * *Files identical despite different names*

### Comparing `chainlit-1.0.502/chainlit/copilot/dist/assets/logo_dark-2a3cf740.svg` & `chainlit-1.0.503/chainlit/copilot/dist/assets/logo_dark-2a3cf740.svg`

 * *Files identical despite different names*

### Comparing `chainlit-1.0.502/chainlit/copilot/dist/assets/logo_light-b078e7bc.svg` & `chainlit-1.0.503/chainlit/copilot/dist/assets/logo_light-b078e7bc.svg`

 * *Files identical despite different names*

### Comparing `chainlit-1.0.502/chainlit/copilot/dist/index.js` & `chainlit-1.0.503/chainlit/copilot/dist/index.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -18820,14 +18820,15 @@
             m = _t.useCallback(() => {
                 t != null && t.socket && (t.socket.removeAllListeners(), t.socket.close())
             }, [t]);
         return {
             connect: f,
             disconnect: m,
             session: t,
+            sessionId: e,
             chatProfile: x,
             idToResume: l,
             setChatProfile: c
         }
     },
     v9 = "token";
```

### Comparing `chainlit-1.0.502/chainlit/data/__init__.py` & `chainlit-1.0.503/chainlit/data/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import functools
 import json
 import os
 from collections import deque
-from typing import TYPE_CHECKING, Dict, List, Literal, Optional, Union, cast
+from typing import TYPE_CHECKING, Dict, List, Literal, Optional, Union, cast, Protocol, Any
 
 import aiofiles
 from chainlit.config import config
 from chainlit.context import context
 from chainlit.logger import logger
 from chainlit.session import WebsocketSession
-from chainlit.types import Feedback, Pagination, ThreadDict, ThreadFilter
+from chainlit.types import Feedback, Pagination, ThreadDict, ThreadFilter, PageInfo, PaginatedResponse
 from chainlit.user import PersistedUser, User
-from literalai import Attachment, PageInfo, PaginatedResponse, Score as LiteralScore, Step as LiteralStep
+from literalai import Attachment, PaginatedResponse as LiteralPaginatedResponse, Score as LiteralScore, Step as LiteralStep
 from literalai.filter import threads_filters as LiteralThreadsFilters
 from literalai.step import StepDict as LiteralStepDict
 
 if TYPE_CHECKING:
     from chainlit.element import Element, ElementDict
     from chainlit.step import FeedbackDict, StepDict
 
@@ -407,20 +407,28 @@
                     "field": "scoreValue",
                     "operator": "eq",
                     "value": filters.feedback,
                     "path": "user-feedback",
                 }
             )
 
-        return await self.client.api.list_threads(
+        literal_response: LiteralPaginatedResponse = await self.client.api.list_threads(
             first=pagination.first,
             after=pagination.cursor,
             filters=literal_filters,
             order_by={"column": "createdAt", "direction": "DESC"},
         )
+        return PaginatedResponse(
+            pageInfo=PageInfo(
+                hasNextPage=literal_response.pageInfo.hasNextPage,
+                startCursor=literal_response.pageInfo.startCursor,
+                endCursor=literal_response.pageInfo.endCursor
+                ),
+            data=literal_response.data,
+        )
 
     async def get_thread(self, thread_id: str) -> "Optional[ThreadDict]":
         thread = await self.client.api.get_thread(id=thread_id)
         if not thread:
             return None
         elements = []  # List[ElementDict]
         steps = []  # List[StepDict]
@@ -458,14 +466,18 @@
             id=thread_id,
             name=name,
             participant_id=user_id,
             metadata=metadata,
             tags=tags,
         )
 
+class BaseStorageClient(Protocol):
+    """Base class for non-text data persistence like Azure Data Lake, S3, Google Storage, etc."""
+    async def upload_file(self, object_key: str, data: Union[bytes, str], mime: str = 'application/octet-stream', overwrite: bool = True) -> Dict[str, Any]:
+        pass
 
 if api_key := os.environ.get("LITERAL_API_KEY"):
     # support legacy LITERAL_SERVER variable as fallback
     server = os.environ.get("LITERAL_API_URL", os.environ.get("LITERAL_SERVER"))
     _data_layer = ChainlitDataLayer(api_key=api_key, server=server)
```

### Comparing `chainlit-1.0.502/chainlit/element.py` & `chainlit-1.0.503/chainlit/element.py`

 * *Files identical despite different names*

### Comparing `chainlit-1.0.502/chainlit/emitter.py` & `chainlit-1.0.503/chainlit/emitter.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,18 +171,22 @@
     async def flush_thread_queues(self, interaction: str):
         if data_layer := get_data_layer():
             if isinstance(self.session.user, PersistedUser):
                 user_id = self.session.user.id
             else:
                 user_id = None
             try:
+                tags = (
+                    [self.session.chat_profile] if self.session.chat_profile else None
+                )
                 await data_layer.update_thread(
                     thread_id=self.session.thread_id,
                     name=interaction,
                     user_id=user_id,
+                    tags=tags,
                 )
             except Exception as e:
                 logger.error(f"Error updating thread: {e}")
             await self.session.flush_method_queue()
 
     async def init_thread(self, interaction: str):
         await self.flush_thread_queues(interaction)
```

### Comparing `chainlit-1.0.502/chainlit/frontend/dist/assets/index-d088547c.css` & `chainlit-1.0.503/chainlit/frontend/dist/assets/index-d088547c.css`

 * *Files identical despite different names*

### Comparing `chainlit-1.0.502/chainlit/frontend/dist/assets/index-e306c2e5.js` & `chainlit-1.0.503/chainlit/frontend/dist/assets/index-a8e1b559.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -18381,14 +18381,15 @@
             C = A.useCallback(() => {
                 t != null && t.socket && (t.socket.removeAllListeners(), t.socket.close())
             }, [t]);
         return {
             connect: T,
             disconnect: C,
             session: t,
+            sessionId: e,
             chatProfile: _,
             idToResume: S,
             setChatProfile: b
         }
     },
     wk = "token";
 
@@ -46536,15 +46537,15 @@
     },
     Nnt = Ant(Ont),
     Int = async e => {
         const t = await fetch(e);
         if (!t.ok) throw new Error("Network response was not ok");
         const n = t.headers.get("content-type");
         return n && n.includes("application/json") ? t.json() : t.text()
-    }, Yse = e => Nnt(e, Int), wnt = A.lazy(() => Gtt(() => import("./react-plotly-cc656f1c.js").then(e => e.r), [])), Dnt = ({
+    }, Yse = e => Nnt(e, Int), wnt = A.lazy(() => Gtt(() => import("./react-plotly-b225b63c.js").then(e => e.r), [])), Dnt = ({
         element: e
     }) => {
         const {
             data: t,
             error: n,
             isLoading: r
         } = Yse(e.url || null);
```

### Comparing `chainlit-1.0.502/chainlit/frontend/dist/assets/logo_dark-2a3cf740.svg` & `chainlit-1.0.503/chainlit/frontend/dist/assets/logo_dark-2a3cf740.svg`

 * *Files identical despite different names*

### Comparing `chainlit-1.0.502/chainlit/frontend/dist/assets/logo_light-b078e7bc.svg` & `chainlit-1.0.503/chainlit/frontend/dist/assets/logo_light-b078e7bc.svg`

 * *Files identical despite different names*

### Comparing `chainlit-1.0.502/chainlit/frontend/dist/assets/react-plotly-cc656f1c.js` & `chainlit-1.0.503/chainlit/frontend/dist/assets/react-plotly-b225b63c.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,12 +1,12 @@
 import {
     r as Bp,
     p as Np,
     g as Up
-} from "./index-e306c2e5.js";
+} from "./index-a8e1b559.js";
 
 function Vp(Cs, El) {
     for (var $s = 0; $s < El.length; $s++) {
         const di = El[$s];
         if (typeof di != "string" && !Array.isArray(di)) {
             for (const Zi in di)
                 if (Zi !== "default" && !(Zi in Cs)) {
```

### Comparing `chainlit-1.0.502/chainlit/frontend/dist/favicon.svg` & `chainlit-1.0.503/chainlit/frontend/dist/favicon.svg`

 * *Files identical despite different names*

### Comparing `chainlit-1.0.502/chainlit/frontend/dist/index.html` & `chainlit-1.0.503/chainlit/frontend/dist/index.html`

 * *Files 13% similar despite different names*

```diff
@@ -18,15 +18,15 @@
       href="https://cdn.jsdelivr.net/npm/katex@0.16.8/dist/katex.min.css"
     />
     <!-- JS INJECTION PLACEHOLDER -->
     <!-- CSS INJECTION PLACEHOLDER -->
     <script>
       const global = globalThis;
     </script>
-    <script type="module" crossorigin src="/assets/index-e306c2e5.js"></script>
+    <script type="module" crossorigin src="/assets/index-a8e1b559.js"></script>
     <link rel="stylesheet" href="/assets/index-d088547c.css">
   </head>
   <body>
     <div id="root"></div>
     
   </body>
 </html>
```

### Comparing `chainlit-1.0.502/chainlit/haystack/callbacks.py` & `chainlit-1.0.503/chainlit/haystack/callbacks.py`

 * *Files identical despite different names*

### Comparing `chainlit-1.0.502/chainlit/input_widget.py` & `chainlit-1.0.503/chainlit/input_widget.py`

 * *Files identical despite different names*

### Comparing `chainlit-1.0.502/chainlit/langchain/callbacks.py` & `chainlit-1.0.503/chainlit/langchain/callbacks.py`

 * *Files identical despite different names*

### Comparing `chainlit-1.0.502/chainlit/langflow/__init__.py` & `chainlit-1.0.503/chainlit/langflow/__init__.py`

 * *Files identical despite different names*

### Comparing `chainlit-1.0.502/chainlit/llama_index/callbacks.py` & `chainlit-1.0.503/chainlit/llama_index/callbacks.py`

 * *Files identical despite different names*

### Comparing `chainlit-1.0.502/chainlit/markdown.py` & `chainlit-1.0.503/chainlit/markdown.py`

 * *Files identical despite different names*

### Comparing `chainlit-1.0.502/chainlit/message.py` & `chainlit-1.0.503/chainlit/message.py`

 * *Files identical despite different names*

### Comparing `chainlit-1.0.502/chainlit/oauth_providers.py` & `chainlit-1.0.503/chainlit/oauth_providers.py`

 * *Files identical despite different names*

### Comparing `chainlit-1.0.502/chainlit/openai/__init__.py` & `chainlit-1.0.503/chainlit/openai/__init__.py`

 * *Files identical despite different names*

### Comparing `chainlit-1.0.502/chainlit/playground/config.py` & `chainlit-1.0.503/chainlit/playground/config.py`

 * *Files identical despite different names*

### Comparing `chainlit-1.0.502/chainlit/playground/provider.py` & `chainlit-1.0.503/chainlit/playground/provider.py`

 * *Files identical despite different names*

### Comparing `chainlit-1.0.502/chainlit/playground/providers/anthropic.py` & `chainlit-1.0.503/chainlit/playground/providers/anthropic.py`

 * *Files identical despite different names*

### Comparing `chainlit-1.0.502/chainlit/playground/providers/huggingface.py` & `chainlit-1.0.503/chainlit/playground/providers/huggingface.py`

 * *Files identical despite different names*

### Comparing `chainlit-1.0.502/chainlit/playground/providers/langchain.py` & `chainlit-1.0.503/chainlit/playground/providers/langchain.py`

 * *Files identical despite different names*

### Comparing `chainlit-1.0.502/chainlit/playground/providers/openai.py` & `chainlit-1.0.503/chainlit/playground/providers/openai.py`

 * *Files identical despite different names*

### Comparing `chainlit-1.0.502/chainlit/playground/providers/vertexai.py` & `chainlit-1.0.503/chainlit/playground/providers/vertexai.py`

 * *Files identical despite different names*

### Comparing `chainlit-1.0.502/chainlit/server.py` & `chainlit-1.0.503/chainlit/server.py`

 * *Files identical despite different names*

### Comparing `chainlit-1.0.502/chainlit/session.py` & `chainlit-1.0.503/chainlit/session.py`

 * *Files identical despite different names*

### Comparing `chainlit-1.0.502/chainlit/socket.py` & `chainlit-1.0.503/chainlit/socket.py`

 * *Files identical despite different names*

### Comparing `chainlit-1.0.502/chainlit/step.py` & `chainlit-1.0.503/chainlit/step.py`

 * *Files identical despite different names*

### Comparing `chainlit-1.0.502/chainlit/sync.py` & `chainlit-1.0.503/chainlit/sync.py`

 * *Files identical despite different names*

### Comparing `chainlit-1.0.502/chainlit/telemetry.py` & `chainlit-1.0.503/chainlit/telemetry.py`

 * *Files identical despite different names*

### Comparing `chainlit-1.0.502/chainlit/translations/en-US.json` & `chainlit-1.0.503/chainlit/translations/en-US.json`

 * *Files identical despite different names*

### Comparing `chainlit-1.0.502/chainlit/translations.py` & `chainlit-1.0.503/chainlit/translations.py`

 * *Files identical despite different names*

### Comparing `chainlit-1.0.502/chainlit/user.py` & `chainlit-1.0.503/chainlit/user.py`

 * *Files identical despite different names*

### Comparing `chainlit-1.0.502/chainlit/user_session.py` & `chainlit-1.0.503/chainlit/user_session.py`

 * *Files identical despite different names*

### Comparing `chainlit-1.0.502/chainlit/utils.py` & `chainlit-1.0.503/chainlit/utils.py`

 * *Files identical despite different names*

### Comparing `chainlit-1.0.502/pyproject.toml` & `chainlit-1.0.503/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chainlit"
-version = "1.0.502"
+version = "1.0.503"
 keywords = ['LLM', 'Agents', 'gen ai', 'chat ui', 'chatbot ui', 'openai', 'copilot', 'langchain', 'conversational ai']
 description = "Build Conversational AI."
 authors = ["Chainlit"]
 license = "Apache-2.0 license"
 repository = "https://github.com/Chainlit/chainlit"
 readme = "README.md"
 exclude = [
@@ -19,15 +19,15 @@
 [tool.poetry.scripts]
 # command_name = module_for_handler : function_for_handler
 chainlit = 'chainlit.cli:cli'
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0.0"
 httpx = ">=0.23.0"
-literalai = "0.0.500"
+literalai = "0.0.502"
 dataclasses_json = "^0.5.7"
 fastapi = "^0.110.1"
 starlette = "^0.37.2"
 uvicorn = "^0.25.0"
 fastapi-socketio = "^0.0.10"
 aiofiles = "^23.1.0"
 syncer = "^2.0.3"
@@ -88,10 +88,20 @@
     "syncer",
     "vertexai.language_models",
     "vertexai.preview.generative_models",
     "google.cloud"
 ]
 ignore_missing_imports = true
 
+[tool.poetry.group.custom-data]
+optional = true
+
+[tool.poetry.group.custom-data.dependencies]
+asyncpg = "^0.29.0"
+SQLAlchemy = "^2.0.28"
+boto3 = "^1.34.73"
+azure-identity = "^1.14.1"
+azure-storage-file-datalake = "^12.14.0"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `chainlit-1.0.502/PKG-INFO` & `chainlit-1.0.503/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chainlit
-Version: 1.0.502
+Version: 1.0.503
 Summary: Build Conversational AI.
 Home-page: https://github.com/Chainlit/chainlit
 License: Apache-2.0 license
 Keywords: LLM,Agents,gen ai,chat ui,chatbot ui,openai,copilot,langchain,conversational ai
 Author: Chainlit
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: Other/Proprietary License
@@ -18,15 +18,15 @@
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: dataclasses_json (>=0.5.7,<0.6.0)
 Requires-Dist: fastapi (>=0.110.1,<0.111.0)
 Requires-Dist: fastapi-socketio (>=0.0.10,<0.0.11)
 Requires-Dist: filetype (>=1.2.0,<2.0.0)
 Requires-Dist: httpx (>=0.23.0)
 Requires-Dist: lazify (>=0.4.0,<0.5.0)
-Requires-Dist: literalai (==0.0.500)
+Requires-Dist: literalai (==0.0.502)
 Requires-Dist: nest-asyncio (>=1.5.6,<2.0.0)
 Requires-Dist: packaging (>=23.1,<24.0)
 Requires-Dist: pydantic (>=1,<3)
 Requires-Dist: pyjwt (>=2.8.0,<3.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: python-graphql-client (>=0.4.3,<0.5.0)
 Requires-Dist: python-multipart (>=0.0.9,<0.0.10)
```

