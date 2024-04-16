# Comparing `tmp/simple_config_sync-0.1.6.tar.gz` & `tmp/simple_config_sync-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_config_sync-0.1.6.tar", last modified: Mon Apr 15 04:27:03 2024, max compression
+gzip compressed data, was "simple_config_sync-0.1.7.tar", last modified: Tue Apr 16 14:28:31 2024, max compression
```

## Comparing `simple_config_sync-0.1.6.tar` & `simple_config_sync-0.1.7.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 hmeqo     (1000) hmeqo     (1000)        0 2024-04-15 04:27:03.694870 simple_config_sync-0.1.6/
--rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)      814 2024-04-15 04:27:03.694870 simple_config_sync-0.1.6/PKG-INFO
--rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)      360 2024-02-28 02:46:26.000000 simple_config_sync-0.1.6/README.md
--rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)      798 2024-04-15 04:03:46.000000 simple_config_sync-0.1.6/pyproject.toml
--rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)       38 2024-04-15 04:27:03.694870 simple_config_sync-0.1.6/setup.cfg
-drwxr-xr-x   0 hmeqo     (1000) hmeqo     (1000)        0 2024-04-15 04:27:03.692870 simple_config_sync-0.1.6/src/
-drwxr-xr-x   0 hmeqo     (1000) hmeqo     (1000)        0 2024-04-15 04:27:03.693870 simple_config_sync-0.1.6/src/simple_config_sync/
--rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)       42 2024-04-15 04:03:32.000000 simple_config_sync-0.1.6/src/simple_config_sync/__init__.py
--rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)       68 2024-04-15 04:00:21.000000 simple_config_sync-0.1.6/src/simple_config_sync/__main__.py
-drwxr-xr-x   0 hmeqo     (1000) hmeqo     (1000)        0 2024-04-15 04:27:03.694870 simple_config_sync-0.1.6/src/simple_config_sync/core/
--rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)      193 2024-04-15 03:59:59.000000 simple_config_sync-0.1.6/src/simple_config_sync/core/__init__.py
--rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)      222 2024-04-15 04:09:41.000000 simple_config_sync-0.1.6/src/simple_config_sync/core/cli.py
--rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)     5052 2024-04-15 03:33:48.000000 simple_config_sync-0.1.6/src/simple_config_sync/core/config.py
--rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)     3649 2024-04-15 03:58:29.000000 simple_config_sync-0.1.6/src/simple_config_sync/core/tui.py
-drwxr-xr-x   0 hmeqo     (1000) hmeqo     (1000)        0 2024-04-15 04:27:03.694870 simple_config_sync-0.1.6/src/simple_config_sync.egg-info/
--rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)      814 2024-04-15 04:27:03.000000 simple_config_sync-0.1.6/src/simple_config_sync.egg-info/PKG-INFO
--rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)      520 2024-04-15 04:27:03.000000 simple_config_sync-0.1.6/src/simple_config_sync.egg-info/SOURCES.txt
--rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)        1 2024-04-15 04:27:03.000000 simple_config_sync-0.1.6/src/simple_config_sync.egg-info/dependency_links.txt
--rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)      124 2024-04-15 04:27:03.000000 simple_config_sync-0.1.6/src/simple_config_sync.egg-info/entry_points.txt
--rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)       42 2024-04-15 04:27:03.000000 simple_config_sync-0.1.6/src/simple_config_sync.egg-info/requires.txt
--rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)       19 2024-04-15 04:27:03.000000 simple_config_sync-0.1.6/src/simple_config_sync.egg-info/top_level.txt
+drwxr-xr-x   0 hmeqo     (1000) hmeqo     (1000)        0 2024-04-16 14:28:31.304746 simple_config_sync-0.1.7/
+-rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)      814 2024-04-16 14:28:31.304746 simple_config_sync-0.1.7/PKG-INFO
+-rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)      360 2024-02-28 02:46:26.000000 simple_config_sync-0.1.7/README.md
+-rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)      871 2024-04-16 14:25:33.000000 simple_config_sync-0.1.7/pyproject.toml
+-rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)       38 2024-04-16 14:28:31.304746 simple_config_sync-0.1.7/setup.cfg
+drwxr-xr-x   0 hmeqo     (1000) hmeqo     (1000)        0 2024-04-16 14:28:31.301746 simple_config_sync-0.1.7/src/
+drwxr-xr-x   0 hmeqo     (1000) hmeqo     (1000)        0 2024-04-16 14:28:31.302746 simple_config_sync-0.1.7/src/simple_config_sync/
+-rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)       42 2024-04-15 04:37:08.000000 simple_config_sync-0.1.7/src/simple_config_sync/__init__.py
+-rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)       68 2024-04-15 04:37:08.000000 simple_config_sync-0.1.7/src/simple_config_sync/__main__.py
+drwxr-xr-x   0 hmeqo     (1000) hmeqo     (1000)        0 2024-04-16 14:28:31.303746 simple_config_sync-0.1.7/src/simple_config_sync/core/
+-rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)      193 2024-04-15 04:37:08.000000 simple_config_sync-0.1.7/src/simple_config_sync/core/__init__.py
+drwxr-xr-x   0 hmeqo     (1000) hmeqo     (1000)        0 2024-04-16 14:28:31.303746 simple_config_sync-0.1.7/src/simple_config_sync/core/assets/
+-rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)     1325 2024-04-15 04:37:08.000000 simple_config_sync-0.1.7/src/simple_config_sync/core/assets/tui.tcss
+-rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)      222 2024-04-15 04:37:08.000000 simple_config_sync-0.1.7/src/simple_config_sync/core/cli.py
+-rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)     5052 2024-04-15 04:37:08.000000 simple_config_sync-0.1.7/src/simple_config_sync/core/config.py
+-rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)     3649 2024-04-15 04:37:08.000000 simple_config_sync-0.1.7/src/simple_config_sync/core/tui.py
+drwxr-xr-x   0 hmeqo     (1000) hmeqo     (1000)        0 2024-04-16 14:28:31.303746 simple_config_sync-0.1.7/src/simple_config_sync.egg-info/
+-rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)      814 2024-04-16 14:28:31.000000 simple_config_sync-0.1.7/src/simple_config_sync.egg-info/PKG-INFO
+-rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)      564 2024-04-16 14:28:31.000000 simple_config_sync-0.1.7/src/simple_config_sync.egg-info/SOURCES.txt
+-rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)        1 2024-04-16 14:28:31.000000 simple_config_sync-0.1.7/src/simple_config_sync.egg-info/dependency_links.txt
+-rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)      124 2024-04-16 14:28:31.000000 simple_config_sync-0.1.7/src/simple_config_sync.egg-info/entry_points.txt
+-rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)       42 2024-04-16 14:28:31.000000 simple_config_sync-0.1.7/src/simple_config_sync.egg-info/requires.txt
+-rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)       19 2024-04-16 14:28:31.000000 simple_config_sync-0.1.7/src/simple_config_sync.egg-info/top_level.txt
```

### Comparing `simple_config_sync-0.1.6/PKG-INFO` & `simple_config_sync-0.1.7/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-config-sync
-Version: 0.1.6
+Version: 0.1.7
 Summary: Used for synchronizing dotfiles across various Linux devices, capable of automatically creating links, automatically deleting links, and selectively synchronizing files.
 Author-email: hmeqo <hmeqocoliniliad@gmail.com>
 License: MIT
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Requires-Dist: textual>=0.52.1
 Requires-Dist: toml>=0.10.2
