# Comparing `tmp/probabilistic_word_embeddings-1.9.0.tar.gz` & `tmp/probabilistic_word_embeddings-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "probabilistic_word_embeddings-1.9.0.tar", max compression
+gzip compressed data, was "probabilistic_word_embeddings-1.9.1.tar", max compression
```

## Comparing `probabilistic_word_embeddings-1.9.0.tar` & `probabilistic_word_embeddings-1.9.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      235 2024-01-31 14:06:35.508869 probabilistic_word_embeddings-1.9.0/README.md
--rw-r--r--   0        0        0     3406 2024-01-30 15:54:34.060852 probabilistic_word_embeddings-1.9.0/probabilistic_word_embeddings/__init__.py
--rw-r--r--   0        0        0    17101 2022-02-11 12:52:21.792289 probabilistic_word_embeddings-1.9.0/probabilistic_word_embeddings/data/eval/Card-660.tsv
--rw-r--r--   0        0        0      544 2022-02-11 12:52:21.794652 probabilistic_word_embeddings-1.9.0/probabilistic_word_embeddings/data/eval/MC-30.tsv
--rw-r--r--   0        0        0    53593 2022-02-11 12:52:21.797827 probabilistic_word_embeddings-1.9.0/probabilistic_word_embeddings/data/eval/MEN-TR-3k.tsv
--rw-r--r--   0        0        0     7219 2022-02-11 12:52:21.805255 probabilistic_word_embeddings-1.9.0/probabilistic_word_embeddings/data/eval/MTurk-287.tsv
--rw-r--r--   0        0        0    19626 2022-11-07 15:05:53.936879 probabilistic_word_embeddings-1.9.0/probabilistic_word_embeddings/data/eval/MTurk-771.tsv
--rw-r--r--   0        0        0     1209 2022-02-11 12:52:21.810618 probabilistic_word_embeddings-1.9.0/probabilistic_word_embeddings/data/eval/RG-65.tsv
--rw-r--r--   0        0        0    49851 2022-02-11 12:52:21.813786 probabilistic_word_embeddings-1.9.0/probabilistic_word_embeddings/data/eval/RW-STANFORD.tsv
--rw-r--r--   0        0        0    18024 2022-02-11 12:52:21.820517 probabilistic_word_embeddings-1.9.0/probabilistic_word_embeddings/data/eval/SimLex999.tsv
--rw-r--r--   0        0        0    62470 2022-02-11 12:52:21.823693 probabilistic_word_embeddings-1.9.0/probabilistic_word_embeddings/data/eval/SimVerb-3500.tsv
--rw-r--r--   0        0        0     7405 2022-02-11 12:52:21.830909 probabilistic_word_embeddings-1.9.0/probabilistic_word_embeddings/data/eval/WS-353-ALL.tsv
--rw-r--r--   0        0        0     5134 2022-02-11 12:52:21.833629 probabilistic_word_embeddings-1.9.0/probabilistic_word_embeddings/data/eval/WS-353-REL.tsv
--rw-r--r--   0        0        0     4002 2022-02-11 12:52:21.835687 probabilistic_word_embeddings-1.9.0/probabilistic_word_embeddings/data/eval/WS-353-SIM.tsv
--rw-r--r--   0        0        0     2614 2022-02-11 12:52:21.837905 probabilistic_word_embeddings-1.9.0/probabilistic_word_embeddings/data/eval/YP-130.tsv
--rw-r--r--   0        0        0     7906 2024-01-30 15:54:34.063406 probabilistic_word_embeddings-1.9.0/probabilistic_word_embeddings/embeddings.py
--rw-r--r--   0        0        0    10932 2024-02-07 13:46:40.735787 probabilistic_word_embeddings-1.9.0/probabilistic_word_embeddings/estimation.py
--rwxr-xr-x   0        0        0    10644 2024-01-30 15:54:34.069929 probabilistic_word_embeddings-1.9.0/probabilistic_word_embeddings/evaluation.py
--rw-r--r--   0        0        0     3551 2024-01-30 15:54:34.073251 probabilistic_word_embeddings-1.9.0/probabilistic_word_embeddings/models.py
--rw-r--r--   0        0        0     6315 2024-01-31 10:23:50.937209 probabilistic_word_embeddings-1.9.0/probabilistic_word_embeddings/preprocessing.py
--rw-r--r--   0        0        0     4239 2024-01-30 15:54:34.078521 probabilistic_word_embeddings-1.9.0/probabilistic_word_embeddings/utils.py
--rw-r--r--   0        0        0      580 2024-02-07 13:46:56.612992 probabilistic_word_embeddings-1.9.0/pyproject.toml
--rw-r--r--   0        0        0     1179 1970-01-01 00:00:00.000000 probabilistic_word_embeddings-1.9.0/PKG-INFO
+-rw-r--r--   0        0        0      235 2024-01-31 14:06:35.508869 probabilistic_word_embeddings-1.9.1/README.md
+-rw-r--r--   0        0        0     3406 2024-01-30 15:54:34.060852 probabilistic_word_embeddings-1.9.1/probabilistic_word_embeddings/__init__.py
+-rw-r--r--   0        0        0    17101 2022-02-11 12:52:21.792289 probabilistic_word_embeddings-1.9.1/probabilistic_word_embeddings/data/eval/Card-660.tsv
+-rw-r--r--   0        0        0      544 2022-02-11 12:52:21.794652 probabilistic_word_embeddings-1.9.1/probabilistic_word_embeddings/data/eval/MC-30.tsv
+-rw-r--r--   0        0        0    53593 2022-02-11 12:52:21.797827 probabilistic_word_embeddings-1.9.1/probabilistic_word_embeddings/data/eval/MEN-TR-3k.tsv
+-rw-r--r--   0        0        0     7219 2022-02-11 12:52:21.805255 probabilistic_word_embeddings-1.9.1/probabilistic_word_embeddings/data/eval/MTurk-287.tsv
+-rw-r--r--   0        0        0    19626 2022-11-07 15:05:53.936879 probabilistic_word_embeddings-1.9.1/probabilistic_word_embeddings/data/eval/MTurk-771.tsv
+-rw-r--r--   0        0        0     1209 2022-02-11 12:52:21.810618 probabilistic_word_embeddings-1.9.1/probabilistic_word_embeddings/data/eval/RG-65.tsv
+-rw-r--r--   0        0        0    49851 2022-02-11 12:52:21.813786 probabilistic_word_embeddings-1.9.1/probabilistic_word_embeddings/data/eval/RW-STANFORD.tsv
+-rw-r--r--   0        0        0    18024 2022-02-11 12:52:21.820517 probabilistic_word_embeddings-1.9.1/probabilistic_word_embeddings/data/eval/SimLex999.tsv
+-rw-r--r--   0        0        0    62470 2022-02-11 12:52:21.823693 probabilistic_word_embeddings-1.9.1/probabilistic_word_embeddings/data/eval/SimVerb-3500.tsv
+-rw-r--r--   0        0        0     7405 2022-02-11 12:52:21.830909 probabilistic_word_embeddings-1.9.1/probabilistic_word_embeddings/data/eval/WS-353-ALL.tsv
+-rw-r--r--   0        0        0     5134 2022-02-11 12:52:21.833629 probabilistic_word_embeddings-1.9.1/probabilistic_word_embeddings/data/eval/WS-353-REL.tsv
+-rw-r--r--   0        0        0     4002 2022-02-11 12:52:21.835687 probabilistic_word_embeddings-1.9.1/probabilistic_word_embeddings/data/eval/WS-353-SIM.tsv
+-rw-r--r--   0        0        0     2614 2022-02-11 12:52:21.837905 probabilistic_word_embeddings-1.9.1/probabilistic_word_embeddings/data/eval/YP-130.tsv
+-rw-r--r--   0        0        0     7906 2024-01-30 15:54:34.063406 probabilistic_word_embeddings-1.9.1/probabilistic_word_embeddings/embeddings.py
+-rw-r--r--   0        0        0    11439 2024-02-07 13:47:48.040797 probabilistic_word_embeddings-1.9.1/probabilistic_word_embeddings/estimation.py
+-rwxr-xr-x   0        0        0    10644 2024-01-30 15:54:34.069929 probabilistic_word_embeddings-1.9.1/probabilistic_word_embeddings/evaluation.py
+-rw-r--r--   0        0        0     3551 2024-01-30 15:54:34.073251 probabilistic_word_embeddings-1.9.1/probabilistic_word_embeddings/models.py
+-rw-r--r--   0        0        0     6315 2024-01-31 10:23:50.937209 probabilistic_word_embeddings-1.9.1/probabilistic_word_embeddings/preprocessing.py
+-rw-r--r--   0        0        0     4239 2024-01-30 15:54:34.078521 probabilistic_word_embeddings-1.9.1/probabilistic_word_embeddings/utils.py
+-rw-r--r--   0        0        0      580 2024-02-07 13:48:04.454527 probabilistic_word_embeddings-1.9.1/pyproject.toml
+-rw-r--r--   0        0        0     1179 1970-01-01 00:00:00.000000 probabilistic_word_embeddings-1.9.1/PKG-INFO
```

### Comparing `probabilistic_word_embeddings-1.9.0/probabilistic_word_embeddings/__init__.py` & `probabilistic_word_embeddings-1.9.1/probabilistic_word_embeddings/__init__.py`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.9.0/probabilistic_word_embeddings/data/eval/Card-660.tsv` & `probabilistic_word_embeddings-1.9.1/probabilistic_word_embeddings/data/eval/Card-660.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.9.0/probabilistic_word_embeddings/data/eval/MC-30.tsv` & `probabilistic_word_embeddings-1.9.1/probabilistic_word_embeddings/data/eval/MC-30.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.9.0/probabilistic_word_embeddings/data/eval/MEN-TR-3k.tsv` & `probabilistic_word_embeddings-1.9.1/probabilistic_word_embeddings/data/eval/MEN-TR-3k.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.9.0/probabilistic_word_embeddings/data/eval/MTurk-287.tsv` & `probabilistic_word_embeddings-1.9.1/probabilistic_word_embeddings/data/eval/MTurk-287.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.9.0/probabilistic_word_embeddings/data/eval/MTurk-771.tsv` & `probabilistic_word_embeddings-1.9.1/probabilistic_word_embeddings/data/eval/MTurk-771.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.9.0/probabilistic_word_embeddings/data/eval/RG-65.tsv` & `probabilistic_word_embeddings-1.9.1/probabilistic_word_embeddings/data/eval/RG-65.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.9.0/probabilistic_word_embeddings/data/eval/RW-STANFORD.tsv` & `probabilistic_word_embeddings-1.9.1/probabilistic_word_embeddings/data/eval/RW-STANFORD.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.9.0/probabilistic_word_embeddings/data/eval/SimLex999.tsv` & `probabilistic_word_embeddings-1.9.1/probabilistic_word_embeddings/data/eval/SimLex999.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.9.0/probabilistic_word_embeddings/data/eval/SimVerb-3500.tsv` & `probabilistic_word_embeddings-1.9.1/probabilistic_word_embeddings/data/eval/SimVerb-3500.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.9.0/probabilistic_word_embeddings/data/eval/WS-353-ALL.tsv` & `probabilistic_word_embeddings-1.9.1/probabilistic_word_embeddings/data/eval/WS-353-ALL.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.9.0/probabilistic_word_embeddings/data/eval/WS-353-REL.tsv` & `probabilistic_word_embeddings-1.9.1/probabilistic_word_embeddings/data/eval/WS-353-REL.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.9.0/probabilistic_word_embeddings/data/eval/WS-353-SIM.tsv` & `probabilistic_word_embeddings-1.9.1/probabilistic_word_embeddings/data/eval/WS-353-SIM.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.9.0/probabilistic_word_embeddings/data/eval/YP-130.tsv` & `probabilistic_word_embeddings-1.9.1/probabilistic_word_embeddings/data/eval/YP-130.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.9.0/probabilistic_word_embeddings/embeddings.py` & `probabilistic_word_embeddings-1.9.1/probabilistic_word_embeddings/embeddings.py`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.9.0/probabilistic_word_embeddings/estimation.py` & `probabilistic_word_embeddings-1.9.1/probabilistic_word_embeddings/estimation.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,47 +119,52 @@
                     logger.log(logging.TRAIN, f"Epoch {epoch} mean training loss after {batch_no} batches: {np.mean(epoch_training_loss)}")
 
     if early_stopping and valid_data is not None and best_valid_weights is not None:
         logger.info("Assign the weights corresponding to the best validation loss")
         embedding.theta.assign(best_valid_weights)
     return embedding
 
