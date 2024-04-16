# Comparing `tmp/e-models-1.8.7.1.tar.gz` & `tmp/e-models-1.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "e-models-1.8.7.1.tar", last modified: Tue Apr 16 15:08:08 2024, max compression
+gzip compressed data, was "e-models-1.8.8.tar", last modified: Tue Apr 16 17:36:35 2024, max compression
```

## Comparing `e-models-1.8.7.1.tar` & `e-models-1.8.8.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2024-04-16 15:08:08.836207 e-models-1.8.7.1/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1501 2023-03-30 21:13:00.000000 e-models-1.8.7.1/LICENSE
--rw-r--r--   0 molveyra  (1001) molveyra  (1001)    13332 2024-04-16 15:08:08.836207 e-models-1.8.7.1/PKG-INFO
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    12478 2024-02-27 17:55:52.000000 e-models-1.8.7.1/README.md
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2024-04-16 15:08:08.832207 e-models-1.8.7.1/e_models.egg-info/
--rw-r--r--   0 molveyra  (1001) molveyra  (1001)    13332 2024-04-16 15:08:08.000000 e-models-1.8.7.1/e_models.egg-info/PKG-INFO
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      710 2024-04-16 15:08:08.000000 e-models-1.8.7.1/e_models.egg-info/SOURCES.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        1 2024-04-16 15:08:08.000000 e-models-1.8.7.1/e_models.egg-info/dependency_links.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      104 2024-04-16 15:08:08.000000 e-models-1.8.7.1/e_models.egg-info/requires.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        8 2024-04-16 15:08:08.000000 e-models-1.8.7.1/e_models.egg-info/top_level.txt
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2024-04-16 15:08:08.832207 e-models-1.8.7.1/emodels/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       24 2024-04-16 15:07:20.000000 e-models-1.8.7.1/emodels/__init__.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      340 2023-11-06 19:18:12.000000 e-models-1.8.7.1/emodels/config.py
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2024-04-16 15:08:08.832207 e-models-1.8.7.1/emodels/datasets/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        0 2023-06-23 18:11:59.000000 e-models-1.8.7.1/emodels/datasets/__init__.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    16404 2023-11-03 19:09:54.000000 e-models-1.8.7.1/emodels/datasets/hugging.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    21173 2024-04-15 19:12:37.000000 e-models-1.8.7.1/emodels/datasets/models.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      374 2023-08-31 18:27:15.000000 e-models-1.8.7.1/emodels/datasets/stypes.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2299 2024-03-14 19:03:35.000000 e-models-1.8.7.1/emodels/datasets/tokenizers.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    12361 2024-03-18 21:52:08.000000 e-models-1.8.7.1/emodels/datasets/utils.py
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2024-04-16 15:08:08.832207 e-models-1.8.7.1/emodels/html2text/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    35479 2023-07-21 16:26:32.000000 e-models-1.8.7.1/emodels/html2text/__init__.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3873 2023-05-04 18:51:26.000000 e-models-1.8.7.1/emodels/html2text/config.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      423 2023-05-04 18:51:26.000000 e-models-1.8.7.1/emodels/html2text/elements.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       71 2023-05-04 18:51:26.000000 e-models-1.8.7.1/emodels/html2text/typing.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     8034 2023-05-04 18:51:26.000000 e-models-1.8.7.1/emodels/html2text/utils.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        0 2023-05-04 18:51:26.000000 e-models-1.8.7.1/emodels/py.typed
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2024-04-16 15:08:08.832207 e-models-1.8.7.1/emodels/scrapyutils/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        0 2023-08-04 13:47:09.000000 e-models-1.8.7.1/emodels/scrapyutils/__init__.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     4734 2024-02-27 12:04:53.000000 e-models-1.8.7.1/emodels/scrapyutils/loader.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     6339 2024-02-27 17:16:48.000000 e-models-1.8.7.1/emodels/scrapyutils/response.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       31 2023-03-30 21:32:48.000000 e-models-1.8.7.1/pyproject.toml
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       38 2024-04-16 15:08:08.836207 e-models-1.8.7.1/setup.cfg
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1088 2024-04-16 15:07:30.000000 e-models-1.8.7.1/setup.py
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2024-04-16 15:08:08.836207 e-models-1.8.7.1/tests/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     6355 2023-08-04 13:47:35.000000 e-models-1.8.7.1/tests/test_html2text.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    12999 2024-02-27 17:16:48.000000 e-models-1.8.7.1/tests/test_scrapyutils.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2024-04-16 17:36:35.159915 e-models-1.8.8/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1501 2023-03-30 21:13:00.000000 e-models-1.8.8/LICENSE
+-rw-r--r--   0 molveyra  (1001) molveyra  (1001)    13330 2024-04-16 17:36:35.159915 e-models-1.8.8/PKG-INFO
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    12478 2024-02-27 17:55:52.000000 e-models-1.8.8/README.md
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2024-04-16 17:36:35.155915 e-models-1.8.8/e_models.egg-info/
+-rw-r--r--   0 molveyra  (1001) molveyra  (1001)    13330 2024-04-16 17:36:35.000000 e-models-1.8.8/e_models.egg-info/PKG-INFO
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      710 2024-04-16 17:36:35.000000 e-models-1.8.8/e_models.egg-info/SOURCES.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        1 2024-04-16 17:36:35.000000 e-models-1.8.8/e_models.egg-info/dependency_links.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      104 2024-04-16 17:36:35.000000 e-models-1.8.8/e_models.egg-info/requires.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        8 2024-04-16 17:36:35.000000 e-models-1.8.8/e_models.egg-info/top_level.txt
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2024-04-16 17:36:35.155915 e-models-1.8.8/emodels/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       22 2024-04-16 17:29:32.000000 e-models-1.8.8/emodels/__init__.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      340 2023-11-06 19:18:12.000000 e-models-1.8.8/emodels/config.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2024-04-16 17:36:35.155915 e-models-1.8.8/emodels/datasets/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        0 2023-06-23 18:11:59.000000 e-models-1.8.8/emodels/datasets/__init__.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    16404 2023-11-03 19:09:54.000000 e-models-1.8.8/emodels/datasets/hugging.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    21428 2024-04-16 17:21:00.000000 e-models-1.8.8/emodels/datasets/models.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      374 2023-08-31 18:27:15.000000 e-models-1.8.8/emodels/datasets/stypes.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2299 2024-03-14 19:03:35.000000 e-models-1.8.8/emodels/datasets/tokenizers.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    12361 2024-03-18 21:52:08.000000 e-models-1.8.8/emodels/datasets/utils.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2024-04-16 17:36:35.155915 e-models-1.8.8/emodels/html2text/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    35479 2023-07-21 16:26:32.000000 e-models-1.8.8/emodels/html2text/__init__.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3873 2023-05-04 18:51:26.000000 e-models-1.8.8/emodels/html2text/config.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      423 2023-05-04 18:51:26.000000 e-models-1.8.8/emodels/html2text/elements.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       71 2023-05-04 18:51:26.000000 e-models-1.8.8/emodels/html2text/typing.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     8034 2023-05-04 18:51:26.000000 e-models-1.8.8/emodels/html2text/utils.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        0 2023-05-04 18:51:26.000000 e-models-1.8.8/emodels/py.typed
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2024-04-16 17:36:35.155915 e-models-1.8.8/emodels/scrapyutils/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        0 2023-08-04 13:47:09.000000 e-models-1.8.8/emodels/scrapyutils/__init__.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     4734 2024-02-27 12:04:53.000000 e-models-1.8.8/emodels/scrapyutils/loader.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     6339 2024-02-27 17:16:48.000000 e-models-1.8.8/emodels/scrapyutils/response.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       31 2023-03-30 21:32:48.000000 e-models-1.8.8/pyproject.toml
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       38 2024-04-16 17:36:35.159915 e-models-1.8.8/setup.cfg
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1086 2024-04-16 17:29:10.000000 e-models-1.8.8/setup.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2024-04-16 17:36:35.159915 e-models-1.8.8/tests/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     6355 2023-08-04 13:47:35.000000 e-models-1.8.8/tests/test_html2text.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    12999 2024-02-27 17:16:48.000000 e-models-1.8.8/tests/test_scrapyutils.py
```

### Comparing `e-models-1.8.7.1/LICENSE` & `e-models-1.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `e-models-1.8.7.1/PKG-INFO` & `e-models-1.8.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e-models
-Version: 1.8.7.1
+Version: 1.8.8
 Summary: Tools for helping build of extraction models with scrapy spiders.
 Home-page: https://github.com/kalessin/emodels
 Author: Martin Olveyra
 Author-email: molveyra@gmail.com
 License: BSD
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `e-models-1.8.7.1/README.md` & `e-models-1.8.8/README.md`

 * *Files identical despite different names*

### Comparing `e-models-1.8.7.1/e_models.egg-info/PKG-INFO` & `e-models-1.8.8/e_models.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e-models
-Version: 1.8.7.1
+Version: 1.8.8
 Summary: Tools for helping build of extraction models with scrapy spiders.
 Home-page: https://github.com/kalessin/emodels
 Author: Martin Olveyra
 Author-email: molveyra@gmail.com
 License: BSD
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `e-models-1.8.7.1/e_models.egg-info/SOURCES.txt` & `e-models-1.8.8/e_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `e-models-1.8.7.1/emodels/datasets/hugging.py` & `e-models-1.8.8/emodels/datasets/hugging.py`

 * *Files identical despite different names*

### Comparing `e-models-1.8.7.1/emodels/datasets/models.py` & `e-models-1.8.8/emodels/datasets/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -472,14 +472,19 @@
         return cls.classify_from_row(row, proba)
 
     @classmethod
     def predict(cls, df: pd.DataFrame, proba: int = -1) -> pd.Series:
         return df.apply(partial(cls.classify_from_row, proba=proba), axis=1)
 
     @classmethod