```

### Comparing `simple_config_sync-0.1.6/pyproject.toml` & `simple_config_sync-0.1.7/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "simple-config-sync"
-version = "0.1.6"
+version = "0.1.7"
 description = "Used for synchronizing dotfiles across various Linux devices, capable of automatically creating links, automatically deleting links, and selectively synchronizing files."
 authors = [{ name = "hmeqo", email = "hmeqocoliniliad@gmail.com" }]
 dependencies = ["textual>=0.52.1", "toml>=0.10.2", "click>=8.1.7"]
 requires-python = ">=3.11"
 readme = "README.md"
 license = { text = "MIT" }
 
@@ -12,14 +12,17 @@
 simpleconfigsync = "simple_config_sync.core:run_cli"
 simpleconfigsync-tui = "simple_config_sync.core:run_tui"
 
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
+[tool.setuptools.package-data]
+"simple_config_sync.core.assets" = ["*"]
+
 [tool.ruff]
 line-length = 120
 
 [tool.ruff.lint]
 ignore = ["F401", "F403", "F405"]
 
 [tool.ruff.format]
```

### Comparing `simple_config_sync-0.1.6/src/simple_config_sync/core/config.py` & `simple_config_sync-0.1.7/src/simple_config_sync/core/config.py`

 * *Files identical despite different names*

### Comparing `simple_config_sync-0.1.6/src/simple_config_sync/core/tui.py` & `simple_config_sync-0.1.7/src/simple_config_sync/core/tui.py`

 * *Files identical despite different names*

### Comparing `simple_config_sync-0.1.6/src/simple_config_sync.egg-info/PKG-INFO` & `simple_config_sync-0.1.7/src/simple_config_sync.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-config-sync
-Version: 0.1.6
+Version: 0.1.7
 Summary: Used for synchronizing dotfiles across various Linux devices, capable of automatically creating links, automatically deleting links, and selectively synchronizing files.
 Author-email: hmeqo <hmeqocoliniliad@gmail.com>
 License: MIT
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Requires-Dist: textual>=0.52.1
 Requires-Dist: toml>=0.10.2
```

### Comparing `simple_config_sync-0.1.6/src/simple_config_sync.egg-info/SOURCES.txt` & `simple_config_sync-0.1.7/src/simple_config_sync.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -7,8 +7,9 @@
 src/simple_config_sync.egg-info/dependency_links.txt
 src/simple_config_sync.egg-info/entry_points.txt
 src/simple_config_sync.egg-info/requires.txt
 src/simple_config_sync.egg-info/top_level.txt
 src/simple_config_sync/core/__init__.py
 src/simple_config_sync/core/cli.py
 src/simple_config_sync/core/config.py
-src/simple_config_sync/core/tui.py
+src/simple_config_sync/core/tui.py
+src/simple_config_sync/core/assets/tui.tcss
```

