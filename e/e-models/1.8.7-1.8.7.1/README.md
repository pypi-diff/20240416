# Comparing `tmp/e-models-1.8.7.tar.gz` & `tmp/e-models-1.8.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "e-models-1.8.7.tar", last modified: Tue Apr  2 20:15:50 2024, max compression
+gzip compressed data, was "e-models-1.8.7.1.tar", last modified: Tue Apr 16 15:08:08 2024, max compression
```

## Comparing `e-models-1.8.7.tar` & `e-models-1.8.7.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2024-04-02 20:15:50.492570 e-models-1.8.7/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1501 2023-03-30 21:13:00.000000 e-models-1.8.7/LICENSE
--rw-r--r--   0 molveyra  (1001) molveyra  (1001)    13330 2024-04-02 20:15:50.492570 e-models-1.8.7/PKG-INFO
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    12478 2024-02-27 17:55:52.000000 e-models-1.8.7/README.md
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2024-04-02 20:15:50.484569 e-models-1.8.7/e_models.egg-info/
--rw-r--r--   0 molveyra  (1001) molveyra  (1001)    13330 2024-04-02 20:15:50.000000 e-models-1.8.7/e_models.egg-info/PKG-INFO
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      710 2024-04-02 20:15:50.000000 e-models-1.8.7/e_models.egg-info/SOURCES.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        1 2024-04-02 20:15:50.000000 e-models-1.8.7/e_models.egg-info/dependency_links.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      104 2024-04-02 20:15:50.000000 e-models-1.8.7/e_models.egg-info/requires.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        8 2024-04-02 20:15:50.000000 e-models-1.8.7/e_models.egg-info/top_level.txt
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2024-04-02 20:15:50.484569 e-models-1.8.7/emodels/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       22 2024-04-02 20:15:07.000000 e-models-1.8.7/emodels/__init__.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      340 2023-11-06 19:18:12.000000 e-models-1.8.7/emodels/config.py
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2024-04-02 20:15:50.488569 e-models-1.8.7/emodels/datasets/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        0 2023-06-23 18:11:59.000000 e-models-1.8.7/emodels/datasets/__init__.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    16404 2023-11-03 19:09:54.000000 e-models-1.8.7/emodels/datasets/hugging.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    20726 2024-04-02 20:12:36.000000 e-models-1.8.7/emodels/datasets/models.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      374 2023-08-31 18:27:15.000000 e-models-1.8.7/emodels/datasets/stypes.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2299 2024-03-14 19:03:35.000000 e-models-1.8.7/emodels/datasets/tokenizers.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    12361 2024-03-18 21:52:08.000000 e-models-1.8.7/emodels/datasets/utils.py
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2024-04-02 20:15:50.488569 e-models-1.8.7/emodels/html2text/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    35479 2023-07-21 16:26:32.000000 e-models-1.8.7/emodels/html2text/__init__.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3873 2023-05-04 18:51:26.000000 e-models-1.8.7/emodels/html2text/config.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      423 2023-05-04 18:51:26.000000 e-models-1.8.7/emodels/html2text/elements.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       71 2023-05-04 18:51:26.000000 e-models-1.8.7/emodels/html2text/typing.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     8034 2023-05-04 18:51:26.000000 e-models-1.8.7/emodels/html2text/utils.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        0 2023-05-04 18:51:26.000000 e-models-1.8.7/emodels/py.typed
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2024-04-02 20:15:50.488569 e-models-1.8.7/emodels/scrapyutils/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        0 2023-08-04 13:47:09.000000 e-models-1.8.7/emodels/scrapyutils/__init__.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     4734 2024-02-27 12:04:53.000000 e-models-1.8.7/emodels/scrapyutils/loader.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     6339 2024-02-27 17:16:48.000000 e-models-1.8.7/emodels/scrapyutils/response.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       31 2023-03-30 21:32:48.000000 e-models-1.8.7/pyproject.toml
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       38 2024-04-02 20:15:50.492570 e-models-1.8.7/setup.cfg
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1086 2024-04-02 20:15:17.000000 e-models-1.8.7/setup.py
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2024-04-02 20:15:50.488569 e-models-1.8.7/tests/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     6355 2023-08-04 13:47:35.000000 e-models-1.8.7/tests/test_html2text.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    12999 2024-02-27 17:16:48.000000 e-models-1.8.7/tests/test_scrapyutils.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2024-04-16 15:08:08.836207 e-models-1.8.7.1/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1501 2023-03-30 21:13:00.000000 e-models-1.8.7.1/LICENSE
+-rw-r--r--   0 molveyra  (1001) molveyra  (1001)    13332 2024-04-16 15:08:08.836207 e-models-1.8.7.1/PKG-INFO
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    12478 2024-02-27 17:55:52.000000 e-models-1.8.7.1/README.md
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2024-04-16 15:08:08.832207 e-models-1.8.7.1/e_models.egg-info/
+-rw-r--r--   0 molveyra  (1001) molveyra  (1001)    13332 2024-04-16 15:08:08.000000 e-models-1.8.7.1/e_models.egg-info/PKG-INFO
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      710 2024-04-16 15:08:08.000000 e-models-1.8.7.1/e_models.egg-info/SOURCES.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        1 2024-04-16 15:08:08.000000 e-models-1.8.7.1/e_models.egg-info/dependency_links.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      104 2024-04-16 15:08:08.000000 e-models-1.8.7.1/e_models.egg-info/requires.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        8 2024-04-16 15:08:08.000000 e-models-1.8.7.1/e_models.egg-info/top_level.txt
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2024-04-16 15:08:08.832207 e-models-1.8.7.1/emodels/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       24 2024-04-16 15:07:20.000000 e-models-1.8.7.1/emodels/__init__.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      340 2023-11-06 19:18:12.000000 e-models-1.8.7.1/emodels/config.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2024-04-16 15:08:08.832207 e-models-1.8.7.1/emodels/datasets/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        0 2023-06-23 18:11:59.000000 e-models-1.8.7.1/emodels/datasets/__init__.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    16404 2023-11-03 19:09:54.000000 e-models-1.8.7.1/emodels/datasets/hugging.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    21173 2024-04-15 19:12:37.000000 e-models-1.8.7.1/emodels/datasets/models.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      374 2023-08-31 18:27:15.000000 e-models-1.8.7.1/emodels/datasets/stypes.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2299 2024-03-14 19:03:35.000000 e-models-1.8.7.1/emodels/datasets/tokenizers.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    12361 2024-03-18 21:52:08.000000 e-models-1.8.7.1/emodels/datasets/utils.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2024-04-16 15:08:08.832207 e-models-1.8.7.1/emodels/html2text/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    35479 2023-07-21 16:26:32.000000 e-models-1.8.7.1/emodels/html2text/__init__.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3873 2023-05-04 18:51:26.000000 e-models-1.8.7.1/emodels/html2text/config.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      423 2023-05-04 18:51:26.000000 e-models-1.8.7.1/emodels/html2text/elements.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       71 2023-05-04 18:51:26.000000 e-models-1.8.7.1/emodels/html2text/typing.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     8034 2023-05-04 18:51:26.000000 e-models-1.8.7.1/emodels/html2text/utils.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        0 2023-05-04 18:51:26.000000 e-models-1.8.7.1/emodels/py.typed
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2024-04-16 15:08:08.832207 e-models-1.8.7.1/emodels/scrapyutils/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        0 2023-08-04 13:47:09.000000 e-models-1.8.7.1/emodels/scrapyutils/__init__.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     4734 2024-02-27 12:04:53.000000 e-models-1.8.7.1/emodels/scrapyutils/loader.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     6339 2024-02-27 17:16:48.000000 e-models-1.8.7.1/emodels/scrapyutils/response.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       31 2023-03-30 21:32:48.000000 e-models-1.8.7.1/pyproject.toml
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       38 2024-04-16 15:08:08.836207 e-models-1.8.7.1/setup.cfg
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1088 2024-04-16 15:07:30.000000 e-models-1.8.7.1/setup.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2024-04-16 15:08:08.836207 e-models-1.8.7.1/tests/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     6355 2023-08-04 13:47:35.000000 e-models-1.8.7.1/tests/test_html2text.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    12999 2024-02-27 17:16:48.000000 e-models-1.8.7.1/tests/test_scrapyutils.py
```

### Comparing `e-models-1.8.7/LICENSE` & `e-models-1.8.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `e-models-1.8.7/PKG-INFO` & `e-models-1.8.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e-models
-Version: 1.8.7
+Version: 1.8.7.1
 Summary: Tools for helping build of extraction models with scrapy spiders.
 Home-page: https://github.com/kalessin/emodels
 Author: Martin Olveyra
 Author-email: molveyra@gmail.com
 License: BSD
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `e-models-1.8.7/README.md` & `e-models-1.8.7.1/README.md`

 * *Files identical despite different names*

### Comparing `e-models-1.8.7/e_models.egg-info/PKG-INFO` & `e-models-1.8.7.1/e_models.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e-models
-Version: 1.8.7
+Version: 1.8.7.1
 Summary: Tools for helping build of extraction models with scrapy spiders.
 Home-page: https://github.com/kalessin/emodels
 Author: Martin Olveyra
 Author-email: molveyra@gmail.com
 License: BSD
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `e-models-1.8.7/e_models.egg-info/SOURCES.txt` & `e-models-1.8.7.1/e_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `e-models-1.8.7/emodels/datasets/hugging.py` & `e-models-1.8.7.1/emodels/datasets/hugging.py`

 * *Files identical despite different names*

### Comparing `e-models-1.8.7/emodels/datasets/models.py` & `e-models-1.8.7.1/emodels/datasets/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -264,14 +264,19 @@
                 yield sd
 
 
 class ModelWithVectorizer(Generic[SAMPLE, E, DF, V], ModelWithDataset[SAMPLE, E]):
     vectorizer_repository: VectorizerFilename
     vectorizer: V | None = None
 
