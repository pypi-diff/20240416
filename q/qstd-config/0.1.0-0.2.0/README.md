# Comparing `tmp/qstd_config-0.1.0.tar.gz` & `tmp/qstd_config-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qstd_config-0.1.0.tar", last modified: Sun Apr  7 17:42:48 2024, max compression
+gzip compressed data, was "qstd_config-0.2.0.tar", last modified: Tue Apr 16 16:57:54 2024, max compression
```

## Comparing `qstd_config-0.1.0.tar` & `qstd_config-0.2.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-04-07 17:42:48.594166 qstd_config-0.1.0/
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     1054 2024-03-24 20:15:12.000000 qstd_config-0.1.0/LICENSE
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     4761 2024-04-07 17:42:48.594166 qstd_config-0.1.0/PKG-INFO
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     4425 2024-03-30 10:45:12.000000 qstd_config-0.1.0/README.md
-drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-04-07 17:42:48.594166 qstd_config-0.1.0/qstd_config/
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       63 2024-03-30 08:39:00.000000 qstd_config-0.1.0/qstd_config/__init__.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      479 2024-03-30 08:43:39.000000 qstd_config-0.1.0/qstd_config/base.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     3665 2024-03-30 09:16:04.000000 qstd_config-0.1.0/qstd_config/config.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     2118 2024-03-29 07:29:07.000000 qstd_config-0.1.0/qstd_config/env.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      976 2024-03-29 07:43:48.000000 qstd_config-0.1.0/qstd_config/proxy.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       88 2024-03-28 10:41:57.000000 qstd_config-0.1.0/qstd_config/types.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     1581 2024-03-30 09:16:23.000000 qstd_config-0.1.0/qstd_config/utils.py
-drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-04-07 17:42:48.594166 qstd_config-0.1.0/qstd_config.egg-info/
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     4761 2024-04-07 17:42:48.000000 qstd_config-0.1.0/qstd_config.egg-info/PKG-INFO
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      437 2024-04-07 17:42:48.000000 qstd_config-0.1.0/qstd_config.egg-info/SOURCES.txt
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)        1 2024-04-07 17:42:48.000000 qstd_config-0.1.0/qstd_config.egg-info/dependency_links.txt
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       42 2024-04-07 17:42:48.000000 qstd_config-0.1.0/qstd_config.egg-info/requires.txt
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       12 2024-04-07 17:42:48.000000 qstd_config-0.1.0/qstd_config.egg-info/top_level.txt
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       38 2024-04-07 17:42:48.594166 qstd_config-0.1.0/setup.cfg
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      719 2024-04-07 17:42:46.000000 qstd_config-0.1.0/setup.py
-drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-04-07 17:42:48.594166 qstd_config-0.1.0/test/
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)        0 2024-03-30 08:37:27.000000 qstd_config-0.1.0/test/__init__.py
-drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-04-07 17:42:48.594166 qstd_config-0.1.0/test/multiprocess/
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     2095 2024-03-30 09:28:13.000000 qstd_config-0.1.0/test/multiprocess/__init__.py
-drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-04-07 17:42:48.594166 qstd_config-0.1.0/test/single_process/
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     1702 2024-03-30 09:16:09.000000 qstd_config-0.1.0/test/single_process/__init__.py
+drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-04-16 16:57:54.015853 qstd_config-0.2.0/
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     1054 2024-03-24 20:15:12.000000 qstd_config-0.2.0/LICENSE
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     4761 2024-04-16 16:57:54.015853 qstd_config-0.2.0/PKG-INFO
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     4425 2024-03-30 10:45:12.000000 qstd_config-0.2.0/README.md
+drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-04-16 16:57:54.015853 qstd_config-0.2.0/qstd_config/
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       63 2024-03-30 08:39:00.000000 qstd_config-0.2.0/qstd_config/__init__.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      479 2024-03-30 08:43:39.000000 qstd_config-0.2.0/qstd_config/base.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     3665 2024-03-30 09:16:04.000000 qstd_config-0.2.0/qstd_config/config.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     2118 2024-03-29 07:29:07.000000 qstd_config-0.2.0/qstd_config/env.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      976 2024-03-29 07:43:48.000000 qstd_config-0.2.0/qstd_config/proxy.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       88 2024-03-28 10:41:57.000000 qstd_config-0.2.0/qstd_config/types.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     1581 2024-03-30 09:16:23.000000 qstd_config-0.2.0/qstd_config/utils.py
+drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-04-16 16:57:54.015853 qstd_config-0.2.0/qstd_config.egg-info/
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     4761 2024-04-16 16:57:54.000000 qstd_config-0.2.0/qstd_config.egg-info/PKG-INFO
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      437 2024-04-16 16:57:54.000000 qstd_config-0.2.0/qstd_config.egg-info/SOURCES.txt
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)        1 2024-04-16 16:57:54.000000 qstd_config-0.2.0/qstd_config.egg-info/dependency_links.txt
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       42 2024-04-16 16:57:54.000000 qstd_config-0.2.0/qstd_config.egg-info/requires.txt
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       12 2024-04-16 16:57:54.000000 qstd_config-0.2.0/qstd_config.egg-info/top_level.txt
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       38 2024-04-16 16:57:54.015853 qstd_config-0.2.0/setup.cfg
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      719 2024-04-16 16:57:39.000000 qstd_config-0.2.0/setup.py
+drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-04-16 16:57:54.015853 qstd_config-0.2.0/test/
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)        0 2024-03-30 08:37:27.000000 qstd_config-0.2.0/test/__init__.py
+drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-04-16 16:57:54.015853 qstd_config-0.2.0/test/multiprocess/
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     2095 2024-03-30 09:28:13.000000 qstd_config-0.2.0/test/multiprocess/__init__.py
+drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-04-16 16:57:54.015853 qstd_config-0.2.0/test/single_process/
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     1702 2024-03-30 09:16:09.000000 qstd_config-0.2.0/test/single_process/__init__.py
```

### Comparing `qstd_config-0.1.0/LICENSE` & `qstd_config-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qstd_config-0.1.0/PKG-INFO` & `qstd_config-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qstd_config
-Version: 0.1.0
+Version: 0.2.0
 Summary: Application configuration manager
 Home-page: https://github.com/QuisEgoSum/qstd-config
 Author: QuisEgoSum
 Author-email: subbotin.evdokim@gmail.com
 License: MIT
 Keywords: config yaml env
 Requires-Python: >=3.7
