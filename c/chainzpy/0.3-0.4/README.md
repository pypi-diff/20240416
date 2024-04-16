# Comparing `tmp/Chainzpy-0.3.tar.gz` & `tmp/chainzpy-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Chainzpy-0.3.tar", last modified: Sun Apr 14 17:22:03 2024, max compression
+gzip compressed data, was "chainzpy-0.4.tar", last modified: Tue Apr 16 20:27:19 2024, max compression
```

## Comparing `Chainzpy-0.3.tar` & `chainzpy-0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 alexanderwilkerson   (501) staff       (20)        0 2024-04-14 17:22:03.638500 Chainzpy-0.3/
-drwxr-xr-x   0 alexanderwilkerson   (501) staff       (20)        0 2024-04-14 17:22:03.636335 Chainzpy-0.3/Chainzpy/
--rw-r--r--   0 alexanderwilkerson   (501) staff       (20)      328 2024-04-14 17:14:47.000000 Chainzpy-0.3/Chainzpy/__init__.py
--rw-r--r--   0 alexanderwilkerson   (501) staff       (20)     3440 2024-04-14 17:15:15.000000 Chainzpy-0.3/Chainzpy/main.py
-drwxr-xr-x   0 alexanderwilkerson   (501) staff       (20)        0 2024-04-14 17:22:03.637786 Chainzpy-0.3/Chainzpy.egg-info/
--rw-r--r--   0 alexanderwilkerson   (501) staff       (20)      251 2024-04-14 17:22:03.000000 Chainzpy-0.3/Chainzpy.egg-info/PKG-INFO
--rw-r--r--   0 alexanderwilkerson   (501) staff       (20)      215 2024-04-14 17:22:03.000000 Chainzpy-0.3/Chainzpy.egg-info/SOURCES.txt
--rw-r--r--   0 alexanderwilkerson   (501) staff       (20)        1 2024-04-14 17:22:03.000000 Chainzpy-0.3/Chainzpy.egg-info/dependency_links.txt
--rw-r--r--   0 alexanderwilkerson   (501) staff       (20)       13 2024-04-14 17:22:03.000000 Chainzpy-0.3/Chainzpy.egg-info/requires.txt
--rw-r--r--   0 alexanderwilkerson   (501) staff       (20)        9 2024-04-14 17:22:03.000000 Chainzpy-0.3/Chainzpy.egg-info/top_level.txt
--rw-r--r--   0 alexanderwilkerson   (501) staff       (20)      251 2024-04-14 17:22:03.638103 Chainzpy-0.3/PKG-INFO
--rw-r--r--   0 alexanderwilkerson   (501) staff       (20)        0 2024-04-14 07:29:26.000000 Chainzpy-0.3/README.md
--rw-r--r--   0 alexanderwilkerson   (501) staff       (20)       38 2024-04-14 17:22:03.638583 Chainzpy-0.3/setup.cfg
--rw-r--r--   0 alexanderwilkerson   (501) staff       (20)      377 2024-04-14 17:22:01.000000 Chainzpy-0.3/setup.py
+drwxr-xr-x   0 alexanderwilkerson   (501) staff       (20)        0 2024-04-16 20:27:19.024042 chainzpy-0.4/
+drwxr-xr-x   0 alexanderwilkerson   (501) staff       (20)        0 2024-04-16 20:27:19.019750 chainzpy-0.4/Chainzpy/
+-rw-r--r--   0 alexanderwilkerson   (501) staff       (20)      328 2024-04-14 17:14:47.000000 chainzpy-0.4/Chainzpy/__init__.py
+-rw-r--r--   0 alexanderwilkerson   (501) staff       (20)     3440 2024-04-14 17:15:15.000000 chainzpy-0.4/Chainzpy/main.py
+drwxr-xr-x   0 alexanderwilkerson   (501) staff       (20)        0 2024-04-16 20:27:19.023168 chainzpy-0.4/Chainzpy.egg-info/
+-rw-r--r--   0 alexanderwilkerson   (501) staff       (20)      251 2024-04-16 20:27:18.000000 chainzpy-0.4/Chainzpy.egg-info/PKG-INFO
+-rw-r--r--   0 alexanderwilkerson   (501) staff       (20)      412 2024-04-16 20:27:18.000000 chainzpy-0.4/Chainzpy.egg-info/SOURCES.txt
+-rw-r--r--   0 alexanderwilkerson   (501) staff       (20)        1 2024-04-16 20:27:18.000000 chainzpy-0.4/Chainzpy.egg-info/dependency_links.txt
+-rw-r--r--   0 alexanderwilkerson   (501) staff       (20)       13 2024-04-16 20:27:18.000000 chainzpy-0.4/Chainzpy.egg-info/requires.txt
+-rw-r--r--   0 alexanderwilkerson   (501) staff       (20)        9 2024-04-16 20:27:18.000000 chainzpy-0.4/Chainzpy.egg-info/top_level.txt
+-rw-r--r--   0 alexanderwilkerson   (501) staff       (20)      251 2024-04-16 20:27:19.023511 chainzpy-0.4/PKG-INFO
+-rw-r--r--   0 alexanderwilkerson   (501) staff       (20)        0 2024-04-14 07:29:26.000000 chainzpy-0.4/README.md
+-rw-r--r--   0 alexanderwilkerson   (501) staff       (20)       38 2024-04-16 20:27:19.024146 chainzpy-0.4/setup.cfg
+-rw-r--r--   0 alexanderwilkerson   (501) staff       (20)      377 2024-04-16 20:27:16.000000 chainzpy-0.4/setup.py
```

### Comparing `Chainzpy-0.3/Chainzpy/main.py` & `chainzpy-0.4/Chainzpy/main.py`

 * *Files identical despite different names*

