# Comparing `tmp/openedx-ledger-1.4.1.tar.gz` & `tmp/openedx_ledger-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openedx-ledger-1.4.1.tar", last modified: Wed Mar 20 11:27:49 2024, max compression
+gzip compressed data, was "openedx_ledger-1.4.2.tar", last modified: Tue Apr 16 13:45:23 2024, max compression
```

## Comparing `openedx-ledger-1.4.1.tar` & `openedx_ledger-1.4.2.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 11:27:49.751440 openedx-ledger-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-03-20 11:27:39.000000 openedx-ledger-1.4.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)    35139 2024-03-20 11:27:39.000000 openedx-ledger-1.4.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-03-20 11:27:39.000000 openedx-ledger-1.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9760 2024-03-20 11:27:49.751440 openedx-ledger-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5964 2024-03-20 11:27:39.000000 openedx-ledger-1.4.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 11:27:49.747439 openedx-ledger-1.4.1/openedx_ledger/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-03-20 11:27:39.000000 openedx-ledger-1.4.1/openedx_ledger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10060 2024-03-20 11:27:39.000000 openedx-ledger-1.4.1/openedx_ledger/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     8979 2024-03-20 11:27:39.000000 openedx-ledger-1.4.1/openedx_ledger/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-03-20 11:27:39.000000 openedx-ledger-1.4.1/openedx_ledger/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-03-20 11:27:39.000000 openedx-ledger-1.4.1/openedx_ledger/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 11:27:49.747439 openedx-ledger-1.4.1/openedx_ledger/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-03-20 11:27:39.000000 openedx-ledger-1.4.1/openedx_ledger/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     6005 2024-03-20 11:27:39.000000 openedx-ledger-1.4.1/openedx_ledger/migrations/0002_historicalledger_historicalreversal_historicaltransaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     4294 2024-03-20 11:27:39.000000 openedx-ledger-1.4.1/openedx_ledger/migrations/0003_field_updates_20230216_1605.py
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-03-20 11:27:39.000000 openedx-ledger-1.4.1/openedx_ledger/migrations/0004_ledger_idpkey_blankable.py
--rw-r--r--   0 runner    (1001) docker     (127)    12708 2024-03-20 11:27:39.000000 openedx-ledger-1.4.1/openedx_ledger/migrations/0005_help_text_and_more_indices.py
--rw-r--r--   0 runner    (1001) docker     (127)     4291 2024-03-20 11:27:39.000000 openedx-ledger-1.4.1/openedx_ledger/migrations/0006_auto_20230404_1744.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-03-20 11:27:39.000000 openedx-ledger-1.4.1/openedx_ledger/migrations/0007_alter_externalfulfillmentprovider_name.py
--rw-r--r--   0 runner    (1001) docker     (127)     5826 2024-03-20 11:27:39.000000 openedx-ledger-1.4.1/openedx_ledger/migrations/0008_adjustment_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-03-20 11:27:39.000000 openedx-ledger-1.4.1/openedx_ledger/migrations/0009_add_email_and_title_to_transactions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-03-20 11:27:39.000000 openedx-ledger-1.4.1/openedx_ledger/migrations/0010_transaction_parent_content_key.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 11:27:39.000000 openedx-ledger-1.4.1/openedx_ledger/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20287 2024-03-20 11:27:39.000000 openedx-ledger-1.4.1/openedx_ledger/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 11:27:49.747439 openedx-ledger-1.4.1/openedx_ledger/signals/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 11:27:39.000000 openedx-ledger-1.4.1/openedx_ledger/signals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-03-20 11:27:39.000000 openedx-ledger-1.4.1/openedx_ledger/signals/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 11:27:49.743440 openedx-ledger-1.4.1/openedx_ledger/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 11:27:49.751440 openedx-ledger-1.4.1/openedx_ledger/templates/edx_ledger/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 11:27:49.751440 openedx-ledger-1.4.1/openedx_ledger/templates/edx_ledger/admin/
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-03-20 11:27:39.000000 openedx-ledger-1.4.1/openedx_ledger/templates/edx_ledger/admin/reverse_transaction.html
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-03-20 11:27:39.000000 openedx-ledger-1.4.1/openedx_ledger/templates/edx_ledger/base.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 11:27:49.751440 openedx-ledger-1.4.1/openedx_ledger/test_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-03-20 11:27:39.000000 openedx-ledger-1.4.1/openedx_ledger/test_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-03-20 11:27:39.000000 openedx-ledger-1.4.1/openedx_ledger/test_utils/factories.py
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-03-20 11:27:39.000000 openedx-ledger-1.4.1/openedx_ledger/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-03-20 11:27:39.000000 openedx-ledger-1.4.1/openedx_ledger/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-03-20 11:27:39.000000 openedx-ledger-1.4.1/openedx_ledger/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 11:27:49.751440 openedx-ledger-1.4.1/openedx_ledger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9760 2024-03-20 11:27:49.000000 openedx-ledger-1.4.1/openedx_ledger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-03-20 11:27:49.000000 openedx-ledger-1.4.1/openedx_ledger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 11:27:49.000000 openedx-ledger-1.4.1/openedx_ledger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 11:27:49.000000 openedx-ledger-1.4.1/openedx_ledger.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-03-20 11:27:49.000000 openedx-ledger-1.4.1/openedx_ledger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-20 11:27:49.000000 openedx-ledger-1.4.1/openedx_ledger.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 11:27:49.751440 openedx-ledger-1.4.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-03-20 11:27:39.000000 openedx-ledger-1.4.1/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-03-20 11:27:39.000000 openedx-ledger-1.4.1/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-03-20 11:27:49.751440 openedx-ledger-1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     6703 2024-03-20 11:27:39.000000 openedx-ledger-1.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 11:27:49.751440 openedx-ledger-1.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5140 2024-03-20 11:27:39.000000 openedx-ledger-1.4.1/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7642 2024-03-20 11:27:39.000000 openedx-ledger-1.4.1/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-03-20 11:27:39.000000 openedx-ledger-1.4.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:45:23.835092 openedx_ledger-1.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-04-16 13:45:20.000000 openedx_ledger-1.4.2/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    35139 2024-04-16 13:45:20.000000 openedx_ledger-1.4.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-16 13:45:20.000000 openedx_ledger-1.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9804 2024-04-16 13:45:23.835092 openedx_ledger-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5964 2024-04-16 13:45:20.000000 openedx_ledger-1.4.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:45:23.831092 openedx_ledger-1.4.2/openedx_ledger/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-16 13:45:20.000000 openedx_ledger-1.4.2/openedx_ledger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10060 2024-04-16 13:45:20.000000 openedx_ledger-1.4.2/openedx_ledger/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8979 2024-04-16 13:45:20.000000 openedx_ledger-1.4.2/openedx_ledger/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-16 13:45:20.000000 openedx_ledger-1.4.2/openedx_ledger/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-16 13:45:20.000000 openedx_ledger-1.4.2/openedx_ledger/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:45:23.835092 openedx_ledger-1.4.2/openedx_ledger/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-04-16 13:45:20.000000 openedx_ledger-1.4.2/openedx_ledger/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6005 2024-04-16 13:45:20.000000 openedx_ledger-1.4.2/openedx_ledger/migrations/0002_historicalledger_historicalreversal_historicaltransaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4294 2024-04-16 13:45:20.000000 openedx_ledger-1.4.2/openedx_ledger/migrations/0003_field_updates_20230216_1605.py
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-16 13:45:20.000000 openedx_ledger-1.4.2/openedx_ledger/migrations/0004_ledger_idpkey_blankable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12708 2024-04-16 13:45:20.000000 openedx_ledger-1.4.2/openedx_ledger/migrations/0005_help_text_and_more_indices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4291 2024-04-16 13:45:20.000000 openedx_ledger-1.4.2/openedx_ledger/migrations/0006_auto_20230404_1744.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-16 13:45:20.000000 openedx_ledger-1.4.2/openedx_ledger/migrations/0007_alter_externalfulfillmentprovider_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5826 2024-04-16 13:45:20.000000 openedx_ledger-1.4.2/openedx_ledger/migrations/0008_adjustment_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-16 13:45:20.000000 openedx_ledger-1.4.2/openedx_ledger/migrations/0009_add_email_and_title_to_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-16 13:45:20.000000 openedx_ledger-1.4.2/openedx_ledger/migrations/0010_transaction_parent_content_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 13:45:20.000000 openedx_ledger-1.4.2/openedx_ledger/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20287 2024-04-16 13:45:20.000000 openedx_ledger-1.4.2/openedx_ledger/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:45:23.835092 openedx_ledger-1.4.2/openedx_ledger/signals/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 13:45:20.000000 openedx_ledger-1.4.2/openedx_ledger/signals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-16 13:45:20.000000 openedx_ledger-1.4.2/openedx_ledger/signals/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:45:23.831092 openedx_ledger-1.4.2/openedx_ledger/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:45:23.835092 openedx_ledger-1.4.2/openedx_ledger/templates/edx_ledger/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:45:23.835092 openedx_ledger-1.4.2/openedx_ledger/templates/edx_ledger/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-16 13:45:20.000000 openedx_ledger-1.4.2/openedx_ledger/templates/edx_ledger/admin/reverse_transaction.html
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-16 13:45:20.000000 openedx_ledger-1.4.2/openedx_ledger/templates/edx_ledger/base.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:45:23.835092 openedx_ledger-1.4.2/openedx_ledger/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-16 13:45:20.000000 openedx_ledger-1.4.2/openedx_ledger/test_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-04-16 13:45:20.000000 openedx_ledger-1.4.2/openedx_ledger/test_utils/factories.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-16 13:45:20.000000 openedx_ledger-1.4.2/openedx_ledger/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-16 13:45:20.000000 openedx_ledger-1.4.2/openedx_ledger/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-04-16 13:45:20.000000 openedx_ledger-1.4.2/openedx_ledger/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:45:23.835092 openedx_ledger-1.4.2/openedx_ledger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9804 2024-04-16 13:45:23.000000 openedx_ledger-1.4.2/openedx_ledger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-16 13:45:23.000000 openedx_ledger-1.4.2/openedx_ledger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 13:45:23.000000 openedx_ledger-1.4.2/openedx_ledger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 13:45:23.000000 openedx_ledger-1.4.2/openedx_ledger.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-16 13:45:23.000000 openedx_ledger-1.4.2/openedx_ledger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-16 13:45:23.000000 openedx_ledger-1.4.2/openedx_ledger.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:45:23.835092 openedx_ledger-1.4.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-16 13:45:20.000000 openedx_ledger-1.4.2/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-16 13:45:20.000000 openedx_ledger-1.4.2/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-16 13:45:23.835092 openedx_ledger-1.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     6703 2024-04-16 13:45:20.000000 openedx_ledger-1.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:45:23.835092 openedx_ledger-1.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5140 2024-04-16 13:45:20.000000 openedx_ledger-1.4.2/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7642 2024-04-16 13:45:20.000000 openedx_ledger-1.4.2/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-04-16 13:45:20.000000 openedx_ledger-1.4.2/tests/test_utils.py
```

### Comparing `openedx-ledger-1.4.1/CHANGELOG.rst` & `openedx_ledger-1.4.2/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,18 @@
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 * Nothing unreleased
 
