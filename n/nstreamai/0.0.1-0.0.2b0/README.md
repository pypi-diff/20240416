# Comparing `tmp/nstreamai-0.0.1.tar.gz` & `tmp/nstreamai-0.0.2b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nstreamai-0.0.1.tar", last modified: Sat Apr  6 20:05:26 2024, max compression
+gzip compressed data, was "nstreamai-0.0.2b0.tar", last modified: Tue Apr 16 13:13:55 2024, max compression
```

## Comparing `nstreamai-0.0.1.tar` & `nstreamai-0.0.2b0.tar`

### file list

```diff
@@ -1,15 +1,31 @@
-drwxr-xr-x   0 shiv       (501) staff       (20)        0 2024-04-06 20:05:26.644241 nstreamai-0.0.1/
--rw-r--r--   0 shiv       (501) staff       (20)    35149 2024-04-06 19:47:11.000000 nstreamai-0.0.1/LICENSE
--rw-r--r--   0 shiv       (501) staff       (20)      550 2024-04-06 20:05:26.644011 nstreamai-0.0.1/PKG-INFO
--rw-r--r--   0 shiv       (501) staff       (20)       15 2024-04-06 19:47:11.000000 nstreamai-0.0.1/README.md
--rw-r--r--   0 shiv       (501) staff       (20)      608 2024-04-06 20:05:22.000000 nstreamai-0.0.1/pyproject.toml
--rw-r--r--   0 shiv       (501) staff       (20)       38 2024-04-06 20:05:26.644319 nstreamai-0.0.1/setup.cfg
-drwxr-xr-x   0 shiv       (501) staff       (20)        0 2024-04-06 20:05:26.642208 nstreamai-0.0.1/src/
-drwxr-xr-x   0 shiv       (501) staff       (20)        0 2024-04-06 20:05:26.643788 nstreamai-0.0.1/src/nstreamai.egg-info/
--rw-r--r--   0 shiv       (501) staff       (20)      550 2024-04-06 20:05:26.000000 nstreamai-0.0.1/src/nstreamai.egg-info/PKG-INFO
--rw-r--r--   0 shiv       (501) staff       (20)      250 2024-04-06 20:05:26.000000 nstreamai-0.0.1/src/nstreamai.egg-info/SOURCES.txt
--rw-r--r--   0 shiv       (501) staff       (20)        1 2024-04-06 20:05:26.000000 nstreamai-0.0.1/src/nstreamai.egg-info/dependency_links.txt
--rw-r--r--   0 shiv       (501) staff       (20)       21 2024-04-06 20:05:26.000000 nstreamai-0.0.1/src/nstreamai.egg-info/top_level.txt
-drwxr-xr-x   0 shiv       (501) staff       (20)        0 2024-04-06 20:05:26.643415 nstreamai-0.0.1/src/nstreamai_nstream_ai/
--rw-r--r--   0 shiv       (501) staff       (20)      257 2024-04-06 20:04:29.000000 nstreamai-0.0.1/src/nstreamai_nstream_ai/__init__.py
--rw-r--r--   0 shiv       (501) staff       (20)     3105 2024-04-06 20:03:26.000000 nstreamai-0.0.1/src/nstreamai_nstream_ai/main.py
+drwxr-xr-x   0 shiv       (501) staff       (20)        0 2024-04-16 13:13:55.056631 nstreamai-0.0.2b0/
+-rw-r--r--   0 shiv       (501) staff       (20)    35149 2024-04-16 12:23:16.000000 nstreamai-0.0.2b0/LICENSE
+-rw-r--r--   0 shiv       (501) staff       (20)    15552 2024-04-16 13:13:55.056160 nstreamai-0.0.2b0/PKG-INFO
+-rw-r--r--   0 shiv       (501) staff       (20)    15009 2024-04-16 13:03:42.000000 nstreamai-0.0.2b0/README.md
+-rw-r--r--   0 shiv       (501) staff       (20)      676 2024-04-16 13:13:51.000000 nstreamai-0.0.2b0/pyproject.toml
+-rw-r--r--   0 shiv       (501) staff       (20)       38 2024-04-16 13:13:55.056681 nstreamai-0.0.2b0/setup.cfg
+drwxr-xr-x   0 shiv       (501) staff       (20)        0 2024-04-16 13:13:55.049414 nstreamai-0.0.2b0/src/
+drwxr-xr-x   0 shiv       (501) staff       (20)        0 2024-04-16 13:13:55.055849 nstreamai-0.0.2b0/src/nstreamai.egg-info/
+-rw-r--r--   0 shiv       (501) staff       (20)    15552 2024-04-16 13:13:55.000000 nstreamai-0.0.2b0/src/nstreamai.egg-info/PKG-INFO
+-rw-r--r--   0 shiv       (501) staff       (20)      829 2024-04-16 13:13:55.000000 nstreamai-0.0.2b0/src/nstreamai.egg-info/SOURCES.txt
+-rw-r--r--   0 shiv       (501) staff       (20)        1 2024-04-16 13:13:55.000000 nstreamai-0.0.2b0/src/nstreamai.egg-info/dependency_links.txt
+-rw-r--r--   0 shiv       (501) staff       (20)       28 2024-04-16 13:13:55.000000 nstreamai-0.0.2b0/src/nstreamai.egg-info/top_level.txt
+drwxr-xr-x   0 shiv       (501) staff       (20)        0 2024-04-16 13:13:55.051933 nstreamai-0.0.2b0/src/nstreamai_nstream_ai/
+-rw-r--r--   0 shiv       (501) staff       (20)       71 2024-04-08 20:31:13.000000 nstreamai-0.0.2b0/src/nstreamai_nstream_ai/__init__.py
+drwxr-xr-x   0 shiv       (501) staff       (20)        0 2024-04-16 13:13:55.054176 nstreamai-0.0.2b0/src/nstreamai_nstream_ai/core/
+-rw-r--r--   0 shiv       (501) staff       (20)     4478 2024-04-16 12:19:23.000000 nstreamai-0.0.2b0/src/nstreamai_nstream_ai/core/nsgraph.py
+-rw-r--r--   0 shiv       (501) staff       (20)     3920 2024-04-16 12:59:38.000000 nstreamai-0.0.2b0/src/nstreamai_nstream_ai/core/nsinit.py
+-rw-r--r--   0 shiv       (501) staff       (20)      679 2024-04-16 12:19:23.000000 nstreamai-0.0.2b0/src/nstreamai_nstream_ai/core/nsneuron.py
+-rw-r--r--   0 shiv       (501) staff       (20)     6961 2024-04-16 12:19:23.000000 nstreamai-0.0.2b0/src/nstreamai_nstream_ai/core/nsnode.py
+drwxr-xr-x   0 shiv       (501) staff       (20)        0 2024-04-16 13:13:55.054592 nstreamai-0.0.2b0/src/nstreamai_nstream_ai/examples/
+-rw-r--r--   0 shiv       (501) staff       (20)     1787 2024-04-16 12:24:03.000000 nstreamai-0.0.2b0/src/nstreamai_nstream_ai/examples/main_context_transfom.py
+-rw-r--r--   0 shiv       (501) staff       (20)     2141 2024-04-16 12:19:23.000000 nstreamai-0.0.2b0/src/nstreamai_nstream_ai/examples/main_prompt.py
+-rw-r--r--   0 shiv       (501) staff       (20)     3531 2024-04-16 12:25:10.000000 nstreamai-0.0.2b0/src/nstreamai_nstream_ai/examples/main_rag_advance.py
+-rw-r--r--   0 shiv       (501) staff       (20)     3531 2024-04-16 12:19:23.000000 nstreamai-0.0.2b0/src/nstreamai_nstream_ai/main.py
+drwxr-xr-x   0 shiv       (501) staff       (20)        0 2024-04-16 13:13:55.055638 nstreamai-0.0.2b0/src/nstreamai_nstream_ai/utils/
+-rw-r--r--   0 shiv       (501) staff       (20)     1890 2024-04-16 12:19:23.000000 nstreamai-0.0.2b0/src/nstreamai_nstream_ai/utils/logger.py
+-rw-r--r--   0 shiv       (501) staff       (20)      531 2024-04-16 12:19:23.000000 nstreamai-0.0.2b0/src/nstreamai_nstream_ai/utils/output_data.py
+-rw-r--r--   0 shiv       (501) staff       (20)     5542 2024-04-09 11:56:26.000000 nstreamai-0.0.2b0/src/nstreamai_nstream_ai/utils/run.py
+-rw-r--r--   0 shiv       (501) staff       (20)     6263 2024-04-16 12:19:23.000000 nstreamai-0.0.2b0/src/nstreamai_nstream_ai/utils/template.py
+-rw-r--r--   0 shiv       (501) staff       (20)     1182 2024-04-09 11:56:26.000000 nstreamai-0.0.2b0/src/nstreamai_nstream_ai/utils/variables.py
+-rw-r--r--   0 shiv       (501) staff       (20)     1191 2024-04-09 11:56:26.000000 nstreamai-0.0.2b0/src/nstreamai_nstream_ai/utils/welcome.py
```

### Comparing `nstreamai-0.0.1/LICENSE` & `nstreamai-0.0.2b0/LICENSE`

 * *Files identical despite different names*

### Comparing `nstreamai-0.0.1/pyproject.toml` & `nstreamai-0.0.2b0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
-requires = ["setuptools>=61.0"]
+requires = ["setuptools>=61.0", "httpx>=0.27.0", "pyfiglet>=1.0.2", "termcolor>=2.4.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nstreamai"
-version = "0.0.1"
+version = "0.0.2-beta"
 authors = [
-  { name = "Shiv", email = "shiv@nstream.ai" },
+  { name = "Nstream AI", email = "hello@nstream.ai" },
 ]
 description = "Official SDK for nstream ai stream processing powered by Gen AI"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

