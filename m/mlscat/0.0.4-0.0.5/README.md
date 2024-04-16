# Comparing `tmp/mlscat-0.0.4.tar.gz` & `tmp/mlscat-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlscat-0.0.4.tar", last modified: Wed Apr 10 06:56:34 2024, max compression
+gzip compressed data, was "mlscat-0.0.5.tar", last modified: Tue Apr 16 12:37:14 2024, max compression
```

## Comparing `mlscat-0.0.4.tar` & `mlscat-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 wink       (501) staff       (20)        0 2024-04-10 06:56:34.523596 mlscat-0.0.4/
--rw-r--r--   0 wink       (501) staff       (20)      756 2024-04-10 06:56:34.523291 mlscat-0.0.4/PKG-INFO
--rw-r--r--   0 wink       (501) staff       (20)      481 2024-04-09 04:32:51.000000 mlscat-0.0.4/README.md
-drwxr-xr-x   0 wink       (501) staff       (20)        0 2024-04-10 06:56:34.519654 mlscat-0.0.4/mlscat/
--rw-r--r--   0 wink       (501) staff       (20)      131 2024-04-10 06:56:27.000000 mlscat-0.0.4/mlscat/__init__.py
--rw-r--r--   0 wink       (501) staff       (20)      172 2024-04-08 14:31:16.000000 mlscat-0.0.4/mlscat/api.py
--rw-r--r--   0 wink       (501) staff       (20)     2110 2024-04-10 06:42:52.000000 mlscat-0.0.4/mlscat/attacks.py
--rw-r--r--   0 wink       (501) staff       (20)     1420 2024-04-09 07:28:32.000000 mlscat-0.0.4/mlscat/ranks.py
--rw-r--r--   0 wink       (501) staff       (20)     1700 2024-04-10 06:37:33.000000 mlscat-0.0.4/mlscat/utils.py
-drwxr-xr-x   0 wink       (501) staff       (20)        0 2024-04-10 06:56:34.522991 mlscat-0.0.4/mlscat.egg-info/
--rw-r--r--   0 wink       (501) staff       (20)      756 2024-04-10 06:56:34.000000 mlscat-0.0.4/mlscat.egg-info/PKG-INFO
--rw-r--r--   0 wink       (501) staff       (20)      250 2024-04-10 06:56:34.000000 mlscat-0.0.4/mlscat.egg-info/SOURCES.txt
--rw-r--r--   0 wink       (501) staff       (20)        1 2024-04-10 06:56:34.000000 mlscat-0.0.4/mlscat.egg-info/dependency_links.txt
--rw-r--r--   0 wink       (501) staff       (20)       13 2024-04-10 06:56:34.000000 mlscat-0.0.4/mlscat.egg-info/requires.txt
--rw-r--r--   0 wink       (501) staff       (20)        7 2024-04-10 06:56:34.000000 mlscat-0.0.4/mlscat.egg-info/top_level.txt
--rw-r--r--   0 wink       (501) staff       (20)       38 2024-04-10 06:56:34.523657 mlscat-0.0.4/setup.cfg
--rw-r--r--   0 wink       (501) staff       (20)      608 2024-04-08 13:19:29.000000 mlscat-0.0.4/setup.py
+drwxr-xr-x   0 wink       (501) staff       (20)        0 2024-04-16 12:37:14.414452 mlscat-0.0.5/
+-rw-r--r--   0 wink       (501) staff       (20)      798 2024-04-16 12:37:14.413747 mlscat-0.0.5/PKG-INFO
+-rw-r--r--   0 wink       (501) staff       (20)      523 2024-04-11 14:01:41.000000 mlscat-0.0.5/README.md
+drwxr-xr-x   0 wink       (501) staff       (20)        0 2024-04-16 12:37:14.409509 mlscat-0.0.5/mlscat/
+-rw-r--r--   0 wink       (501) staff       (20)      131 2024-04-16 12:36:56.000000 mlscat-0.0.5/mlscat/__init__.py
+-rw-r--r--   0 wink       (501) staff       (20)      172 2024-04-08 14:31:16.000000 mlscat-0.0.5/mlscat/api.py
+-rw-r--r--   0 wink       (501) staff       (20)     2110 2024-04-16 12:37:11.000000 mlscat-0.0.5/mlscat/attacks.py
+-rw-r--r--   0 wink       (501) staff       (20)     1420 2024-04-09 07:28:32.000000 mlscat-0.0.5/mlscat/ranks.py
+-rw-r--r--   0 wink       (501) staff       (20)     2216 2024-04-16 12:35:18.000000 mlscat-0.0.5/mlscat/utils.py
+drwxr-xr-x   0 wink       (501) staff       (20)        0 2024-04-16 12:37:14.412685 mlscat-0.0.5/mlscat.egg-info/
+-rw-r--r--   0 wink       (501) staff       (20)      798 2024-04-16 12:37:14.000000 mlscat-0.0.5/mlscat.egg-info/PKG-INFO
+-rw-r--r--   0 wink       (501) staff       (20)      250 2024-04-16 12:37:14.000000 mlscat-0.0.5/mlscat.egg-info/SOURCES.txt
+-rw-r--r--   0 wink       (501) staff       (20)        1 2024-04-16 12:37:14.000000 mlscat-0.0.5/mlscat.egg-info/dependency_links.txt
+-rw-r--r--   0 wink       (501) staff       (20)       13 2024-04-16 12:37:14.000000 mlscat-0.0.5/mlscat.egg-info/requires.txt
+-rw-r--r--   0 wink       (501) staff       (20)        7 2024-04-16 12:37:14.000000 mlscat-0.0.5/mlscat.egg-info/top_level.txt
+-rw-r--r--   0 wink       (501) staff       (20)       38 2024-04-16 12:37:14.414531 mlscat-0.0.5/setup.cfg
+-rw-r--r--   0 wink       (501) staff       (20)      608 2024-04-08 13:19:29.000000 mlscat-0.0.5/setup.py
```

### Comparing `mlscat-0.0.4/PKG-INFO` & `mlscat-0.0.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlscat
-Version: 0.0.4
+Version: 0.0.5
 Summary: A small cat help you enjoy your side channel attack journal!
 Author: i4mhmh
 Author-email: i4mhmh@outlook.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: pandas
