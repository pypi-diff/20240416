# Comparing `tmp/ctlsettings-0.3.1.tar.gz` & `tmp/ctlsettings-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/nataliadittren/Desktop/workspace/ctlsettings/dist/.tmp-nsjeebz3/ctlsettings-0.3.1.tar", last modified: Mon Jan  8 19:11:06 2024, max compression
+gzip compressed data, was "ctlsettings-0.3.2.tar", last modified: Tue Apr 16 17:23:55 2024, max compression
```

## Comparing `ctlsettings-0.3.1.tar` & `ctlsettings-0.3.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 nataliadittren   (502) staff       (20)        0 2024-01-08 19:11:06.904750 ctlsettings-0.3.1/
--rw-r--r--   0 nataliadittren   (502) staff       (20)    35149 2023-08-17 17:27:01.000000 ctlsettings-0.3.1/LICENSE
--rw-r--r--   0 nataliadittren   (502) staff       (20)      733 2024-01-08 19:11:06.904352 ctlsettings-0.3.1/PKG-INFO
--rw-r--r--   0 nataliadittren   (502) staff       (20)     4364 2023-08-17 17:27:01.000000 ctlsettings-0.3.1/README.md
-drwxr-xr-x   0 nataliadittren   (502) staff       (20)        0 2024-01-08 19:11:06.901772 ctlsettings-0.3.1/ctlsettings/
--rw-r--r--   0 nataliadittren   (502) staff       (20)        0 2023-08-17 17:27:01.000000 ctlsettings-0.3.1/ctlsettings/__init__.py
--rw-r--r--   0 nataliadittren   (502) staff       (20)     2886 2024-01-08 18:58:50.000000 ctlsettings-0.3.1/ctlsettings/production.py
--rw-r--r--   0 nataliadittren   (502) staff       (20)     5869 2024-01-08 18:58:50.000000 ctlsettings-0.3.1/ctlsettings/shared.py
--rw-r--r--   0 nataliadittren   (502) staff       (20)     3044 2024-01-08 18:58:50.000000 ctlsettings-0.3.1/ctlsettings/staging.py
--rw-r--r--   0 nataliadittren   (502) staff       (20)      197 2023-08-17 17:27:01.000000 ctlsettings-0.3.1/ctlsettings/storages.py
-drwxr-xr-x   0 nataliadittren   (502) staff       (20)        0 2024-01-08 19:11:06.903871 ctlsettings-0.3.1/ctlsettings.egg-info/
--rw-r--r--   0 nataliadittren   (502) staff       (20)      733 2024-01-08 19:11:06.000000 ctlsettings-0.3.1/ctlsettings.egg-info/PKG-INFO
--rw-r--r--   0 nataliadittren   (502) staff       (20)      319 2024-01-08 19:11:06.000000 ctlsettings-0.3.1/ctlsettings.egg-info/SOURCES.txt
--rw-r--r--   0 nataliadittren   (502) staff       (20)        1 2024-01-08 19:11:06.000000 ctlsettings-0.3.1/ctlsettings.egg-info/dependency_links.txt
--rw-r--r--   0 nataliadittren   (502) staff       (20)      178 2024-01-08 19:11:06.000000 ctlsettings-0.3.1/ctlsettings.egg-info/requires.txt
--rw-r--r--   0 nataliadittren   (502) staff       (20)       12 2024-01-08 19:11:06.000000 ctlsettings-0.3.1/ctlsettings.egg-info/top_level.txt
--rw-r--r--   0 nataliadittren   (502) staff       (20)       38 2024-01-08 19:11:06.904858 ctlsettings-0.3.1/setup.cfg
--rw-r--r--   0 nataliadittren   (502) staff       (20)      869 2024-01-08 19:08:55.000000 ctlsettings-0.3.1/setup.py
+drwxr-xr-x   0 nik       (1000) nik       (1000)        0 2024-04-16 17:23:55.130837 ctlsettings-0.3.2/
+-rw-r--r--   0 nik       (1000) nik       (1000)    35149 2023-01-05 21:11:11.000000 ctlsettings-0.3.2/LICENSE
+-rw-r--r--   0 nik       (1000) nik       (1000)      733 2024-04-16 17:23:55.130837 ctlsettings-0.3.2/PKG-INFO
+-rw-r--r--   0 nik       (1000) nik       (1000)     4364 2024-04-16 17:23:05.000000 ctlsettings-0.3.2/README.md
+drwxr-xr-x   0 nik       (1000) nik       (1000)        0 2024-04-16 17:23:55.129837 ctlsettings-0.3.2/ctlsettings/
+-rw-r--r--   0 nik       (1000) nik       (1000)        0 2023-01-10 19:22:37.000000 ctlsettings-0.3.2/ctlsettings/__init__.py
+-rw-r--r--   0 nik       (1000) nik       (1000)     2979 2024-04-05 15:01:50.000000 ctlsettings-0.3.2/ctlsettings/production.py
+-rw-r--r--   0 nik       (1000) nik       (1000)     5943 2024-03-21 15:19:30.000000 ctlsettings-0.3.2/ctlsettings/shared.py
+-rw-r--r--   0 nik       (1000) nik       (1000)     3137 2024-04-05 15:01:50.000000 ctlsettings-0.3.2/ctlsettings/staging.py
+-rw-r--r--   0 nik       (1000) nik       (1000)      197 2023-02-21 21:02:15.000000 ctlsettings-0.3.2/ctlsettings/storages.py
+drwxr-xr-x   0 nik       (1000) nik       (1000)        0 2024-04-16 17:23:55.130837 ctlsettings-0.3.2/ctlsettings.egg-info/
+-rw-r--r--   0 nik       (1000) nik       (1000)      733 2024-04-16 17:23:55.000000 ctlsettings-0.3.2/ctlsettings.egg-info/PKG-INFO
+-rw-r--r--   0 nik       (1000) nik       (1000)      319 2024-04-16 17:23:55.000000 ctlsettings-0.3.2/ctlsettings.egg-info/SOURCES.txt
+-rw-r--r--   0 nik       (1000) nik       (1000)        1 2024-04-16 17:23:55.000000 ctlsettings-0.3.2/ctlsettings.egg-info/dependency_links.txt
+-rw-r--r--   0 nik       (1000) nik       (1000)      178 2024-04-16 17:23:55.000000 ctlsettings-0.3.2/ctlsettings.egg-info/requires.txt
+-rw-r--r--   0 nik       (1000) nik       (1000)       12 2024-04-16 17:23:55.000000 ctlsettings-0.3.2/ctlsettings.egg-info/top_level.txt
+-rw-r--r--   0 nik       (1000) nik       (1000)       38 2024-04-16 17:23:55.130837 ctlsettings-0.3.2/setup.cfg
+-rw-r--r--   0 nik       (1000) nik       (1000)      869 2024-04-16 17:23:05.000000 ctlsettings-0.3.2/setup.py
```

### Comparing `ctlsettings-0.3.1/LICENSE` & `ctlsettings-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ctlsettings-0.3.1/PKG-INFO` & `ctlsettings-0.3.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctlsettings
-Version: 0.3.1
+Version: 0.3.2
 Summary: Columbia CTL common Django base settings
 Home-page: https://github.com/ccnmtl/ctlsettings
 Author: Columbia University Center for Teaching and Learning
 Author-email: ctl-dev@columbia.edu
 License: GPL-3.0-or-later
 Platform: any
 License-File: LICENSE
