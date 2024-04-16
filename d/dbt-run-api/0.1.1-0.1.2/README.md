# Comparing `tmp/dbt_run_api-0.1.1.tar.gz` & `tmp/dbt_run_api-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_run_api-0.1.1.tar", max compression
+gzip compressed data, was "dbt_run_api-0.1.2.tar", max compression
```

## Comparing `dbt_run_api-0.1.1.tar` & `dbt_run_api-0.1.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     1060 2024-04-12 12:22:01.064012 dbt_run_api-0.1.1/LICENSE
--rw-r--r--   0        0        0     1059 2024-04-12 12:22:01.064012 dbt_run_api-0.1.1/dbt_run_api/__init__.py
--rw-r--r--   0        0        0      346 2024-04-12 12:22:01.064012 dbt_run_api-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      495 1970-01-01 00:00:00.000000 dbt_run_api-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1060 2024-04-16 09:53:12.558606 dbt_run_api-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1059 2024-04-16 09:53:12.558606 dbt_run_api-0.1.2/dbt_run_api/__init__.py
+-rw-r--r--   0        0        0      346 2024-04-16 09:53:12.558606 dbt_run_api-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      495 1970-01-01 00:00:00.000000 dbt_run_api-0.1.2/PKG-INFO
```

### Comparing `dbt_run_api-0.1.1/LICENSE` & `dbt_run_api-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_run_api-0.1.1/dbt_run_api/__init__.py` & `dbt_run_api-0.1.2/dbt_run_api/__init__.py`

 * *Files identical despite different names*

