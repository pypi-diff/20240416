# Comparing `tmp/reflex_hosting_cli-0.1.8.tar.gz` & `tmp/reflex_hosting_cli-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reflex_hosting_cli-0.1.8.tar", max compression
+gzip compressed data, was "reflex_hosting_cli-0.1.9.tar", max compression
```

## Comparing `reflex_hosting_cli-0.1.8.tar` & `reflex_hosting_cli-0.1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    11358 2023-12-04 23:51:41.799351 reflex_hosting_cli-0.1.8/LICENSE
--rw-r--r--   0        0        0       45 2023-11-03 21:55:30.491137 reflex_hosting_cli-0.1.8/README.md
--rw-r--r--   0        0        0     1673 2024-02-09 17:56:53.711961 reflex_hosting_cli-0.1.8/pyproject.toml
--rw-r--r--   0        0        0       43 2023-12-04 23:51:41.800614 reflex_hosting_cli-0.1.8/reflex_cli/__init__.py
--rw-r--r--   0        0        0    11890 2024-01-31 22:53:29.414708 reflex_hosting_cli-0.1.8/reflex_cli/cli.py
--rw-r--r--   0        0        0      255 2024-01-31 22:53:29.415820 reflex_hosting_cli-0.1.8/reflex_cli/constants/__init__.py
--rw-r--r--   0        0        0     1270 2023-12-04 23:51:41.801328 reflex_hosting_cli-0.1.8/reflex_cli/constants/base.py
--rw-r--r--   0        0        0      664 2023-12-04 23:51:41.801627 reflex_hosting_cli-0.1.8/reflex_cli/constants/compiler.py
--rw-r--r--   0        0        0     1585 2024-01-31 22:53:29.416159 reflex_hosting_cli-0.1.8/reflex_cli/constants/hosting.py
--rw-r--r--   0        0        0    10597 2024-01-31 22:53:29.416640 reflex_hosting_cli-0.1.8/reflex_cli/deployments.py
--rw-r--r--   0        0        0       24 2023-12-04 23:51:41.802162 reflex_hosting_cli-0.1.8/reflex_cli/utils/__init__.py
--rw-r--r--   0        0        0     3625 2023-12-05 19:48:55.837351 reflex_hosting_cli-0.1.8/reflex_cli/utils/console.py
--rw-r--r--   0        0        0     6619 2024-01-31 22:53:29.416956 reflex_hosting_cli-0.1.8/reflex_cli/utils/dependency.py
--rw-r--r--   0        0        0    66881 2024-01-31 22:53:29.417666 reflex_hosting_cli-0.1.8/reflex_cli/utils/hosting.py
--rw-r--r--   0        0        0     1335 1970-01-01 00:00:00.000000 reflex_hosting_cli-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-12-04 23:51:41.799351 reflex_hosting_cli-0.1.9/LICENSE
+-rw-r--r--   0        0        0       45 2023-11-03 21:55:30.491137 reflex_hosting_cli-0.1.9/README.md
+-rw-r--r--   0        0        0     1692 2024-03-15 06:33:37.935475 reflex_hosting_cli-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0       43 2023-12-04 23:51:41.800614 reflex_hosting_cli-0.1.9/reflex_cli/__init__.py
+-rw-r--r--   0        0        0    11890 2024-01-31 22:53:29.414708 reflex_hosting_cli-0.1.9/reflex_cli/cli.py
+-rw-r--r--   0        0        0      255 2024-01-31 22:53:29.415820 reflex_hosting_cli-0.1.9/reflex_cli/constants/__init__.py
+-rw-r--r--   0        0        0     1270 2023-12-04 23:51:41.801328 reflex_hosting_cli-0.1.9/reflex_cli/constants/base.py
+-rw-r--r--   0        0        0      664 2023-12-04 23:51:41.801627 reflex_hosting_cli-0.1.9/reflex_cli/constants/compiler.py
+-rw-r--r--   0        0        0     1585 2024-01-31 22:53:29.416159 reflex_hosting_cli-0.1.9/reflex_cli/constants/hosting.py
+-rw-r--r--   0        0        0    10597 2024-01-31 22:53:29.416640 reflex_hosting_cli-0.1.9/reflex_cli/deployments.py
+-rw-r--r--   0        0        0       24 2023-12-04 23:51:41.802162 reflex_hosting_cli-0.1.9/reflex_cli/utils/__init__.py
+-rw-r--r--   0        0        0     3625 2023-12-05 19:48:55.837351 reflex_hosting_cli-0.1.9/reflex_cli/utils/console.py
+-rw-r--r--   0        0        0     6619 2024-01-31 22:53:29.416956 reflex_hosting_cli-0.1.9/reflex_cli/utils/dependency.py
+-rw-r--r--   0        0        0    66881 2024-01-31 22:53:29.417666 reflex_hosting_cli-0.1.9/reflex_cli/utils/hosting.py
+-rw-r--r--   0        0        0     1327 1970-01-01 00:00:00.000000 reflex_hosting_cli-0.1.9/PKG-INFO
```

### Comparing `reflex_hosting_cli-0.1.8/LICENSE` & `reflex_hosting_cli-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `reflex_hosting_cli-0.1.8/reflex_cli/cli.py` & `reflex_hosting_cli-0.1.9/reflex_cli/cli.py`

 * *Files identical despite different names*

