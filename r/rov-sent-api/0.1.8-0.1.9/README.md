# Comparing `tmp/rov_sent_api-0.1.8.tar.gz` & `tmp/rov_sent_api-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rov_sent_api-0.1.8.tar", max compression
+gzip compressed data, was "rov_sent_api-0.1.9.tar", max compression
```

## Comparing `rov_sent_api-0.1.8.tar` & `rov_sent_api-0.1.9.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      332 2023-11-14 21:04:26.296941 rov_sent_api-0.1.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-11-08 16:10:42.786424 rov_sent_api-0.1.8/README.md
--rw-r--r--   0        0        0        0 2023-11-08 16:10:42.786424 rov_sent_api-0.1.8/rov_sent_api/__init__.py
--rw-r--r--   0        0        0     6796 2023-11-14 21:04:10.687427 rov_sent_api-0.1.8/rov_sent_api/sentinel_api.py
--rw-r--r--   0        0        0      532 1970-01-01 00:00:00.000000 rov_sent_api-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      332 2023-11-15 17:44:09.149129 rov_sent_api-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-11-08 16:10:42.786424 rov_sent_api-0.1.9/README.md
+-rw-r--r--   0        0        0        0 2023-11-08 16:10:42.786424 rov_sent_api-0.1.9/rov_sent_api/__init__.py
+-rw-r--r--   0        0        0     6879 2023-11-15 17:42:38.519607 rov_sent_api-0.1.9/rov_sent_api/sentinel_api.py
+-rw-r--r--   0        0        0      532 1970-01-01 00:00:00.000000 rov_sent_api-0.1.9/PKG-INFO
```

### Comparing `rov_sent_api-0.1.8/rov_sent_api/sentinel_api.py` & `rov_sent_api-0.1.9/rov_sent_api/sentinel_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,38 +119,38 @@
             str: the absolute path of the downloaded product
         """
         access_token = self._get_access_token()
         url = f"{self.download_url}/Products({uuid})/$value"
 
         headers = {"Authorization": f"Bearer {access_token}"}
 
-        session = requests.Session()
-        session.headers.update(headers)
-        response = session.get(url, headers=headers, stream=True)
-
-        info = self.info(uuid)
-        title = info["title"] + ".zip"
-        final_path = os.path.join(path, title)
-
-        total_size = info["size"]
-        chunk_size = 8192
-        with open(final_path, "wb") as file:
-            for i, chunk in enumerate(response.iter_content(chunk_size=chunk_size)):
-                if chunk:
-                    file.write(chunk)
-
-                    # calculate current percentage
-                    c = i * chunk_size / total_size * 100
-                    # write current % to console, pause for .1ms, then flush console
-                    sys.stdout.write(
-                        f"\r{title} {i*chunk_size} / {total_size} ({round(c, 4)}%)"
-                    )
-                    sys.stdout.flush()
+        with requests.Session() as session:
+            session.headers.update(headers)
+            response = session.get(url, headers=headers, stream=True)
+
+            info = self.info(uuid)
+            title = info["title"] + ".zip"
+            final_path = os.path.join(path, title)
+
+            total_size = info["size"]
+            chunk_size = 8192
+            with open(final_path, "wb") as file:
+                for i, chunk in enumerate(response.iter_content(chunk_size=chunk_size)):
+                    if chunk:
+                        file.write(chunk)
+
+                        # calculate current percentage
+                        c = i * chunk_size / total_size * 100
+                        # write current % to console, pause for .1ms, then flush console
+                        sys.stdout.write(
+                            f"\r{title} {i*chunk_size} / {total_size} ({round(c, 4)}%)"
+                        )
+                        sys.stdout.flush()
 
-        return os.path.abspath(final_path)
+            return os.path.abspath(final_path)
     
     def is_online(self, uuid:str) -> bool:
         """Test if this product is online for 
 
         Args:
             uuid (str): the uuid of the product to test
```

### Comparing `rov_sent_api-0.1.8/PKG-INFO` & `rov_sent_api-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rov-sent-api
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 Author: Pablo Cano
 Author-email: pablo.cano@rovisen.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

