# Comparing `tmp/pre5g-3.3.tar.gz` & `tmp/pre5g-3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pre5g-3.3.tar", last modified: Tue Apr 16 03:59:43 2024, max compression
+gzip compressed data, was "dist/pre5g-3.4.tar", last modified: Tue Apr 16 04:11:59 2024, max compression
```

## Comparing `pre5g-3.3.tar` & `pre5g-3.4.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxrwxr-x   0 trainee   (1003) trainee   (1003)        0 2024-04-16 03:59:43.211875 pre5g-3.3/
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     1063 2024-03-26 07:38:31.000000 pre5g-3.3/LICENSE
--rw-r--r--   0 trainee   (1003) trainee   (1003)      491 2024-04-16 03:59:43.211875 pre5g-3.3/PKG-INFO
--rw-rw-r--   0 trainee   (1003) trainee   (1003)       82 2024-03-26 07:39:06.000000 pre5g-3.3/README.md
-drwxrwxr-x   0 trainee   (1003) trainee   (1003)        0 2024-04-16 03:59:43.210875 pre5g-3.3/pre5g/
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     1137 2024-04-04 11:14:45.000000 pre5g-3.3/pre5g/__init__.py
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     1042 2024-04-08 06:54:23.000000 pre5g-3.3/pre5g/labelen.py
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     2707 2024-04-01 11:33:46.000000 pre5g-3.3/pre5g/normalization.py
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     4306 2024-04-08 09:30:56.000000 pre5g-3.3/pre5g/nullvalue.py
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     2691 2024-04-16 03:59:18.000000 pre5g-3.3/pre5g/onehoten.py
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     3355 2024-04-15 10:02:56.000000 pre5g-3.3/pre5g/robustscaler.py
--rw-rw-r--   0 trainee   (1003) trainee   (1003)        0 2024-04-15 11:30:20.000000 pre5g-3.3/pre5g/setup.py
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     3124 2024-04-01 11:39:06.000000 pre5g-3.3/pre5g/standardization.py
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     2422 2024-04-15 07:20:59.000000 pre5g-3.3/pre5g/winsorization.py
-drwxrwxr-x   0 trainee   (1003) trainee   (1003)        0 2024-04-16 03:59:43.211875 pre5g-3.3/pre5g.egg-info/
--rw-r--r--   0 trainee   (1003) trainee   (1003)      491 2024-04-16 03:59:43.000000 pre5g-3.3/pre5g.egg-info/PKG-INFO
--rw-rw-r--   0 trainee   (1003) trainee   (1003)      322 2024-04-16 03:59:43.000000 pre5g-3.3/pre5g.egg-info/SOURCES.txt
--rw-rw-r--   0 trainee   (1003) trainee   (1003)        1 2024-04-16 03:59:43.000000 pre5g-3.3/pre5g.egg-info/dependency_links.txt
--rw-rw-r--   0 trainee   (1003) trainee   (1003)        6 2024-04-16 03:59:43.000000 pre5g-3.3/pre5g.egg-info/top_level.txt
--rw-rw-r--   0 trainee   (1003) trainee   (1003)       38 2024-04-16 03:59:43.212875 pre5g-3.3/setup.cfg
--rw-rw-r--   0 trainee   (1003) trainee   (1003)      600 2024-04-16 03:59:27.000000 pre5g-3.3/setup.py
+drwxrwxr-x   0 trainee   (1003) trainee   (1003)        0 2024-04-16 04:11:59.090962 pre5g-3.4/
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     1063 2024-03-26 07:38:31.000000 pre5g-3.4/LICENSE
+-rw-r--r--   0 trainee   (1003) trainee   (1003)      491 2024-04-16 04:11:59.089962 pre5g-3.4/PKG-INFO
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)       82 2024-03-26 07:39:06.000000 pre5g-3.4/README.md
+drwxrwxr-x   0 trainee   (1003) trainee   (1003)        0 2024-04-16 04:11:59.088962 pre5g-3.4/pre5g/
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     1137 2024-04-04 11:14:45.000000 pre5g-3.4/pre5g/__init__.py
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     1042 2024-04-08 06:54:23.000000 pre5g-3.4/pre5g/labelen.py
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     2707 2024-04-01 11:33:46.000000 pre5g-3.4/pre5g/normalization.py
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     4306 2024-04-08 09:30:56.000000 pre5g-3.4/pre5g/nullvalue.py
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     2831 2024-04-16 04:07:05.000000 pre5g-3.4/pre5g/onehoten.py
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     3355 2024-04-15 10:02:56.000000 pre5g-3.4/pre5g/robustscaler.py
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     3124 2024-04-01 11:39:06.000000 pre5g-3.4/pre5g/standardization.py
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     2422 2024-04-15 07:20:59.000000 pre5g-3.4/pre5g/winsorization.py
+drwxrwxr-x   0 trainee   (1003) trainee   (1003)        0 2024-04-16 04:11:59.089962 pre5g-3.4/pre5g.egg-info/
+-rw-r--r--   0 trainee   (1003) trainee   (1003)      491 2024-04-16 04:11:59.000000 pre5g-3.4/pre5g.egg-info/PKG-INFO
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)      307 2024-04-16 04:11:59.000000 pre5g-3.4/pre5g.egg-info/SOURCES.txt
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)        1 2024-04-16 04:11:59.000000 pre5g-3.4/pre5g.egg-info/dependency_links.txt
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)        6 2024-04-16 04:11:59.000000 pre5g-3.4/pre5g.egg-info/top_level.txt
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)       38 2024-04-16 04:11:59.090962 pre5g-3.4/setup.cfg
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)      600 2024-04-16 04:11:54.000000 pre5g-3.4/setup.py
```

### Comparing `pre5g-3.3/LICENSE` & `pre5g-3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pre5g-3.3/pre5g/__init__.py` & `pre5g-3.4/pre5g/__init__.py`

 * *Files identical despite different names*

### Comparing `pre5g-3.3/pre5g/labelen.py` & `pre5g-3.4/pre5g/labelen.py`

 * *Files identical despite different names*

### Comparing `pre5g-3.3/pre5g/normalization.py` & `pre5g-3.4/pre5g/normalization.py`

 * *Files identical despite different names*

### Comparing `pre5g-3.3/pre5g/nullvalue.py` & `pre5g-3.4/pre5g/nullvalue.py`

 * *Files identical despite different names*

### Comparing `pre5g-3.3/pre5g/onehoten.py` & `pre5g-3.4/pre5g/onehoten.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,14 +57,17 @@
         if column in data.columns and data[column].dtype == 'object':
             # Perform one-hot encoding
             encoded_column = pd.get_dummies(data[column], prefix=column)
             # Store the names of the one-hot encoded columns
             column_names.extend(encoded_column.columns)
             # Drop original column and concatenate one-hot encoded columns
             encoded_data = pd.concat([encoded_data.drop(column, axis=1), encoded_column], axis=1)
+        else:
+            # If column is not categorical, simply add it to the list of column names
+            column_names.append(column)
     
     # Convert DataFrame to list of lists
     encoded_list = encoded_data.values.tolist()
     
     # Insert column names as the first element in the list
     encoded_list.insert(0, column_names)
```

### Comparing `pre5g-3.3/pre5g/robustscaler.py` & `pre5g-3.4/pre5g/robustscaler.py`

 * *Files identical despite different names*

### Comparing `pre5g-3.3/pre5g/standardization.py` & `pre5g-3.4/pre5g/standardization.py`

 * *Files identical despite different names*

### Comparing `pre5g-3.3/pre5g/winsorization.py` & `pre5g-3.4/pre5g/winsorization.py`

 * *Files identical despite different names*

### Comparing `pre5g-3.3/setup.py` & `pre5g-3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pre5g',
-    version='3.3',
+    version='3.4',
     packages=find_packages(),
     description='An preprocessing package',
     author='SnehaM',
     author_email='1js20cs161@gmail.com',
     license='MIT',
     keywords=['example', 'package'],
     classifiers=[
```

