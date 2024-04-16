# Comparing `tmp/Velkoz-0.0.52.tar.gz` & `tmp/Velkoz-0.0.55.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Velkoz-0.0.52.tar", last modified: Tue Apr 16 15:12:36 2024, max compression
+gzip compressed data, was "Velkoz-0.0.55.tar", last modified: Tue Apr 16 15:58:07 2024, max compression
```

## Comparing `Velkoz-0.0.52.tar` & `Velkoz-0.0.55.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 15:12:36.162689 Velkoz-0.0.52/
--rw-rw-rw-   0        0        0      563 2024-04-16 15:12:36.161402 Velkoz-0.0.52/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-16 15:12:35.846274 Velkoz-0.0.52/Velkoz/
--rw-rw-rw-   0        0        0      785 2024-04-16 11:13:15.000000 Velkoz-0.0.52/Velkoz/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 15:12:35.901290 Velkoz-0.0.52/Velkoz/data/
--rw-rw-rw-   0        0        0       48 2024-04-13 20:58:45.000000 Velkoz-0.0.52/Velkoz/data/__init__.py
--rw-rw-rw-   0        0        0     2638 2024-04-16 15:11:09.000000 Velkoz-0.0.52/Velkoz/data/champion.py
--rw-rw-rw-   0        0        0     1738 2024-04-16 00:04:58.000000 Velkoz-0.0.52/Velkoz/data/common.py
-drwxrwxrwx   0        0        0        0 2024-04-16 15:12:35.976179 Velkoz-0.0.52/Velkoz/eye/
--rw-rw-rw-   0        0        0      150 2024-03-23 23:06:35.000000 Velkoz-0.0.52/Velkoz/eye/__init__.py
--rw-rw-rw-   0        0        0      523 2024-04-10 19:31:41.000000 Velkoz-0.0.52/Velkoz/eye/account.py
--rw-rw-rw-   0        0        0      591 2024-04-09 19:37:05.000000 Velkoz-0.0.52/Velkoz/eye/champion_mastery.py
--rw-rw-rw-   0        0        0        8 2024-03-22 13:50:02.000000 Velkoz-0.0.52/Velkoz/eye/common.py
--rw-rw-rw-   0        0        0     7581 2024-04-12 12:51:42.000000 Velkoz-0.0.52/Velkoz/eye/match.py
--rw-rw-rw-   0        0        0     1976 2024-04-10 19:31:40.000000 Velkoz-0.0.52/Velkoz/eye/summoner.py
--rw-rw-rw-   0        0        0     3276 2024-04-16 15:09:23.000000 Velkoz-0.0.52/Velkoz/settings.py
--rw-rw-rw-   0        0        0     1032 2024-04-16 15:12:10.000000 Velkoz-0.0.52/Velkoz/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-16 15:12:36.067685 Velkoz-0.0.52/Velkoz/supp/
--rw-rw-rw-   0        0        0      154 2024-04-16 10:08:55.000000 Velkoz-0.0.52/Velkoz/supp/__init__.py
--rw-rw-rw-   0        0        0      601 2024-04-10 19:50:35.000000 Velkoz-0.0.52/Velkoz/supp/account.py
--rw-rw-rw-   0        0        0      280 2024-04-16 11:05:52.000000 Velkoz-0.0.52/Velkoz/supp/champion.py
--rw-rw-rw-   0        0        0     1165 2024-04-11 21:19:17.000000 Velkoz-0.0.52/Velkoz/supp/champion_mastery.py
--rw-rw-rw-   0        0        0      270 2024-04-11 21:19:18.000000 Velkoz-0.0.52/Velkoz/supp/match.py
--rw-rw-rw-   0        0        0     1681 2024-04-10 19:50:14.000000 Velkoz-0.0.52/Velkoz/supp/summoner.py
-drwxrwxrwx   0        0        0        0 2024-04-16 15:12:36.159220 Velkoz-0.0.52/Velkoz/tentacles/
--rw-rw-rw-   0        0        0      213 2024-04-11 21:19:17.000000 Velkoz-0.0.52/Velkoz/tentacles/__init__.py
--rw-rw-rw-   0        0        0     1224 2024-03-22 11:07:43.000000 Velkoz-0.0.52/Velkoz/tentacles/account.py
--rw-rw-rw-   0        0        0     3340 2024-04-11 21:19:18.000000 Velkoz-0.0.52/Velkoz/tentacles/champion_mastery.py
--rw-rw-rw-   0        0        0     4543 2024-04-12 22:57:44.000000 Velkoz-0.0.52/Velkoz/tentacles/common.py
--rw-rw-rw-   0        0        0       60 2024-04-05 19:09:48.000000 Velkoz-0.0.52/Velkoz/tentacles/config.py
--rw-rw-rw-   0        0        0     1650 2024-03-22 13:51:43.000000 Velkoz-0.0.52/Velkoz/tentacles/match.py
--rw-rw-rw-   0        0        0     1416 2024-03-22 11:06:12.000000 Velkoz-0.0.52/Velkoz/tentacles/summoner.py
--rw-rw-rw-   0        0        0     6575 2024-04-16 15:11:30.000000 Velkoz-0.0.52/Velkoz/velkoz.py
-drwxrwxrwx   0        0        0        0 2024-04-16 15:12:36.160752 Velkoz-0.0.52/Velkoz.egg-info/
--rw-rw-rw-   0        0        0      563 2024-04-16 15:12:35.000000 Velkoz-0.0.52/Velkoz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      780 2024-04-16 15:12:35.000000 Velkoz-0.0.52/Velkoz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 15:12:35.000000 Velkoz-0.0.52/Velkoz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-16 15:12:35.000000 Velkoz-0.0.52/Velkoz.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-16 15:12:35.000000 Velkoz-0.0.52/Velkoz.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-16 15:12:36.162689 Velkoz-0.0.52/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-16 15:58:07.669357 Velkoz-0.0.55/
+-rw-rw-rw-   0        0        0      563 2024-04-16 15:58:07.667805 Velkoz-0.0.55/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-16 15:58:07.627935 Velkoz-0.0.55/Velkoz/
+-rw-rw-rw-   0        0        0      785 2024-04-16 11:13:15.000000 Velkoz-0.0.55/Velkoz/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 15:58:07.647106 Velkoz-0.0.55/Velkoz/data/
+-rw-rw-rw-   0        0        0       48 2024-04-13 20:58:45.000000 Velkoz-0.0.55/Velkoz/data/__init__.py
+-rw-rw-rw-   0        0        0     2638 2024-04-16 15:11:09.000000 Velkoz-0.0.55/Velkoz/data/champion.py
+-rw-rw-rw-   0        0        0     2057 2024-04-16 15:44:04.000000 Velkoz-0.0.55/Velkoz/data/common.py
+drwxrwxrwx   0        0        0        0 2024-04-16 15:58:07.654285 Velkoz-0.0.55/Velkoz/eye/
+-rw-rw-rw-   0        0        0      150 2024-03-23 23:06:35.000000 Velkoz-0.0.55/Velkoz/eye/__init__.py
+-rw-rw-rw-   0        0        0      523 2024-04-10 19:31:41.000000 Velkoz-0.0.55/Velkoz/eye/account.py
+-rw-rw-rw-   0        0        0      591 2024-04-09 19:37:05.000000 Velkoz-0.0.55/Velkoz/eye/champion_mastery.py
+-rw-rw-rw-   0        0        0        8 2024-03-22 13:50:02.000000 Velkoz-0.0.55/Velkoz/eye/common.py
+-rw-rw-rw-   0        0        0     7581 2024-04-12 12:51:42.000000 Velkoz-0.0.55/Velkoz/eye/match.py
+-rw-rw-rw-   0        0        0     1976 2024-04-10 19:31:40.000000 Velkoz-0.0.55/Velkoz/eye/summoner.py
+-rw-rw-rw-   0        0        0     3276 2024-04-16 15:09:23.000000 Velkoz-0.0.55/Velkoz/settings.py
+-rw-rw-rw-   0        0        0     1032 2024-04-16 15:57:38.000000 Velkoz-0.0.55/Velkoz/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 15:58:07.659333 Velkoz-0.0.55/Velkoz/supp/
+-rw-rw-rw-   0        0        0      154 2024-04-16 10:08:55.000000 Velkoz-0.0.55/Velkoz/supp/__init__.py
+-rw-rw-rw-   0        0        0      601 2024-04-10 19:50:35.000000 Velkoz-0.0.55/Velkoz/supp/account.py
+-rw-rw-rw-   0        0        0      280 2024-04-16 11:05:52.000000 Velkoz-0.0.55/Velkoz/supp/champion.py
+-rw-rw-rw-   0        0        0     1165 2024-04-11 21:19:17.000000 Velkoz-0.0.55/Velkoz/supp/champion_mastery.py
+-rw-rw-rw-   0        0        0      270 2024-04-11 21:19:18.000000 Velkoz-0.0.55/Velkoz/supp/match.py
+-rw-rw-rw-   0        0        0     1681 2024-04-10 19:50:14.000000 Velkoz-0.0.55/Velkoz/supp/summoner.py
+drwxrwxrwx   0        0        0        0 2024-04-16 15:58:07.665804 Velkoz-0.0.55/Velkoz/tentacles/
+-rw-rw-rw-   0        0        0      213 2024-04-11 21:19:17.000000 Velkoz-0.0.55/Velkoz/tentacles/__init__.py
+-rw-rw-rw-   0        0        0     1224 2024-03-22 11:07:43.000000 Velkoz-0.0.55/Velkoz/tentacles/account.py
+-rw-rw-rw-   0        0        0     3340 2024-04-11 21:19:18.000000 Velkoz-0.0.55/Velkoz/tentacles/champion_mastery.py
+-rw-rw-rw-   0        0        0     4543 2024-04-12 22:57:44.000000 Velkoz-0.0.55/Velkoz/tentacles/common.py
+-rw-rw-rw-   0        0        0       60 2024-04-05 19:09:48.000000 Velkoz-0.0.55/Velkoz/tentacles/config.py
+-rw-rw-rw-   0        0        0     1650 2024-03-22 13:51:43.000000 Velkoz-0.0.55/Velkoz/tentacles/match.py
+-rw-rw-rw-   0        0        0     1416 2024-03-22 11:06:12.000000 Velkoz-0.0.55/Velkoz/tentacles/summoner.py
+-rw-rw-rw-   0        0        0     6575 2024-04-16 15:11:30.000000 Velkoz-0.0.55/Velkoz/velkoz.py
+drwxrwxrwx   0        0        0        0 2024-04-16 15:58:07.666809 Velkoz-0.0.55/Velkoz.egg-info/
+-rw-rw-rw-   0        0        0      563 2024-04-16 15:58:07.000000 Velkoz-0.0.55/Velkoz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      780 2024-04-16 15:58:07.000000 Velkoz-0.0.55/Velkoz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 15:58:07.000000 Velkoz-0.0.55/Velkoz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-16 15:58:07.000000 Velkoz-0.0.55/Velkoz.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-16 15:58:07.000000 Velkoz-0.0.55/Velkoz.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-16 15:58:07.669357 Velkoz-0.0.55/setup.cfg
```

### Comparing `Velkoz-0.0.52/PKG-INFO` & `Velkoz-0.0.55/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Velkoz
-Version: 0.0.52
+Version: 0.0.55
 Summary: Velkoz Riot Api package
 Author: Nabattis
 Author-email: <ferreirafernando6205@gmail.com>
 Keywords: python,riotapi,api,velkoz
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `Velkoz-0.0.52/Velkoz/__init__.py` & `Velkoz-0.0.55/Velkoz/__init__.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.52/Velkoz/data/champion.py` & `Velkoz-0.0.55/Velkoz/data/champion.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.52/Velkoz/eye/account.py` & `Velkoz-0.0.55/Velkoz/eye/account.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.52/Velkoz/eye/champion_mastery.py` & `Velkoz-0.0.55/Velkoz/eye/champion_mastery.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.52/Velkoz/eye/match.py` & `Velkoz-0.0.55/Velkoz/eye/match.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.52/Velkoz/eye/summoner.py` & `Velkoz-0.0.55/Velkoz/eye/summoner.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.52/Velkoz/settings.py` & `Velkoz-0.0.55/Velkoz/settings.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.52/Velkoz/setup.py` & `Velkoz-0.0.55/Velkoz/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
  #python setup.py sdist bdist_wheel
-VERSION = '0.0.52' 
+VERSION = '0.0.55' 
 DESCRIPTION = 'Velkoz Riot Api package'
 LONG_DESCRIPTION = 'Package that uses RiotApi to get information.\n Made to gain experience so it is not something as advanced as the other packages that do the same. Would not recommend.'
 
 # Setting up
 setup(
         name="Velkoz", 
         version=VERSION,
```

