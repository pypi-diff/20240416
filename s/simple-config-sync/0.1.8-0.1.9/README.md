# Comparing `tmp/simple_config_sync-0.1.8.tar.gz` & `tmp/simple_config_sync-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_config_sync-0.1.8.tar", last modified: Tue Apr 16 15:12:08 2024, max compression
+gzip compressed data, was "simple_config_sync-0.1.9.tar", last modified: Tue Apr 16 15:13:27 2024, max compression
```

## Comparing `simple_config_sync-0.1.8.tar` & `simple_config_sync-0.1.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 hmeqo     (1000) hmeqo     (1000)        0 2024-04-16 15:12:08.408015 simple_config_sync-0.1.8/
--rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)      814 2024-04-16 15:12:08.408015 simple_config_sync-0.1.8/PKG-INFO
--rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)      360 2024-02-28 02:46:26.000000 simple_config_sync-0.1.8/README.md
--rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)      871 2024-04-16 15:12:00.000000 simple_config_sync-0.1.8/pyproject.toml
--rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)       38 2024-04-16 15:12:08.408015 simple_config_sync-0.1.8/setup.cfg
-drwxr-xr-x   0 hmeqo     (1000) hmeqo     (1000)        0 2024-04-16 15:12:08.406015 simple_config_sync-0.1.8/src/
-drwxr-xr-x   0 hmeqo     (1000) hmeqo     (1000)        0 2024-04-16 15:12:08.407015 simple_config_sync-0.1.8/src/simple_config_sync/
--rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)       42 2024-04-15 04:37:08.000000 simple_config_sync-0.1.8/src/simple_config_sync/__init__.py
--rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)       68 2024-04-15 04:37:08.000000 simple_config_sync-0.1.8/src/simple_config_sync/__main__.py
-drwxr-xr-x   0 hmeqo     (1000) hmeqo     (1000)        0 2024-04-16 15:12:08.408015 simple_config_sync-0.1.8/src/simple_config_sync/core/
--rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)      193 2024-04-15 04:37:08.000000 simple_config_sync-0.1.8/src/simple_config_sync/core/__init__.py
-drwxr-xr-x   0 hmeqo     (1000) hmeqo     (1000)        0 2024-04-16 15:12:08.408015 simple_config_sync-0.1.8/src/simple_config_sync/core/assets/
--rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)     1325 2024-04-15 04:37:08.000000 simple_config_sync-0.1.8/src/simple_config_sync/core/assets/tui.tcss
--rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)      222 2024-04-15 04:37:08.000000 simple_config_sync-0.1.8/src/simple_config_sync/core/cli.py
--rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)     5185 2024-04-16 15:11:23.000000 simple_config_sync-0.1.8/src/simple_config_sync/core/config.py
--rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)     3678 2024-04-16 15:04:47.000000 simple_config_sync-0.1.8/src/simple_config_sync/core/tui.py
-drwxr-xr-x   0 hmeqo     (1000) hmeqo     (1000)        0 2024-04-16 15:12:08.408015 simple_config_sync-0.1.8/src/simple_config_sync.egg-info/
--rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)      814 2024-04-16 15:12:08.000000 simple_config_sync-0.1.8/src/simple_config_sync.egg-info/PKG-INFO
--rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)      564 2024-04-16 15:12:08.000000 simple_config_sync-0.1.8/src/simple_config_sync.egg-info/SOURCES.txt
--rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)        1 2024-04-16 15:12:08.000000 simple_config_sync-0.1.8/src/simple_config_sync.egg-info/dependency_links.txt
--rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)      124 2024-04-16 15:12:08.000000 simple_config_sync-0.1.8/src/simple_config_sync.egg-info/entry_points.txt
--rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)       42 2024-04-16 15:12:08.000000 simple_config_sync-0.1.8/src/simple_config_sync.egg-info/requires.txt
--rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)       19 2024-04-16 15:12:08.000000 simple_config_sync-0.1.8/src/simple_config_sync.egg-info/top_level.txt
+drwxr-xr-x   0 hmeqo     (1000) hmeqo     (1000)        0 2024-04-16 15:13:27.604971 simple_config_sync-0.1.9/
+-rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)      814 2024-04-16 15:13:27.604971 simple_config_sync-0.1.9/PKG-INFO
+-rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)      360 2024-02-28 02:46:26.000000 simple_config_sync-0.1.9/README.md
+-rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)      871 2024-04-16 15:13:20.000000 simple_config_sync-0.1.9/pyproject.toml
+-rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)       38 2024-04-16 15:13:27.604971 simple_config_sync-0.1.9/setup.cfg
+drwxr-xr-x   0 hmeqo     (1000) hmeqo     (1000)        0 2024-04-16 15:13:27.602971 simple_config_sync-0.1.9/src/
+drwxr-xr-x   0 hmeqo     (1000) hmeqo     (1000)        0 2024-04-16 15:13:27.603971 simple_config_sync-0.1.9/src/simple_config_sync/
+-rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)       42 2024-04-16 15:13:08.000000 simple_config_sync-0.1.9/src/simple_config_sync/__init__.py
+-rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)       68 2024-04-15 04:37:08.000000 simple_config_sync-0.1.9/src/simple_config_sync/__main__.py
+drwxr-xr-x   0 hmeqo     (1000) hmeqo     (1000)        0 2024-04-16 15:13:27.604971 simple_config_sync-0.1.9/src/simple_config_sync/core/
+-rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)      193 2024-04-15 04:37:08.000000 simple_config_sync-0.1.9/src/simple_config_sync/core/__init__.py
+drwxr-xr-x   0 hmeqo     (1000) hmeqo     (1000)        0 2024-04-16 15:13:27.604971 simple_config_sync-0.1.9/src/simple_config_sync/core/assets/
+-rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)     1325 2024-04-15 04:37:08.000000 simple_config_sync-0.1.9/src/simple_config_sync/core/assets/tui.tcss
+-rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)      222 2024-04-15 04:37:08.000000 simple_config_sync-0.1.9/src/simple_config_sync/core/cli.py
+-rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)     5185 2024-04-16 15:11:23.000000 simple_config_sync-0.1.9/src/simple_config_sync/core/config.py
+-rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)     3678 2024-04-16 15:04:47.000000 simple_config_sync-0.1.9/src/simple_config_sync/core/tui.py
+drwxr-xr-x   0 hmeqo     (1000) hmeqo     (1000)        0 2024-04-16 15:13:27.604971 simple_config_sync-0.1.9/src/simple_config_sync.egg-info/
+-rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)      814 2024-04-16 15:13:27.000000 simple_config_sync-0.1.9/src/simple_config_sync.egg-info/PKG-INFO
+-rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)      564 2024-04-16 15:13:27.000000 simple_config_sync-0.1.9/src/simple_config_sync.egg-info/SOURCES.txt
+-rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)        1 2024-04-16 15:13:27.000000 simple_config_sync-0.1.9/src/simple_config_sync.egg-info/dependency_links.txt
+-rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)      124 2024-04-16 15:13:27.000000 simple_config_sync-0.1.9/src/simple_config_sync.egg-info/entry_points.txt
+-rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)       42 2024-04-16 15:13:27.000000 simple_config_sync-0.1.9/src/simple_config_sync.egg-info/requires.txt
+-rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)       19 2024-04-16 15:13:27.000000 simple_config_sync-0.1.9/src/simple_config_sync.egg-info/top_level.txt
```

### Comparing `simple_config_sync-0.1.8/PKG-INFO` & `simple_config_sync-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-config-sync
-Version: 0.1.8
+Version: 0.1.9
 Summary: Used for synchronizing dotfiles across various Linux devices, capable of automatically creating links, automatically deleting links, and selectively synchronizing files.
 Author-email: hmeqo <hmeqocoliniliad@gmail.com>
 License: MIT
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Requires-Dist: textual>=0.52.1
 Requires-Dist: toml>=0.10.2
