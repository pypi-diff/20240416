# Comparing `tmp/scratchattach-1.6.3.tar.gz` & `tmp/scratchattach-1.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scratchattach-1.6.3.tar", last modified: Tue Apr 16 18:52:02 2024, max compression
+gzip compressed data, was "scratchattach-1.6.4.tar", last modified: Tue Apr 16 19:12:40 2024, max compression
```

## Comparing `scratchattach-1.6.3.tar` & `scratchattach-1.6.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 18:52:02.650414 scratchattach-1.6.3/
--rw-rw-rw-   0        0        0     1101 2023-09-02 14:18:05.000000 scratchattach-1.6.3/LICENSE
--rw-rw-rw-   0        0        0     4042 2024-04-16 18:52:02.649406 scratchattach-1.6.3/PKG-INFO
--rw-rw-rw-   0        0        0     3309 2023-09-04 01:43:11.000000 scratchattach-1.6.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-16 18:52:02.633878 scratchattach-1.6.3/scratchattach/
--rw-rw-rw-   0        0        0     2719 2023-09-16 14:17:22.000000 scratchattach-1.6.3/scratchattach/__init__.py
--rw-rw-rw-   0        0        0    20823 2024-04-16 18:51:10.000000 scratchattach-1.6.3/scratchattach/cloud.py
--rw-rw-rw-   0        0        0    24874 2024-04-16 18:08:07.000000 scratchattach-1.6.3/scratchattach/cloud_requests.py
--rw-rw-rw-   0        0        0     2600 2024-04-16 18:08:07.000000 scratchattach-1.6.3/scratchattach/encoder.py
--rw-rw-rw-   0        0        0     4221 2023-10-25 12:34:35.000000 scratchattach-1.6.3/scratchattach/exceptions.py
--rw-rw-rw-   0        0        0    10508 2023-09-04 01:29:36.000000 scratchattach-1.6.3/scratchattach/forum.py
--rw-rw-rw-   0        0        0    31197 2024-04-16 18:33:18.000000 scratchattach-1.6.3/scratchattach/project.py
--rw-rw-rw-   0        0        0    22000 2023-09-30 18:44:30.000000 scratchattach-1.6.3/scratchattach/session.py
--rw-rw-rw-   0        0        0    20487 2024-04-16 18:08:07.000000 scratchattach-1.6.3/scratchattach/studio.py
--rw-rw-rw-   0        0        0    34892 2023-11-24 17:38:57.000000 scratchattach-1.6.3/scratchattach/user.py
-drwxrwxrwx   0        0        0        0 2024-04-16 18:52:02.649406 scratchattach-1.6.3/scratchattach.egg-info/
--rw-rw-rw-   0        0        0     4042 2024-04-16 18:52:02.000000 scratchattach-1.6.3/scratchattach.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      463 2024-04-16 18:52:02.000000 scratchattach-1.6.3/scratchattach.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 18:52:02.000000 scratchattach-1.6.3/scratchattach.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2024-04-16 18:52:02.000000 scratchattach-1.6.3/scratchattach.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-16 18:52:02.000000 scratchattach-1.6.3/scratchattach.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-16 18:52:02.650414 scratchattach-1.6.3/setup.cfg
--rw-rw-rw-   0        0        0     1108 2024-04-16 18:50:58.000000 scratchattach-1.6.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 19:12:40.170194 scratchattach-1.6.4/
+-rw-rw-rw-   0        0        0     1101 2023-09-02 14:18:05.000000 scratchattach-1.6.4/LICENSE
+-rw-rw-rw-   0        0        0     4042 2024-04-16 19:12:40.170194 scratchattach-1.6.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3309 2023-09-04 01:43:11.000000 scratchattach-1.6.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-16 19:12:40.157689 scratchattach-1.6.4/scratchattach/
+-rw-rw-rw-   0        0        0     2719 2023-09-16 14:17:22.000000 scratchattach-1.6.4/scratchattach/__init__.py
+-rw-rw-rw-   0        0        0    20822 2024-04-16 19:12:00.000000 scratchattach-1.6.4/scratchattach/cloud.py
+-rw-rw-rw-   0        0        0    24874 2024-04-16 18:08:07.000000 scratchattach-1.6.4/scratchattach/cloud_requests.py
+-rw-rw-rw-   0        0        0     2600 2024-04-16 18:08:07.000000 scratchattach-1.6.4/scratchattach/encoder.py
+-rw-rw-rw-   0        0        0     4221 2023-10-25 12:34:35.000000 scratchattach-1.6.4/scratchattach/exceptions.py
+-rw-rw-rw-   0        0        0    10508 2023-09-04 01:29:36.000000 scratchattach-1.6.4/scratchattach/forum.py
+-rw-rw-rw-   0        0        0    31197 2024-04-16 18:33:18.000000 scratchattach-1.6.4/scratchattach/project.py
+-rw-rw-rw-   0        0        0    22000 2023-09-30 18:44:30.000000 scratchattach-1.6.4/scratchattach/session.py
+-rw-rw-rw-   0        0        0    20487 2024-04-16 18:08:07.000000 scratchattach-1.6.4/scratchattach/studio.py
+-rw-rw-rw-   0        0        0    34892 2023-11-24 17:38:57.000000 scratchattach-1.6.4/scratchattach/user.py
+drwxrwxrwx   0        0        0        0 2024-04-16 19:12:40.169193 scratchattach-1.6.4/scratchattach.egg-info/
+-rw-rw-rw-   0        0        0     4042 2024-04-16 19:12:40.000000 scratchattach-1.6.4/scratchattach.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      463 2024-04-16 19:12:40.000000 scratchattach-1.6.4/scratchattach.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 19:12:40.000000 scratchattach-1.6.4/scratchattach.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2024-04-16 19:12:40.000000 scratchattach-1.6.4/scratchattach.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-16 19:12:40.000000 scratchattach-1.6.4/scratchattach.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-16 19:12:40.170194 scratchattach-1.6.4/setup.cfg
+-rw-rw-rw-   0        0        0     1108 2024-04-16 19:12:23.000000 scratchattach-1.6.4/setup.py
```

### Comparing `scratchattach-1.6.3/LICENSE` & `scratchattach-1.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `scratchattach-1.6.3/PKG-INFO` & `scratchattach-1.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratchattach
-Version: 1.6.3
+Version: 1.6.4
 Summary: An Scratch API Wrapper for scra tch.mit.edu
 Home-page: https://github.com/TimMcCool/scratchattach
 Author: TimMcCool
 Author-email: timkrome2006@gmail.com
 Keywords: scratch api,scratchattach,scratch api python,scratch python,scratch for python,scratch,scratch cloud,scratch cloud variables,scratch bot
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `scratchattach-1.6.3/README.md` & `scratchattach-1.6.4/README.md`

 * *Files identical despite different names*

### Comparing `scratchattach-1.6.3/scratchattach/__init__.py` & `scratchattach-1.6.4/scratchattach/__init__.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.6.3/scratchattach/cloud.py` & `scratchattach-1.6.4/scratchattach/cloud.py`

 * *Files 0% similar despite different names*

```diff
@@ -158,15 +158,15 @@
             if cloud_host is None:
                 cloud_host = "wss://clouddata.turbowarp.org/"
                 self.cloud_host = cloud_host
             self.websocket.connect(
                 cloud_host,
                 enable_multithread=True,
                 timeout = self._ws_timeout,
-                headers = {"User-Agent":"scratchattach/1.6.3"}
+                header = {"User-Agent":"scratchattach/1.6.4"}
             )
         except Exception:
             raise(exceptions.ConnectionError)
         self._connect_timestamp = time.time()
 
 
     def set_var(self, variable, value):
