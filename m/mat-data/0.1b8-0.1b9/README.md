# Comparing `tmp/mat-data-0.1b8.tar.gz` & `tmp/mat-data-0.1b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mat-data-0.1b8.tar", last modified: Sun Dec 17 04:03:02 2023, max compression
+gzip compressed data, was "mat-data-0.1b9.tar", last modified: Sun Dec 17 10:35:00 2023, max compression
```

## Comparing `mat-data-0.1b8.tar` & `mat-data-0.1b9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-12-17 04:03:02.907711 mat-data-0.1b8/
--rw-r--r--   0 tarlisportela   (501) staff       (20)       86 2023-12-16 13:47:10.000000 mat-data-0.1b8/CHANGELOG.md
--rw-r--r--   0 tarlisportela   (501) staff       (20)    35129 2023-12-15 20:34:29.000000 mat-data-0.1b8/LICENSE
--rw-r--r--   0 tarlisportela   (501) staff       (20)      147 2023-12-15 20:28:19.000000 mat-data-0.1b8/MANIFEST.in
--rw-r--r--   0 tarlisportela   (501) staff       (20)   598446 2023-12-16 13:33:41.000000 mat-data-0.1b8/MAT-data-Tutorial.html
--rwx------   0 tarlisportela   (501) staff       (20)    43714 2023-12-17 04:02:46.000000 mat-data-0.1b8/MAT-data-Tutorial.ipynb
--rw-r--r--   0 tarlisportela   (501) staff       (20)     5435 2023-12-17 04:03:02.907475 mat-data-0.1b8/PKG-INFO
--rw-r--r--   0 tarlisportela   (501) staff       (20)     3165 2023-12-16 13:44:41.000000 mat-data-0.1b8/README.md
--rw-r--r--   0 tarlisportela   (501) staff       (20)      717 2023-12-16 03:29:23.000000 mat-data-0.1b8/Steps to Build.txt
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-12-17 04:03:02.906817 mat-data-0.1b8/mat_data.egg-info/
--rw-r--r--   0 tarlisportela   (501) staff       (20)     5435 2023-12-17 04:03:02.000000 mat-data-0.1b8/mat_data.egg-info/PKG-INFO
--rw-r--r--   0 tarlisportela   (501) staff       (20)      522 2023-12-17 04:03:02.000000 mat-data-0.1b8/mat_data.egg-info/SOURCES.txt
--rw-r--r--   0 tarlisportela   (501) staff       (20)        1 2023-12-17 04:03:02.000000 mat-data-0.1b8/mat_data.egg-info/dependency_links.txt
--rw-r--r--   0 tarlisportela   (501) staff       (20)      148 2023-12-17 04:03:02.000000 mat-data-0.1b8/mat_data.egg-info/requires.txt
--rw-r--r--   0 tarlisportela   (501) staff       (20)        8 2023-12-17 04:03:02.000000 mat-data-0.1b8/mat_data.egg-info/top_level.txt
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-12-17 04:03:02.902195 mat-data-0.1b8/matdata/
--rw-r--r--   0 tarlisportela   (501) staff       (20)    35129 2023-12-15 20:34:29.000000 mat-data-0.1b8/matdata/LICENSE
--rw-r--r--   0 tarlisportela   (501) staff       (20)     3165 2023-12-16 13:44:41.000000 mat-data-0.1b8/matdata/README.md
--rw-r--r--   0 tarlisportela   (501) staff       (20)        0 2023-12-15 20:25:37.000000 mat-data-0.1b8/matdata/__init__.py
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-12-17 04:03:02.899269 mat-data-0.1b8/matdata/assets/
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-12-17 04:03:02.902341 mat-data-0.1b8/matdata/assets/sample/
--rw-rw-r--   0 tarlisportela   (501) staff       (20)  7716732 2021-02-10 16:01:46.000000 mat-data-0.1b8/matdata/assets/sample/Foursquare_Sample.csv
--rw-r--r--   0 tarlisportela   (501) staff       (20)     6080 2023-12-17 04:02:29.000000 mat-data-0.1b8/matdata/datasets.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)    26386 2023-12-16 17:27:28.000000 mat-data-0.1b8/matdata/generator.py
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-12-17 04:03:02.906591 mat-data-0.1b8/matdata/inc/
--rw-r--r--   0 tarlisportela   (501) staff       (20)        0 2023-12-15 20:26:21.000000 mat-data-0.1b8/matdata/inc/__init__.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)    13708 2023-12-16 17:42:48.000000 mat-data-0.1b8/matdata/inc/converter.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)    52699 2023-12-16 17:28:01.000000 mat-data-0.1b8/matdata/inc/ts_io.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)    33310 2023-12-17 03:43:53.000000 mat-data-0.1b8/matdata/preprocess.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)     2131 2023-12-17 04:02:55.000000 mat-data-0.1b8/pyproject.toml
--rw-r--r--   0 tarlisportela   (501) staff       (20)       38 2023-12-17 04:03:02.907747 mat-data-0.1b8/setup.cfg
--rw-r--r--   0 tarlisportela   (501) staff       (20)     2340 2023-12-16 04:06:58.000000 mat-data-0.1b8/setup.py
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-12-17 10:35:00.482799 mat-data-0.1b9/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)       86 2023-12-16 13:47:10.000000 mat-data-0.1b9/CHANGELOG.md
+-rw-r--r--   0 tarlisportela   (501) staff       (20)    35129 2023-12-15 20:34:29.000000 mat-data-0.1b9/LICENSE
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      147 2023-12-15 20:28:19.000000 mat-data-0.1b9/MANIFEST.in
+-rw-r--r--   0 tarlisportela   (501) staff       (20)   598446 2023-12-16 13:33:41.000000 mat-data-0.1b9/MAT-data-Tutorial.html
+-rwx------   0 tarlisportela   (501) staff       (20)    43673 2023-12-17 04:10:42.000000 mat-data-0.1b9/MAT-data-Tutorial.ipynb
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     5435 2023-12-17 10:35:00.482381 mat-data-0.1b9/PKG-INFO
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     3165 2023-12-16 13:44:41.000000 mat-data-0.1b9/README.md
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      717 2023-12-16 03:29:23.000000 mat-data-0.1b9/Steps to Build.txt
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-12-17 10:35:00.481400 mat-data-0.1b9/mat_data.egg-info/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     5435 2023-12-17 10:35:00.000000 mat-data-0.1b9/mat_data.egg-info/PKG-INFO
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      522 2023-12-17 10:35:00.000000 mat-data-0.1b9/mat_data.egg-info/SOURCES.txt
+-rw-r--r--   0 tarlisportela   (501) staff       (20)        1 2023-12-17 10:35:00.000000 mat-data-0.1b9/mat_data.egg-info/dependency_links.txt
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      148 2023-12-17 10:35:00.000000 mat-data-0.1b9/mat_data.egg-info/requires.txt
+-rw-r--r--   0 tarlisportela   (501) staff       (20)        8 2023-12-17 10:35:00.000000 mat-data-0.1b9/mat_data.egg-info/top_level.txt
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-12-17 10:35:00.467044 mat-data-0.1b9/matdata/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)    35129 2023-12-15 20:34:29.000000 mat-data-0.1b9/matdata/LICENSE
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     3165 2023-12-16 13:44:41.000000 mat-data-0.1b9/matdata/README.md
+-rw-r--r--   0 tarlisportela   (501) staff       (20)        0 2023-12-15 20:25:37.000000 mat-data-0.1b9/matdata/__init__.py
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-12-17 10:35:00.460065 mat-data-0.1b9/matdata/assets/
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-12-17 10:35:00.468067 mat-data-0.1b9/matdata/assets/sample/
+-rw-rw-r--   0 tarlisportela   (501) staff       (20)  7716732 2021-02-10 16:01:46.000000 mat-data-0.1b9/matdata/assets/sample/Foursquare_Sample.csv
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     6080 2023-12-17 04:02:29.000000 mat-data-0.1b9/matdata/datasets.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)    26386 2023-12-16 17:27:28.000000 mat-data-0.1b9/matdata/generator.py
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-12-17 10:35:00.479147 mat-data-0.1b9/matdata/inc/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)        0 2023-12-15 20:26:21.000000 mat-data-0.1b9/matdata/inc/__init__.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)    13708 2023-12-16 17:42:48.000000 mat-data-0.1b9/matdata/inc/converter.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)    52699 2023-12-16 17:28:01.000000 mat-data-0.1b9/matdata/inc/ts_io.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)    34728 2023-12-17 10:34:32.000000 mat-data-0.1b9/matdata/preprocess.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     2131 2023-12-17 10:34:44.000000 mat-data-0.1b9/pyproject.toml
+-rw-r--r--   0 tarlisportela   (501) staff       (20)       38 2023-12-17 10:35:00.482859 mat-data-0.1b9/setup.cfg
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     2340 2023-12-16 04:06:58.000000 mat-data-0.1b9/setup.py
```

### Comparing `mat-data-0.1b8/LICENSE` & `mat-data-0.1b9/LICENSE`

 * *Files identical despite different names*

### Comparing `mat-data-0.1b8/MAT-data-Tutorial.html` & `mat-data-0.1b9/MAT-data-Tutorial.html`

 * *Files identical despite different names*

### Comparing `mat-data-0.1b8/MAT-data-Tutorial.ipynb` & `mat-data-0.1b9/MAT-data-Tutorial.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9995039682539683%*

 * *Differences: {"'cells'": "{10: {'metadata': {delete: ['jp-MarkdownHeadingCollapsed']}}}"}*

