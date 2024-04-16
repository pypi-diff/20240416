# Comparing `tmp/baseapp-notifications-0.2.4.tar.gz` & `tmp/baseapp-notifications-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baseapp-notifications-0.2.4.tar", last modified: Thu Apr 11 19:03:56 2024, max compression
+gzip compressed data, was "baseapp-notifications-0.2.5.tar", last modified: Tue Apr 16 11:36:22 2024, max compression
```

## Comparing `baseapp-notifications-0.2.4.tar` & `baseapp-notifications-0.2.5.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:03:56.518541 baseapp-notifications-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-11 19:03:54.000000 baseapp-notifications-0.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    13400 2024-04-11 19:03:56.518541 baseapp-notifications-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10365 2024-04-11 19:03:54.000000 baseapp-notifications-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:03:56.514541 baseapp-notifications-0.2.4/baseapp_notifications/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-11 19:03:54.000000 baseapp-notifications-0.2.4/baseapp_notifications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-11 19:03:54.000000 baseapp-notifications-0.2.4/baseapp_notifications/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-11 19:03:54.000000 baseapp-notifications-0.2.4/baseapp_notifications/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-11 19:03:54.000000 baseapp-notifications-0.2.4/baseapp_notifications/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:03:56.518541 baseapp-notifications-0.2.4/baseapp_notifications/graphql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 19:03:54.000000 baseapp-notifications-0.2.4/baseapp_notifications/graphql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-11 19:03:54.000000 baseapp-notifications-0.2.4/baseapp_notifications/graphql/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-04-11 19:03:54.000000 baseapp-notifications-0.2.4/baseapp_notifications/graphql/mutations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-04-11 19:03:54.000000 baseapp-notifications-0.2.4/baseapp_notifications/graphql/object_types.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 19:03:54.000000 baseapp-notifications-0.2.4/baseapp_notifications/graphql/queries.py
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-04-11 19:03:54.000000 baseapp-notifications-0.2.4/baseapp_notifications/graphql/subscriptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:03:56.518541 baseapp-notifications-0.2.4/baseapp_notifications/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-04-11 19:03:54.000000 baseapp-notifications-0.2.4/baseapp_notifications/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-11 19:03:54.000000 baseapp-notifications-0.2.4/baseapp_notifications/migrations/0002_notificationsetting.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 19:03:54.000000 baseapp-notifications-0.2.4/baseapp_notifications/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-11 19:03:54.000000 baseapp-notifications-0.2.4/baseapp_notifications/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-04-11 19:03:54.000000 baseapp-notifications-0.2.4/baseapp_notifications/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:03:56.514541 baseapp-notifications-0.2.4/baseapp_notifications/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:03:56.518541 baseapp-notifications-0.2.4/baseapp_notifications/templates/emails/
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-11 19:03:54.000000 baseapp-notifications-0.2.4/baseapp_notifications/templates/emails/notification-body.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-11 19:03:54.000000 baseapp-notifications-0.2.4/baseapp_notifications/templates/emails/notification-body.txt.j2
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-11 19:03:54.000000 baseapp-notifications-0.2.4/baseapp_notifications/templates/emails/notification-subject.txt.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:03:56.518541 baseapp-notifications-0.2.4/baseapp_notifications/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 19:03:54.000000 baseapp-notifications-0.2.4/baseapp_notifications/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-11 19:03:54.000000 baseapp-notifications-0.2.4/baseapp_notifications/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-11 19:03:54.000000 baseapp-notifications-0.2.4/baseapp_notifications/tests/factories.py
--rw-r--r--   0 runner    (1001) docker     (127)    10430 2024-04-11 19:03:54.000000 baseapp-notifications-0.2.4/baseapp_notifications/tests/test_graphql_mutations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-04-11 19:03:54.000000 baseapp-notifications-0.2.4/baseapp_notifications/tests/test_graphql_queries.py
--rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-04-11 19:03:54.000000 baseapp-notifications-0.2.4/baseapp_notifications/tests/test_graphql_subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-04-11 19:03:54.000000 baseapp-notifications-0.2.4/baseapp_notifications/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4471 2024-04-11 19:03:54.000000 baseapp-notifications-0.2.4/baseapp_notifications/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:03:56.514541 baseapp-notifications-0.2.4/baseapp_notifications.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13400 2024-04-11 19:03:56.000000 baseapp-notifications-0.2.4/baseapp_notifications.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-04-11 19:03:56.000000 baseapp-notifications-0.2.4/baseapp_notifications.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 19:03:56.000000 baseapp-notifications-0.2.4/baseapp_notifications.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-11 19:03:56.000000 baseapp-notifications-0.2.4/baseapp_notifications.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-11 19:03:56.000000 baseapp-notifications-0.2.4/baseapp_notifications.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-11 19:03:54.000000 baseapp-notifications-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-11 19:03:56.518541 baseapp-notifications-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-11 19:03:54.000000 baseapp-notifications-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:03:56.518541 baseapp-notifications-0.2.4/testproject/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 19:03:54.000000 baseapp-notifications-0.2.4/testproject/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-11 19:03:54.000000 baseapp-notifications-0.2.4/testproject/graphql.py
--rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-04-11 19:03:54.000000 baseapp-notifications-0.2.4/testproject/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 19:03:54.000000 baseapp-notifications-0.2.4/testproject/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-11 19:03:54.000000 baseapp-notifications-0.2.4/testproject/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-11 19:03:54.000000 baseapp-notifications-0.2.4/testproject/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:36:22.909184 baseapp-notifications-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-16 11:36:22.000000 baseapp-notifications-0.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    13400 2024-04-16 11:36:22.909184 baseapp-notifications-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10365 2024-04-16 11:36:22.000000 baseapp-notifications-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:36:22.905184 baseapp-notifications-0.2.5/baseapp_notifications/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-16 11:36:22.000000 baseapp-notifications-0.2.5/baseapp_notifications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-16 11:36:22.000000 baseapp-notifications-0.2.5/baseapp_notifications/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-16 11:36:22.000000 baseapp-notifications-0.2.5/baseapp_notifications/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-16 11:36:22.000000 baseapp-notifications-0.2.5/baseapp_notifications/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:36:22.905184 baseapp-notifications-0.2.5/baseapp_notifications/graphql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 11:36:22.000000 baseapp-notifications-0.2.5/baseapp_notifications/graphql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-16 11:36:22.000000 baseapp-notifications-0.2.5/baseapp_notifications/graphql/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-04-16 11:36:22.000000 baseapp-notifications-0.2.5/baseapp_notifications/graphql/mutations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-04-16 11:36:22.000000 baseapp-notifications-0.2.5/baseapp_notifications/graphql/object_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 11:36:22.000000 baseapp-notifications-0.2.5/baseapp_notifications/graphql/queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-04-16 11:36:22.000000 baseapp-notifications-0.2.5/baseapp_notifications/graphql/subscriptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:36:22.905184 baseapp-notifications-0.2.5/baseapp_notifications/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-04-16 11:36:22.000000 baseapp-notifications-0.2.5/baseapp_notifications/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-16 11:36:22.000000 baseapp-notifications-0.2.5/baseapp_notifications/migrations/0002_notificationsetting.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 11:36:22.000000 baseapp-notifications-0.2.5/baseapp_notifications/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-16 11:36:22.000000 baseapp-notifications-0.2.5/baseapp_notifications/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-04-16 11:36:22.000000 baseapp-notifications-0.2.5/baseapp_notifications/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:36:22.901184 baseapp-notifications-0.2.5/baseapp_notifications/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:36:22.905184 baseapp-notifications-0.2.5/baseapp_notifications/templates/emails/
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-16 11:36:22.000000 baseapp-notifications-0.2.5/baseapp_notifications/templates/emails/notification-body.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-16 11:36:22.000000 baseapp-notifications-0.2.5/baseapp_notifications/templates/emails/notification-body.txt.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-16 11:36:22.000000 baseapp-notifications-0.2.5/baseapp_notifications/templates/emails/notification-subject.txt.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:36:22.909184 baseapp-notifications-0.2.5/baseapp_notifications/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 11:36:22.000000 baseapp-notifications-0.2.5/baseapp_notifications/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-16 11:36:22.000000 baseapp-notifications-0.2.5/baseapp_notifications/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-16 11:36:22.000000 baseapp-notifications-0.2.5/baseapp_notifications/tests/factories.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10430 2024-04-16 11:36:22.000000 baseapp-notifications-0.2.5/baseapp_notifications/tests/test_graphql_mutations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-04-16 11:36:22.000000 baseapp-notifications-0.2.5/baseapp_notifications/tests/test_graphql_queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-04-16 11:36:22.000000 baseapp-notifications-0.2.5/baseapp_notifications/tests/test_graphql_subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-04-16 11:36:22.000000 baseapp-notifications-0.2.5/baseapp_notifications/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4471 2024-04-16 11:36:22.000000 baseapp-notifications-0.2.5/baseapp_notifications/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:36:22.905184 baseapp-notifications-0.2.5/baseapp_notifications.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13400 2024-04-16 11:36:22.000000 baseapp-notifications-0.2.5/baseapp_notifications.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-04-16 11:36:22.000000 baseapp-notifications-0.2.5/baseapp_notifications.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 11:36:22.000000 baseapp-notifications-0.2.5/baseapp_notifications.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-16 11:36:22.000000 baseapp-notifications-0.2.5/baseapp_notifications.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-16 11:36:22.000000 baseapp-notifications-0.2.5/baseapp_notifications.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-16 11:36:22.000000 baseapp-notifications-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-16 11:36:22.909184 baseapp-notifications-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-16 11:36:22.000000 baseapp-notifications-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:36:22.909184 baseapp-notifications-0.2.5/testproject/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 11:36:22.000000 baseapp-notifications-0.2.5/testproject/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-16 11:36:22.000000 baseapp-notifications-0.2.5/testproject/graphql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-04-16 11:36:22.000000 baseapp-notifications-0.2.5/testproject/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 11:36:22.000000 baseapp-notifications-0.2.5/testproject/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-16 11:36:22.000000 baseapp-notifications-0.2.5/testproject/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-16 11:36:22.000000 baseapp-notifications-0.2.5/testproject/wsgi.py
```

### Comparing `baseapp-notifications-0.2.4/PKG-INFO` & `baseapp-notifications-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baseapp-notifications
-Version: 0.2.4
+Version: 0.2.5
 Summary: BaseApp Notifications
 Home-page: https://github.com/silverlogic/baseapp-backend
 Author: The SilverLogic
 Author-email: dev@tsl.io
 License: BSD-3-Clause  # Example license
 Description: # BaseApp Notifications