@@ -13,14 +13,15 @@
 
 A small cat that helps you enjoy your side channel attack journey!
 
 ## Features
 
 - Read Datasets: We provide a simple method to read some exist datasets(it would be better if there have the same structure!
 - Cal Rank: try to give the key and result nparray
+- Simple Attack: CPA, Correlation.
 
 example:
 
 ```python
 import mlscat as cat
 
 print(cat.__version__)
@@ -33,8 +34,8 @@
 To install mlscat, just follow one steps:
 
 `pip install mlscat`
 
 ## Benefits
 
 - Reduce Workload.
-- Reduce Errors.
+- Increase hair volume.
```

### Comparing `mlscat-0.0.4/mlscat/attacks.py` & `mlscat-0.0.5/mlscat/attacks.py`

 * *Files identical despite different names*

### Comparing `mlscat-0.0.4/mlscat/ranks.py` & `mlscat-0.0.5/mlscat/ranks.py`

 * *Files identical despite different names*

### Comparing `mlscat-0.0.4/mlscat/utils.py` & `mlscat-0.0.5/mlscat/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -25,8 +25,30 @@
 def get_mid(p, k, mask, mask_scheme):
     if mask == -1:
         return int(AES_Sbox[p ^ k])
     if mask_scheme == 'bool':
         return int(AES_Sbox[p ^ k] ^ mask)
     # TODO: Supporting custom mask scheme
     else:
-        pass
+        pass
+
+
+def fit_cnn(data):
+    '''
+    `fit_cnn`
+
+    ## Parameters
+    `data`: ndarray which saved the traces
+
+    ## return 
+    array which fit cnn inputs
+    '''
+    return np.expand_dims(data, 1)
+
+def get_targets(plaintexts):
+    targets = np.zeros(shape=(plaintexts.shape[0], 256))
+    for num, plaintext in enumerate(plaintexts):
+        tmp_targets = np.zeros(shape=256)
+        for key in range(256):
+            tmp_targets[key] = AES_Sbox[key ^ plaintext]
+        targets[num] = tmp_targets
+    return targets
```

### Comparing `mlscat-0.0.4/mlscat.egg-info/PKG-INFO` & `mlscat-0.0.5/mlscat.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlscat
-Version: 0.0.4
+Version: 0.0.5
 Summary: A small cat help you enjoy your side channel attack journal!
 Author: i4mhmh
 Author-email: i4mhmh@outlook.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: pandas
@@ -13,14 +13,15 @@
 
 A small cat that helps you enjoy your side channel attack journey!
 
 ## Features
 
 - Read Datasets: We provide a simple method to read some exist datasets(it would be better if there have the same structure!
 - Cal Rank: try to give the key and result nparray
+- Simple Attack: CPA, Correlation.
 
 example:
 
 ```python
 import mlscat as cat
 
 print(cat.__version__)
@@ -33,8 +34,8 @@
 To install mlscat, just follow one steps:
 
 `pip install mlscat`
 
 ## Benefits
 
 - Reduce Workload.
-- Reduce Errors.
+- Increase hair volume.
```

### Comparing `mlscat-0.0.4/setup.py` & `mlscat-0.0.5/setup.py`

 * *Files identical despite different names*

