# Comparing `tmp/zalando_cli_bundle-24.6.0.tar.gz` & `tmp/zalando_cli_bundle-24.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zalando_cli_bundle-24.6.0.tar", max compression
+gzip compressed data, was "zalando_cli_bundle-24.7.0.tar", max compression
```

## Comparing `zalando_cli_bundle-24.6.0.tar` & `zalando_cli_bundle-24.7.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     1251 2024-04-11 07:31:59.000000 zalando_cli_bundle-24.6.0/pyproject.toml
--rw-r--r--   0        0        0       30 2024-04-10 08:25:25.000000 zalando_cli_bundle-24.6.0/zalando_cli_bundle/__main__.py
--rw-r--r--   0        0        0      581 2024-04-10 08:25:25.000000 zalando_cli_bundle-24.6.0/zalando_cli_bundle/cli.py
--rw-r--r--   0        0        0     1343 1970-01-01 00:00:00.000000 zalando_cli_bundle-24.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1206 2024-04-16 11:51:11.000000 zalando_cli_bundle-24.7.0/pyproject.toml
+-rw-r--r--   0        0        0       30 2024-04-16 11:51:11.000000 zalando_cli_bundle-24.7.0/zalando_cli_bundle/__main__.py
+-rw-r--r--   0        0        0      581 2024-04-16 11:51:11.000000 zalando_cli_bundle-24.7.0/zalando_cli_bundle/cli.py
+-rw-r--r--   0        0        0     1293 1970-01-01 00:00:00.000000 zalando_cli_bundle-24.7.0/PKG-INFO
```

### Comparing `zalando_cli_bundle-24.6.0/pyproject.toml` & `zalando_cli_bundle-24.7.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 [tool.poetry]
 name = "zalando-cli-bundle"
-version = "24.6.0"
+version = "24.7.0"
 description = "CLI bundle for Zalando developers"
 authors = ["Henning Jacobs <henning@zalando.de>"]
 classifiers = [
     "Framework :: Pytest",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Intended Audience :: System Administrators",
     "Operating System :: POSIX :: Linux",
     "Programming Language :: Python",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: Implementation :: CPython",
 ]
```

### Comparing `zalando_cli_bundle-24.6.0/zalando_cli_bundle/cli.py` & `zalando_cli_bundle-24.7.0/zalando_cli_bundle/cli.py`

 * *Files identical despite different names*

### Comparing `zalando_cli_bundle-24.6.0/PKG-INFO` & `zalando_cli_bundle-24.7.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zalando-cli-bundle
-Version: 24.6.0
+Version: 24.7.0
 Summary: CLI bundle for Zalando developers
 Home-page: https://github.bus.zalan.do/developer-productivity/zalando-cli-bundle
 Author: Henning Jacobs
 Author-email: henning@zalando.de
 Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Console
 Classifier: Framework :: Pytest
@@ -14,15 +14,14 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Dist: click (>=8,<9)
 Requires-Dist: stups-cli-support (>=1.1.22,<2.0.0)
 Requires-Dist: stups-kio (>=0.1.25,<0.2.0)
 Requires-Dist: stups-pierone (>=1.1.53,<2.0.0)
 Requires-Dist: stups-zign (>=1.2,<2.0)
 Requires-Dist: zalando-aws-cli (>=1.2.7,<2.0.0)
```

