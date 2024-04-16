# Comparing `tmp/mlflow-oidc-auth-1.1.2.tar.gz` & `tmp/mlflow_oidc_auth-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlflow-oidc-auth-1.1.2.tar", last modified: Wed Apr 10 23:25:34 2024, max compression
+gzip compressed data, was "mlflow_oidc_auth-1.2.0.tar", last modified: Tue Apr 16 04:30:51 2024, max compression
```

## Comparing `mlflow-oidc-auth-1.1.2.tar` & `mlflow_oidc_auth-1.2.0.tar`

### file list

```diff
@@ -1,53 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:25:34.939401 mlflow-oidc-auth-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11328 2024-04-10 23:24:24.000000 mlflow-oidc-auth-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    17487 2024-04-10 23:25:34.939401 mlflow-oidc-auth-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-04-10 23:24:24.000000 mlflow-oidc-auth-1.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:25:34.931401 mlflow-oidc-auth-1.1.2/mlflow_oidc_auth/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-10 23:24:24.000000 mlflow-oidc-auth-1.1.2/mlflow_oidc_auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-04-10 23:24:24.000000 mlflow-oidc-auth-1.1.2/mlflow_oidc_auth/app.py
--rw-r--r--   0 runner    (1001) docker     (127)    12050 2024-04-10 23:24:24.000000 mlflow-oidc-auth-1.1.2/mlflow_oidc_auth/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-10 23:24:24.000000 mlflow-oidc-auth-1.1.2/mlflow_oidc_auth/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:25:34.935401 mlflow-oidc-auth-1.1.2/mlflow_oidc_auth/db/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 23:24:24.000000 mlflow-oidc-auth-1.1.2/mlflow_oidc_auth/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-10 23:24:24.000000 mlflow-oidc-auth-1.1.2/mlflow_oidc_auth/db/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:25:34.935401 mlflow-oidc-auth-1.1.2/mlflow_oidc_auth/db/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 23:24:24.000000 mlflow-oidc-auth-1.1.2/mlflow_oidc_auth/db/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-04-10 23:24:24.000000 mlflow-oidc-auth-1.1.2/mlflow_oidc_auth/db/migrations/alembic.ini
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-10 23:24:24.000000 mlflow-oidc-auth-1.1.2/mlflow_oidc_auth/db/migrations/env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:25:34.935401 mlflow-oidc-auth-1.1.2/mlflow_oidc_auth/db/migrations/versions/
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-10 23:24:24.000000 mlflow-oidc-auth-1.1.2/mlflow_oidc_auth/db/migrations/versions/8606fa83a998_initial_migration.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 23:24:24.000000 mlflow-oidc-auth-1.1.2/mlflow_oidc_auth/db/migrations/versions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-10 23:24:24.000000 mlflow-oidc-auth-1.1.2/mlflow_oidc_auth/db/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-04-10 23:24:24.000000 mlflow-oidc-auth-1.1.2/mlflow_oidc_auth/db/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-04-10 23:24:24.000000 mlflow-oidc-auth-1.1.2/mlflow_oidc_auth/entities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-10 23:24:24.000000 mlflow-oidc-auth-1.1.2/mlflow_oidc_auth/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-10 23:24:24.000000 mlflow-oidc-auth-1.1.2/mlflow_oidc_auth/routes.py
--rw-r--r--   0 runner    (1001) docker     (127)    10567 2024-04-10 23:24:24.000000 mlflow-oidc-auth-1.1.2/mlflow_oidc_auth/sqlalchemy_store.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:25:34.935401 mlflow-oidc-auth-1.1.2/mlflow_oidc_auth/static/
--rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-10 23:24:24.000000 mlflow-oidc-auth-1.1.2/mlflow_oidc_auth/static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     4861 2024-04-10 23:24:24.000000 mlflow-oidc-auth-1.1.2/mlflow_oidc_auth/static/style.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:25:34.935401 mlflow-oidc-auth-1.1.2/mlflow_oidc_auth/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-10 23:24:24.000000 mlflow-oidc-auth-1.1.2/mlflow_oidc_auth/templates/_footer.html
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-10 23:24:24.000000 mlflow-oidc-auth-1.1.2/mlflow_oidc_auth/templates/_head.html
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-10 23:24:24.000000 mlflow-oidc-auth-1.1.2/mlflow_oidc_auth/templates/_header.html
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-10 23:24:24.000000 mlflow-oidc-auth-1.1.2/mlflow_oidc_auth/templates/auth.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:25:34.939401 mlflow-oidc-auth-1.1.2/mlflow_oidc_auth/ui/
--rw-r--r--   0 runner    (1001) docker     (127)    17029 2024-04-10 23:25:31.000000 mlflow-oidc-auth-1.1.2/mlflow_oidc_auth/ui/398.70c7e628915a6c39.js
--rw-r--r--   0 runner    (1001) docker     (127)    17458 2024-04-10 23:25:31.000000 mlflow-oidc-auth-1.1.2/mlflow_oidc_auth/ui/3rdpartylicenses.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-04-10 23:25:31.000000 mlflow-oidc-auth-1.1.2/mlflow_oidc_auth/ui/953.94c6a01c085d9731.js
--rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-10 23:25:31.000000 mlflow-oidc-auth-1.1.2/mlflow_oidc_auth/ui/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)    12068 2024-04-10 23:25:32.000000 mlflow-oidc-auth-1.1.2/mlflow_oidc_auth/ui/index.html
--rw-r--r--   0 runner    (1001) docker     (127)   703509 2024-04-10 23:25:31.000000 mlflow-oidc-auth-1.1.2/mlflow_oidc_auth/ui/main.84383ebc03062e87.js
--rw-r--r--   0 runner    (1001) docker     (127)    35227 2024-04-10 23:25:31.000000 mlflow-oidc-auth-1.1.2/mlflow_oidc_auth/ui/polyfills.90a0049d0bf863c4.js
--rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-04-10 23:25:31.000000 mlflow-oidc-auth-1.1.2/mlflow_oidc_auth/ui/runtime.0cd10aef5e6b1db8.js
--rw-r--r--   0 runner    (1001) docker     (127)   301021 2024-04-10 23:25:31.000000 mlflow-oidc-auth-1.1.2/mlflow_oidc_auth/ui/styles.68f068b304676cf1.css
--rw-r--r--   0 runner    (1001) docker     (127)    18394 2024-04-10 23:24:24.000000 mlflow-oidc-auth-1.1.2/mlflow_oidc_auth/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:25:34.939401 mlflow-oidc-auth-1.1.2/mlflow_oidc_auth.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17487 2024-04-10 23:25:34.000000 mlflow-oidc-auth-1.1.2/mlflow_oidc_auth.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-10 23:25:34.000000 mlflow-oidc-auth-1.1.2/mlflow_oidc_auth.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 23:25:34.000000 mlflow-oidc-auth-1.1.2/mlflow_oidc_auth.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-10 23:25:34.000000 mlflow-oidc-auth-1.1.2/mlflow_oidc_auth.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-10 23:25:34.000000 mlflow-oidc-auth-1.1.2/mlflow_oidc_auth.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-10 23:25:34.000000 mlflow-oidc-auth-1.1.2/mlflow_oidc_auth.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-10 23:24:24.000000 mlflow-oidc-auth-1.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 23:25:34.939401 mlflow-oidc-auth-1.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:30:51.731897 mlflow_oidc_auth-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11328 2024-04-16 04:29:44.000000 mlflow_oidc_auth-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    17262 2024-04-16 04:30:51.731897 mlflow_oidc_auth-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-16 04:29:44.000000 mlflow_oidc_auth-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:30:51.723897 mlflow_oidc_auth-1.2.0/mlflow_oidc_auth/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-16 04:29:44.000000 mlflow_oidc_auth-1.2.0/mlflow_oidc_auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-04-16 04:29:44.000000 mlflow_oidc_auth-1.2.0/mlflow_oidc_auth/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12050 2024-04-16 04:29:44.000000 mlflow_oidc_auth-1.2.0/mlflow_oidc_auth/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-04-16 04:29:44.000000 mlflow_oidc_auth-1.2.0/mlflow_oidc_auth/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:30:51.727897 mlflow_oidc_auth-1.2.0/mlflow_oidc_auth/db/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 04:29:44.000000 mlflow_oidc_auth-1.2.0/mlflow_oidc_auth/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-16 04:29:44.000000 mlflow_oidc_auth-1.2.0/mlflow_oidc_auth/db/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:30:51.727897 mlflow_oidc_auth-1.2.0/mlflow_oidc_auth/db/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 04:29:44.000000 mlflow_oidc_auth-1.2.0/mlflow_oidc_auth/db/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-04-16 04:29:44.000000 mlflow_oidc_auth-1.2.0/mlflow_oidc_auth/db/migrations/alembic.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-16 04:29:44.000000 mlflow_oidc_auth-1.2.0/mlflow_oidc_auth/db/migrations/env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:30:51.727897 mlflow_oidc_auth-1.2.0/mlflow_oidc_auth/db/migrations/versions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-16 04:29:44.000000 mlflow_oidc_auth-1.2.0/mlflow_oidc_auth/db/migrations/versions/8606fa83a998_initial_migration.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 04:29:44.000000 mlflow_oidc_auth-1.2.0/mlflow_oidc_auth/db/migrations/versions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-16 04:29:44.000000 mlflow_oidc_auth-1.2.0/mlflow_oidc_auth/db/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-04-16 04:29:44.000000 mlflow_oidc_auth-1.2.0/mlflow_oidc_auth/db/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-04-16 04:29:44.000000 mlflow_oidc_auth-1.2.0/mlflow_oidc_auth/entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-16 04:29:44.000000 mlflow_oidc_auth-1.2.0/mlflow_oidc_auth/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-16 04:29:44.000000 mlflow_oidc_auth-1.2.0/mlflow_oidc_auth/routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10567 2024-04-16 04:29:44.000000 mlflow_oidc_auth-1.2.0/mlflow_oidc_auth/sqlalchemy_store.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:30:51.727897 mlflow_oidc_auth-1.2.0/mlflow_oidc_auth/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-16 04:29:44.000000 mlflow_oidc_auth-1.2.0/mlflow_oidc_auth/static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     4861 2024-04-16 04:29:44.000000 mlflow_oidc_auth-1.2.0/mlflow_oidc_auth/static/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:30:51.727897 mlflow_oidc_auth-1.2.0/mlflow_oidc_auth/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-16 04:29:44.000000 mlflow_oidc_auth-1.2.0/mlflow_oidc_auth/templates/_footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-16 04:29:44.000000 mlflow_oidc_auth-1.2.0/mlflow_oidc_auth/templates/_head.html
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-16 04:29:44.000000 mlflow_oidc_auth-1.2.0/mlflow_oidc_auth/templates/auth.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:30:51.731897 mlflow_oidc_auth-1.2.0/mlflow_oidc_auth/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)    16975 2024-04-16 04:30:48.000000 mlflow_oidc_auth-1.2.0/mlflow_oidc_auth/ui/398.7b4ae9e14c5af3b5.js
+-rw-r--r--   0 runner    (1001) docker     (127)    17458 2024-04-16 04:30:48.000000 mlflow_oidc_auth-1.2.0/mlflow_oidc_auth/ui/3rdpartylicenses.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-04-16 04:30:48.000000 mlflow_oidc_auth-1.2.0/mlflow_oidc_auth/ui/953.94c6a01c085d9731.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-16 04:30:48.000000 mlflow_oidc_auth-1.2.0/mlflow_oidc_auth/ui/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    12068 2024-04-16 04:30:49.000000 mlflow_oidc_auth-1.2.0/mlflow_oidc_auth/ui/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)   703564 2024-04-16 04:30:48.000000 mlflow_oidc_auth-1.2.0/mlflow_oidc_auth/ui/main.aa12189a64349ade.js
+-rw-r--r--   0 runner    (1001) docker     (127)    35227 2024-04-16 04:30:48.000000 mlflow_oidc_auth-1.2.0/mlflow_oidc_auth/ui/polyfills.90a0049d0bf863c4.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-04-16 04:30:48.000000 mlflow_oidc_auth-1.2.0/mlflow_oidc_auth/ui/runtime.253378063cb1a335.js
+-rw-r--r--   0 runner    (1001) docker     (127)   301021 2024-04-16 04:30:48.000000 mlflow_oidc_auth-1.2.0/mlflow_oidc_auth/ui/styles.68f068b304676cf1.css
+-rw-r--r--   0 runner    (1001) docker     (127)    34435 2024-04-16 04:29:44.000000 mlflow_oidc_auth-1.2.0/mlflow_oidc_auth/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:30:51.731897 mlflow_oidc_auth-1.2.0/mlflow_oidc_auth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17262 2024-04-16 04:30:51.000000 mlflow_oidc_auth-1.2.0/mlflow_oidc_auth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-16 04:30:51.000000 mlflow_oidc_auth-1.2.0/mlflow_oidc_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 04:30:51.000000 mlflow_oidc_auth-1.2.0/mlflow_oidc_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-16 04:30:51.000000 mlflow_oidc_auth-1.2.0/mlflow_oidc_auth.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-16 04:30:51.000000 mlflow_oidc_auth-1.2.0/mlflow_oidc_auth.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-16 04:30:51.000000 mlflow_oidc_auth-1.2.0/mlflow_oidc_auth.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-16 04:29:44.000000 mlflow_oidc_auth-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 04:30:51.731897 mlflow_oidc_auth-1.2.0/setup.cfg
```

### Comparing `mlflow-oidc-auth-1.1.2/LICENSE` & `mlflow_oidc_auth-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mlflow-oidc-auth-1.1.2/PKG-INFO` & `mlflow_oidc_auth-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlflow-oidc-auth
-Version: 1.1.2
+Version: 1.2.0
 Summary: OIDC auth plugin for MLflow
 Maintainer-email: Data Platform folks <noreply@example.com>
 License: 				Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -205,15 +205,15 @@
            limitations under the License.
         
 Project-URL: homepage, https://github.com/data-platform-hq/mlflow-oidc-auth
 Project-URL: issues, https://github.com/data-platform-hq/mlflow-oidc-auth/issues
 Project-URL: documentation, https://github.com/data-platform-hq/mlflow-oidc-auth/tree/main/docs/
 Project-URL: repository, https://github.com/data-platform-hq/mlflow-oidc-auth
 Keywords: mlflow,oauth2,oidc
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Information Technology
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: Apache Software License
@@ -253,17 +253,14 @@
 | OIDC_AUTHORIZATION_URL | OIDC Auth URL (if discovery URL is not defined) |
 | OIDC_TOKEN_URL         | OIDC Token URL (if discovery URL is not defined) |
 | OIDC_USER_URL          | OIDC User info URL (if discovery URL is not defined) |
 | SECRET_KEY             | Key to perform cookie encryption |
 | OAUTHLIB_INSECURE_TRANSPORT | Development only. Allow to use insecure endpoints for OIDC |
 | LOG_LEVEL                   | Application log level |
 | OIDC_USERS_DB_URI | Database connection string |
