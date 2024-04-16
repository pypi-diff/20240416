# Comparing `tmp/yeabm25-0.1.2.tar.gz` & `tmp/yeabm25-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeabm25-0.1.2.tar", last modified: Fri Apr  5 10:10:54 2024, max compression
+gzip compressed data, was "yeabm25-0.1.3.tar", last modified: Tue Apr 16 19:02:20 2024, max compression
```

## Comparing `yeabm25-0.1.2.tar` & `yeabm25-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 10:10:54.326377 yeabm25-0.1.2/
--rw-rw-rw-   0        0        0    11558 2024-03-24 19:44:05.000000 yeabm25-0.1.2/LICENSE
--rw-rw-rw-   0        0        0    16841 2024-04-05 10:10:54.326377 yeabm25-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     3057 2024-04-02 16:49:16.000000 yeabm25-0.1.2/README.md
--rw-rw-rw-   0        0        0      848 2024-04-05 10:10:14.000000 yeabm25-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-05 10:10:54.326377 yeabm25-0.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-05 10:10:54.295130 yeabm25-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2024-04-05 10:10:54.310752 yeabm25-0.1.2/src/yeabm25/
--rw-rw-rw-   0        0        0       39 2024-03-23 17:47:15.000000 yeabm25-0.1.2/src/yeabm25/__init__.py
--rw-rw-rw-   0        0        0    11440 2024-04-03 19:45:20.000000 yeabm25-0.1.2/src/yeabm25/bm25.py
-drwxrwxrwx   0        0        0        0 2024-04-05 10:10:54.326377 yeabm25-0.1.2/src/yeabm25.egg-info/
--rw-rw-rw-   0        0        0    16841 2024-04-05 10:10:54.000000 yeabm25-0.1.2/src/yeabm25.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      272 2024-04-05 10:10:54.000000 yeabm25-0.1.2/src/yeabm25.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 10:10:54.000000 yeabm25-0.1.2/src/yeabm25.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2024-04-05 10:10:54.000000 yeabm25-0.1.2/src/yeabm25.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-05 10:10:54.000000 yeabm25-0.1.2/src/yeabm25.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-05 10:10:54.326377 yeabm25-0.1.2/tests/
--rw-rw-rw-   0        0        0     1806 2024-03-31 15:19:12.000000 yeabm25-0.1.2/tests/test_yeabm25.py
+drwxrwxrwx   0        0        0        0 2024-04-16 19:02:20.810759 yeabm25-0.1.3/
+-rw-rw-rw-   0        0        0    11558 2024-03-24 19:44:05.000000 yeabm25-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0    17302 2024-04-16 19:02:20.808759 yeabm25-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3518 2024-04-11 16:21:24.000000 yeabm25-0.1.3/README.md
+-rw-rw-rw-   0        0        0      848 2024-04-16 18:50:44.000000 yeabm25-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-16 19:02:20.810759 yeabm25-0.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-16 19:02:20.773476 yeabm25-0.1.3/src/
+drwxrwxrwx   0        0        0        0 2024-04-16 19:02:20.779760 yeabm25-0.1.3/src/yeabm25/
+-rw-rw-rw-   0        0        0       39 2024-03-23 17:47:15.000000 yeabm25-0.1.3/src/yeabm25/__init__.py
+-rw-rw-rw-   0        0        0    12133 2024-04-16 18:47:47.000000 yeabm25-0.1.3/src/yeabm25/bm25.py
+drwxrwxrwx   0        0        0        0 2024-04-16 19:02:20.806759 yeabm25-0.1.3/src/yeabm25.egg-info/
+-rw-rw-rw-   0        0        0    17302 2024-04-16 19:02:20.000000 yeabm25-0.1.3/src/yeabm25.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2024-04-16 19:02:20.000000 yeabm25-0.1.3/src/yeabm25.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 19:02:20.000000 yeabm25-0.1.3/src/yeabm25.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2024-04-16 19:02:20.000000 yeabm25-0.1.3/src/yeabm25.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-16 19:02:20.000000 yeabm25-0.1.3/src/yeabm25.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-16 19:02:20.805758 yeabm25-0.1.3/tests/
+-rw-rw-rw-   0        0        0     2339 2024-04-16 18:49:39.000000 yeabm25-0.1.3/tests/test_yeabm25.py
```

### Comparing `yeabm25-0.1.2/LICENSE` & `yeabm25-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `yeabm25-0.1.2/PKG-INFO` & `yeabm25-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yeabm25
-Version: 0.1.2
+Version: 0.1.3
 Summary: Yet Another BM25 algorithm implementation with update method, so that you dont need to fit on old + new documents.
 Author-email: Demir Tonchev <{surname}.{name}@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -256,35 +256,41 @@
 ```
 
 This work is inspired(and uses some code and ideas) by this great package - https://github.com/dorianbrown/rank_bm25/tree/master.
 The main focus is creating document and query vectors (supports sparse vectors). Then using the vectors with your favourite Vector DB.
 
 How to get the document and query vectors: 
 ```python
-# recommended approach for large corpus, returns iterator. Each element is list[float]
-# returns generator object
-yeabm.iter_document_vectors()
-# use it 
-for vector in yeabm.iter_document_vectors():
+# recommended approach for large corpus, returns iterator. Each element is sparse vector. 
+# To represent a sparse vector we can use:
+# - Dict[int, float] <--- This is currently the sparse format in YeaBM25
+# - Any of the scipy.sparse sparse matrices class family with shape[0] == 1
+# - Iterable[Tuple[int, float]]
+
+# this method returns generator object
+yeabm.iter_document_vectors() # or
+yeabm.iter_document_vectors_sparse() # <--- recommended for usage with Vector DB
+# use it in loop
+for vector in yeabm.iter_document_vectors_sparse():
     # dostuff could be put in DB. 
     dostuff(vector)
 
 query = ...
 yeabm.encode_query(query)
 ```
 
 Why would you want to do that? Essentially the BM25 score formula is a sum, so it is a perfect candidate for one of the metrics any DB
