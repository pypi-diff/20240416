# Comparing `tmp/llama_iris-0.3.1b2.tar.gz` & `tmp/llama_iris-0.3.1b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_iris-0.3.1b2.tar", max compression
+gzip compressed data, was "llama_iris-0.3.1b3.tar", max compression
```

## Comparing `llama_iris-0.3.1b2.tar` & `llama_iris-0.3.1b3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1086 2024-02-16 18:20:46.355103 llama_iris-0.3.1b2/LICENSE
--rw-r--r--   0        0        0      128 2024-02-16 18:20:46.355103 llama_iris-0.3.1b2/README.md
--rw-r--r--   0        0        0      224 2024-02-16 18:20:46.355103 llama_iris-0.3.1b2/llama_iris/__init__.py
--rw-r--r--   0        0        0    10160 2024-02-16 18:20:46.355103 llama_iris-0.3.1b2/llama_iris/vectorstore.py
--rw-r--r--   0        0        0     1060 2024-02-16 18:21:00.079054 llama_iris-0.3.1b2/pyproject.toml
--rw-r--r--   0        0        0     1253 1970-01-01 00:00:00.000000 llama_iris-0.3.1b2/PKG-INFO
+-rw-r--r--   0        0        0     1086 2024-04-16 10:57:03.085854 llama_iris-0.3.1b3/LICENSE
+-rw-r--r--   0        0        0     1108 2024-04-16 10:57:03.085854 llama_iris-0.3.1b3/README.md
+-rw-r--r--   0        0        0      224 2024-04-16 10:57:03.085854 llama_iris-0.3.1b3/llama_iris/__init__.py
+-rw-r--r--   0        0        0    10160 2024-04-16 10:57:03.085854 llama_iris-0.3.1b3/llama_iris/vectorstore.py
+-rw-r--r--   0        0        0     1060 2024-04-16 10:57:16.357998 llama_iris-0.3.1b3/pyproject.toml
+-rw-r--r--   0        0        0     2233 1970-01-01 00:00:00.000000 llama_iris-0.3.1b3/PKG-INFO
```

### Comparing `llama_iris-0.3.1b2/LICENSE` & `llama_iris-0.3.1b3/LICENSE`

 * *Files identical despite different names*

### Comparing `llama_iris-0.3.1b2/llama_iris/vectorstore.py` & `llama_iris-0.3.1b3/llama_iris/vectorstore.py`

 * *Files identical despite different names*

### Comparing `llama_iris-0.3.1b2/pyproject.toml` & `llama_iris-0.3.1b3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [tool.poetry]
 name = "llama-iris"
 classifiers = [
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Topic :: Software Development :: Libraries :: Application Frameworks",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
-version = "0.3.1b2"
+version = "0.3.1b3"
 description = "Interface between LLMs and your data"
 authors = ["Dmitry Maslennikov <dmitry@caretdev.com>"]
 keywords = ["LLM", "NLP", "RAG", "data", "devtools", "index", "retrieval", "iris"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "llama_iris"}]
 repository = "https://github.com/caretdev/llama-iris"
```

