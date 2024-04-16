# Comparing `tmp/setech-1.2.0.tar.gz` & `tmp/setech-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "setech-1.2.0.tar", last modified: Wed Apr 10 13:58:28 2024, max compression
+gzip compressed data, was "setech-1.2.1.tar", last modified: Tue Apr 16 11:12:15 2024, max compression
```

## Comparing `setech-1.2.0.tar` & `setech-1.2.1.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-04-10 13:58:28.427983 setech-1.2.0/
--rw-r--r--   0 eriks     (1000) eriks     (1000)     1059 2024-04-03 10:57:10.000000 setech-1.2.0/LICENCE
--rw-r--r--   0 eriks     (1000) eriks     (1000)     5345 2024-04-10 13:58:28.427983 setech-1.2.0/PKG-INFO
--rw-r--r--   0 eriks     (1000) eriks     (1000)     4473 2024-04-03 21:15:13.000000 setech-1.2.0/README.md
--rw-r--r--   0 eriks     (1000) eriks     (1000)     1912 2024-04-10 13:58:19.000000 setech-1.2.0/pyproject.toml
--rw-r--r--   0 eriks     (1000) eriks     (1000)       38 2024-04-10 13:58:28.427983 setech-1.2.0/setup.cfg
-drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-04-10 13:58:28.424650 setech-1.2.0/src/
-drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-04-10 13:58:28.427983 setech-1.2.0/src/setech/
--rw-r--r--   0 eriks     (1000) eriks     (1000)      117 2024-04-10 13:58:19.000000 setech-1.2.0/src/setech/__init__.py
-drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-04-10 13:58:28.427983 setech-1.2.0/src/setech/api_client/
--rw-r--r--   0 eriks     (1000) eriks     (1000)      115 2024-04-03 13:03:49.000000 setech-1.2.0/src/setech/api_client/__init__.py
--rw-r--r--   0 eriks     (1000) eriks     (1000)     4832 2024-04-03 09:38:51.000000 setech-1.2.0/src/setech/api_client/_base.py
--rw-r--r--   0 eriks     (1000) eriks     (1000)     2258 2024-04-03 09:38:51.000000 setech-1.2.0/src/setech/api_client/async_client.py
--rw-r--r--   0 eriks     (1000) eriks     (1000)     2163 2024-04-03 09:38:59.000000 setech-1.2.0/src/setech/api_client/sync_client.py
-drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-04-10 13:58:28.427983 setech-1.2.0/src/setech/constants/
--rw-r--r--   0 eriks     (1000) eriks     (1000)      125 2024-04-03 14:55:19.000000 setech-1.2.0/src/setech/constants/__init__.py
--rw-r--r--   0 eriks     (1000) eriks     (1000)      519 2024-04-03 14:22:18.000000 setech-1.2.0/src/setech/constants/date.py
-drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-04-10 13:58:28.427983 setech-1.2.0/src/setech/logging/
--rw-r--r--   0 eriks     (1000) eriks     (1000)      138 2024-04-10 13:57:32.000000 setech-1.2.0/src/setech/logging/__init__.py
--rw-r--r--   0 eriks     (1000) eriks     (1000)     1394 2024-04-03 20:53:03.000000 setech-1.2.0/src/setech/logging/formatters.py
--rw-r--r--   0 eriks     (1000) eriks     (1000)     1718 2024-04-04 13:24:48.000000 setech-1.2.0/src/setech/logging/handlers.py
--rw-r--r--   0 eriks     (1000) eriks     (1000)        0 2024-03-19 14:21:21.000000 setech-1.2.0/src/setech/py.typed
-drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-04-10 13:58:28.427983 setech-1.2.0/src/setech/utils/
--rw-r--r--   0 eriks     (1000) eriks     (1000)      921 2024-04-10 13:57:32.000000 setech-1.2.0/src/setech/utils/__init__.py
--rw-r--r--   0 eriks     (1000) eriks     (1000)      849 2024-04-10 13:57:32.000000 setech-1.2.0/src/setech/utils/numeric.py
--rw-r--r--   0 eriks     (1000) eriks     (1000)     2013 2024-04-10 13:57:32.000000 setech-1.2.0/src/setech/utils/parse.py
--rw-r--r--   0 eriks     (1000) eriks     (1000)     5598 2024-04-10 13:57:32.000000 setech-1.2.0/src/setech/utils/ssn.py
--rw-r--r--   0 eriks     (1000) eriks     (1000)     1097 2024-04-03 14:55:19.000000 setech-1.2.0/src/setech/utils/text.py
--rw-r--r--   0 eriks     (1000) eriks     (1000)     1034 2024-04-03 15:03:11.000000 setech-1.2.0/src/setech/utils/validators.py
--rw-r--r--   0 eriks     (1000) eriks     (1000)     1453 2024-04-10 13:57:32.000000 setech-1.2.0/src/setech/utils/various.py
-drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-04-10 13:58:28.427983 setech-1.2.0/src/setech.egg-info/
--rw-r--r--   0 eriks     (1000) eriks     (1000)     5345 2024-04-10 13:58:28.000000 setech-1.2.0/src/setech.egg-info/PKG-INFO
--rw-r--r--   0 eriks     (1000) eriks     (1000)      732 2024-04-10 13:58:28.000000 setech-1.2.0/src/setech.egg-info/SOURCES.txt
--rw-r--r--   0 eriks     (1000) eriks     (1000)        1 2024-04-10 13:58:28.000000 setech-1.2.0/src/setech.egg-info/dependency_links.txt
--rw-r--r--   0 eriks     (1000) eriks     (1000)       50 2024-04-10 13:58:28.000000 setech-1.2.0/src/setech.egg-info/requires.txt
--rw-r--r--   0 eriks     (1000) eriks     (1000)        7 2024-04-10 13:58:28.000000 setech-1.2.0/src/setech.egg-info/top_level.txt
+drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-04-16 11:12:15.919209 setech-1.2.1/
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     1059 2024-04-03 10:57:10.000000 setech-1.2.1/LICENCE
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     5345 2024-04-16 11:12:15.919209 setech-1.2.1/PKG-INFO
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     4473 2024-04-03 21:15:13.000000 setech-1.2.1/README.md
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     1912 2024-04-16 11:12:09.000000 setech-1.2.1/pyproject.toml
+-rw-r--r--   0 eriks     (1000) eriks     (1000)       38 2024-04-16 11:12:15.919209 setech-1.2.1/setup.cfg
+drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-04-16 11:12:15.915876 setech-1.2.1/src/
+drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-04-16 11:12:15.915876 setech-1.2.1/src/setech/
+-rw-r--r--   0 eriks     (1000) eriks     (1000)      117 2024-04-16 11:12:09.000000 setech-1.2.1/src/setech/__init__.py
+drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-04-16 11:12:15.915876 setech-1.2.1/src/setech/api_client/
+-rw-r--r--   0 eriks     (1000) eriks     (1000)      115 2024-04-03 13:03:49.000000 setech-1.2.1/src/setech/api_client/__init__.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     6368 2024-04-16 11:12:02.000000 setech-1.2.1/src/setech/api_client/_base.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     2332 2024-04-16 11:12:02.000000 setech-1.2.1/src/setech/api_client/async_client.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     2237 2024-04-16 11:12:02.000000 setech-1.2.1/src/setech/api_client/sync_client.py
+drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-04-16 11:12:15.919209 setech-1.2.1/src/setech/constants/
+-rw-r--r--   0 eriks     (1000) eriks     (1000)      125 2024-04-03 14:55:19.000000 setech-1.2.1/src/setech/constants/__init__.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)      519 2024-04-03 14:22:18.000000 setech-1.2.1/src/setech/constants/date.py
+drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-04-16 11:12:15.919209 setech-1.2.1/src/setech/logging/
+-rw-r--r--   0 eriks     (1000) eriks     (1000)      138 2024-04-10 13:57:32.000000 setech-1.2.1/src/setech/logging/__init__.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     1394 2024-04-03 20:53:03.000000 setech-1.2.1/src/setech/logging/formatters.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     1718 2024-04-04 13:24:48.000000 setech-1.2.1/src/setech/logging/handlers.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)        0 2024-03-19 14:21:21.000000 setech-1.2.1/src/setech/py.typed
+drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-04-16 11:12:15.919209 setech-1.2.1/src/setech/utils/
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     1058 2024-04-16 11:12:02.000000 setech-1.2.1/src/setech/utils/__init__.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)      878 2024-04-16 11:12:02.000000 setech-1.2.1/src/setech/utils/numeric.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     3954 2024-04-16 11:12:02.000000 setech-1.2.1/src/setech/utils/parse.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     5598 2024-04-10 13:57:32.000000 setech-1.2.1/src/setech/utils/ssn.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     1097 2024-04-03 14:55:19.000000 setech-1.2.1/src/setech/utils/text.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     1034 2024-04-12 10:20:23.000000 setech-1.2.1/src/setech/utils/validators.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)      324 2024-04-16 11:12:02.000000 setech-1.2.1/src/setech/utils/various.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     1204 2024-04-16 11:12:02.000000 setech-1.2.1/src/setech/utils/warnings.py
+drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-04-16 11:12:15.919209 setech-1.2.1/src/setech.egg-info/
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     5345 2024-04-16 11:12:15.000000 setech-1.2.1/src/setech.egg-info/PKG-INFO
+-rw-r--r--   0 eriks     (1000) eriks     (1000)      761 2024-04-16 11:12:15.000000 setech-1.2.1/src/setech.egg-info/SOURCES.txt
+-rw-r--r--   0 eriks     (1000) eriks     (1000)        1 2024-04-16 11:12:15.000000 setech-1.2.1/src/setech.egg-info/dependency_links.txt
+-rw-r--r--   0 eriks     (1000) eriks     (1000)       50 2024-04-16 11:12:15.000000 setech-1.2.1/src/setech.egg-info/requires.txt
+-rw-r--r--   0 eriks     (1000) eriks     (1000)        7 2024-04-16 11:12:15.000000 setech-1.2.1/src/setech.egg-info/top_level.txt
```

### Comparing `setech-1.2.0/LICENCE` & `setech-1.2.1/LICENCE`

 * *Files identical despite different names*

### Comparing `setech-1.2.0/PKG-INFO` & `setech-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setech
-Version: 1.2.0
+Version: 1.2.1
 Summary: Setech utilities
 Author-email: Eriks Karls <eriks.karls@sefinance.lv>
 Project-URL: Homepage, https://pypi.org/project/setech/
 Keywords: setech,logging,api-client,utility,utils
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `setech-1.2.0/README.md` & `setech-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `setech-1.2.0/pyproject.toml` & `setech-1.2.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 
 [tool.setuptools.dynamic]
 version = { attr = "setech.__version__" }
 
 
 [tool.bumpversion]
