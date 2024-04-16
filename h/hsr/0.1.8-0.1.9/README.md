# Comparing `tmp/hsr-0.1.8.tar.gz` & `tmp/hsr-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hsr-0.1.8.tar", last modified: Mon Apr 15 09:19:55 2024, max compression
+gzip compressed data, was "hsr-0.1.9.tar", last modified: Tue Apr 16 19:31:54 2024, max compression
```

## Comparing `hsr-0.1.8.tar` & `hsr-0.1.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 marcellocostamagna   (501) staff       (20)        0 2024-04-15 09:19:55.140887 hsr-0.1.8/
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)    34523 2024-02-21 11:44:17.000000 hsr-0.1.8/LICENSE
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)       33 2024-04-09 12:22:09.000000 hsr-0.1.8/MANIFEST.in
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)     1931 2024-04-15 09:19:55.138908 hsr-0.1.8/PKG-INFO
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)     1712 2024-02-28 12:10:43.000000 hsr-0.1.8/README.md
-drwxr-xr-x   0 marcellocostamagna   (501) staff       (20)        0 2024-04-15 09:19:54.697943 hsr-0.1.8/hsr/
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)      180 2024-02-21 11:44:17.000000 hsr-0.1.8/hsr/__init__.py
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)     7806 2024-02-21 11:44:17.000000 hsr-0.1.8/hsr/fingerprint.py
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)     4761 2024-02-21 11:44:17.000000 hsr-0.1.8/hsr/hsr_cli.py
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)     9745 2024-03-07 09:58:34.000000 hsr-0.1.8/hsr/pca_transform.py
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)     4342 2024-03-07 09:57:05.000000 hsr-0.1.8/hsr/pre_processing.py
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)     9553 2024-03-20 12:00:09.000000 hsr-0.1.8/hsr/similarity.py
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)     3830 2024-02-21 11:44:17.000000 hsr-0.1.8/hsr/utils.py
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)      229 2024-04-15 09:19:26.000000 hsr-0.1.8/hsr/version.py
-drwxr-xr-x   0 marcellocostamagna   (501) staff       (20)        0 2024-04-15 09:19:55.136671 hsr-0.1.8/hsr.egg-info/
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)     1931 2024-04-15 09:19:54.000000 hsr-0.1.8/hsr.egg-info/PKG-INFO
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)      476 2024-04-15 09:19:54.000000 hsr-0.1.8/hsr.egg-info/SOURCES.txt
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)        1 2024-04-15 09:19:54.000000 hsr-0.1.8/hsr.egg-info/dependency_links.txt
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)       41 2024-04-15 09:19:54.000000 hsr-0.1.8/hsr.egg-info/entry_points.txt
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)       18 2024-04-15 09:19:54.000000 hsr-0.1.8/hsr.egg-info/requires.txt
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)        4 2024-04-15 09:19:54.000000 hsr-0.1.8/hsr.egg-info/top_level.txt
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)       38 2024-04-15 09:19:55.141155 hsr-0.1.8/setup.cfg
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)     1018 2024-04-10 12:14:01.000000 hsr-0.1.8/setup.py
-drwxr-xr-x   0 marcellocostamagna   (501) staff       (20)        0 2024-04-15 09:19:55.132587 hsr-0.1.8/tests/
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)       17 2024-03-07 14:03:24.000000 hsr-0.1.8/tests/__init__.py
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)     3230 2024-03-07 14:03:14.000000 hsr-0.1.8/tests/test_fingerprint.py
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)     1320 2024-03-07 14:03:15.000000 hsr-0.1.8/tests/test_pca.py
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)     5315 2024-03-07 14:03:16.000000 hsr-0.1.8/tests/test_preprocessing.py
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)     2241 2024-03-07 14:03:18.000000 hsr-0.1.8/tests/test_similarity.py
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)     1562 2024-03-07 14:03:20.000000 hsr-0.1.8/tests/test_utils.py
+drwxr-xr-x   0 marcellocostamagna   (501) staff       (20)        0 2024-04-16 19:31:54.703136 hsr-0.1.9/
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)    34523 2024-02-21 11:44:17.000000 hsr-0.1.9/LICENSE
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)       33 2024-04-09 12:22:09.000000 hsr-0.1.9/MANIFEST.in
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)     1931 2024-04-16 19:31:54.702105 hsr-0.1.9/PKG-INFO
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)     1712 2024-02-28 12:10:43.000000 hsr-0.1.9/README.md
+drwxr-xr-x   0 marcellocostamagna   (501) staff       (20)        0 2024-04-16 19:31:54.491222 hsr-0.1.9/hsr/
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)      180 2024-02-21 11:44:17.000000 hsr-0.1.9/hsr/__init__.py
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)     7806 2024-02-21 11:44:17.000000 hsr-0.1.9/hsr/fingerprint.py
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)     4761 2024-02-21 11:44:17.000000 hsr-0.1.9/hsr/hsr_cli.py
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)    10341 2024-04-16 19:30:14.000000 hsr-0.1.9/hsr/pca_transform.py
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)     4342 2024-03-07 09:57:05.000000 hsr-0.1.9/hsr/pre_processing.py
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)     9553 2024-03-20 12:00:09.000000 hsr-0.1.9/hsr/similarity.py
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)     3830 2024-02-21 11:44:17.000000 hsr-0.1.9/hsr/utils.py
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)      229 2024-04-16 19:30:58.000000 hsr-0.1.9/hsr/version.py
+drwxr-xr-x   0 marcellocostamagna   (501) staff       (20)        0 2024-04-16 19:31:54.700925 hsr-0.1.9/hsr.egg-info/
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)     1931 2024-04-16 19:31:52.000000 hsr-0.1.9/hsr.egg-info/PKG-INFO
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)      476 2024-04-16 19:31:53.000000 hsr-0.1.9/hsr.egg-info/SOURCES.txt
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)        1 2024-04-16 19:31:52.000000 hsr-0.1.9/hsr.egg-info/dependency_links.txt
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)       41 2024-04-16 19:31:52.000000 hsr-0.1.9/hsr.egg-info/entry_points.txt
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)       18 2024-04-16 19:31:52.000000 hsr-0.1.9/hsr.egg-info/requires.txt
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)        4 2024-04-16 19:31:52.000000 hsr-0.1.9/hsr.egg-info/top_level.txt
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)       38 2024-04-16 19:31:54.703281 hsr-0.1.9/setup.cfg
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)     1018 2024-04-10 12:14:01.000000 hsr-0.1.9/setup.py
+drwxr-xr-x   0 marcellocostamagna   (501) staff       (20)        0 2024-04-16 19:31:54.699990 hsr-0.1.9/tests/
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)       17 2024-03-07 14:03:24.000000 hsr-0.1.9/tests/__init__.py
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)     3230 2024-03-07 14:03:14.000000 hsr-0.1.9/tests/test_fingerprint.py
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)     1320 2024-03-07 14:03:15.000000 hsr-0.1.9/tests/test_pca.py
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)     5315 2024-03-07 14:03:16.000000 hsr-0.1.9/tests/test_preprocessing.py
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)     2241 2024-03-07 14:03:18.000000 hsr-0.1.9/tests/test_similarity.py
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)     1562 2024-03-07 14:03:20.000000 hsr-0.1.9/tests/test_utils.py
```

### Comparing `hsr-0.1.8/LICENSE` & `hsr-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `hsr-0.1.8/PKG-INFO` & `hsr-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hsr
-Version: 0.1.8
+Version: 0.1.9
 Author: Marcello Costamagna
 License: AGPL-3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: rdkit
```

