# Comparing `tmp/tesseract_olap-0.9.2.tar.gz` & `tmp/tesseract_olap-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tesseract_olap-0.9.2.tar", max compression
+gzip compressed data, was "tesseract_olap-0.9.3.tar", max compression
```

## Comparing `tesseract_olap-0.9.2.tar` & `tesseract_olap-0.9.3.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     2589 2024-04-03 16:41:13.935447 tesseract_olap-0.9.2/PACKAGE.md
--rw-r--r--   0        0        0     1298 2024-04-03 16:41:13.935447 tesseract_olap-0.9.2/pyproject.toml
--rw-r--r--   0        0        0      478 2024-04-03 16:41:13.935447 tesseract_olap-0.9.2/tesseract_olap/__init__.py
--rw-r--r--   0        0        0      320 2024-04-03 16:41:13.935447 tesseract_olap-0.9.2/tesseract_olap/backend/__init__.py
--rw-r--r--   0        0        0     1806 2024-04-03 16:41:13.935447 tesseract_olap-0.9.2/tesseract_olap/backend/cache.py
--rw-r--r--   0        0        0       79 2024-04-03 16:41:13.935447 tesseract_olap-0.9.2/tesseract_olap/backend/clickhouse/__init__.py
--rw-r--r--   0        0        0     7219 2024-04-03 16:41:13.935447 tesseract_olap-0.9.2/tesseract_olap/backend/clickhouse/backend.py
--rw-r--r--   0        0        0     2714 2024-04-03 16:41:13.935447 tesseract_olap-0.9.2/tesseract_olap/backend/clickhouse/dialect.py
--rw-r--r--   0        0        0    20624 2024-04-03 16:41:13.935447 tesseract_olap-0.9.2/tesseract_olap/backend/clickhouse/sqlbuild.py
--rw-r--r--   0        0        0     3743 2024-04-03 16:41:13.935447 tesseract_olap-0.9.2/tesseract_olap/backend/models.py
--rw-r--r--   0        0        0     2731 2024-04-03 16:41:13.935447 tesseract_olap-0.9.2/tesseract_olap/backend/redis.py
--rw-r--r--   0        0        0      571 2024-04-03 16:41:13.935447 tesseract_olap-0.9.2/tesseract_olap/common/__init__.py
--rw-r--r--   0        0        0     2461 2024-04-03 16:41:13.935447 tesseract_olap-0.9.2/tesseract_olap/common/strings.py
--rw-r--r--   0        0        0      385 2024-04-03 16:41:13.935447 tesseract_olap-0.9.2/tesseract_olap/common/types.py
--rw-r--r--   0        0        0      787 2024-04-03 16:41:13.935447 tesseract_olap-0.9.2/tesseract_olap/exceptions/__init__.py
--rw-r--r--   0        0        0     1596 2024-04-03 16:41:13.935447 tesseract_olap-0.9.2/tesseract_olap/exceptions/backend.py
--rw-r--r--   0        0        0     3461 2024-04-03 16:41:13.935447 tesseract_olap-0.9.2/tesseract_olap/exceptions/query.py
--rw-r--r--   0        0        0     3712 2024-04-03 16:41:13.935447 tesseract_olap-0.9.2/tesseract_olap/exceptions/schema.py
--rw-r--r--   0        0        0      741 2024-04-03 16:41:13.935447 tesseract_olap-0.9.2/tesseract_olap/exceptions/server.py
--rw-r--r--   0        0        0      511 2024-04-03 16:41:13.935447 tesseract_olap-0.9.2/tesseract_olap/logiclayer/__init__.py
--rw-r--r--   0        0        0    10203 2024-04-03 16:41:13.935447 tesseract_olap-0.9.2/tesseract_olap/logiclayer/dependencies.py
--rw-r--r--   0        0        0     5539 2024-04-03 16:41:13.935447 tesseract_olap-0.9.2/tesseract_olap/logiclayer/module.py
--rw-r--r--   0        0        0     4468 2024-04-03 16:41:13.935447 tesseract_olap-0.9.2/tesseract_olap/logiclayer/response.py
--rw-r--r--   0        0        0     1166 2024-04-03 16:41:13.939447 tesseract_olap-0.9.2/tesseract_olap/query/__init__.py
--rw-r--r--   0        0        0     3318 2024-04-03 16:41:13.939447 tesseract_olap-0.9.2/tesseract_olap/query/enums.py
--rw-r--r--   0        0        0    12543 2024-04-03 16:41:13.939447 tesseract_olap-0.9.2/tesseract_olap/query/models.py
--rw-r--r--   0        0        0    12963 2024-04-03 16:41:13.939447 tesseract_olap-0.9.2/tesseract_olap/query/queries.py
--rw-r--r--   0        0        0    10178 2024-04-03 16:41:13.939447 tesseract_olap-0.9.2/tesseract_olap/query/requests.py
--rw-r--r--   0        0        0     1721 2024-04-03 16:41:13.939447 tesseract_olap-0.9.2/tesseract_olap/schema/__init__.py
--rw-r--r--   0        0        0     5432 2024-04-03 16:41:13.939447 tesseract_olap-0.9.2/tesseract_olap/schema/aggregators.py
--rw-r--r--   0        0        0     3587 2024-04-03 16:41:13.939447 tesseract_olap-0.9.2/tesseract_olap/schema/csv.py
--rw-r--r--   0        0        0     4744 2024-04-03 16:41:13.939447 tesseract_olap-0.9.2/tesseract_olap/schema/enums.py
--rw-r--r--   0        0        0     2542 2024-04-03 16:41:13.939447 tesseract_olap-0.9.2/tesseract_olap/schema/json.py
--rw-r--r--   0        0        0     9528 2024-04-03 16:41:13.939447 tesseract_olap-0.9.2/tesseract_olap/schema/models.py
--rw-r--r--   0        0        0    11992 2024-04-03 16:41:13.939447 tesseract_olap-0.9.2/tesseract_olap/schema/parser.py
--rw-r--r--   0        0        0     5184 2024-04-03 16:41:13.939447 tesseract_olap-0.9.2/tesseract_olap/schema/public.py
--rw-r--r--   0        0        0     4824 2024-04-03 16:41:13.939447 tesseract_olap-0.9.2/tesseract_olap/schema/schema.xsd
--rw-r--r--   0        0        0    23758 2024-04-03 16:41:13.939447 tesseract_olap-0.9.2/tesseract_olap/schema/traverse.py
--rw-r--r--   0        0        0    18520 2024-04-03 16:41:13.939447 tesseract_olap-0.9.2/tesseract_olap/schema/xml.py
--rw-r--r--   0        0        0       64 2024-04-03 16:41:13.939447 tesseract_olap-0.9.2/tesseract_olap/server/__init__.py
--rw-r--r--   0        0        0     4674 2024-04-03 16:41:13.939447 tesseract_olap-0.9.2/tesseract_olap/server/schema.py
--rw-r--r--   0        0        0     3542 2024-04-03 16:41:13.939447 tesseract_olap-0.9.2/tesseract_olap/server/server.py
--rw-r--r--   0        0        0     3960 1970-01-01 00:00:00.000000 tesseract_olap-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0     2589 2024-03-15 00:23:52.753141 tesseract_olap-0.9.3/PACKAGE.md
+-rw-r--r--   0        0        0     1320 2024-04-16 19:20:26.872800 tesseract_olap-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0      562 2024-04-16 18:43:02.221430 tesseract_olap-0.9.3/tesseract_olap/__init__.py
+-rw-r--r--   0        0        0      397 2024-04-16 16:46:29.714821 tesseract_olap-0.9.3/tesseract_olap/backend/__init__.py
+-rw-r--r--   0        0        0     2815 2024-04-16 16:46:29.714821 tesseract_olap-0.9.3/tesseract_olap/backend/cache.py
+-rw-r--r--   0        0        0       84 2023-12-12 19:31:05.053659 tesseract_olap-0.9.3/tesseract_olap/backend/clickhouse/__init__.py
+-rw-r--r--   0        0        0     7219 2024-04-03 16:02:12.590243 tesseract_olap-0.9.3/tesseract_olap/backend/clickhouse/backend.py
+-rw-r--r--   0        0        0     2714 2024-03-21 19:13:55.671898 tesseract_olap-0.9.3/tesseract_olap/backend/clickhouse/dialect.py
+-rw-r--r--   0        0        0    20624 2024-04-02 20:13:34.560489 tesseract_olap-0.9.3/tesseract_olap/backend/clickhouse/sqlbuild.py
+-rw-r--r--   0        0        0     3743 2024-04-02 16:29:24.355193 tesseract_olap-0.9.3/tesseract_olap/backend/models.py
+-rw-r--r--   0        0        0     2836 2024-04-16 16:46:29.730422 tesseract_olap-0.9.3/tesseract_olap/backend/valkey.py
+-rw-r--r--   0        0        0      571 2024-04-02 15:44:57.403234 tesseract_olap-0.9.3/tesseract_olap/common/__init__.py
+-rw-r--r--   0        0        0     2461 2024-04-02 17:20:54.212089 tesseract_olap-0.9.3/tesseract_olap/common/strings.py
+-rw-r--r--   0        0        0      399 2023-12-12 19:31:05.137658 tesseract_olap-0.9.3/tesseract_olap/common/types.py
+-rw-r--r--   0        0        0      787 2024-03-28 19:35:52.289762 tesseract_olap-0.9.3/tesseract_olap/exceptions/__init__.py
+-rw-r--r--   0        0        0     1596 2024-04-03 00:40:34.602127 tesseract_olap-0.9.3/tesseract_olap/exceptions/backend.py
+-rw-r--r--   0        0        0     3576 2024-04-16 19:11:41.156439 tesseract_olap-0.9.3/tesseract_olap/exceptions/query.py
+-rw-r--r--   0        0        0     3712 2024-03-28 19:32:15.041429 tesseract_olap-0.9.3/tesseract_olap/exceptions/schema.py
+-rw-r--r--   0        0        0      741 2024-03-28 19:33:42.379457 tesseract_olap-0.9.3/tesseract_olap/exceptions/server.py
+-rw-r--r--   0        0        0      528 2023-12-12 19:31:05.153661 tesseract_olap-0.9.3/tesseract_olap/logiclayer/__init__.py
+-rw-r--r--   0        0        0    11052 2024-04-16 18:30:11.173365 tesseract_olap-0.9.3/tesseract_olap/logiclayer/dependencies.py
+-rw-r--r--   0        0        0     6326 2024-04-16 19:11:28.486182 tesseract_olap-0.9.3/tesseract_olap/logiclayer/module.py
+-rw-r--r--   0        0        0     4477 2024-04-16 18:35:36.963968 tesseract_olap-0.9.3/tesseract_olap/logiclayer/response.py
+-rw-r--r--   0        0        0     1166 2024-04-02 17:32:08.076597 tesseract_olap-0.9.3/tesseract_olap/query/__init__.py
+-rw-r--r--   0        0        0     3318 2024-04-01 21:27:27.862280 tesseract_olap-0.9.3/tesseract_olap/query/enums.py
+-rw-r--r--   0        0        0    12543 2024-04-02 20:23:58.946279 tesseract_olap-0.9.3/tesseract_olap/query/models.py
+-rw-r--r--   0        0        0    13039 2024-04-16 19:09:01.435800 tesseract_olap-0.9.3/tesseract_olap/query/queries.py
+-rw-r--r--   0        0        0    10178 2024-04-02 16:17:50.023716 tesseract_olap-0.9.3/tesseract_olap/query/requests.py
+-rw-r--r--   0        0        0     1763 2024-04-16 18:36:26.257633 tesseract_olap-0.9.3/tesseract_olap/schema/__init__.py
+-rw-r--r--   0        0        0     5432 2024-04-02 15:24:33.879569 tesseract_olap-0.9.3/tesseract_olap/schema/aggregators.py
+-rw-r--r--   0        0        0     3587 2024-03-25 21:23:44.777212 tesseract_olap-0.9.3/tesseract_olap/schema/csv.py
+-rw-r--r--   0        0        0     4744 2024-04-01 20:55:50.142052 tesseract_olap-0.9.3/tesseract_olap/schema/enums.py
+-rw-r--r--   0        0        0     2542 2024-03-14 23:53:07.076800 tesseract_olap-0.9.3/tesseract_olap/schema/json.py
+-rw-r--r--   0        0        0     9528 2024-04-03 00:58:10.522977 tesseract_olap-0.9.3/tesseract_olap/schema/models.py
+-rw-r--r--   0        0        0    11992 2024-04-01 15:57:37.686893 tesseract_olap-0.9.3/tesseract_olap/schema/parser.py
+-rw-r--r--   0        0        0     5306 2024-04-16 18:38:50.208477 tesseract_olap-0.9.3/tesseract_olap/schema/public.py
+-rw-r--r--   0        0        0     4824 2024-03-07 16:34:52.541289 tesseract_olap-0.9.3/tesseract_olap/schema/schema.xsd
+-rw-r--r--   0        0        0    23758 2024-04-16 19:07:35.244865 tesseract_olap-0.9.3/tesseract_olap/schema/traverse.py
+-rw-r--r--   0        0        0    19086 2024-03-28 20:20:53.653136 tesseract_olap-0.9.3/tesseract_olap/schema/xml.py
+-rw-r--r--   0        0        0       64 2024-03-21 21:10:19.073197 tesseract_olap-0.9.3/tesseract_olap/server/__init__.py
+-rw-r--r--   0        0        0     4674 2024-03-28 19:25:27.542934 tesseract_olap-0.9.3/tesseract_olap/server/schema.py
+-rw-r--r--   0        0        0     3713 2024-04-16 16:47:39.771505 tesseract_olap-0.9.3/tesseract_olap/server/server.py
+-rw-r--r--   0        0        0     4003 1970-01-01 00:00:00.000000 tesseract_olap-0.9.3/PKG-INFO
```

### Comparing `tesseract_olap-0.9.2/PACKAGE.md` & `tesseract_olap-0.9.3/PACKAGE.md`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.2/pyproject.toml` & `tesseract_olap-0.9.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tesseract-olap"
-version = "0.9.2"
+version = "0.9.3"
 description = "A simple OLAP library."
 authors = [
   "Francisco Abarzua <francisco@datawheel.us>",
   "Jelmy Hermosilla <jelmy@datawheel.us>",
 ]
 maintainers = [
   "Francisco Abarzua <francisco@datawheel.us>",
@@ -22,25 +22,26 @@
 lxml = "^4.6.0"
 orjson = "^3.9.15"
 polars = "^0.20.0"
 PyPika = ">=0.48.0 <1.0"
 redis = {version="^5.0.0", optional = true}
 typing-extensions = ">=3.7.4"
 xlsxwriter = "^3.2.0"
+lfudacache = "^0.0.2"
 
 [tool.poetry.extras]
 clickhouse = ["clickhouse-driver", "clickhouse-cityhash"]
 redis = ["redis"]
 
 [tool.poetry.group.dev.dependencies]
 clickhouse-cityhash = "^1.0.2.4"
 clickhouse-driver = "^0.2.0"
 fastapi = ">=0.100.0"
 granian = {extras = ["reload"], version = "^1.1.2"}
-logiclayer = "^0.3.0"
+logiclayer = "^0.3.2"
 lxml-stubs = "^0.4.0"
 pytest = "^8.0.0"
 pytest-asyncio = "^0.20.0"
 redis = "^5.0.3"
 ruff = "^0.3.0"
 sqlparse = "^0.4.0"
 tomli = "^2.0.1"
```