```diff
@@ -564,15 +564,14 @@
             "source": [
                 "convertDataset(data_path)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
-                "jp-MarkdownHeadingCollapsed": true,
                 "tags": []
             },
             "source": [
                 "### 2. Synthetic Data Generation\n",
                 "\n",
                 "TODO"
             ]
```

### Comparing `mat-data-0.1b8/PKG-INFO` & `mat-data-0.1b9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mat-data
-Version: 0.1b8
+Version: 0.1b9
 Summary: MAT-data: Data Preprocessing for Multiple Aspect Trajectory Data Mining
 Home-page: https://github.com/ttportela/mat-data
 Author: Tarlis Tortelli Portela
 Author-email: Tarlis Tortelli Portela <tarlis@tarlis.com.br>
 Maintainer-email: Tarlis Tortelli Portela <tarlis@tarlis.com.br>
 License: GPL Version 3 or superior (see LICENSE file)
 Project-URL: Homepage, https://github.com/ttportela/mat-data
```

### Comparing `mat-data-0.1b8/README.md` & `mat-data-0.1b9/README.md`

 * *Files identical despite different names*

### Comparing `mat-data-0.1b8/Steps to Build.txt` & `mat-data-0.1b9/Steps to Build.txt`

 * *Files identical despite different names*

### Comparing `mat-data-0.1b8/mat_data.egg-info/PKG-INFO` & `mat-data-0.1b9/mat_data.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mat-data
-Version: 0.1b8
+Version: 0.1b9
 Summary: MAT-data: Data Preprocessing for Multiple Aspect Trajectory Data Mining
 Home-page: https://github.com/ttportela/mat-data
 Author: Tarlis Tortelli Portela
 Author-email: Tarlis Tortelli Portela <tarlis@tarlis.com.br>
 Maintainer-email: Tarlis Tortelli Portela <tarlis@tarlis.com.br>
 License: GPL Version 3 or superior (see LICENSE file)
 Project-URL: Homepage, https://github.com/ttportela/mat-data
