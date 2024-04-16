# Comparing `tmp/langchain_iris-0.1.2b1.tar.gz` & `tmp/langchain_iris-0.1.2b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_iris-0.1.2b1.tar", last modified: Tue Apr 16 10:13:55 2024, max compression
+gzip compressed data, was "langchain_iris-0.1.2b2.tar", last modified: Tue Apr 16 10:21:47 2024, max compression
```

## Comparing `langchain_iris-0.1.2b1.tar` & `langchain_iris-0.1.2b2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:13:55.412489 langchain_iris-0.1.2b1/
--rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-04-16 10:13:55.412489 langchain_iris-0.1.2b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-16 10:13:37.000000 langchain_iris-0.1.2b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:13:55.412489 langchain_iris-0.1.2b1/langchain_iris/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-16 10:13:37.000000 langchain_iris-0.1.2b1/langchain_iris/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20035 2024-04-16 10:13:37.000000 langchain_iris-0.1.2b1/langchain_iris/vectorstores.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:13:55.412489 langchain_iris-0.1.2b1/langchain_iris.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-04-16 10:13:55.000000 langchain_iris-0.1.2b1/langchain_iris.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-16 10:13:55.000000 langchain_iris-0.1.2b1/langchain_iris.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 10:13:55.000000 langchain_iris-0.1.2b1/langchain_iris.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-16 10:13:55.000000 langchain_iris-0.1.2b1/langchain_iris.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-16 10:13:55.000000 langchain_iris-0.1.2b1/langchain_iris.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-16 10:13:55.412489 langchain_iris-0.1.2b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-16 10:13:37.000000 langchain_iris-0.1.2b1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:13:55.412489 langchain_iris-0.1.2b1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    10436 2024-04-16 10:13:37.000000 langchain_iris-0.1.2b1/tests/test_vectorstores.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:21:47.012828 langchain_iris-0.1.2b2/
+-rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-04-16 10:21:47.012828 langchain_iris-0.1.2b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-16 10:21:24.000000 langchain_iris-0.1.2b2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:21:47.012828 langchain_iris-0.1.2b2/langchain_iris/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-16 10:21:24.000000 langchain_iris-0.1.2b2/langchain_iris/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19669 2024-04-16 10:21:24.000000 langchain_iris-0.1.2b2/langchain_iris/vectorstores.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:21:47.012828 langchain_iris-0.1.2b2/langchain_iris.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-04-16 10:21:47.000000 langchain_iris-0.1.2b2/langchain_iris.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-16 10:21:47.000000 langchain_iris-0.1.2b2/langchain_iris.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 10:21:47.000000 langchain_iris-0.1.2b2/langchain_iris.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-16 10:21:47.000000 langchain_iris-0.1.2b2/langchain_iris.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-16 10:21:47.000000 langchain_iris-0.1.2b2/langchain_iris.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-16 10:21:47.012828 langchain_iris-0.1.2b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-16 10:21:24.000000 langchain_iris-0.1.2b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:21:47.012828 langchain_iris-0.1.2b2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    10436 2024-04-16 10:21:24.000000 langchain_iris-0.1.2b2/tests/test_vectorstores.py
```

### Comparing `langchain_iris-0.1.2b1/PKG-INFO` & `langchain_iris-0.1.2b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-iris
-Version: 0.1.2b1
+Version: 0.1.2b2
 Summary: The InterSystems IRIS adoption for Langchain
 Home-page: https://github.com/caretdev/langchain-iris
 Project-URL: Source, https://github.com/caretdev/langchain-iris
 Project-URL: Tracker, https://github.com/caretdev/langchain-iris/issues
 Keywords: "InterSystems IRIS"
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `langchain_iris-0.1.2b1/README.md` & `langchain_iris-0.1.2b2/README.md`

 * *Files identical despite different names*

### Comparing `langchain_iris-0.1.2b1/langchain_iris/vectorstores.py` & `langchain_iris-0.1.2b2/langchain_iris/vectorstores.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,47 +1,40 @@
 from __future__ import annotations
 
 import contextlib
 import json
 import enum
 import logging
 import uuid
-from functools import partial
 from typing import (
-    TYPE_CHECKING,
     Any,
     Callable,
     Dict,
     Sequence,
     Generator,
     Iterable,
     List,
     Optional,
     Tuple,
     Type,
 )
 
-import numpy as np
 from sqlalchemy import (
     Connection,
     and_,
     asc,
-    literal,
     VARCHAR,
-    UUID,
     TEXT,
     Column,
-    String,
     Table,
     create_engine,
     insert,
     text,
     delete,
     Row,
-    func,
 )
 from sqlalchemy_iris import IRISListBuild
 from sqlalchemy_iris import IRISVector as IRISVectorType
 
 from sqlalchemy.orm import Session
 
 try:
@@ -49,39 +42,35 @@
 except ImportError:
     from sqlalchemy.ext.declarative import declarative_base
 
 from langchain_core.documents import Document
 from langchain_core.embeddings import Embeddings
 from langchain_core.vectorstores import VectorStore
 
-from langchain.utils import get_from_dict_or_env
-from langchain.vectorstores.utils import maximal_marginal_relevance
-
 Base = declarative_base()  # type: Any
 
 
 class DistanceStrategy(str, enum.Enum):
     """Enumerator of the Distance strategies."""
 
     EUCLIDEAN = "l2"
     COSINE = "cosine"
