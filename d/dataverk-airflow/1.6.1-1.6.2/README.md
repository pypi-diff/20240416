# Comparing `tmp/dataverk_airflow-1.6.1.tar.gz` & `tmp/dataverk_airflow-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataverk_airflow-1.6.1.tar", max compression
+gzip compressed data, was "dataverk_airflow-1.6.2.tar", max compression
```

## Comparing `dataverk_airflow-1.6.1.tar` & `dataverk_airflow-1.6.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1061 2024-03-07 09:12:09.438398 dataverk_airflow-1.6.1/LICENSE
--rw-r--r--   0        0        0     8319 2024-03-07 09:12:09.438398 dataverk_airflow-1.6.1/README.md
--rw-r--r--   0        0        0      381 2024-03-07 09:12:09.438398 dataverk_airflow-1.6.1/dataverk_airflow/__init__.py
--rw-r--r--   0        0        0      752 2024-03-07 09:12:09.438398 dataverk_airflow-1.6.1/dataverk_airflow/bucket_read.py
--rw-r--r--   0        0        0     1264 2024-03-07 09:12:09.438398 dataverk_airflow-1.6.1/dataverk_airflow/git_clone.py
--rw-r--r--   0        0        0     9712 2024-03-07 09:12:09.438398 dataverk_airflow-1.6.1/dataverk_airflow/kubernetes_operator.py
--rw-r--r--   0        0        0     4222 2024-03-07 09:12:09.438398 dataverk_airflow-1.6.1/dataverk_airflow/notebook_operator.py
--rw-r--r--   0        0        0     1058 2024-03-07 09:12:09.438398 dataverk_airflow-1.6.1/dataverk_airflow/notifications.py
--rw-r--r--   0        0        0     4051 2024-03-07 09:12:09.438398 dataverk_airflow-1.6.1/dataverk_airflow/python_operator.py
--rw-r--r--   0        0        0     5716 2024-03-07 09:12:09.438398 dataverk_airflow-1.6.1/dataverk_airflow/quarto_operator.py
--rw-r--r--   0        0        0      877 2024-03-07 09:12:09.690399 dataverk_airflow-1.6.1/pyproject.toml
--rw-r--r--   0        0        0     9295 1970-01-01 00:00:00.000000 dataverk_airflow-1.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1061 2024-04-16 08:29:00.920227 dataverk_airflow-1.6.2/LICENSE
+-rw-r--r--   0        0        0     8319 2024-04-16 08:29:00.920227 dataverk_airflow-1.6.2/README.md
+-rw-r--r--   0        0        0      381 2024-04-16 08:29:00.920227 dataverk_airflow-1.6.2/dataverk_airflow/__init__.py
+-rw-r--r--   0        0        0      752 2024-04-16 08:29:00.924227 dataverk_airflow-1.6.2/dataverk_airflow/bucket_read.py
+-rw-r--r--   0        0        0     1264 2024-04-16 08:29:00.924227 dataverk_airflow-1.6.2/dataverk_airflow/git_clone.py
+-rw-r--r--   0        0        0     9712 2024-04-16 08:29:00.924227 dataverk_airflow-1.6.2/dataverk_airflow/kubernetes_operator.py
+-rw-r--r--   0        0        0     4222 2024-04-16 08:29:00.924227 dataverk_airflow-1.6.2/dataverk_airflow/notebook_operator.py
+-rw-r--r--   0        0        0     1058 2024-04-16 08:29:00.924227 dataverk_airflow-1.6.2/dataverk_airflow/notifications.py
+-rw-r--r--   0        0        0     4051 2024-04-16 08:29:00.924227 dataverk_airflow-1.6.2/dataverk_airflow/python_operator.py
+-rw-r--r--   0        0        0     5716 2024-04-16 08:29:00.924227 dataverk_airflow-1.6.2/dataverk_airflow/quarto_operator.py
+-rw-r--r--   0        0        0      877 2024-04-16 08:29:01.184227 dataverk_airflow-1.6.2/pyproject.toml
+-rw-r--r--   0        0        0     9295 1970-01-01 00:00:00.000000 dataverk_airflow-1.6.2/PKG-INFO
```

### Comparing `dataverk_airflow-1.6.1/LICENSE` & `dataverk_airflow-1.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dataverk_airflow-1.6.1/README.md` & `dataverk_airflow-1.6.2/README.md`

 * *Files identical despite different names*

### Comparing `dataverk_airflow-1.6.1/dataverk_airflow/bucket_read.py` & `dataverk_airflow-1.6.2/dataverk_airflow/bucket_read.py`

 * *Files identical despite different names*

### Comparing `dataverk_airflow-1.6.1/dataverk_airflow/git_clone.py` & `dataverk_airflow-1.6.2/dataverk_airflow/git_clone.py`

 * *Files identical despite different names*

### Comparing `dataverk_airflow-1.6.1/dataverk_airflow/kubernetes_operator.py` & `dataverk_airflow-1.6.2/dataverk_airflow/kubernetes_operator.py`

 * *Files identical despite different names*

### Comparing `dataverk_airflow-1.6.1/dataverk_airflow/notebook_operator.py` & `dataverk_airflow-1.6.2/dataverk_airflow/notebook_operator.py`

 * *Files identical despite different names*

### Comparing `dataverk_airflow-1.6.1/dataverk_airflow/notifications.py` & `dataverk_airflow-1.6.2/dataverk_airflow/notifications.py`

 * *Files identical despite different names*

### Comparing `dataverk_airflow-1.6.1/dataverk_airflow/python_operator.py` & `dataverk_airflow-1.6.2/dataverk_airflow/python_operator.py`

 * *Files identical despite different names*

### Comparing `dataverk_airflow-1.6.1/dataverk_airflow/quarto_operator.py` & `dataverk_airflow-1.6.2/dataverk_airflow/quarto_operator.py`

 * *Files identical despite different names*

### Comparing `dataverk_airflow-1.6.1/pyproject.toml` & `dataverk_airflow-1.6.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dataverk-airflow"
-version = "1.6.1"
+version = "1.6.2"
 description = ""
 authors = ["NAV", "NADA"]
 readme = "README.md"
 packages = [{include = "dataverk_airflow"}]
 repository = "https://github.com/navikt/dataverk-airflow"
 classifiers = [
   'Development Status :: 5 - Production/Stable',
```

### Comparing `dataverk_airflow-1.6.1/PKG-INFO` & `dataverk_airflow-1.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataverk-airflow
-Version: 1.6.1
+Version: 1.6.2
 Summary: 
 Home-page: https://github.com/navikt/dataverk-airflow
 Author: NAV
 Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Apache Airflow
 Classifier: Framework :: Apache Airflow :: Provider
```

