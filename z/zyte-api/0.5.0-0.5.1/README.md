# Comparing `tmp/zyte-api-0.5.0.tar.gz` & `tmp/zyte_api-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zyte-api-0.5.0.tar", last modified: Fri Apr  5 12:41:02 2024, max compression
+gzip compressed data, was "zyte_api-0.5.1.tar", last modified: Tue Apr 16 08:02:00 2024, max compression
```

## Comparing `zyte-api-0.5.0.tar` & `zyte_api-0.5.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:41:02.167657 zyte-api-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-04-05 12:40:37.000000 zyte-api-0.5.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-05 12:40:37.000000 zyte-api-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-05 12:40:37.000000 zyte-api-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3554 2024-04-05 12:41:02.167657 zyte-api-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-04-05 12:40:37.000000 zyte-api-0.5.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-05 12:40:37.000000 zyte-api-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-05 12:41:02.167657 zyte-api-0.5.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1439 2024-04-05 12:40:37.000000 zyte-api-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:41:02.163657 zyte-api-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 12:40:37.000000 zyte-api-0.5.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-05 12:40:37.000000 zyte-api-0.5.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6219 2024-04-05 12:40:37.000000 zyte-api-0.5.0/tests/mockserver.py
--rw-r--r--   0 runner    (1001) docker     (127)    13251 2024-04-05 12:40:37.000000 zyte-api-0.5.0/tests/test_async.py
--rw-r--r--   0 runner    (1001) docker     (127)     8190 2024-04-05 12:40:37.000000 zyte-api-0.5.0/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-05 12:40:37.000000 zyte-api-0.5.0/tests/test_retry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-04-05 12:40:37.000000 zyte-api-0.5.0/tests/test_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-04-05 12:40:37.000000 zyte-api-0.5.0/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:41:02.167657 zyte-api-0.5.0/zyte_api/
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-05 12:40:37.000000 zyte-api-0.5.0/zyte_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6770 2024-04-05 12:40:37.000000 zyte-api-0.5.0/zyte_api/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-05 12:40:37.000000 zyte-api-0.5.0/zyte_api/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6473 2024-04-05 12:40:37.000000 zyte-api-0.5.0/zyte_api/_async.py
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-05 12:40:37.000000 zyte-api-0.5.0/zyte_api/_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     6227 2024-04-05 12:40:37.000000 zyte-api-0.5.0/zyte_api/_retry.py
--rw-r--r--   0 runner    (1001) docker     (127)     6771 2024-04-05 12:40:37.000000 zyte-api-0.5.0/zyte_api/_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-05 12:40:37.000000 zyte-api-0.5.0/zyte_api/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:41:02.167657 zyte-api-0.5.0/zyte_api/aio/
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-05 12:40:37.000000 zyte-api-0.5.0/zyte_api/aio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-05 12:40:37.000000 zyte-api-0.5.0/zyte_api/aio/client.py
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-05 12:40:37.000000 zyte-api-0.5.0/zyte_api/aio/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-05 12:40:37.000000 zyte-api-0.5.0/zyte_api/aio/retry.py
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-05 12:40:37.000000 zyte-api-0.5.0/zyte_api/apikey.py
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-05 12:40:37.000000 zyte-api-0.5.0/zyte_api/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-04-05 12:40:37.000000 zyte-api-0.5.0/zyte_api/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5389 2024-04-05 12:40:37.000000 zyte-api-0.5.0/zyte_api/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-05 12:40:37.000000 zyte-api-0.5.0/zyte_api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:41:02.167657 zyte-api-0.5.0/zyte_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3554 2024-04-05 12:41:02.000000 zyte-api-0.5.0/zyte_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-05 12:41:02.000000 zyte-api-0.5.0/zyte_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 12:41:02.000000 zyte-api-0.5.0/zyte_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-05 12:41:02.000000 zyte-api-0.5.0/zyte_api.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-05 12:41:02.000000 zyte-api-0.5.0/zyte_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-05 12:41:02.000000 zyte-api-0.5.0/zyte_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:02:00.428574 zyte_api-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-04-16 08:01:49.000000 zyte_api-0.5.1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-16 08:01:49.000000 zyte_api-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-16 08:01:49.000000 zyte_api-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3554 2024-04-16 08:02:00.428574 zyte_api-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-04-16 08:01:49.000000 zyte_api-0.5.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-16 08:01:49.000000 zyte_api-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-16 08:02:00.428574 zyte_api-0.5.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1439 2024-04-16 08:01:49.000000 zyte_api-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:02:00.424574 zyte_api-0.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 08:01:49.000000 zyte_api-0.5.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-16 08:01:49.000000 zyte_api-0.5.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6219 2024-04-16 08:01:49.000000 zyte_api-0.5.1/tests/mockserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14966 2024-04-16 08:01:49.000000 zyte_api-0.5.1/tests/test_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8190 2024-04-16 08:01:49.000000 zyte_api-0.5.1/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-16 08:01:49.000000 zyte_api-0.5.1/tests/test_retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5442 2024-04-16 08:01:49.000000 zyte_api-0.5.1/tests/test_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-04-16 08:01:49.000000 zyte_api-0.5.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:02:00.424574 zyte_api-0.5.1/zyte_api/
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-16 08:01:49.000000 zyte_api-0.5.1/zyte_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6770 2024-04-16 08:01:49.000000 zyte_api-0.5.1/zyte_api/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-16 08:01:49.000000 zyte_api-0.5.1/zyte_api/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6516 2024-04-16 08:01:49.000000 zyte_api-0.5.1/zyte_api/_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-16 08:01:49.000000 zyte_api-0.5.1/zyte_api/_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6227 2024-04-16 08:01:49.000000 zyte_api-0.5.1/zyte_api/_retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6838 2024-04-16 08:01:49.000000 zyte_api-0.5.1/zyte_api/_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-16 08:01:49.000000 zyte_api-0.5.1/zyte_api/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:02:00.428574 zyte_api-0.5.1/zyte_api/aio/
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-16 08:01:49.000000 zyte_api-0.5.1/zyte_api/aio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-16 08:01:49.000000 zyte_api-0.5.1/zyte_api/aio/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-16 08:01:49.000000 zyte_api-0.5.1/zyte_api/aio/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-16 08:01:49.000000 zyte_api-0.5.1/zyte_api/aio/retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-16 08:01:49.000000 zyte_api-0.5.1/zyte_api/apikey.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-16 08:01:49.000000 zyte_api-0.5.1/zyte_api/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-04-16 08:01:49.000000 zyte_api-0.5.1/zyte_api/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5389 2024-04-16 08:01:49.000000 zyte_api-0.5.1/zyte_api/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-16 08:01:49.000000 zyte_api-0.5.1/zyte_api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:02:00.428574 zyte_api-0.5.1/zyte_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3554 2024-04-16 08:02:00.000000 zyte_api-0.5.1/zyte_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-16 08:02:00.000000 zyte_api-0.5.1/zyte_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 08:02:00.000000 zyte_api-0.5.1/zyte_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-16 08:02:00.000000 zyte_api-0.5.1/zyte_api.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-16 08:02:00.000000 zyte_api-0.5.1/zyte_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-16 08:02:00.000000 zyte_api-0.5.1/zyte_api.egg-info/top_level.txt
```

### Comparing `zyte-api-0.5.0/CHANGES.rst` & `zyte_api-0.5.1/CHANGES.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 Changes
 =======
 