-supports - inner product.
+supports - **inner product (IP)**.
 ```python
 # 
 bm_index.get_scores(['quick', 'fox'])
 # ~ [1.30, 0.0, 0.72, 0.0, 0.0, 0.0]
 
 # you get the same scores like so:
-yeabm.get_embeddings() @ np.asarray(yeabm.encode_query(['fox', 'quick']))
+yeabm.get_embeddings() @ np.asarray(yeabm.encode_query_dense(['fox', 'quick']))
 # ~ [1.30, 0.0, 0.72, 0.0, 0.0, 0.0]
 ```
 Of course you would like to leave the last calculation to the Vector DB.
 
 One more opinionated implementation is that words that are found in more than half of the corpus would not have idf of 0. It would be small 
 but still positive. For example in other implementations:
 
@@ -295,7 +301,10 @@
 # [0. 0. 0. 0. 0. 0.]
 # where 
 yeabm.get_scores(['brown'])
 #[0.18 0.28 0.33  0. 0. 0.]
 # this is helpful if the user is looking for a term that is abundant in the corpus and would still get somewhat useful results
 # where with BM25Okapi you would get essentially random results (or no results).
 ```
+
+### Usage examples:
+- [Use sparse vectors with Milvus DB](examples/sparse_vector_milvus.ipynb)
```

### Comparing `yeabm25-0.1.2/README.md` & `yeabm25-0.1.3/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -39,35 +39,41 @@
 ```
 
 This work is inspired(and uses some code and ideas) by this great package - https://github.com/dorianbrown/rank_bm25/tree/master.
 The main focus is creating document and query vectors (supports sparse vectors). Then using the vectors with your favourite Vector DB.
 
 How to get the document and query vectors: 
 ```python