```

### Comparing `scratchattach-1.6.3/scratchattach/cloud_requests.py` & `scratchattach-1.6.4/scratchattach/cloud_requests.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.6.3/scratchattach/encoder.py` & `scratchattach-1.6.4/scratchattach/encoder.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.6.3/scratchattach/exceptions.py` & `scratchattach-1.6.4/scratchattach/exceptions.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.6.3/scratchattach/forum.py` & `scratchattach-1.6.4/scratchattach/forum.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.6.3/scratchattach/project.py` & `scratchattach-1.6.4/scratchattach/project.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.6.3/scratchattach/session.py` & `scratchattach-1.6.4/scratchattach/session.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.6.3/scratchattach/studio.py` & `scratchattach-1.6.4/scratchattach/studio.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.6.3/scratchattach/user.py` & `scratchattach-1.6.4/scratchattach/user.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.6.3/scratchattach.egg-info/PKG-INFO` & `scratchattach-1.6.4/scratchattach.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratchattach
-Version: 1.6.3
+Version: 1.6.4
 Summary: An Scratch API Wrapper for scra tch.mit.edu
 Home-page: https://github.com/TimMcCool/scratchattach
 Author: TimMcCool
 Author-email: timkrome2006@gmail.com
 Keywords: scratch api,scratchattach,scratch api python,scratch python,scratch for python,scratch,scratch cloud,scratch cloud variables,scratch bot
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `scratchattach-1.6.3/setup.py` & `scratchattach-1.6.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '1.6.3'
+VERSION = '1.6.4'
 DESCRIPTION = 'An Scratch API Wrapper for scra tch.mit.edu'
 LONG_DESCRIPTION = DESCRIPTION
 
 # Setting up
 setup(
     name="scratchattach",
     version=VERSION,
```