-def mean_field_vi(embedding, data, model="cbow", ws=5, ns=5, batch_size=25000, epochs=5, init_mean=True, init_std=0.05, evaluate=True, valid_data=None, elbo_history=False, loglevel="DEBUG"):
+def mean_field_vi(embedding, data=None, data_generator=None, N=None, model="cbow", ws=5, ns=5, batch_size=25000, epochs=5, init_mean=True, init_std=0.05, evaluate=True, valid_data=None, elbo_history=False,    loglevel="DEBUG"):
     """
     Perform mean-field variational inference.
     
     Args:
         embedding: Embedding with a suitable vocabulary and log_prob function. Subclass of pwe.Embedding
         data: Data as a list of python strings.
+        data_generator: Data as a generator that yields (i, j, x) tuples, where i are the center words as tf.Tensor (str),
+            j are the context words as tf.Tensor (str), and x the Bernoulli outcomes as tf.Tensor (int). Alternative to 'data'.
+        N (int): number of observations. Only necessary when using 'data_generator'.
         model (str): Word embedding model, either 'sgns' or 'cbow'.
         ws (int): SGNS or CBOW window size
         ns (int): SGNS or CBOW number of negative samples
         batch_size (int): Batch size in the training process 
         epochs (int): The number of passes over the data.
         init_mean (bool): Randomize the initial values of the embedding. If False, uses the values provided in the 'embedding' argument.
         init_std (float / np.array / tf.Tensor): Default value for the standard deviations. Can be a scalar (float) or an array (np.array / tf.Tensor)
         evaluate (bool): Whether to run word similarity evaluation during training on the standard English evaluation data sets
         valid_data: Data as a list of python strings.
         elbo_history (bool): Whether to return the ELBO history as a list
-    
+
     Returns:
         A tuple consisting of the means as a pwe.Embedding and the standard deviations as an np.array
     """
     logger = get_logger(loglevel, name="vi")
     if not isinstance(embedding, Embedding):
         warnings.warn("embedding is not a subclass of probabilistic_word_embeddings.Embedding")
     if model not in ["sgns", "cbow"]:
         raise ValueError("model must be 'sgns' or 'cbow'")
 