### Comparing `Velkoz-0.0.52/Velkoz/supp/account.py` & `Velkoz-0.0.55/Velkoz/supp/account.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.52/Velkoz/supp/champion_mastery.py` & `Velkoz-0.0.55/Velkoz/supp/champion_mastery.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.52/Velkoz/supp/summoner.py` & `Velkoz-0.0.55/Velkoz/supp/summoner.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.52/Velkoz/tentacles/account.py` & `Velkoz-0.0.55/Velkoz/tentacles/account.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.52/Velkoz/tentacles/champion_mastery.py` & `Velkoz-0.0.55/Velkoz/tentacles/champion_mastery.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.52/Velkoz/tentacles/common.py` & `Velkoz-0.0.55/Velkoz/tentacles/common.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.52/Velkoz/tentacles/match.py` & `Velkoz-0.0.55/Velkoz/tentacles/match.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.52/Velkoz/tentacles/summoner.py` & `Velkoz-0.0.55/Velkoz/tentacles/summoner.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.52/Velkoz/velkoz.py` & `Velkoz-0.0.55/Velkoz/velkoz.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.52/Velkoz.egg-info/PKG-INFO` & `Velkoz-0.0.55/Velkoz.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Velkoz
-Version: 0.0.52
+Version: 0.0.55
 Summary: Velkoz Riot Api package
 Author: Nabattis
 Author-email: <ferreirafernando6205@gmail.com>
 Keywords: python,riotapi,api,velkoz
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `Velkoz-0.0.52/Velkoz.egg-info/SOURCES.txt` & `Velkoz-0.0.55/Velkoz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

