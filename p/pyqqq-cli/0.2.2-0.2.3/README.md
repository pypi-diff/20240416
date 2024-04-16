# Comparing `tmp/pyqqq_cli-0.2.2.tar.gz` & `tmp/pyqqq_cli-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqqq_cli-0.2.2.tar", max compression
+gzip compressed data, was "pyqqq_cli-0.2.3.tar", max compression
```

## Comparing `pyqqq_cli-0.2.2.tar` & `pyqqq_cli-0.2.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1063 2024-03-22 07:02:26.408726 pyqqq_cli-0.2.2/LICENSE
--rw-r--r--   0        0        0      937 2024-03-22 07:01:48.074678 pyqqq_cli-0.2.2/README.md
--rw-r--r--   0        0        0      655 2024-04-15 02:24:05.912336 pyqqq_cli-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      358 2024-04-01 04:44:33.805339 pyqqq_cli-0.2.2/qupiato/cli/config.py
--rw-r--r--   0        0        0     6509 2024-04-15 01:50:45.209668 pyqqq_cli-0.2.2/qupiato/cli/main.py
--rw-r--r--   0        0        0     4459 2024-04-12 07:48:42.606234 pyqqq_cli-0.2.2/qupiato/cli/utils.py
--rw-r--r--   0        0        0     1809 1970-01-01 00:00:00.000000 pyqqq_cli-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-03-22 07:02:26.408726 pyqqq_cli-0.2.3/LICENSE
+-rw-r--r--   0        0        0      937 2024-03-22 07:01:48.074678 pyqqq_cli-0.2.3/README.md
+-rw-r--r--   0        0        0      655 2024-04-16 01:40:36.280640 pyqqq_cli-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      358 2024-04-01 04:44:33.805339 pyqqq_cli-0.2.3/qupiato/cli/config.py
+-rw-r--r--   0        0        0     6509 2024-04-15 01:50:45.209668 pyqqq_cli-0.2.3/qupiato/cli/main.py
+-rw-r--r--   0        0        0     4459 2024-04-12 07:48:42.606234 pyqqq_cli-0.2.3/qupiato/cli/utils.py
+-rw-r--r--   0        0        0     1809 1970-01-01 00:00:00.000000 pyqqq_cli-0.2.3/PKG-INFO
```

### Comparing `pyqqq_cli-0.2.2/LICENSE` & `pyqqq_cli-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyqqq_cli-0.2.2/README.md` & `pyqqq_cli-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `pyqqq_cli-0.2.2/pyproject.toml` & `pyqqq_cli-0.2.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "pyqqq-cli"
-version = "0.2.2"
+version = "0.2.3"
 description = "CLI tool for controlling strategies deployed on the PyQQQ platform."
 authors = ["PyQQQ team <pyqqq.cs@gmail.com>"]
 readme = "README.md"
 packages = [{include = "qupiato"}]
 license = "MIT"
 documentation = "https://qupiato-sdk-18secs-cf54ebea1b14b422537daf0462fb86d68f4582d064a4.gitlab.io"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 click = "^8.1.7"
 websockets = "^12.0"
 python-dotenv = "^1.0.1"
 requests = "^2.31.0"
-pyqqq = "^0.7.5"
+pyqqq = "^0.7.7"
 pyyaml = "^6.0.1"
 
 [tool.poetry.scripts]
 qqq = 'qupiato.cli.main:main'
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `pyqqq_cli-0.2.2/qupiato/cli/main.py` & `pyqqq_cli-0.2.3/qupiato/cli/main.py`

 * *Files identical despite different names*

### Comparing `pyqqq_cli-0.2.2/qupiato/cli/utils.py` & `pyqqq_cli-0.2.3/qupiato/cli/utils.py`

 * *Files identical despite different names*

### Comparing `pyqqq_cli-0.2.2/PKG-INFO` & `pyqqq_cli-0.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: pyqqq-cli
-Version: 0.2.2
+Version: 0.2.3
 Summary: CLI tool for controlling strategies deployed on the PyQQQ platform.
 License: MIT
 Author: PyQQQ team
 Author-email: pyqqq.cs@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=8.1.7,<9.0.0)
-Requires-Dist: pyqqq (>=0.7.5,<0.8.0)
+Requires-Dist: pyqqq (>=0.7.7,<0.8.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: websockets (>=12.0,<13.0)
 Project-URL: Documentation, https://qupiato-sdk-18secs-cf54ebea1b14b422537daf0462fb86d68f4582d064a4.gitlab.io
 Description-Content-Type: text/markdown
```

