# Comparing `tmp/lookout_cli-1.2.0.tar.gz` & `tmp/lookout_cli-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lookout_cli-1.2.0.tar", last modified: Mon Apr 15 07:15:02 2024, max compression
+gzip compressed data, was "lookout_cli-1.2.1.tar", last modified: Mon Apr 15 09:21:28 2024, max compression
```

## Comparing `lookout_cli-1.2.0.tar` & `lookout_cli-1.2.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-15 07:15:02.985630 lookout_cli-1.2.0/
--rw-r--r--   0 runner    (1000) runner    (1001)     1511 2024-04-15 07:15:02.985630 lookout_cli-1.2.0/PKG-INFO
--rw-rw-r--   0 runner    (1000) runner    (1001)      700 2024-04-15 07:13:44.000000 lookout_cli-1.2.0/README.md
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-15 07:15:02.985630 lookout_cli-1.2.0/lookout_cli/
--rw-rw-r--   0 runner    (1000) runner    (1001)        0 2024-04-15 07:13:44.000000 lookout_cli-1.2.0/lookout_cli/__init__.py
--rw-rw-r--   0 runner    (1000) runner    (1001)      424 2024-04-15 07:13:44.000000 lookout_cli-1.2.0/lookout_cli/banner.py
--rw-rw-r--   0 runner    (1000) runner    (1001)     1102 2024-04-15 07:13:44.000000 lookout_cli-1.2.0/lookout_cli/cli.py
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-15 07:15:02.985630 lookout_cli-1.2.0/lookout_cli/docker/
--rw-rw-r--   0 runner    (1000) runner    (1001)     2649 2024-04-15 07:13:44.000000 lookout_cli-1.2.0/lookout_cli/docker/docker-compose.dev.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      212 2024-04-15 07:13:44.000000 lookout_cli-1.2.0/lookout_cli/docker/docker-compose.gpu.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      221 2024-04-15 07:13:44.000000 lookout_cli-1.2.0/lookout_cli/docker/docker-compose.network-host.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      428 2024-04-15 07:13:44.000000 lookout_cli-1.2.0/lookout_cli/docker/docker-compose.network-shared.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      990 2024-04-15 07:13:44.000000 lookout_cli-1.2.0/lookout_cli/docker/docker-compose.yaml
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-15 07:15:02.985630 lookout_cli-1.2.0/lookout_cli/groups/
--rw-rw-r--   0 runner    (1000) runner    (1001)        0 2024-04-15 07:13:44.000000 lookout_cli-1.2.0/lookout_cli/groups/__init__.py
--rw-rw-r--   0 runner    (1000) runner    (1001)     8509 2024-04-15 07:13:44.000000 lookout_cli-1.2.0/lookout_cli/groups/base.py
--rw-rw-r--   0 runner    (1000) runner    (1001)      832 2024-04-15 07:13:44.000000 lookout_cli-1.2.0/lookout_cli/groups/setup.py
--rw-rw-r--   0 runner    (1000) runner    (1001)     3600 2024-04-15 07:13:44.000000 lookout_cli-1.2.0/lookout_cli/helpers.py
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-15 07:15:02.985630 lookout_cli-1.2.0/lookout_cli/test/
--rw-rw-r--   0 runner    (1000) runner    (1001)       70 2024-04-15 07:13:44.000000 lookout_cli-1.2.0/lookout_cli/test/lookout_cli_test.py
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-15 07:15:02.985630 lookout_cli-1.2.0/lookout_cli.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1001)     1511 2024-04-15 07:15:02.000000 lookout_cli-1.2.0/lookout_cli.egg-info/PKG-INFO
--rw-rw-r--   0 runner    (1000) runner    (1001)      712 2024-04-15 07:15:02.000000 lookout_cli-1.2.0/lookout_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)        1 2024-04-15 07:15:02.000000 lookout_cli-1.2.0/lookout_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)       48 2024-04-15 07:15:02.000000 lookout_cli-1.2.0/lookout_cli.egg-info/entry_points.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)       76 2024-04-15 07:15:02.000000 lookout_cli-1.2.0/lookout_cli.egg-info/requires.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)       12 2024-04-15 07:15:02.000000 lookout_cli-1.2.0/lookout_cli.egg-info/top_level.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)        1 2024-04-15 07:14:50.000000 lookout_cli-1.2.0/lookout_cli.egg-info/zip-safe
--rw-rw-r--   0 runner    (1000) runner    (1001)      997 2024-04-15 07:15:02.985630 lookout_cli-1.2.0/setup.cfg
--rw-rw-r--   0 runner    (1000) runner    (1001)       38 2024-04-15 07:13:44.000000 lookout_cli-1.2.0/setup.py
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-15 09:21:28.906791 lookout_cli-1.2.1/
+-rw-r--r--   0 runner    (1000) runner    (1001)     1511 2024-04-15 09:21:28.906791 lookout_cli-1.2.1/PKG-INFO
+-rw-rw-r--   0 runner    (1000) runner    (1001)      700 2024-04-15 09:20:10.000000 lookout_cli-1.2.1/README.md
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-15 09:21:28.906791 lookout_cli-1.2.1/lookout_cli/
+-rw-rw-r--   0 runner    (1000) runner    (1001)        0 2024-04-15 09:20:10.000000 lookout_cli-1.2.1/lookout_cli/__init__.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)      424 2024-04-15 09:20:10.000000 lookout_cli-1.2.1/lookout_cli/banner.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)     1102 2024-04-15 09:20:10.000000 lookout_cli-1.2.1/lookout_cli/cli.py
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-15 09:21:28.906791 lookout_cli-1.2.1/lookout_cli/docker/
+-rw-rw-r--   0 runner    (1000) runner    (1001)     2649 2024-04-15 09:20:10.000000 lookout_cli-1.2.1/lookout_cli/docker/docker-compose.dev.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      212 2024-04-15 09:20:10.000000 lookout_cli-1.2.1/lookout_cli/docker/docker-compose.gpu.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      221 2024-04-15 09:20:10.000000 lookout_cli-1.2.1/lookout_cli/docker/docker-compose.network-host.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      428 2024-04-15 09:20:10.000000 lookout_cli-1.2.1/lookout_cli/docker/docker-compose.network-shared.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      990 2024-04-15 09:20:10.000000 lookout_cli-1.2.1/lookout_cli/docker/docker-compose.yaml
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-15 09:21:28.906791 lookout_cli-1.2.1/lookout_cli/groups/
+-rw-rw-r--   0 runner    (1000) runner    (1001)        0 2024-04-15 09:20:10.000000 lookout_cli-1.2.1/lookout_cli/groups/__init__.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)     8509 2024-04-15 09:20:10.000000 lookout_cli-1.2.1/lookout_cli/groups/base.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)      832 2024-04-15 09:20:10.000000 lookout_cli-1.2.1/lookout_cli/groups/setup.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)     3600 2024-04-15 09:20:10.000000 lookout_cli-1.2.1/lookout_cli/helpers.py
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-15 09:21:28.906791 lookout_cli-1.2.1/lookout_cli/test/
+-rw-rw-r--   0 runner    (1000) runner    (1001)       70 2024-04-15 09:20:10.000000 lookout_cli-1.2.1/lookout_cli/test/lookout_cli_test.py
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-15 09:21:28.906791 lookout_cli-1.2.1/lookout_cli.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1001)     1511 2024-04-15 09:21:28.000000 lookout_cli-1.2.1/lookout_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 runner    (1000) runner    (1001)      712 2024-04-15 09:21:28.000000 lookout_cli-1.2.1/lookout_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)        1 2024-04-15 09:21:28.000000 lookout_cli-1.2.1/lookout_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)       48 2024-04-15 09:21:28.000000 lookout_cli-1.2.1/lookout_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)       76 2024-04-15 09:21:28.000000 lookout_cli-1.2.1/lookout_cli.egg-info/requires.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)       12 2024-04-15 09:21:28.000000 lookout_cli-1.2.1/lookout_cli.egg-info/top_level.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)        1 2024-04-15 09:21:16.000000 lookout_cli-1.2.1/lookout_cli.egg-info/zip-safe
+-rw-rw-r--   0 runner    (1000) runner    (1001)      997 2024-04-15 09:21:28.910791 lookout_cli-1.2.1/setup.cfg
+-rw-rw-r--   0 runner    (1000) runner    (1001)       38 2024-04-15 09:20:10.000000 lookout_cli-1.2.1/setup.py
```

### Comparing `lookout_cli-1.2.0/PKG-INFO` & `lookout_cli-1.2.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lookout_cli
-Version: 1.2.0
+Version: 1.2.1
 Summary: A CLI for interacting with Lookout+
 Home-page: https://github.com/Greenroom-Robotics/lookout
 Author: Greenroom Robotics
 Author-email: team@greenroomrobotics.com
 Maintainer: David Revay
 Maintainer-email: david.revay@greenroomrobotics.com
 License: Copyright (C) 2023, Greenroom Robotics