+    def __init_subclass__(cls):
+        super().__init_subclass__()
+        if hasattr(cls, "vectorizer_repository") and cls.vectorizer_repository is not None:
+            assert cls.vectorizer is None, "model vectorizer must be initially None when you set vectorizer_repository"
+
     @classmethod
     @abstractmethod
     def instantiate_vectorizer(cls) -> V:
         ...
 
     @classmethod
     def load_vectorizer(cls) -> V:
@@ -297,14 +302,17 @@
             joblib.dump(vectorizer, vectorizer_local)
             cls._fshelper().upload_file(vectorizer_local, cls.vectorizer_repository)
         return joblib.load(vectorizer_local)
 
     @classmethod
     def get_vectorizer(cls) -> V:
         if cls.vectorizer is None:
+            assert (
+                cls.vectorizer_repository is not None
+            ), "vectorizer_repository attribute is required when vectorizer is trainable."
             cls.vectorizer = cls.load_vectorizer()
         return cls.vectorizer
 
     @classmethod
     def reset(cls):
         if hasattr(cls, "vectorizer_repository"):
             cls.delete_model_files(cls.vectorizer_repository)
```

### Comparing `e-models-1.8.7/emodels/datasets/tokenizers.py` & `e-models-1.8.7.1/emodels/datasets/tokenizers.py`

 * *Files identical despite different names*

### Comparing `e-models-1.8.7/emodels/datasets/utils.py` & `e-models-1.8.7.1/emodels/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `e-models-1.8.7/emodels/html2text/__init__.py` & `e-models-1.8.7.1/emodels/html2text/__init__.py`

 * *Files identical despite different names*

