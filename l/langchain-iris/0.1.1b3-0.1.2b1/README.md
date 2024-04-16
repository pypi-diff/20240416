# Comparing `tmp/langchain-iris-0.1.1b3.tar.gz` & `tmp/langchain_iris-0.1.2b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain-iris-0.1.1b3.tar", last modified: Fri Feb 16 19:58:43 2024, max compression
+gzip compressed data, was "langchain_iris-0.1.2b1.tar", last modified: Tue Apr 16 10:13:55 2024, max compression
```

## Comparing `langchain-iris-0.1.1b3.tar` & `langchain_iris-0.1.2b1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 19:58:43.343123 langchain-iris-0.1.1b3/
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-02-16 19:58:43.343123 langchain-iris-0.1.1b3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-02-16 19:58:19.000000 langchain-iris-0.1.1b3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 19:58:43.339123 langchain-iris-0.1.1b3/langchain_iris/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-02-16 19:58:19.000000 langchain-iris-0.1.1b3/langchain_iris/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20035 2024-02-16 19:58:19.000000 langchain-iris-0.1.1b3/langchain_iris/vectorstores.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 19:58:43.343123 langchain-iris-0.1.1b3/langchain_iris.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-02-16 19:58:43.000000 langchain-iris-0.1.1b3/langchain_iris.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-02-16 19:58:43.000000 langchain-iris-0.1.1b3/langchain_iris.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-16 19:58:43.000000 langchain-iris-0.1.1b3/langchain_iris.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-02-16 19:58:43.000000 langchain-iris-0.1.1b3/langchain_iris.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-16 19:58:43.000000 langchain-iris-0.1.1b3/langchain_iris.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-02-16 19:58:43.343123 langchain-iris-0.1.1b3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-02-16 19:58:19.000000 langchain-iris-0.1.1b3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 19:58:43.343123 langchain-iris-0.1.1b3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    10436 2024-02-16 19:58:19.000000 langchain-iris-0.1.1b3/tests/test_vectorstores.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:13:55.412489 langchain_iris-0.1.2b1/
+-rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-04-16 10:13:55.412489 langchain_iris-0.1.2b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-16 10:13:37.000000 langchain_iris-0.1.2b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:13:55.412489 langchain_iris-0.1.2b1/langchain_iris/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-16 10:13:37.000000 langchain_iris-0.1.2b1/langchain_iris/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20035 2024-04-16 10:13:37.000000 langchain_iris-0.1.2b1/langchain_iris/vectorstores.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:13:55.412489 langchain_iris-0.1.2b1/langchain_iris.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-04-16 10:13:55.000000 langchain_iris-0.1.2b1/langchain_iris.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-16 10:13:55.000000 langchain_iris-0.1.2b1/langchain_iris.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 10:13:55.000000 langchain_iris-0.1.2b1/langchain_iris.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-16 10:13:55.000000 langchain_iris-0.1.2b1/langchain_iris.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-16 10:13:55.000000 langchain_iris-0.1.2b1/langchain_iris.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-16 10:13:55.412489 langchain_iris-0.1.2b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-16 10:13:37.000000 langchain_iris-0.1.2b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:13:55.412489 langchain_iris-0.1.2b1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    10436 2024-04-16 10:13:37.000000 langchain_iris-0.1.2b1/tests/test_vectorstores.py
```

### Comparing `langchain-iris-0.1.1b3/langchain_iris/vectorstores.py` & `langchain_iris-0.1.2b1/langchain_iris/vectorstores.py`

 * *Files identical despite different names*

### Comparing `langchain-iris-0.1.1b3/setup.cfg` & `langchain_iris-0.1.2b1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = langchain-iris
-version = 0.1.1b3
+version = 0.1.2b1
 description = The InterSystems IRIS adoption for Langchain
 long_description = file: README.md
 url = https://github.com/caretdev/langchain-iris
 long_description_content_type = text/markdown
 classifiers = 
 	Development Status :: 3 - Alpha
 	Intended Audience :: Developers
```

### Comparing `langchain-iris-0.1.1b3/tests/test_vectorstores.py` & `langchain_iris-0.1.2b1/tests/test_vectorstores.py`

 * *Files identical despite different names*

