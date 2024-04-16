# Comparing `tmp/airflow-clickhouse-plugin-1.2.0.tar.gz` & `tmp/airflow_clickhouse_plugin-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airflow-clickhouse-plugin-1.2.0.tar", last modified: Fri Mar  1 17:51:41 2024, max compression
+gzip compressed data, was "airflow_clickhouse_plugin-1.3.0.tar", last modified: Tue Apr 16 13:08:26 2024, max compression
```

## Comparing `airflow-clickhouse-plugin-1.2.0.tar` & `airflow_clickhouse_plugin-1.3.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 17:51:41.420319 airflow-clickhouse-plugin-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-03-01 17:51:36.000000 airflow-clickhouse-plugin-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    23641 2024-03-01 17:51:41.420319 airflow-clickhouse-plugin-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    22230 2024-03-01 17:51:36.000000 airflow-clickhouse-plugin-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-03-01 17:51:36.000000 airflow-clickhouse-plugin-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-01 17:51:36.000000 airflow-clickhouse-plugin-1.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-01 17:51:41.420319 airflow-clickhouse-plugin-1.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 17:51:41.412319 airflow-clickhouse-plugin-1.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 17:51:41.416319 airflow-clickhouse-plugin-1.2.0/src/airflow_clickhouse_plugin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 17:51:41.416319 airflow-clickhouse-plugin-1.2.0/src/airflow_clickhouse_plugin/hooks/
--rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-03-01 17:51:36.000000 airflow-clickhouse-plugin-1.2.0/src/airflow_clickhouse_plugin/hooks/clickhouse.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-03-01 17:51:36.000000 airflow-clickhouse-plugin-1.2.0/src/airflow_clickhouse_plugin/hooks/clickhouse_dbapi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 17:51:41.416319 airflow-clickhouse-plugin-1.2.0/src/airflow_clickhouse_plugin/operators/
--rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-03-01 17:51:36.000000 airflow-clickhouse-plugin-1.2.0/src/airflow_clickhouse_plugin/operators/clickhouse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-03-01 17:51:36.000000 airflow-clickhouse-plugin-1.2.0/src/airflow_clickhouse_plugin/operators/clickhouse_dbapi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 17:51:41.416319 airflow-clickhouse-plugin-1.2.0/src/airflow_clickhouse_plugin/sensors/
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-03-01 17:51:36.000000 airflow-clickhouse-plugin-1.2.0/src/airflow_clickhouse_plugin/sensors/clickhouse.py
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-03-01 17:51:36.000000 airflow-clickhouse-plugin-1.2.0/src/airflow_clickhouse_plugin/sensors/clickhouse_dbapi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 17:51:41.416319 airflow-clickhouse-plugin-1.2.0/src/airflow_clickhouse_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    23641 2024-03-01 17:51:41.000000 airflow-clickhouse-plugin-1.2.0/src/airflow_clickhouse_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-03-01 17:51:41.000000 airflow-clickhouse-plugin-1.2.0/src/airflow_clickhouse_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 17:51:41.000000 airflow-clickhouse-plugin-1.2.0/src/airflow_clickhouse_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-03-01 17:51:41.000000 airflow-clickhouse-plugin-1.2.0/src/airflow_clickhouse_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-01 17:51:41.000000 airflow-clickhouse-plugin-1.2.0/src/airflow_clickhouse_plugin.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:08:26.895722 airflow_clickhouse_plugin-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-16 13:08:23.000000 airflow_clickhouse_plugin-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    23786 2024-04-16 13:08:26.895722 airflow_clickhouse_plugin-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    22373 2024-04-16 13:08:23.000000 airflow_clickhouse_plugin-1.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-04-16 13:08:23.000000 airflow_clickhouse_plugin-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-16 13:08:23.000000 airflow_clickhouse_plugin-1.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 13:08:26.895722 airflow_clickhouse_plugin-1.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:08:26.891722 airflow_clickhouse_plugin-1.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:08:26.891722 airflow_clickhouse_plugin-1.3.0/src/airflow_clickhouse_plugin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:08:26.895722 airflow_clickhouse_plugin-1.3.0/src/airflow_clickhouse_plugin/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-04-16 13:08:23.000000 airflow_clickhouse_plugin-1.3.0/src/airflow_clickhouse_plugin/hooks/clickhouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-16 13:08:23.000000 airflow_clickhouse_plugin-1.3.0/src/airflow_clickhouse_plugin/hooks/clickhouse_dbapi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:08:26.895722 airflow_clickhouse_plugin-1.3.0/src/airflow_clickhouse_plugin/operators/
+-rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-04-16 13:08:23.000000 airflow_clickhouse_plugin-1.3.0/src/airflow_clickhouse_plugin/operators/clickhouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-04-16 13:08:23.000000 airflow_clickhouse_plugin-1.3.0/src/airflow_clickhouse_plugin/operators/clickhouse_dbapi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:08:26.895722 airflow_clickhouse_plugin-1.3.0/src/airflow_clickhouse_plugin/sensors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-16 13:08:23.000000 airflow_clickhouse_plugin-1.3.0/src/airflow_clickhouse_plugin/sensors/clickhouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-16 13:08:23.000000 airflow_clickhouse_plugin-1.3.0/src/airflow_clickhouse_plugin/sensors/clickhouse_dbapi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:08:26.895722 airflow_clickhouse_plugin-1.3.0/src/airflow_clickhouse_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    23786 2024-04-16 13:08:26.000000 airflow_clickhouse_plugin-1.3.0/src/airflow_clickhouse_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-16 13:08:26.000000 airflow_clickhouse_plugin-1.3.0/src/airflow_clickhouse_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 13:08:26.000000 airflow_clickhouse_plugin-1.3.0/src/airflow_clickhouse_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-16 13:08:26.000000 airflow_clickhouse_plugin-1.3.0/src/airflow_clickhouse_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-16 13:08:26.000000 airflow_clickhouse_plugin-1.3.0/src/airflow_clickhouse_plugin.egg-info/top_level.txt
```

### Comparing `airflow-clickhouse-plugin-1.2.0/LICENSE` & `airflow_clickhouse_plugin-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `airflow-clickhouse-plugin-1.2.0/PKG-INFO` & `airflow_clickhouse_plugin-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow-clickhouse-plugin
-Version: 1.2.0
+Version: 1.3.0
 Summary: airflow-clickhouse-plugin — Airflow plugin to execute ClickHouse commands and queries
 Author-email: "Anton Bryzgalov, Viktor Taranenko" <tony.bryzgaloff@gmail.com>
 License: MIT License
 Project-URL: GitHub, https://github.com/bryzgaloff/airflow-clickhouse-plugin
 Project-URL: Documentation, https://github.com/bryzgaloff/airflow-clickhouse-plugin#airflow-clickhouse-plugin
 Project-URL: Changelog, https://github.com/bryzgaloff/airflow-clickhouse-plugin/releases
 Project-URL: Issues, https://github.com/bryzgaloff/airflow-clickhouse-plugin/issues
@@ -16,17 +16,17 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: clickhouse-driver~=0.2.0
-Requires-Dist: apache-airflow<2.9.0,>=2.0.0
+Requires-Dist: apache-airflow<2.10.0,>=2.0.0
 Provides-Extra: common-sql
-Requires-Dist: apache-airflow[common.sql]<2.9.0,>=2.2.0; extra == "common-sql"
+Requires-Dist: apache-airflow[common.sql]<2.10.0,>=2.2.0; extra == "common-sql"
 Requires-Dist: apache-airflow-providers-common-sql>=1.3.0; extra == "common-sql"
 Requires-Dist: clickhouse-driver>=0.2.1; extra == "common-sql"
 
 # Airflow ClickHouse Plugin
 
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/airflow-clickhouse-plugin)
 ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/bryzgaloff/airflow-clickhouse-plugin/tests.yml?branch=master)
@@ -90,14 +90,15 @@
 
 ## Python and Airflow versions support
 
 Different versions of the plugin support different combinations of Python and Airflow versions. We _primarily_ support **Airflow 2.0+ and Python 3.8+**. If you need to use the plugin with older Python-Airflow combinations, pick a suitable plugin version:
 
 | airflow-clickhouse-plugin version | Airflow version         | Python version     |
 |-----------------------------------|-------------------------|--------------------|
+| 1.3.0                             | \>=2.0.0,<2.10.0        | ~=3.8              |
 | 1.2.0                             | \>=2.0.0,<2.9.0         | ~=3.8              |
 | 1.1.0                             | \>=2.0.0,<2.8.0         | ~=3.8              |
 | 1.0.0                             | \>=2.0.0,<2.7.0         | ~=3.8              |
 | 0.11.0                            | ~=2.0.0,\>=2.2.0,<2.7.0 | ~=3.7              |
 | 0.10.0,0.10.1                     | ~=2.0.0,\>=2.2.0,<2.6.0 | ~=3.7              |
 | 0.9.0,0.9.1                       | ~=2.0.0,\>=2.2.0,<2.5.0 | ~=3.7              |
 | 0.8.2                             | \>=2.0.0,<2.4.0         | ~=3.7              |
@@ -408,14 +409,15 @@
 * [@was-av](https://github.com/was-av)
 * Maxim Tarasov, [@MaximTar](https://github.com/MaximTar)
 * [@dvnrvn](https://github.com/dvnrvn)
 * Giovanni Corsetti, [@CorsettiS](https://github.com/CorsettiS)
 * Dmytro Zhyzniev, [@1ng4lipt](https://github.com/1ng4lipt)
 * Anton Bezdenezhnykh, [@GaMeRaM](https://github.com/GaMeRaM)
 * Andrey, [@bobelev](https://github.com/bobelev)
+* Misha Epikhin, [@epikhinm](https://github.com/epikhinm)
 
 
 [airflow]: https://airflow.apache.org/
 [ch-driver]: https://github.com/mymarilyn/clickhouse-driver
 [ch-driver-docs]: https://clickhouse-driver.readthedocs.io/en/latest/
 [ch-driver-execute-summary]: https://clickhouse-driver.readthedocs.io/en/latest/quickstart.html#selecting-data
 [ch-driver-execute-reference]: https://clickhouse-driver.readthedocs.io/en/latest/api.html#clickhouse_driver.Client.execute
```