+0.5.1 (2024-04-16)
+------------------
+
+* :class:`~zyte_api.ZyteAPI` and :class:`~zyte_api.AsyncZyteAPI` sessions no
+  longer need to be used as context managers, and can instead be closed with a
+  ``close()`` method.
+
 0.5.0 (2024-04-05)
 ------------------
 
 * Removed Python 3.7 support.
 
 * Added :class:`~zyte_api.ZyteAPI` and :class:`~zyte_api.AsyncZyteAPI` to
   provide both sync and async Python interfaces with a cleaner API.
```

### Comparing `zyte-api-0.5.0/LICENSE` & `zyte_api-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zyte-api-0.5.0/PKG-INFO` & `zyte_api-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zyte-api
-Version: 0.5.0
+Version: 0.5.1
 Summary: Python interface to Zyte API
 Home-page: https://github.com/zytedata/python-zyte-api
 Author: Zyte Group Ltd
 Author-email: opensource@zyte.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `zyte-api-0.5.0/README.rst` & `zyte_api-0.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `zyte-api-0.5.0/setup.py` & `zyte_api-0.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `zyte-api-0.5.0/tests/mockserver.py` & `zyte_api-0.5.1/tests/mockserver.py`

 * *Files identical despite different names*

### Comparing `zyte-api-0.5.0/tests/test_async.py` & `zyte_api-0.5.1/tests/test_async.py`

 * *Files 4% similar despite different names*

