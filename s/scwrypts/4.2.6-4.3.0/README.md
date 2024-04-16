# Comparing `tmp/scwrypts-4.2.6.tar.gz` & `tmp/scwrypts-4.3.0.tar.gz`

## Comparing `scwrypts-4.2.6.tar` & `scwrypts-4.3.0.tar`

### file list

```diff
@@ -1,52 +1,53 @@
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 scwrypts-4.2.6/scwrypts/__init__.py
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 scwrypts-4.2.6/scwrypts/env.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 scwrypts-4.2.6/scwrypts/data/__init__.py
--rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 scwrypts-4.2.6/scwrypts/data/converter.py
--rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 scwrypts-4.2.6/scwrypts/data/test_converter.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 scwrypts-4.2.6/scwrypts/fzf/__init__.py
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 scwrypts-4.2.6/scwrypts/fzf/client.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 scwrypts-4.2.6/scwrypts/http/__init__.py
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 scwrypts-4.2.6/scwrypts/http/client.py
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 scwrypts-4.2.6/scwrypts/http/conftest.py
--rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 scwrypts-4.2.6/scwrypts/http/test_client.py
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 scwrypts-4.2.6/scwrypts/http/directus/__init__.py
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 scwrypts-4.2.6/scwrypts/http/directus/client.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 scwrypts-4.2.6/scwrypts/http/directus/collections.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 scwrypts-4.2.6/scwrypts/http/directus/conftest.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 scwrypts-4.2.6/scwrypts/http/directus/fields.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 scwrypts-4.2.6/scwrypts/http/directus/graphql.py
--rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 scwrypts-4.2.6/scwrypts/http/directus/test_client.py
--rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 scwrypts-4.2.6/scwrypts/http/directus/test_graphql.py
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 scwrypts-4.2.6/scwrypts/http/discord/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 scwrypts-4.2.6/scwrypts/http/discord/client.py
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 scwrypts-4.2.6/scwrypts/http/discord/conftest.py
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 scwrypts-4.2.6/scwrypts/http/discord/send_message.py
--rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 scwrypts-4.2.6/scwrypts/http/discord/test_client.py
--rw-r--r--   0        0        0     3499 2020-02-02 00:00:00.000000 scwrypts-4.2.6/scwrypts/http/discord/test_send_message.py
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 scwrypts-4.2.6/scwrypts/http/linear/__init__.py
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 scwrypts-4.2.6/scwrypts/http/linear/client.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 scwrypts-4.2.6/scwrypts/http/linear/conftest.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 scwrypts-4.2.6/scwrypts/http/linear/graphql.py
--rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 scwrypts-4.2.6/scwrypts/http/linear/test_client.py
--rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 scwrypts-4.2.6/scwrypts/http/linear/test_graphql.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 scwrypts-4.2.6/scwrypts/io/__init__.py
--rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 scwrypts-4.2.6/scwrypts/io/combined_io_stream.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 scwrypts-4.2.6/scwrypts/redis/__init__.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 scwrypts-4.2.6/scwrypts/redis/client.py
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 scwrypts-4.2.6/scwrypts/scwrypts/__init__.py
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 scwrypts-4.2.6/scwrypts/scwrypts/exceptions.py
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 scwrypts-4.2.6/scwrypts/scwrypts/execute.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 scwrypts-4.2.6/scwrypts/scwrypts/interactive.py
--rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 scwrypts-4.2.6/scwrypts/scwrypts/scwrypts.py
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 scwrypts-4.2.6/scwrypts/test/__init__.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 scwrypts-4.2.6/scwrypts/test/character_set.py
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 scwrypts-4.2.6/scwrypts/test/exceptions.py
--rw-r--r--   0        0        0    11329 2020-02-02 00:00:00.000000 scwrypts-4.2.6/scwrypts/test/generate.py
--rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 scwrypts-4.2.6/scwrypts/test/test_generate.py
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 scwrypts-4.2.6/scwrypts/twilio/__init__.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 scwrypts-4.2.6/scwrypts/twilio/client.py
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 scwrypts-4.2.6/scwrypts/twilio/send_sms.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 scwrypts-4.2.6/.gitignore
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 scwrypts-4.2.6/README.md
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 scwrypts-4.2.6/pyproject.toml
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 scwrypts-4.2.6/PKG-INFO
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 scwrypts-4.3.0/scwrypts/__init__.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 scwrypts-4.3.0/scwrypts/env.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 scwrypts-4.3.0/scwrypts/data/__init__.py
+-rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 scwrypts-4.3.0/scwrypts/data/converter.py
+-rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 scwrypts-4.3.0/scwrypts/data/test_converter.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 scwrypts-4.3.0/scwrypts/fzf/__init__.py
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 scwrypts-4.3.0/scwrypts/fzf/client.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 scwrypts-4.3.0/scwrypts/http/__init__.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 scwrypts-4.3.0/scwrypts/http/client.py
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 scwrypts-4.3.0/scwrypts/http/conftest.py
+-rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 scwrypts-4.3.0/scwrypts/http/test_client.py
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 scwrypts-4.3.0/scwrypts/http/directus/__init__.py
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 scwrypts-4.3.0/scwrypts/http/directus/client.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 scwrypts-4.3.0/scwrypts/http/directus/collections.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 scwrypts-4.3.0/scwrypts/http/directus/conftest.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 scwrypts-4.3.0/scwrypts/http/directus/fields.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 scwrypts-4.3.0/scwrypts/http/directus/graphql.py
+-rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 scwrypts-4.3.0/scwrypts/http/directus/test_client.py
+-rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 scwrypts-4.3.0/scwrypts/http/directus/test_graphql.py
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 scwrypts-4.3.0/scwrypts/http/discord/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 scwrypts-4.3.0/scwrypts/http/discord/client.py
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 scwrypts-4.3.0/scwrypts/http/discord/conftest.py
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 scwrypts-4.3.0/scwrypts/http/discord/send_message.py
+-rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 scwrypts-4.3.0/scwrypts/http/discord/test_client.py
+-rw-r--r--   0        0        0     3499 2020-02-02 00:00:00.000000 scwrypts-4.3.0/scwrypts/http/discord/test_send_message.py
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 scwrypts-4.3.0/scwrypts/http/linear/__init__.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 scwrypts-4.3.0/scwrypts/http/linear/client.py
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 scwrypts-4.3.0/scwrypts/http/linear/conftest.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 scwrypts-4.3.0/scwrypts/http/linear/graphql.py
+-rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 scwrypts-4.3.0/scwrypts/http/linear/test_client.py
+-rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 scwrypts-4.3.0/scwrypts/http/linear/test_graphql.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 scwrypts-4.3.0/scwrypts/io/__init__.py
+-rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 scwrypts-4.3.0/scwrypts/io/combined_io_stream.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 scwrypts-4.3.0/scwrypts/redis/__init__.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 scwrypts-4.3.0/scwrypts/redis/client.py
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 scwrypts-4.3.0/scwrypts/scwrypts/__init__.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 scwrypts-4.3.0/scwrypts/scwrypts/exceptions.py
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 scwrypts-4.3.0/scwrypts/scwrypts/execute.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 scwrypts-4.3.0/scwrypts/scwrypts/interactive.py
+-rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 scwrypts-4.3.0/scwrypts/scwrypts/scwrypts.py
+-rw-r--r--   0        0        0     6217 2020-02-02 00:00:00.000000 scwrypts-4.3.0/scwrypts/scwrypts/test_scwrypts.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 scwrypts-4.3.0/scwrypts/test/__init__.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 scwrypts-4.3.0/scwrypts/test/character_set.py
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 scwrypts-4.3.0/scwrypts/test/exceptions.py
+-rw-r--r--   0        0        0    11751 2020-02-02 00:00:00.000000 scwrypts-4.3.0/scwrypts/test/generate.py
+-rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 scwrypts-4.3.0/scwrypts/test/test_generate.py
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 scwrypts-4.3.0/scwrypts/twilio/__init__.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 scwrypts-4.3.0/scwrypts/twilio/client.py
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 scwrypts-4.3.0/scwrypts/twilio/send_sms.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 scwrypts-4.3.0/.gitignore
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 scwrypts-4.3.0/README.md
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 scwrypts-4.3.0/pyproject.toml
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 scwrypts-4.3.0/PKG-INFO
```

