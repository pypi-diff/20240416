# Comparing `tmp/wslink-2.0.0.tar.gz` & `tmp/wslink-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wslink-2.0.0.tar", last modified: Wed Apr 10 21:41:58 2024, max compression
+gzip compressed data, was "wslink-2.0.1.tar", last modified: Tue Apr 16 15:42:42 2024, max compression
```

## Comparing `wslink-2.0.0.tar` & `wslink-2.0.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:41:58.829609 wslink-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-10 21:41:28.000000 wslink-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-04-10 21:41:58.829609 wslink-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-04-10 21:41:28.000000 wslink-2.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-10 21:41:58.829609 wslink-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-04-10 21:41:28.000000 wslink-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:41:58.821609 wslink-2.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:41:58.825609 wslink-2.0.0/src/wslink/
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-10 21:41:28.000000 wslink-2.0.0/src/wslink/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-04-10 21:41:28.000000 wslink-2.0.0/src/wslink/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:41:58.825609 wslink-2.0.0/src/wslink/backends/
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-10 21:41:28.000000 wslink-2.0.0/src/wslink/backends/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:41:58.829609 wslink-2.0.0/src/wslink/backends/aiohttp/
--rw-r--r--   0 runner    (1001) docker     (127)     8463 2024-04-10 21:41:28.000000 wslink-2.0.0/src/wslink/backends/aiohttp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8897 2024-04-10 21:41:28.000000 wslink-2.0.0/src/wslink/backends/aiohttp/launcher.py
--rw-r--r--   0 runner    (1001) docker     (127)    13311 2024-04-10 21:41:28.000000 wslink-2.0.0/src/wslink/backends/aiohttp/relay.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:41:58.829609 wslink-2.0.0/src/wslink/backends/generic/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-10 21:41:28.000000 wslink-2.0.0/src/wslink/backends/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4149 2024-04-10 21:41:28.000000 wslink-2.0.0/src/wslink/backends/generic/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:41:58.829609 wslink-2.0.0/src/wslink/backends/jupyter/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-10 21:41:28.000000 wslink-2.0.0/src/wslink/backends/jupyter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3858 2024-04-10 21:41:28.000000 wslink-2.0.0/src/wslink/backends/jupyter/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:41:58.829609 wslink-2.0.0/src/wslink/backends/tornado/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-10 21:41:28.000000 wslink-2.0.0/src/wslink/backends/tornado/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-04-10 21:41:28.000000 wslink-2.0.0/src/wslink/backends/tornado/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     7130 2024-04-10 21:41:28.000000 wslink-2.0.0/src/wslink/chunking.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    21170 2024-04-10 21:41:28.000000 wslink-2.0.0/src/wslink/launcher.py
--rw-r--r--   0 runner    (1001) docker     (127)    15886 2024-04-10 21:41:28.000000 wslink-2.0.0/src/wslink/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-10 21:41:28.000000 wslink-2.0.0/src/wslink/publish.py
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-10 21:41:28.000000 wslink-2.0.0/src/wslink/relay.py
--rw-r--r--   0 runner    (1001) docker     (127)     9440 2024-04-10 21:41:28.000000 wslink-2.0.0/src/wslink/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-04-10 21:41:28.000000 wslink-2.0.0/src/wslink/ssl_context.py
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-10 21:41:28.000000 wslink-2.0.0/src/wslink/uri.py
--rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-04-10 21:41:28.000000 wslink-2.0.0/src/wslink/websocket.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:41:58.829609 wslink-2.0.0/src/wslink.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-04-10 21:41:58.000000 wslink-2.0.0/src/wslink.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-10 21:41:58.000000 wslink-2.0.0/src/wslink.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 21:41:58.000000 wslink-2.0.0/src/wslink.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-10 21:41:58.000000 wslink-2.0.0/src/wslink.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-10 21:41:58.000000 wslink-2.0.0/src/wslink.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:42:42.576406 wslink-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-16 15:42:08.000000 wslink-2.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-04-16 15:42:42.576406 wslink-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-04-16 15:42:08.000000 wslink-2.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-16 15:42:42.576406 wslink-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-04-16 15:42:08.000000 wslink-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:42:42.572406 wslink-2.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:42:42.576406 wslink-2.0.1/src/wslink/
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-16 15:42:08.000000 wslink-2.0.1/src/wslink/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-04-16 15:42:08.000000 wslink-2.0.1/src/wslink/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:42:42.576406 wslink-2.0.1/src/wslink/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-16 15:42:08.000000 wslink-2.0.1/src/wslink/backends/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:42:42.576406 wslink-2.0.1/src/wslink/backends/aiohttp/
+-rw-r--r--   0 runner    (1001) docker     (127)     8463 2024-04-16 15:42:08.000000 wslink-2.0.1/src/wslink/backends/aiohttp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8897 2024-04-16 15:42:08.000000 wslink-2.0.1/src/wslink/backends/aiohttp/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13311 2024-04-16 15:42:08.000000 wslink-2.0.1/src/wslink/backends/aiohttp/relay.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:42:42.576406 wslink-2.0.1/src/wslink/backends/generic/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-16 15:42:08.000000 wslink-2.0.1/src/wslink/backends/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4149 2024-04-16 15:42:08.000000 wslink-2.0.1/src/wslink/backends/generic/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:42:42.576406 wslink-2.0.1/src/wslink/backends/jupyter/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-16 15:42:08.000000 wslink-2.0.1/src/wslink/backends/jupyter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3858 2024-04-16 15:42:08.000000 wslink-2.0.1/src/wslink/backends/jupyter/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:42:42.576406 wslink-2.0.1/src/wslink/backends/tornado/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-16 15:42:08.000000 wslink-2.0.1/src/wslink/backends/tornado/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-04-16 15:42:08.000000 wslink-2.0.1/src/wslink/backends/tornado/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7130 2024-04-16 15:42:08.000000 wslink-2.0.1/src/wslink/chunking.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21170 2024-04-16 15:42:08.000000 wslink-2.0.1/src/wslink/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15886 2024-04-16 15:42:08.000000 wslink-2.0.1/src/wslink/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-16 15:42:08.000000 wslink-2.0.1/src/wslink/publish.py
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-16 15:42:08.000000 wslink-2.0.1/src/wslink/relay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9325 2024-04-16 15:42:08.000000 wslink-2.0.1/src/wslink/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-04-16 15:42:08.000000 wslink-2.0.1/src/wslink/ssl_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-16 15:42:08.000000 wslink-2.0.1/src/wslink/uri.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-04-16 15:42:08.000000 wslink-2.0.1/src/wslink/websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:42:42.576406 wslink-2.0.1/src/wslink.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-04-16 15:42:42.000000 wslink-2.0.1/src/wslink.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-16 15:42:42.000000 wslink-2.0.1/src/wslink.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 15:42:42.000000 wslink-2.0.1/src/wslink.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-16 15:42:42.000000 wslink-2.0.1/src/wslink.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-16 15:42:42.000000 wslink-2.0.1/src/wslink.egg-info/top_level.txt
```

### Comparing `wslink-2.0.0/PKG-INFO` & `wslink-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wslink
-Version: 2.0.0
+Version: 2.0.1
 Summary: Python/JavaScript library for communicating over WebSocket
 Home-page: https://github.com/kitware/wslink
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: BSD-3-Clause
 Keywords: websocket javascript rpc pubsub
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `wslink-2.0.0/README.rst` & `wslink-2.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `wslink-2.0.0/setup.py` & `wslink-2.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `wslink-2.0.0/src/wslink/LICENSE` & `wslink-2.0.1/src/wslink/LICENSE`

 * *Files identical despite different names*

