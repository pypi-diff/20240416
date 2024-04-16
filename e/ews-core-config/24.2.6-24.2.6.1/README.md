# Comparing `tmp/ews-core-config-24.2.6.tar.gz` & `tmp/ews-core-config-24.2.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ews-core-config-24.2.6.tar", last modified: Mon Feb 26 06:38:33 2024, max compression
+gzip compressed data, was "ews-core-config-24.2.6.1.tar", last modified: Mon Feb 26 12:50:59 2024, max compression
```

## Comparing `ews-core-config-24.2.6.tar` & `ews-core-config-24.2.6.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 06:38:33.300358 ews-core-config-24.2.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-02-26 06:38:04.000000 ews-core-config-24.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-02-26 06:38:33.300358 ews-core-config-24.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-26 06:38:04.000000 ews-core-config-24.2.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-02-26 06:38:04.000000 ews-core-config-24.2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-26 06:38:33.300358 ews-core-config-24.2.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 06:38:33.296358 ews-core-config-24.2.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 06:38:33.296358 ews-core-config-24.2.6/src/ews_core_config/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-02-26 06:38:04.000000 ews-core-config-24.2.6/src/ews_core_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-02-26 06:38:04.000000 ews-core-config-24.2.6/src/ews_core_config/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-02-26 06:38:04.000000 ews-core-config-24.2.6/src/ews_core_config/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 06:38:33.300358 ews-core-config-24.2.6/src/ews_core_config.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-02-26 06:38:33.000000 ews-core-config-24.2.6/src/ews_core_config.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-02-26 06:38:33.000000 ews-core-config-24.2.6/src/ews_core_config.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-26 06:38:33.000000 ews-core-config-24.2.6/src/ews_core_config.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-26 06:38:33.000000 ews-core-config-24.2.6/src/ews_core_config.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-26 06:38:33.000000 ews-core-config-24.2.6/src/ews_core_config.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 06:38:33.300358 ews-core-config-24.2.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-02-26 06:38:04.000000 ews-core-config-24.2.6/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-02-26 06:38:04.000000 ews-core-config-24.2.6/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 12:50:59.645762 ews-core-config-24.2.6.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-02-26 12:50:39.000000 ews-core-config-24.2.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-02-26 12:50:59.645762 ews-core-config-24.2.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-26 12:50:39.000000 ews-core-config-24.2.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-02-26 12:50:39.000000 ews-core-config-24.2.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-26 12:50:59.645762 ews-core-config-24.2.6.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 12:50:59.641762 ews-core-config-24.2.6.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 12:50:59.641762 ews-core-config-24.2.6.1/src/ews_core_config/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-02-26 12:50:39.000000 ews-core-config-24.2.6.1/src/ews_core_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-02-26 12:50:39.000000 ews-core-config-24.2.6.1/src/ews_core_config/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-02-26 12:50:39.000000 ews-core-config-24.2.6.1/src/ews_core_config/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 12:50:59.645762 ews-core-config-24.2.6.1/src/ews_core_config.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-02-26 12:50:59.000000 ews-core-config-24.2.6.1/src/ews_core_config.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-02-26 12:50:59.000000 ews-core-config-24.2.6.1/src/ews_core_config.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-26 12:50:59.000000 ews-core-config-24.2.6.1/src/ews_core_config.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-26 12:50:59.000000 ews-core-config-24.2.6.1/src/ews_core_config.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-26 12:50:59.000000 ews-core-config-24.2.6.1/src/ews_core_config.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 12:50:59.645762 ews-core-config-24.2.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-02-26 12:50:39.000000 ews-core-config-24.2.6.1/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-02-26 12:50:39.000000 ews-core-config-24.2.6.1/tests/test_version.py
```

### Comparing `ews-core-config-24.2.6/LICENSE` & `ews-core-config-24.2.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ews-core-config-24.2.6/PKG-INFO` & `ews-core-config-24.2.6.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ews-core-config
-Version: 24.2.6
+Version: 24.2.6.1
 Summary: A simple TOML configuration for EWS settings
 Author-email: EWS Consulting <github@ews-consulting.com>
 License: MIT License
         
         Copyright (c) 2024 EWS Consulting
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `ews-core-config-24.2.6/pyproject.toml` & `ews-core-config-24.2.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ews-core-config-24.2.6/src/ews_core_config/config.py` & `ews-core-config-24.2.6.1/src/ews_core_config/config.py`

 * *Files identical despite different names*

### Comparing `ews-core-config-24.2.6/src/ews_core_config/version.py` & `ews-core-config-24.2.6.1/src/ews_core_config/version.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 __all__ = ("VERSION", "version_info")
 
-VERSION = "24.2.6"
+VERSION = "24.2.6.1"
 
 
 def version_info() -> str:
     """
     Show the version info
 
     Example:
```

### Comparing `ews-core-config-24.2.6/src/ews_core_config.egg-info/PKG-INFO` & `ews-core-config-24.2.6.1/src/ews_core_config.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ews-core-config
-Version: 24.2.6
+Version: 24.2.6.1
 Summary: A simple TOML configuration for EWS settings
 Author-email: EWS Consulting <github@ews-consulting.com>
 License: MIT License
         
         Copyright (c) 2024 EWS Consulting
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `ews-core-config-24.2.6/tests/test_version.py` & `ews-core-config-24.2.6.1/tests/test_version.py`

 * *Files identical despite different names*