```diff
@@ -384,15 +384,15 @@
     for future in asyncio.as_completed(futures):
         await future
     assert client._semaphore.__aenter__.call_count == len(queries)
     assert client._semaphore.__aexit__.call_count == len(queries)
 
 
 @pytest.mark.asyncio
-async def test_session(mockserver):
+async def test_session_context_manager(mockserver):
     client = AsyncZyteAPI(api_key="a", api_url=mockserver.urljoin("/"))
     queries = [
         {"url": "https://a.example", "httpResponseBody": True},
         {"url": "https://exception.example", "httpResponseBody": True},
         {"url": "https://b.example", "httpResponseBody": True},
     ]
     expected_results = [
@@ -404,32 +404,81 @@
         {
             "url": "https://b.example",
             "httpResponseBody": "PGh0bWw+PGJvZHk+SGVsbG88aDE+V29ybGQhPC9oMT48L2JvZHk+PC9odG1sPg==",
         },
     ]
     actual_results = []
     async with client.session() as session:
-        assert session._context.connector.limit == client.n_conn
+        assert session._session.connector.limit == client.n_conn
         actual_results.append(await session.get(queries[0]))
         for future in session.iter(queries[1:]):
             try:
                 result = await future
             except Exception as e:
                 result = e
             actual_results.append(result)
-        aiohttp_session = session._context
+        aiohttp_session = session._session
         assert not aiohttp_session.closed
     assert aiohttp_session.closed
-    assert session._context is None
 
     with pytest.raises(RuntimeError):
         await session.get(queries[0])
 
     with pytest.raises(RuntimeError):
-        session.iter(queries[1:])
+        future = next(iter(session.iter(queries[1:])))
+        await future
+
+    assert len(actual_results) == len(expected_results)
+    for actual_result in actual_results:
+        if isinstance(actual_result, Exception):
+            assert Exception in expected_results
+        else:
+            assert actual_result in expected_results
+
+
+@pytest.mark.asyncio
+async def test_session_no_context_manager(mockserver):
+    client = AsyncZyteAPI(api_key="a", api_url=mockserver.urljoin("/"))
+    queries = [
+        {"url": "https://a.example", "httpResponseBody": True},
+        {"url": "https://exception.example", "httpResponseBody": True},
+        {"url": "https://b.example", "httpResponseBody": True},
+    ]
+    expected_results = [
+        {
+            "url": "https://a.example",
+            "httpResponseBody": "PGh0bWw+PGJvZHk+SGVsbG88aDE+V29ybGQhPC9oMT48L2JvZHk+PC9odG1sPg==",
+        },
+        Exception,
+        {
+            "url": "https://b.example",
+            "httpResponseBody": "PGh0bWw+PGJvZHk+SGVsbG88aDE+V29ybGQhPC9oMT48L2JvZHk+PC9odG1sPg==",
+        },
+    ]
+    actual_results = []
+    session = client.session()
+    assert session._session.connector.limit == client.n_conn
+    actual_results.append(await session.get(queries[0]))
+    for future in session.iter(queries[1:]):
+        try:
+            result = await future
+        except Exception as e:
+            result = e
+        actual_results.append(result)
+    aiohttp_session = session._session
+    assert not aiohttp_session.closed
+    await session.close()
+    assert aiohttp_session.closed
+
+    with pytest.raises(RuntimeError):
+        await session.get(queries[0])
+
+    with pytest.raises(RuntimeError):
+        future = next(iter(session.iter(queries[1:])))
+        await future
 
     assert len(actual_results) == len(expected_results)
     for actual_result in actual_results:
         if isinstance(actual_result, Exception):
             assert Exception in expected_results
         else:
             assert actual_result in expected_results
```