### Comparing `wslink-2.0.0/src/wslink/__init__.py` & `wslink-2.0.1/src/wslink/__init__.py`

 * *Files identical despite different names*

### Comparing `wslink-2.0.0/src/wslink/backends/__init__.py` & `wslink-2.0.1/src/wslink/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `wslink-2.0.0/src/wslink/backends/aiohttp/__init__.py` & `wslink-2.0.1/src/wslink/backends/aiohttp/__init__.py`

 * *Files identical despite different names*

### Comparing `wslink-2.0.0/src/wslink/backends/aiohttp/launcher.py` & `wslink-2.0.1/src/wslink/backends/aiohttp/launcher.py`

 * *Files identical despite different names*

### Comparing `wslink-2.0.0/src/wslink/backends/aiohttp/relay.py` & `wslink-2.0.1/src/wslink/backends/aiohttp/relay.py`

 * *Files identical despite different names*

### Comparing `wslink-2.0.0/src/wslink/backends/generic/core.py` & `wslink-2.0.1/src/wslink/backends/generic/core.py`

 * *Files identical despite different names*

### Comparing `wslink-2.0.0/src/wslink/backends/jupyter/core.py` & `wslink-2.0.1/src/wslink/backends/jupyter/core.py`

 * *Files identical despite different names*