### Comparing `tesseract_olap-0.9.2/tesseract_olap/backend/cache.py` & `tesseract_olap-0.9.3/tesseract_olap/backend/cache.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,74 +1,108 @@
-import abc
-from enum import Enum
-from typing import Union
-
-import polars as pl
-
-from tesseract_olap.query import AnyQuery
-
-from .models import Result
-
-CacheConnectionStatus = Enum("CacheConnectionStatus", ["CLOSED", "CONNECTED"])
-
-
-class CacheProvider(abc.ABC):
-    """Base class for the implementation of a cache layer for the Backend."""
-
-    def __repr__(self):
-        return f"{type(self).__name__}"
-
-    @abc.abstractmethod
-    def connect(self) -> "CacheConnection":
-        raise NotImplementedError
-
-
-class CacheConnection(abc.ABC):
-    """Internal Base class for individual connections to the cache layer."""
-
-    @property
-    @abc.abstractmethod
-    def status(self) -> "CacheConnectionStatus":
-        raise NotImplementedError
-
-    @abc.abstractmethod
-    def close(self) -> None:
-        raise NotImplementedError
-
-    @abc.abstractmethod
-    def store(self, query: "AnyQuery", result: "Result[pl.DataFrame]") -> None:
-        raise NotImplementedError
-
-    @abc.abstractmethod
-    def retrieve(self, query: "AnyQuery") -> Union[Result[pl.DataFrame], None]:
-        raise NotImplementedError
-
-    @abc.abstractmethod
-    def ping(self) -> bool:
-        raise NotImplementedError
-
-
-class DummyProvider(CacheProvider):
-    """A CacheProvider used when the user doesn't set a valid one. Will always MISS."""
-
-    def connect(self):
-        return DummyConnection()
-
-
-class DummyConnection(CacheConnection):
-    """The CacheConnection associated to DummyProvider. Will always MISS."""
-
-    @property
-    def status(self):
-        return CacheConnectionStatus.CONNECTED
-
-    def close(self):
-        pass
-
-    def store(self, query: "AnyQuery", result: "Result[pl.DataFrame]"):
-        pass
-
-    def retrieve(self, query: "AnyQuery"):
-        return None
-
-    def ping(self):
-        return True
+import abc
+from enum import Enum
+from typing import Union
+
+import polars as pl
+from lfudacache import LFUDACache
+
+from tesseract_olap.query import AnyQuery
+
+from .models import Result
+
+CacheConnectionStatus = Enum("CacheConnectionStatus", ["CLOSED", "CONNECTED"])
+
+
+class CacheProvider(abc.ABC):
+    """Base class for the implementation of a cache layer for the Backend."""
+
+    def __repr__(self):
+        return f"{type(self).__name__}"
+
+    @abc.abstractmethod
+    def connect(self) -> "CacheConnection":
+        raise NotImplementedError
+
+
+class CacheConnection(abc.ABC):
+    """Internal Base class for individual connections to the cache layer."""
+
+    @property
+    @abc.abstractmethod
+    def status(self) -> "CacheConnectionStatus":
+        raise NotImplementedError
+
+    @abc.abstractmethod
+    def close(self) -> None:
+        raise NotImplementedError
+
+    @abc.abstractmethod
+    def store(self, query: "AnyQuery", result: "Result[pl.DataFrame]") -> None:
+        raise NotImplementedError
+
+    @abc.abstractmethod
+    def retrieve(self, query: "AnyQuery") -> Union["Result[pl.DataFrame]", None]:
+        raise NotImplementedError
+
+    @abc.abstractmethod
+    def ping(self) -> bool:
+        raise NotImplementedError
+
+
+class DummyProvider(CacheProvider):
+    """A CacheProvider used when the user doesn't set a valid one. Will always MISS."""
+
+    def connect(self):
+        return DummyConnection()
+
+
+class DummyConnection(CacheConnection):
+    """The CacheConnection associated to DummyProvider. Will always MISS."""
+
+    @property
+    def status(self):
+        return CacheConnectionStatus.CONNECTED
+
+    def close(self):
+        pass
+
+    def store(self, query: "AnyQuery", result: "Result[pl.DataFrame]"):
+        pass
+
+    def retrieve(self, query: "AnyQuery"):
+        return None
+
+    def ping(self):
+        return True
+
+
+class LfuProvider(CacheProvider):
+    """Stores elements in a dictionary under the Least Frequently Used caching stategy."""
+
+    def __init__(self, maxsize: int = 64) -> None:
+        self.store = LFUDACache(maxsize)
+
+    def connect(self):
+        return LfuConnection(self.store)
+
+
+class LfuConnection(CacheConnection):
+    """The CacheConnection associated to LfuProvider."""
+
+    def __init__(self, store: "LFUDACache") -> None:
+        self.storage = store
+
+    @property
+    def status(self):
+        return CacheConnectionStatus.CONNECTED
+
+    def close(self):
+        pass
+
+    def store(self, query: "AnyQuery", result: "Result[pl.DataFrame]"):
+        self.storage[query.key] = result
+
+    def retrieve(self, query: "AnyQuery") -> Union["Result[pl.DataFrame]", None]:
+        return self.storage.get(query.key)
+
+    def ping(self):
+        return True
```

### Comparing `tesseract_olap-0.9.2/tesseract_olap/backend/clickhouse/backend.py` & `tesseract_olap-0.9.3/tesseract_olap/backend/clickhouse/backend.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.2/tesseract_olap/backend/clickhouse/dialect.py` & `tesseract_olap-0.9.3/tesseract_olap/backend/clickhouse/dialect.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.2/tesseract_olap/backend/clickhouse/sqlbuild.py` & `tesseract_olap-0.9.3/tesseract_olap/backend/clickhouse/sqlbuild.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.2/tesseract_olap/backend/models.py` & `tesseract_olap-0.9.3/tesseract_olap/backend/models.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.2/tesseract_olap/backend/redis.py` & `tesseract_olap-0.9.3/tesseract_olap/backend/valkey.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,75 +1,75 @@
-from io import BytesIO
-from typing import TYPE_CHECKING, Union
-
-import polars as pl
-import redis
-
-from tesseract_olap.backend import Result
-from tesseract_olap.common import hide_dsn_password
-from tesseract_olap.exceptions.backend import UpstreamInternalError, UpstreamNotPrepared
-
-from .cache import CacheConnection, CacheConnectionStatus, CacheProvider
-
-if TYPE_CHECKING:
-    from tesseract_olap.query import AnyQuery
-
-
-class RedisProvider(CacheProvider):
-    def __init__(self, dsn: str, **kwargs):
-        self.dsn = dsn
-        self.pool = redis.ConnectionPool.from_url(dsn, **kwargs)
-
-    def __repr__(self):
-        return f"{type(self).__name__}(dsn='{hide_dsn_password(self.dsn)}')"
-
-    def connect(self):
-        try:
-            return RedisConnection(self.pool, single_connection_client=True)
-        except redis.ConnectionError as exc:
-            raise UpstreamNotPrepared(*exc.args).with_traceback(exc.__traceback__)
-        except redis.RedisError as exc:
-            raise UpstreamInternalError(*exc.args).with_traceback(exc.__traceback__)
-
-
-class RedisConnection(CacheConnection):
-    def __init__(self, pool: redis.ConnectionPool, **kwargs):
-        self.redis = redis.Redis(connection_pool=pool, **kwargs)
-
-    @property
-    def status(self) -> CacheConnectionStatus:
-        return (
-            CacheConnectionStatus.CONNECTED
-            if self.redis.connection is not None and self.redis.ping()
-            else CacheConnectionStatus.CLOSED
-        )
-
-    def close(self) -> None:
-        return self.redis.close()
-
-    def exists(self, query: "AnyQuery") -> bool:
-        return self.redis.exists(query.key) == 1
-
-    def store(self, query: "AnyQuery", result: "Result[pl.DataFrame]") -> None:
-        dfio = result.data.write_ipc(file=None, compression="lz4")
-        try:
-            self.redis.set(query.key, dfio.getvalue())
-        except redis.ConnectionError as exc:
-            raise UpstreamNotPrepared(*exc.args).with_traceback(exc.__traceback__)
-        except redis.RedisError as exc:
-            raise UpstreamInternalError(*exc.args).with_traceback(exc.__traceback__)
-
-    def retrieve(self, query: "AnyQuery") -> Union["Result[pl.DataFrame]", None]:
-        try:
-            res: bytes = self.redis.get(query.key)  # type: ignore
-        except redis.ConnectionError as exc:
-            raise UpstreamNotPrepared(*exc.args).with_traceback(exc.__traceback__)
-        except redis.RedisError as exc:
-            raise UpstreamInternalError(*exc.args).with_traceback(exc.__traceback__)
-
-        if res is None:
-            return None
-
-        return Result(data=pl.read_ipc(BytesIO(res)), columns=query.columns)
-
-    def ping(self) -> bool:
-        return self.redis.ping()  # type: ignore
+from io import BytesIO
+from typing import TYPE_CHECKING, Union
+
+import polars as pl
+import redis as valkey
+
+from tesseract_olap.backend import Result
+from tesseract_olap.common import hide_dsn_password
+from tesseract_olap.exceptions.backend import UpstreamInternalError, UpstreamNotPrepared
+
+from .cache import CacheConnection, CacheConnectionStatus, CacheProvider
+
+if TYPE_CHECKING:
+    from tesseract_olap.query import AnyQuery
+
+
+class ValkeyProvider(CacheProvider):
+    def __init__(self, dsn: str, **kwargs):
+        self.dsn = dsn
+        self.pool = valkey.ConnectionPool.from_url(dsn, **kwargs)
+
+    def __repr__(self):
+        return f"{type(self).__name__}(dsn='{hide_dsn_password(self.dsn)}')"
+
+    def connect(self):
+        try:
+            return ValkeyConnection(self.pool, single_connection_client=True)
+        except valkey.ConnectionError as exc:
+            raise UpstreamNotPrepared(*exc.args).with_traceback(exc.__traceback__)
+        except valkey.RedisError as exc:
+            raise UpstreamInternalError(*exc.args).with_traceback(exc.__traceback__)
+
+
+class ValkeyConnection(CacheConnection):
+    def __init__(self, pool: valkey.ConnectionPool, **kwargs):
+        self.valkey = valkey.Redis(connection_pool=pool, **kwargs)
+
+    @property
+    def status(self) -> CacheConnectionStatus:
+        return (
+            CacheConnectionStatus.CONNECTED
+            if self.valkey.connection is not None and self.valkey.ping()
+            else CacheConnectionStatus.CLOSED
+        )
+
+    def close(self) -> None:
+        return self.valkey.close()
+
+    def exists(self, query: "AnyQuery") -> bool:
+        return self.valkey.exists(query.key) == 1
+
+    def store(self, query: "AnyQuery", result: "Result[pl.DataFrame]") -> None:
+        dfio = result.data.write_ipc(file=None, compression="lz4")
+        try:
+            self.valkey.set(query.key, dfio.getvalue())
+        except valkey.ConnectionError as exc:
+            raise UpstreamNotPrepared(*exc.args).with_traceback(exc.__traceback__)
+        except valkey.RedisError as exc:
+            raise UpstreamInternalError(*exc.args).with_traceback(exc.__traceback__)
+
+    def retrieve(self, query: "AnyQuery") -> Union["Result[pl.DataFrame]", None]:
+        try:
+            res: bytes = self.valkey.get(query.key)  # type: ignore
+        except valkey.ConnectionError as exc:
+            raise UpstreamNotPrepared(*exc.args).with_traceback(exc.__traceback__)
+        except valkey.RedisError as exc:
+            raise UpstreamInternalError(*exc.args).with_traceback(exc.__traceback__)
+
+        if res is None:
+            return None
+
+        return Result(data=pl.read_ipc(BytesIO(res)), columns=query.columns)
+
+    def ping(self) -> bool:
+        return self.valkey.ping()  # type: ignore
```

### Comparing `tesseract_olap-0.9.2/tesseract_olap/common/__init__.py` & `tesseract_olap-0.9.3/tesseract_olap/common/__init__.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.2/tesseract_olap/common/strings.py` & `tesseract_olap-0.9.3/tesseract_olap/common/strings.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.2/tesseract_olap/exceptions/__init__.py` & `tesseract_olap-0.9.3/tesseract_olap/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.2/tesseract_olap/exceptions/backend.py` & `tesseract_olap-0.9.3/tesseract_olap/exceptions/backend.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.2/tesseract_olap/exceptions/query.py` & `tesseract_olap-0.9.3/tesseract_olap/exceptions/query.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Query exceptions module.
 
 The errors in this module refer to problems during the retrieval of data from
 the backend, but happening at the core side of the code.
 """
 
-from typing import Optional
+from typing import Iterable, Optional
 
 from tesseract_olap.common import Array
 
 from . import QueryError
 
 
 class InvalidQuery(QueryError):
@@ -100,9 +100,11 @@
     requested parameters.
 
     Should be raised before the query is executed against the upstream server.
     """
 
     code = 403
 
