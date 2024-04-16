# Comparing `tmp/torrent_tool-0.0.3.1.tar.gz` & `tmp/torrent_tool-0.0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torrent_tool-0.0.3.1.tar", max compression
+gzip compressed data, was "torrent_tool-0.0.3.2.tar", max compression
```

## Comparing `torrent_tool-0.0.3.1.tar` & `torrent_tool-0.0.3.2.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 torrent_tool-0.0.3.1/LICENSE
--rw-r--r--   0        0        0     1098 2024-03-26 15:00:02.592466 torrent_tool-0.0.3.1/pyproject.toml
--rw-r--r--   0        0        0     1811 2024-03-26 14:59:41.100942 torrent_tool-0.0.3.1/readme.md
--rwxr-xr-x   0        0        0     6845 2024-03-26 14:59:53.797013 torrent_tool-0.0.3.1/torrent_tool.py
--rw-r--r--   0        0        0     3297 1970-01-01 00:00:00.000000 torrent_tool-0.0.3.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 torrent_tool-0.0.3.2/LICENSE
+-rw-r--r--   0        0        0     1093 2024-04-16 15:01:40.106595 torrent_tool-0.0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     1811 2024-03-26 14:59:41.100942 torrent_tool-0.0.3.2/readme.md
+-rwxr-xr-x   0        0        0     6845 2024-03-26 14:59:53.797013 torrent_tool-0.0.3.2/torrent_tool/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 torrent_tool-0.0.3.2/torrent_tool/py.typed
+-rw-r--r--   0        0        0     3295 1970-01-01 00:00:00.000000 torrent_tool-0.0.3.2/PKG-INFO
```

### Comparing `torrent_tool-0.0.3.1/LICENSE` & `torrent_tool-0.0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `torrent_tool-0.0.3.1/pyproject.toml` & `torrent_tool-0.0.3.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "torrent_tool"
-version = "0.0.3.1"
+version = "0.0.3.2"
 description = "torrent tool."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
-homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-cmdline/torrent_tool"
-repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-cmdline/torrent_tool"
+homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/torrent_tool"
+repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/torrent_tool"
 keywords = ["torrent", "magnet"]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Development Status :: 5 - Production/Stable",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.10",
@@ -26,8 +26,8 @@
 ]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [[tool.poetry.packages]]
-include = "torrent_tool.py"
+include = "torrent_tool"
```

### Comparing `torrent_tool-0.0.3.1/readme.md` & `torrent_tool-0.0.3.2/readme.md`

 * *Files identical despite different names*

### Comparing `torrent_tool-0.0.3.1/torrent_tool.py` & `torrent_tool-0.0.3.2/torrent_tool/__init__.py`

 * *Files identical despite different names*

### Comparing `torrent_tool-0.0.3.1/PKG-INFO` & `torrent_tool-0.0.3.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: torrent_tool
-Version: 0.0.3.1
+Version: 0.0.3.2
 Summary: torrent tool.
-Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-cmdline/torrent_tool
+Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/torrent_tool
 License: MIT
 Keywords: torrent,magnet
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -24,15 +24,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Project-URL: Repository, https://github.com/ChenyangGao/web-mount-packs/tree/main/python-cmdline/torrent_tool
+Project-URL: Repository, https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/torrent_tool
 Description-Content-Type: text/markdown
 
 # BitTorrent Tool Module
 
 - [The BitTorrent Protocol Specification](http://www.bittorrent.org/beps/bep_0003.html)
 - [Peer-to-Peer (P2P) Architecture](https://www.rfc-editor.org/rfc/rfc5694)
 - [Peer-to-Peer Streaming Peer Protocol (PPSPP)](https://www.rfc-editor.org/rfc/rfc7574.txt)
```