### Comparing `wslink-2.0.0/src/wslink/backends/tornado/core.py` & `wslink-2.0.1/src/wslink/backends/tornado/core.py`

 * *Files identical despite different names*

### Comparing `wslink-2.0.0/src/wslink/chunking.py` & `wslink-2.0.1/src/wslink/chunking.py`

 * *Files identical despite different names*

### Comparing `wslink-2.0.0/src/wslink/launcher.py` & `wslink-2.0.1/src/wslink/launcher.py`

 * *Files identical despite different names*

### Comparing `wslink-2.0.0/src/wslink/protocol.py` & `wslink-2.0.1/src/wslink/protocol.py`

 * *Files identical despite different names*

### Comparing `wslink-2.0.0/src/wslink/publish.py` & `wslink-2.0.1/src/wslink/publish.py`

 * *Files identical despite different names*

### Comparing `wslink-2.0.0/src/wslink/server.py` & `wslink-2.0.1/src/wslink/server.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,74 +14,68 @@
 from wslink import backends
 
 ws_server = None
 
 
 # =============================================================================
 # Setup default arguments to be parsed
-#   -s, --nosignalhandlers
-#   -d, --debug
-#   -i, --host     localhost
+#   --nosignalhandlers
+#   --debug
+#   --host     localhost
 #   -p, --port     8080
-#   -t, --timeout  300 (seconds)
-#   -c, --content  '/www'  (No content means WebSocket only)
-#   -a, --authKey  vtkweb-secret
+#   --timeout  300 (seconds)
+#   --content  '/www'  (No content means WebSocket only)
+#   --authKey  vtkweb-secret
 # =============================================================================
 
 
 def add_arguments(parser):
     """
     Add arguments known to this module. parser must be
     argparse.ArgumentParser instance.
     """
 
     parser.add_argument(
-        "-d", "--debug", help="log debugging messages to stdout", action="store_true"
+        "--debug", help="log debugging messages to stdout", action="store_true"
     )
     parser.add_argument(
-        "-s",
         "--nosignalhandlers",
         help="Prevent installation of signal handlers so server can be started inside a thread.",
         action="store_true",
     )
     parser.add_argument(
-        "-i",
         "--host",
         type=str,
         default="localhost",
         help="the interface for the web-server to listen on (default: 0.0.0.0)",
     )
     parser.add_argument(
         "-p",
         "--port",
         type=int,
         default=8080,
         help="port number for the web-server to listen on (default: 8080)",
     )
     parser.add_argument(
-        "-t",
         "--timeout",
         type=int,
         default=300,
         help="timeout for reaping process on idle in seconds (default: 300s, 0 to disable)",
     )
     parser.add_argument(
-        "-c",
         "--content",
         default="",
         help="root for web-pages to serve (default: none)",
     )
     parser.add_argument(
-        "-a",
         "--authKey",
         default="wslink-secret",
         help="Authentication key for clients to connect to the WebSocket.",
     )
     parser.add_argument(
-        "-ws",
         "--ws-endpoint",
         type=str,
         default="ws",
         dest="ws",
         help="Specify WebSocket endpoint. (e.g. foo/bar/ws, Default: ws)",
     )
     parser.add_argument(
```

### Comparing `wslink-2.0.0/src/wslink/ssl_context.py` & `wslink-2.0.1/src/wslink/ssl_context.py`

 * *Files identical despite different names*

### Comparing `wslink-2.0.0/src/wslink/websocket.py` & `wslink-2.0.1/src/wslink/websocket.py`

 * *Files identical despite different names*

### Comparing `wslink-2.0.0/src/wslink.egg-info/PKG-INFO` & `wslink-2.0.1/src/wslink.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wslink
-Version: 2.0.0
+Version: 2.0.1
 Summary: Python/JavaScript library for communicating over WebSocket
 Home-page: https://github.com/kitware/wslink
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: BSD-3-Clause
 Keywords: websocket javascript rpc pubsub
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `wslink-2.0.0/src/wslink.egg-info/SOURCES.txt` & `wslink-2.0.1/src/wslink.egg-info/SOURCES.txt`

 * *Files identical despite different names*

