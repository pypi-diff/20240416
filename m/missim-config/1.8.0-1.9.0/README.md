# Comparing `tmp/missim_config-1.8.0.tar.gz` & `tmp/missim_config-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "missim_config-1.8.0.tar", last modified: Mon Apr  8 01:46:59 2024, max compression
+gzip compressed data, was "missim_config-1.9.0.tar", last modified: Wed Apr 10 08:34:15 2024, max compression
```

## Comparing `missim_config-1.8.0.tar` & `missim_config-1.9.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-08 01:46:59.275406 missim_config-1.8.0/
--rw-r--r--   0 runner    (1000) runner    (1001)     1263 2024-04-08 01:46:59.275406 missim_config-1.8.0/PKG-INFO
--rw-rw-r--   0 runner    (1000) runner    (1001)      521 2024-04-08 01:46:35.000000 missim_config-1.8.0/README.md
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-08 01:46:59.275406 missim_config-1.8.0/missim_config/
--rw-rw-r--   0 runner    (1000) runner    (1001)     2701 2024-04-08 01:46:35.000000 missim_config-1.8.0/missim_config/__init__.py
--rw-rw-r--   0 runner    (1000) runner    (1001)      432 2024-04-08 01:46:35.000000 missim_config-1.8.0/missim_config/generate_schemas.py
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-08 01:46:59.275406 missim_config-1.8.0/missim_config/schemas/
--rw-rw-r--   0 runner    (1000) runner    (1001)      970 2024-04-08 01:46:35.000000 missim_config-1.8.0/missim_config/schemas/missim.schema.json
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-08 01:46:59.275406 missim_config-1.8.0/missim_config/test/
--rw-rw-r--   0 runner    (1000) runner    (1001)       72 2024-04-08 01:46:35.000000 missim_config-1.8.0/missim_config/test/missim_config_test.py
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-08 01:46:59.275406 missim_config-1.8.0/missim_config.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1001)     1263 2024-04-08 01:46:59.000000 missim_config-1.8.0/missim_config.egg-info/PKG-INFO
--rw-rw-r--   0 runner    (1000) runner    (1001)      386 2024-04-08 01:46:59.000000 missim_config-1.8.0/missim_config.egg-info/SOURCES.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)        1 2024-04-08 01:46:59.000000 missim_config-1.8.0/missim_config.egg-info/dependency_links.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)       35 2024-04-08 01:46:59.000000 missim_config-1.8.0/missim_config.egg-info/requires.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)       14 2024-04-08 01:46:59.000000 missim_config-1.8.0/missim_config.egg-info/top_level.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)        1 2024-04-08 01:46:48.000000 missim_config-1.8.0/missim_config.egg-info/zip-safe
--rw-rw-r--   0 runner    (1000) runner    (1001)      871 2024-04-08 01:46:59.275406 missim_config-1.8.0/setup.cfg
--rw-rw-r--   0 runner    (1000) runner    (1001)       38 2024-04-08 01:46:35.000000 missim_config-1.8.0/setup.py
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-10 08:34:15.062174 missim_config-1.9.0/
+-rw-r--r--   0 runner    (1000) runner    (1001)     1263 2024-04-10 08:34:15.062174 missim_config-1.9.0/PKG-INFO
+-rw-rw-r--   0 runner    (1000) runner    (1001)      521 2024-04-10 08:33:52.000000 missim_config-1.9.0/README.md
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-10 08:34:15.062174 missim_config-1.9.0/missim_config/
+-rw-rw-r--   0 runner    (1000) runner    (1001)     2729 2024-04-10 08:33:52.000000 missim_config-1.9.0/missim_config/__init__.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)      432 2024-04-10 08:33:52.000000 missim_config-1.9.0/missim_config/generate_schemas.py
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-10 08:34:15.062174 missim_config-1.9.0/missim_config/schemas/
+-rw-rw-r--   0 runner    (1000) runner    (1001)     1041 2024-04-10 08:33:52.000000 missim_config-1.9.0/missim_config/schemas/missim.schema.json
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-10 08:34:15.062174 missim_config-1.9.0/missim_config/test/
+-rw-rw-r--   0 runner    (1000) runner    (1001)       72 2024-04-10 08:33:52.000000 missim_config-1.9.0/missim_config/test/missim_config_test.py
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-10 08:34:15.062174 missim_config-1.9.0/missim_config.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1001)     1263 2024-04-10 08:34:15.000000 missim_config-1.9.0/missim_config.egg-info/PKG-INFO
+-rw-rw-r--   0 runner    (1000) runner    (1001)      386 2024-04-10 08:34:15.000000 missim_config-1.9.0/missim_config.egg-info/SOURCES.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)        1 2024-04-10 08:34:15.000000 missim_config-1.9.0/missim_config.egg-info/dependency_links.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)       35 2024-04-10 08:34:15.000000 missim_config-1.9.0/missim_config.egg-info/requires.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)       14 2024-04-10 08:34:15.000000 missim_config-1.9.0/missim_config.egg-info/top_level.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)        1 2024-04-10 08:34:04.000000 missim_config-1.9.0/missim_config.egg-info/zip-safe
+-rw-rw-r--   0 runner    (1000) runner    (1001)      871 2024-04-10 08:34:15.062174 missim_config-1.9.0/setup.cfg
+-rw-rw-r--   0 runner    (1000) runner    (1001)       38 2024-04-10 08:33:52.000000 missim_config-1.9.0/setup.py
```

### Comparing `missim_config-1.8.0/PKG-INFO` & `missim_config-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: missim_config
-Version: 1.8.0
+Version: 1.9.0
 Summary: A library for reading / writing Missim config files
 Home-page: https://github.com/Greenroom-Robotics/missim
 Author: Greenroom Robotics
 Author-email: team@greenroomrobotics.com
 Maintainer: David Revay
 Maintainer-email: david.revay@greenroomrobotics.com
 License: Copyright (C) 2023, Greenroom Robotics
