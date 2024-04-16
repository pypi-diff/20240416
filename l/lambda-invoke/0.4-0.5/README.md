# Comparing `tmp/lambda-invoke-0.4.tar.gz` & `tmp/lambda_invoke-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lambda-invoke-0.4.tar", last modified: Wed Apr 12 03:35:06 2023, max compression
+gzip compressed data, was "lambda_invoke-0.5.tar", last modified: Tue Apr 16 15:37:28 2024, max compression
```

## Comparing `lambda-invoke-0.4.tar` & `lambda_invoke-0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 03:35:06.289003 lambda-invoke-0.4/
--rw-r--r--   0 root         (0) root         (0)      156 2023-04-12 03:35:00.000000 lambda-invoke-0.4/AUTHORS.rst
--rw-r--r--   0 root         (0) root         (0)     1073 2023-04-12 03:35:00.000000 lambda-invoke-0.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1094 2023-04-12 03:35:06.289003 lambda-invoke-0.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      471 2023-04-12 03:35:00.000000 lambda-invoke-0.4/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 03:35:06.289003 lambda-invoke-0.4/lambda_invoke/
--rw-r--r--   0 root         (0) root         (0)       70 2023-04-12 03:35:00.000000 lambda-invoke-0.4/lambda_invoke/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4317 2023-04-12 03:35:00.000000 lambda-invoke-0.4/lambda_invoke/simple_proxy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 03:35:06.289003 lambda-invoke-0.4/lambda_invoke.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1094 2023-04-12 03:35:06.000000 lambda-invoke-0.4/lambda_invoke.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      358 2023-04-12 03:35:06.000000 lambda-invoke-0.4/lambda_invoke.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 03:35:06.000000 lambda-invoke-0.4/lambda_invoke.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 03:35:06.000000 lambda-invoke-0.4/lambda_invoke.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       99 2023-04-12 03:35:06.000000 lambda-invoke-0.4/lambda_invoke.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-04-12 03:35:06.000000 lambda-invoke-0.4/lambda_invoke.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       90 2023-04-12 03:35:00.000000 lambda-invoke-0.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1014 2023-04-12 03:35:06.293003 lambda-invoke-0.4/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 03:35:06.289003 lambda-invoke-0.4/tests/
--rw-r--r--   0 root         (0) root         (0)     5545 2023-04-12 03:35:00.000000 lambda-invoke-0.4/tests/test_simple_proxy.py
+drwxr-xr-x   0 tox       (1000) tox       (1000)        0 2024-04-16 15:37:28.534296 lambda_invoke-0.5/
+-rw-r--r--   0 tox       (1000) tox       (1000)      156 2021-12-13 02:14:12.000000 lambda_invoke-0.5/AUTHORS.rst
+-rw-r--r--   0 tox       (1000) tox       (1000)     1073 2021-12-13 02:31:40.000000 lambda_invoke-0.5/LICENSE
+-rw-r--r--   0 tox       (1000) tox       (1000)     1637 2024-04-16 15:37:28.534296 lambda_invoke-0.5/PKG-INFO
+-rw-r--r--   0 tox       (1000) tox       (1000)      471 2021-12-14 03:30:11.000000 lambda_invoke-0.5/README.rst
+drwxr-xr-x   0 tox       (1000) tox       (1000)        0 2024-04-16 15:37:28.534296 lambda_invoke-0.5/lambda_invoke/
+-rw-r--r--   0 tox       (1000) tox       (1000)       70 2021-12-14 03:40:14.000000 lambda_invoke-0.5/lambda_invoke/__init__.py
+-rw-r--r--   0 tox       (1000) tox       (1000)     4687 2024-04-16 15:23:10.000000 lambda_invoke-0.5/lambda_invoke/simple_proxy.py
+drwxr-xr-x   0 tox       (1000) tox       (1000)        0 2024-04-16 15:37:28.534296 lambda_invoke-0.5/lambda_invoke.egg-info/
+-rw-r--r--   0 tox       (1000) tox       (1000)     1637 2024-04-16 15:37:28.000000 lambda_invoke-0.5/lambda_invoke.egg-info/PKG-INFO
+-rw-r--r--   0 tox       (1000) tox       (1000)      358 2024-04-16 15:37:28.000000 lambda_invoke-0.5/lambda_invoke.egg-info/SOURCES.txt
+-rw-r--r--   0 tox       (1000) tox       (1000)        1 2024-04-16 15:37:28.000000 lambda_invoke-0.5/lambda_invoke.egg-info/dependency_links.txt
+-rw-r--r--   0 tox       (1000) tox       (1000)        1 2024-04-16 15:27:37.000000 lambda_invoke-0.5/lambda_invoke.egg-info/not-zip-safe
+-rw-r--r--   0 tox       (1000) tox       (1000)       99 2024-04-16 15:37:28.000000 lambda_invoke-0.5/lambda_invoke.egg-info/requires.txt
+-rw-r--r--   0 tox       (1000) tox       (1000)       14 2024-04-16 15:37:28.000000 lambda_invoke-0.5/lambda_invoke.egg-info/top_level.txt
+-rw-r--r--   0 tox       (1000) tox       (1000)       90 2021-12-13 02:27:07.000000 lambda_invoke-0.5/pyproject.toml
+-rw-r--r--   0 tox       (1000) tox       (1000)     1014 2024-04-16 15:37:28.534296 lambda_invoke-0.5/setup.cfg
+drwxr-xr-x   0 tox       (1000) tox       (1000)        0 2024-04-16 15:37:28.534296 lambda_invoke-0.5/tests/
+-rw-r--r--   0 tox       (1000) tox       (1000)     7154 2024-04-16 15:23:10.000000 lambda_invoke-0.5/tests/test_simple_proxy.py
```

### Comparing `lambda-invoke-0.4/LICENSE` & `lambda_invoke-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lambda-invoke-0.4/lambda_invoke/simple_proxy.py` & `lambda_invoke-0.5/lambda_invoke/simple_proxy.py`

 * *Files 10% similar despite different names*

```diff
@@ -70,15 +70,29 @@
         host_parts = self.url.hostname.split(".")
         if len(host_parts) > 1:
             return f"{host_parts[-1]}:{host_parts[-2]}"
         return host_parts[0]
 
     @property
     def request_query_string(self):