-current_version = "1.2.0"
+current_version = "1.2.1"
 commit = true
 tag = true
 tag_name = "v{new_version}"
 tag_message = "Bump version: {current_version} → {new_version}"
 allow_dirty = false
 parse = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)"
 serialize = ["{major}.{minor}.{patch}"]
```

### Comparing `setech-1.2.0/src/setech/api_client/_base.py` & `setech-1.2.1/src/setech/api_client/_base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 from abc import ABC, abstractmethod
 from typing import Any, Coroutine
 
 import httpx
 from pydantic import HttpUrl
 
-from setech.utils import get_logger, get_nonce, shortify_log_dict
+from setech.utils import get_logger, get_nonce, shortify_log_extra_data
 
 _TypeSyncAsyncResponse = httpx.Response | Coroutine[Any, Any, httpx.Response]
 
 
 class BaseClient(ABC):
     base_url: HttpUrl
     _session: httpx._client.BaseClient
@@ -19,89 +19,148 @@
     def __init__(self, nonce: str = "", session: httpx._client.BaseClient | None = None):
         self._nonce = nonce or get_nonce()
         self._session = session or httpx.Client()
         self._logger = get_logger("APIClient")
 
     @abstractmethod
     def get(self, endpoint: str, *, params: Any = None, **kwargs: Any) -> _TypeSyncAsyncResponse:
+        """
+        Send a `GET` request.
+
+        :param endpoint: Endpoint path to which to make request
+        **Parameters**: See `httpx.request`.
+        """
         pass
 
     @abstractmethod
     def post(self, endpoint: str, *, json: Any = None, data: Any = None, **kwargs: Any) -> _TypeSyncAsyncResponse:
+        """
+        Send a `POST` request.
+
+        :param endpoint: Endpoint path to which to make request
+        **Parameters**: See `httpx.request`.
+        """
         pass
 
     @abstractmethod
     def put(self, endpoint: str, *, json: Any = None, data: Any = None, **kwargs: Any) -> _TypeSyncAsyncResponse:
+        """
+        Send a `PUT` request.
+
+        :param endpoint: Endpoint path to which to make request
+        **Parameters**: See `httpx.request`.
+        """
         pass
 
     @abstractmethod
     def patch(self, endpoint: str, *, json: Any = None, data: Any = None, **kwargs: Any) -> _TypeSyncAsyncResponse:
+        """
+        Send a `PATCH` request.
+
+        :param endpoint: Endpoint path to which to make request
+        **Parameters**: See `httpx.request`.
+        """
         pass
 
     @abstractmethod
     def delete(self, endpoint: str, *, params: Any = None, **kwargs: Any) -> _TypeSyncAsyncResponse:
+        """
+        Send a `DELETE` request.
+
+        :param endpoint: Endpoint path to which to make request
+        :param params: See `httpx.request`.
+        :param kwargs: See `httpx.request`.
+        """
         pass
 
     @abstractmethod
     def head(self, endpoint: str, *, params: Any = None, **kwargs: Any) -> _TypeSyncAsyncResponse:
+        """
+        Send a `HEAD` request.
+
+        :param endpoint: Endpoint path to which to make request
+        **Parameters**: See `httpx.request`.
+        """
         pass
 
     @abstractmethod
     def options(self, endpoint: str, *, params: Any = None, **kwargs: Any) -> _TypeSyncAsyncResponse:
+        """
+        Send a `OPTIONS` request.
+
+        :param endpoint: Endpoint path to which to make request
+        **Parameters**: See `httpx.request`.
+        """
         pass
 
     @abstractmethod
     def trace(self, endpoint: str, *, params: Any = None, **kwargs: Any) -> _TypeSyncAsyncResponse:
         pass
 
     @abstractmethod
     def connect(self, endpoint: str, *, params: Any = None, **kwargs: Any) -> _TypeSyncAsyncResponse:
         pass
 
     @abstractmethod
     def _request(self, method: str, endpoint: str, **kwargs: Any) -> _TypeSyncAsyncResponse:
         pass
 
+    def before_request(self, request: httpx.Request) -> None:
+        pass
+
+    def after_request(self, response: httpx.Response) -> None:
+        pass
+
     def _make_full_url(self, endpoint: str) -> str:
         return f"{self.base_url}{endpoint}"
 
     def prepare_authentication(self, request: httpx.Request) -> httpx.Request:
         return request
 
     def _prepare_request(self, method: str, endpoint: str, **kwargs: Any) -> httpx.Request:
         full_url = self._make_full_url(endpoint)
 
         self._debug_log_request(method, full_url)
         request: httpx.Request = self._session.build_request(method=method, url=full_url, **kwargs)
         self._debug_log_prepared_request(request)