### Comparing `scwrypts-4.2.6/scwrypts/data/converter.py` & `scwrypts-4.3.0/scwrypts/data/converter.py`

 * *Files identical despite different names*

### Comparing `scwrypts-4.2.6/scwrypts/data/test_converter.py` & `scwrypts-4.3.0/scwrypts/data/test_converter.py`

 * *Files identical despite different names*

### Comparing `scwrypts-4.2.6/scwrypts/fzf/client.py` & `scwrypts-4.3.0/scwrypts/fzf/client.py`

 * *Files identical despite different names*

### Comparing `scwrypts-4.2.6/scwrypts/http/client.py` & `scwrypts-4.3.0/scwrypts/http/client.py`

 * *Files identical despite different names*

### Comparing `scwrypts-4.2.6/scwrypts/http/conftest.py` & `scwrypts-4.3.0/scwrypts/http/conftest.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,40 @@
 from types import SimpleNamespace
 
 from pytest import fixture
 
-from scwrypts.test import generate
+from scwrypts.test import get_generator
 from scwrypts.test.character_set import uri
 
-options = {
+generate = get_generator({
         'str_length_minimum':   8,
         'str_length_maximum': 128,
         'uuid_output_type':   str,
-        }
+        })
 
 def get_request_client_sample_data():
     return {
-            'base_url' : generate(str, options | {'character_set': uri}),
-            'endpoint' : generate(str, options | {'character_set': uri}),
-            'method'   : generate(str, options),
-            'response' : generate('requests_Response', options | {'depth': 4}),
+            'base_url' : generate(str, {'character_set': uri}),
+            'endpoint' : generate(str, {'character_set': uri}),
+            'method'   : generate(str),
+            'response' : generate('requests_Response', {'depth': 4}),
             'payload'  : generate(dict, {
-                **options,
                 'depth': 1,
                 'data_types': { str, 'uuid' },
                 }),
             }
 
 @fixture(name='sample')
 def fixture_sample():
     return SimpleNamespace(
             **get_request_client_sample_data(),
 
             headers = generate(dict, {
-                **options,
                 'depth': 1,
                 'data_types': { str, 'uuid' },
                 }),
 
             payload_headers = generate(dict, {
-                **options,
                 'depth': 1,
                 'data_types': { str, 'uuid' },
                 }),
             )