+    def predict_from_samples(cls, samples: List[SAMPLE], proba: int = -1) -> pd.Series:
+        df = pd.DataFrame([cls.get_row_from_sample(s) for s in samples])
+        return cls.predict(df, proba)
+
+    @classmethod
     def evaluate(cls, proba: int = -1, proba_threshold: float = 0.5):
         datasets = cls.get_dataset()
         predicted = cls.predict(datasets.X_train, proba)
         if proba >= 0:
             predicted = (predicted > proba_threshold).astype(numpy.int64)
         y_train = datasets.Y_train
 
@@ -537,14 +542,15 @@
         features: Sequence[DF] = cls.get_training_X_features(datasets.X_train)
         vfeatures: Sequence[Sequence[float]] = vectorizer.transform(features)
         model.fit(vfeatures, datasets.Y_train)
         return model
 
     @classmethod
     def classify_from_row(cls, row: pd.Series, proba: int = -1) -> float:
+        row = row[list(cls.features)]
         vectorizer: V = cls.get_vectorizer()
         model: M = cls.get_trained_model()
         X_features: Sequence[DF] = cls.get_features_from_dataframe_row(row)
         X_transformed: Sequence[Sequence[float]] = vectorizer.transform(X_features)
         if proba >= 0:
             return model.predict_proba(X_transformed)[0][proba]
         return model.predict(X_transformed)[0]