```

### Comparing `lookout_cli-1.2.0/README.md` & `lookout_cli-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `lookout_cli-1.2.0/lookout_cli/cli.py` & `lookout_cli-1.2.1/lookout_cli/cli.py`

 * *Files identical despite different names*

### Comparing `lookout_cli-1.2.0/lookout_cli/docker/docker-compose.dev.yaml` & `lookout_cli-1.2.1/lookout_cli/docker/docker-compose.dev.yaml`

 * *Files identical despite different names*

### Comparing `lookout_cli-1.2.0/lookout_cli/docker/docker-compose.yaml` & `lookout_cli-1.2.1/lookout_cli/docker/docker-compose.yaml`

 * *Files identical despite different names*

### Comparing `lookout_cli-1.2.0/lookout_cli/groups/base.py` & `lookout_cli-1.2.1/lookout_cli/groups/base.py`

 * *Files identical despite different names*

### Comparing `lookout_cli-1.2.0/lookout_cli/groups/setup.py` & `lookout_cli-1.2.1/lookout_cli/groups/setup.py`

 * *Files identical despite different names*

### Comparing `lookout_cli-1.2.0/lookout_cli/helpers.py` & `lookout_cli-1.2.1/lookout_cli/helpers.py`

 * *Files identical despite different names*

### Comparing `lookout_cli-1.2.0/lookout_cli.egg-info/PKG-INFO` & `lookout_cli-1.2.1/lookout_cli.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lookout_cli
-Version: 1.2.0
+Version: 1.2.1
 Summary: A CLI for interacting with Lookout+
 Home-page: https://github.com/Greenroom-Robotics/lookout
 Author: Greenroom Robotics
 Author-email: team@greenroomrobotics.com
 Maintainer: David Revay
 Maintainer-email: david.revay@greenroomrobotics.com
 License: Copyright (C) 2023, Greenroom Robotics
```

### Comparing `lookout_cli-1.2.0/lookout_cli.egg-info/SOURCES.txt` & `lookout_cli-1.2.1/lookout_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lookout_cli-1.2.0/setup.cfg` & `lookout_cli-1.2.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = lookout_cli
-version = 1.2.0
+version = 1.2.1
 url = https://github.com/Greenroom-Robotics/lookout
 author = Greenroom Robotics
 author_email = team@greenroomrobotics.com
 maintainer = David Revay
 maintainer_email = david.revay@greenroomrobotics.com
 classifiers = 
 	Development Status :: 3 - Alpha
```

