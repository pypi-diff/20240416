# Comparing `tmp/pre5g-3.7.tar.gz` & `tmp/pre5g-3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pre5g-3.7.tar", last modified: Tue Apr 16 05:35:31 2024, max compression
+gzip compressed data, was "dist/pre5g-3.8.tar", last modified: Tue Apr 16 05:44:47 2024, max compression
```

## Comparing `pre5g-3.7.tar` & `pre5g-3.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 trainee   (1003) trainee   (1003)        0 2024-04-16 05:35:31.662017 pre5g-3.7/
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     1063 2024-03-26 07:38:31.000000 pre5g-3.7/LICENSE
--rw-r--r--   0 trainee   (1003) trainee   (1003)      491 2024-04-16 05:35:31.662017 pre5g-3.7/PKG-INFO
--rw-rw-r--   0 trainee   (1003) trainee   (1003)       82 2024-03-26 07:39:06.000000 pre5g-3.7/README.md
-drwxrwxr-x   0 trainee   (1003) trainee   (1003)        0 2024-04-16 05:35:31.653017 pre5g-3.7/pre5g/
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     1137 2024-04-04 11:14:45.000000 pre5g-3.7/pre5g/__init__.py
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     1933 2024-04-16 05:35:02.000000 pre5g-3.7/pre5g/labelen.py
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     2707 2024-04-01 11:33:46.000000 pre5g-3.7/pre5g/normalization.py
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     3398 2024-04-16 05:16:56.000000 pre5g-3.7/pre5g/nullvalue.py
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     3134 2024-04-16 04:29:45.000000 pre5g-3.7/pre5g/onehoten.py
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     3355 2024-04-15 10:02:56.000000 pre5g-3.7/pre5g/robustscaler.py
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     3124 2024-04-01 11:39:06.000000 pre5g-3.7/pre5g/standardization.py
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     2422 2024-04-15 07:20:59.000000 pre5g-3.7/pre5g/winsorization.py
-drwxrwxr-x   0 trainee   (1003) trainee   (1003)        0 2024-04-16 05:35:31.661017 pre5g-3.7/pre5g.egg-info/
--rw-r--r--   0 trainee   (1003) trainee   (1003)      491 2024-04-16 05:35:31.000000 pre5g-3.7/pre5g.egg-info/PKG-INFO
--rw-rw-r--   0 trainee   (1003) trainee   (1003)      307 2024-04-16 05:35:31.000000 pre5g-3.7/pre5g.egg-info/SOURCES.txt
--rw-rw-r--   0 trainee   (1003) trainee   (1003)        1 2024-04-16 05:35:31.000000 pre5g-3.7/pre5g.egg-info/dependency_links.txt
--rw-rw-r--   0 trainee   (1003) trainee   (1003)        6 2024-04-16 05:35:31.000000 pre5g-3.7/pre5g.egg-info/top_level.txt
--rw-rw-r--   0 trainee   (1003) trainee   (1003)       38 2024-04-16 05:35:31.662017 pre5g-3.7/setup.cfg
--rw-rw-r--   0 trainee   (1003) trainee   (1003)      600 2024-04-16 05:35:26.000000 pre5g-3.7/setup.py
+drwxrwxr-x   0 trainee   (1003) trainee   (1003)        0 2024-04-16 05:44:47.176076 pre5g-3.8/
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     1063 2024-03-26 07:38:31.000000 pre5g-3.8/LICENSE
+-rw-r--r--   0 trainee   (1003) trainee   (1003)      491 2024-04-16 05:44:47.176076 pre5g-3.8/PKG-INFO
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)       82 2024-03-26 07:39:06.000000 pre5g-3.8/README.md
+drwxrwxr-x   0 trainee   (1003) trainee   (1003)        0 2024-04-16 05:44:47.167076 pre5g-3.8/pre5g/
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     1137 2024-04-04 11:14:45.000000 pre5g-3.8/pre5g/__init__.py
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     1878 2024-04-16 05:44:00.000000 pre5g-3.8/pre5g/labelen.py
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     2707 2024-04-01 11:33:46.000000 pre5g-3.8/pre5g/normalization.py
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     3398 2024-04-16 05:16:56.000000 pre5g-3.8/pre5g/nullvalue.py
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     3134 2024-04-16 04:29:45.000000 pre5g-3.8/pre5g/onehoten.py
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     3355 2024-04-15 10:02:56.000000 pre5g-3.8/pre5g/robustscaler.py
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     3124 2024-04-01 11:39:06.000000 pre5g-3.8/pre5g/standardization.py
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     2422 2024-04-15 07:20:59.000000 pre5g-3.8/pre5g/winsorization.py
+drwxrwxr-x   0 trainee   (1003) trainee   (1003)        0 2024-04-16 05:44:47.176076 pre5g-3.8/pre5g.egg-info/
+-rw-r--r--   0 trainee   (1003) trainee   (1003)      491 2024-04-16 05:44:47.000000 pre5g-3.8/pre5g.egg-info/PKG-INFO
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)      307 2024-04-16 05:44:47.000000 pre5g-3.8/pre5g.egg-info/SOURCES.txt
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)        1 2024-04-16 05:44:47.000000 pre5g-3.8/pre5g.egg-info/dependency_links.txt
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)        6 2024-04-16 05:44:47.000000 pre5g-3.8/pre5g.egg-info/top_level.txt
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)       38 2024-04-16 05:44:47.176076 pre5g-3.8/setup.cfg
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)      600 2024-04-16 05:44:39.000000 pre5g-3.8/setup.py
```

### Comparing `pre5g-3.7/LICENSE` & `pre5g-3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pre5g-3.7/pre5g/__init__.py` & `pre5g-3.8/pre5g/__init__.py`

 * *Files identical despite different names*

### Comparing `pre5g-3.7/pre5g/labelen.py` & `pre5g-3.8/pre5g/labelen.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,25 +38,24 @@
 
     Parameters:
     data (DataFrame): The input DataFrame.
     columns (list): List of column names to label encode.
 
     Returns:
     DataFrame: The DataFrame with selected columns label encoded.
