# Comparing `tmp/danila-lib-1.0.4.tar.gz` & `tmp/danila-lib-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "danila-lib-1.0.4.tar", last modified: Mon Apr 15 17:25:42 2024, max compression
+gzip compressed data, was "danila-lib-1.0.5.tar", last modified: Tue Apr 16 08:16:11 2024, max compression
```

## Comparing `danila-lib-1.0.4.tar` & `danila-lib-1.0.5.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 17:25:42.576403 danila-lib-1.0.4/
--rw-rw-rw-   0        0        0     4169 2024-04-15 17:25:42.575407 danila-lib-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-15 12:08:08.000000 danila-lib-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-15 17:25:42.553505 danila-lib-1.0.4/danila/
--rw-rw-rw-   0        0        0        0 2024-04-15 11:55:56.000000 danila-lib-1.0.4/danila/__init__.py
--rw-rw-rw-   0        0        0      402 2024-04-15 17:25:24.000000 danila-lib-1.0.4/danila/danila.py
-drwxrwxrwx   0        0        0        0 2024-04-15 17:25:42.571425 danila-lib-1.0.4/danila_lib.egg-info/
--rw-rw-rw-   0        0        0     4169 2024-04-15 17:25:42.000000 danila-lib-1.0.4/danila_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      355 2024-04-15 17:25:42.000000 danila-lib-1.0.4/danila_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 17:25:42.000000 danila-lib-1.0.4/danila_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1881 2024-04-15 17:25:42.000000 danila-lib-1.0.4/danila_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-15 17:25:42.000000 danila-lib-1.0.4/danila_lib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-15 17:25:42.571425 danila-lib-1.0.4/data/
--rw-rw-rw-   0        0        0        0 2024-04-15 12:01:57.000000 danila-lib-1.0.4/data/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 17:25:42.572420 danila-lib-1.0.4/data/neuro/
--rw-rw-rw-   0        0        0     3808 2024-04-15 17:24:43.000000 danila-lib-1.0.4/data/neuro/Rama_classify_class.py
--rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.0.4/data/neuro/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 17:25:42.573416 danila-lib-1.0.4/data/result/
--rw-rw-rw-   0        0        0       89 2023-11-28 06:30:22.000000 danila-lib-1.0.4/data/result/Class_im.py
--rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.0.4/data/result/__init__.py
--rw-rw-rw-   0        0        0       42 2024-04-15 17:25:42.580385 danila-lib-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      983 2024-04-15 17:25:35.000000 danila-lib-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 08:16:11.513296 danila-lib-1.0.5/
+-rw-rw-rw-   0        0        0     5292 2024-04-16 08:16:11.512300 danila-lib-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1125 2024-04-16 08:15:57.000000 danila-lib-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-16 08:16:11.485421 danila-lib-1.0.5/danila/
+-rw-rw-rw-   0        0        0        0 2024-04-15 11:55:56.000000 danila-lib-1.0.5/danila/__init__.py
+-rw-rw-rw-   0        0        0      663 2024-04-16 08:05:12.000000 danila-lib-1.0.5/danila/danila.py
+drwxrwxrwx   0        0        0        0 2024-04-16 08:16:11.504336 danila-lib-1.0.5/danila_lib.egg-info/
+-rw-rw-rw-   0        0        0     5292 2024-04-16 08:16:11.000000 danila-lib-1.0.5/danila_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      376 2024-04-16 08:16:11.000000 danila-lib-1.0.5/danila_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 08:16:11.000000 danila-lib-1.0.5/danila_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1881 2024-04-16 08:16:11.000000 danila-lib-1.0.5/danila_lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-16 08:16:11.000000 danila-lib-1.0.5/danila_lib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-16 08:16:11.505331 danila-lib-1.0.5/data/
+-rw-rw-rw-   0        0        0        0 2024-04-15 12:01:57.000000 danila-lib-1.0.5/data/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 08:16:11.506327 danila-lib-1.0.5/data/neuro/
+-rw-rw-rw-   0        0        0     2721 2024-04-16 08:05:12.000000 danila-lib-1.0.5/data/neuro/Rama_classify_class.py
+-rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.0.5/data/neuro/__init__.py
+-rw-rw-rw-   0        0        0       71 2024-04-16 07:31:21.000000 danila-lib-1.0.5/data/neuro/models.py
+drwxrwxrwx   0        0        0        0 2024-04-16 08:16:11.511304 danila-lib-1.0.5/data/result/
+-rw-rw-rw-   0        0        0       89 2023-11-28 06:30:22.000000 danila-lib-1.0.5/data/result/Class_im.py
+-rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.0.5/data/result/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-04-16 08:16:11.514291 danila-lib-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      983 2024-04-16 08:16:08.000000 danila-lib-1.0.5/setup.py
```

### Comparing `danila-lib-1.0.4/danila_lib.egg-info/requires.txt` & `danila-lib-1.0.5/danila_lib.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `danila-lib-1.0.4/setup.py` & `danila-lib-1.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
   with open('requirements.txt', 'r') as f:
     a = f.read()
   b = a.split()
   return b
 
 setup(
   name='danila-lib',
-  version='1.0.4',
+  version='1.0.5',
   author='arseniy_zhuck',
   author_email='arseniyzhuck@mail.ru',
   description='This is the module for detecting and classifying text on rama pictures',
   long_description=readme(),
   long_description_content_type='text/markdown',
   url='https://github.com/Arseniy-Zhuck/danila_lib',
   packages=find_packages(),
```