### Comparing `airflow-clickhouse-plugin-1.2.0/README.md` & `airflow_clickhouse_plugin-1.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -62,14 +62,15 @@
 
 ## Python and Airflow versions support
 
 Different versions of the plugin support different combinations of Python and Airflow versions. We _primarily_ support **Airflow 2.0+ and Python 3.8+**. If you need to use the plugin with older Python-Airflow combinations, pick a suitable plugin version:
 
 | airflow-clickhouse-plugin version | Airflow version         | Python version     |
 |-----------------------------------|-------------------------|--------------------|
+| 1.3.0                             | \>=2.0.0,<2.10.0        | ~=3.8              |
 | 1.2.0                             | \>=2.0.0,<2.9.0         | ~=3.8              |
 | 1.1.0                             | \>=2.0.0,<2.8.0         | ~=3.8              |
 | 1.0.0                             | \>=2.0.0,<2.7.0         | ~=3.8              |
 | 0.11.0                            | ~=2.0.0,\>=2.2.0,<2.7.0 | ~=3.7              |
 | 0.10.0,0.10.1                     | ~=2.0.0,\>=2.2.0,<2.6.0 | ~=3.7              |
 | 0.9.0,0.9.1                       | ~=2.0.0,\>=2.2.0,<2.5.0 | ~=3.7              |
 | 0.8.2                             | \>=2.0.0,<2.4.0         | ~=3.7              |
