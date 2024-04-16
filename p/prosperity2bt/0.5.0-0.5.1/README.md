# Comparing `tmp/prosperity2bt-0.5.0.tar.gz` & `tmp/prosperity2bt-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prosperity2bt-0.5.0.tar", last modified: Mon Apr 15 11:32:55 2024, max compression
+gzip compressed data, was "prosperity2bt-0.5.1.tar", last modified: Tue Apr 16 13:36:55 2024, max compression
```

## Comparing `prosperity2bt-0.5.0.tar` & `prosperity2bt-0.5.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:32:55.416466 prosperity2bt-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-15 11:32:50.000000 prosperity2bt-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5822 2024-04-15 11:32:55.412466 prosperity2bt-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-04-15 11:32:50.000000 prosperity2bt-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:32:55.392466 prosperity2bt-0.5.0/prosperity2bt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:32:50.000000 prosperity2bt-0.5.0/prosperity2bt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8461 2024-04-15 11:32:50.000000 prosperity2bt-0.5.0/prosperity2bt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-04-15 11:32:50.000000 prosperity2bt-0.5.0/prosperity2bt/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-15 11:32:50.000000 prosperity2bt-0.5.0/prosperity2bt/datamodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-15 11:32:50.000000 prosperity2bt-0.5.0/prosperity2bt/file_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-04-15 11:32:50.000000 prosperity2bt-0.5.0/prosperity2bt/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:32:55.396466 prosperity2bt-0.5.0/prosperity2bt/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:32:50.000000 prosperity2bt-0.5.0/prosperity2bt/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:32:55.396466 prosperity2bt-0.5.0/prosperity2bt/resources/round0/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:32:50.000000 prosperity2bt-0.5.0/prosperity2bt/resources/round0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   249265 2024-04-15 11:32:50.000000 prosperity2bt-0.5.0/prosperity2bt/resources/round0/prices_round_0_day_-2.csv
--rw-r--r--   0 runner    (1001) docker     (127)    38097 2024-04-15 11:32:50.000000 prosperity2bt-0.5.0/prosperity2bt/resources/round0/trades_round_0_day_-2_nn.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:32:55.404466 prosperity2bt-0.5.0/prosperity2bt/resources/round1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:32:50.000000 prosperity2bt-0.5.0/prosperity2bt/resources/round1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  1257340 2024-04-15 11:32:50.000000 prosperity2bt-0.5.0/prosperity2bt/resources/round1/prices_round_1_day_-1.csv
--rw-r--r--   0 runner    (1001) docker     (127)  1258643 2024-04-15 11:32:50.000000 prosperity2bt-0.5.0/prosperity2bt/resources/round1/prices_round_1_day_-2.csv
--rw-r--r--   0 runner    (1001) docker     (127)  1237383 2024-04-15 11:32:50.000000 prosperity2bt-0.5.0/prosperity2bt/resources/round1/prices_round_1_day_0.csv
--rw-r--r--   0 runner    (1001) docker     (127)   204939 2024-04-15 11:32:50.000000 prosperity2bt-0.5.0/prosperity2bt/resources/round1/trades_round_1_day_-1_nn.csv
--rw-r--r--   0 runner    (1001) docker     (127)   208522 2024-04-15 11:32:50.000000 prosperity2bt-0.5.0/prosperity2bt/resources/round1/trades_round_1_day_-2_nn.csv
--rw-r--r--   0 runner    (1001) docker     (127)   202884 2024-04-15 11:32:50.000000 prosperity2bt-0.5.0/prosperity2bt/resources/round1/trades_round_1_day_0_nn.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:32:55.412466 prosperity2bt-0.5.0/prosperity2bt/resources/round3/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:32:50.000000 prosperity2bt-0.5.0/prosperity2bt/resources/round3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  2581061 2024-04-15 11:32:50.000000 prosperity2bt-0.5.0/prosperity2bt/resources/round3/prices_round_3_day_0.csv
--rw-r--r--   0 runner    (1001) docker     (127)  2580446 2024-04-15 11:32:50.000000 prosperity2bt-0.5.0/prosperity2bt/resources/round3/prices_round_3_day_1.csv
--rw-r--r--   0 runner    (1001) docker     (127)  2580491 2024-04-15 11:32:50.000000 prosperity2bt-0.5.0/prosperity2bt/resources/round3/prices_round_3_day_2.csv
--rw-r--r--   0 runner    (1001) docker     (127)   148534 2024-04-15 11:32:50.000000 prosperity2bt-0.5.0/prosperity2bt/resources/round3/trades_round_3_day_0_nn.csv
--rw-r--r--   0 runner    (1001) docker     (127)   142870 2024-04-15 11:32:50.000000 prosperity2bt-0.5.0/prosperity2bt/resources/round3/trades_round_3_day_1_nn.csv
--rw-r--r--   0 runner    (1001) docker     (127)   146400 2024-04-15 11:32:50.000000 prosperity2bt-0.5.0/prosperity2bt/resources/round3/trades_round_3_day_2_nn.csv
--rw-r--r--   0 runner    (1001) docker     (127)     9660 2024-04-15 11:32:50.000000 prosperity2bt-0.5.0/prosperity2bt/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:32:55.412466 prosperity2bt-0.5.0/prosperity2bt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5822 2024-04-15 11:32:55.000000 prosperity2bt-0.5.0/prosperity2bt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-04-15 11:32:55.000000 prosperity2bt-0.5.0/prosperity2bt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 11:32:55.000000 prosperity2bt-0.5.0/prosperity2bt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-15 11:32:55.000000 prosperity2bt-0.5.0/prosperity2bt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-15 11:32:55.000000 prosperity2bt-0.5.0/prosperity2bt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-15 11:32:55.000000 prosperity2bt-0.5.0/prosperity2bt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-15 11:32:53.000000 prosperity2bt-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 11:32:55.416466 prosperity2bt-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:36:55.012262 prosperity2bt-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-16 13:36:48.000000 prosperity2bt-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5822 2024-04-16 13:36:55.012262 prosperity2bt-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-04-16 13:36:48.000000 prosperity2bt-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:36:54.992262 prosperity2bt-0.5.1/prosperity2bt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 13:36:48.000000 prosperity2bt-0.5.1/prosperity2bt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8740 2024-04-16 13:36:48.000000 prosperity2bt-0.5.1/prosperity2bt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-04-16 13:36:48.000000 prosperity2bt-0.5.1/prosperity2bt/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-16 13:36:48.000000 prosperity2bt-0.5.1/prosperity2bt/datamodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-16 13:36:48.000000 prosperity2bt-0.5.1/prosperity2bt/file_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-04-16 13:36:48.000000 prosperity2bt-0.5.1/prosperity2bt/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:36:54.992262 prosperity2bt-0.5.1/prosperity2bt/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 13:36:48.000000 prosperity2bt-0.5.1/prosperity2bt/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:36:54.996262 prosperity2bt-0.5.1/prosperity2bt/resources/round0/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 13:36:48.000000 prosperity2bt-0.5.1/prosperity2bt/resources/round0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   249265 2024-04-16 13:36:48.000000 prosperity2bt-0.5.1/prosperity2bt/resources/round0/prices_round_0_day_-2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    38097 2024-04-16 13:36:48.000000 prosperity2bt-0.5.1/prosperity2bt/resources/round0/trades_round_0_day_-2_nn.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:36:55.000262 prosperity2bt-0.5.1/prosperity2bt/resources/round1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 13:36:48.000000 prosperity2bt-0.5.1/prosperity2bt/resources/round1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1257340 2024-04-16 13:36:48.000000 prosperity2bt-0.5.1/prosperity2bt/resources/round1/prices_round_1_day_-1.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  1258643 2024-04-16 13:36:48.000000 prosperity2bt-0.5.1/prosperity2bt/resources/round1/prices_round_1_day_-2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  1237383 2024-04-16 13:36:48.000000 prosperity2bt-0.5.1/prosperity2bt/resources/round1/prices_round_1_day_0.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   204939 2024-04-16 13:36:48.000000 prosperity2bt-0.5.1/prosperity2bt/resources/round1/trades_round_1_day_-1_nn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   208522 2024-04-16 13:36:48.000000 prosperity2bt-0.5.1/prosperity2bt/resources/round1/trades_round_1_day_-2_nn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   202884 2024-04-16 13:36:48.000000 prosperity2bt-0.5.1/prosperity2bt/resources/round1/trades_round_1_day_0_nn.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:36:55.012262 prosperity2bt-0.5.1/prosperity2bt/resources/round3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 13:36:48.000000 prosperity2bt-0.5.1/prosperity2bt/resources/round3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  2581061 2024-04-16 13:36:48.000000 prosperity2bt-0.5.1/prosperity2bt/resources/round3/prices_round_3_day_0.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  2580446 2024-04-16 13:36:48.000000 prosperity2bt-0.5.1/prosperity2bt/resources/round3/prices_round_3_day_1.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  2580491 2024-04-16 13:36:48.000000 prosperity2bt-0.5.1/prosperity2bt/resources/round3/prices_round_3_day_2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   148534 2024-04-16 13:36:48.000000 prosperity2bt-0.5.1/prosperity2bt/resources/round3/trades_round_3_day_0_nn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   142870 2024-04-16 13:36:48.000000 prosperity2bt-0.5.1/prosperity2bt/resources/round3/trades_round_3_day_1_nn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   146400 2024-04-16 13:36:48.000000 prosperity2bt-0.5.1/prosperity2bt/resources/round3/trades_round_3_day_2_nn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     9660 2024-04-16 13:36:48.000000 prosperity2bt-0.5.1/prosperity2bt/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:36:55.012262 prosperity2bt-0.5.1/prosperity2bt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5822 2024-04-16 13:36:54.000000 prosperity2bt-0.5.1/prosperity2bt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-04-16 13:36:54.000000 prosperity2bt-0.5.1/prosperity2bt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 13:36:54.000000 prosperity2bt-0.5.1/prosperity2bt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-16 13:36:54.000000 prosperity2bt-0.5.1/prosperity2bt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-16 13:36:54.000000 prosperity2bt-0.5.1/prosperity2bt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-16 13:36:54.000000 prosperity2bt-0.5.1/prosperity2bt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-16 13:36:52.000000 prosperity2bt-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 13:36:55.012262 prosperity2bt-0.5.1/setup.cfg
```

### Comparing `prosperity2bt-0.5.0/LICENSE` & `prosperity2bt-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.5.0/PKG-INFO` & `prosperity2bt-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prosperity2bt
-Version: 0.5.0
+Version: 0.5.1
 Summary: Backtester for IMC Prosperity 2 algorithms
 Author-email: Jasper van Merle <jaspervmerle@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Jasper van Merle
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `prosperity2bt-0.5.0/README.md` & `prosperity2bt-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.5.0/prosperity2bt/__main__.py` & `prosperity2bt-0.5.1/prosperity2bt/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -152,16 +152,20 @@
 
     def log_message(self, format: str, *args: Any) -> None:
         return
 
 def open_visualizer(output_file: Path) -> None:
     http_handler = partial(HTTPRequestHandler, directory=output_file.parent)
     http_server = HTTPServer(("localhost", 0), http_handler)
+    http_server.timeout = 5
 
     webbrowser.open(f"https://jmerle.github.io/imc-prosperity-2-visualizer/?open=http://localhost:{http_server.server_port}/{output_file.name}")
+
+    # Chrome makes 2 requests: 1 OPTIONS request to check for CORS headers and 1 GET request to get the data
+    # Some users reported their browser only makes 1 request, in that case the second call is terminated after `http_server.timeout` seconds
     http_server.handle_request()
     http_server.handle_request()
 
 def format_path(path: Path) -> str:
     cwd = Path.cwd()
     if path.is_relative_to(cwd):
         return str(path.relative_to(cwd))
```

