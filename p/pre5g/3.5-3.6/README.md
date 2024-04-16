# Comparing `tmp/pre5g-3.5.tar.gz` & `tmp/pre5g-3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pre5g-3.5.tar", last modified: Tue Apr 16 04:30:06 2024, max compression
+gzip compressed data, was "dist/pre5g-3.6.tar", last modified: Tue Apr 16 05:17:10 2024, max compression
```

## Comparing `pre5g-3.5.tar` & `pre5g-3.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 trainee   (1003) trainee   (1003)        0 2024-04-16 04:30:06.575567 pre5g-3.5/
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     1063 2024-03-26 07:38:31.000000 pre5g-3.5/LICENSE
--rw-r--r--   0 trainee   (1003) trainee   (1003)      491 2024-04-16 04:30:06.574567 pre5g-3.5/PKG-INFO
--rw-rw-r--   0 trainee   (1003) trainee   (1003)       82 2024-03-26 07:39:06.000000 pre5g-3.5/README.md
-drwxrwxr-x   0 trainee   (1003) trainee   (1003)        0 2024-04-16 04:30:06.573567 pre5g-3.5/pre5g/
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     1137 2024-04-04 11:14:45.000000 pre5g-3.5/pre5g/__init__.py
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     1042 2024-04-08 06:54:23.000000 pre5g-3.5/pre5g/labelen.py
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     2707 2024-04-01 11:33:46.000000 pre5g-3.5/pre5g/normalization.py
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     4306 2024-04-08 09:30:56.000000 pre5g-3.5/pre5g/nullvalue.py
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     3134 2024-04-16 04:29:45.000000 pre5g-3.5/pre5g/onehoten.py
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     3355 2024-04-15 10:02:56.000000 pre5g-3.5/pre5g/robustscaler.py
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     3124 2024-04-01 11:39:06.000000 pre5g-3.5/pre5g/standardization.py
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     2422 2024-04-15 07:20:59.000000 pre5g-3.5/pre5g/winsorization.py
-drwxrwxr-x   0 trainee   (1003) trainee   (1003)        0 2024-04-16 04:30:06.574567 pre5g-3.5/pre5g.egg-info/
--rw-r--r--   0 trainee   (1003) trainee   (1003)      491 2024-04-16 04:30:06.000000 pre5g-3.5/pre5g.egg-info/PKG-INFO
--rw-rw-r--   0 trainee   (1003) trainee   (1003)      307 2024-04-16 04:30:06.000000 pre5g-3.5/pre5g.egg-info/SOURCES.txt
--rw-rw-r--   0 trainee   (1003) trainee   (1003)        1 2024-04-16 04:30:06.000000 pre5g-3.5/pre5g.egg-info/dependency_links.txt
--rw-rw-r--   0 trainee   (1003) trainee   (1003)        6 2024-04-16 04:30:06.000000 pre5g-3.5/pre5g.egg-info/top_level.txt
--rw-rw-r--   0 trainee   (1003) trainee   (1003)       38 2024-04-16 04:30:06.575567 pre5g-3.5/setup.cfg
--rw-rw-r--   0 trainee   (1003) trainee   (1003)      600 2024-04-16 04:29:51.000000 pre5g-3.5/setup.py
+drwxrwxr-x   0 trainee   (1003) trainee   (1003)        0 2024-04-16 05:17:10.849445 pre5g-3.6/
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     1063 2024-03-26 07:38:31.000000 pre5g-3.6/LICENSE
+-rw-r--r--   0 trainee   (1003) trainee   (1003)      491 2024-04-16 05:17:10.849445 pre5g-3.6/PKG-INFO
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)       82 2024-03-26 07:39:06.000000 pre5g-3.6/README.md
+drwxrwxr-x   0 trainee   (1003) trainee   (1003)        0 2024-04-16 05:17:10.848445 pre5g-3.6/pre5g/
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     1137 2024-04-04 11:14:45.000000 pre5g-3.6/pre5g/__init__.py
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     1042 2024-04-08 06:54:23.000000 pre5g-3.6/pre5g/labelen.py
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     2707 2024-04-01 11:33:46.000000 pre5g-3.6/pre5g/normalization.py
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     3398 2024-04-16 05:16:56.000000 pre5g-3.6/pre5g/nullvalue.py
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     3134 2024-04-16 04:29:45.000000 pre5g-3.6/pre5g/onehoten.py
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     3355 2024-04-15 10:02:56.000000 pre5g-3.6/pre5g/robustscaler.py
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     3124 2024-04-01 11:39:06.000000 pre5g-3.6/pre5g/standardization.py
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     2422 2024-04-15 07:20:59.000000 pre5g-3.6/pre5g/winsorization.py
+drwxrwxr-x   0 trainee   (1003) trainee   (1003)        0 2024-04-16 05:17:10.849445 pre5g-3.6/pre5g.egg-info/
+-rw-r--r--   0 trainee   (1003) trainee   (1003)      491 2024-04-16 05:17:10.000000 pre5g-3.6/pre5g.egg-info/PKG-INFO
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)      307 2024-04-16 05:17:10.000000 pre5g-3.6/pre5g.egg-info/SOURCES.txt
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)        1 2024-04-16 05:17:10.000000 pre5g-3.6/pre5g.egg-info/dependency_links.txt
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)        6 2024-04-16 05:17:10.000000 pre5g-3.6/pre5g.egg-info/top_level.txt
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)       38 2024-04-16 05:17:10.849445 pre5g-3.6/setup.cfg
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)      600 2024-04-16 05:17:00.000000 pre5g-3.6/setup.py
```

### Comparing `pre5g-3.5/LICENSE` & `pre5g-3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pre5g-3.5/pre5g/__init__.py` & `pre5g-3.6/pre5g/__init__.py`

 * *Files identical despite different names*

### Comparing `pre5g-3.5/pre5g/labelen.py` & `pre5g-3.6/pre5g/labelen.py`

 * *Files identical despite different names*

### Comparing `pre5g-3.5/pre5g/normalization.py` & `pre5g-3.6/pre5g/normalization.py`

 * *Files identical despite different names*

### Comparing `pre5g-3.5/pre5g/onehoten.py` & `pre5g-3.6/pre5g/onehoten.py`

 * *Files identical despite different names*

### Comparing `pre5g-3.5/pre5g/robustscaler.py` & `pre5g-3.6/pre5g/robustscaler.py`

 * *Files identical despite different names*

### Comparing `pre5g-3.5/pre5g/standardization.py` & `pre5g-3.6/pre5g/standardization.py`

 * *Files identical despite different names*

### Comparing `pre5g-3.5/pre5g/winsorization.py` & `pre5g-3.6/pre5g/winsorization.py`

 * *Files identical despite different names*

### Comparing `pre5g-3.5/setup.py` & `pre5g-3.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pre5g',
-    version='3.5',
+    version='3.6',
     packages=find_packages(),
     description='An preprocessing package',
     author='SnehaM',
     author_email='1js20cs161@gmail.com',
     license='MIT',
     keywords=['example', 'package'],
     classifiers=[
```