### Comparing `zyte-api-0.5.0/tests/test_main.py` & `zyte_api-0.5.1/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `zyte-api-0.5.0/tests/test_sync.py` & `zyte_api-0.5.1/tests/test_sync.py`

 * *Files 14% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     client.get(queries[0])
     next(iter(client.iter(queries[1:2])))
     client.get(queries[2])
     assert client._async_client._semaphore.__aenter__.call_count == len(queries)
     assert client._async_client._semaphore.__aexit__.call_count == len(queries)
 
 
-def test_session(mockserver):
+def test_session_context_manager(mockserver):
     client = ZyteAPI(api_key="a", api_url=mockserver.urljoin("/"))
     queries = [
         {"url": "https://a.example", "httpResponseBody": True},
         {"url": "https://exception.example", "httpResponseBody": True},
         {"url": "https://b.example", "httpResponseBody": True},
     ]
     expected_results = [
@@ -83,28 +83,68 @@
         {
             "url": "https://b.example",
             "httpResponseBody": "PGh0bWw+PGJvZHk+SGVsbG88aDE+V29ybGQhPC9oMT48L2JvZHk+PC9odG1sPg==",
         },
     ]
     actual_results = []
     with client.session() as session:
-        assert session._context.connector.limit == client._async_client.n_conn
+        assert session._session.connector.limit == client._async_client.n_conn
         actual_results.append(session.get(queries[0]))
         for result in session.iter(queries[1:]):
             actual_results.append(result)
-        aiohttp_session = session._context
+        aiohttp_session = session._session
         assert not aiohttp_session.closed
     assert aiohttp_session.closed
-    assert session._context is None
 
     with pytest.raises(RuntimeError):
         session.get(queries[0])
 
+    assert isinstance(next(iter(session.iter(queries[1:]))), RuntimeError)
+
+    assert len(actual_results) == len(expected_results)
+    for actual_result in actual_results:
+        if isinstance(actual_result, Exception):
+            assert Exception in expected_results
+        else:
+            assert actual_result in expected_results
+
+
+def test_session_no_context_manager(mockserver):
+    client = ZyteAPI(api_key="a", api_url=mockserver.urljoin("/"))
+    queries = [
+        {"url": "https://a.example", "httpResponseBody": True},
+        {"url": "https://exception.example", "httpResponseBody": True},
+        {"url": "https://b.example", "httpResponseBody": True},
+    ]
+    expected_results = [
+        {
+            "url": "https://a.example",
+            "httpResponseBody": "PGh0bWw+PGJvZHk+SGVsbG88aDE+V29ybGQhPC9oMT48L2JvZHk+PC9odG1sPg==",
+        },
+        Exception,
+        {
+            "url": "https://b.example",
+            "httpResponseBody": "PGh0bWw+PGJvZHk+SGVsbG88aDE+V29ybGQhPC9oMT48L2JvZHk+PC9odG1sPg==",
+        },
+    ]
+    actual_results = []
+    session = client.session()
+    assert session._session.connector.limit == client._async_client.n_conn
+    actual_results.append(session.get(queries[0]))
+    for result in session.iter(queries[1:]):
+        actual_results.append(result)
+    aiohttp_session = session._session
+    assert not aiohttp_session.closed
+    session.close()
+    assert aiohttp_session.closed
+
     with pytest.raises(RuntimeError):
-        session.iter(queries[1:])
+        session.get(queries[0])
+
+    assert isinstance(next(iter(session.iter(queries[1:]))), RuntimeError)
 
     assert len(actual_results) == len(expected_results)
     for actual_result in actual_results:
         if isinstance(actual_result, Exception):
             assert Exception in expected_results
         else:
             assert actual_result in expected_results
```

### Comparing `zyte-api-0.5.0/tests/test_utils.py` & `zyte_api-0.5.1/tests/test_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -110,15 +110,16 @@
 
 
 def test_process_query_bytes():
     with raises(ValueError):
         _process_query({"url": b"https://example.com"})
 
 