```

### Comparing `ctlsettings-0.3.1/README.md` & `ctlsettings-0.3.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 ### Installation
 
 First, install it with
 
     $ pip install ctlsettings
 
-or add `ctlsettings==0.2.0` to your `requirements.txt`.
+or add `ctlsettings==0.3.2` to your `requirements.txt`.
 
 ### Dependencies
 
 The following libraries are used in some way, so they'll need to be installed:
 
 * django-cas-ng
 * django-debug-toolbar
```

### Comparing `ctlsettings-0.3.1/ctlsettings/production.py` & `ctlsettings-0.3.2/ctlsettings/production.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,17 @@
                 'format': '{asctime} {levelname} {message}',
                 'style': '{'
             },
         },
         'handlers': {
             'file': {
                 'level': 'INFO',
-                'class': 'logging.FileHandler',
+                'class': 'logging.handlers.RotatingFileHandler',
+                'backupCount': 4,
+                'maxBytes': 10*1024*1024,
                 'filename': '/var/log/django/' + project + '.log',
                 'formatter': 'timestamped',
             },
         },
         'loggers': {
             'django': {
                 'handlers': ['file'],
```

### Comparing `ctlsettings-0.3.1/ctlsettings/shared.py` & `ctlsettings-0.3.2/ctlsettings/shared.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,18 @@
         '127.0.0.1',
     ]
 
     public_ip = get_ec2_instance_ip()
     if public_ip:
         ALLOWED_HOSTS += [public_ip]
 
+    CSRF_TRUSTED_ORIGINS = [
+        'https://*.ctl.columbia.edu',
+    ]
+
     DATABASES = {
         'default': {
             'ENGINE': 'django.db.backends.postgresql',
             'NAME': project,
             'HOST': '',
             'PORT': 5432,
             'USER': '',
```

### Comparing `ctlsettings-0.3.1/ctlsettings/staging.py` & `ctlsettings-0.3.2/ctlsettings/staging.py`

 * *Files 3% similar despite different names*

```diff
@@ -82,15 +82,17 @@
                 'format': '{asctime} {levelname} {message}',
                 'style': '{'
             },
         },
         'handlers': {
             'file': {
                 'level': 'INFO',
-                'class': 'logging.FileHandler',
+                'class': 'logging.handlers.RotatingFileHandler',
+                'backupCount': 4,
+                'maxBytes': 10*1024*1024,
                 'filename': '/var/log/django/' + project + '.log',
                 'formatter': 'timestamped',
             },
         },
         'loggers': {
             'django': {
                 'handlers': ['file'],
```

### Comparing `ctlsettings-0.3.1/ctlsettings.egg-info/PKG-INFO` & `ctlsettings-0.3.2/ctlsettings.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctlsettings
-Version: 0.3.1
+Version: 0.3.2
 Summary: Columbia CTL common Django base settings
 Home-page: https://github.com/ccnmtl/ctlsettings
 Author: Columbia University Center for Teaching and Learning
 Author-email: ctl-dev@columbia.edu
 License: GPL-3.0-or-later
 Platform: any
 License-File: LICENSE
```

### Comparing `ctlsettings-0.3.1/setup.py` & `ctlsettings-0.3.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='ctlsettings',
-    version='0.3.1',
+    version='0.3.2',
     author='Columbia University Center for Teaching and Learning',
     author_email='ctl-dev@columbia.edu',
     url='https://github.com/ccnmtl/ctlsettings',
     description='Columbia CTL common Django base settings',
     long_description='common settings we use across all our projects',
     install_requires = [
         'django-cas-ng',
```

