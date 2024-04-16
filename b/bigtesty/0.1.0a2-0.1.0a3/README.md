# Comparing `tmp/bigtesty-0.1.0a2.tar.gz` & `tmp/bigtesty-0.1.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigtesty-0.1.0a2.tar", last modified: Wed Apr  3 16:55:11 2024, max compression
+gzip compressed data, was "bigtesty-0.1.0a3.tar", last modified: Tue Apr 16 18:25:02 2024, max compression
```

## Comparing `bigtesty-0.1.0a2.tar` & `bigtesty-0.1.0a3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:55:11.325067 bigtesty-0.1.0a2/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-03 16:54:55.000000 bigtesty-0.1.0a2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-03 16:55:11.325067 bigtesty-0.1.0a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-03 16:54:55.000000 bigtesty-0.1.0a2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:55:11.325067 bigtesty-0.1.0a2/bigtesty/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:54:55.000000 bigtesty-0.1.0a2/bigtesty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-03 16:54:55.000000 bigtesty-0.1.0a2/bigtesty/arguments.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:55:11.325067 bigtesty-0.1.0a2/bigtesty/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:54:55.000000 bigtesty-0.1.0a2/bigtesty/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-03 16:54:55.000000 bigtesty-0.1.0a2/bigtesty/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-03 16:54:55.000000 bigtesty-0.1.0a2/bigtesty/dataset_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-03 16:54:55.000000 bigtesty-0.1.0a2/bigtesty/definition_test_config_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-03 16:54:55.000000 bigtesty-0.1.0a2/bigtesty/definition_test_file_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-03 16:54:55.000000 bigtesty-0.1.0a2/bigtesty/files_loader_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:55:11.325067 bigtesty-0.1.0a2/bigtesty/given/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:54:55.000000 bigtesty-0.1.0a2/bigtesty/given/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-03 16:54:55.000000 bigtesty-0.1.0a2/bigtesty/given/insertion_test_data_bigquery.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:55:11.325067 bigtesty-0.1.0a2/bigtesty/infra/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:54:55.000000 bigtesty-0.1.0a2/bigtesty/infra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-04-03 16:54:55.000000 bigtesty-0.1.0a2/bigtesty/infra/create_iac_for_datasets_with_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-03 16:54:55.000000 bigtesty-0.1.0a2/bigtesty/infra/datasets_with_tables_config_file_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-03 16:54:55.000000 bigtesty-0.1.0a2/bigtesty/infra/datasets_with_tables_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-04-03 16:54:55.000000 bigtesty-0.1.0a2/bigtesty/infra/launch_tests_ephemeral_infra.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-03 16:54:55.000000 bigtesty-0.1.0a2/bigtesty/lambda_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:55:11.325067 bigtesty-0.1.0a2/bigtesty/then/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:54:55.000000 bigtesty-0.1.0a2/bigtesty/then/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4659 2024-04-03 16:54:55.000000 bigtesty-0.1.0a2/bigtesty/then/assertion_and_tests_reports_result.py
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-03 16:54:55.000000 bigtesty-0.1.0a2/bigtesty/then/failure_test_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:55:11.325067 bigtesty-0.1.0a2/bigtesty.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-03 16:55:11.000000 bigtesty-0.1.0a2/bigtesty.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-03 16:55:11.000000 bigtesty-0.1.0a2/bigtesty.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 16:55:11.000000 bigtesty-0.1.0a2/bigtesty.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-03 16:55:11.000000 bigtesty-0.1.0a2/bigtesty.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-03 16:55:11.000000 bigtesty-0.1.0a2/bigtesty.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-03 16:55:11.000000 bigtesty-0.1.0a2/bigtesty.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 16:55:11.325067 bigtesty-0.1.0a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-03 16:54:55.000000 bigtesty-0.1.0a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:25:02.707820 bigtesty-0.1.0a3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-16 18:24:48.000000 bigtesty-0.1.0a3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-16 18:25:02.707820 bigtesty-0.1.0a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-16 18:24:48.000000 bigtesty-0.1.0a3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:25:02.707820 bigtesty-0.1.0a3/bigtesty/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 18:24:48.000000 bigtesty-0.1.0a3/bigtesty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-16 18:24:48.000000 bigtesty-0.1.0a3/bigtesty/arguments.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:25:02.707820 bigtesty-0.1.0a3/bigtesty/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 18:24:48.000000 bigtesty-0.1.0a3/bigtesty/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-16 18:24:48.000000 bigtesty-0.1.0a3/bigtesty/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-16 18:24:48.000000 bigtesty-0.1.0a3/bigtesty/dataset_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-16 18:24:48.000000 bigtesty-0.1.0a3/bigtesty/definition_test_config_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-16 18:24:48.000000 bigtesty-0.1.0a3/bigtesty/definition_test_file_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-16 18:24:48.000000 bigtesty-0.1.0a3/bigtesty/files_loader_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:25:02.707820 bigtesty-0.1.0a3/bigtesty/given/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 18:24:48.000000 bigtesty-0.1.0a3/bigtesty/given/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-16 18:24:48.000000 bigtesty-0.1.0a3/bigtesty/given/insertion_test_data_bigquery.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:25:02.707820 bigtesty-0.1.0a3/bigtesty/infra/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 18:24:48.000000 bigtesty-0.1.0a3/bigtesty/infra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-04-16 18:24:48.000000 bigtesty-0.1.0a3/bigtesty/infra/create_iac_for_datasets_with_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-16 18:24:48.000000 bigtesty-0.1.0a3/bigtesty/infra/datasets_with_tables_config_file_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-16 18:24:48.000000 bigtesty-0.1.0a3/bigtesty/infra/datasets_with_tables_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-04-16 18:24:48.000000 bigtesty-0.1.0a3/bigtesty/infra/launch_tests_ephemeral_infra.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-16 18:24:48.000000 bigtesty-0.1.0a3/bigtesty/lambda_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:25:02.707820 bigtesty-0.1.0a3/bigtesty/then/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 18:24:48.000000 bigtesty-0.1.0a3/bigtesty/then/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4659 2024-04-16 18:24:48.000000 bigtesty-0.1.0a3/bigtesty/then/assertion_and_tests_reports_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-16 18:24:48.000000 bigtesty-0.1.0a3/bigtesty/then/failure_test_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:25:02.707820 bigtesty-0.1.0a3/bigtesty.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-16 18:25:02.000000 bigtesty-0.1.0a3/bigtesty.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-16 18:25:02.000000 bigtesty-0.1.0a3/bigtesty.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 18:25:02.000000 bigtesty-0.1.0a3/bigtesty.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-16 18:25:02.000000 bigtesty-0.1.0a3/bigtesty.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-16 18:25:02.000000 bigtesty-0.1.0a3/bigtesty.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-16 18:25:02.000000 bigtesty-0.1.0a3/bigtesty.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 18:25:02.707820 bigtesty-0.1.0a3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-16 18:24:48.000000 bigtesty-0.1.0a3/setup.py
```

### Comparing `bigtesty-0.1.0a2/LICENSE` & `bigtesty-0.1.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `bigtesty-0.1.0a2/PKG-INFO` & `bigtesty-0.1.0a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigtesty
-Version: 0.1.0a2
+Version: 0.1.0a3
 Summary: BigTesty is an integration testing framework for BigQuery
 Home-page: https://github.com/tosun-si/bigtesty
 Author: Mazlum TOSUN
 Author-email: mazlum.tosun@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bigtesty-0.1.0a2/README.md` & `bigtesty-0.1.0a3/README.md`

 * *Files identical despite different names*