+[1.4.2]
+*******
+* feat: Dependency updates
+
 [1.4.1]
 *******
 * feat: Add python 3.12 support
 
 [1.4.0]
 *******
 * feat: Add parent_content_key field to Transaction model (ENT-8389)
```

### Comparing `openedx-ledger-1.4.1/LICENSE.txt` & `openedx_ledger-1.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openedx-ledger-1.4.1/PKG-INFO` & `openedx_ledger-1.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openedx-ledger
-Version: 1.4.1
+Version: 1.4.2
 Summary: Records transactions against a ledger, denominated in units of value.
 Home-page: https://github.com/openedx/openedx-ledger
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -222,14 +222,18 @@
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 * Nothing unreleased
 
+[1.4.2]
+*******
+* feat: Dependency updates
+
 [1.4.1]
 *******
 * feat: Add python 3.12 support
 
 [1.4.0]
 *******
 * feat: Add parent_content_key field to Transaction model (ENT-8389)
```

### Comparing `openedx-ledger-1.4.1/README.rst` & `openedx_ledger-1.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `openedx-ledger-1.4.1/openedx_ledger/admin.py` & `openedx_ledger-1.4.2/openedx_ledger/admin.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-1.4.1/openedx_ledger/api.py` & `openedx_ledger-1.4.2/openedx_ledger/api.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-1.4.1/openedx_ledger/migrations/0001_initial.py` & `openedx_ledger-1.4.2/openedx_ledger/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-1.4.1/openedx_ledger/migrations/0002_historicalledger_historicalreversal_historicaltransaction.py` & `openedx_ledger-1.4.2/openedx_ledger/migrations/0002_historicalledger_historicalreversal_historicaltransaction.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-1.4.1/openedx_ledger/migrations/0003_field_updates_20230216_1605.py` & `openedx_ledger-1.4.2/openedx_ledger/migrations/0003_field_updates_20230216_1605.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-1.4.1/openedx_ledger/migrations/0004_ledger_idpkey_blankable.py` & `openedx_ledger-1.4.2/openedx_ledger/migrations/0004_ledger_idpkey_blankable.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-1.4.1/openedx_ledger/migrations/0005_help_text_and_more_indices.py` & `openedx_ledger-1.4.2/openedx_ledger/migrations/0005_help_text_and_more_indices.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-1.4.1/openedx_ledger/migrations/0006_auto_20230404_1744.py` & `openedx_ledger-1.4.2/openedx_ledger/migrations/0006_auto_20230404_1744.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-1.4.1/openedx_ledger/migrations/0008_adjustment_model.py` & `openedx_ledger-1.4.2/openedx_ledger/migrations/0008_adjustment_model.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-1.4.1/openedx_ledger/migrations/0009_add_email_and_title_to_transactions.py` & `openedx_ledger-1.4.2/openedx_ledger/migrations/0009_add_email_and_title_to_transactions.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-1.4.1/openedx_ledger/migrations/0010_transaction_parent_content_key.py` & `openedx_ledger-1.4.2/openedx_ledger/migrations/0010_transaction_parent_content_key.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-1.4.1/openedx_ledger/models.py` & `openedx_ledger-1.4.2/openedx_ledger/models.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-1.4.1/openedx_ledger/templates/edx_ledger/admin/reverse_transaction.html` & `openedx_ledger-1.4.2/openedx_ledger/templates/edx_ledger/admin/reverse_transaction.html`

 * *Files identical despite different names*

