# Comparing `tmp/powerpax-0.1.1.tar.gz` & `tmp/powerpax-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "powerpax-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "powerpax-0.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `powerpax-0.1.1.tar` & `powerpax-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1077 2024-02-15 15:56:19.288485 powerpax-0.1.1/LICENSE.txt
--rw-r--r--   0        0        0     1355 2024-02-15 15:56:19.288485 powerpax-0.1.1/README.md
--rw-r--r--   0        0        0     2123 2024-02-15 15:56:19.288485 powerpax-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      635 2024-02-15 15:56:19.288485 powerpax-0.1.1/src/powerpax/__init__.py
--rw-r--r--   0        0        0    15890 2024-02-15 15:56:19.288485 powerpax-0.1.1/src/powerpax/_loop.py
--rw-r--r--   0        0        0      735 2024-02-15 15:56:19.288485 powerpax-0.1.1/src/powerpax/_tree.py
--rw-r--r--   0        0        0     4790 2024-02-15 15:56:19.288485 powerpax-0.1.1/src/powerpax/_vmap.py
--rw-r--r--   0        0        0       16 2024-02-15 15:56:19.288485 powerpax-0.1.1/tests/requirements.txt
--rw-r--r--   0        0        0     1127 2024-02-15 15:56:19.288485 powerpax-0.1.1/tests/test_checkpoint_chunked_scan.py
--rw-r--r--   0        0        0     1017 2024-02-15 15:56:19.288485 powerpax-0.1.1/tests/test_chunked_vmap.py
--rw-r--r--   0        0        0     1631 2024-02-15 15:56:19.288485 powerpax-0.1.1/tests/test_sliced_scan.py
--rw-r--r--   0        0        0      429 2024-02-15 15:56:19.288485 powerpax-0.1.1/tests/test_static.py
--rw-r--r--   0        0        0     2421 1970-01-01 00:00:00.000000 powerpax-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-04-16 01:15:13.576588 powerpax-0.1.2/LICENSE.txt
+-rw-r--r--   0        0        0     1355 2024-04-16 01:15:13.576588 powerpax-0.1.2/README.md
+-rw-r--r--   0        0        0     2123 2024-04-16 01:15:13.576588 powerpax-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      635 2024-04-16 01:15:13.576588 powerpax-0.1.2/src/powerpax/__init__.py
+-rw-r--r--   0        0        0    15900 2024-04-16 01:15:13.576588 powerpax-0.1.2/src/powerpax/_loop.py
+-rw-r--r--   0        0        0      735 2024-04-16 01:15:13.576588 powerpax-0.1.2/src/powerpax/_tree.py
+-rw-r--r--   0        0        0     4790 2024-04-16 01:15:13.576588 powerpax-0.1.2/src/powerpax/_vmap.py
+-rw-r--r--   0        0        0       16 2024-04-16 01:15:13.576588 powerpax-0.1.2/tests/requirements.txt
+-rw-r--r--   0        0        0     1127 2024-04-16 01:15:13.576588 powerpax-0.1.2/tests/test_checkpoint_chunked_scan.py
+-rw-r--r--   0        0        0     1017 2024-04-16 01:15:13.576588 powerpax-0.1.2/tests/test_chunked_vmap.py
+-rw-r--r--   0        0        0     1631 2024-04-16 01:15:13.576588 powerpax-0.1.2/tests/test_sliced_scan.py
+-rw-r--r--   0        0        0      429 2024-04-16 01:15:13.576588 powerpax-0.1.2/tests/test_static.py
+-rw-r--r--   0        0        0     2421 1970-01-01 00:00:00.000000 powerpax-0.1.2/PKG-INFO
```

### Comparing `powerpax-0.1.1/LICENSE.txt` & `powerpax-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `powerpax-0.1.1/README.md` & `powerpax-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `powerpax-0.1.1/pyproject.toml` & `powerpax-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `powerpax-0.1.1/src/powerpax/__init__.py` & `powerpax-0.1.2/src/powerpax/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,13 +6,13 @@
 This package provides a small set of useful utilities for working with
 JAX. For example, functions to limit the memory consumption of
 :func:`jax.vmap` (:func:`ppx.chunked_vmap <powerpax.chunked_vmap>`) or
 to keep the outputs of only a subset of :func:`jax.lax.scan`
 iterations (:func:`ppx.sliced_scan <powerpax.sliced_scan>`).
 """
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 __all__ = ["chunked_vmap", "sliced_scan", "checkpoint_chunked_scan", "Static"]
 
 from ._vmap import chunked_vmap
 from ._loop import sliced_scan, checkpoint_chunked_scan
 from ._tree import Static
```

### Comparing `powerpax-0.1.1/src/powerpax/_loop.py` & `powerpax-0.1.2/src/powerpax/_loop.py`

 * *Files 1% similar despite different names*

```diff
@@ -226,15 +226,15 @@
 
     def scan_y_to_carry(carry, x):
         old_carry, _ = carry
         new_carry, new_y = f(old_carry, x)
         return (new_carry, new_y), None
 
     def inner_scan(carry, xs):
-        dummy_y = jax.tree_map(
+        dummy_y = jax.tree_util.tree_map(
             lambda sd: jnp.zeros(sd.shape, dtype=sd.dtype),
             jax.eval_shape(
                 lambda carry, xs: f(
                     carry, jax.tree_util.tree_map(operator.itemgetter(0), xs)
                 )[1],
                 carry,
                 xs,
```

### Comparing `powerpax-0.1.1/src/powerpax/_tree.py` & `powerpax-0.1.2/src/powerpax/_tree.py`

 * *Files identical despite different names*

### Comparing `powerpax-0.1.1/src/powerpax/_vmap.py` & `powerpax-0.1.2/src/powerpax/_vmap.py`

 * *Files identical despite different names*

### Comparing `powerpax-0.1.1/tests/test_checkpoint_chunked_scan.py` & `powerpax-0.1.2/tests/test_checkpoint_chunked_scan.py`

 * *Files identical despite different names*

### Comparing `powerpax-0.1.1/tests/test_chunked_vmap.py` & `powerpax-0.1.2/tests/test_chunked_vmap.py`

 * *Files identical despite different names*

### Comparing `powerpax-0.1.1/tests/test_sliced_scan.py` & `powerpax-0.1.2/tests/test_sliced_scan.py`

 * *Files identical despite different names*

### Comparing `powerpax-0.1.1/PKG-INFO` & `powerpax-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: powerpax
-Version: 0.1.1
+Version: 0.1.2
 Summary: Small collection of useful utilities for JAX
 Author: Karl Otness
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