-    if not isinstance(data, tf.Tensor):
-        data = tf.constant(data)
-
     optimizer = tf.keras.optimizers.experimental.Adam(learning_rate=0.001)
     e = embedding
-    N = len(data)
+
+    if data is not None:
+        if not isinstance(data, tf.Tensor):
+            data = tf.constant(data)
+        N = len(data)
+
     batches = N // batch_size
     
     q_mean_init = embedding.theta
     if init_mean:
         q_mean_init = tf.random.normal(e.theta.shape, dtype=tf.float64) * 0.00001
     q_mean = tf.Variable(q_mean_init)
     if type(init_std) == float:
@@ -182,16 +187,19 @@
         epoch_logprobs = []
         for batch in progressbar.progressbar(random.sample(range(batches),batches)):
             # Reparametrization trick, Q = mu + sigma * epsilon
             epsilon = tf.random.normal(q_std_log.shape, dtype=tf.float64)
             z = q_mean + tf.multiply(tf.math.exp(q_std_log), epsilon)
             embedding.theta.assign(z)
             
-            start_ix = batch_size * batch
-            i,j,x  = generate_batch(data, model=model, ws=ws, ns=ns, batch_size=batch_size, start_ix=start_ix)
+            if data is None:
+                i,j,x = next(data_generator)
+            else:
+                start_ix = batch_size * batch
+                i,j,x  = generate_batch(data, model=model, ws=ws, ns=ns, batch_size=batch_size, start_ix=start_ix)
 
             with tf.GradientTape() as tape:
                 if model == "cbow":
                     log_prob = tf.reduce_sum(cbow_likelihood(e, i, j, x=x)) + e.log_prob(batch_size, N)
                 elif model == "sgns":
                     log_prob = tf.reduce_sum(sgns_likelihood(e, i, j, x=x)) + e.log_prob(batch_size, N)
                 epoch_logprobs.append(log_prob * N / batch_size)