```

### Comparing `e-models-1.8.7.1/emodels/datasets/tokenizers.py` & `e-models-1.8.8/emodels/datasets/tokenizers.py`

 * *Files identical despite different names*

### Comparing `e-models-1.8.7.1/emodels/datasets/utils.py` & `e-models-1.8.8/emodels/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `e-models-1.8.7.1/emodels/html2text/__init__.py` & `e-models-1.8.8/emodels/html2text/__init__.py`

 * *Files identical despite different names*

### Comparing `e-models-1.8.7.1/emodels/html2text/config.py` & `e-models-1.8.8/emodels/html2text/config.py`

 * *Files identical despite different names*

### Comparing `e-models-1.8.7.1/emodels/html2text/utils.py` & `e-models-1.8.8/emodels/html2text/utils.py`

 * *Files identical despite different names*

### Comparing `e-models-1.8.7.1/emodels/scrapyutils/loader.py` & `e-models-1.8.8/emodels/scrapyutils/loader.py`

 * *Files identical despite different names*

### Comparing `e-models-1.8.7.1/emodels/scrapyutils/response.py` & `e-models-1.8.8/emodels/scrapyutils/response.py`

 * *Files identical despite different names*

### Comparing `e-models-1.8.7.1/setup.py` & `e-models-1.8.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Automatically created by: shub deploy
 
 from setuptools import setup, find_packages
 
 setup(
     name         = 'e-models',
-    version      = '1.8.7.1',
+    version      = '1.8.8',
     description  = 'Tools for helping build of extraction models with scrapy spiders.',
     long_description = open('README.md').read(),
     long_description_content_type = 'text/markdown',
     license      = 'BSD',
     author       = 'Martin Olveyra',
     author_email = 'molveyra@gmail.com',
     url          = 'https://github.com/kalessin/emodels',
```

### Comparing `e-models-1.8.7.1/tests/test_html2text.py` & `e-models-1.8.8/tests/test_html2text.py`

 * *Files identical despite different names*

### Comparing `e-models-1.8.7.1/tests/test_scrapyutils.py` & `e-models-1.8.8/tests/test_scrapyutils.py`

 * *Files identical despite different names*