@@ -380,14 +381,15 @@
 * [@was-av](https://github.com/was-av)
 * Maxim Tarasov, [@MaximTar](https://github.com/MaximTar)
 * [@dvnrvn](https://github.com/dvnrvn)
 * Giovanni Corsetti, [@CorsettiS](https://github.com/CorsettiS)
 * Dmytro Zhyzniev, [@1ng4lipt](https://github.com/1ng4lipt)
 * Anton Bezdenezhnykh, [@GaMeRaM](https://github.com/GaMeRaM)
 * Andrey, [@bobelev](https://github.com/bobelev)
+* Misha Epikhin, [@epikhinm](https://github.com/epikhinm)
 
 
 [airflow]: https://airflow.apache.org/
 [ch-driver]: https://github.com/mymarilyn/clickhouse-driver
 [ch-driver-docs]: https://clickhouse-driver.readthedocs.io/en/latest/
 [ch-driver-execute-summary]: https://clickhouse-driver.readthedocs.io/en/latest/quickstart.html#selecting-data
 [ch-driver-execute-reference]: https://clickhouse-driver.readthedocs.io/en/latest/api.html#clickhouse_driver.Client.execute
```

### Comparing `airflow-clickhouse-plugin-1.2.0/pyproject.toml` & `airflow_clickhouse_plugin-1.3.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "setuptools",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "airflow-clickhouse-plugin"
-version = "1.2.0"
+version = "1.3.0"
 description = "airflow-clickhouse-plugin — Airflow plugin to execute ClickHouse commands and queries"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { text = "MIT License" }
 authors = [
     { name = "Anton Bryzgalov, Viktor Taranenko", email = "tony.bryzgaloff@gmail.com" },
 ]
@@ -35,15 +35,15 @@
 GitHub = "https://github.com/bryzgaloff/airflow-clickhouse-plugin"
 Documentation = "https://github.com/bryzgaloff/airflow-clickhouse-plugin#airflow-clickhouse-plugin"
 Changelog = "https://github.com/bryzgaloff/airflow-clickhouse-plugin/releases"
 Issues = "https://github.com/bryzgaloff/airflow-clickhouse-plugin/issues"
 
 [project.optional-dependencies]
 "common.sql" = [
-    "apache-airflow[common.sql]>=2.2.0,<2.9.0",
+    "apache-airflow[common.sql]>=2.2.0,<2.10.0",
     "apache-airflow-providers-common-sql>=1.3.0",  # introduces SQLExecuteQueryOperator
     "clickhouse-driver>=0.2.1",
 ]
 
 [tool.setuptools.dynamic]
 dependencies = { file = ["requirements.txt"] }
```

### Comparing `airflow-clickhouse-plugin-1.2.0/src/airflow_clickhouse_plugin/hooks/clickhouse.py` & `airflow_clickhouse_plugin-1.3.0/src/airflow_clickhouse_plugin/hooks/clickhouse.py`

 * *Files identical despite different names*

### Comparing `airflow-clickhouse-plugin-1.2.0/src/airflow_clickhouse_plugin/hooks/clickhouse_dbapi.py` & `airflow_clickhouse_plugin-1.3.0/src/airflow_clickhouse_plugin/hooks/clickhouse_dbapi.py`

 * *Files identical despite different names*

### Comparing `airflow-clickhouse-plugin-1.2.0/src/airflow_clickhouse_plugin/operators/clickhouse.py` & `airflow_clickhouse_plugin-1.3.0/src/airflow_clickhouse_plugin/operators/clickhouse.py`

 * *Files identical despite different names*

### Comparing `airflow-clickhouse-plugin-1.2.0/src/airflow_clickhouse_plugin/operators/clickhouse_dbapi.py` & `airflow_clickhouse_plugin-1.3.0/src/airflow_clickhouse_plugin/operators/clickhouse_dbapi.py`

 * *Files identical despite different names*

### Comparing `airflow-clickhouse-plugin-1.2.0/src/airflow_clickhouse_plugin/sensors/clickhouse.py` & `airflow_clickhouse_plugin-1.3.0/src/airflow_clickhouse_plugin/sensors/clickhouse.py`

 * *Files identical despite different names*

### Comparing `airflow-clickhouse-plugin-1.2.0/src/airflow_clickhouse_plugin.egg-info/PKG-INFO` & `airflow_clickhouse_plugin-1.3.0/src/airflow_clickhouse_plugin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow-clickhouse-plugin
-Version: 1.2.0
+Version: 1.3.0
 Summary: airflow-clickhouse-plugin — Airflow plugin to execute ClickHouse commands and queries
 Author-email: "Anton Bryzgalov, Viktor Taranenko" <tony.bryzgaloff@gmail.com>
 License: MIT License
 Project-URL: GitHub, https://github.com/bryzgaloff/airflow-clickhouse-plugin
 Project-URL: Documentation, https://github.com/bryzgaloff/airflow-clickhouse-plugin#airflow-clickhouse-plugin
 Project-URL: Changelog, https://github.com/bryzgaloff/airflow-clickhouse-plugin/releases
 Project-URL: Issues, https://github.com/bryzgaloff/airflow-clickhouse-plugin/issues
@@ -16,17 +16,17 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: clickhouse-driver~=0.2.0
-Requires-Dist: apache-airflow<2.9.0,>=2.0.0
+Requires-Dist: apache-airflow<2.10.0,>=2.0.0
 Provides-Extra: common-sql
-Requires-Dist: apache-airflow[common.sql]<2.9.0,>=2.2.0; extra == "common-sql"
+Requires-Dist: apache-airflow[common.sql]<2.10.0,>=2.2.0; extra == "common-sql"
 Requires-Dist: apache-airflow-providers-common-sql>=1.3.0; extra == "common-sql"
 Requires-Dist: clickhouse-driver>=0.2.1; extra == "common-sql"
 
 # Airflow ClickHouse Plugin
 
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/airflow-clickhouse-plugin)
 ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/bryzgaloff/airflow-clickhouse-plugin/tests.yml?branch=master)
@@ -90,14 +90,15 @@
 
 ## Python and Airflow versions support
 
 Different versions of the plugin support different combinations of Python and Airflow versions. We _primarily_ support **Airflow 2.0+ and Python 3.8+**. If you need to use the plugin with older Python-Airflow combinations, pick a suitable plugin version:
 
 | airflow-clickhouse-plugin version | Airflow version         | Python version     |
 |-----------------------------------|-------------------------|--------------------|
+| 1.3.0                             | \>=2.0.0,<2.10.0        | ~=3.8              |
 | 1.2.0                             | \>=2.0.0,<2.9.0         | ~=3.8              |
 | 1.1.0                             | \>=2.0.0,<2.8.0         | ~=3.8              |
 | 1.0.0                             | \>=2.0.0,<2.7.0         | ~=3.8              |
 | 0.11.0                            | ~=2.0.0,\>=2.2.0,<2.7.0 | ~=3.7              |
 | 0.10.0,0.10.1                     | ~=2.0.0,\>=2.2.0,<2.6.0 | ~=3.7              |
 | 0.9.0,0.9.1                       | ~=2.0.0,\>=2.2.0,<2.5.0 | ~=3.7              |
 | 0.8.2                             | \>=2.0.0,<2.4.0         | ~=3.7              |
@@ -408,14 +409,15 @@
 * [@was-av](https://github.com/was-av)
 * Maxim Tarasov, [@MaximTar](https://github.com/MaximTar)
 * [@dvnrvn](https://github.com/dvnrvn)
 * Giovanni Corsetti, [@CorsettiS](https://github.com/CorsettiS)
 * Dmytro Zhyzniev, [@1ng4lipt](https://github.com/1ng4lipt)
 * Anton Bezdenezhnykh, [@GaMeRaM](https://github.com/GaMeRaM)
 * Andrey, [@bobelev](https://github.com/bobelev)
+* Misha Epikhin, [@epikhinm](https://github.com/epikhinm)
 
 
 [airflow]: https://airflow.apache.org/
 [ch-driver]: https://github.com/mymarilyn/clickhouse-driver
 [ch-driver-docs]: https://clickhouse-driver.readthedocs.io/en/latest/
 [ch-driver-execute-summary]: https://clickhouse-driver.readthedocs.io/en/latest/quickstart.html#selecting-data
 [ch-driver-execute-reference]: https://clickhouse-driver.readthedocs.io/en/latest/api.html#clickhouse_driver.Client.execute
```

### Comparing `airflow-clickhouse-plugin-1.2.0/src/airflow_clickhouse_plugin.egg-info/SOURCES.txt` & `airflow_clickhouse_plugin-1.3.0/src/airflow_clickhouse_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