-        return {key: value[0] for key, value in parse_qs(self.url.query).items()}
+        qs = {
+            "queryStringParameters": {
+                key: value[0]
+                for key, value in parse_qs(self.url.query).items()
+                if len(value) == 1
+            }
+        }
+        multi_value_qs = {
+            key: value
+            for key, value in parse_qs(self.url.query).items()
+            if len(value) > 1
+        }
+        if multi_value_qs:
+            qs["multiValueQueryStringParameters"] = multi_value_qs
+        return qs
 
     @property
     def request_body(self):
         if not self.body:
             return False, None
         try:
             if isinstance(self.body, str):
@@ -96,19 +110,19 @@
         """
         base64_encoded, body = self.request_body
         return {
             "resource": self.url.path,
             "httpMethod": self.method,
             "path": self.url.path,
             "pathParameters": "",
-            "queryStringParameters": self.request_query_string,
             "headers": self.headers,
             "body": body,
             "isBase64Encoded": base64_encoded,
             "requestContext": {},
+            **self.request_query_string,
         }
 
     @property
     def request_payload_json(self):
         return json.dumps(self.request_payload, cls=_JSONEncoder)
 
     @property
```

### Comparing `lambda-invoke-0.4/setup.cfg` & `lambda_invoke-0.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = lambda-invoke
-version = 0.4
+version = 0.5
 author = Ilya Sukhanov
 author_email = ilya@sukhanov.net
 license = MIT license
 description = Conveniently invoke lambda mimicking a proxy invocation
 keywords = 
 	aws
 	lambda-invoke
```

### Comparing `lambda-invoke-0.4/tests/test_simple_proxy.py` & `lambda_invoke-0.5/tests/test_simple_proxy.py`

 * *Files 22% similar despite different names*

```diff
@@ -103,14 +103,54 @@
         assert response.status_code == 200
 
     def test_json_serialize_fallthrough(self):
         json.dumps({"foo": "bar"}, cls=_JSONEncoder)
         with self.assertRaises(TypeError):
             json.dumps({"foo": datetime.fromisoformat("2021-06-19")}, cls=_JSONEncoder)
 
+    def test_query_string(self):
+        proxy = LambdaSimpleProxy(
+            "us-east-1", "get", "http://example/?a=1&b=2", {}, None
+        )
+        response = proxy.send(self.mock_client)
+        assert response.status_code == 200
+        sent_payload = json.loads(
+            self.mock_client.invoke.call_args.kwargs.get("Payload")
+        )
+        assert sent_payload.get("queryStringParameters") == {"a": "1", "b": "2"}
+        assert "multiValueQueryStringParameters" not in sent_payload.keys()
+
+    def test_mix_multi_value_query_string(self):
+        proxy = LambdaSimpleProxy(
+            "us-east-1", "get", "http://example/?a=1&b=2&a=bob", {}, None
+        )
+        response = proxy.send(self.mock_client)
+        assert response.status_code == 200
+        sent_payload = json.loads(
+            self.mock_client.invoke.call_args.kwargs.get("Payload")
+        )
+        assert sent_payload.get("queryStringParameters") == {"b": "2"}
+        assert sent_payload.get("multiValueQueryStringParameters") == {
+            "a": ["1", "bob"]
+        }
+
+    def test_only_multi_value_query_string(self):
+        proxy = LambdaSimpleProxy(
+            "us-east-1", "get", "http://example/?a=1&a=bob", {}, None
+        )
+        response = proxy.send(self.mock_client)
+        assert response.status_code == 200
+        sent_payload = json.loads(
+            self.mock_client.invoke.call_args.kwargs.get("Payload")
+        )
+        assert sent_payload.get("queryStringParameters") == {}
+        assert sent_payload.get("multiValueQueryStringParameters") == {
+            "a": ["1", "bob"]
+        }
+
 
 class TestSimpleProxyAsync(IsolatedAsyncioTestCase):
     async def test_200_ok_async(self):
         proxy = LambdaSimpleProxy("us-east-1", "get", "http://example/", {}, None)
         mock_client = MagicMock()
         mock_invoke_result = MagicMock()
         mock_client.invoke = AsyncMock(side_effect=mock_invoke_result)
```

