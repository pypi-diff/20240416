# Comparing `tmp/life360-7.0.0b0.tar.gz` & `tmp/life360-7.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "life360-7.0.0b0.tar", last modified: Mon Apr  8 23:25:41 2024, max compression
+gzip compressed data, was "life360-7.0.0b1.tar", last modified: Tue Apr 16 15:21:12 2024, max compression
```

## Comparing `life360-7.0.0b0.tar` & `life360-7.0.0b1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:25:41.793051 life360-7.0.0b0/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-08 23:25:39.000000 life360-7.0.0b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-08 23:25:41.793051 life360-7.0.0b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-08 23:25:39.000000 life360-7.0.0b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:25:41.793051 life360-7.0.0b0/life360/
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-08 23:25:39.000000 life360-7.0.0b0/life360/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10262 2024-04-08 23:25:39.000000 life360-7.0.0b0/life360/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-08 23:25:39.000000 life360-7.0.0b0/life360/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-08 23:25:39.000000 life360-7.0.0b0/life360/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-08 23:25:39.000000 life360-7.0.0b0/life360/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:25:41.793051 life360-7.0.0b0/life360.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-08 23:25:41.000000 life360-7.0.0b0/life360.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-08 23:25:41.000000 life360-7.0.0b0/life360.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 23:25:41.000000 life360-7.0.0b0/life360.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-08 23:25:41.000000 life360-7.0.0b0/life360.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-08 23:25:41.000000 life360-7.0.0b0/life360.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 23:25:41.793051 life360-7.0.0b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-08 23:25:39.000000 life360-7.0.0b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:21:12.506760 life360-7.0.0b1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-16 15:21:07.000000 life360-7.0.0b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-16 15:21:12.506760 life360-7.0.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-16 15:21:07.000000 life360-7.0.0b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:21:12.506760 life360-7.0.0b1/life360/
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-16 15:21:07.000000 life360-7.0.0b1/life360/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11197 2024-04-16 15:21:07.000000 life360-7.0.0b1/life360/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-16 15:21:07.000000 life360-7.0.0b1/life360/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-16 15:21:07.000000 life360-7.0.0b1/life360/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-16 15:21:07.000000 life360-7.0.0b1/life360/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:21:12.506760 life360-7.0.0b1/life360.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-16 15:21:12.000000 life360-7.0.0b1/life360.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-16 15:21:12.000000 life360-7.0.0b1/life360.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 15:21:12.000000 life360-7.0.0b1/life360.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-16 15:21:12.000000 life360-7.0.0b1/life360.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-16 15:21:12.000000 life360-7.0.0b1/life360.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 15:21:12.506760 life360-7.0.0b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-16 15:21:07.000000 life360-7.0.0b1/setup.py
```

### Comparing `life360-7.0.0b0/LICENSE` & `life360-7.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `life360-7.0.0b0/PKG-INFO` & `life360-7.0.0b1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: life360
-Version: 7.0.0b0
+Version: 7.0.0b1
 Summary: Life360 Communications Module
 Home-page: https://github.com/pnbruckner/life360
 Author: Phil Bruckner
 Author-email: pnbruckner@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `life360-7.0.0b0/README.md` & `life360-7.0.0b1/README.md`

 * *Files identical despite different names*

### Comparing `life360-7.0.0b0/life360/__init__.py` & `life360-7.0.0b1/life360/__init__.py`

 * *Files identical despite different names*

### Comparing `life360-7.0.0b0/life360/api.py` & `life360-7.0.0b1/life360/api.py`

 * *Files 13% similar despite different names*

```diff
@@ -113,84 +113,110 @@
         3 -> No informational redactions
         4 -> No redactions
         """
         self._session = session
         if max_retries < 0:
             raise ValueError("max_retries must be non-negative")
         self._max_attempts = max_retries + 1
-        self._verbosity = verbosity
         self._authorization = authorization
+        self.verbosity = verbosity
         self._etags: dict[str, str] = {}
 
     @property
+    def verbosity(self) -> int:
+        """Return verbosity level."""
+        return self._verbosity
+
+    @verbosity.setter
+    def verbosity(self, value: int) -> None:
+        """Set verbosity level."""
+        if not (0 <= value <= 4):
+            raise ValueError("verbosity must be between 0 and 4, inclusive")
+        self._verbosity = value
+
+    @property
     def authorization(self) -> str | None:
         """Return authorization."""
         return self._authorization
 
-    async def login_by_username(self, username: str, password: str) -> None:
+    async def login_by_username(self, username: str, password: str) -> str:
         """Log into Life360 server using username & password."""
         reply = cast(
             Mapping[str, str],
             await self._request(
                 _TOKEN_URL,
-                "post",
+                method="post",
+                raise_not_modified=False,
                 data={
                     "grant_type": "password",
                     "username": username,
                     "password": password,
                 },
                 authorization=f"Basic {CLIENT_TOKEN}",
             ),
         )
         try:
             self._authorization = f"{reply['token_type']} {reply['access_token']}"
         except KeyError:
             raise Life360Error(
                 f"Unexpected response while logging in by username: {reply}"
             ) from None
+        return self._authorization
 
-    async def get_circles(self) -> list[dict[str, str]]:
+    async def get_circles(
+        self, *, raise_not_modified: bool = False
+    ) -> list[dict[str, str]]:
         """Get basic data about all Circles."""
         return cast(
             dict[str, list[dict[str, str]]],
-            await self._request(_CIRCLES_URL),
+            await self._request(_CIRCLES_URL, raise_not_modified),
         )["circles"]
 
-    async def get_circle_members(self, cid: str) -> list[dict[str, Any]]:
+    async def get_circle_members(
+        self, cid: str, *, raise_not_modified: bool = False
+    ) -> list[dict[str, Any]]:
         """Get details for Members in given Circle."""
         return cast(
             dict[str, list[dict[str, Any]]],
-            await self._request(_CIRCLE_MEMBERS_URL_FMT.format(cid=cid)),
+            await self._request(
+                _CIRCLE_MEMBERS_URL_FMT.format(cid=cid), raise_not_modified
+            ),
         )["members"]
 
-    async def get_circle_member(self, cid: str, mid: str) -> dict[str, Any]:
+    async def get_circle_member(
+        self, cid: str, mid: str, *, raise_not_modified: bool = False
+    ) -> dict[str, Any]:
         """Get details for Member as seen from given Circle."""
         return cast(
             dict[str, Any],
-            await self._request(_MEMBER_URL_FMT.format(cid=cid, mid=mid)),
+            await self._request(
+                _MEMBER_URL_FMT.format(cid=cid, mid=mid), raise_not_modified
+            ),
         )
 
     async def _request(
         self,
         url: str,
+        /,
+        raise_not_modified: bool,
         method: str = "get",
         *,
         authorization: str | None = None,
         **kwargs: dict[str, Any],
     ) -> Any:
         """Make a request to server."""
         if authorization is None:
             authorization = self._authorization
         if authorization is None:
             raise LoginError("Must login")
 
         headers = _HEADERS
         if authorization != "":
             headers["authorization"] = authorization
-        if etag := self._etags.get(url):
+        if raise_not_modified and (etag := self._etags.get(url)):
             headers["if-none-match"] = etag
         kwargs.setdefault("headers", {}).update(headers)
 
         for attempt in range(1, self._max_attempts + 1):
             resp: ClientResponse | None = None
             status: int | None = None
             try:
@@ -213,15 +239,15 @@
                     continue
                 # Try to return a useful error message.
                 try:
                     err_msg = cast(
                         Mapping[str, str],
                         await cast(ClientResponse, resp).json(),
                     )["errorMessage"].lower()
-                except (AttributeError, ClientError, JSONDecodeError):
+                except (AttributeError, ClientError, KeyError, JSONDecodeError):
                     err_msg = self._redact(_format_exc(exc), _URL_REDACTIONS)
                 match status:
                     case HTTP_Error.UNAUTHORIZED:
                         authenticate = None
                         with suppress(KeyError):
                             authenticate = cast(
                                 LooseHeaders, cast(ClientResponseError, exc).headers
@@ -248,52 +274,56 @@
             if status == HTTP_Error.NOT_MODIFIED:
                 raise NotModified
             if etag := resp.headers.get("l360-etag"):
                 self._etags[url] = etag
             try:
                 return await resp.json()
             except (ClientError, JSONDecodeError) as exc:
+                try:
+                    resp_ = await resp.text()
+                except ClientError:
+                    resp_ = str(resp)
                 _LOGGER.debug(
                     "While parsing response: %r: %s",
-                    resp,
+                    resp_,
                     self._redact(repr(exc), _EXC_REPR_REDACTIONS),
                 )
                 raise Life360Error(
                     self._redact(_format_exc(exc), _URL_REDACTIONS)
                 ) from None
 
     async def _dump_resp_text(self, resp: ClientResponse | None) -> None:
         """Dump response text to log."""
-        if resp is None or self._verbosity < 2:
+        if resp is None or self.verbosity < 2:
             return
         try:
             if not (text := await resp.text()):
                 return
         except ClientError:
             return
         _LOGGER.debug(
             "resp data: %s",
             self._redact(
                 text,
                 _RESP_TEXT_ALL_REDACTIONS
-                if self._verbosity < 3
+                if self.verbosity < 3
                 else _RESP_TEXT_BASIC_REDACTIONS,
             ),
         )
 
     async def _dump_resp(self, resp: ClientResponse) -> None:
         """Dump response to log."""
-        if self._verbosity < 1:
+        if self.verbosity < 1:
             return
         resp_repr = repr(resp).replace("\n", " ")
         _LOGGER.debug("resp: %s", self._redact(resp_repr, _RESP_REPR_REDACTIONS))
         await self._dump_resp_text(resp)
 
     def _redact(self, string: str, redactions: Iterable[re.Pattern]) -> str:
         """Redact string for lower verbosity levels."""
-        if self._verbosity >= 4:
+        if self.verbosity >= 4:
             return string
         for redaction in redactions:
             while m := redaction.search(string):
                 for i in range(m.lastindex, 0, -1):  # type: ignore[arg-type]
                     string = "REDACTED".join([string[: m.start(i)], string[m.end(i) :]])
         return string
```

### Comparing `life360-7.0.0b0/life360/const.py` & `life360-7.0.0b1/life360/const.py`

 * *Files identical despite different names*

### Comparing `life360-7.0.0b0/life360/exceptions.py` & `life360-7.0.0b1/life360/exceptions.py`

 * *Files identical despite different names*

### Comparing `life360-7.0.0b0/life360.egg-info/PKG-INFO` & `life360-7.0.0b1/life360.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: life360
-Version: 7.0.0b0
+Version: 7.0.0b1
 Summary: Life360 Communications Module
 Home-page: https://github.com/pnbruckner/life360
 Author: Phil Bruckner
 Author-email: pnbruckner@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `life360-7.0.0b0/setup.py` & `life360-7.0.0b1/setup.py`

 * *Files identical despite different names*

