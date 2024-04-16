# Comparing `tmp/prerun-0.1.8.tar.gz` & `tmp/prerun-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prerun-0.1.8.tar", last modified: Tue Apr 16 04:23:13 2024, max compression
+gzip compressed data, was "prerun-1.0.0.tar", last modified: Tue Apr 16 07:48:41 2024, max compression
```

## Comparing `prerun-0.1.8.tar` & `prerun-1.0.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:23:13.143890 prerun-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-16 04:23:06.000000 prerun-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-16 04:23:13.143890 prerun-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-16 04:23:06.000000 prerun-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-16 04:23:06.000000 prerun-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 04:23:13.143890 prerun-0.1.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:23:13.139890 prerun-0.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:23:13.143890 prerun-0.1.8/src/prerun/
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-16 04:23:06.000000 prerun-0.1.8/src/prerun/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-16 04:23:06.000000 prerun-0.1.8/src/prerun/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-16 04:23:06.000000 prerun-0.1.8/src/prerun/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-16 04:23:06.000000 prerun-0.1.8/src/prerun/recv_bytes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-04-16 04:23:06.000000 prerun-0.1.8/src/prerun/server.py
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-16 04:23:06.000000 prerun-0.1.8/src/prerun/sigint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:23:13.143890 prerun-0.1.8/src/prerun.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-16 04:23:13.000000 prerun-0.1.8/src/prerun.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-16 04:23:13.000000 prerun-0.1.8/src/prerun.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 04:23:13.000000 prerun-0.1.8/src/prerun.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-16 04:23:13.000000 prerun-0.1.8/src/prerun.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-16 04:23:13.000000 prerun-0.1.8/src/prerun.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-16 04:23:13.000000 prerun-0.1.8/src/prerun.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:48:41.524508 prerun-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-16 07:48:36.000000 prerun-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-16 07:48:41.524508 prerun-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-16 07:48:36.000000 prerun-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-16 07:48:36.000000 prerun-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 07:48:41.524508 prerun-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:48:41.524508 prerun-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:48:41.524508 prerun-1.0.0/src/prerun/
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-16 07:48:36.000000 prerun-1.0.0/src/prerun/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-16 07:48:36.000000 prerun-1.0.0/src/prerun/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-16 07:48:36.000000 prerun-1.0.0/src/prerun/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-16 07:48:36.000000 prerun-1.0.0/src/prerun/recv_bytes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-04-16 07:48:36.000000 prerun-1.0.0/src/prerun/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-16 07:48:36.000000 prerun-1.0.0/src/prerun/sigint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:48:41.524508 prerun-1.0.0/src/prerun.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-16 07:48:41.000000 prerun-1.0.0/src/prerun.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-16 07:48:41.000000 prerun-1.0.0/src/prerun.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 07:48:41.000000 prerun-1.0.0/src/prerun.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-16 07:48:41.000000 prerun-1.0.0/src/prerun.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-16 07:48:41.000000 prerun-1.0.0/src/prerun.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-16 07:48:41.000000 prerun-1.0.0/src/prerun.egg-info/top_level.txt
```

### Comparing `prerun-0.1.8/LICENSE` & `prerun-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prerun-0.1.8/PKG-INFO` & `prerun-1.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prerun
-Version: 0.1.8
+Version: 1.0.0
 Summary: Prerun
 License: Copyright (c) <year> <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
         use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
@@ -23,13 +23,13 @@
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/sfanxiang/prerun
 Keywords: development
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: psutil>=5.9.0
 
 # Prerun
```

### Comparing `prerun-0.1.8/pyproject.toml` & `prerun-1.0.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "prerun"
-version = "0.1.8"
+version = "1.0.0"
 description = "Prerun"
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 license = {file = "LICENSE"}
 keywords = ["development"]
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
 ]
```

### Comparing `prerun-0.1.8/src/prerun/client.py` & `prerun-1.0.0/src/prerun/client.py`

 * *Files identical despite different names*

### Comparing `prerun-0.1.8/src/prerun/server.py` & `prerun-1.0.0/src/prerun/server.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import code
 import json
 import multiprocessing
 import os
 import runpy
 import secrets
 import signal
 import socket
@@ -37,16 +38,25 @@
     sys.stdin = open(0, closefd=False)
 
     os.environ.clear()
     for k, v in data["environ"].items():
         os.environ[k] = v
     os.chdir(data["cwd"])
 
-    sys.argv = list(data["args"])
-    runpy.run_path(data["args"][0], run_name="__main__")
+    if not data["args"]:
+        import readline
+        import rlcompleter
+
+        code_locals = {}
+        readline.set_completer(rlcompleter.Completer(code_locals).complete)
+        readline.parse_and_bind("tab: complete")
+        code.interact(local=code_locals, exitmsg="")
+    else:
+        sys.argv = list(data["args"])
+        runpy.run_path(data["args"][0], run_name="__main__")
 
 
 def run(stdio, preloader, conn, socks_to_close):
     sigint_defer()
 
     for s in socks_to_close:
         s.close()
@@ -75,15 +85,16 @@
         if p.exitcode is None:
             for child in proc.children(recursive=True):
                 child.kill()
             proc.kill()
         raise
 
     try:
-        sigint_once()
+        if data["args"]:
+            sigint_once()
         try:
             c1.send({"args": data["args"], "cwd": data["cwd"], "environ": data["environ"]})
         except:
             pass
         c1.close()
         p.join()
         sigint_defer()
@@ -157,15 +168,25 @@
 def server(args):
     multiprocessing.set_start_method("fork")
 
     sigint_defer()
     stdio = [os.dup(0)]
     os.set_inheritable(stdio[0], True)
 
-    preloader, num_proc = args[0], int(args[1])
+    if len(args) < 1:
+        sys.stderr.write("Expected server argument.\n\nSee --help for more information.\n\n")
+        return 1
+    preloader = args[0]
+    num_proc = 4
+    if len(args) > 1:
+        try:
+            num_proc = int(args[1])
+        except ValueError:
+            sys.stderr.write("Number of processes must be an integer.\n\nSee --help for more information.\n\n")
+            return 1
 
     sock = socket.socket(socket.AF_UNIX, socket.SOCK_STREAM)
     sock_path = secrets.token_hex(16)
     sock_path = f"/tmp/prerun_{sock_path}"
     sock.bind(sock_path)
     sock.listen()
```

### Comparing `prerun-0.1.8/src/prerun/sigint.py` & `prerun-1.0.0/src/prerun/sigint.py`

 * *Files identical despite different names*

### Comparing `prerun-0.1.8/src/prerun.egg-info/PKG-INFO` & `prerun-1.0.0/src/prerun.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prerun
-Version: 0.1.8
+Version: 1.0.0
 Summary: Prerun
 License: Copyright (c) <year> <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
         use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
@@ -23,13 +23,13 @@
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/sfanxiang/prerun
 Keywords: development
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: psutil>=5.9.0
 
 # Prerun
```