-    def __init__(self) -> None:
-        super().__init__("Request doesn't count with the necessary permissions.")
+    def __init__(self, resource: str, roles: Iterable[str]) -> None:
+        super().__init__("You don't have authorization to access this resource.")
+        self.resource = resource
+        self.request_roles = roles
```

### Comparing `tesseract_olap-0.9.2/tesseract_olap/exceptions/schema.py` & `tesseract_olap-0.9.3/tesseract_olap/exceptions/schema.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.2/tesseract_olap/exceptions/server.py` & `tesseract_olap-0.9.3/tesseract_olap/exceptions/server.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.2/tesseract_olap/logiclayer/dependencies.py` & `tesseract_olap-0.9.3/tesseract_olap/logiclayer/dependencies.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Dict, List, Optional, Set, Tuple, Union
 
-from fastapi import Depends, Query, Request
+from fastapi import Depends, Header, Query, Request
+from logiclayer import AuthToken, AuthTokenType
 from typing_extensions import Annotated, Literal
 
 from tesseract_olap.common import FALSEY_STRINGS, TRUTHY_STRINGS
 from tesseract_olap.query import (
     AnyOrder,
     DataRequest,
     DataRequestParams,
@@ -16,14 +17,34 @@
 SingleFilterCondition = Tuple[NumericConstraint]
 DoubleFilterCondition = Tuple[
     NumericConstraint, Literal["and", "or"], NumericConstraint
 ]
 FilterCondition = Union[SingleFilterCondition, DoubleFilterCondition]
 
 
+def auth_token(
+    header_auth: Annotated[Optional[str], Header(alias="authorization")] = None,
+    header_jwt: Annotated[Optional[str], Header(alias="x-tesseract-jwt")] = None,
+    query_token: Annotated[Optional[str], Query(alias="token")] = None,
+):
+    if header_jwt:
+        return AuthToken(AuthTokenType.JWTOKEN, header_jwt)
+    if query_token:
+        return AuthToken(AuthTokenType.APIKEY, query_token)
+    if header_auth:
+        if header_auth.startswith("Bearer "):
+            return AuthToken(AuthTokenType.JWTOKEN, header_auth[7:])
+        if header_auth.startswith("Basic "):
+            return AuthToken(AuthTokenType.BASIC, header_auth[6:])
+        if header_auth.startswith("Digest "):
+            return AuthToken(AuthTokenType.DIGEST, header_auth[7:])
+
+    return None
+
+
 def query_cuts_include(
     request: Request,
     include: Annotated[
         str,
         Query(
             description="""\
 Specifies which values should be considered for the aggregation.
```

### Comparing `tesseract_olap-0.9.2/tesseract_olap/logiclayer/module.py` & `tesseract_olap-0.9.3/tesseract_olap/logiclayer/module.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,24 +6,25 @@
 
 import dataclasses
 import os
 from pathlib import Path
 from typing import Optional, Union
 
 import logiclayer as ll
-from fastapi import Depends, HTTPException, Request, status
+from fastapi import Depends, Request
 from fastapi.responses import JSONResponse, RedirectResponse
 
 from tesseract_olap import __version__ as tesseract_version
 from tesseract_olap.exceptions import QueryError, TesseractError
+from tesseract_olap.exceptions.query import NotAuthorized
 from tesseract_olap.query import DataQuery, DataRequest, MembersQuery, MembersRequest
-from tesseract_olap.schema import PublicCube, PublicSchema
+from tesseract_olap.schema import TesseractCube, TesseractSchema
 from tesseract_olap.server import OlapServer
 
-from .dependencies import dataquery_params, membersquery_params
+from .dependencies import auth_token, dataquery_params, membersquery_params
 from .response import (
     MembersResModel,
     ResponseFormat,
     StatusResModel,
     data_response,
     members_response,
 )
@@ -77,70 +78,84 @@
             version=tesseract_version,
         )
 
     @ll.route("GET", "/cubes", name="public_schema")
     def public_schema(
         self,
         locale: Optional[str] = None,
-    ) -> PublicSchema:
+        token: Optional[ll.AuthToken] = Depends(auth_token),
+    ) -> TesseractSchema:
         """Returns the public schema with all the available cubes."""
-        roles = []
-        return PublicSchema.from_entity(self.server.schema, roles=roles, locale=locale)
+        roles = self.auth.get_roles(token)
+        return TesseractSchema.from_entity(
+            self.server.schema, roles=roles, locale=locale
+        )
 
     @ll.route("GET", "/cubes/{cube_name}", name="public_schema_cube")
     def public_schema_cube(
         self,
         cube_name: str,
         locale: Optional[str] = None,
-    ) -> PublicCube:
+        token: Optional[ll.AuthToken] = Depends(auth_token),
+    ) -> TesseractCube:
         """Returns the public schema for the single specified cube."""
-        roles = []
+        roles = self.auth.get_roles(token)
         cube = self.server.schema.get_cube(cube_name)
         if not cube.is_authorized(roles):
-            raise HTTPException(
-                status.HTTP_403_FORBIDDEN,
-                "You don't have authorization to access this cube. "
-                "Check your credentials and try again.",
-            )
+            raise NotAuthorized(f"Cube({cube})", roles)
         locale = self.server.schema.default_locale if locale is None else locale
-        return PublicCube.from_entity(cube, locale=locale)
+        return TesseractCube.from_entity(cube, locale=locale)
 
     @ll.route("GET", "/data", name="redirect_data", response_class=RedirectResponse)
     def query_data_redirect(self, request: Request):
         """Redirects the request to the canonical endpoint in jsonrecords format."""
         return f"{request.url.path}.jsonrecords?{request.url.query}"
 
     @ll.route("GET", "/data.{extension}", name="route_data")
     def query_data(
         self,
         extension: ResponseFormat,
         params: DataRequest = Depends(dataquery_params),
+        token: Optional[ll.AuthToken] = Depends(auth_token),
     ):
         """Executes a request for data from the server."""
+        params.roles = self.auth.get_roles(token)
         query = DataQuery.from_request(self.server.schema, params)
         with self.server.session() as session:
             result = session.fetch_dataframe(query)
         return data_response(params, query, result, extension)
 
     @ll.route("GET", "/members", name="route_members")
     def query_members(
         self,
         params: MembersRequest = Depends(membersquery_params),
+        token: Optional[ll.AuthToken] = Depends(auth_token),
     ) -> MembersResModel:
         """Executes a request for the members of a level."""
+        params.roles = self.auth.get_roles(token)
         query = MembersQuery.from_request(self.server.schema, params)
         with self.server.session() as session:
             result = session.fetch_records(query)
         return members_response(params, query, result)
 
     @ll.route("GET", "/debug/schema", debug=True)
     def debug_schema(self):
         """Returns the true internal schema, used to validate the requests."""
         return dataclasses.asdict(self.server.raw_schema)
 
     @ll.exception_handler(TesseractError)
     def exc_tesseracterror(self, request: Request, exc: TesseractError):
+        if isinstance(exc, NotAuthorized):
+            if self.debug:
+                detail = (
+                    f"Requested resource '{exc.resource}' is not allowed for the roles "
+                    f"provided by authorization credentials: '{', '.join(exc.request_roles)}'"
+                )
+                content = {"error": True, "type": "NotAuthorized", "detail": detail}
+            else:
+                content = {"error": True, "detail": exc.message}
+
         if self.debug or isinstance(exc, QueryError):
             content = {"error": True, "type": type(exc).__name__, "detail": exc.message}
         else:
             content = {"error": True, "detail": "Backend error"}
         return JSONResponse(content, status_code=exc.code)
```

### Comparing `tesseract_olap-0.9.2/tesseract_olap/logiclayer/response.py` & `tesseract_olap-0.9.3/tesseract_olap/logiclayer/response.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from fastapi.responses import FileResponse, Response
 from starlette.background import BackgroundTask
 from typing_extensions import Literal
 
 from tesseract_olap.backend import Result
 from tesseract_olap.common import AnyDict
 from tesseract_olap.query import DataQuery, DataRequest, MembersQuery, MembersRequest
-from tesseract_olap.schema import Annotations, MemberType, PublicProperty
+from tesseract_olap.schema import Annotations, MemberType, TesseractProperty
 
 
 class ResponseFormat(str, Enum):
     csv = "csv"
     excel = "xlsx"
     jsonarrays = "jsonarrays"
     jsonrecords = "jsonrecords"
@@ -46,15 +46,15 @@
 
 @dataclass(eq=False, order=False)
 class MembersResModel:
     name: str
     caption: str
     depth: int
     annotations: Annotations
-    properties: List["PublicProperty"]
+    properties: List["TesseractProperty"]
     dtypes: Mapping[str, MemberType]
     members: List[AnyDict]
 
 
 def data_response(
     params: DataRequest,
     query: DataQuery,
@@ -112,15 +112,15 @@
 
     return MembersResModel(
         name=level.name,
         caption=level.get_caption(locale),
         depth=level.depth,
         annotations=dict(level.annotations),
         properties=[
-            PublicProperty.from_entity(item, locale) for item in level.properties
+            TesseractProperty.from_entity(item, locale) for item in level.properties
         ],
         dtypes=result.columns,
         members=[nest_keys(row) for row in result.data]
         if with_parents
         else result.data,
     )
```

### Comparing `tesseract_olap-0.9.2/tesseract_olap/query/__init__.py` & `tesseract_olap-0.9.3/tesseract_olap/query/__init__.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.2/tesseract_olap/query/enums.py` & `tesseract_olap-0.9.3/tesseract_olap/query/enums.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.2/tesseract_olap/query/models.py` & `tesseract_olap-0.9.3/tesseract_olap/query/models.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.2/tesseract_olap/query/queries.py` & `tesseract_olap-0.9.3/tesseract_olap/query/queries.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,15 @@
         """Generates a new :class:`Query` instance from the parameters defined
         in a :class:`DataRequest` object.
 
         If any of the parameters can't be found on the Schema, raises a derivate
         of the :class:`InvalidQuery` error.
         """
         if not schema.is_authorized(request):
-            raise NotAuthorized()
+            raise NotAuthorized(f"Cube({request.cube})", request.roles)
 
         cube = schema.get_cube(request.cube)
 
         return cls(
             cube=cube,
             fields_qualitative=_get_data_hierarfields(cube, request),
             fields_quantitative=_get_data_measurefields(cube, request),
@@ -165,15 +165,15 @@
 
     @classmethod
     def from_request(cls, schema: "SchemaTraverser", request: "MembersRequest"):
         """Generates a new :class:`MembersQuery` instance from a user-provided
         :class:`MembersRequest` instance.
         """
         if not schema.is_authorized(request):
-            raise NotAuthorized()
+            raise NotAuthorized(f"Cube({request.cube})", request.roles)
 
         cube = schema.get_cube(request.cube)
 
         return cls(
             cube=cube,
             hiefield=_get_members_hierarfield(cube, request),
             locale=schema.default_locale if request.locale is None else request.locale,
```

### Comparing `tesseract_olap-0.9.2/tesseract_olap/query/requests.py` & `tesseract_olap-0.9.3/tesseract_olap/query/requests.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.2/tesseract_olap/schema/__init__.py` & `tesseract_olap-0.9.3/tesseract_olap/schema/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,21 +20,21 @@
     Property,
     PropertyUsage,
     Schema,
     Table,
 )
 from .parser import Interpreter, Lexer, Parser
 from .public import (
-    PublicCube,
-    PublicDimension,
-    PublicHierarchy,
-    PublicLevel,
-    PublicMeasure,
-    PublicProperty,
-    PublicSchema,
+    TesseractCube,
+    TesseractDimension,
+    TesseractHierarchy,
+    TesseractLevel,
+    TesseractMeasure,
+    TesseractProperty,
+    TesseractSchema,
 )
 from .traverse import (
     ColumnEntity,
     CubeTraverser,
     DimensionTraverser,
     HierarchyTraverser,
     LevelTraverser,
@@ -72,18 +72,18 @@
     "parse_csv_schema",
     "parse_json_schema",
     "parse_xml_schema",
     "Parser",
     "Property",
     "PropertyTraverser",
     "PropertyUsage",
-    "PublicCube",
-    "PublicDimension",
-    "PublicHierarchy",
-    "PublicLevel",
-    "PublicMeasure",
-    "PublicProperty",
-    "PublicSchema",
     "Schema",
     "SchemaTraverser",
     "Table",
+    "TesseractCube",
+    "TesseractDimension",
+    "TesseractHierarchy",
+    "TesseractLevel",
+    "TesseractMeasure",
+    "TesseractProperty",
+    "TesseractSchema",
 )
```

### Comparing `tesseract_olap-0.9.2/tesseract_olap/schema/aggregators.py` & `tesseract_olap-0.9.3/tesseract_olap/schema/aggregators.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.2/tesseract_olap/schema/csv.py` & `tesseract_olap-0.9.3/tesseract_olap/schema/csv.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.2/tesseract_olap/schema/enums.py` & `tesseract_olap-0.9.3/tesseract_olap/schema/enums.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.2/tesseract_olap/schema/json.py` & `tesseract_olap-0.9.3/tesseract_olap/schema/json.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.2/tesseract_olap/schema/models.py` & `tesseract_olap-0.9.3/tesseract_olap/schema/models.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.2/tesseract_olap/schema/parser.py` & `tesseract_olap-0.9.3/tesseract_olap/schema/parser.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.2/tesseract_olap/schema/public.py` & `tesseract_olap-0.9.3/tesseract_olap/schema/public.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,79 +1,80 @@
 from dataclasses import dataclass
 from functools import lru_cache
-from typing import List, Optional
+from typing import Iterable, List, Optional
 
 from . import traverse
 from .enums import DimensionType, MemberType
 from .models import Annotations
 
 
 @dataclass(eq=False, frozen=True, order=False)
-class PublicSchema:
+class TesseractSchema:
     name: str
     locales: List[str]
     default_locale: str
     annotations: Annotations
-    cubes: List["PublicCube"]
+    cubes: List["TesseractCube"]
 
     @classmethod
     def from_entity(
         cls,
         entity: traverse.SchemaTraverser,
-        roles: List[str] = [],
+        roles: Iterable[str] = [],
         locale: Optional[str] = None,
     ):
         """Generates a dataclass-schema object describing this entity."""
         default_locale = entity.schema.default_locale
         locale = default_locale if locale is None else locale
         return cls(
             name=entity.schema.name,
             locales=sorted(entity.get_locale_available()),
             default_locale=default_locale,
             cubes=[
-                PublicCube.from_entity(item, locale)
+                TesseractCube.from_entity(item, locale)
                 for item in entity.cube_map.values()
                 if item.visible and item.is_authorized(roles)
             ],
             annotations=dict(entity.schema.annotations),
         )
 
 
 @dataclass(eq=False, frozen=True, order=False)
-class PublicCube:
+class TesseractCube:
     name: str
     caption: str
     annotations: Annotations
-    dimensions: List["PublicDimension"]
-    measures: List["PublicMeasure"]
+    dimensions: List["TesseractDimension"]
+    measures: List["TesseractMeasure"]
 
     @classmethod
     @lru_cache(maxsize=256)
     def from_entity(cls, entity: traverse.CubeTraverser, locale: str):
         """Generates a dataclass-schema object describing this entity."""
         return cls(
             name=entity.name,
             caption=entity.get_caption(locale),
             dimensions=[
-                PublicDimension.from_entity(item, locale) for item in entity.dimensions
+                TesseractDimension.from_entity(item, locale)
+                for item in entity.dimensions
             ],
             measures=[
-                PublicMeasure.from_entity(item, locale) for item in entity.measures
+                TesseractMeasure.from_entity(item, locale) for item in entity.measures
             ],
             annotations=dict(entity.annotations),
         )
 
 
 @dataclass(eq=False, frozen=True, order=False)
-class PublicMeasure:
+class TesseractMeasure:
     name: str
     caption: str
     aggregator: str
     annotations: Annotations
-    attached: List["PublicMeasure"]
+    attached: List["TesseractMeasure"]
 
     @classmethod
     def from_entity(cls, entity: traverse.AnyMeasure, locale: str):
         """Generates a dataclass-schema object describing this entity."""
         return cls(
             name=entity.name,
             caption=entity.get_caption(locale),
@@ -82,79 +83,81 @@
             attached=[
                 cls.from_entity(item, locale) for item in entity.submeasures.values()
             ],
         )
 
 
 @dataclass(eq=False, frozen=True, order=False)
-class PublicDimension:
+class TesseractDimension:
     name: str
     caption: str
     type: DimensionType
     annotations: Annotations
-    hierarchies: List["PublicHierarchy"]
+    hierarchies: List["TesseractHierarchy"]
     default_hierarchy: str
 
     @classmethod
     def from_entity(cls, entity: traverse.DimensionTraverser, locale: str):
         """Generates a dataclass-schema object describing this entity."""
         return cls(
             name=entity.name,
             caption=entity.get_caption(locale),
             type=entity.dim_type,
             annotations=dict(entity.annotations),
             hierarchies=[
-                PublicHierarchy.from_entity(item, locale) for item in entity.hierarchies
+                TesseractHierarchy.from_entity(item, locale)
+                for item in entity.hierarchies
             ],
             default_hierarchy=entity._entity.default_hierarchy,
         )
 
 
 @dataclass(eq=False, frozen=True, order=False)
-class PublicHierarchy:
+class TesseractHierarchy:
     name: str
     caption: str
     annotations: Annotations
-    levels: List["PublicLevel"]
+    levels: List["TesseractLevel"]
 
     @classmethod
     def from_entity(cls, entity: traverse.HierarchyTraverser, locale: str):
         """Generates a dataclass-schema object describing this entity."""
         return cls(
             name=entity.name,
             caption=entity.get_caption(locale),
             annotations=dict(entity.annotations),
-            levels=[PublicLevel.from_entity(item, locale) for item in entity.levels],
+            levels=[TesseractLevel.from_entity(item, locale) for item in entity.levels],
         )
 
 
 @dataclass(eq=False, frozen=True, order=False)
-class PublicLevel:
+class TesseractLevel:
     name: str
     caption: str
     depth: int
     annotations: Annotations
-    properties: List["PublicProperty"]
+    properties: List["TesseractProperty"]
 
     @classmethod
     def from_entity(cls, entity: traverse.LevelTraverser, locale: str):
         """Generates a dataclass-schema object describing this entity."""
         return cls(
             name=entity.name,
             caption=entity.get_caption(locale),
             depth=entity.depth,
             annotations=dict(entity.annotations),
             properties=[
-                PublicProperty.from_entity(item, locale) for item in entity.properties
+                TesseractProperty.from_entity(item, locale)
+                for item in entity.properties
             ],
         )
 
 
 @dataclass(eq=False, frozen=True, order=False)
-class PublicProperty:
+class TesseractProperty:
     name: str
     caption: str
     type: MemberType
     annotations: Annotations
 
     @classmethod
     def from_entity(cls, entity: traverse.PropertyTraverser, locale: str):
```

### Comparing `tesseract_olap-0.9.2/tesseract_olap/schema/schema.xsd` & `tesseract_olap-0.9.3/tesseract_olap/schema/schema.xsd`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.2/tesseract_olap/schema/traverse.py` & `tesseract_olap-0.9.3/tesseract_olap/schema/traverse.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.2/tesseract_olap/schema/xml.py` & `tesseract_olap-0.9.3/tesseract_olap/schema/xml.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,566 +1,566 @@
-"""XML Schema parsing module
-
-Defines subclasses for the core Entity classes, parsed from an XML document.
-"""
-
-import logging
-from ast import literal_eval as eval_tuple
-from collections import OrderedDict
-from pathlib import Path
-from typing import (
-    Generator,
-    Iterable,
-    List,
-    Optional,
-    TextIO,
-    Tuple,
-    Type,
-    TypeVar,
-    Union,
-)
-
-import immutables as immu
-from lxml import etree
-
-from tesseract_olap.common import is_numeric, numerify
-from tesseract_olap.exceptions.schema import (
-    InvalidXMLAttributeValue,
-    MissingXMLAttribute,
-    MissingXMLNode,
-)
-
-from . import models
-from .aggregators import Aggregator
-from .csv import parse_csv
-from .enums import AggregatorType, DimensionType, MemberType
-
-logger = logging.getLogger(__name__)
-
-XMLEntity = Union[
-    "XMLSharedDimension",
-    "XMLHierarchy",
-    "XMLLevel",
-    "XMLProperty",
-    "XMLInlineTable",
-    "XMLCube",
-    "XMLDimensionUsage",
-    "XMLHierarchyUsage",
-    "XMLLevelUsage",
-    "XMLPropertyUsage",
-    "XMLPrivateDimension",
-    "XMLMeasure",
-    "XMLCalculatedMeasure",
-]
-
-AnyXMLEntity = TypeVar("AnyXMLEntity", bound=XMLEntity)
-
-
-class XMLSchema(models.Schema):
-    tag = "Schema"
-
-    @classmethod
-    def parse(cls, node: etree._Element, index: int = 0):
-        """Parse a <Schema> XML node."""
-        name = _get_attr(node, "name")
-        logger.debug("Parsing node <%s name='%s' />", cls.tag, name)
-
-        cube_gen = _yield_children_nodes(node, XMLCube)
-        shareddim_gen = _yield_children_nodes(node, XMLSharedDimension)
-        sharedtbl_gen = _yield_children_nodes(node, XMLInlineTable)
-
-        return cls(
-            name=name,
-            cube_map=OrderedDict(cube_gen),
-            shared_dimension_map=immu.Map(shareddim_gen),
-            shared_table_map=immu.Map(sharedtbl_gen),
-            default_locale=node.get("default_locale", "xx"),
-            annotations=immu.Map(_yield_annotations(node)),
-        )
-
-
-class XMLAccessControl(models.AccessControl):
-    tag = "Access"
-
-    @classmethod
-    def parse(cls, node: etree._Element):
-        """Parse all <Access> XML node that are directly under this node."""
-
-        rules_gen = (
-            (role, _get_attr(item, "rule") == "allow")
-            for item in node.iterchildren(cls.tag)
-            for role in _get_attr(item, "roles").split(",")
-        )
-
-        return cls(
-            public=node.get("public", "true") == "true",
-            rules=immu.Map(rules_gen),
-        )
-
-
-class XMLCube(models.Cube):
-    tag = "Cube"
-
-    @classmethod
-    def parse(cls, node: etree._Element, index: int):
-        """Parse a <Cube> XML node."""
-        name = _get_attr(node, "name")
-        logger.debug("Parsing node <%s name='%s' />", cls.tag, name)
-
-        table = _find_table_ref(node)
-        if table is None:
-            raise MissingXMLNode(node.tag, name, "Table")
-
-        dimension_map = OrderedDict(
-            _yield_children_nodes(node, XMLPrivateDimension, XMLDimensionUsage)
-        )
-        if len(dimension_map) == 0:
-            raise MissingXMLNode(node.tag, name, "Dimension")
-
-        measure_map = OrderedDict(
-            _yield_children_nodes(node, XMLMeasure, XMLCalculatedMeasure)
-        )
-        if len(measure_map) == 0:
-            raise MissingXMLNode(node.tag, name, "Measure")
-
-        return cls(
-            name=name,
-            captions=immu.Map(_yield_locale_pairs(node, "caption")),
-            acl=XMLAccessControl.parse(node),
-            dimension_map=dimension_map,
-            measure_map=measure_map,
-            table=table,
-            annotations=immu.Map(_yield_annotations(node)),
-            subset_table=node.get("subset_table", "false").lower() != "false",
-            visible=node.get("visible", "true").lower() != "false",
-        )
-
-
-class XMLDimensionUsage(models.DimensionUsage):
-    tag = "DimensionUsage"
-
-    @classmethod
-    def parse(cls, node: etree._Element, index: int):
-        """Parse a <DimensionUsage> XML node."""
-        name = _get_attr(node, "name")
-        logger.debug("Parsing node <%s name='%s' />", cls.tag, name)
-
-        return cls(
-            name=name,
-            source=_get_attr(node, "source"),
-            foreign_key=_get_attr(node, "foreign_key"),
-            annotations=immu.Map(_yield_annotations(node)),
-            captions=immu.Map(_yield_locale_pairs(node, "caption")),
-            hierarchy_map=OrderedDict(
-                _yield_children_nodes(node, XMLHierarchyUsage, attr="source")
-            ),
-        )
-
-
-class XMLHierarchyUsage(models.HierarchyUsage):
-    tag = "HierarchyUsage"
-
-    @classmethod
-    def parse(cls, node: etree._Element, index: int):
-        """Parse a <HierarchyUsage> XML node."""
-        name = _get_attr(node, "name")
-        logger.debug("Parsing node <%s name='%s' />", cls.tag, name)
-
-        return cls(
-            name=name,
-            source=_get_attr(node, "source"),
-            annotations=immu.Map(_yield_annotations(node)),
-            captions=immu.Map(_yield_locale_pairs(node, "caption")),
-            level_map=OrderedDict(
-                _yield_children_nodes(node, XMLLevelUsage, attr="source")
-            ),
-        )
-
-
-class XMLLevelUsage(models.LevelUsage):
-    tag = "LevelUsage"
-
-    @classmethod
-    def parse(cls, node: etree._Element, index: int):
-        """Parse a <LevelUsage> XML node."""
-        name = _get_attr(node, "name")
-        logger.debug("Parsing node <%s name='%s' />", cls.tag, name)
-
-        return cls(
-            name=name,
-            source=_get_attr(node, "source"),
-            annotations=immu.Map(_yield_annotations(node)),
-            captions=immu.Map(_yield_locale_pairs(node, "caption")),
-            property_map=OrderedDict(
-                _yield_children_nodes(node, XMLPropertyUsage, attr="source")
-            ),
-        )
-
-
-class XMLPropertyUsage(models.PropertyUsage):
-    tag = "PropertyUsage"
-
-    @classmethod
-    def parse(cls, node: etree._Element, index: int):
-        """Parse a <PropertyUsage> XML node."""
-        name = _get_attr(node, "name")
-        logger.debug("Parsing node <%s name='%s' />", cls.tag, name)
-
-        return cls(
-            name=name,
-            source=_get_attr(node, "source"),
-            annotations=immu.Map(_yield_annotations(node)),
-            captions=immu.Map(_yield_locale_pairs(node, "caption")),
-        )
-
-
-class XMLTable(models.Table):
-    tag = "Table"
-
-    @classmethod
-    def parse(cls, node: etree._Element, index: int):
-        """Parse a <Table> XML node."""
-        name = _get_attr(node, "name")
-        logger.debug("Parsing node <%s name='%s' />", cls.tag, name)
-
-        return cls(
-            name=name,
-            schema=node.get("schema"),
-            primary_key=node.get("primary_key", "id"),
-        )
-
-
-class XMLInlineTable(models.InlineTable):
-    tag = "InlineTable"
-
-    @classmethod
-    def parse(cls, node: etree._Element, index: int):
-        """Parse a <InlineTable> XML node."""
-        name = _get_attr(node, "name")
-        logger.debug("Parsing node <%s name='%s' />", cls.tag, name)
-
-        node_format = _get_attr(node, "format")
-
-        if node_format == "csv":
-            node_format = "text/csv"
-
-        if node_format == "tuples":
-            headers, rows = cls.parse_tuples(node)
-        elif node_format.startswith("text/csv"):
-            content = [] if node.text is None else node.text.strip().splitlines()
-            headers, *rows = parse_csv(content, mimetype=node_format)
-            headers = tuple(str(item) for item in headers)
-        else:
-            raise InvalidXMLAttributeValue(node.tag, name, "format", node_format)
-
-        return cls(
-            name=name,
-            headers=headers,
-            types=cls.infer_types(rows),
-            rows=rows,
-        )
-
-    @staticmethod
-    def parse_tuples(
-        node: etree._Element,
-    ) -> Tuple[Tuple[str, ...], List[Tuple[Union[str, float], ...]]]:
-        """Parse the child nodes from an InlineTable with `tuples` format."""
-        try:
-            # try parsing literal tuples with ast.eval()
-            children: List[Tuple[Union[str, float], ...]] = [
-                eval_tuple(line)
-                for line in (item.text for item in node.iterchildren("Row"))
-                if line
-            ]
-        except SyntaxError:
-            # Python `tuples` looks similar to CSV, so let's try with it
-            row_iter = (
-                line[1:-1] if line.startswith("(") and line.endswith(")") else line
-                for line in (item.text for item in node.iterchildren("Row"))
-                if line is not None
-            )
-            children = parse_csv(row_iter, skipinitialspace=True)
-        # at least 2 rows must be present: a header list and a data row
-        if len(children) < 2:
-            raise MissingXMLNode(node.tag, _get_attr(node, "name"), "Row")
-        headers = tuple(str(item) for item in children[0])
-        return headers, children[1:]
-
-
-class XMLSharedDimension(models.Dimension):
-    tag = "SharedDimension"
-
-    @classmethod
-    def parse(cls, node: etree._Element, index: int):
-        """Parse a Shared <Dimension> XML node."""
-        name = _get_attr(node, "name")
-        logger.debug("Parsing node <%s name='%s' />", cls.tag, name)
-
-        dim_type = node.get("type")
-
-        hierarchy_map = OrderedDict(_yield_children_nodes(node, XMLHierarchy))
-
-        default_hierarchy = node.get("default_hierarchy")
-        if default_hierarchy not in hierarchy_map:
-            default_hierarchy = next(iter(hierarchy_map.keys()))
-
-        return cls(
-            name=name,
-            captions=immu.Map(_yield_locale_pairs(node, "caption")),
-            default_hierarchy=default_hierarchy,
-            dim_type=DimensionType.from_str(dim_type),
-            foreign_key=node.get("foreign_key"),
-            hierarchy_map=hierarchy_map,
-            annotations=immu.Map(_yield_annotations(node)),
-        )
-
-
-class XMLPrivateDimension(models.Dimension):
-    tag = "Dimension"
-
-    @classmethod
-    def parse(cls, node: etree._Element, index: int):
-        """Parse a Private <Dimension> XML node."""
-        dimension: cls = XMLSharedDimension.parse.__func__(cls, node, index)
-
-        # foreign keys are required in Private Dimensions
-        if dimension.foreign_key is None:
-            raise MissingXMLAttribute(node.tag, "foreign_key")
-
-        return dimension
-
-
-class XMLHierarchy(models.Hierarchy):
-    tag = "Hierarchy"
-
-    @classmethod
-    def parse(cls, node: etree._Element, index: int):
-        """Parse a <Hierarchy> XML node."""
-        name = _get_attr(node, "name")
-        logger.debug("Parsing node <%s name='%s' />", cls.tag, name)
-
-        level_map = OrderedDict(_yield_children_nodes(node, XMLLevel))
-        if len(level_map) == 0:
-            raise MissingXMLNode(node.tag, name, "Level")
-
-        default_pk = ""
-        for item in level_map.values():
-            default_pk = item.key_column
-
-        return cls(
-            name=name,
-            primary_key=node.get("primary_key", default_pk),
-            captions=immu.Map(_yield_locale_pairs(node, "caption")),
-            table=_find_table_ref(node),
-            level_map=level_map,
-            default_member=cls._parse_default_member(node),
-            annotations=immu.Map(_yield_annotations(node)),
-        )
-
-    @staticmethod
-    def _parse_default_member(node: etree._Element):
-        items: List[str] = node.get("default_member", "").split(".", maxsplit=1)
-        return (items[0], items[1]) if len(items) == 2 else None
-
-
-class XMLLevel(models.Level):
-    tag = "Level"
-
-    @classmethod
-    def parse(cls, node: etree._Element, index: int):
-        """Parse a <Level> XML node."""
-        name = _get_attr(node, "name")
-        logger.debug("Parsing node <%s name='%s' />", cls.tag, name)
-
-        key_type = node.get("key_type")
-
-        return cls(
-            name=name,
-            depth=index + 1,
-            key_column=_get_attr(node, "key_column"),
-            key_type=MemberType.from_str(key_type),
-            captions=immu.Map(_yield_locale_pairs(node, "caption")),
-            name_column_map=immu.Map(_yield_locale_pairs(node, "name_column")),
-            property_map=OrderedDict(_yield_children_nodes(node, XMLProperty)),
-            annotations=immu.Map(_yield_annotations(node)),
-        )
-
-
-class XMLProperty(models.Property):
-    tag = "Property"
-
-    @classmethod
-    def parse(cls, node: etree._Element, index: int):
-        """Parse a <Property> XML node."""
-        name = _get_attr(node, "name")
-        logger.debug("Parsing node <%s name='%s' />", cls.tag, name)
-
-        key_type = node.get("key_type")
-
-        keycol_map = immu.Map(_yield_locale_pairs(node, "key_column"))
-        if len(keycol_map) == 0:
-            raise MissingXMLAttribute(node.tag, "key_column")
-
-        return cls(
-            name=name,
-            annotations=immu.Map(_yield_annotations(node)),
-            captions=immu.Map(_yield_locale_pairs(node, "caption")),
-            key_column_map=keycol_map,
-            key_type=MemberType.from_str(key_type),
-        )
-
-
-class XMLMeasure(models.Measure):
-    tag = "Measure"
-
-    @classmethod
-    def parse(cls, node: etree._Element, index: int):
-        """Parse a <Measure> XML node."""
-        name = _get_attr(node, "name")
-        logger.debug("Parsing node <%s name='%s' />", cls.tag, name)
-
-        return cls(
-            name=name,
-            key_column=_get_attr(node, "key_column"),
-            aggregator=cls._get_aggregator(node),
-            annotations=immu.Map(_yield_annotations(node)),
-            captions=immu.Map(_yield_locale_pairs(node, "caption")),
-            submeasures=immu.Map(_yield_children_nodes(node, cls)),
-        )
-
-    @staticmethod
-    def _get_aggregator(mea_node: etree._Element) -> Aggregator:
-        """
-        Raises:
-            :class:`MissingXMLAttribute` --
-                If the node doesn't have an `aggregator` attribute or an
-                `<Agregation>` child node.
-
-            :class:`InvalidXMLAttributeValue` --
-                If the aggregator defined for this node has an unexpected value.
-        """
-
-        agg_node = mea_node.find("Aggregation")
-
-        # if there's an <Aggregation> node, get its `type`
-        # else get the `<Measure>`'s `aggregator` attribute
-        node, attr = (mea_node, "aggregator") if agg_node is None else (agg_node, "type")
-        value = _get_attr(node, attr)
-
-        try:
-            agg_type = AggregatorType.from_str(value)
-        except ValueError:
-            node_name = _get_attr(mea_node, "name")
-            raise InvalidXMLAttributeValue(node.tag, node_name, attr, value)
-        else:
-            agg_cls = Aggregator.from_enum(agg_type)
-            agg_args = {
-                str(k).replace("-", "_"): numerify(v) if is_numeric(v) else str(v)
-                for k, v in node.attrib.items()
-            }
-            return agg_cls.new(agg_args)
-
-
-class XMLCalculatedMeasure(models.CalculatedMeasure):
-    tag = "CalculatedMeasure"
-
-    @classmethod
-    def parse(cls, node: etree._Element, index: int):
-        """Parse a <CalculatedMeasure> XML node."""
-        name = _get_attr(node, "name")
-        logger.debug("Parsing node <%s name='%s' />", cls.tag, name)
-
-        return cls(
-            name=name,
-            formula=cls._parse_formula(_get_attr(node, "formula")),
-            annotations=immu.Map(_yield_annotations(node)),
-            captions=immu.Map(_yield_locale_pairs(node, "caption")),
-        )
-
-
-def _find_table_ref(node: etree._Element):
-    gen_tables = (item for item in node.iterchildren("InlineTable", "Table", "TableUsage"))
-    table_node = next(gen_tables, None)
-
-    if table_node is None:
-        return None
-    elif table_node.tag == "InlineTable":
-        return XMLInlineTable.parse(table_node, 0)
-    elif table_node.tag == "Table":
-        return XMLTable.parse(table_node, 0)
-    elif table_node.tag == "TableUsage":
-        return _get_attr(table_node, "source")
-
-    raise MissingXMLNode(node.tag, _get_attr(node, "name"), "Table")
-
-
-def _get_attr(node: etree._Element, attr: str) -> str:
-    """Retrieves an attribute from a node.
-
-    If the attribute is not present, raises :class:`MissingXMLAttribute`.
-    """
-    try:
-        value = node.attrib[attr]
-    except KeyError as exc:
-        raise MissingXMLAttribute(node.tag, attr) from exc
-    else:
-        return str(value)
-
-
-def _yield_annotations(node: etree._Element) -> Iterable[Tuple[str, Optional[str]]]:
-    """Yields a pair of (name, value) for each Annotation in the node."""
-    return (
-        (_get_attr(item, "name"), item.text)
-        for item in node.iterchildren("Annotation")
-    )
-
-
-def _yield_children_nodes(
-    node: etree._Element,
-    *children: Type[AnyXMLEntity],
-    attr: str = "name",
-) -> Generator[Tuple[str, AnyXMLEntity], None, None]:
-    tags = (item.tag for item in children)
-    parsers = {item.tag: item.parse for item in children}
-    for index, item in enumerate(node.iterchildren(*tags)):
-        reducer = parsers[item.tag]
-        yield _get_attr(item, attr), reducer(item, index)
-
-
-def _yield_locale_pairs(node: etree._Element,
-                        attribute: str) -> Generator[Tuple[str, str], None, None]:
-    attr_value = node.get(attribute)
-    if attr_value is not None:
-        yield ("xx", attr_value)
-
-    for child_node in node.iterchildren("LocalizedAttr"):
-        child_attr = _get_attr(child_node, "attr")
-        if child_attr != attribute:
-            continue
-
-        child_value = child_node.get("value", child_node.text)
-        if child_value is not None:
-            yield (_get_attr(child_node, "locale"), child_value)
-
-
-def parse_xml_schema(source: Union[str, Path, TextIO]) -> XMLSchema:
-    """Attempts to parse an object into a XMLSchema.
-
-    This function accepts:
-    - A raw XML :class:`str`
-    - A local path (as a :class:`pathlib.Path`) to a XML file
-    - A not-binary read-only :class:`TextIO` instance for a file-like object
-    """
-    parser = etree.XMLParser(encoding="utf-8",
-                             remove_blank_text=True,
-                             remove_comments=True)
-
-    # if argument is str, is assumed to be a raw XML string
-    if isinstance(source, str):
-        root = etree.fromstring(source, parser)
-        return XMLSchema.parse(root)
-
-    # if argument is pathlib.Path or TextIO, open it and parse contents
-    else:
-        tree = etree.parse(source, parser)
-        root = tree.getroot()
-        return XMLSchema.parse(root)
+"""XML Schema parsing module
+
+Defines subclasses for the core Entity classes, parsed from an XML document.
+"""
+
+import logging
+from ast import literal_eval as eval_tuple
+from collections import OrderedDict
+from pathlib import Path
+from typing import (
+    Generator,
+    Iterable,
+    List,
+    Optional,
+    TextIO,
+    Tuple,
+    Type,
+    TypeVar,
+    Union,
+)
+
+import immutables as immu
+from lxml import etree
+
+from tesseract_olap.common import is_numeric, numerify
+from tesseract_olap.exceptions.schema import (
+    InvalidXMLAttributeValue,
+    MissingXMLAttribute,
+    MissingXMLNode,
+)
+
+from . import models
+from .aggregators import Aggregator
+from .csv import parse_csv
+from .enums import AggregatorType, DimensionType, MemberType
+
+logger = logging.getLogger(__name__)
+
+XMLEntity = Union[
+    "XMLSharedDimension",
+    "XMLHierarchy",
+    "XMLLevel",
+    "XMLProperty",
+    "XMLInlineTable",
+    "XMLCube",
+    "XMLDimensionUsage",
+    "XMLHierarchyUsage",
+    "XMLLevelUsage",
+    "XMLPropertyUsage",
+    "XMLPrivateDimension",
+    "XMLMeasure",
+    "XMLCalculatedMeasure",
+]
+
+AnyXMLEntity = TypeVar("AnyXMLEntity", bound=XMLEntity)
+
+
+class XMLSchema(models.Schema):
+    tag = "Schema"
+
+    @classmethod
+    def parse(cls, node: etree._Element, index: int = 0):
+        """Parse a <Schema> XML node."""
+        name = _get_attr(node, "name")
+        logger.debug("Parsing node <%s name='%s' />", cls.tag, name)
+
+        cube_gen = _yield_children_nodes(node, XMLCube)
+        shareddim_gen = _yield_children_nodes(node, XMLSharedDimension)
+        sharedtbl_gen = _yield_children_nodes(node, XMLInlineTable)
+
+        return cls(
+            name=name,
+            cube_map=OrderedDict(cube_gen),
+            shared_dimension_map=immu.Map(shareddim_gen),
+            shared_table_map=immu.Map(sharedtbl_gen),
+            default_locale=node.get("default_locale", "xx"),
+            annotations=immu.Map(_yield_annotations(node)),
+        )
+
+
+class XMLAccessControl(models.AccessControl):
+    tag = "Access"
+
+    @classmethod
+    def parse(cls, node: etree._Element):
+        """Parse all <Access> XML node that are directly under this node."""
+
+        rules_gen = (
+            (role, _get_attr(item, "rule") == "allow")
+            for item in node.iterchildren(cls.tag)
+            for role in _get_attr(item, "roles").split(",")
+        )
+
+        return cls(
+            public=node.get("public", "true") == "true",
+            rules=immu.Map(rules_gen),
+        )
+
+
+class XMLCube(models.Cube):
+    tag = "Cube"
+
+    @classmethod
+    def parse(cls, node: etree._Element, index: int):
+        """Parse a <Cube> XML node."""
+        name = _get_attr(node, "name")
+        logger.debug("Parsing node <%s name='%s' />", cls.tag, name)
+
+        table = _find_table_ref(node)
+        if table is None:
+            raise MissingXMLNode(node.tag, name, "Table")
+
+        dimension_map = OrderedDict(
+            _yield_children_nodes(node, XMLPrivateDimension, XMLDimensionUsage)
+        )
+        if len(dimension_map) == 0:
+            raise MissingXMLNode(node.tag, name, "Dimension")
+
+        measure_map = OrderedDict(
+            _yield_children_nodes(node, XMLMeasure, XMLCalculatedMeasure)
+        )
+        if len(measure_map) == 0:
+            raise MissingXMLNode(node.tag, name, "Measure")
+
+        return cls(
+            name=name,
+            captions=immu.Map(_yield_locale_pairs(node, "caption")),
+            acl=XMLAccessControl.parse(node),
+            dimension_map=dimension_map,
+            measure_map=measure_map,
+            table=table,
+            annotations=immu.Map(_yield_annotations(node)),
+            subset_table=node.get("subset_table", "false").lower() != "false",
+            visible=node.get("visible", "true").lower() != "false",
+        )
+
+
+class XMLDimensionUsage(models.DimensionUsage):
+    tag = "DimensionUsage"
+
+    @classmethod
+    def parse(cls, node: etree._Element, index: int):
+        """Parse a <DimensionUsage> XML node."""
+        name = _get_attr(node, "name")
+        logger.debug("Parsing node <%s name='%s' />", cls.tag, name)
+
+        return cls(
+            name=name,
+            source=_get_attr(node, "source"),
+            foreign_key=_get_attr(node, "foreign_key"),
+            annotations=immu.Map(_yield_annotations(node)),
+            captions=immu.Map(_yield_locale_pairs(node, "caption")),
+            hierarchy_map=OrderedDict(
+                _yield_children_nodes(node, XMLHierarchyUsage, attr="source")
+            ),
+        )
+
+
+class XMLHierarchyUsage(models.HierarchyUsage):
+    tag = "HierarchyUsage"
+
+    @classmethod
+    def parse(cls, node: etree._Element, index: int):
+        """Parse a <HierarchyUsage> XML node."""
+        name = _get_attr(node, "name")
+        logger.debug("Parsing node <%s name='%s' />", cls.tag, name)
+
+        return cls(
+            name=name,
+            source=_get_attr(node, "source"),
+            annotations=immu.Map(_yield_annotations(node)),
+            captions=immu.Map(_yield_locale_pairs(node, "caption")),
+            level_map=OrderedDict(
+                _yield_children_nodes(node, XMLLevelUsage, attr="source")
+            ),
+        )
+
+
+class XMLLevelUsage(models.LevelUsage):
+    tag = "LevelUsage"
+
+    @classmethod
+    def parse(cls, node: etree._Element, index: int):
+        """Parse a <LevelUsage> XML node."""
+        name = _get_attr(node, "name")
+        logger.debug("Parsing node <%s name='%s' />", cls.tag, name)
+
+        return cls(
+            name=name,
+            source=_get_attr(node, "source"),
+            annotations=immu.Map(_yield_annotations(node)),
+            captions=immu.Map(_yield_locale_pairs(node, "caption")),
+            property_map=OrderedDict(
+                _yield_children_nodes(node, XMLPropertyUsage, attr="source")
+            ),
+        )
+
+
+class XMLPropertyUsage(models.PropertyUsage):
+    tag = "PropertyUsage"
+
+    @classmethod
+    def parse(cls, node: etree._Element, index: int):
+        """Parse a <PropertyUsage> XML node."""
+        name = _get_attr(node, "name")
+        logger.debug("Parsing node <%s name='%s' />", cls.tag, name)
+
+        return cls(
+            name=name,
+            source=_get_attr(node, "source"),
+            annotations=immu.Map(_yield_annotations(node)),
+            captions=immu.Map(_yield_locale_pairs(node, "caption")),
+        )
+
+
+class XMLTable(models.Table):
+    tag = "Table"
+
+    @classmethod
+    def parse(cls, node: etree._Element, index: int):
+        """Parse a <Table> XML node."""
+        name = _get_attr(node, "name")
+        logger.debug("Parsing node <%s name='%s' />", cls.tag, name)
+
+        return cls(
+            name=name,
+            schema=node.get("schema"),
+            primary_key=node.get("primary_key", "id"),
+        )
+
+
+class XMLInlineTable(models.InlineTable):
+    tag = "InlineTable"
+
+    @classmethod
+    def parse(cls, node: etree._Element, index: int):
+        """Parse a <InlineTable> XML node."""
+        name = _get_attr(node, "name")
+        logger.debug("Parsing node <%s name='%s' />", cls.tag, name)
+
+        node_format = _get_attr(node, "format")
+
+        if node_format == "csv":
+            node_format = "text/csv"
+
+        if node_format == "tuples":
+            headers, rows = cls.parse_tuples(node)
+        elif node_format.startswith("text/csv"):
+            content = [] if node.text is None else node.text.strip().splitlines()
+            headers, *rows = parse_csv(content, mimetype=node_format)
+            headers = tuple(str(item) for item in headers)
+        else:
+            raise InvalidXMLAttributeValue(node.tag, name, "format", node_format)
+
+        return cls(
+            name=name,
+            headers=headers,
+            types=cls.infer_types(rows),
+            rows=rows,
+        )
+
+    @staticmethod
+    def parse_tuples(
+        node: etree._Element,
+    ) -> Tuple[Tuple[str, ...], List[Tuple[Union[str, float], ...]]]:
+        """Parse the child nodes from an InlineTable with `tuples` format."""
+        try:
+            # try parsing literal tuples with ast.eval()
+            children: List[Tuple[Union[str, float], ...]] = [
+                eval_tuple(line)
+                for line in (item.text for item in node.iterchildren("Row"))
+                if line
+            ]
+        except SyntaxError:
+            # Python `tuples` looks similar to CSV, so let's try with it
+            row_iter = (
+                line[1:-1] if line.startswith("(") and line.endswith(")") else line
+                for line in (item.text for item in node.iterchildren("Row"))
+                if line is not None
+            )
+            children = parse_csv(row_iter, skipinitialspace=True)
+        # at least 2 rows must be present: a header list and a data row
+        if len(children) < 2:
+            raise MissingXMLNode(node.tag, _get_attr(node, "name"), "Row")
+        headers = tuple(str(item) for item in children[0])
+        return headers, children[1:]
+
+
+class XMLSharedDimension(models.Dimension):
+    tag = "SharedDimension"
+
+    @classmethod
+    def parse(cls, node: etree._Element, index: int):
+        """Parse a Shared <Dimension> XML node."""
+        name = _get_attr(node, "name")
+        logger.debug("Parsing node <%s name='%s' />", cls.tag, name)
+
+        dim_type = node.get("type")
+
+        hierarchy_map = OrderedDict(_yield_children_nodes(node, XMLHierarchy))
+
+        default_hierarchy = node.get("default_hierarchy")
+        if default_hierarchy not in hierarchy_map:
+            default_hierarchy = next(iter(hierarchy_map.keys()))
+
+        return cls(
+            name=name,
+            captions=immu.Map(_yield_locale_pairs(node, "caption")),
+            default_hierarchy=default_hierarchy,
+            dim_type=DimensionType.from_str(dim_type),
+            foreign_key=node.get("foreign_key"),
+            hierarchy_map=hierarchy_map,
+            annotations=immu.Map(_yield_annotations(node)),
+        )
+
+
+class XMLPrivateDimension(models.Dimension):
+    tag = "Dimension"
+
+    @classmethod
+    def parse(cls, node: etree._Element, index: int):
+        """Parse a Private <Dimension> XML node."""
+        dimension: cls = XMLSharedDimension.parse.__func__(cls, node, index)
+
+        # foreign keys are required in Private Dimensions
+        if dimension.foreign_key is None:
+            raise MissingXMLAttribute(node.tag, "foreign_key")
+
+        return dimension
+
+
+class XMLHierarchy(models.Hierarchy):
+    tag = "Hierarchy"
+
+    @classmethod
+    def parse(cls, node: etree._Element, index: int):
+        """Parse a <Hierarchy> XML node."""
+        name = _get_attr(node, "name")
+        logger.debug("Parsing node <%s name='%s' />", cls.tag, name)
+
+        level_map = OrderedDict(_yield_children_nodes(node, XMLLevel))
+        if len(level_map) == 0:
+            raise MissingXMLNode(node.tag, name, "Level")
+
+        default_pk = ""
+        for item in level_map.values():
+            default_pk = item.key_column
+
+        return cls(
+            name=name,
+            primary_key=node.get("primary_key", default_pk),
+            captions=immu.Map(_yield_locale_pairs(node, "caption")),
+            table=_find_table_ref(node),
+            level_map=level_map,
+            default_member=cls._parse_default_member(node),
+            annotations=immu.Map(_yield_annotations(node)),
+        )
+
+    @staticmethod
+    def _parse_default_member(node: etree._Element):
+        items: List[str] = node.get("default_member", "").split(".", maxsplit=1)
+        return (items[0], items[1]) if len(items) == 2 else None
+
+
+class XMLLevel(models.Level):
+    tag = "Level"
+
+    @classmethod
+    def parse(cls, node: etree._Element, index: int):
+        """Parse a <Level> XML node."""
+        name = _get_attr(node, "name")
+        logger.debug("Parsing node <%s name='%s' />", cls.tag, name)
+
+        key_type = node.get("key_type")
+
+        return cls(
+            name=name,
+            depth=index + 1,
+            key_column=_get_attr(node, "key_column"),
+            key_type=MemberType.from_str(key_type),
+            captions=immu.Map(_yield_locale_pairs(node, "caption")),
+            name_column_map=immu.Map(_yield_locale_pairs(node, "name_column")),
+            property_map=OrderedDict(_yield_children_nodes(node, XMLProperty)),
+            annotations=immu.Map(_yield_annotations(node)),
+        )
+
+
+class XMLProperty(models.Property):
+    tag = "Property"
+
+    @classmethod
+    def parse(cls, node: etree._Element, index: int):
+        """Parse a <Property> XML node."""
+        name = _get_attr(node, "name")
+        logger.debug("Parsing node <%s name='%s' />", cls.tag, name)
+
+        key_type = node.get("key_type")
+
+        keycol_map = immu.Map(_yield_locale_pairs(node, "key_column"))
+        if len(keycol_map) == 0:
+            raise MissingXMLAttribute(node.tag, "key_column")
+
+        return cls(
+            name=name,
+            annotations=immu.Map(_yield_annotations(node)),
+            captions=immu.Map(_yield_locale_pairs(node, "caption")),
+            key_column_map=keycol_map,
+            key_type=MemberType.from_str(key_type),
+        )
+
+
+class XMLMeasure(models.Measure):
+    tag = "Measure"
+
+    @classmethod
+    def parse(cls, node: etree._Element, index: int):
+        """Parse a <Measure> XML node."""
+        name = _get_attr(node, "name")
+        logger.debug("Parsing node <%s name='%s' />", cls.tag, name)
+
+        return cls(
+            name=name,
+            key_column=_get_attr(node, "key_column"),
+            aggregator=cls._get_aggregator(node),
+            annotations=immu.Map(_yield_annotations(node)),
+            captions=immu.Map(_yield_locale_pairs(node, "caption")),
+            submeasures=immu.Map(_yield_children_nodes(node, cls)),
+        )
+
+    @staticmethod
+    def _get_aggregator(mea_node: etree._Element) -> Aggregator:
+        """
+        Raises:
+            :class:`MissingXMLAttribute` --
+                If the node doesn't have an `aggregator` attribute or an
+                `<Agregation>` child node.
+
+            :class:`InvalidXMLAttributeValue` --
+                If the aggregator defined for this node has an unexpected value.
+        """
+
+        agg_node = mea_node.find("Aggregation")
+
+        # if there's an <Aggregation> node, get its `type`
+        # else get the `<Measure>`'s `aggregator` attribute
+        node, attr = (mea_node, "aggregator") if agg_node is None else (agg_node, "type")
+        value = _get_attr(node, attr)
+
+        try:
+            agg_type = AggregatorType.from_str(value)
+        except ValueError:
+            node_name = _get_attr(mea_node, "name")
+            raise InvalidXMLAttributeValue(node.tag, node_name, attr, value)
+        else:
+            agg_cls = Aggregator.from_enum(agg_type)
+            agg_args = {
+                str(k).replace("-", "_"): numerify(v) if is_numeric(v) else str(v)
+                for k, v in node.attrib.items()
+            }
+            return agg_cls.new(agg_args)
+
+
+class XMLCalculatedMeasure(models.CalculatedMeasure):
+    tag = "CalculatedMeasure"
+
+    @classmethod
+    def parse(cls, node: etree._Element, index: int):
+        """Parse a <CalculatedMeasure> XML node."""
+        name = _get_attr(node, "name")
+        logger.debug("Parsing node <%s name='%s' />", cls.tag, name)
+
+        return cls(
+            name=name,
+            formula=cls._parse_formula(_get_attr(node, "formula")),
+            annotations=immu.Map(_yield_annotations(node)),
+            captions=immu.Map(_yield_locale_pairs(node, "caption")),
+        )
+
+
+def _find_table_ref(node: etree._Element):
+    gen_tables = (item for item in node.iterchildren("InlineTable", "Table", "TableUsage"))
+    table_node = next(gen_tables, None)
+
+    if table_node is None:
+        return None
+    elif table_node.tag == "InlineTable":
+        return XMLInlineTable.parse(table_node, 0)
+    elif table_node.tag == "Table":
+        return XMLTable.parse(table_node, 0)
+    elif table_node.tag == "TableUsage":
+        return _get_attr(table_node, "source")
+
+    raise MissingXMLNode(node.tag, _get_attr(node, "name"), "Table")
+
+
+def _get_attr(node: etree._Element, attr: str) -> str:
+    """Retrieves an attribute from a node.
+
+    If the attribute is not present, raises :class:`MissingXMLAttribute`.
+    """
+    try:
+        value = node.attrib[attr]
+    except KeyError as exc:
+        raise MissingXMLAttribute(node.tag, attr) from exc
+    else:
+        return str(value)
+
+
+def _yield_annotations(node: etree._Element) -> Iterable[Tuple[str, Optional[str]]]:
+    """Yields a pair of (name, value) for each Annotation in the node."""
+    return (
+        (_get_attr(item, "name"), item.text)
+        for item in node.iterchildren("Annotation")
+    )
+
+
+def _yield_children_nodes(
+    node: etree._Element,
+    *children: Type[AnyXMLEntity],
+    attr: str = "name",
+) -> Generator[Tuple[str, AnyXMLEntity], None, None]:
+    tags = (item.tag for item in children)
+    parsers = {item.tag: item.parse for item in children}
+    for index, item in enumerate(node.iterchildren(*tags)):
+        reducer = parsers[item.tag]
+        yield _get_attr(item, attr), reducer(item, index)
+
+
+def _yield_locale_pairs(node: etree._Element,
+                        attribute: str) -> Generator[Tuple[str, str], None, None]:
+    attr_value = node.get(attribute)
+    if attr_value is not None:
+        yield ("xx", attr_value)
+
+    for child_node in node.iterchildren("LocalizedAttr"):
+        child_attr = _get_attr(child_node, "attr")
+        if child_attr != attribute:
+            continue
+
+        child_value = child_node.get("value", child_node.text)
+        if child_value is not None:
+            yield (_get_attr(child_node, "locale"), child_value)
+
+
+def parse_xml_schema(source: Union[str, Path, TextIO]) -> XMLSchema:
+    """Attempts to parse an object into a XMLSchema.
+
+    This function accepts:
+    - A raw XML :class:`str`
+    - A local path (as a :class:`pathlib.Path`) to a XML file
+    - A not-binary read-only :class:`TextIO` instance for a file-like object
+    """
+    parser = etree.XMLParser(encoding="utf-8",
+                             remove_blank_text=True,
+                             remove_comments=True)
+
+    # if argument is str, is assumed to be a raw XML string
+    if isinstance(source, str):
+        root = etree.fromstring(source, parser)
+        return XMLSchema.parse(root)
+
+    # if argument is pathlib.Path or TextIO, open it and parse contents
+    else:
+        tree = etree.parse(source, parser)
+        root = tree.getroot()
+        return XMLSchema.parse(root)
```

### Comparing `tesseract_olap-0.9.2/tesseract_olap/server/schema.py` & `tesseract_olap-0.9.3/tesseract_olap/server/schema.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.2/tesseract_olap/server/server.py` & `tesseract_olap-0.9.3/tesseract_olap/server/server.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 from pathlib import Path
 from typing import Union
 
 from typing_extensions import deprecated
 
-from tesseract_olap.backend import Backend, CacheProvider, DummyProvider
+from tesseract_olap.backend import Backend, CacheProvider, DummyProvider, LfuProvider
 from tesseract_olap.exceptions.query import InvalidQuery
 from tesseract_olap.exceptions.server import UnknownBackendError
 from tesseract_olap.query import (
     AnyRequest,
     DataQuery,
     DataRequest,
     MembersQuery,
@@ -102,13 +102,21 @@
         return ClickhouseBackend(dsn)
 
     raise UnknownBackendError(dsn)
 
 
 def _setup_cache(dsn: str) -> CacheProvider:
     """Generates a new instance of a CacheProvider bundled in this package."""
-    if dsn.startswith("redis:") or dsn.startswith("rediss:"):
-        from tesseract_olap.backend.redis import RedisProvider
+    if dsn == ":memory:":
+        return LfuProvider()
 
-        return RedisProvider(dsn)
+    if (
+        dsn.startswith("valkey:")
+        or dsn.startswith("valkeys:")
+        or dsn.startswith("redis:")
+        or dsn.startswith("rediss:")
+    ):
+        from tesseract_olap.backend.valkey import ValkeyProvider
+
+        return ValkeyProvider(dsn)
 
     return DummyProvider()
```

### Comparing `tesseract_olap-0.9.2/PKG-INFO` & `tesseract_olap-0.9.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tesseract-olap
-Version: 0.9.2
+Version: 0.9.3
 Summary: A simple OLAP library.
 Home-page: https://github.com/Datawheel/tesseract-python
 License: MIT
 Author: Francisco Abarzua
 Author-email: francisco@datawheel.us
 Maintainer: Francisco Abarzua
 Maintainer-email: francisco@datawheel.us
@@ -19,14 +19,15 @@
 Provides-Extra: clickhouse
 Provides-Extra: redis
 Requires-Dist: PyPika (>=0.48.0,<1.0)
 Requires-Dist: clickhouse-cityhash (>=1.0.2.4,<2.0.0.0) ; extra == "clickhouse"
 Requires-Dist: clickhouse-driver[lz4] (>=0.2.0,<0.3.0) ; extra == "clickhouse"
 Requires-Dist: httpx (>=0.18.0,<1.0)
 Requires-Dist: immutables (>=0.16,<1.0)
+Requires-Dist: lfudacache (>=0.0.2,<0.0.3)
 Requires-Dist: lxml (>=4.6.0,<5.0.0)
 Requires-Dist: orjson (>=3.9.15,<4.0.0)
 Requires-Dist: polars (>=0.20.0,<0.21.0)
 Requires-Dist: redis (>=5.0.0,<6.0.0) ; extra == "redis"
 Requires-Dist: typing-extensions (>=3.7.4)
 Requires-Dist: xlsxwriter (>=3.2.0,<4.0.0)
 Project-URL: Repository, https://github.com/Datawheel/tesseract-python
```