-| MLFLOW_TRACKING_USERNAME | Credentials for internal communications via API |
-| MLFLOW_TRACKING_PASSWORD | Credentials for internal communications via API |
-| MLFLOW_TRACKING_URI | URI for internal communications via API |
 
 # Configuration examples
 
 ## Okta
 
 ```bash
 OIDC_DISCOVERY_URL = 'https://<your_domain>.okta.com/.well-known/openid-configuration'
```

### Comparing `mlflow-oidc-auth-1.1.2/README.md` & `mlflow_oidc_auth-1.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -20,17 +20,14 @@
 | OIDC_AUTHORIZATION_URL | OIDC Auth URL (if discovery URL is not defined) |
 | OIDC_TOKEN_URL         | OIDC Token URL (if discovery URL is not defined) |
 | OIDC_USER_URL          | OIDC User info URL (if discovery URL is not defined) |
 | SECRET_KEY             | Key to perform cookie encryption |
 | OAUTHLIB_INSECURE_TRANSPORT | Development only. Allow to use insecure endpoints for OIDC |
 | LOG_LEVEL                   | Application log level |
 | OIDC_USERS_DB_URI | Database connection string |
-| MLFLOW_TRACKING_USERNAME | Credentials for internal communications via API |
-| MLFLOW_TRACKING_PASSWORD | Credentials for internal communications via API |
-| MLFLOW_TRACKING_URI | URI for internal communications via API |
 
 # Configuration examples
 
 ## Okta
 
 ```bash
 OIDC_DISCOVERY_URL = 'https://<your_domain>.okta.com/.well-known/openid-configuration'
```