-        self._debug(f"Prepared {request.method} request to '{request.url}'", extra=request.__dict__)
-
         self._info_log_request_sending(
-            request, kwargs.get("content") or kwargs.get("files") or kwargs.get("data") or kwargs.get("json")
+            request,
+            dict(
+                content=kwargs.get("content"),
+                files=kwargs.get("files"),
+                data=kwargs.get("data"),
+                json=kwargs.get("json"),
+            ),
         )
         return request
 
     def _debug_log_request(self, method: str, full_url: str) -> None:
         self._debug(f"Preparing {method} request for '{full_url}'")
 
     def _debug_log_prepared_request(self, request: httpx.Request) -> None:
         self._debug(f"Prepared {request.method} request to '{request.url}'", extra=request.__dict__)
 
     def _info_log_request_sending(self, request: httpx.Request, log_payload: Any) -> None:
         self._info(
-            f"Sending {request.method} request to '{request.url}' with payload={shortify_log_dict(log_payload)!r}",
-            extra={"payload": shortify_log_dict(log_payload)},
+            f"Sending {request.method} request to '{request.url}'",
+            extra={"payload": shortify_log_extra_data(log_payload)},
         )
 
     def _info_log_response(self, response: httpx.Response) -> None:
-        str_repr_content = response.content.decode("utf8")[:500]
-        self._info(
-            f"Response {response.status_code=} {str_repr_content=}",
-            extra={"status_code": response.status_code, "content": str_repr_content},
-        )
+        try:
+            str_repr_content = response.content.decode("utf8")[:500]
+            self._info(
+                f"Response {response.status_code=} {str_repr_content=}",
+                extra={"status_code": response.status_code, "content": str_repr_content},
+            )
+        except:  # noqa
+            self._info(
+                f"Response {response.status_code=}",
+                extra={"response": response.__dict__},
+            )
 
     def _info(self, msg: str, *args: Any, **kwargs: Any) -> None:
         self._log("INFO", f"[{self._nonce}] {msg}", *args, **kwargs)
 
     def _debug(self, msg: str, *args: Any, **kwargs: Any) -> None:
         self._log("DEBUG", f"[{self._nonce}] {msg}", *args, **kwargs)
```

### Comparing `setech-1.2.0/src/setech/api_client/async_client.py` & `setech-1.2.1/src/setech/api_client/async_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,11 +36,13 @@
         return await self._request("GET", endpoint, params=params, **kwargs)
 
     async def connect(self, endpoint: str, *, params: Any = None, **kwargs: Any) -> httpx.Response:
         return await self._request("GET", endpoint, params=params, **kwargs)
 
     async def _request(self, method: str, endpoint: str, **kwargs: Any) -> httpx.Response:
         request = self._prepare_request(method, endpoint, **kwargs)
+        self.before_request(request)
         response = await self._session.send(request, auth=self.prepare_authentication)
         self._info_log_response(response)
+        self.after_request(response)
 
         return response
```

### Comparing `setech-1.2.0/src/setech/api_client/sync_client.py` & `setech-1.2.1/src/setech/api_client/sync_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,11 +37,13 @@
         return self._request("TRACE", endpoint, params=params, **kwargs)
 
     def connect(self, endpoint: str, *, params: Any = None, **kwargs: Any) -> httpx.Response:
         return self._request("CONNECT", endpoint, params=params, **kwargs)
 
     def _request(self, method: str, endpoint: str, **kwargs: Any) -> httpx.Response:
         request = self._prepare_request(method, endpoint, **kwargs)
+        self.before_request(request)
         response = self._session.send(request, auth=self.prepare_authentication)
         self._info_log_response(response)
+        self.after_request(response)
 
         return response