### Comparing `e-models-1.8.7/emodels/html2text/config.py` & `e-models-1.8.7.1/emodels/html2text/config.py`

 * *Files identical despite different names*

### Comparing `e-models-1.8.7/emodels/html2text/utils.py` & `e-models-1.8.7.1/emodels/html2text/utils.py`

 * *Files identical despite different names*

### Comparing `e-models-1.8.7/emodels/scrapyutils/loader.py` & `e-models-1.8.7.1/emodels/scrapyutils/loader.py`

 * *Files identical despite different names*

### Comparing `e-models-1.8.7/emodels/scrapyutils/response.py` & `e-models-1.8.7.1/emodels/scrapyutils/response.py`

 * *Files identical despite different names*

### Comparing `e-models-1.8.7/setup.py` & `e-models-1.8.7.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Automatically created by: shub deploy
 
 from setuptools import setup, find_packages
 
 setup(
     name         = 'e-models',
-    version      = '1.8.7',
+    version      = '1.8.7.1',
     description  = 'Tools for helping build of extraction models with scrapy spiders.',
     long_description = open('README.md').read(),
     long_description_content_type = 'text/markdown',
     license      = 'BSD',
     author       = 'Martin Olveyra',
     author_email = 'molveyra@gmail.com',
     url          = 'https://github.com/kalessin/emodels',
```

### Comparing `e-models-1.8.7/tests/test_html2text.py` & `e-models-1.8.7.1/tests/test_html2text.py`

 * *Files identical despite different names*

### Comparing `e-models-1.8.7/tests/test_scrapyutils.py` & `e-models-1.8.7.1/tests/test_scrapyutils.py`

 * *Files identical despite different names*