```

### Comparing `scwrypts-4.2.6/scwrypts/http/test_client.py` & `scwrypts-4.3.0/scwrypts/http/test_client.py`

 * *Files identical despite different names*

### Comparing `scwrypts-4.2.6/scwrypts/http/directus/__init__.py` & `scwrypts-4.3.0/scwrypts/http/directus/__init__.py`

 * *Files identical despite different names*

### Comparing `scwrypts-4.2.6/scwrypts/http/directus/test_client.py` & `scwrypts-4.3.0/scwrypts/http/directus/test_client.py`

 * *Files identical despite different names*

### Comparing `scwrypts-4.2.6/scwrypts/http/directus/test_graphql.py` & `scwrypts-4.3.0/scwrypts/http/directus/test_graphql.py`

 * *Files identical despite different names*

### Comparing `scwrypts-4.2.6/scwrypts/http/discord/conftest.py` & `scwrypts-4.3.0/scwrypts/http/discord/conftest.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 from string import ascii_letters, digits
 from types import SimpleNamespace
 
 from pytest import fixture
 
-from scwrypts.test import generate
 from scwrypts.test.character_set import uri
-from ..conftest import options, get_request_client_sample_data
+from ..conftest import generate, get_request_client_sample_data
 
 @fixture(name='sample')
 def fixture_sample():
     return SimpleNamespace(
             **{
                 **get_request_client_sample_data(),
                 'base_url': 'https://discord.com/api',
                 },
-            bot_token  = generate(str, options | {'character_set': uri}),
-            username   = generate(str, options | {'character_set': ascii_letters + digits}),
-            avatar_url = generate(str, options | {'character_set': uri}),
-            webhook    = generate(str, options | {'character_set': uri}),
-            channel_id = generate(str, options | {'character_set': uri}),
-            content_header = generate(str, options),
-            content_footer = generate(str, options),
-            content = generate(str, options),
+            bot_token  = generate(str, {'character_set': uri}),
+            username   = generate(str, {'character_set': ascii_letters + digits}),
+            avatar_url = generate(str, {'character_set': uri}),
+            webhook    = generate(str, {'character_set': uri}),
+            channel_id = generate(str, {'character_set': uri}),
+            content_header = generate(str),
+            content_footer = generate(str),
+            content = generate(str),
         )
```

### Comparing `scwrypts-4.2.6/scwrypts/http/discord/send_message.py` & `scwrypts-4.3.0/scwrypts/http/discord/send_message.py`

 * *Files identical despite different names*

### Comparing `scwrypts-4.2.6/scwrypts/http/discord/test_client.py` & `scwrypts-4.3.0/scwrypts/http/discord/test_client.py`

 * *Files identical despite different names*

### Comparing `scwrypts-4.2.6/scwrypts/http/discord/test_send_message.py` & `scwrypts-4.3.0/scwrypts/http/discord/test_send_message.py`

 * *Files identical despite different names*

### Comparing `scwrypts-4.2.6/scwrypts/http/linear/conftest.py` & `scwrypts-4.3.0/scwrypts/http/linear/conftest.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from string import ascii_letters, digits
 from types import SimpleNamespace
 
 from pytest import fixture
 