```

### Comparing `mat-data-0.1b8/mat_data.egg-info/SOURCES.txt` & `mat-data-0.1b9/mat_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mat-data-0.1b8/matdata/LICENSE` & `mat-data-0.1b9/matdata/LICENSE`

 * *Files identical despite different names*

### Comparing `mat-data-0.1b8/matdata/README.md` & `mat-data-0.1b9/matdata/README.md`

 * *Files identical despite different names*

### Comparing `mat-data-0.1b8/matdata/assets/sample/Foursquare_Sample.csv` & `mat-data-0.1b9/matdata/assets/sample/Foursquare_Sample.csv`

 * *Files identical despite different names*

### Comparing `mat-data-0.1b8/matdata/datasets.py` & `mat-data-0.1b9/matdata/datasets.py`

 * *Files identical despite different names*

### Comparing `mat-data-0.1b8/matdata/generator.py` & `mat-data-0.1b9/matdata/generator.py`

 * *Files identical despite different names*

### Comparing `mat-data-0.1b8/matdata/inc/converter.py` & `mat-data-0.1b9/matdata/inc/converter.py`

 * *Files identical despite different names*

### Comparing `mat-data-0.1b8/matdata/inc/ts_io.py` & `mat-data-0.1b9/matdata/inc/ts_io.py`

 * *Files identical despite different names*

### Comparing `mat-data-0.1b8/matdata/preprocess.py` & `mat-data-0.1b9/matdata/preprocess.py`

 * *Files 2% similar despite different names*

```diff
@@ -453,26 +453,24 @@
     
     if not ktrain:
         ktrain, ktest = splitData(df, k, random_num, tid_col, class_col)
     else:
         print("Train and test data provided.")
     
 #     print("Writing files...")