-def test_deprecated_create_session():
+@pytest.mark.asyncio  # https://github.com/aio-libs/aiohttp/pull/1468
+async def test_deprecated_create_session():
     from zyte_api.aio.client import create_session as _create_session
 
     with pytest.warns(
         DeprecationWarning,
         match=r"^zyte_api\.aio\.client\.create_session is deprecated",
     ):
         _create_session()
```

### Comparing `zyte-api-0.5.0/zyte_api/__main__.py` & `zyte_api-0.5.1/zyte_api/__main__.py`

 * *Files identical despite different names*

### Comparing `zyte-api-0.5.0/zyte_api/_async.py` & `zyte_api-0.5.1/zyte_api/_async.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,62 +29,52 @@
         return session.post
 
 
 class _AsyncSession:
     def __init__(self, client, **session_kwargs):
         self._client = client
         self._session = create_session(client.n_conn, **session_kwargs)
-        self._context = None
 
     async def __aenter__(self):
-        self._context = await self._session.__aenter__()
         return self
 
     async def __aexit__(self, *exc_info):
-        result = await self._context.__aexit__(*exc_info)
-        self._context = None
-        return result
+        await self._session.close()
 
-    def _check_context(self):
-        if self._context is None:
-            raise RuntimeError(
-                "Attempt to use session method on a session either not opened "
-                "or already closed."
-            )
+    async def close(self):
+        await self._session.close()
 
     async def get(
         self,
         query: dict,
         *,
         endpoint: str = "extract",
         handle_retries=True,
         retrying: Optional[AsyncRetrying] = None,
     ):
-        self._check_context()
         return await self._client.get(
             query=query,
             endpoint=endpoint,
             handle_retries=handle_retries,
             retrying=retrying,
-            session=self._context,
+            session=self._session,
         )
 
     def iter(
         self,
         queries: List[dict],
         *,
         endpoint: str = "extract",
         handle_retries=True,
         retrying: Optional[AsyncRetrying] = None,
     ) -> Iterator[Future]:
-        self._check_context()
         return self._client.iter(
             queries=queries,
             endpoint=endpoint,
-            session=self._context,
+            session=self._session,
             handle_retries=handle_retries,
             retrying=retrying,
         )
 
 
 class AsyncZyteAPI:
     """:ref:`Asynchronous Zyte API client <asyncio_api>`.
@@ -204,8 +194,22 @@
                 handle_retries=handle_retries,
                 retrying=retrying,
             )
 
         return asyncio.as_completed([_request(query) for query in queries])
 
     def session(self, **kwargs):
+        """Asynchronous equivalent to :meth:`ZyteAPI.session`.
+
+        You do not need to use :meth:`~AsyncZyteAPI.session` as an async
+        context manager as long as you await ``close()`` on the object it
+        returns when you are done:
+
+        .. code-block:: python
+
+            session = client.session()
+            try:
+                ...
+            finally:
+                await session.close()
+        """
         return _AsyncSession(client=self, **kwargs)
```

### Comparing `zyte-api-0.5.0/zyte_api/_errors.py` & `zyte_api-0.5.1/zyte_api/_errors.py`

 * *Files identical despite different names*

### Comparing `zyte-api-0.5.0/zyte_api/_retry.py` & `zyte_api-0.5.1/zyte_api/_retry.py`

 * *Files identical despite different names*

### Comparing `zyte-api-0.5.0/zyte_api/_sync.py` & `zyte_api-0.5.1/zyte_api/_sync.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,65 +16,61 @@
         asyncio.set_event_loop(loop)
         return loop
 
 
 class _Session:
     def __init__(self, client, **session_kwargs):
         self._client = client
-        self._session = client._async_client.session(**session_kwargs)
-        self._context = None
 
-    def __enter__(self):
+        # https://github.com/aio-libs/aiohttp/pull/1468
+        async def create_session():
+            return client._async_client.session(**session_kwargs)._session
+
         loop = _get_loop()
-        self._context = loop.run_until_complete(self._session.__aenter__())._context
+        self._session = loop.run_until_complete(create_session())
+
+    def __enter__(self):
         return self
 
     def __exit__(self, *exc_info):
         loop = _get_loop()
-        result = loop.run_until_complete(self._context.__aexit__(*exc_info))
-        self._context = None
-        return result
-
-    def _check_context(self):
-        if self._context is None:
-            raise RuntimeError(
-                "Attempt to use session method on a session either not opened "
-                "or already closed."
-            )
+        loop.run_until_complete(self._session.close())
+
+    def close(self):
+        loop = _get_loop()
+        loop.run_until_complete(self._session.close())
 
     def get(
         self,
         query: dict,
         *,
         endpoint: str = "extract",
         handle_retries=True,
         retrying: Optional[AsyncRetrying] = None,
     ):
-        self._check_context()
         return self._client.get(
             query=query,
             endpoint=endpoint,
             handle_retries=handle_retries,
             retrying=retrying,
-            session=self._context,
+            session=self._session,
         )
 
     def iter(
         self,
         queries: List[dict],
         *,
         endpoint: str = "extract",
         handle_retries=True,
         retrying: Optional[AsyncRetrying] = None,
     ) -> Generator[Union[dict, Exception], None, None]:
-        self._check_context()
         return self._client.iter(
             queries=queries,
             endpoint=endpoint,
-            session=self._context,
+            session=self._session,
             handle_retries=handle_retries,
             retrying=retrying,
         )
 
 
 class ZyteAPI:
     """:ref:`Synchronous Zyte API client <sync>`.