```

### Comparing `simple_config_sync-0.1.8/pyproject.toml` & `simple_config_sync-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "simple-config-sync"
-version = "0.1.8"
+version = "0.1.9"
 description = "Used for synchronizing dotfiles across various Linux devices, capable of automatically creating links, automatically deleting links, and selectively synchronizing files."
 authors = [{ name = "hmeqo", email = "hmeqocoliniliad@gmail.com" }]
 dependencies = ["textual>=0.52.1", "toml>=0.10.2", "click>=8.1.7"]
 requires-python = ">=3.11"
 readme = "README.md"
 license = { text = "MIT" }
```

### Comparing `simple_config_sync-0.1.8/src/simple_config_sync/core/assets/tui.tcss` & `simple_config_sync-0.1.9/src/simple_config_sync/core/assets/tui.tcss`

 * *Files identical despite different names*

### Comparing `simple_config_sync-0.1.8/src/simple_config_sync/core/config.py` & `simple_config_sync-0.1.9/src/simple_config_sync/core/config.py`

 * *Files identical despite different names*

### Comparing `simple_config_sync-0.1.8/src/simple_config_sync/core/tui.py` & `simple_config_sync-0.1.9/src/simple_config_sync/core/tui.py`

 * *Files identical despite different names*

### Comparing `simple_config_sync-0.1.8/src/simple_config_sync.egg-info/PKG-INFO` & `simple_config_sync-0.1.9/src/simple_config_sync.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-config-sync
-Version: 0.1.8
+Version: 0.1.9
 Summary: Used for synchronizing dotfiles across various Linux devices, capable of automatically creating links, automatically deleting links, and selectively synchronizing files.
 Author-email: hmeqo <hmeqocoliniliad@gmail.com>
 License: MIT
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Requires-Dist: textual>=0.52.1
 Requires-Dist: toml>=0.10.2
```

### Comparing `simple_config_sync-0.1.8/src/simple_config_sync.egg-info/SOURCES.txt` & `simple_config_sync-0.1.9/src/simple_config_sync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