### Comparing `bigtesty-0.1.0a2/bigtesty/cli/main.py` & `bigtesty-0.1.0a3/bigtesty/cli/main.py`

 * *Files identical despite different names*

### Comparing `bigtesty-0.1.0a2/bigtesty/definition_test_config_helper.py` & `bigtesty-0.1.0a3/bigtesty/definition_test_config_helper.py`

 * *Files identical despite different names*

### Comparing `bigtesty-0.1.0a2/bigtesty/given/insertion_test_data_bigquery.py` & `bigtesty-0.1.0a3/bigtesty/given/insertion_test_data_bigquery.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 def insert_test_data_to_bq_tables(
         project_id: str,
         root_test_folder: str,
         datasets_hash: str,
         scenarios: List[Dict]) -> None:
     client = bigquery.Client(project=project_id)
 
+    raise ValueError("Error, missing required value")
+
     for scenario in scenarios:
         for given in scenario['given']:
             print("###### GIVEN")
             print(given)
 
             input_file_path = f"{root_test_folder}/{given['input_file_path']}"
             input = given.get('input')
```

### Comparing `bigtesty-0.1.0a2/bigtesty/infra/create_iac_for_datasets_with_tables.py` & `bigtesty-0.1.0a3/bigtesty/infra/create_iac_for_datasets_with_tables.py`

 * *Files identical despite different names*

### Comparing `bigtesty-0.1.0a2/bigtesty/infra/datasets_with_tables_config_file_loader.py` & `bigtesty-0.1.0a3/bigtesty/infra/datasets_with_tables_config_file_loader.py`

 * *Files identical despite different names*

### Comparing `bigtesty-0.1.0a2/bigtesty/infra/datasets_with_tables_factory.py` & `bigtesty-0.1.0a3/bigtesty/infra/datasets_with_tables_factory.py`

 * *Files identical despite different names*

### Comparing `bigtesty-0.1.0a2/bigtesty/then/assertion_and_tests_reports_result.py` & `bigtesty-0.1.0a3/bigtesty/then/assertion_and_tests_reports_result.py`

 * *Files identical despite different names*

### Comparing `bigtesty-0.1.0a2/bigtesty.egg-info/PKG-INFO` & `bigtesty-0.1.0a3/bigtesty.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigtesty
-Version: 0.1.0a2
+Version: 0.1.0a3
 Summary: BigTesty is an integration testing framework for BigQuery
 Home-page: https://github.com/tosun-si/bigtesty
 Author: Mazlum TOSUN
 Author-email: mazlum.tosun@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bigtesty-0.1.0a2/bigtesty.egg-info/SOURCES.txt` & `bigtesty-0.1.0a3/bigtesty.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bigtesty-0.1.0a2/setup.py` & `bigtesty-0.1.0a3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # The text of the README file
 long_desc = ""
 if os.path.isfile(path):
     long_desc = path.read_text()
 
 setup(
     name="bigtesty",
-    version="0.1.0a2",
+    version="0.1.0a3",
     entry_points='''
         [console_scripts]
         bigtesty=bigtesty.cli.main:run
     ''',
     install_requires=[
         "pulumi-gcp==6.67.0",
         "google-cloud-bigquery==3.7.0",
```