```

### Comparing `setech-1.2.0/src/setech/constants/date.py` & `setech-1.2.1/src/setech/constants/date.py`

 * *Files identical despite different names*

### Comparing `setech-1.2.0/src/setech/logging/formatters.py` & `setech-1.2.1/src/setech/logging/formatters.py`

 * *Files identical despite different names*

### Comparing `setech-1.2.0/src/setech/logging/handlers.py` & `setech-1.2.1/src/setech/logging/handlers.py`

 * *Files identical despite different names*

### Comparing `setech-1.2.0/src/setech/utils/__init__.py` & `setech-1.2.1/src/setech/utils/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,37 @@
 from .numeric import round_decimal
-from .parse import SetechJSONEncoder, as_decimal, as_decimal_or_none, str_as_date, str_as_date_or_none
+from .parse import (
+    SetechJSONEncoder,
+    as_decimal,
+    as_decimal_or_none,
+    jsonify_value,
+    shorten_value,
+    shortify_log_extra_data,
+    str_as_date,
+    str_as_date_or_none,
+)
 from .ssn import generate_aged_latvian_personal_code, generate_random_latvian_personal_code
 from .text import convert_datetime_to_latvian_words, convert_number_to_latvian_words
 from .validators import validate_iban, validate_latvian_personal_code
-from .various import get_logger, get_nonce, shorten_value, shortify_log_dict
+from .various import get_logger, get_nonce
 
 __all__ = [
     "round_decimal",
     "SetechJSONEncoder",
-    "str_as_date",
-    "str_as_date_or_none",
     "as_decimal",
     "as_decimal_or_none",
+    "jsonify_value",
+    "shorten_value",
+    "shortify_log_extra_data",
+    "str_as_date",
+    "str_as_date_or_none",
     "convert_datetime_to_latvian_words",
     "convert_number_to_latvian_words",
     "generate_aged_latvian_personal_code",
     "generate_random_latvian_personal_code",
     "validate_iban",
     "validate_latvian_personal_code",
     "get_logger",
     "get_nonce",
     "shorten_value",
-    "shortify_log_dict",
+    "shortify_log_extra_data",
 ]
```

### Comparing `setech-1.2.0/src/setech/utils/numeric.py` & `setech-1.2.1/src/setech/utils/numeric.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import decimal
 
+__all__ = ["round_decimal"]
+
 
 def round_decimal(dec: decimal.Decimal, precision: int = 4) -> decimal.Decimal:
     """Round decimal value to a predefined precision from the start of the value. Examples:
         - dec=123.456, precision=7 -> 123.4560,
         - dec=123.456, precision=5 -> 123.46,
         - dec=123.456, precision=3 -> 123,
         - dec=123.456, precision=2 -> 120;
```

### Comparing `setech-1.2.0/src/setech/utils/ssn.py` & `setech-1.2.1/src/setech/utils/ssn.py`

 * *Files identical despite different names*

### Comparing `setech-1.2.0/src/setech/utils/text.py` & `setech-1.2.1/src/setech/utils/text.py`

 * *Files identical despite different names*

### Comparing `setech-1.2.0/src/setech/utils/validators.py` & `setech-1.2.1/src/setech/utils/validators.py`

 * *Files identical despite different names*

### Comparing `setech-1.2.0/src/setech.egg-info/PKG-INFO` & `setech-1.2.1/src/setech.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setech
-Version: 1.2.0
+Version: 1.2.1
 Summary: Setech utilities
 Author-email: Eriks Karls <eriks.karls@sefinance.lv>
 Project-URL: Homepage, https://pypi.org/project/setech/
 Keywords: setech,logging,api-client,utility,utils
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `setech-1.2.0/src/setech.egg-info/SOURCES.txt` & `setech-1.2.1/src/setech.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -19,8 +19,9 @@
 src/setech/logging/handlers.py
 src/setech/utils/__init__.py
 src/setech/utils/numeric.py
 src/setech/utils/parse.py
 src/setech/utils/ssn.py
 src/setech/utils/text.py
 src/setech/utils/validators.py
-src/setech/utils/various.py
+src/setech/utils/various.py
+src/setech/utils/warnings.py
```