### Comparing `openedx-ledger-1.4.1/openedx_ledger/templates/edx_ledger/base.html` & `openedx_ledger-1.4.2/openedx_ledger/templates/edx_ledger/base.html`

 * *Files identical despite different names*

### Comparing `openedx-ledger-1.4.1/openedx_ledger/test_utils/factories.py` & `openedx_ledger-1.4.2/openedx_ledger/test_utils/factories.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-1.4.1/openedx_ledger/utils.py` & `openedx_ledger-1.4.2/openedx_ledger/utils.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-1.4.1/openedx_ledger/views.py` & `openedx_ledger-1.4.2/openedx_ledger/views.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-1.4.1/openedx_ledger.egg-info/PKG-INFO` & `openedx_ledger-1.4.2/openedx_ledger.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openedx-ledger
-Version: 1.4.1
+Version: 1.4.2
 Summary: Records transactions against a ledger, denominated in units of value.
 Home-page: https://github.com/openedx/openedx-ledger
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -222,14 +222,18 @@
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 * Nothing unreleased
 
+[1.4.2]
+*******
+* feat: Dependency updates
+
 [1.4.1]
 *******
 * feat: Add python 3.12 support
 
 [1.4.0]
 *******
 * feat: Add parent_content_key field to Transaction model (ENT-8389)
```

### Comparing `openedx-ledger-1.4.1/openedx_ledger.egg-info/SOURCES.txt` & `openedx_ledger-1.4.2/openedx_ledger.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openedx-ledger-1.4.1/setup.py` & `openedx_ledger-1.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-1.4.1/tests/test_api.py` & `openedx_ledger-1.4.2/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-1.4.1/tests/test_models.py` & `openedx_ledger-1.4.2/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-1.4.1/tests/test_utils.py` & `openedx_ledger-1.4.2/tests/test_utils.py`

 * *Files identical despite different names*

