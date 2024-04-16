# Comparing `tmp/dekpkglock-0.1.8.tar.gz` & `tmp/dekpkglock-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dekpkglock-0.1.8.tar", last modified: Sun Apr  7 07:21:49 2024, max compression
+gzip compressed data, was "dekpkglock-0.1.9.tar", last modified: Tue Apr  9 09:50:40 2024, max compression
```

## Comparing `dekpkglock-0.1.8.tar` & `dekpkglock-0.1.9.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0      123 2024-04-07 07:21:47.768668 dekpkglock-0.1.8/README.md
--rw-r--r--   0        0        0        0 2024-04-07 07:21:47.768668 dekpkglock-0.1.8/dekpkglock/__init__.py
--rw-r--r--   0        0        0       42 2024-04-07 07:21:47.768668 dekpkglock-0.1.8/dekpkglock/click/__entry__.py
--rw-r--r--   0        0        0      479 2024-04-07 07:21:47.768668 dekpkglock-0.1.8/dekpkglock/click/__init__.py
--rw-r--r--   0        0        0      244 2024-04-07 07:21:47.768668 dekpkglock-0.1.8/dekpkglock/core/__init__.py
--rw-r--r--   0        0        0     2244 2024-04-07 07:21:47.768668 dekpkglock-0.1.8/dekpkglock/core/base/__init__.py
--rw-r--r--   0        0        0     1030 2024-04-07 07:21:47.768668 dekpkglock-0.1.8/dekpkglock/core/pdm.py
--rw-r--r--   0        0        0   140317 2024-04-07 07:21:47.768668 dekpkglock-0.1.8/dekpkglock/resources/pdm/dekspider/project/0.1.44/pdm.lock
--rw-r--r--   0        0        0   140317 2024-04-07 07:21:47.768668 dekpkglock-0.1.8/dekpkglock/resources/pdm/dekspider/project/0.1.45/pdm.lock
--rw-r--r--   0        0        0   101191 2024-04-07 07:21:47.772668 dekpkglock-0.1.8/dekpkglock/resources/pdm/dekspider/project/0.1.46/pdm.lock
--rw-r--r--   0        0        0   101213 2024-04-07 07:21:47.772668 dekpkglock-0.1.8/dekpkglock/resources/pdm/dekspider/project/0.1.47/pdm.lock
--rw-r--r--   0        0        0   101647 2024-04-07 07:21:47.772668 dekpkglock-0.1.8/dekpkglock/resources/pdm/dekspider/project/0.1.48/pdm.lock
--rw-r--r--   0        0        0   101647 2024-04-07 07:21:47.772668 dekpkglock-0.1.8/dekpkglock/resources/pdm/dekspider/project/0.1.49/pdm.lock
--rw-r--r--   0        0        0   101647 2024-04-07 07:21:47.772668 dekpkglock-0.1.8/dekpkglock/resources/pdm/dekspider/project/0.1.50/pdm.lock
--rw-r--r--   0        0        0    31259 2024-04-07 07:21:47.772668 dekpkglock-0.1.8/dekpkglock/resources/pdm/djcreator/project/0.1.47/pdm.lock
--rw-r--r--   0        0        0   123953 2024-04-07 07:21:47.772668 dekpkglock-0.1.8/dekpkglock/resources/pdm/djcreator/wrapper/0.1.47/pdm.lock
--rw-r--r--   0        0        0      476 2024-04-07 07:21:49.108677 dekpkglock-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      359 1970-01-01 00:00:00.000000 dekpkglock-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      123 2024-04-09 09:50:39.020932 dekpkglock-0.1.9/README.md
+-rw-r--r--   0        0        0        0 2024-04-09 09:50:39.020932 dekpkglock-0.1.9/dekpkglock/__init__.py
+-rw-r--r--   0        0        0       42 2024-04-09 09:50:39.020932 dekpkglock-0.1.9/dekpkglock/click/__entry__.py
+-rw-r--r--   0        0        0      479 2024-04-09 09:50:39.020932 dekpkglock-0.1.9/dekpkglock/click/__init__.py
+-rw-r--r--   0        0        0      244 2024-04-09 09:50:39.020932 dekpkglock-0.1.9/dekpkglock/core/__init__.py
+-rw-r--r--   0        0        0     2244 2024-04-09 09:50:39.020932 dekpkglock-0.1.9/dekpkglock/core/base/__init__.py
+-rw-r--r--   0        0        0     1030 2024-04-09 09:50:39.020932 dekpkglock-0.1.9/dekpkglock/core/pdm.py
+-rw-r--r--   0        0        0   140317 2024-04-09 09:50:39.020932 dekpkglock-0.1.9/dekpkglock/resources/pdm/dekspider/project/0.1.44/pdm.lock
+-rw-r--r--   0        0        0   140317 2024-04-09 09:50:39.024932 dekpkglock-0.1.9/dekpkglock/resources/pdm/dekspider/project/0.1.45/pdm.lock
+-rw-r--r--   0        0        0   101191 2024-04-09 09:50:39.024932 dekpkglock-0.1.9/dekpkglock/resources/pdm/dekspider/project/0.1.46/pdm.lock
+-rw-r--r--   0        0        0   101213 2024-04-09 09:50:39.024932 dekpkglock-0.1.9/dekpkglock/resources/pdm/dekspider/project/0.1.47/pdm.lock
+-rw-r--r--   0        0        0   101647 2024-04-09 09:50:39.024932 dekpkglock-0.1.9/dekpkglock/resources/pdm/dekspider/project/0.1.48/pdm.lock
+-rw-r--r--   0        0        0   101647 2024-04-09 09:50:39.024932 dekpkglock-0.1.9/dekpkglock/resources/pdm/dekspider/project/0.1.49/pdm.lock
+-rw-r--r--   0        0        0   101647 2024-04-09 09:50:39.024932 dekpkglock-0.1.9/dekpkglock/resources/pdm/dekspider/project/0.1.50/pdm.lock
+-rw-r--r--   0        0        0    98442 2024-04-09 09:50:39.024932 dekpkglock-0.1.9/dekpkglock/resources/pdm/dekspider/project/0.1.54/pdm.lock
+-rw-r--r--   0        0        0    31259 2024-04-09 09:50:39.028932 dekpkglock-0.1.9/dekpkglock/resources/pdm/djcreator/project/0.1.47/pdm.lock
+-rw-r--r--   0        0        0   123953 2024-04-09 09:50:39.028932 dekpkglock-0.1.9/dekpkglock/resources/pdm/djcreator/wrapper/0.1.47/pdm.lock
+-rw-r--r--   0        0        0      476 2024-04-09 09:50:40.300950 dekpkglock-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      359 1970-01-01 00:00:00.000000 dekpkglock-0.1.9/PKG-INFO
```

### Comparing `dekpkglock-0.1.8/dekpkglock/core/base/__init__.py` & `dekpkglock-0.1.9/dekpkglock/core/base/__init__.py`

 * *Files identical despite different names*

### Comparing `dekpkglock-0.1.8/dekpkglock/core/pdm.py` & `dekpkglock-0.1.9/dekpkglock/core/pdm.py`

 * *Files identical despite different names*

### Comparing `dekpkglock-0.1.8/dekpkglock/resources/pdm/dekspider/project/0.1.44/pdm.lock` & `dekpkglock-0.1.9/dekpkglock/resources/pdm/dekspider/project/0.1.44/pdm.lock`

 * *Files identical despite different names*

### Comparing `dekpkglock-0.1.8/dekpkglock/resources/pdm/dekspider/project/0.1.45/pdm.lock` & `dekpkglock-0.1.9/dekpkglock/resources/pdm/dekspider/project/0.1.45/pdm.lock`

 * *Files identical despite different names*

### Comparing `dekpkglock-0.1.8/dekpkglock/resources/pdm/dekspider/project/0.1.46/pdm.lock` & `dekpkglock-0.1.9/dekpkglock/resources/pdm/dekspider/project/0.1.46/pdm.lock`

 * *Files identical despite different names*

### Comparing `dekpkglock-0.1.8/dekpkglock/resources/pdm/dekspider/project/0.1.47/pdm.lock` & `dekpkglock-0.1.9/dekpkglock/resources/pdm/dekspider/project/0.1.47/pdm.lock`

 * *Files identical despite different names*

### Comparing `dekpkglock-0.1.8/dekpkglock/resources/pdm/dekspider/project/0.1.48/pdm.lock` & `dekpkglock-0.1.9/dekpkglock/resources/pdm/dekspider/project/0.1.48/pdm.lock`

 * *Files identical despite different names*

### Comparing `dekpkglock-0.1.8/dekpkglock/resources/pdm/dekspider/project/0.1.49/pdm.lock` & `dekpkglock-0.1.9/dekpkglock/resources/pdm/dekspider/project/0.1.49/pdm.lock`

 * *Files identical despite different names*

### Comparing `dekpkglock-0.1.8/dekpkglock/resources/pdm/dekspider/project/0.1.50/pdm.lock` & `dekpkglock-0.1.9/dekpkglock/resources/pdm/dekspider/project/0.1.50/pdm.lock`

 * *Files identical despite different names*

### Comparing `dekpkglock-0.1.8/dekpkglock/resources/pdm/djcreator/project/0.1.47/pdm.lock` & `dekpkglock-0.1.9/dekpkglock/resources/pdm/djcreator/project/0.1.47/pdm.lock`

 * *Files identical despite different names*

### Comparing `dekpkglock-0.1.8/dekpkglock/resources/pdm/djcreator/wrapper/0.1.47/pdm.lock` & `dekpkglock-0.1.9/dekpkglock/resources/pdm/djcreator/wrapper/0.1.47/pdm.lock`

 * *Files identical despite different names*