-# recommended approach for large corpus, returns iterator. Each element is list[float]
-# returns generator object
-yeabm.iter_document_vectors()
-# use it 
-for vector in yeabm.iter_document_vectors():
+# recommended approach for large corpus, returns iterator. Each element is sparse vector. 
+# To represent a sparse vector we can use:
+# - Dict[int, float] <--- This is currently the sparse format in YeaBM25
+# - Any of the scipy.sparse sparse matrices class family with shape[0] == 1
+# - Iterable[Tuple[int, float]]
+
+# this method returns generator object
+yeabm.iter_document_vectors() # or
+yeabm.iter_document_vectors_sparse() # <--- recommended for usage with Vector DB
+# use it in loop
+for vector in yeabm.iter_document_vectors_sparse():
     # dostuff could be put in DB. 
     dostuff(vector)
 
 query = ...
 yeabm.encode_query(query)
 ```
 
 Why would you want to do that? Essentially the BM25 score formula is a sum, so it is a perfect candidate for one of the metrics any DB
-supports - inner product.
+supports - **inner product (IP)**.
 ```python
 # 
 bm_index.get_scores(['quick', 'fox'])
 # ~ [1.30, 0.0, 0.72, 0.0, 0.0, 0.0]
 
 # you get the same scores like so:
-yeabm.get_embeddings() @ np.asarray(yeabm.encode_query(['fox', 'quick']))
+yeabm.get_embeddings() @ np.asarray(yeabm.encode_query_dense(['fox', 'quick']))
 # ~ [1.30, 0.0, 0.72, 0.0, 0.0, 0.0]
 ```
 Of course you would like to leave the last calculation to the Vector DB.
 
 One more opinionated implementation is that words that are found in more than half of the corpus would not have idf of 0. It would be small 
 but still positive. For example in other implementations:
 
@@ -77,8 +83,11 @@
 okapi.get_scores(['brown']) 
 # [0. 0. 0. 0. 0. 0.]
 # where 
 yeabm.get_scores(['brown'])
 #[0.18 0.28 0.33  0. 0. 0.]
 # this is helpful if the user is looking for a term that is abundant in the corpus and would still get somewhat useful results
 # where with BM25Okapi you would get essentially random results (or no results).
-```
+```
+
+### Usage examples:
+- [Use sparse vectors with Milvus DB](examples/sparse_vector_milvus.ipynb)
```

### Comparing `yeabm25-0.1.2/pyproject.toml` & `yeabm25-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 package-dir = {"" = "src"}
 
 [project]
 name = "yeabm25"
 description = """Yet Another BM25 algorithm implementation with update method, so that you dont need to fit on old + new documents.
 Also you can get document and query vectors to use with any Vector DB."""
 requires-python = ">=3.10"