### Comparing `mlflow-oidc-auth-1.1.2/mlflow_oidc_auth/app.py` & `mlflow_oidc_auth-1.2.0/mlflow_oidc_auth/app.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,41 +21,42 @@
 
 # UI routes
 app.add_url_rule(rule=routes.STATIC, methods=["GET"], view_func=views.oidc_static)
 app.add_url_rule(rule=routes.UI, methods=["GET"], view_func=views.oidc_ui)
 app.add_url_rule(rule=routes.UI_ROOT, methods=["GET"], view_func=views.oidc_ui)
 
 # User token
-app.add_url_rule(rule=routes.CREATE_ACCESS_TOKEN, methods=["GET"], view_func=views.create_access_token)
+app.add_url_rule(rule=routes.GET_ACCESS_TOKEN, methods=["GET"], view_func=views.create_access_token)
 app.add_url_rule(rule=routes.GET_CURRENT_USER, methods=["GET"], view_func=views.get_current_user)
 
 # UI routes support
 app.add_url_rule(rule=routes.GET_EXPERIMENTS, methods=["GET"], view_func=views.get_experiments)
 app.add_url_rule(rule=routes.GET_MODELS, methods=["GET"], view_func=views.get_models)
 app.add_url_rule(rule=routes.GET_USERS, methods=["GET"], view_func=views.get_users)
 app.add_url_rule(rule=routes.GET_USER_EXPERIMENTS, methods=["GET"], view_func=views.get_user_experiments)
 app.add_url_rule(rule=routes.GET_USER_MODELS, methods=["GET"], view_func=views.get_user_models)
 app.add_url_rule(rule=routes.GET_EXPERIMENT_USERS, methods=["GET"], view_func=views.get_experiment_users)
 app.add_url_rule(rule=routes.GET_MODEL_USERS, methods=["GET"], view_func=views.get_model_users)
 
 # User management
 app.add_url_rule(rule=routes.CREATE_USER, methods=["POST"], view_func=views.create_user)
 app.add_url_rule(rule=routes.GET_USER, methods=["GET"], view_func=views.get_user)
-app.add_url_rule(rule=routes.UPDATE_USER_PASSWORD, methods=["GET"], view_func=views.update_username_password)
-app.add_url_rule(rule=routes.UPDATE_USER_ADMIN, methods=["GET"], view_func=views.update_user_admin)
-app.add_url_rule(rule=routes.DELETE_USER, methods=["GET"], view_func=views.delete_user)
+app.add_url_rule(rule=routes.UPDATE_USER_PASSWORD, methods=["PATCH"], view_func=views.update_username_password)
+app.add_url_rule(rule=routes.UPDATE_USER_ADMIN, methods=["PATCH"], view_func=views.update_user_admin)
+app.add_url_rule(rule=routes.DELETE_USER, methods=["DELETE"], view_func=views.delete_user)
 
 # permission management
 app.add_url_rule(rule=routes.CREATE_EXPERIMENT_PERMISSION, methods=["POST"], view_func=views.create_experiment_permission)
 app.add_url_rule(rule=routes.GET_EXPERIMENT_PERMISSION, methods=["GET"], view_func=views.get_experiment_permission)
-app.add_url_rule(rule=routes.UPDATE_EXPERIMENT_PERMISSION, methods=["POST"], view_func=views.update_experiment_permission)
-app.add_url_rule(rule=routes.DELETE_EXPERIMENT_PERMISSION, methods=["POST"], view_func=views.delete_experiment_permission)
-app.add_url_rule(rule=routes.CREATE_REGISTERED_MODEL_PERMISSION, methods=["POST"], view_func=views.create_model_permission)
-app.add_url_rule(rule=routes.GET_REGISTERED_MODEL_PERMISSION, methods=["GET"], view_func=views.get_model_permission)
-app.add_url_rule(rule=routes.UPDATE_REGISTERED_MODEL_PERMISSION, methods=["POST"], view_func=views.update_model_permission)
-app.add_url_rule(rule=routes.DELETE_REGISTERED_MODEL_PERMISSION, methods=["POST"], view_func=views.delete_model_permission)
+app.add_url_rule(rule=routes.UPDATE_EXPERIMENT_PERMISSION, methods=["PATCH"], view_func=views.update_experiment_permission)
+app.add_url_rule(rule=routes.DELETE_EXPERIMENT_PERMISSION, methods=["DELETE"], view_func=views.delete_experiment_permission)
+app.add_url_rule(rule=routes.CREATE_REGISTERED_MODEL_PERMISSION, methods=["POST"], view_func=views.create_registered_model_permission)
+app.add_url_rule(rule=routes.GET_REGISTERED_MODEL_PERMISSION, methods=["GET"], view_func=views.get_registered_model_permission)
+app.add_url_rule(rule=routes.UPDATE_REGISTERED_MODEL_PERMISSION, methods=["PATCH"], view_func=views.update_registered_model_permission)
+app.add_url_rule(rule=routes.DELETE_REGISTERED_MODEL_PERMISSION, methods=["DELETE"], view_func=views.delete_registered_model_permission)
 
 # Add new hooks
 app.before_request(views.before_request_hook)
+app.after_request(views.after_request_hook)
 
 # Set up session
 Session(app)
```

### Comparing `mlflow-oidc-auth-1.1.2/mlflow_oidc_auth/client.py` & `mlflow_oidc_auth-1.2.0/mlflow_oidc_auth/client.py`

 * *Files identical despite different names*

### Comparing `mlflow-oidc-auth-1.1.2/mlflow_oidc_auth/config.py` & `mlflow_oidc_auth-1.2.0/mlflow_oidc_auth/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from dotenv import load_dotenv
 from mlflow_oidc_auth.app import app
 
 load_dotenv()  # take environment variables from .env.
 
 
 class AppConfig:
+    DEFAULT_MLFLOW_PERMISSION = os.environ.get("DEFAULT_MLFLOW_PERMISSION", "MANAGE")
     SECRET_KEY = os.environ.get("SECRET_KEY", secrets.token_hex(16))
     SESSION_TYPE = "cachelib"
     LEVEL = logging.DEBUG if os.environ.get("DEBUG") else logging.INFO
     LOG_LEVEL = os.environ.get("LOG_LEVEL", LEVEL)
     OIDC_USERS_DB_URI = os.environ.get("OIDC_USERS_DB_URI", "sqlite:///auth.db")
     OIDC_GROUP_NAME = os.environ.get("OIDC_GROUP_NAME", "mlflow")
     OIDC_ADMIN_GROUP_NAME = os.environ.get("OIDC_ADMIN_GROUP_NAME", "mlflow-admin")
@@ -31,14 +32,12 @@
     else:
         OIDC_AUTHORIZATION_URL = os.environ.get("OIDC_AUTHORIZATION_URL", None)
         OIDC_TOKEN_URL = os.environ.get("OIDC_TOKEN_URL", None)
         OIDC_USER_URL = os.environ.get("OIDC_USER_URL", None)
     OIDC_REDIRECT_URI = os.environ.get("OIDC_REDIRECT_URI", None)
     OIDC_CLIENT_ID = os.environ.get("OIDC_CLIENT_ID", None)
     OIDC_CLIENT_SECRET = os.environ.get("OIDC_CLIENT_SECRET", None)
-    MLFLOW_TRACKING_URI = os.environ.get("MLFLOW_TRACKING_URI", "http://localhost:8080")
-    MLFLOW_TRACKING_USERNAME = os.environ.get("MLFLOW_TRACKING_USERNAME", secrets.token_urlsafe(32))
-    MLFLOW_TRACKING_PASSWORD = os.environ.get("MLFLOW_TRACKING_PASSWORD", secrets.token_urlsafe(72))
+
 
     @staticmethod
     def get_property(property_name):
         return getattr(AppConfig, property_name, None)
