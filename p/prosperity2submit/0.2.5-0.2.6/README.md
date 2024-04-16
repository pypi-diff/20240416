# Comparing `tmp/prosperity2submit-0.2.5.tar.gz` & `tmp/prosperity2submit-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prosperity2submit-0.2.5.tar", last modified: Sat Apr 13 14:28:44 2024, max compression
+gzip compressed data, was "prosperity2submit-0.2.6.tar", last modified: Tue Apr 16 13:38:09 2024, max compression
```

## Comparing `prosperity2submit-0.2.5.tar` & `prosperity2submit-0.2.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:28:44.865189 prosperity2submit-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-13 14:28:40.000000 prosperity2submit-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4727 2024-04-13 14:28:44.865189 prosperity2submit-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-04-13 14:28:40.000000 prosperity2submit-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:28:44.865189 prosperity2submit-0.2.5/prosperity2submit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 14:28:40.000000 prosperity2submit-0.2.5/prosperity2submit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-13 14:28:40.000000 prosperity2submit-0.2.5/prosperity2submit/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6871 2024-04-13 14:28:40.000000 prosperity2submit-0.2.5/prosperity2submit/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:28:44.865189 prosperity2submit-0.2.5/prosperity2submit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4727 2024-04-13 14:28:44.000000 prosperity2submit-0.2.5/prosperity2submit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-13 14:28:44.000000 prosperity2submit-0.2.5/prosperity2submit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 14:28:44.000000 prosperity2submit-0.2.5/prosperity2submit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-13 14:28:44.000000 prosperity2submit-0.2.5/prosperity2submit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-13 14:28:44.000000 prosperity2submit-0.2.5/prosperity2submit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-13 14:28:44.000000 prosperity2submit-0.2.5/prosperity2submit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-13 14:28:42.000000 prosperity2submit-0.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 14:28:44.865189 prosperity2submit-0.2.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:38:09.280030 prosperity2submit-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-16 13:38:05.000000 prosperity2submit-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4727 2024-04-16 13:38:09.280030 prosperity2submit-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-04-16 13:38:05.000000 prosperity2submit-0.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:38:09.280030 prosperity2submit-0.2.6/prosperity2submit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 13:38:05.000000 prosperity2submit-0.2.6/prosperity2submit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-16 13:38:05.000000 prosperity2submit-0.2.6/prosperity2submit/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7147 2024-04-16 13:38:05.000000 prosperity2submit-0.2.6/prosperity2submit/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:38:09.280030 prosperity2submit-0.2.6/prosperity2submit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4727 2024-04-16 13:38:09.000000 prosperity2submit-0.2.6/prosperity2submit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-16 13:38:09.000000 prosperity2submit-0.2.6/prosperity2submit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 13:38:09.000000 prosperity2submit-0.2.6/prosperity2submit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-16 13:38:09.000000 prosperity2submit-0.2.6/prosperity2submit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-16 13:38:09.000000 prosperity2submit-0.2.6/prosperity2submit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-16 13:38:09.000000 prosperity2submit-0.2.6/prosperity2submit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-16 13:38:07.000000 prosperity2submit-0.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 13:38:09.280030 prosperity2submit-0.2.6/setup.cfg
```

### Comparing `prosperity2submit-0.2.5/LICENSE` & `prosperity2submit-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `prosperity2submit-0.2.5/PKG-INFO` & `prosperity2submit-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prosperity2submit
-Version: 0.2.5
+Version: 0.2.6
 Summary: Command-line submitter for IMC Prosperity 2 algorithms
 Author-email: Jasper van Merle <jaspervmerle@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Jasper van Merle
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `prosperity2submit-0.2.5/README.md` & `prosperity2submit-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `prosperity2submit-0.2.5/prosperity2submit/__main__.py` & `prosperity2submit-0.2.6/prosperity2submit/__main__.py`

 * *Files identical despite different names*

### Comparing `prosperity2submit-0.2.5/prosperity2submit/core.py` & `prosperity2submit-0.2.6/prosperity2submit/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -159,19 +159,23 @@
     def end_headers(self) -> None:
         self.send_header("Access-Control-Allow-Origin", "*")
         return super().end_headers()
 
     def log_message(self, format: str, *args: Any) -> None:
         return
 
-def open_in_visualizer(output_file: Path) -> None:
+def open_visualizer(output_file: Path) -> None:
     http_handler = partial(HTTPRequestHandler, directory=output_file.parent)
     http_server = HTTPServer(("localhost", 0), http_handler)
+    http_server.timeout = 5
 
     webbrowser.open(f"https://jmerle.github.io/imc-prosperity-2-visualizer/?open=http://localhost:{http_server.server_port}/{output_file.name}")
+
+    # Chrome makes 2 requests: 1 OPTIONS request to check for CORS headers and 1 GET request to get the data
+    # Some users reported their browser only makes 1 request, in that case the second call is terminated after `http_server.timeout` seconds
     http_server.handle_request()
     http_server.handle_request()
 
 def submit(algorithm_file: Path, output_file: Optional[Path], open_visualizer: bool) -> None:
     round = get_current_round()
 
     submit_algorithm(algorithm_file)
```

### Comparing `prosperity2submit-0.2.5/prosperity2submit.egg-info/PKG-INFO` & `prosperity2submit-0.2.6/prosperity2submit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prosperity2submit
-Version: 0.2.5
+Version: 0.2.6
 Summary: Command-line submitter for IMC Prosperity 2 algorithms
 Author-email: Jasper van Merle <jaspervmerle@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Jasper van Merle
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `prosperity2submit-0.2.5/pyproject.toml` & `prosperity2submit-0.2.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "prosperity2submit"
 description = "Command-line submitter for IMC Prosperity 2 algorithms"
-version = "0.2.5"
+version = "0.2.6"
 readme = "README.md"
 license = {file = "LICENSE"}
 authors = [{name = "Jasper van Merle", email = "jaspervmerle@gmail.com"}]
 keywords = ["imc", "prosperity", "submit", "submitter"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
```

