# Comparing `tmp/izihawa_trident_client-1.2.2.tar.gz` & `tmp/izihawa_trident_client-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "izihawa_trident_client-1.2.2.tar", max compression
+gzip compressed data, was "izihawa_trident_client-1.2.3.tar", max compression
```

## Comparing `izihawa_trident_client-1.2.2.tar` & `izihawa_trident_client-1.2.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       64 2023-12-10 19:54:01.661696 izihawa_trident_client-1.2.2/README.md
--rw-r--r--   0        0        0      348 2024-04-15 07:21:48.524345 izihawa_trident_client-1.2.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-19 06:00:51.101322 izihawa_trident_client-1.2.2/trident/__init__.py
--rw-r--r--   0        0        0     4655 2024-04-15 07:21:42.943547 izihawa_trident_client-1.2.2/trident/client.py
--rw-r--r--   0        0        0      563 1970-01-01 00:00:00.000000 izihawa_trident_client-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0       64 2023-12-10 19:54:01.661696 izihawa_trident_client-1.2.3/README.md
+-rw-r--r--   0        0        0      348 2024-04-16 09:59:21.752554 izihawa_trident_client-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-01-19 06:00:51.101322 izihawa_trident_client-1.2.3/trident/__init__.py
+-rw-r--r--   0        0        0     4980 2024-04-16 09:59:16.347631 izihawa_trident_client-1.2.3/trident/client.py
+-rw-r--r--   0        0        0      563 1970-01-01 00:00:00.000000 izihawa_trident_client-1.2.3/PKG-INFO
```

### Comparing `izihawa_trident_client-1.2.2/trident/client.py` & `izihawa_trident_client-1.2.3/trident/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,22 @@
     async def blobs_get(self, hash_: str, timeout: float = None) -> bytes | None:
         url = f"/blobs/{hash_}"
         response = await self.get(url, timeout=timeout)
         if response is None:
             return None
         return await response.read()
 
+    async def blobs_get_chunks(self, hash_: str, timeout: float = None) -> AsyncGenerator[bytes, None]:
+        url = f"/blobs/{hash_}"
+        response = await self.get(url, timeout=timeout)
+        if response is None:
+            return
+        async for data, _ in response.content.iter_chunks():
+            yield data
+
     async def tables_ls(self) -> dict:
         response = await self.get(f"/tables/")
         return await response.json()
 
     async def tables_create(self, table: str, storage: str) -> bytes:
         url = f"/tables/{table}/"
         response = await self.post(url, params={'storage': storage})
```

### Comparing `izihawa_trident_client-1.2.2/PKG-INFO` & `izihawa_trident_client-1.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: izihawa-trident-client
-Version: 1.2.2
+Version: 1.2.3
 Summary: 
 Author: Pasha Podolsky
 Author-email: ppodolsky@me.com
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