```

### Comparing `probabilistic_word_embeddings-1.9.0/probabilistic_word_embeddings/evaluation.py` & `probabilistic_word_embeddings-1.9.1/probabilistic_word_embeddings/evaluation.py`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.9.0/probabilistic_word_embeddings/models.py` & `probabilistic_word_embeddings-1.9.1/probabilistic_word_embeddings/models.py`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.9.0/probabilistic_word_embeddings/preprocessing.py` & `probabilistic_word_embeddings-1.9.1/probabilistic_word_embeddings/preprocessing.py`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.9.0/probabilistic_word_embeddings/utils.py` & `probabilistic_word_embeddings-1.9.1/probabilistic_word_embeddings/utils.py`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.9.0/pyproject.toml` & `probabilistic_word_embeddings-1.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "probabilistic-word-embeddings"
-version = "1.9.0"
+version = "1.9.1"
 description = "Probabilistic Word Embeddings for Python"
 authors = ["Your Name <you@example.com>"]
 license = "MIT"
 readme = "README.md"
 documentation = "https://ninpnin.github.io/probabilistic-word-embeddings/"
 
 [tool.poetry.dependencies]
```

### Comparing `probabilistic_word_embeddings-1.9.0/PKG-INFO` & `probabilistic_word_embeddings-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: probabilistic-word-embeddings
-Version: 1.9.0
+Version: 1.9.1
 Summary: Probabilistic Word Embeddings for Python
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