```

### Comparing `baseapp-notifications-0.2.4/README.md` & `baseapp-notifications-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `baseapp-notifications-0.2.4/baseapp_notifications/base.py` & `baseapp-notifications-0.2.5/baseapp_notifications/base.py`

 * *Files identical despite different names*

### Comparing `baseapp-notifications-0.2.4/baseapp_notifications/graphql/mutations.py` & `baseapp-notifications-0.2.5/baseapp_notifications/graphql/mutations.py`

 * *Files identical despite different names*

### Comparing `baseapp-notifications-0.2.4/baseapp_notifications/graphql/object_types.py` & `baseapp-notifications-0.2.5/baseapp_notifications/graphql/object_types.py`

 * *Files identical despite different names*

### Comparing `baseapp-notifications-0.2.4/baseapp_notifications/graphql/subscriptions.py` & `baseapp-notifications-0.2.5/baseapp_notifications/graphql/subscriptions.py`

 * *Files identical despite different names*

### Comparing `baseapp-notifications-0.2.4/baseapp_notifications/migrations/0001_initial.py` & `baseapp-notifications-0.2.5/baseapp_notifications/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `baseapp-notifications-0.2.4/baseapp_notifications/migrations/0002_notificationsetting.py` & `baseapp-notifications-0.2.5/baseapp_notifications/migrations/0002_notificationsetting.py`

 * *Files identical despite different names*