-    dict: A dictionary containing the label encoders used for each column.
     """
     # Copy the original DataFrame
     encoded_data = data.copy()
     
     # Initialize LabelEncoder
     label_encoders = {}
     
     # Iterate through selected columns
     for column in columns:
         # Check if column exists and is categorical
         if column in data.columns and data[column].dtype == 'object':
+            # Initialize LabelEncoder for the column
+            label_encoders[column] = LabelEncoder()
             # Perform label encoding
-            label_encoder = LabelEncoder()
-            encoded_data[column] = label_encoder.fit_transform(data[column])
-            label_encoders[column] = label_encoder
+            encoded_data[column] = label_encoders[column].fit_transform(data[column])
     
     return encoded_data, label_encoders
```

### Comparing `pre5g-3.7/pre5g/normalization.py` & `pre5g-3.8/pre5g/normalization.py`

 * *Files identical despite different names*

### Comparing `pre5g-3.7/pre5g/nullvalue.py` & `pre5g-3.8/pre5g/nullvalue.py`

 * *Files identical despite different names*

### Comparing `pre5g-3.7/pre5g/onehoten.py` & `pre5g-3.8/pre5g/onehoten.py`

 * *Files identical despite different names*

### Comparing `pre5g-3.7/pre5g/robustscaler.py` & `pre5g-3.8/pre5g/robustscaler.py`

 * *Files identical despite different names*

### Comparing `pre5g-3.7/pre5g/standardization.py` & `pre5g-3.8/pre5g/standardization.py`

 * *Files identical despite different names*

### Comparing `pre5g-3.7/pre5g/winsorization.py` & `pre5g-3.8/pre5g/winsorization.py`

 * *Files identical despite different names*

### Comparing `pre5g-3.7/setup.py` & `pre5g-3.8/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pre5g',
-    version='3.7',
+    version='3.8',
     packages=find_packages(),
     description='An preprocessing package',
     author='SnehaM',
     author_email='1js20cs161@gmail.com',
     license='MIT',
     keywords=['example', 'package'],
     classifiers=[
```