```

### Comparing `mlflow-oidc-auth-1.1.2/mlflow_oidc_auth/db/migrations/alembic.ini` & `mlflow_oidc_auth-1.2.0/mlflow_oidc_auth/db/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `mlflow-oidc-auth-1.1.2/mlflow_oidc_auth/db/migrations/env.py` & `mlflow_oidc_auth-1.2.0/mlflow_oidc_auth/db/migrations/env.py`

 * *Files identical despite different names*

### Comparing `mlflow-oidc-auth-1.1.2/mlflow_oidc_auth/db/migrations/versions/8606fa83a998_initial_migration.py` & `mlflow_oidc_auth-1.2.0/mlflow_oidc_auth/db/migrations/versions/8606fa83a998_initial_migration.py`

 * *Files identical despite different names*

### Comparing `mlflow-oidc-auth-1.1.2/mlflow_oidc_auth/db/models.py` & `mlflow_oidc_auth-1.2.0/mlflow_oidc_auth/db/models.py`

 * *Files identical despite different names*

### Comparing `mlflow-oidc-auth-1.1.2/mlflow_oidc_auth/db/utils.py` & `mlflow_oidc_auth-1.2.0/mlflow_oidc_auth/db/utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-oidc-auth-1.1.2/mlflow_oidc_auth/entities.py` & `mlflow_oidc_auth-1.2.0/mlflow_oidc_auth/entities.py`

 * *Files identical despite different names*

### Comparing `mlflow-oidc-auth-1.1.2/mlflow_oidc_auth/permissions.py` & `mlflow_oidc_auth-1.2.0/mlflow_oidc_auth/permissions.py`

 * *Files identical despite different names*

### Comparing `mlflow-oidc-auth-1.1.2/mlflow_oidc_auth/routes.py` & `mlflow_oidc_auth-1.2.0/mlflow_oidc_auth/routes.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 CALLBACK = "/callback"
 
 STATIC = "/oidc/static/<path:filename>"
 UI = "/oidc/ui/<path:filename>"
 UI_ROOT = "/oidc/ui/"
 
 # create access token for current user
-CREATE_ACCESS_TOKEN = _get_rest_path("/mlflow/users/access-token")
+GET_ACCESS_TOKEN = _get_rest_path("/mlflow/users/access-token")
 # get infrmation about current user
 GET_CURRENT_USER = _get_rest_path("/mlflow/users/current")
 # list of experiments, models, users
 GET_EXPERIMENTS = _get_rest_path("/mlflow/experiments")
 GET_MODELS = _get_rest_path("/mlflow/registered-models")
 GET_USERS = _get_rest_path("/mlflow/users")
 # list of experiments, models, filtered by user
```

### Comparing `mlflow-oidc-auth-1.1.2/mlflow_oidc_auth/sqlalchemy_store.py` & `mlflow_oidc_auth-1.2.0/mlflow_oidc_auth/sqlalchemy_store.py`

 * *Files identical despite different names*

### Comparing `mlflow-oidc-auth-1.1.2/mlflow_oidc_auth/static/favicon.ico` & `mlflow_oidc_auth-1.2.0/mlflow_oidc_auth/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `mlflow-oidc-auth-1.1.2/mlflow_oidc_auth/static/style.css` & `mlflow_oidc_auth-1.2.0/mlflow_oidc_auth/static/style.css`

 * *Files identical despite different names*

### Comparing `mlflow-oidc-auth-1.1.2/mlflow_oidc_auth/ui/398.70c7e628915a6c39.js` & `mlflow_oidc_auth-1.2.0/mlflow_oidc_auth/ui/398.7b4ae9e14c5af3b5.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -64,16 +64,16 @@
                                 entityName: e,
                                 entityType: P.W.MODEL,
                                 permission: n
                             }
                         }).afterClosed().pipe((0, E.h)(Boolean), (0, a.w)(({
                             permission: h
                         }) => this.permissionDataService.updateModelPermission({
-                            model_name: e,
-                            new_permission: h,
+                            name: e,
+                            permission: h,
                             user_name: s
                         })))
                     }
                     openEditUserPermissionsForExperimentModal(e, s, n) {
                         return this.dialog.open(g.jA, {
                             data: {
                                 userName: s,
@@ -81,15 +81,15 @@
                                 entityType: P.W.EXPERIMENT,
                                 permission: n
                             }
                         }).afterClosed().pipe((0, E.h)(Boolean), (0, a.w)(({
                             permission: h
                         }) => this.permissionDataService.updateExperimentPermission({
                             experiment_id: e,
-                            new_permission: h,
+                            permission: h,
                             user_name: s
                         })))
                     }
                     openGrantModelPermissionModal(e) {
                         return this.modelDataService.getAllModels().pipe((0, a.w)(s => this.dialog.open(g.Rt, {
                             data: {
                                 entityType: P.W.MODEL,
@@ -148,15 +148,15 @@
                                 users: e
                             }
                         }).afterClosed()), (0, E.h)(Boolean), (0, a.w)(({
                             user: e,
                             permission: s
                         }) => this.permissionDataService.createExperimentPermission({
                             experiment_id: this.experimentId,
-                            new_permission: s,
+                            permission: s,
                             user_name: e
                         })), (0, a.w)(() => this.loadUsersForExperiment(this.experimentId))).subscribe(e => this.userDataSource = e)
                     }
                     loadUsersForExperiment(e) {
                         return this.experimentDataService.getUsersForExperiment(e)
                     }
                 }