### Comparing `baseapp-notifications-0.2.4/baseapp_notifications/tasks.py` & `baseapp-notifications-0.2.5/baseapp_notifications/tasks.py`

 * *Files identical despite different names*

### Comparing `baseapp-notifications-0.2.4/baseapp_notifications/templates/emails/notification-body.html.j2` & `baseapp-notifications-0.2.5/baseapp_notifications/templates/emails/notification-body.html.j2`

 * *Files identical despite different names*

### Comparing `baseapp-notifications-0.2.4/baseapp_notifications/tests/factories.py` & `baseapp-notifications-0.2.5/baseapp_notifications/tests/factories.py`

 * *Files identical despite different names*

### Comparing `baseapp-notifications-0.2.4/baseapp_notifications/tests/test_graphql_mutations.py` & `baseapp-notifications-0.2.5/baseapp_notifications/tests/test_graphql_mutations.py`

 * *Files identical despite different names*

### Comparing `baseapp-notifications-0.2.4/baseapp_notifications/tests/test_graphql_queries.py` & `baseapp-notifications-0.2.5/baseapp_notifications/tests/test_graphql_queries.py`

 * *Files identical despite different names*

### Comparing `baseapp-notifications-0.2.4/baseapp_notifications/tests/test_graphql_subscriptions.py` & `baseapp-notifications-0.2.5/baseapp_notifications/tests/test_graphql_subscriptions.py`

 * *Files identical despite different names*