@@ -182,28 +178,38 @@
         ):
             try:
                 yield loop.run_until_complete(future)
             except Exception as exception:
                 yield exception
 
     def session(self, **kwargs):
-        """:ref:`Context manager <context-managers>` to create a contextual
-        session.
+        """:ref:`Context manager <context-managers>` to create a session.
 
-        A contextual session is an object that has the same API as the client
-        object, except:
+        A session is an object that has the same API as the client object,
+        except:
 
         -   :meth:`get` and :meth:`iter` do not have a *session* parameter,
-            the contextual session creates an :class:`aiohttp.ClientSession`
-            object and passes it to :meth:`get` and :meth:`iter` automatically.
+            the session creates an :class:`aiohttp.ClientSession` object and
+            passes it to :meth:`get` and :meth:`iter` automatically.
 
         -   It does not have a :meth:`session` method.
 
         Using the same :class:`aiohttp.ClientSession` object for all Zyte API
         requests improves performance by keeping a pool of reusable connections
         to Zyte API.
 
         The :class:`aiohttp.ClientSession` object is created with sane defaults
         for Zyte API, but you can use *kwargs* to pass additional parameters to
         :class:`aiohttp.ClientSession` and even override those sane defaults.
+
+        You do not need to use :meth:`session` as a context manager as long as
+        you call ``close()`` on the object it returns when you are done:
+
+        .. code-block:: python
+
+            session = client.session()
+            try:
+                ...
+            finally:
+                session.close()
         """
         return _Session(client=self, **kwargs)
```

### Comparing `zyte-api-0.5.0/zyte_api/_utils.py` & `zyte_api-0.5.1/zyte_api/_utils.py`

 * *Files identical despite different names*

### Comparing `zyte-api-0.5.0/zyte_api/aio/__init__.py` & `zyte_api-0.5.1/zyte_api/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `zyte-api-0.5.0/zyte_api/apikey.py` & `zyte_api-0.5.1/zyte_api/apikey.py`

 * *Files identical despite different names*

### Comparing `zyte-api-0.5.0/zyte_api/errors.py` & `zyte_api-0.5.1/zyte_api/errors.py`

 * *Files identical despite different names*

### Comparing `zyte-api-0.5.0/zyte_api/stats.py` & `zyte_api-0.5.1/zyte_api/stats.py`

 * *Files identical despite different names*

### Comparing `zyte-api-0.5.0/zyte_api/utils.py` & `zyte_api-0.5.1/zyte_api/utils.py`

 * *Files identical despite different names*

### Comparing `zyte-api-0.5.0/zyte_api.egg-info/PKG-INFO` & `zyte_api-0.5.1/zyte_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zyte-api
-Version: 0.5.0
+Version: 0.5.1
 Summary: Python interface to Zyte API
 Home-page: https://github.com/zytedata/python-zyte-api
 Author: Zyte Group Ltd
 Author-email: opensource@zyte.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `zyte-api-0.5.0/zyte_api.egg-info/SOURCES.txt` & `zyte_api-0.5.1/zyte_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