-version = "0.1.2"
+version = "0.1.3"
 keywords = ["text", "bm25", "dense vector embeddings", "information retrieval", "hybrid search"]
 readme = "README.md"
 dependencies = [
   "numpy>=1.26",
 ]
 authors = [
   {name = "Demir Tonchev", email = "{surname}.{name}@gmail.com"},
```

### Comparing `yeabm25-0.1.2/src/yeabm25/bm25.py` & `yeabm25-0.1.3/src/yeabm25/bm25.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 import math
 from pathlib import Path
 import numpy as np
 from collections import defaultdict, Counter
 from dataclasses import dataclass, field
-from typing import TypeAlias, Optional
+from typing import Literal, TypeAlias, Optional
 
 # type alias just for readability
 Vector1d: TypeAlias = np.ndarray | list[float]
 SparseVector: TypeAlias = dict[int, float]  # #TODO | Iterable[Tuple[int, float]], scipy sparse
 
 # experimental
 # this is created with possible compatibility with haystack>2.0
-
-
 @dataclass
 class BMDocument:
     content: list[str]
     meta: dict = field(default_factory=dict)
     embedding: Optional[Vector1d] = None
 
     def __len__(self):
@@ -251,33 +249,45 @@
         for idx, word in enumerate(self.features_):
             word_freq = np.asarray([doc.get(word, 0) for doc in self.doc_freqs])
             word_vector = self.idf.get(word, 0) * (word_freq * (self.k1 + 1) /
                                                    (word_freq + self.k1 * (1 - self.b + self.b * doc_len / self.avgdl)))
             matrix[:, idx] = word_vector
         return matrix
 
-    def state_dict(self):
-        return {
-            'k1': self.k1,
-            'b': self.b,
-            'epsilon': self.epsilon,
-            'avgdl': self.avgdl,
-            'idf': self.idf,
-        }
+    def state_dict(self, state: Literal['encodeonly', 'full'] = 'encodeonly'):
+        """ Exports the current state
+        Parameters
+        ----------
+        state : Literal['encodeonly', 'full']
+            encodeonly - exports only state that is sufficient for loading later and only encoding new queries.
+            full - exports full state that is suitable for update, encoding of documents and queries.
+        """
+        if state == 'encodeonly':
+            return {
+                'k1': self.k1,
+                'b': self.b,
+                'epsilon': self.epsilon,
+                'idf': self.idf,
+            }
+        elif state == 'full':
+            raise ValueError('option "full" currently is not supported')
+        else:
+            raise ValueError(f'option {state} unknown')
 
     @classmethod
     def from_state_dict(cls, state_dict):
         # ugly but effetive for now
-        bm_index = cls()
-        bm_index.__dict__.update(**state_dict)
-        return bm_index
+        yeabm = cls()
+        yeabm.__dict__.update(**state_dict)
+        yeabm._ftoi()
+        return yeabm
 
-    def serialize(self, fout: Path | str, method: str = 'json', **kwargs):
+    def serialize(self, fout: Path | str, state: Literal['encodeonly', 'full'] = 'encodeonly', method: str = 'json', **kwargs):
         try:
-            _serializers_registry[method](self.state_dict(), fout, **kwargs)
+            _serializers_registry[method](self.state_dict(state=state), fout, **kwargs)
         except KeyError:
             raise
 
     @classmethod
     def deserialize(cls, fin, method: str = 'json'):
         loaded_state_dict = _deserializers_registry[method](fin)
         return cls.from_state_dict(loaded_state_dict)
```

### Comparing `yeabm25-0.1.2/src/yeabm25.egg-info/PKG-INFO` & `yeabm25-0.1.3/src/yeabm25.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yeabm25
-Version: 0.1.2
+Version: 0.1.3
 Summary: Yet Another BM25 algorithm implementation with update method, so that you dont need to fit on old + new documents.
 Author-email: Demir Tonchev <{surname}.{name}@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -256,35 +256,41 @@
 ```
 
 This work is inspired(and uses some code and ideas) by this great package - https://github.com/dorianbrown/rank_bm25/tree/master.
 The main focus is creating document and query vectors (supports sparse vectors). Then using the vectors with your favourite Vector DB.
 
 How to get the document and query vectors: 
 ```python
-# recommended approach for large corpus, returns iterator. Each element is list[float]
-# returns generator object
-yeabm.iter_document_vectors()
-# use it 
-for vector in yeabm.iter_document_vectors():
+# recommended approach for large corpus, returns iterator. Each element is sparse vector. 
+# To represent a sparse vector we can use:
+# - Dict[int, float] <--- This is currently the sparse format in YeaBM25
+# - Any of the scipy.sparse sparse matrices class family with shape[0] == 1
+# - Iterable[Tuple[int, float]]
+
+# this method returns generator object
+yeabm.iter_document_vectors() # or
+yeabm.iter_document_vectors_sparse() # <--- recommended for usage with Vector DB
+# use it in loop
+for vector in yeabm.iter_document_vectors_sparse():
     # dostuff could be put in DB. 
     dostuff(vector)
 
 query = ...
 yeabm.encode_query(query)
 ```
 
 Why would you want to do that? Essentially the BM25 score formula is a sum, so it is a perfect candidate for one of the metrics any DB
-supports - inner product.
+supports - **inner product (IP)**.
 ```python
 # 
 bm_index.get_scores(['quick', 'fox'])
 # ~ [1.30, 0.0, 0.72, 0.0, 0.0, 0.0]
 
 # you get the same scores like so:
-yeabm.get_embeddings() @ np.asarray(yeabm.encode_query(['fox', 'quick']))
+yeabm.get_embeddings() @ np.asarray(yeabm.encode_query_dense(['fox', 'quick']))
 # ~ [1.30, 0.0, 0.72, 0.0, 0.0, 0.0]
 ```
 Of course you would like to leave the last calculation to the Vector DB.
 
 One more opinionated implementation is that words that are found in more than half of the corpus would not have idf of 0. It would be small 
 but still positive. For example in other implementations:
 
@@ -295,7 +301,10 @@
 # [0. 0. 0. 0. 0. 0.]
 # where 
 yeabm.get_scores(['brown'])
 #[0.18 0.28 0.33  0. 0. 0.]
 # this is helpful if the user is looking for a term that is abundant in the corpus and would still get somewhat useful results
 # where with BM25Okapi you would get essentially random results (or no results).
 ```
+
+### Usage examples:
+- [Use sparse vectors with Milvus DB](examples/sparse_vector_milvus.ipynb)
```

### Comparing `yeabm25-0.1.2/tests/test_yeabm25.py` & `yeabm25-0.1.3/tests/test_yeabm25.py`

 * *Files 13% similar despite different names*

```diff
@@ -25,23 +25,45 @@
     yeabm = YeaBM25(epsilon=1)
     yeabm.fit(corpus=corpus)
     # the terms that are present in more than half of the corpus would get corrected
     terms_with_idf_correction = [k for k, v in yeabm.word_df.items() if v >= yeabm.corpus_size // 2]
     for term in terms_with_idf_correction:
         assert yeabm.idf[term] == yeabm.average_idf
 
+
 @pytest.mark.parametrize("epsilon", [0.25, 0.5, 0.75])
 def test_top_n(corpus, epsilon):
     yeabm = YeaBM25(epsilon=epsilon)
     yeabm.fit(corpus=corpus)
     scores = yeabm.get_top_n(['brown', 'quick', 'fox'], n=3)
     assert [i for i in scores] == [0, 2, 1]
     scores = yeabm.get_top_n(['man', 'windy', 'london'], n=3)
     assert [i for i in scores] == [4, 5, 3]
 
+
 @pytest.mark.parametrize("query, expected", [
     (['fox', 'quick'], [1, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0]),
-    (['cat', 'raven'], [0] * 14)])
+    (['cat', 'raven'], [0] * 14)
+])
+def test_encode_query_dense(corpus, query, expected):
+    yeabm = YeaBM25()
+    yeabm.fit(corpus)
+    assert yeabm.encode_query_dense(query) == expected
+
+
+@pytest.mark.parametrize("query, expected", [
+    (['fox', 'lazy'], {1: 1.0, 3: 1.0}),
+    (['cat', 'raven'], {})
+])
 def test_encode_query(corpus, query, expected):
     yeabm = YeaBM25()
     yeabm.fit(corpus)
-    assert yeabm.encode_query(query) == expected
+    assert yeabm.encode_query(query) == expected
+
+
+def test_fromdict_encodeonly(corpus):
+    yeabm = YeaBM25()
+    yeabm.fit(corpus=corpus)
+    state_dict = yeabm.state_dict(state='encodeonly')
+    new_yeabm = YeaBM25.from_state_dict(state_dict)
+
+    assert yeabm.idf == new_yeabm.idf
```

