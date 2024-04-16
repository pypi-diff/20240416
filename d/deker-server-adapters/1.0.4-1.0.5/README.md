# Comparing `tmp/deker_server_adapters-1.0.4.tar.gz` & `tmp/deker_server_adapters-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deker_server_adapters-1.0.4.tar", max compression
+gzip compressed data, was "deker_server_adapters-1.0.5.tar", max compression
```

## Comparing `deker_server_adapters-1.0.4.tar` & `deker_server_adapters-1.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    35149 2024-03-06 10:05:54.091452 deker_server_adapters-1.0.4/LICENSE
--rw-r--r--   0        0        0      356 2024-03-06 10:05:54.091452 deker_server_adapters-1.0.4/README.md
--rw-r--r--   0        0        0       45 2024-03-06 10:05:54.091452 deker_server_adapters-1.0.4/deker_server_adapters/__init__.py
--rw-r--r--   0        0        0     2716 2024-03-06 10:05:54.091452 deker_server_adapters-1.0.4/deker_server_adapters/array_adapter.py
--rw-r--r--   0        0        0    17085 2024-03-06 10:05:54.091452 deker_server_adapters-1.0.4/deker_server_adapters/base.py
--rw-r--r--   0        0        0     4475 2024-03-06 10:05:54.091452 deker_server_adapters-1.0.4/deker_server_adapters/collection_adapter.py
--rw-r--r--   0        0        0      582 2024-03-06 10:05:54.091452 deker_server_adapters-1.0.4/deker_server_adapters/consts.py
--rw-r--r--   0        0        0     2646 2024-03-06 10:05:54.091452 deker_server_adapters-1.0.4/deker_server_adapters/errors.py
--rw-r--r--   0        0        0     7013 2024-03-06 10:05:54.091452 deker_server_adapters-1.0.4/deker_server_adapters/factory.py
--rw-r--r--   0        0        0     4575 2024-03-06 10:05:54.091452 deker_server_adapters-1.0.4/deker_server_adapters/hash_ring.py
--rw-r--r--   0        0        0     2690 2024-03-06 10:05:54.091452 deker_server_adapters-1.0.4/deker_server_adapters/httpx_client.py
--rw-r--r--   0        0        0     2586 2024-03-06 10:05:54.091452 deker_server_adapters-1.0.4/deker_server_adapters/utils.py
--rw-r--r--   0        0        0      895 2024-03-06 10:05:54.091452 deker_server_adapters-1.0.4/deker_server_adapters/varray_adapter.py
--rw-r--r--   0        0        0     7094 2024-03-06 10:06:01.519475 deker_server_adapters-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     1596 1970-01-01 00:00:00.000000 deker_server_adapters-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-16 13:47:25.277088 deker_server_adapters-1.0.5/LICENSE
+-rw-r--r--   0        0        0      356 2024-04-16 13:47:25.277088 deker_server_adapters-1.0.5/README.md
+-rw-r--r--   0        0        0       45 2024-04-16 13:47:25.277088 deker_server_adapters-1.0.5/deker_server_adapters/__init__.py
+-rw-r--r--   0        0        0     2716 2024-04-16 13:47:25.277088 deker_server_adapters-1.0.5/deker_server_adapters/array_adapter.py
+-rw-r--r--   0        0        0    16842 2024-04-16 13:47:25.277088 deker_server_adapters-1.0.5/deker_server_adapters/base.py
+-rw-r--r--   0        0        0     4475 2024-04-16 13:47:25.277088 deker_server_adapters-1.0.5/deker_server_adapters/collection_adapter.py
+-rw-r--r--   0        0        0      582 2024-04-16 13:47:25.277088 deker_server_adapters-1.0.5/deker_server_adapters/consts.py
+-rw-r--r--   0        0        0     2743 2024-04-16 13:47:25.277088 deker_server_adapters-1.0.5/deker_server_adapters/errors.py
+-rw-r--r--   0        0        0     7087 2024-04-16 13:47:25.277088 deker_server_adapters-1.0.5/deker_server_adapters/factory.py
+-rw-r--r--   0        0        0     4673 2024-04-16 13:47:25.277088 deker_server_adapters-1.0.5/deker_server_adapters/hash_ring.py
+-rw-r--r--   0        0        0     2690 2024-04-16 13:47:25.277088 deker_server_adapters-1.0.5/deker_server_adapters/httpx_client.py
+-rw-r--r--   0        0        0     3802 2024-04-16 13:47:25.277088 deker_server_adapters-1.0.5/deker_server_adapters/utils.py
+-rw-r--r--   0        0        0      895 2024-04-16 13:47:25.277088 deker_server_adapters-1.0.5/deker_server_adapters/varray_adapter.py
+-rw-r--r--   0        0        0     7094 2024-04-16 13:47:33.585137 deker_server_adapters-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1596 1970-01-01 00:00:00.000000 deker_server_adapters-1.0.5/PKG-INFO
```

### Comparing `deker_server_adapters-1.0.4/LICENSE` & `deker_server_adapters-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `deker_server_adapters-1.0.4/deker_server_adapters/array_adapter.py` & `deker_server_adapters-1.0.5/deker_server_adapters/array_adapter.py`

 * *Files identical despite different names*