-    MAX_INNER_PRODUCT = "inner"
+    DOT_PRODUCT = "dot"
 
 
 DEFAULT_DISTANCE_STRATEGY = DistanceStrategy.COSINE
 
 _LANGCHAIN_DEFAULT_COLLECTION_NAME = "langchain"
 
 Base = declarative_base()
 
 
 class IRISVector(VectorStore):
     _conn = None
     native_vector = False
-    native_vector_cosine_similarity = False
 
     def __init__(
         self,
         embedding_function: Embeddings,
         dimension: int = None,
         connection_string: Optional[str] = None,
         collection_name: str = _LANGCHAIN_DEFAULT_COLLECTION_NAME,
@@ -197,45 +186,42 @@
             raise Exception(f"Failed to create vector functions: {e}") from e
 
     @property
     def distance_strategy(self) -> str:
         if self.native_vector:
             if self._distance_strategy == DistanceStrategy.COSINE:
                 return self.table.c.embedding.cosine
-            elif self._distance_strategy == DistanceStrategy.MAX_INNER_PRODUCT:
-                return self.table.c.embedding.max_inner_product
+            elif self._distance_strategy == DistanceStrategy.DOT_PRODUCT:
+                return self.table.c.embedding.DOT_product
             # elif self._distance_strategy == DistanceStrategy.EUCLIDEAN:
             #     return "langchain_l2_distance"
             else:
                 raise ValueError(
                     f"Got unexpected value for distance: {self._distance_strategy}. "
                     f"Should be one of {', '.join([ds.value for ds in DistanceStrategy])}."
                 )
 
         if self._distance_strategy == DistanceStrategy.EUCLIDEAN:
             return "langchain_l2_distance"
         elif self._distance_strategy == DistanceStrategy.COSINE:
             return "langchain_cosine_distance"
-        elif self._distance_strategy == DistanceStrategy.MAX_INNER_PRODUCT:
+        elif self._distance_strategy == DistanceStrategy.DOT_PRODUCT:
             return "langchain_inner_distance"
         else:
             raise ValueError(
                 f"Got unexpected value for distance: {self._distance_strategy}. "
                 f"Should be one of {', '.join([ds.value for ds in DistanceStrategy])}."
             )
 
     def connect(self) -> Connection:
         engine = create_engine(self.connection_string, **self.engine_args)
         conn = engine.connect()
         try:
             if conn.dialect.supports_vectors:
                 self.native_vector = True
-                self.native_vector_cosine_similarity = (
-                    conn.dialect.vector_cosine_similarity
-                )
         except:  # noqa
             pass
         return conn
 
     def __del__(self) -> None:
         if self._conn:
             self._conn.close()
@@ -303,16 +289,16 @@
 
         # Default strategy is to rely on distance strategy provided
         # in vectorstore constructor
         if self._distance_strategy == DistanceStrategy.COSINE:
             return self._cosine_relevance_score_fn
         elif self._distance_strategy == DistanceStrategy.EUCLIDEAN:
             return self._euclidean_relevance_score_fn
-        elif self._distance_strategy == DistanceStrategy.MAX_INNER_PRODUCT:
-            return self._max_inner_product_relevance_score_fn
+        elif self._distance_strategy == DistanceStrategy.DOT_PRODUCT:
+            return self._DOT_product_relevance_score_fn
         else:
             raise ValueError(
                 "No supported normalization function"
                 f" for distance_strategy of {self._distance_strategy}."
                 "Consider providing relevance_score_fn to IRISVector constructor."
             )
 
@@ -546,15 +532,19 @@
 
         documents_with_scores = [
             (
                 Document(
                     page_content=result.document,
                     metadata=json.loads(result.metadata),
                 ),
-                round(float(result.distance), 15) if self.embedding_function is not None else None,
+                (
+                    round(float(result.distance), 15)
+                    if self.embedding_function is not None
+                    else None
+                ),
             )
             for result in results
         ]
         return documents_with_scores
 
     def similarity_search_by_vector(
         self,
```

### Comparing `langchain_iris-0.1.2b1/langchain_iris.egg-info/PKG-INFO` & `langchain_iris-0.1.2b2/langchain_iris.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-iris
-Version: 0.1.2b1
+Version: 0.1.2b2
 Summary: The InterSystems IRIS adoption for Langchain
 Home-page: https://github.com/caretdev/langchain-iris
 Project-URL: Source, https://github.com/caretdev/langchain-iris
 Project-URL: Tracker, https://github.com/caretdev/langchain-iris/issues
 Keywords: "InterSystems IRIS"
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `langchain_iris-0.1.2b1/setup.cfg` & `langchain_iris-0.1.2b2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = langchain-iris
-version = 0.1.2b1
+version = 0.1.2b2
 description = The InterSystems IRIS adoption for Langchain
 long_description = file: README.md
 url = https://github.com/caretdev/langchain-iris
 long_description_content_type = text/markdown
 classifiers = 
 	Development Status :: 3 - Alpha
 	Intended Audience :: Developers
```

### Comparing `langchain_iris-0.1.2b1/tests/test_vectorstores.py` & `langchain_iris-0.1.2b2/tests/test_vectorstores.py`

 * *Files identical despite different names*