### Comparing `hsr-0.1.8/README.md` & `hsr-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `hsr-0.1.8/hsr/fingerprint.py` & `hsr-0.1.9/hsr/fingerprint.py`

 * *Files identical despite different names*

### Comparing `hsr-0.1.8/hsr/hsr_cli.py` & `hsr-0.1.9/hsr/hsr_cli.py`

 * *Files identical despite different names*

### Comparing `hsr-0.1.8/hsr/pca_transform.py` & `hsr-0.1.9/hsr/pca_transform.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,22 +60,31 @@
     
     threshold = 1e-4
     significant_indices = np.where(abs(eigenvalues) > threshold)[0]
 
     # Handle chirality
     if chirality:
         reduced_eigenvectors = extract_relevant_subspace(eigenvectors, significant_indices)
+        # If the number of eigenvectors is different from the number of significant indices,
+        # the chirality cannot be unambigously. The result may not be consistent.
+        if reduced_eigenvectors.shape[1] != len(significant_indices):
+            print(f'WARNING: Chirality may not be consistent. {reduced_eigenvectors.shape[1]-len(significant_indices)} vectors have arbitrary signs.')
+        
         determinant = np.linalg.det(reduced_eigenvectors) 
-        if determinant < 0:
-            eigenvectors[:, 0] *= -1
+        # if determinant < 0:
+        #     eigenvectors[:, 0] *= -1
    
         adjusted_eigenvectors, n_changes, best_eigenvector_to_flip  = adjust_eigenvector_signs(original_data, eigenvectors[:, significant_indices], chirality) 
         eigenvectors[:, significant_indices] = adjusted_eigenvectors
 