### Comparing `deker_server_adapters-1.0.4/deker_server_adapters/base.py` & `deker_server_adapters-1.0.5/deker_server_adapters/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from httpx import Response, TimeoutException
 from numpy import ndarray
 
 from deker_server_adapters.consts import NOT_FOUND, STATUS_CREATED, STATUS_OK, TIMEOUT, ArrayType
 from deker_server_adapters.errors import DekerServerError, DekerTimeoutServer, FilteringByIdInClusterIsForbidden
 from deker_server_adapters.hash_ring import HashRing
 from deker_server_adapters.httpx_client import HttpxClient
-from deker_server_adapters.utils import make_request
+from deker_server_adapters.utils import get_hash_by_primary_attrs, get_hash_key, make_request
 
 
 if TYPE_CHECKING:
     from deker.ABC.base_adapters import BaseArrayAdapter, BaseVArrayAdapter
     from deker.ABC.base_schemas import BaseArraysSchema
 
 logger = logging.getLogger(__name__)
@@ -140,27 +140,20 @@
             "custom_attributes": convert_datetime_attrs_to_iso(
                 array["custom_attributes"],
             ),
         }
 
         if isinstance(array, dict):
             kwargs["id_"] = array.get("id_") or (self.client.cluster_mode and get_id() or None)
+            array["id_"] = kwargs["id_"]
 
         path = self.collection_path.raw_url.rstrip("/")
 
         if self.type == ArrayType.array and self.client.cluster_mode:
-            if isinstance(array, dict):
-                if array.get("primary_attributes"):
-                    node_id = self.get_node_by_primary_attrs(array.get("primary_attributes"))  # type: ignore[arg-type]
-                else:
-                    node_id = self.hash_ring.get_node(kwargs.get("id_"))  # type: ignore[arg-type, assignment]
-
-            else:
-                node_id = self.get_node(array)
-
+            node_id = self.hash_ring.get_node(get_hash_key(array))
             node = self.get_host_url(node_id)
             path = self.__merge_node_and_collection_path(node)
 
         response = self.client.post(f"{path}/{self.type.name}s", json=kwargs)
         if response.status_code != STATUS_CREATED:
             raise DekerServerError(response, "Couldn't create an array")
 
@@ -382,15 +375,15 @@
             else:
                 attrs.append(str(primary_attributes[attr.name]))  # type: ignore[index]
 
         primary_path = "/".join(attrs)
 
         # We read an Array through the node it belongs
         if self.client.cluster_mode:
-            node_id = self.get_node_by_primary_attrs(primary_attributes)
+            node_id = self.hash_ring.get_node(get_hash_by_primary_attrs(primary_attributes))
             node = self.get_host_url(node_id)
             path = self.__merge_node_and_collection_path(node)
         else:
             path = self.collection_path.raw_url.rstrip("/")
 
         response = self.client.get(
             f"{path}/{self.type.name}/by-primary/{primary_path}",
```

### Comparing `deker_server_adapters-1.0.4/deker_server_adapters/collection_adapter.py` & `deker_server_adapters-1.0.5/deker_server_adapters/collection_adapter.py`

 * *Files identical despite different names*

### Comparing `deker_server_adapters-1.0.4/deker_server_adapters/consts.py` & `deker_server_adapters-1.0.5/deker_server_adapters/consts.py`

 * *Files identical despite different names*

### Comparing `deker_server_adapters-1.0.4/deker_server_adapters/errors.py` & `deker_server_adapters-1.0.5/deker_server_adapters/errors.py`

 * *Files 5% similar despite different names*

```diff
@@ -81,7 +81,11 @@
 class FilteringByIdInClusterIsForbidden(DekerBaseApplicationError):
     """If we try to filter by in in collection with primary attributes (in cluster)."""
 
     message = (
         "Collection has primary attributes in the schema."
         "Filtering by ID is not allowed. Use filtering by primary attributes."
     )
+
+
+class HashRingError(DekerBaseApplicationError):
+    """If there is a problem with HashRing."""
```

### Comparing `deker_server_adapters-1.0.4/deker_server_adapters/factory.py` & `deker_server_adapters-1.0.5/deker_server_adapters/factory.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,24 +5,26 @@
 from deker.ctx import CTX
 from deker.uri import Uri
 from httpx import Response
 
 from deker_server_adapters.array_adapter import ServerArrayAdapter
 from deker_server_adapters.collection_adapter import ServerCollectionAdapter
 from deker_server_adapters.consts import STATUS_OK
-from deker_server_adapters.errors import DekerClusterError, DekerServerError, HealthcheckError
+from deker_server_adapters.errors import DekerClusterError, DekerServerError
 from deker_server_adapters.hash_ring import HashRing
 from deker_server_adapters.httpx_client import HttpxClient
 from deker_server_adapters.utils import get_api_version, get_leader_and_nodes_mapping, make_request
 from deker_server_adapters.varray_adapter import ServerVarrayAdapter
 
 
 if TYPE_CHECKING:
     from deker.ABC.base_adapters import BaseArrayAdapter, BaseCollectionAdapter, BaseStorageAdapter, BaseVArrayAdapter
 
+CLUSTER_MODE = "cluster"
+
 
 class AdaptersFactory(BaseAdaptersFactory):
     """Factory that produces server adapters."""
 
     uri_schemes = ("http", "https")
 
     def __init__(self, ctx: "CTX", uri: "Uri") -> None:
@@ -53,20 +55,17 @@
 
         self.httpx_client = HttpxClient(**kwargs)
         # We have to keep reference to ctx, to be able to set new configuration
         self.httpx_client.ctx = copied_ctx
         copied_ctx.extra["httpx_client"] = self.httpx_client
 
         # Cluster config
-        if hasattr(uri, "servers") and uri.servers:
-            self.get_cluster_config_and_configure_context(copied_ctx)
+        self.get_config_and_configure_context(copied_ctx)
 
         # Single server
-        else:
-            self.do_healthcheck(ctx=copied_ctx, in_cluster=False)
 
         super().__init__(copied_ctx, uri)
 
     def close(self) -> None:
         """Shutdown executor and httpx client."""
         self.httpx_client.close()
         super().close()
@@ -121,76 +120,86 @@
         """Make server collection adapter.
 
         :param args: Won't be passed further
         :param kwargs: Won't be passed further
         """
         return ServerCollectionAdapter(self.ctx)
 
-    def do_healthcheck(self, ctx: CTX, in_cluster: bool = False) -> Optional[Dict]:
+    def do_healthcheck(self, ctx: CTX) -> Optional[Dict]:
         """Check if server is alive.
 
         Fetches config as well.
         :param ctx: App context
-        :param in_cluster: If we are in cluster
         """
 
         def check_response(response: Optional[Response], client: HttpxClient) -> None:
             if response is None or response.status_code != STATUS_OK:
                 client.close()
                 raise DekerServerError(
                     response,
                     "Healthcheck failed. Deker client will be closed.",
                 )
 
         url = f"{get_api_version()}/ping"
 
         # If we do healthcheck in cluster
-        nodes = [*ctx.uri.servers] if in_cluster else [ctx.uri.raw_url]
+        nodes = [*ctx.uri.servers] if ctx.uri.servers else [ctx.uri.raw_url]
         response = make_request(url=url, nodes=nodes, client=self.httpx_client)
         check_response(response=response, client=self.httpx_client)
 
-        if in_cluster:
-            try:
-                config = response.json()  # type: ignore[union-attr]
-                if config.get("mode") != "cluster":
-                    raise HealthcheckError
-                return config
-            except JSONDecodeError:
+        try:
+            config = response.json()  # type: ignore[union-attr]
+            return config
+        except JSONDecodeError:
+            if ctx.uri.servers:
                 raise DekerClusterError(response, "Server responded with wrong config. Couldn't parse json")
-            except HealthcheckError:
-                raise DekerClusterError(
-                    response,
-                    "Server responded with wrong config."
-                    " Key 'mode' either doesn't exist or its value differs from 'cluster'",
-                )
 
     def __set_cluster_config(self, cluster_config: Dict, ctx: CTX) -> None:
         """Set cluster config in the CTX.
 
         :param cluster_config: Custer config json from server
-        :param ctx: App cotext (Deker CTX)
+        :param ctx: App context (Deker CTX)
         """
         leader_node, ids, id_to_host_mapping, nodes = get_leader_and_nodes_mapping(cluster_config)
 
         if leader_node is None:
             raise DekerServerError(None, f"Leader node cannot be setted {cluster_config=}")
 
         # Set variables in context
         ctx.extra["leader_node"] = Uri.create(leader_node)
         ctx.extra["nodes_mapping"] = id_to_host_mapping
         ctx.extra["hash_ring"] = HashRing(ids)
         ctx.extra["nodes"] = nodes
 
-    def get_cluster_config_and_configure_context(self, ctx: CTX) -> None:
+    def __is_mode_cluster(self, config: Optional[dict], ctx: CTX) -> bool:
+        """Check if mode from config is set to cluster.
+
+        :param config: Config from response
+        :param ctx: Context of app
+        """
+        if not ctx.uri.servers:
+            return config is not None and config.get("mode") == CLUSTER_MODE
+
+        if config is None or config.get("mode") != CLUSTER_MODE:
+            raise DekerClusterError(
+                config,
+                "Server responded with wrong config."
+                " Key 'mode' either doesn't exist or its value differs from 'cluster'",
+            )
+
+        return True
+
+    def get_config_and_configure_context(self, ctx: CTX) -> None:
         """Get info from node and set config.
 
         :param ctx: CTX where client and config will be injected
         """
-        # Get Cluster config
-        cluster_config = self.do_healthcheck(ctx, in_cluster=True)
-
-        # Set cluster config
-        self.__set_cluster_config(cluster_config, ctx)  # type: ignore[arg-type]
+        # Get config
+        config = self.do_healthcheck(ctx)
 
-        # Set Httpx client based on cluster config
-        self.httpx_client.base_url = ctx.extra["leader_node"].raw_url
-        self.httpx_client.cluster_mode = True
+        if self.__is_mode_cluster(config, ctx):
+            # Set cluster config
+            self.__set_cluster_config(config, ctx)  # type: ignore[arg-type]
+
+            # Set Httpx client based on cluster config
+            self.httpx_client.base_url = ctx.extra["leader_node"].raw_url
+            self.httpx_client.cluster_mode = True
```

### Comparing `deker_server_adapters-1.0.4/deker_server_adapters/hash_ring.py` & `deker_server_adapters-1.0.5/deker_server_adapters/hash_ring.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import hashlib
 import math
 
 from bisect import bisect
 from typing import Callable, Generator, List, Optional, Set, Tuple, Union
 
+from deker_server_adapters.errors import HashRingError
+
 
 md5_constructor = hashlib.md5
 
 
 class HashRing:
     """Class for hash ring."""
 
@@ -57,23 +59,23 @@
 
         if not weights:
             weights = {}  # type: ignore[var-annotated]
         self.weights = weights
 
         self._generate_circle()
 
-    def get_node(self, string_key: str) -> Optional[str]:
+    def get_node(self, string_key: str) -> str:
         """Return hash ring by given a string key a corresponding node.
 
         If the hash ring is empty, `None` is returned.
         :param string_key: String key
         """
         pos = self.get_node_pos(string_key)
         if pos is None:
-            return None
+            raise HashRingError(f"Couldn't find a position in {self.ring}")
         return self.ring[self._sorted_keys[pos]]
 
     def get_node_pos(self, string_key: str) -> Optional[int]:
         """Return node and position.
 
         Given a string key a corresponding node in the hash ring
         is returned along with it's position in the ring.
```

### Comparing `deker_server_adapters-1.0.4/deker_server_adapters/httpx_client.py` & `deker_server_adapters-1.0.5/deker_server_adapters/httpx_client.py`

 * *Files identical despite different names*

### Comparing `deker_server_adapters-1.0.4/deker_server_adapters/varray_adapter.py` & `deker_server_adapters-1.0.5/deker_server_adapters/varray_adapter.py`

 * *Files identical despite different names*

### Comparing `deker_server_adapters-1.0.4/pyproject.toml` & `deker_server_adapters-1.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning>=1.0.0,<2.0.0"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 
 [tool.poetry]
 name = "deker_server_adapters"
-version = "1.0.4"
+version = "1.0.5"
 description = "Plugin with server adapters for Deker"
 authors = ["OpenWeather <info@openweathermap.org>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 packages = [{include = "deker_server_adapters"}]
 documentation = 'https://docs.deker.io/'
 homepage = 'https://deker.io/'
```

### Comparing `deker_server_adapters-1.0.4/PKG-INFO` & `deker_server_adapters-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deker_server_adapters
-Version: 1.0.4
+Version: 1.0.5
 Summary: Plugin with server adapters for Deker
 Home-page: https://deker.io/
 License: GPL-3.0-only
 Author: OpenWeather
 Author-email: info@openweathermap.org
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```