-from scwrypts.test import generate
 from scwrypts.test.character_set import uri
-from ..conftest import options, get_request_client_sample_data
+from ..conftest import generate, get_request_client_sample_data
 
 @fixture(name='sample')
 def fixture_sample():
     return SimpleNamespace(
             **{
                 **get_request_client_sample_data(),
                 'base_url': 'https://api.linear.app',
                 },
-            api_token = generate(str, options | {'character_set': uri}),
-            query     = generate(str, options),
+            api_token = generate(str, {'character_set': uri}),
+            query     = generate(str),
         )
```

### Comparing `scwrypts-4.2.6/scwrypts/http/linear/test_client.py` & `scwrypts-4.3.0/scwrypts/http/linear/test_client.py`

 * *Files identical despite different names*

### Comparing `scwrypts-4.2.6/scwrypts/http/linear/test_graphql.py` & `scwrypts-4.3.0/scwrypts/http/linear/test_graphql.py`

 * *Files identical despite different names*

### Comparing `scwrypts-4.2.6/scwrypts/io/combined_io_stream.py` & `scwrypts-4.3.0/scwrypts/io/combined_io_stream.py`

 * *Files identical despite different names*

### Comparing `scwrypts-4.2.6/scwrypts/scwrypts/__init__.py` & `scwrypts-4.3.0/scwrypts/scwrypts/__init__.py`

 * *Files identical despite different names*

### Comparing `scwrypts-4.2.6/scwrypts/scwrypts/exceptions.py` & `scwrypts-4.3.0/scwrypts/scwrypts/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 class MissingFlagAndEnvironmentVariableError(EnvironmentError, ArgumentError):
     def __init__(self, flags, env_var):
         super().__init__(f'must provide at least one of : {{ flags: {flags} OR {env_var} }}')
 
 
 class MissingScwryptsExecutableError(EnvironmentError):
     def __init__(self):
-        super().__init__(f'scwrypts must be installed and available on your PATH')
+        super().__init__('scwrypts must be installed and available on your PATH')
 
 
 class BadScwryptsLookupError(ValueError):
     def __init__(self):
         super().__init__('must provide name/group/type or scwrypt lookup patterns')
```

### Comparing `scwrypts-4.2.6/scwrypts/scwrypts/execute.py` & `scwrypts-4.3.0/scwrypts/scwrypts/execute.py`

 * *Files identical despite different names*

### Comparing `scwrypts-4.2.6/scwrypts/scwrypts/interactive.py` & `scwrypts-4.3.0/scwrypts/scwrypts/interactive.py`

 * *Files identical despite different names*

### Comparing `scwrypts-4.2.6/scwrypts/test/generate.py` & `scwrypts-4.3.0/scwrypts/test/generate.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,14 +41,29 @@
         'yaml_initial_type': dict,  # typically dict or list
         'yaml_bool_nullable': True,
         'yaml_use_default_flow_style': False,
         'yaml_output_type': 'stringio',  # str or 'stringio'
         'requests_response_status_code': status_codes.codes[200],
         }
 
+def get_generator(default_options=None):
+    if default_options is None:
+        default_options = {}
+
+    def generator_function(data_type=None, options_overrides=None):
+        if options_overrides is None:
+            options_overrides = {}
+
+        return generate(
+                data_type = data_type,
+                options = default_options | options_overrides,
+                )
+
+    return generator_function
+
 def generate(data_type=None, options=None):
     '''
     generate random data with the call of a function
         use data_type to generate a single value
 
         use options to set generation options (key = type, value = kwargs)
```

### Comparing `scwrypts-4.2.6/scwrypts/test/test_generate.py` & `scwrypts-4.3.0/scwrypts/test/test_generate.py`

 * *Files identical despite different names*

### Comparing `scwrypts-4.2.6/scwrypts/twilio/send_sms.py` & `scwrypts-4.3.0/scwrypts/twilio/send_sms.py`

 * *Files identical despite different names*

### Comparing `scwrypts-4.2.6/pyproject.toml` & `scwrypts-4.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scwrypts-4.2.6/PKG-INFO` & `scwrypts-4.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: scwrypts
-Version: 4.2.6
+Version: 4.3.0
 Summary: scwrypts library and invoker
 Project-URL: homepage, https://github.com/wrynegade/scwrypts
 Project-URL: issues, https://github.com/wrynegade/scwrypts/issues
 Author-email: yage <yage@yage.io>
 License-Expression: GPL-3.0-or-later
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
```