@@ -216,15 +216,15 @@
                     ngOnInit() {
                         this.modelId = this.route.snapshot.paramMap.get("id") ?? "", this.loadUsersForModel(this.modelId).subscribe(e => {
                             this.userDataSource = e
                         })
                     }
                     revokePermissionForUser(e) {
                         this.permissionDataService.deleteModelPermission({
-                            model_name: this.modelId,
+                            name: this.modelId,
                             user_name: e.username
                         }).pipe((0, p.b)(() => this.snackService.openSnackBar("Permission revoked successfully")), (0, a.w)(() => this.loadUsersForModel(this.modelId))).subscribe(s => this.userDataSource = s)
                     }
                     editPermissionForUser({
                         username: e,
                         permission: s
                     }) {
@@ -252,16 +252,16 @@
                             data: {
                                 users: e
                             }
                         }).afterClosed()), (0, E.h)(Boolean), (0, a.w)(({
                             user: e,
                             permission: s
                         }) => this.permissionDataService.createModelPermission({
-                            model_name: this.modelId,
-                            new_permission: s,
+                            name: this.modelId,
+                            permission: s,
                             user_name: e
                         })), (0, a.w)(() => this.loadUsersForModel(this.modelId))).subscribe(e => {
                             this.userDataSource = e
                         })
                     }
                 }
                 return t.\u0275fac = function(e) {
@@ -348,16 +348,16 @@
                         }
                         addModelPermissionToUser() {
                             this.permissionModalService.openGrantModelPermissionModal(this.userId).pipe((0, E.h)(Boolean), (0, a.w)(({
                                 entity: e,
                                 permission: s
                             }) => this.permissionDataService.createModelPermission({
                                 user_name: this.userId,
-                                model_name: e,
-                                new_permission: s
+                                name: e,
+                                permission: s
                             })), (0, p.b)(() => this.snackBarService.openSnackBar("Permission granted successfully")), (0, a.w)(() => this.modelDataService.getModelsForUser(this.userId))).subscribe(e => this.modelsDataSource = e)
                         }
                         addExperimentPermissionToUser() {
                             this.expDataService.getAllExperiments().pipe((0, a.w)(e => this.dialog.open(g.Rt, {
                                 data: {
                                     entityType: P.W.EXPERIMENT,
                                     entities: e.map(({
@@ -367,15 +367,15 @@
                                 }
                             }).afterClosed()), (0, E.h)(Boolean), (0, a.w)(({
                                 entity: e,
                                 permission: s
                             }) => this.permissionDataService.createExperimentPermission({
                                 user_name: this.userId,
                                 experiment_name: e,
-                                new_permission: s
+                                permission: s
                             })), (0, p.b)(() => this.snackBarService.openSnackBar("Permission granted successfully")), (0, a.w)(() => this.expDataService.getExperimentsForUser(this.userId))).subscribe(e => this.experimentsDataSource = e)
                         }
                         handleExperimentActions(e) {
                             const n = {
                                 [c.EDIT]: this.handleEditUserPermissionForExperiment.bind(this),
                                 [c.REVOKE]: this.revokeExperimentPermissionForUser.bind(this)
                             } [e.action.action];
@@ -387,15 +387,15 @@
                                 user_name: this.userId
                             }).pipe((0, p.b)(() => this.snackBarService.openSnackBar("Permission revoked successfully")), (0, a.w)(() => this.expDataService.getExperimentsForUser(this.userId))).subscribe(s => this.experimentsDataSource = s)
                         }
                         revokeModelPermissionForUser({
                             name: e
                         }) {
                             this.permissionDataService.deleteModelPermission({
-                                model_name: e,
+                                name: e,
                                 user_name: this.userId
                             }).pipe((0, p.b)(() => this.snackBarService.openSnackBar("Permission revoked successfully")), (0, a.w)(() => this.modelDataService.getModelsForUser(this.userId))).subscribe(s => this.modelsDataSource = s)
                         }
                         handleModelActions({
                             action: e,
                             item: s
                         }) {
```

### Comparing `mlflow-oidc-auth-1.1.2/mlflow_oidc_auth/ui/3rdpartylicenses.txt` & `mlflow_oidc_auth-1.2.0/mlflow_oidc_auth/ui/3rdpartylicenses.txt`

 * *Files identical despite different names*

### Comparing `mlflow-oidc-auth-1.1.2/mlflow_oidc_auth/ui/953.94c6a01c085d9731.js` & `mlflow_oidc_auth-1.2.0/mlflow_oidc_auth/ui/953.94c6a01c085d9731.js`

 * *Files identical despite different names*

### Comparing `mlflow-oidc-auth-1.1.2/mlflow_oidc_auth/ui/favicon.ico` & `mlflow_oidc_auth-1.2.0/mlflow_oidc_auth/ui/favicon.ico`

 * *Files identical despite different names*

### Comparing `mlflow-oidc-auth-1.1.2/mlflow_oidc_auth/ui/index.html` & `mlflow_oidc_auth-1.2.0/mlflow_oidc_auth/ui/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -6,10 +6,10 @@
   <link rel="icon" type="image/x-icon" href="favicon.ico">
   <link rel="preconnect" href="https://fonts.gstatic.com">
   <style type="text/css">@font-face{font-family:'Roboto';font-style:normal;font-weight:300;font-display:swap;src:url(https://fonts.gstatic.com/s/roboto/v30/KFOlCnqEu92Fr1MmSU5fCRc4AMP6lbBP.woff2) format('woff2');unicode-range:U+0460-052F, U+1C80-1C88, U+20B4, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F;}@font-face{font-family:'Roboto';font-style:normal;font-weight:300;font-display:swap;src:url(https://fonts.gstatic.com/s/roboto/v30/KFOlCnqEu92Fr1MmSU5fABc4AMP6lbBP.woff2) format('woff2');unicode-range:U+0301, U+0400-045F, U+0490-0491, U+04B0-04B1, U+2116;}@font-face{font-family:'Roboto';font-style:normal;font-weight:300;font-display:swap;src:url(https://fonts.gstatic.com/s/roboto/v30/KFOlCnqEu92Fr1MmSU5fCBc4AMP6lbBP.woff2) format('woff2');unicode-range:U+1F00-1FFF;}@font-face{font-family:'Roboto';font-style:normal;font-weight:300;font-display:swap;src:url(https://fonts.gstatic.com/s/roboto/v30/KFOlCnqEu92Fr1MmSU5fBxc4AMP6lbBP.woff2) format('woff2');unicode-range:U+0370-0377, U+037A-037F, U+0384-038A, U+038C, U+038E-03A1, U+03A3-03FF;}@font-face{font-family:'Roboto';font-style:normal;font-weight:300;font-display:swap;src:url(https://fonts.gstatic.com/s/roboto/v30/KFOlCnqEu92Fr1MmSU5fCxc4AMP6lbBP.woff2) format('woff2');unicode-range:U+0102-0103, U+0110-0111, U+0128-0129, U+0168-0169, U+01A0-01A1, U+01AF-01B0, U+0300-0301, U+0303-0304, U+0308-0309, U+0323, U+0329, U+1EA0-1EF9, U+20AB;}@font-face{font-family:'Roboto';font-style:normal;font-weight:300;font-display:swap;src:url(https://fonts.gstatic.com/s/roboto/v30/KFOlCnqEu92Fr1MmSU5fChc4AMP6lbBP.woff2) format('woff2');unicode-range:U+0100-02AF, U+0304, U+0308, U+0329, U+1E00-1E9F, U+1EF2-1EFF, U+2020, U+20A0-20AB, U+20AD-20C0, U+2113, U+2C60-2C7F, U+A720-A7FF;}@font-face{font-family:'Roboto';font-style:normal;font-weight:300;font-display:swap;src:url(https://fonts.gstatic.com/s/roboto/v30/KFOlCnqEu92Fr1MmSU5fBBc4AMP6lQ.woff2) format('woff2');unicode-range:U+0000-00FF, U+0131, U+0152-0153, U+02BB-02BC, U+02C6, U+02DA, U+02DC, U+0304, U+0308, U+0329, U+2000-206F, U+2074, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD;}@font-face{font-family:'Roboto';font-style:normal;font-weight:400;font-display:swap;src:url(https://fonts.gstatic.com/s/roboto/v30/KFOmCnqEu92Fr1Mu72xKKTU1Kvnz.woff2) format('woff2');unicode-range:U+0460-052F, U+1C80-1C88, U+20B4, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F;}@font-face{font-family:'Roboto';font-style:normal;font-weight:400;font-display:swap;src:url(https://fonts.gstatic.com/s/roboto/v30/KFOmCnqEu92Fr1Mu5mxKKTU1Kvnz.woff2) format('woff2');unicode-range:U+0301, U+0400-045F, U+0490-0491, U+04B0-04B1, U+2116;}@font-face{font-family:'Roboto';font-style:normal;font-weight:400;font-display:swap;src:url(https://fonts.gstatic.com/s/roboto/v30/KFOmCnqEu92Fr1Mu7mxKKTU1Kvnz.woff2) format('woff2');unicode-range:U+1F00-1FFF;}@font-face{font-family:'Roboto';font-style:normal;font-weight:400;font-display:swap;src:url(https://fonts.gstatic.com/s/roboto/v30/KFOmCnqEu92Fr1Mu4WxKKTU1Kvnz.woff2) format('woff2');unicode-range:U+0370-0377, U+037A-037F, U+0384-038A, U+038C, U+038E-03A1, U+03A3-03FF;}@font-face{font-family:'Roboto';font-style:normal;font-weight:400;font-display:swap;src:url(https://fonts.gstatic.com/s/roboto/v30/KFOmCnqEu92Fr1Mu7WxKKTU1Kvnz.woff2) format('woff2');unicode-range:U+0102-0103, U+0110-0111, U+0128-0129, U+0168-0169, U+01A0-01A1, U+01AF-01B0, U+0300-0301, U+0303-0304, U+0308-0309, U+0323, U+0329, U+1EA0-1EF9, U+20AB;}@font-face{font-family:'Roboto';font-style:normal;font-weight:400;font-display:swap;src:url(https://fonts.gstatic.com/s/roboto/v30/KFOmCnqEu92Fr1Mu7GxKKTU1Kvnz.woff2) format('woff2');unicode-range:U+0100-02AF, U+0304, U+0308, U+0329, U+1E00-1E9F, U+1EF2-1EFF, U+2020, U+20A0-20AB, U+20AD-20C0, U+2113, U+2C60-2C7F, U+A720-A7FF;}@font-face{font-family:'Roboto';font-style:normal;font-weight:400;font-display:swap;src:url(https://fonts.gstatic.com/s/roboto/v30/KFOmCnqEu92Fr1Mu4mxKKTU1Kg.woff2) format('woff2');unicode-range:U+0000-00FF, U+0131, U+0152-0153, U+02BB-02BC, U+02C6, U+02DA, U+02DC, U+0304, U+0308, U+0329, U+2000-206F, U+2074, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD;}@font-face{font-family:'Roboto';font-style:normal;font-weight:500;font-display:swap;src:url(https://fonts.gstatic.com/s/roboto/v30/KFOlCnqEu92Fr1MmEU9fCRc4AMP6lbBP.woff2) format('woff2');unicode-range:U+0460-052F, U+1C80-1C88, U+20B4, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F;}@font-face{font-family:'Roboto';font-style:normal;font-weight:500;font-display:swap;src:url(https://fonts.gstatic.com/s/roboto/v30/KFOlCnqEu92Fr1MmEU9fABc4AMP6lbBP.woff2) format('woff2');unicode-range:U+0301, U+0400-045F, U+0490-0491, U+04B0-04B1, U+2116;}@font-face{font-family:'Roboto';font-style:normal;font-weight:500;font-display:swap;src:url(https://fonts.gstatic.com/s/roboto/v30/KFOlCnqEu92Fr1MmEU9fCBc4AMP6lbBP.woff2) format('woff2');unicode-range:U+1F00-1FFF;}@font-face{font-family:'Roboto';font-style:normal;font-weight:500;font-display:swap;src:url(https://fonts.gstatic.com/s/roboto/v30/KFOlCnqEu92Fr1MmEU9fBxc4AMP6lbBP.woff2) format('woff2');unicode-range:U+0370-0377, U+037A-037F, U+0384-038A, U+038C, U+038E-03A1, U+03A3-03FF;}@font-face{font-family:'Roboto';font-style:normal;font-weight:500;font-display:swap;src:url(https://fonts.gstatic.com/s/roboto/v30/KFOlCnqEu92Fr1MmEU9fCxc4AMP6lbBP.woff2) format('woff2');unicode-range:U+0102-0103, U+0110-0111, U+0128-0129, U+0168-0169, U+01A0-01A1, U+01AF-01B0, U+0300-0301, U+0303-0304, U+0308-0309, U+0323, U+0329, U+1EA0-1EF9, U+20AB;}@font-face{font-family:'Roboto';font-style:normal;font-weight:500;font-display:swap;src:url(https://fonts.gstatic.com/s/roboto/v30/KFOlCnqEu92Fr1MmEU9fChc4AMP6lbBP.woff2) format('woff2');unicode-range:U+0100-02AF, U+0304, U+0308, U+0329, U+1E00-1E9F, U+1EF2-1EFF, U+2020, U+20A0-20AB, U+20AD-20C0, U+2113, U+2C60-2C7F, U+A720-A7FF;}@font-face{font-family:'Roboto';font-style:normal;font-weight:500;font-display:swap;src:url(https://fonts.gstatic.com/s/roboto/v30/KFOlCnqEu92Fr1MmEU9fBBc4AMP6lQ.woff2) format('woff2');unicode-range:U+0000-00FF, U+0131, U+0152-0153, U+02BB-02BC, U+02C6, U+02DA, U+02DC, U+0304, U+0308, U+0329, U+2000-206F, U+2074, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD;}</style>
   <style type="text/css">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2');}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased;}</style>
 <style>.mat-typography{font:400 14px/20px Roboto,Helvetica Neue,sans-serif;letter-spacing:normal}@charset "UTF-8";html,body{height:100%}body{margin:0;font-family:Roboto,Helvetica Neue,sans-serif}:root{--bs-blue:#0d6efd;--bs-indigo:#6610f2;--bs-purple:#6f42c1;--bs-pink:#d63384;--bs-red:#dc3545;--bs-orange:#fd7e14;--bs-yellow:#ffc107;--bs-green:#198754;--bs-teal:#20c997;--bs-cyan:#0dcaf0;--bs-black:#000;--bs-white:#fff;--bs-gray:#6c757d;--bs-gray-dark:#343a40;--bs-gray-100:#f8f9fa;--bs-gray-200:#e9ecef;--bs-gray-300:#dee2e6;--bs-gray-400:#ced4da;--bs-gray-500:#adb5bd;--bs-gray-600:#6c757d;--bs-gray-700:#495057;--bs-gray-800:#343a40;--bs-gray-900:#212529;--bs-primary:#0d6efd;--bs-secondary:#6c757d;--bs-success:#198754;--bs-info:#0dcaf0;--bs-warning:#ffc107;--bs-danger:#dc3545;--bs-light:#f8f9fa;--bs-dark:#212529;--bs-primary-rgb:13, 110, 253;--bs-secondary-rgb:108, 117, 125;--bs-success-rgb:25, 135, 84;--bs-info-rgb:13, 202, 240;--bs-warning-rgb:255, 193, 7;--bs-danger-rgb:220, 53, 69;--bs-light-rgb:248, 249, 250;--bs-dark-rgb:33, 37, 41;--bs-primary-text-emphasis:#052c65;--bs-secondary-text-emphasis:#2b2f32;--bs-success-text-emphasis:#0a3622;--bs-info-text-emphasis:#055160;--bs-warning-text-emphasis:#664d03;--bs-danger-text-emphasis:#58151c;--bs-light-text-emphasis:#495057;--bs-dark-text-emphasis:#495057;--bs-primary-bg-subtle:#cfe2ff;--bs-secondary-bg-subtle:#e2e3e5;--bs-success-bg-subtle:#d1e7dd;--bs-info-bg-subtle:#cff4fc;--bs-warning-bg-subtle:#fff3cd;--bs-danger-bg-subtle:#f8d7da;--bs-light-bg-subtle:#fcfcfd;--bs-dark-bg-subtle:#ced4da;--bs-primary-border-subtle:#9ec5fe;--bs-secondary-border-subtle:#c4c8cb;--bs-success-border-subtle:#a3cfbb;--bs-info-border-subtle:#9eeaf9;--bs-warning-border-subtle:#ffe69c;--bs-danger-border-subtle:#f1aeb5;--bs-light-border-subtle:#e9ecef;--bs-dark-border-subtle:#adb5bd;--bs-white-rgb:255, 255, 255;--bs-black-rgb:0, 0, 0;--bs-font-sans-serif:system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", "Noto Sans", "Liberation Sans", Arial, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji";--bs-font-monospace:SFMono-Regular, Menlo, Monaco, Consolas, "Liberation Mono", "Courier New", monospace;--bs-gradient:linear-gradient(180deg, rgba(255, 255, 255, .15), rgba(255, 255, 255, 0));--bs-body-font-family:var(--bs-font-sans-serif);--bs-body-font-size:1rem;--bs-body-font-weight:400;--bs-body-line-height:1.5;--bs-body-color:#212529;--bs-body-color-rgb:33, 37, 41;--bs-body-bg:#fff;--bs-body-bg-rgb:255, 255, 255;--bs-emphasis-color:#000;--bs-emphasis-color-rgb:0, 0, 0;--bs-secondary-color:rgba(33, 37, 41, .75);--bs-secondary-color-rgb:33, 37, 41;--bs-secondary-bg:#e9ecef;--bs-secondary-bg-rgb:233, 236, 239;--bs-tertiary-color:rgba(33, 37, 41, .5);--bs-tertiary-color-rgb:33, 37, 41;--bs-tertiary-bg:#f8f9fa;--bs-tertiary-bg-rgb:248, 249, 250;--bs-heading-color:inherit;--bs-link-color:#0d6efd;--bs-link-color-rgb:13, 110, 253;--bs-link-decoration:underline;--bs-link-hover-color:#0a58ca;--bs-link-hover-color-rgb:10, 88, 202;--bs-code-color:#d63384;--bs-highlight-color:#212529;--bs-highlight-bg:#fff3cd;--bs-border-width:1px;--bs-border-style:solid;--bs-border-color:#dee2e6;--bs-border-color-translucent:rgba(0, 0, 0, .175);--bs-border-radius:.375rem;--bs-border-radius-sm:.25rem;--bs-border-radius-lg:.5rem;--bs-border-radius-xl:1rem;--bs-border-radius-xxl:2rem;--bs-border-radius-2xl:var(--bs-border-radius-xxl);--bs-border-radius-pill:50rem;--bs-box-shadow:0 .5rem 1rem rgba(0, 0, 0, .15);--bs-box-shadow-sm:0 .125rem .25rem rgba(0, 0, 0, .075);--bs-box-shadow-lg:0 1rem 3rem rgba(0, 0, 0, .175);--bs-box-shadow-inset:inset 0 1px 2px rgba(0, 0, 0, .075);--bs-focus-ring-width:.25rem;--bs-focus-ring-opacity:.25;--bs-focus-ring-color:rgba(13, 110, 253, .25);--bs-form-valid-color:#198754;--bs-form-valid-border-color:#198754;--bs-form-invalid-color:#dc3545;--bs-form-invalid-border-color:#dc3545}*,*:before,*:after{box-sizing:border-box}@media (prefers-reduced-motion: no-preference){:root{scroll-behavior:smooth}}body{margin:0;font-family:var(--bs-body-font-family);font-size:var(--bs-body-font-size);font-weight:var(--bs-body-font-weight);line-height:var(--bs-body-line-height);color:var(--bs-body-color);text-align:var(--bs-body-text-align);background-color:var(--bs-body-bg);-webkit-text-size-adjust:100%;-webkit-tap-highlight-color:rgba(0,0,0,0)}:root{--bs-breakpoint-xs:0;--bs-breakpoint-sm:576px;--bs-breakpoint-md:768px;--bs-breakpoint-lg:992px;--bs-breakpoint-xl:1200px;--bs-breakpoint-xxl:1400px}</style><link rel="stylesheet" href="styles.68f068b304676cf1.css" media="print" onload="this.media='all'"><noscript><link rel="stylesheet" href="styles.68f068b304676cf1.css"></noscript></head>
 <body class="mat-typography">
   <app-root></app-root>
-<script src="runtime.0cd10aef5e6b1db8.js" type="module"></script><script src="polyfills.90a0049d0bf863c4.js" type="module"></script><script src="main.84383ebc03062e87.js" type="module"></script>
+<script src="runtime.253378063cb1a335.js" type="module"></script><script src="polyfills.90a0049d0bf863c4.js" type="module"></script><script src="main.aa12189a64349ade.js" type="module"></script>
 
 </body></html>
```

### Comparing `mlflow-oidc-auth-1.1.2/mlflow_oidc_auth/ui/main.84383ebc03062e87.js` & `mlflow_oidc_auth-1.2.0/mlflow_oidc_auth/ui/main.aa12189a64349ade.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -9,18 +9,18 @@
                 ALL_EXPERIMENTS: "/api/2.0/mlflow/experiments",
                 EXPERIMENTS_FOR_USER: "/api/2.0/mlflow/users/${userName}/experiments",
                 USERS_FOR_EXPERIMENT: "/api/2.0/mlflow/experiments/${experimentName}/users",
                 ALL_MODELS: "/api/2.0/mlflow/registered-models",
                 MODELS_FOR_USER: "/api/2.0/mlflow/users/${userName}/registered-models",
                 USERS_FOR_MODEL: "/api/2.0/mlflow/registered-models/${modelName}/users",
                 CREATE_EXPERIMENT_PERMISSION: "/api/2.0/mlflow/experiments/permissions/create",
-                CREATE_MODEL_PERMISSION: "/api/2.0/mlflow/registered-models/permissions/create",
                 UPDATE_EXPERIMENT_PERMISSION: "/api/2.0/mlflow/experiments/permissions/update",
-                UPDATE_MODEL_PERMISSION: "/api/2.0/mlflow/registered-models/permissions/update",
                 DELETE_EXPERIMENT_PERMISSION: "/api/2.0/mlflow/experiments/permissions/delete",
+                CREATE_MODEL_PERMISSION: "/api/2.0/mlflow/registered-models/permissions/create",
+                UPDATE_MODEL_PERMISSION: "/api/2.0/mlflow/registered-models/permissions/update",
                 DELETE_MODEL_PERMISSION: "/api/2.0/mlflow/registered-models/permissions/delete",
                 GET_ALL_USERS: "/api/2.0/mlflow/users",
                 GET_ACCESS_TOKEN: "/api/2.0/mlflow/users/access-token",
                 GET_CURRENT_USER: "/api/2.0/mlflow/users/current"
             }
         },
         2590: (Ht, $e, v) => {
@@ -45,15 +45,15 @@
                 S = v(7392),
                 C = v(4859),
                 F = v(9197);
             const O = function() {
                     return ["/home"]
                 },
                 De = function() {
-                    return ["/admin-panel"]
+                    return ["/manage"]
                 };
             let L = (() => {
                 class be {
                     constructor() {
                         this.name = ""
                     }
                     ngOnInit() {}
@@ -77,15 +77,15 @@
                         [1, "py-3"],
                         [1, "col-12", "d-flex", "align-items-center"],
                         [1, "mx-3"],
                         ["mat-button", "", 3, "routerLink"],
                         ["mat-button", "", "aria-label", "logout", 1, "logout", 3, "routerLink", "click"]
                     ],
                     template: function(fe, Te) {
-                        1 & fe && (s.TgZ(0, "header", 0)(1, "div", 1)(2, "span"), s._uU(3), s.qZA(), s.TgZ(4, "nav", 2)(5, "a", 3), s._uU(6, "Home"), s.qZA(), s.TgZ(7, "a", 3), s._uU(8, "Admin panel"), s.qZA()(), s.TgZ(9, "button", 4), s.NdJ("click", function() {
+                        1 & fe && (s.TgZ(0, "header", 0)(1, "div", 1)(2, "span"), s._uU(3), s.qZA(), s.TgZ(4, "nav", 2)(5, "a", 3), s._uU(6, "Home"), s.qZA(), s.TgZ(7, "a", 3), s._uU(8, "Manage Permissions"), s.qZA()(), s.TgZ(9, "button", 4), s.NdJ("click", function() {
                             return Te.logout()
                         }), s.TgZ(10, "mat-icon"), s._uU(11, "exit_to_app"), s.qZA(), s.TgZ(12, "span"), s._uU(13, "Logout"), s.qZA()()()()), 2 & fe && (s.xp6(3), s.hij("Hello, ", Te.name, ""), s.xp6(2), s.Q6J("routerLink", s.DdM(4, O)), s.xp6(2), s.Q6J("routerLink", s.DdM(5, De)), s.xp6(2), s.Q6J("routerLink", "/logout"))
                     },
                     dependencies: [S.Hw, C.lW, C.zs, F.yS, F.rH],
                     styles: [".logout[_ngcontent-%COMP%]{margin-left:auto}"]
                 }), be
             })()
@@ -101,26 +101,29 @@
                 ac: () => s.a
             });
             var s = v(6709),
                 S = v(6290),
                 C = v(5938),
                 F = v(4006),
                 O = (() => {
-                    return (J = O || (O = {})).EDIT = "EDIT", J.READ = "READ", J.MANAGE = "MANAGE", O;
+                    return (J = O || (O = {})).EDIT = "EDIT", J.READ = "READ", J.MANAGE = "MANAGE", J.NO_PERMISSIONS = "NO_PERMISSIONS", O;
                     var J
                 })();
             const De = [{
                 value: O.EDIT,
                 title: "Edit"
             }, {
                 value: O.READ,
                 title: "Read"
             }, {
                 value: O.MANAGE,
                 title: "Manage"
+            }, {
+                value: O.NO_PERMISSIONS,
+                title: "No permissions"
             }];
             var L = v(4650),
                 be = v(9549),
                 Me = v(4144),
                 fe = v(4859),
                 Te = v(6895);
 
@@ -527,34 +530,34 @@
                     }
                     createExperimentPermission(L) {
                         return this.http.post(s.T.CREATE_EXPERIMENT_PERMISSION, L, {
                             responseType: "text"
                         })
                     }
                     updateExperimentPermission(L) {
-                        return this.http.post(s.T.UPDATE_EXPERIMENT_PERMISSION, L, {
+                        return this.http.patch(s.T.UPDATE_EXPERIMENT_PERMISSION, L, {
                             responseType: "text"
                         })
                     }
                     deleteExperimentPermission(L) {
-                        return this.http.post(s.T.DELETE_EXPERIMENT_PERMISSION, L, {
-                            responseType: "text"
+                        return this.http.delete(s.T.DELETE_EXPERIMENT_PERMISSION, {
+                            body: L
                         })
                     }
                     createModelPermission(L) {
                         return this.http.post(s.T.CREATE_MODEL_PERMISSION, L)
                     }
                     updateModelPermission(L) {
-                        return this.http.post(s.T.UPDATE_MODEL_PERMISSION, L, {
+                        return this.http.patch(s.T.UPDATE_MODEL_PERMISSION, L, {
                             responseType: "text"
                         })
                     }
                     deleteModelPermission(L) {
-                        return this.http.post(s.T.DELETE_MODEL_PERMISSION, L, {
-                            responseType: "text"
+                        return this.http.delete(s.T.DELETE_MODEL_PERMISSION, {
+                            body: L
                         })
                     }
                 }
                 return O.\u0275fac = function(L) {
                     return new(L || O)(S.LFG(C.eN))
                 }, O.\u0275prov = S.Yz7({
                     token: O,
@@ -1569,15 +1572,15 @@
             var s = v(1481),
                 S = v(4650),
                 C = v(9197);
             const F = [{
                 path: "home",
                 loadChildren: () => v.e(953).then(v.bind(v, 2953)).then(B => B.HomePageModule)
             }, {
-                path: "admin-panel",
+                path: "manage",
                 loadChildren: () => v.e(398).then(v.bind(v, 4398)).then(B => B.AdminPageModule)
             }, {
                 path: "**",
                 pathMatch: "full",
                 redirectTo: "home"
             }];
             let O = (() => {
```

### Comparing `mlflow-oidc-auth-1.1.2/mlflow_oidc_auth/ui/polyfills.90a0049d0bf863c4.js` & `mlflow_oidc_auth-1.2.0/mlflow_oidc_auth/ui/polyfills.90a0049d0bf863c4.js`

 * *Files identical despite different names*

### Comparing `mlflow-oidc-auth-1.1.2/mlflow_oidc_auth/ui/runtime.0cd10aef5e6b1db8.js` & `mlflow_oidc_auth-1.2.0/mlflow_oidc_auth/ui/runtime.253378063cb1a335.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -29,15 +29,15 @@
         e[n] = [t, o, f]
     }, r.d = (e, i) => {
         for (var t in i) r.o(i, t) && !r.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: i[t]
         })
     }, r.f = {}, r.e = e => Promise.all(Object.keys(r.f).reduce((i, t) => (r.f[t](e, i), i), [])), r.u = e => e + "." + {
-        398: "70c7e628915a6c39",
+        398: "7b4ae9e14c5af3b5",
         953: "94c6a01c085d9731"
     } [e] + ".js", r.miniCssF = e => {}, r.o = (e, i) => Object.prototype.hasOwnProperty.call(e, i), (() => {
         var e = {},
             i = "mlflow-oidc-auth-front:";
         r.l = (t, o, f, n) => {
             if (e[t]) e[t].push(o);
             else {
```

### Comparing `mlflow-oidc-auth-1.1.2/mlflow_oidc_auth/ui/styles.68f068b304676cf1.css` & `mlflow_oidc_auth-1.2.0/mlflow_oidc_auth/ui/styles.68f068b304676cf1.css`

 * *Files identical despite different names*

### Comparing `mlflow-oidc-auth-1.1.2/mlflow_oidc_auth.egg-info/PKG-INFO` & `mlflow_oidc_auth-1.2.0/mlflow_oidc_auth.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlflow-oidc-auth
-Version: 1.1.2
+Version: 1.2.0
 Summary: OIDC auth plugin for MLflow
 Maintainer-email: Data Platform folks <noreply@example.com>
 License: 				Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -205,15 +205,15 @@
            limitations under the License.
         
 Project-URL: homepage, https://github.com/data-platform-hq/mlflow-oidc-auth
 Project-URL: issues, https://github.com/data-platform-hq/mlflow-oidc-auth/issues
 Project-URL: documentation, https://github.com/data-platform-hq/mlflow-oidc-auth/tree/main/docs/
 Project-URL: repository, https://github.com/data-platform-hq/mlflow-oidc-auth
 Keywords: mlflow,oauth2,oidc
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Information Technology
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: Apache Software License
@@ -253,17 +253,14 @@
 | OIDC_AUTHORIZATION_URL | OIDC Auth URL (if discovery URL is not defined) |
 | OIDC_TOKEN_URL         | OIDC Token URL (if discovery URL is not defined) |
 | OIDC_USER_URL          | OIDC User info URL (if discovery URL is not defined) |
 | SECRET_KEY             | Key to perform cookie encryption |
 | OAUTHLIB_INSECURE_TRANSPORT | Development only. Allow to use insecure endpoints for OIDC |
 | LOG_LEVEL                   | Application log level |
 | OIDC_USERS_DB_URI | Database connection string |
-| MLFLOW_TRACKING_USERNAME | Credentials for internal communications via API |
-| MLFLOW_TRACKING_PASSWORD | Credentials for internal communications via API |
-| MLFLOW_TRACKING_URI | URI for internal communications via API |
 
 # Configuration examples
 
 ## Okta
 
 ```bash
 OIDC_DISCOVERY_URL = 'https://<your_domain>.okta.com/.well-known/openid-configuration'
```

### Comparing `mlflow-oidc-auth-1.1.2/mlflow_oidc_auth.egg-info/SOURCES.txt` & `mlflow_oidc_auth-1.2.0/mlflow_oidc_auth.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -25,18 +25,17 @@
 mlflow_oidc_auth/db/migrations/env.py
 mlflow_oidc_auth/db/migrations/versions/8606fa83a998_initial_migration.py
 mlflow_oidc_auth/db/migrations/versions/__init__.py
 mlflow_oidc_auth/static/favicon.ico
 mlflow_oidc_auth/static/style.css
 mlflow_oidc_auth/templates/_footer.html
 mlflow_oidc_auth/templates/_head.html
-mlflow_oidc_auth/templates/_header.html
 mlflow_oidc_auth/templates/auth.html
-mlflow_oidc_auth/ui/398.70c7e628915a6c39.js
+mlflow_oidc_auth/ui/398.7b4ae9e14c5af3b5.js
 mlflow_oidc_auth/ui/3rdpartylicenses.txt
 mlflow_oidc_auth/ui/953.94c6a01c085d9731.js
 mlflow_oidc_auth/ui/favicon.ico
 mlflow_oidc_auth/ui/index.html
-mlflow_oidc_auth/ui/main.84383ebc03062e87.js
+mlflow_oidc_auth/ui/main.aa12189a64349ade.js
 mlflow_oidc_auth/ui/polyfills.90a0049d0bf863c4.js
-mlflow_oidc_auth/ui/runtime.0cd10aef5e6b1db8.js
+mlflow_oidc_auth/ui/runtime.253378063cb1a335.js
 mlflow_oidc_auth/ui/styles.68f068b304676cf1.css
```

### Comparing `mlflow-oidc-auth-1.1.2/pyproject.toml` & `mlflow_oidc_auth-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [project]
 name = "mlflow-oidc-auth"
 dynamic = ["version"]
 description = "OIDC auth plugin for MLflow"
 readme = "README.md"
 keywords = ["mlflow", "oauth2", "oidc"]
 classifiers = [
-  "Development Status :: 3 - Alpha",
+  "Development Status :: 4 - Beta",
   "Intended Audience :: Developers",
   "Intended Audience :: End Users/Desktop",
   "Intended Audience :: Science/Research",
   "Intended Audience :: Information Technology",
   "Topic :: Scientific/Engineering :: Artificial Intelligence",
   "Topic :: Software Development :: Libraries :: Python Modules",
   "License :: OSI Approved :: Apache Software License",
```