```

### Comparing `qstd_config-0.1.0/README.md` & `qstd_config-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `qstd_config-0.1.0/qstd_config/config.py` & `qstd_config-0.2.0/qstd_config/config.py`

 * *Files identical despite different names*

### Comparing `qstd_config-0.1.0/qstd_config/env.py` & `qstd_config-0.2.0/qstd_config/env.py`

 * *Files identical despite different names*

### Comparing `qstd_config-0.1.0/qstd_config/proxy.py` & `qstd_config-0.2.0/qstd_config/proxy.py`

 * *Files identical despite different names*

### Comparing `qstd_config-0.1.0/qstd_config/utils.py` & `qstd_config-0.2.0/qstd_config/utils.py`

 * *Files identical despite different names*

### Comparing `qstd_config-0.1.0/qstd_config.egg-info/PKG-INFO` & `qstd_config-0.2.0/qstd_config.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qstd-config
-Version: 0.1.0
+Version: 0.2.0
 Summary: Application configuration manager
 Home-page: https://github.com/QuisEgoSum/qstd-config
 Author: QuisEgoSum
 Author-email: subbotin.evdokim@gmail.com
 License: MIT
 Keywords: config yaml env
 Requires-Python: >=3.7
```

### Comparing `qstd_config-0.1.0/setup.py` & `qstd_config-0.2.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 def readme():
     with open('README.md', 'r') as f:
         return f.read()
 
 
 setup(
     name='qstd_config',
-    version='0.1.0',
+    version='0.2.0',
     author='QuisEgoSum',
     author_email='subbotin.evdokim@gmail.com',
     description='Application configuration manager',
     long_description=readme(),
     long_description_content_type='text/markdown',
     url='https://github.com/QuisEgoSum/qstd-config',
     packages=find_packages(exclude=['tmp', 'example', '*test*']),
     install_requires=[
-        'pydantic==1.10.0',
-        'PyYAML==6.0',
-        'jsonref==0.2'
+        'pydantic>=1.10.0',
+        'PyYAML>=6.0',
+        'jsonref>=0.2'
     ],
     keywords='config yaml env',
     python_requires='>=3.7',
     license='MIT',
     include_package_data=False
 )
```

### Comparing `qstd_config-0.1.0/test/multiprocess/__init__.py` & `qstd_config-0.2.0/test/multiprocess/__init__.py`

 * *Files identical despite different names*

### Comparing `qstd_config-0.1.0/test/single_process/__init__.py` & `qstd_config-0.2.0/test/single_process/__init__.py`

 * *Files identical despite different names*