-    for x in range(k):
-        path = 'run'+str(x+1)
-        
-        if not os.path.exists(os.path.join(data_path, path)):
-            os.makedirs(os.path.join(data_path, path))
-            
+    for x in range(k):            
         train_aux = ktrain[x]
         test_aux  = ktest[x]
-            
         
-        print("Writing files ... " + str(x+1) +'/'+str(k))
         for outType in outformats:
+            print("Writing", outType, "files ... " + str(x+1) +'/'+str(k))
+            path = 'run'+str(x+1)
+            if not os.path.exists(os.path.join(data_path, path)):
+                os.makedirs(os.path.join(data_path, path))
+                
             writeFiles(data_path, os.path.join(path, fileprefix), train_aux, test_aux, tid_col, class_col, \
                      columns_order_zip if outType in ['zip', 'mat'] else columns_order_csv, mat_columns, None, \
                      outType, opSuff=str(x+1))
     print("Done.")
     print(" --------------------------------------------------------------------------------")
     
     return ktrain, ktest
@@ -492,19 +490,19 @@
     else:
         columns_order_zip = list(df.columns)
         columns_order_csv = list(df.columns)
     
     train = df.loc[df[tid_col].isin(train_index)]
     test  = df.loc[df[tid_col].isin(test_index)]
     
-    path = 'S'+str(int(sample_size*100))
-    if not os.path.exists(os.path.join(data_path, path)):
-            os.makedirs(os.path.join(data_path, path))
-    
     for outType in outformats:
+        path = 'S'+str(int(sample_size*100))
+        if not os.path.exists(os.path.join(data_path, path)):
+                os.makedirs(os.path.join(data_path, path))
+            
         writeFiles(data_path, os.path.join(path, fileprefix), train, test, tid_col, class_col, \
                  columns_order_zip if outType in ['zip', 'mat'] else columns_order_csv, mat_columns, None, outType, opSuff=path)
     
     return train, test
     
 # TODO fix stratify:
 def kfold_stratify(data_path, df, k=10, inc=1, limit=10, random_num=1, tid_col='tid', class_col='label', fileprefix='', 
@@ -521,33 +519,68 @@
         
     if not ktrain:
         ktrain, ktest = splitData(df, k, random_num, tid_col, class_col, ignore_ltk=ignore_ltk)
     else:
         print("Train and test data provided.")
     
     for x in range(0, limit, inc):
-        path = 'S'+str((x+1)*int(100/k))
         
-        if not os.path.exists(os.path.join(data_path, path)):
-            os.makedirs(os.path.join(data_path, path))
-            
         train_aux = ktrain[0]
         test_aux  = ktest[0]
         for y in range(1, x+1):
             train_aux = pd.concat([train_aux,  ktrain[y]])
             test_aux  = pd.concat([test_aux,   ktest[y]])
             
         for outType in outformats:
+            path = 'S'+str((x+1)*int(100/k))
+
+            if not os.path.exists(os.path.join(data_path, path)):
+                os.makedirs(os.path.join(data_path, path))
+            
             writeFiles(data_path, os.path.join(path, fileprefix), train_aux, test_aux, tid_col, class_col, \
                      columns_order_zip if outType in ['zip', 'mat'] else columns_order_csv, mat_columns, None, outType, opSuff=str(x+1))
     print(" Done.")
     print(" --------------------------------------------------------------------------------")
     
     return ktrain, ktest
 
+def klabels_stratify(df, kl=10, train_size=0.7, random_num=1, tid_col='tid', class_col='label', 
+             organize_columns=True, mat_columns=None, fileprefix='', outformats=['zip', 'csv', 'mat'], data_path='.'):
+
+    min_elements=1
+    
+    random.seed(random_num)
+    labels = df[class_col].unique()
+
+    n = min_elements if lk < min_elements else n
+
+    labels_index = random.sample(list(labels), n)
+    df = df.loc[df[class_col].isin(labels_index)]
+    
+    train_index, test_index, _ = splitTIDs(df, train_size, random_num, tid_col, class_col, min_elements=min_elements)
+    
+    if organize_columns:
+        df, columns_order_zip, columns_order_csv = organizeFrame(df, None, tid_col, class_col)
+    else:
+        columns_order_zip = list(df.columns)
+        columns_order_csv = list(df.columns)
+    
+    train = df.loc[df[tid_col].isin(train_index)]
+    test  = df.loc[df[tid_col].isin(test_index)]
+    
+    for outType in outformats:
+        path = 'L'+str(n)
+        if not os.path.exists(os.path.join(data_path, path)):
+                os.makedirs(os.path.join(data_path, path))
+                
+        writeFiles(data_path, os.path.join(path, fileprefix), train, test, tid_col, class_col, \
+                 columns_order_zip if outType in ['zip', 'mat'] else columns_order_csv, mat_columns, None, outType, opSuff=path)
+    
+    return train, test
+
 #def stratify(data_path, df, k=10, inc=1, limit=10, random_num=1, tid_col='tid', class_col='label', fileprefix='', 
 #             ktrain=None, ktest=None, organize_columns=True, mat_columns=None, outformats=['zip', 'csv', 'mat'], ignore_ltk=True):
 #    importer(['S', 'KFold'], globals())
 #    
 #    print(str(k)+"-fold stratification of train and test in... " + data_path)
 #    
 #    if organize_columns:
```

### Comparing `mat-data-0.1b8/pyproject.toml` & `mat-data-0.1b9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 [project]
 name = "mat-data"
-version = "0.1b8"
+version = "0.1b9"
 description = "MAT-data: Data Preprocessing for Multiple Aspect Trajectory Data Mining"
 authors = [
     {name = "Tarlis Tortelli Portela", email = "tarlis@tarlis.com.br"},
  ]
 maintainers = [
     {name = "Tarlis Tortelli Portela", email = "tarlis@tarlis.com.br"},
  ]
```

### Comparing `mat-data-0.1b8/setup.py` & `mat-data-0.1b9/setup.py`

 * *Files identical despite different names*