### Comparing `baseapp-notifications-0.2.4/baseapp_notifications/tests/test_utils.py` & `baseapp-notifications-0.2.5/baseapp_notifications/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `baseapp-notifications-0.2.4/baseapp_notifications/utils.py` & `baseapp-notifications-0.2.5/baseapp_notifications/utils.py`

 * *Files identical despite different names*

### Comparing `baseapp-notifications-0.2.4/baseapp_notifications.egg-info/PKG-INFO` & `baseapp-notifications-0.2.5/baseapp_notifications.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baseapp-notifications
-Version: 0.2.4
+Version: 0.2.5
 Summary: BaseApp Notifications
 Home-page: https://github.com/silverlogic/baseapp-backend
 Author: The SilverLogic
 Author-email: dev@tsl.io
 License: BSD-3-Clause  # Example license
 Description: # BaseApp Notifications
```

### Comparing `baseapp-notifications-0.2.4/baseapp_notifications.egg-info/SOURCES.txt` & `baseapp-notifications-0.2.5/baseapp_notifications.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `baseapp-notifications-0.2.4/setup.cfg` & `baseapp-notifications-0.2.5/setup.cfg`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = baseapp_notifications
-version = 0.2.4
+version = 0.2.5
 description = BaseApp Notifications
 long_description = file: README.md
 url = https://github.com/silverlogic/baseapp-backend
 author = The SilverLogic
 author_email = dev@tsl.io
 license = BSD-3-Clause  # Example license
 
@@ -12,15 +12,15 @@
 include_package_data = true
 packages = find:
 python_requires = >=3.9
 install_requires = 
 	baseapp-core[graphql] >= 0.2.11
 	djmail >= 2.0
 	django-notifications-hq >= 1.8
-	django-push-notifications[WP,APNS_ASYNC] @ git+https://github.com/silverlogic/django-push-notifications.git@820599c17c74e59f0e19c10fd4de8dee50671cbe
+	baseapp-django-push-notifications[WP,APNS_ASYNC] == 3.0.3rc2
 
 [options.package_data]
 baseapp_notifications = 
 	*.j2
 	*.html
 	*.png
```

### Comparing `baseapp-notifications-0.2.4/testproject/graphql.py` & `baseapp-notifications-0.2.5/testproject/graphql.py`

 * *Files identical despite different names*

### Comparing `baseapp-notifications-0.2.4/testproject/settings.py` & `baseapp-notifications-0.2.5/testproject/settings.py`

 * *Files identical despite different names*