-        if n_changes % 2 == 1:            
+        # if n_changes % 2 == 1:            
+        #     eigenvectors[:, best_eigenvector_to_flip] *= -1
+        
+        # New approach to handle chirality by determinant imposition
+        if determinant*(-1)**n_changes < 0:
             eigenvectors[:, best_eigenvector_to_flip] *= -1
     
         transformed_data = np.dot(original_data, eigenvectors)
         dimesnionality = len(significant_indices)
         
         if print_steps:
             print(f'Covariance matrix:\n{covariance_matrix}\n')
@@ -100,15 +109,15 @@
         print(f'Transformed data:\n{transformed_data}\n')
 
     if return_axes:
         return transformed_data, eigenvectors
     else:
         return  transformed_data
 
-def adjust_eigenvector_signs(original_data, eigenvectors, chirality=False, tolerance= 1e-4):
+def adjust_eigenvector_signs(original_data, eigenvectors, chirality=False, tolerance= 1e-10):
     """
     Adjust the sign of eigenvectors based on the data's projections.
 
     This function iterates through each eigenvector and determines its sign by examining 
     the direction of the data's maximum projection along that eigenvector. If the maximum 
     projection is negative, the sign of the eigenvector is flipped. The function also 
     handles special cases such as symmetric distributions of projections and can adjust
```

### Comparing `hsr-0.1.8/hsr/pre_processing.py` & `hsr-0.1.9/hsr/pre_processing.py`

 * *Files identical despite different names*

### Comparing `hsr-0.1.8/hsr/similarity.py` & `hsr-0.1.9/hsr/similarity.py`

 * *Files identical despite different names*

### Comparing `hsr-0.1.8/hsr/utils.py` & `hsr-0.1.9/hsr/utils.py`

 * *Files identical despite different names*

### Comparing `hsr-0.1.8/hsr.egg-info/PKG-INFO` & `hsr-0.1.9/hsr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hsr
-Version: 0.1.8
+Version: 0.1.9
 Author: Marcello Costamagna
 License: AGPL-3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: rdkit
```

### Comparing `hsr-0.1.8/setup.py` & `hsr-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `hsr-0.1.8/tests/test_fingerprint.py` & `hsr-0.1.9/tests/test_fingerprint.py`

 * *Files identical despite different names*

### Comparing `hsr-0.1.8/tests/test_pca.py` & `hsr-0.1.9/tests/test_pca.py`

 * *Files identical despite different names*

### Comparing `hsr-0.1.8/tests/test_preprocessing.py` & `hsr-0.1.9/tests/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `hsr-0.1.8/tests/test_similarity.py` & `hsr-0.1.9/tests/test_similarity.py`

 * *Files identical despite different names*

### Comparing `hsr-0.1.8/tests/test_utils.py` & `hsr-0.1.9/tests/test_utils.py`

 * *Files identical despite different names*