### Comparing `reflex_hosting_cli-0.1.8/reflex_cli/constants/base.py` & `reflex_hosting_cli-0.1.9/reflex_cli/constants/base.py`

 * *Files identical despite different names*

### Comparing `reflex_hosting_cli-0.1.8/reflex_cli/constants/compiler.py` & `reflex_hosting_cli-0.1.9/reflex_cli/constants/compiler.py`

 * *Files identical despite different names*

### Comparing `reflex_hosting_cli-0.1.8/reflex_cli/constants/hosting.py` & `reflex_hosting_cli-0.1.9/reflex_cli/constants/hosting.py`

 * *Files identical despite different names*

### Comparing `reflex_hosting_cli-0.1.8/reflex_cli/deployments.py` & `reflex_hosting_cli-0.1.9/reflex_cli/deployments.py`

 * *Files identical despite different names*

### Comparing `reflex_hosting_cli-0.1.8/reflex_cli/utils/console.py` & `reflex_hosting_cli-0.1.9/reflex_cli/utils/console.py`

 * *Files identical despite different names*

### Comparing `reflex_hosting_cli-0.1.8/reflex_cli/utils/dependency.py` & `reflex_hosting_cli-0.1.9/reflex_cli/utils/dependency.py`

 * *Files identical despite different names*

### Comparing `reflex_hosting_cli-0.1.8/reflex_cli/utils/hosting.py` & `reflex_hosting_cli-0.1.9/reflex_cli/utils/hosting.py`

 * *Files identical despite different names*

### Comparing `reflex_hosting_cli-0.1.8/PKG-INFO` & `reflex_hosting_cli-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reflex-hosting-cli
-Version: 0.1.8
+Version: 0.1.9
 Summary: Reflex Hosting CLI
 Home-page: https://reflex.dev
 License: Apache-2.0
 Keywords: web,framework
 Author: Nikhil Rao
 Author-email: nikhil@reflex.dev
 Requires-Python: >=3.8,<4.0
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: charset-normalizer (>=3.3.2,<4.0.0)
-Requires-Dist: httpx (>=0.24.0,<0.26.0)
+Requires-Dist: httpx (>=0.25.1)
 Requires-Dist: pipdeptree (>=2.13.1,<3.0.0)
 Requires-Dist: pipreqs (>=0.4.13,<0.5.0)
 Requires-Dist: platformdirs (>=3.10.0,<4.0.0)
 Requires-Dist: pydantic (>=1.10.2,<2.0.0)
 Requires-Dist: python-dateutil (>=2.8.1)
 Requires-Dist: rich (>=13.0.0,<14.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
```