### Comparing `prosperity2bt-0.5.0/prosperity2bt/data.py` & `prosperity2bt-0.5.1/prosperity2bt/data.py`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.5.0/prosperity2bt/datamodel.py` & `prosperity2bt-0.5.1/prosperity2bt/datamodel.py`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.5.0/prosperity2bt/file_reader.py` & `prosperity2bt-0.5.1/prosperity2bt/file_reader.py`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.5.0/prosperity2bt/models.py` & `prosperity2bt-0.5.1/prosperity2bt/models.py`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.5.0/prosperity2bt/resources/round0/prices_round_0_day_-2.csv` & `prosperity2bt-0.5.1/prosperity2bt/resources/round0/prices_round_0_day_-2.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.5.0/prosperity2bt/resources/round0/trades_round_0_day_-2_nn.csv` & `prosperity2bt-0.5.1/prosperity2bt/resources/round0/trades_round_0_day_-2_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.5.0/prosperity2bt/resources/round1/prices_round_1_day_-1.csv` & `prosperity2bt-0.5.1/prosperity2bt/resources/round1/prices_round_1_day_-1.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.5.0/prosperity2bt/resources/round1/prices_round_1_day_-2.csv` & `prosperity2bt-0.5.1/prosperity2bt/resources/round1/prices_round_1_day_-2.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.5.0/prosperity2bt/resources/round1/prices_round_1_day_0.csv` & `prosperity2bt-0.5.1/prosperity2bt/resources/round1/prices_round_1_day_0.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.5.0/prosperity2bt/resources/round1/trades_round_1_day_-1_nn.csv` & `prosperity2bt-0.5.1/prosperity2bt/resources/round1/trades_round_1_day_-1_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.5.0/prosperity2bt/resources/round1/trades_round_1_day_-2_nn.csv` & `prosperity2bt-0.5.1/prosperity2bt/resources/round1/trades_round_1_day_-2_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.5.0/prosperity2bt/resources/round1/trades_round_1_day_0_nn.csv` & `prosperity2bt-0.5.1/prosperity2bt/resources/round1/trades_round_1_day_0_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.5.0/prosperity2bt/resources/round3/prices_round_3_day_0.csv` & `prosperity2bt-0.5.1/prosperity2bt/resources/round3/prices_round_3_day_0.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.5.0/prosperity2bt/resources/round3/prices_round_3_day_1.csv` & `prosperity2bt-0.5.1/prosperity2bt/resources/round3/prices_round_3_day_1.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.5.0/prosperity2bt/resources/round3/prices_round_3_day_2.csv` & `prosperity2bt-0.5.1/prosperity2bt/resources/round3/prices_round_3_day_2.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.5.0/prosperity2bt/resources/round3/trades_round_3_day_0_nn.csv` & `prosperity2bt-0.5.1/prosperity2bt/resources/round3/trades_round_3_day_0_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.5.0/prosperity2bt/resources/round3/trades_round_3_day_1_nn.csv` & `prosperity2bt-0.5.1/prosperity2bt/resources/round3/trades_round_3_day_1_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.5.0/prosperity2bt/resources/round3/trades_round_3_day_2_nn.csv` & `prosperity2bt-0.5.1/prosperity2bt/resources/round3/trades_round_3_day_2_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.5.0/prosperity2bt/runner.py` & `prosperity2bt-0.5.1/prosperity2bt/runner.py`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.5.0/prosperity2bt.egg-info/PKG-INFO` & `prosperity2bt-0.5.1/prosperity2bt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prosperity2bt
-Version: 0.5.0
+Version: 0.5.1
 Summary: Backtester for IMC Prosperity 2 algorithms
 Author-email: Jasper van Merle <jaspervmerle@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Jasper van Merle
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `prosperity2bt-0.5.0/prosperity2bt.egg-info/SOURCES.txt` & `prosperity2bt-0.5.1/prosperity2bt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.5.0/pyproject.toml` & `prosperity2bt-0.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "prosperity2bt"
 description = "Backtester for IMC Prosperity 2 algorithms"
-version = "0.5.0"
+version = "0.5.1"
 readme = "README.md"
 license = {file = "LICENSE"}
 authors = [{name = "Jasper van Merle", email = "jaspervmerle@gmail.com"}]
 keywords = ["imc", "prosperity", "backtest", "backtester"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
```