```

### Comparing `missim_config-1.8.0/README.md` & `missim_config-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `missim_config-1.8.0/missim_config/__init__.py` & `missim_config-1.9.0/missim_config/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     SHARED = "shared"
     HOST = "host"
 
 
 @dataclass
 class MissimConfig:
     ros_domain_id: int = 0
+    static_peers: str = ";"
     log_level: LogLevel = LogLevel.INFO
     mode: Mode = Mode.LOW_FIDELITY
     network: Network = Network.HOST
     sim_speed: float = 1.0
     use_https: bool = False
```

### Comparing `missim_config-1.8.0/missim_config/schemas/missim.schema.json` & `missim_config-1.9.0/missim_config/schemas/missim.schema.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9800000000000001%*

 * *Differences: {"'properties'": "{'static_peers': OrderedDict([('type', 'str'), ('default', ';')])}"}*

```diff
@@ -48,12 +48,16 @@
                 }
             ],
             "default": "host"
         },
         "ros_domain_id": {
             "default": 0,
             "type": "integer"
+        },
+        "static_peers": {
+            "default": ";",
+            "type": "str"
         }
     },
     "title": "MissimConfig",
     "type": "object"
 }
```

### Comparing `missim_config-1.8.0/missim_config.egg-info/PKG-INFO` & `missim_config-1.9.0/missim_config.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: missim_config
-Version: 1.8.0
+Version: 1.9.0
 Summary: A library for reading / writing Missim config files
 Home-page: https://github.com/Greenroom-Robotics/missim
 Author: Greenroom Robotics
 Author-email: team@greenroomrobotics.com
 Maintainer: David Revay
 Maintainer-email: david.revay@greenroomrobotics.com
 License: Copyright (C) 2023, Greenroom Robotics
```

### Comparing `missim_config-1.8.0/setup.cfg` & `missim_config-1.9.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = missim_config
-version = 1.8.0
+version = 1.9.0
 url = https://github.com/Greenroom-Robotics/missim
 author = Greenroom Robotics
 author_email = team@greenroomrobotics.com
 maintainer = David Revay
 maintainer_email = david.revay@greenroomrobotics.com
 classifiers = 
 	Development Status :: 3 - Alpha
```

