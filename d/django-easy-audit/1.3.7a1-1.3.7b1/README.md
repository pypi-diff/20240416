# Comparing `tmp/django_easy_audit-1.3.7a1.tar.gz` & `tmp/django_easy_audit-1.3.7b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_easy_audit-1.3.7a1.tar", max compression
+gzip compressed data, was "django_easy_audit-1.3.7b1.tar", max compression
```

## Comparing `django_easy_audit-1.3.7a1.tar` & `django_easy_audit-1.3.7b1.tar`

### file list

```diff
@@ -1,48 +1,49 @@
--rw-r--r--   0        0        0    35141 2023-08-21 13:56:07.207792 django_easy_audit-1.3.7a1/LICENSE
--rw-r--r--   0        0        0     8759 2024-03-18 20:11:05.417037 django_easy_audit-1.3.7a1/README.md
--rw-r--r--   0        0        0        0 2024-03-18 20:11:05.417037 django_easy_audit-1.3.7a1/easyaudit/__init__.py
--rw-r--r--   0        0        0     5534 2024-03-18 20:11:05.417037 django_easy_audit-1.3.7a1/easyaudit/admin.py
--rw-r--r--   0        0        0     5037 2024-03-18 20:11:05.417037 django_easy_audit-1.3.7a1/easyaudit/admin_helpers.py
--rw-r--r--   0        0        0      359 2024-03-18 20:11:05.417037 django_easy_audit-1.3.7a1/easyaudit/apps.py
--rw-r--r--   0        0        0      411 2024-03-18 20:11:05.417037 django_easy_audit-1.3.7a1/easyaudit/backends.py
--rw-r--r--   0        0        0     3490 2024-03-18 20:11:05.417037 django_easy_audit-1.3.7a1/easyaudit/crudhistory_admin_mixin.py
--rw-r--r--   0        0        0     3170 2023-08-21 13:56:07.207792 django_easy_audit-1.3.7a1/easyaudit/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     6139 2023-08-21 13:56:07.207792 django_easy_audit-1.3.7a1/easyaudit/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2943 2023-08-21 13:56:07.207792 django_easy_audit-1.3.7a1/easyaudit/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     4185 2023-08-21 13:56:07.207792 django_easy_audit-1.3.7a1/easyaudit/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3376 2023-08-21 13:56:07.207792 django_easy_audit-1.3.7a1/easyaudit/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     4622 2023-08-21 13:56:07.207792 django_easy_audit-1.3.7a1/easyaudit/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2023-08-21 13:56:07.207792 django_easy_audit-1.3.7a1/easyaudit/middleware/__init__.py
--rw-r--r--   0        0        0     1799 2024-03-18 20:11:05.417037 django_easy_audit-1.3.7a1/easyaudit/middleware/easyaudit.py
--rw-r--r--   0        0        0     2225 2024-03-18 20:11:05.417037 django_easy_audit-1.3.7a1/easyaudit/migrations/0001_initial.py
--rw-r--r--   0        0        0      748 2024-03-18 20:11:05.417037 django_easy_audit-1.3.7a1/easyaudit/migrations/0002_auto_20170125_0759.py
--rw-r--r--   0        0        0      773 2024-03-18 20:11:05.417037 django_easy_audit-1.3.7a1/easyaudit/migrations/0003_auto_20170228_1505.py
--rw-r--r--   0        0        0      432 2024-03-18 20:11:05.417037 django_easy_audit-1.3.7a1/easyaudit/migrations/0004_auto_20170620_1354.py
--rw-r--r--   0        0        0      513 2024-03-18 20:11:05.417037 django_easy_audit-1.3.7a1/easyaudit/migrations/0005_auto_20170713_1155.py
--rw-r--r--   0        0        0     1499 2024-03-18 20:11:05.417037 django_easy_audit-1.3.7a1/easyaudit/migrations/0006_auto_20171018_1242.py
--rw-r--r--   0        0        0      956 2024-03-18 20:11:05.417037 django_easy_audit-1.3.7a1/easyaudit/migrations/0007_auto_20180105_0838.py
--rw-r--r--   0        0        0      640 2024-03-18 20:11:05.417037 django_easy_audit-1.3.7a1/easyaudit/migrations/0008_auto_20180220_1908.py
--rw-r--r--   0        0        0      570 2024-03-18 20:11:05.417037 django_easy_audit-1.3.7a1/easyaudit/migrations/0009_auto_20180314_2225.py
--rw-r--r--   0        0        0      404 2023-08-21 13:56:07.207792 django_easy_audit-1.3.7a1/easyaudit/migrations/0010_repr_text.py
--rw-r--r--   0        0        0      368 2024-03-18 20:11:05.417037 django_easy_audit-1.3.7a1/easyaudit/migrations/0011_auto_20181101_1339.py
--rw-r--r--   0        0        0     1455 2024-03-18 20:11:05.417037 django_easy_audit-1.3.7a1/easyaudit/migrations/0012_auto_20181018_0012.py
--rw-r--r--   0        0        0      700 2023-08-21 13:56:07.207792 django_easy_audit-1.3.7a1/easyaudit/migrations/0013_auto_20190723_0126.py
--rw-r--r--   0        0        0      395 2023-08-21 13:56:07.207792 django_easy_audit-1.3.7a1/easyaudit/migrations/0014_auto_20200513_0008.py
--rw-r--r--   0        0        0     5081 2023-08-21 13:56:07.207792 django_easy_audit-1.3.7a1/easyaudit/migrations/0015_auto_20201019_1217.py
--rw-r--r--   0        0        0      721 2023-08-21 13:56:07.207792 django_easy_audit-1.3.7a1/easyaudit/migrations/0016_alter_crudevent_event_type.py
--rw-r--r--   0        0        0      453 2023-08-21 13:56:07.207792 django_easy_audit-1.3.7a1/easyaudit/migrations/0017_alter_requestevent_datetime.py
--rw-r--r--   0        0        0      424 2024-03-18 20:11:05.417037 django_easy_audit-1.3.7a1/easyaudit/migrations/0018_rename_crudevent_object_id_content_type_index.py
--rw-r--r--   0        0        0     1989 2024-03-18 20:11:05.417037 django_easy_audit-1.3.7a1/easyaudit/migrations/0019_alter_crudevent_changed_fields_and_more.py
--rw-r--r--   0        0        0        0 2023-08-21 13:56:07.207792 django_easy_audit-1.3.7a1/easyaudit/migrations/__init__.py
--rw-r--r--   0        0        0     4391 2024-03-18 20:11:05.417037 django_easy_audit-1.3.7a1/easyaudit/models.py
--rw-r--r--   0        0        0     6668 2024-03-18 20:11:05.417037 django_easy_audit-1.3.7a1/easyaudit/settings.py
--rw-r--r--   0        0        0        0 2023-08-21 13:56:07.207792 django_easy_audit-1.3.7a1/easyaudit/signals/__init__.py
--rw-r--r--   0        0        0     2486 2024-03-18 20:11:05.417037 django_easy_audit-1.3.7a1/easyaudit/signals/auth_signals.py
--rw-r--r--   0        0        0     3692 2024-03-18 20:11:05.417037 django_easy_audit-1.3.7a1/easyaudit/signals/crud_flows.py
--rw-r--r--   0        0        0     8905 2024-03-18 20:11:05.417037 django_easy_audit-1.3.7a1/easyaudit/signals/model_signals.py
--rw-r--r--   0        0        0     3263 2024-03-18 20:11:05.417037 django_easy_audit-1.3.7a1/easyaudit/signals/request_signals.py
--rw-r--r--   0        0        0      558 2024-03-18 20:11:05.417037 django_easy_audit-1.3.7a1/easyaudit/templates/admin/easyaudit/change_list.html
--rw-r--r--   0        0        0     1488 2024-03-18 20:11:05.417037 django_easy_audit-1.3.7a1/easyaudit/templates/admin/easyaudit/purge_confirmation.html
--rw-r--r--   0        0        0     2825 2024-03-18 20:11:05.417037 django_easy_audit-1.3.7a1/easyaudit/utils.py
--rw-r--r--   0        0        0     3254 2024-03-18 20:11:24.289145 django_easy_audit-1.3.7a1/pyproject.toml
--rw-r--r--   0        0        0    10075 1970-01-01 00:00:00.000000 django_easy_audit-1.3.7a1/PKG-INFO
+-rw-r--r--   0        0        0    35141 2023-08-21 13:56:07.207792 django_easy_audit-1.3.7b1/LICENSE
+-rw-r--r--   0        0        0     8759 2024-03-18 20:11:05.417037 django_easy_audit-1.3.7b1/README.md
+-rw-r--r--   0        0        0        0 2024-03-18 20:11:05.417037 django_easy_audit-1.3.7b1/easyaudit/__init__.py
+-rw-r--r--   0        0        0     5534 2024-03-18 20:11:05.417037 django_easy_audit-1.3.7b1/easyaudit/admin.py
+-rw-r--r--   0        0        0     5037 2024-03-18 20:11:05.417037 django_easy_audit-1.3.7b1/easyaudit/admin_helpers.py
+-rw-r--r--   0        0        0      359 2024-03-18 20:11:05.417037 django_easy_audit-1.3.7b1/easyaudit/apps.py
+-rw-r--r--   0        0        0      411 2024-03-18 20:11:05.417037 django_easy_audit-1.3.7b1/easyaudit/backends.py
+-rw-r--r--   0        0        0     3490 2024-03-18 20:11:05.417037 django_easy_audit-1.3.7b1/easyaudit/crudhistory_admin_mixin.py
+-rw-r--r--   0        0        0     3170 2023-08-21 13:56:07.207792 django_easy_audit-1.3.7b1/easyaudit/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     6139 2023-08-21 13:56:07.207792 django_easy_audit-1.3.7b1/easyaudit/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2943 2023-08-21 13:56:07.207792 django_easy_audit-1.3.7b1/easyaudit/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     4185 2023-08-21 13:56:07.207792 django_easy_audit-1.3.7b1/easyaudit/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3376 2023-08-21 13:56:07.207792 django_easy_audit-1.3.7b1/easyaudit/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     4622 2023-08-21 13:56:07.207792 django_easy_audit-1.3.7b1/easyaudit/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2023-08-21 13:56:07.207792 django_easy_audit-1.3.7b1/easyaudit/middleware/__init__.py
+-rw-r--r--   0        0        0     1799 2024-03-18 20:11:05.417037 django_easy_audit-1.3.7b1/easyaudit/middleware/easyaudit.py
+-rw-r--r--   0        0        0     2225 2024-03-18 20:11:05.417037 django_easy_audit-1.3.7b1/easyaudit/migrations/0001_initial.py
+-rw-r--r--   0        0        0      748 2024-03-18 20:11:05.417037 django_easy_audit-1.3.7b1/easyaudit/migrations/0002_auto_20170125_0759.py
+-rw-r--r--   0        0        0      773 2024-03-18 20:11:05.417037 django_easy_audit-1.3.7b1/easyaudit/migrations/0003_auto_20170228_1505.py
+-rw-r--r--   0        0        0      432 2024-03-18 20:11:05.417037 django_easy_audit-1.3.7b1/easyaudit/migrations/0004_auto_20170620_1354.py
+-rw-r--r--   0        0        0    12548 2024-04-16 20:20:09.665990 django_easy_audit-1.3.7b1/easyaudit/migrations/0004_auto_20170620_1354_squashed_0019_alter_crudevent_changed_fields_and_more.py
+-rw-r--r--   0        0        0      513 2024-03-18 20:11:05.417037 django_easy_audit-1.3.7b1/easyaudit/migrations/0005_auto_20170713_1155.py
+-rw-r--r--   0        0        0     1499 2024-03-18 20:11:05.417037 django_easy_audit-1.3.7b1/easyaudit/migrations/0006_auto_20171018_1242.py
+-rw-r--r--   0        0        0      956 2024-03-18 20:11:05.417037 django_easy_audit-1.3.7b1/easyaudit/migrations/0007_auto_20180105_0838.py
+-rw-r--r--   0        0        0      640 2024-03-18 20:11:05.417037 django_easy_audit-1.3.7b1/easyaudit/migrations/0008_auto_20180220_1908.py
+-rw-r--r--   0        0        0      570 2024-03-18 20:11:05.417037 django_easy_audit-1.3.7b1/easyaudit/migrations/0009_auto_20180314_2225.py
+-rw-r--r--   0        0        0      404 2023-08-21 13:56:07.207792 django_easy_audit-1.3.7b1/easyaudit/migrations/0010_repr_text.py
+-rw-r--r--   0        0        0      368 2024-03-18 20:11:05.417037 django_easy_audit-1.3.7b1/easyaudit/migrations/0011_auto_20181101_1339.py
+-rw-r--r--   0        0        0     1455 2024-03-18 20:11:05.417037 django_easy_audit-1.3.7b1/easyaudit/migrations/0012_auto_20181018_0012.py
+-rw-r--r--   0        0        0      700 2023-08-21 13:56:07.207792 django_easy_audit-1.3.7b1/easyaudit/migrations/0013_auto_20190723_0126.py
+-rw-r--r--   0        0        0      395 2023-08-21 13:56:07.207792 django_easy_audit-1.3.7b1/easyaudit/migrations/0014_auto_20200513_0008.py
+-rw-r--r--   0        0        0     5081 2023-08-21 13:56:07.207792 django_easy_audit-1.3.7b1/easyaudit/migrations/0015_auto_20201019_1217.py
+-rw-r--r--   0        0        0      721 2023-08-21 13:56:07.207792 django_easy_audit-1.3.7b1/easyaudit/migrations/0016_alter_crudevent_event_type.py
+-rw-r--r--   0        0        0      453 2023-08-21 13:56:07.207792 django_easy_audit-1.3.7b1/easyaudit/migrations/0017_alter_requestevent_datetime.py
+-rw-r--r--   0        0        0      424 2024-03-18 20:11:05.417037 django_easy_audit-1.3.7b1/easyaudit/migrations/0018_rename_crudevent_object_id_content_type_index.py
+-rw-r--r--   0        0        0     1989 2024-03-18 20:11:05.417037 django_easy_audit-1.3.7b1/easyaudit/migrations/0019_alter_crudevent_changed_fields_and_more.py
+-rw-r--r--   0        0        0        0 2023-08-21 13:56:07.207792 django_easy_audit-1.3.7b1/easyaudit/migrations/__init__.py
+-rw-r--r--   0        0        0     4391 2024-03-18 20:11:05.417037 django_easy_audit-1.3.7b1/easyaudit/models.py
+-rw-r--r--   0        0        0     6668 2024-03-18 20:11:05.417037 django_easy_audit-1.3.7b1/easyaudit/settings.py
+-rw-r--r--   0        0        0        0 2023-08-21 13:56:07.207792 django_easy_audit-1.3.7b1/easyaudit/signals/__init__.py
+-rw-r--r--   0        0        0     2486 2024-03-18 20:11:05.417037 django_easy_audit-1.3.7b1/easyaudit/signals/auth_signals.py
+-rw-r--r--   0        0        0     3692 2024-03-18 20:11:05.417037 django_easy_audit-1.3.7b1/easyaudit/signals/crud_flows.py
+-rw-r--r--   0        0        0     8905 2024-03-18 20:11:05.417037 django_easy_audit-1.3.7b1/easyaudit/signals/model_signals.py
+-rw-r--r--   0        0        0     3263 2024-03-18 20:11:05.417037 django_easy_audit-1.3.7b1/easyaudit/signals/request_signals.py
+-rw-r--r--   0        0        0      558 2024-03-18 20:11:05.417037 django_easy_audit-1.3.7b1/easyaudit/templates/admin/easyaudit/change_list.html
+-rw-r--r--   0        0        0     1488 2024-03-18 20:11:05.417037 django_easy_audit-1.3.7b1/easyaudit/templates/admin/easyaudit/purge_confirmation.html
+-rw-r--r--   0        0        0     2825 2024-03-18 20:11:05.417037 django_easy_audit-1.3.7b1/easyaudit/utils.py
+-rw-r--r--   0        0        0     3196 2024-04-16 20:20:51.422249 django_easy_audit-1.3.7b1/pyproject.toml
+-rw-r--r--   0        0        0    10075 1970-01-01 00:00:00.000000 django_easy_audit-1.3.7b1/PKG-INFO
```

### Comparing `django_easy_audit-1.3.7a1/LICENSE` & `django_easy_audit-1.3.7b1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_easy_audit-1.3.7a1/README.md` & `django_easy_audit-1.3.7b1/README.md`

 * *Files identical despite different names*

### Comparing `django_easy_audit-1.3.7a1/easyaudit/admin.py` & `django_easy_audit-1.3.7b1/easyaudit/admin.py`

 * *Files identical despite different names*

### Comparing `django_easy_audit-1.3.7a1/easyaudit/admin_helpers.py` & `django_easy_audit-1.3.7b1/easyaudit/admin_helpers.py`

 * *Files identical despite different names*

### Comparing `django_easy_audit-1.3.7a1/easyaudit/crudhistory_admin_mixin.py` & `django_easy_audit-1.3.7b1/easyaudit/crudhistory_admin_mixin.py`

 * *Files identical despite different names*

### Comparing `django_easy_audit-1.3.7a1/easyaudit/locale/de/LC_MESSAGES/django.mo` & `django_easy_audit-1.3.7b1/easyaudit/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_easy_audit-1.3.7a1/easyaudit/locale/de/LC_MESSAGES/django.po` & `django_easy_audit-1.3.7b1/easyaudit/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_easy_audit-1.3.7a1/easyaudit/locale/fr/LC_MESSAGES/django.mo` & `django_easy_audit-1.3.7b1/easyaudit/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_easy_audit-1.3.7a1/easyaudit/locale/fr/LC_MESSAGES/django.po` & `django_easy_audit-1.3.7b1/easyaudit/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_easy_audit-1.3.7a1/easyaudit/locale/ru/LC_MESSAGES/django.mo` & `django_easy_audit-1.3.7b1/easyaudit/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_easy_audit-1.3.7a1/easyaudit/locale/ru/LC_MESSAGES/django.po` & `django_easy_audit-1.3.7b1/easyaudit/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_easy_audit-1.3.7a1/easyaudit/middleware/easyaudit.py` & `django_easy_audit-1.3.7b1/easyaudit/middleware/easyaudit.py`

 * *Files identical despite different names*

### Comparing `django_easy_audit-1.3.7a1/easyaudit/migrations/0001_initial.py` & `django_easy_audit-1.3.7b1/easyaudit/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_easy_audit-1.3.7a1/easyaudit/migrations/0002_auto_20170125_0759.py` & `django_easy_audit-1.3.7b1/easyaudit/migrations/0002_auto_20170125_0759.py`

 * *Files identical despite different names*

### Comparing `django_easy_audit-1.3.7a1/easyaudit/migrations/0003_auto_20170228_1505.py` & `django_easy_audit-1.3.7b1/easyaudit/migrations/0003_auto_20170228_1505.py`

 * *Files identical despite different names*

### Comparing `django_easy_audit-1.3.7a1/easyaudit/migrations/0005_auto_20170713_1155.py` & `django_easy_audit-1.3.7b1/easyaudit/migrations/0005_auto_20170713_1155.py`

 * *Files identical despite different names*

### Comparing `django_easy_audit-1.3.7a1/easyaudit/migrations/0006_auto_20171018_1242.py` & `django_easy_audit-1.3.7b1/easyaudit/migrations/0006_auto_20171018_1242.py`

 * *Files identical despite different names*

### Comparing `django_easy_audit-1.3.7a1/easyaudit/migrations/0007_auto_20180105_0838.py` & `django_easy_audit-1.3.7b1/easyaudit/migrations/0007_auto_20180105_0838.py`

 * *Files identical despite different names*

### Comparing `django_easy_audit-1.3.7a1/easyaudit/migrations/0008_auto_20180220_1908.py` & `django_easy_audit-1.3.7b1/easyaudit/migrations/0008_auto_20180220_1908.py`

 * *Files identical despite different names*

### Comparing `django_easy_audit-1.3.7a1/easyaudit/migrations/0009_auto_20180314_2225.py` & `django_easy_audit-1.3.7b1/easyaudit/migrations/0009_auto_20180314_2225.py`

 * *Files identical despite different names*

### Comparing `django_easy_audit-1.3.7a1/easyaudit/migrations/0012_auto_20181018_0012.py` & `django_easy_audit-1.3.7b1/easyaudit/migrations/0012_auto_20181018_0012.py`

 * *Files identical despite different names*

### Comparing `django_easy_audit-1.3.7a1/easyaudit/migrations/0013_auto_20190723_0126.py` & `django_easy_audit-1.3.7b1/easyaudit/migrations/0013_auto_20190723_0126.py`

 * *Files identical despite different names*

### Comparing `django_easy_audit-1.3.7a1/easyaudit/migrations/0015_auto_20201019_1217.py` & `django_easy_audit-1.3.7b1/easyaudit/migrations/0015_auto_20201019_1217.py`

 * *Files identical despite different names*

### Comparing `django_easy_audit-1.3.7a1/easyaudit/migrations/0016_alter_crudevent_event_type.py` & `django_easy_audit-1.3.7b1/easyaudit/migrations/0016_alter_crudevent_event_type.py`

 * *Files identical despite different names*

### Comparing `django_easy_audit-1.3.7a1/easyaudit/migrations/0019_alter_crudevent_changed_fields_and_more.py` & `django_easy_audit-1.3.7b1/easyaudit/migrations/0019_alter_crudevent_changed_fields_and_more.py`

 * *Files identical despite different names*

### Comparing `django_easy_audit-1.3.7a1/easyaudit/models.py` & `django_easy_audit-1.3.7b1/easyaudit/models.py`

 * *Files identical despite different names*

### Comparing `django_easy_audit-1.3.7a1/easyaudit/settings.py` & `django_easy_audit-1.3.7b1/easyaudit/settings.py`

 * *Files identical despite different names*

### Comparing `django_easy_audit-1.3.7a1/easyaudit/signals/auth_signals.py` & `django_easy_audit-1.3.7b1/easyaudit/signals/auth_signals.py`

 * *Files identical despite different names*

### Comparing `django_easy_audit-1.3.7a1/easyaudit/signals/crud_flows.py` & `django_easy_audit-1.3.7b1/easyaudit/signals/crud_flows.py`

 * *Files identical despite different names*

### Comparing `django_easy_audit-1.3.7a1/easyaudit/signals/model_signals.py` & `django_easy_audit-1.3.7b1/easyaudit/signals/model_signals.py`

 * *Files identical despite different names*

### Comparing `django_easy_audit-1.3.7a1/easyaudit/signals/request_signals.py` & `django_easy_audit-1.3.7b1/easyaudit/signals/request_signals.py`

 * *Files identical despite different names*

### Comparing `django_easy_audit-1.3.7a1/easyaudit/templates/admin/easyaudit/change_list.html` & `django_easy_audit-1.3.7b1/easyaudit/templates/admin/easyaudit/change_list.html`

 * *Files identical despite different names*

### Comparing `django_easy_audit-1.3.7a1/easyaudit/templates/admin/easyaudit/purge_confirmation.html` & `django_easy_audit-1.3.7b1/easyaudit/templates/admin/easyaudit/purge_confirmation.html`

 * *Files identical despite different names*

### Comparing `django_easy_audit-1.3.7a1/easyaudit/utils.py` & `django_easy_audit-1.3.7b1/easyaudit/utils.py`

 * *Files identical despite different names*

### Comparing `django_easy_audit-1.3.7a1/pyproject.toml` & `django_easy_audit-1.3.7b1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-easy-audit"
-version = "1.3.7.a1"
+version = "1.3.7-b1"
 description = "Yet another Django audit log app, hopefully the simplest one."
 license = "GPL3"
 authors = ["Natán Calzolari <natancalzolari@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/soynatan/django-easy-audit"
 repository = "https://github.com/soynatan/django-easy-audit"
 documentation = "https://github.com/soynatan/django-easy-audit/wiki"
@@ -40,26 +40,23 @@
 ruff = "^0.1.11"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.4.4"
 pytest-asyncio = "^0.23.3"
 pytest-cov = "^4.1.0"
 pytest-django = "^4.7.0"
-pytest-ruff = "^0.2.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
 addopts = [
     "--ds=tests.settings",         # Forces pytest-django to use test settings
-    "--ruff",
-    "--ruff-format",
     "--ignore-glob='*/models.py'",
 ]
 
 [tool.ruff]
 extend-exclude = ["migrations"]
 ignore = [
     "D1",     # Missing docstrings
```

### Comparing `django_easy_audit-1.3.7a1/PKG-INFO` & `django_easy_audit-1.3.7b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-easy-audit
-Version: 1.3.7a1
+Version: 1.3.7b1
 Summary: Yet another Django audit log app, hopefully the simplest one.
 Home-page: https://github.com/soynatan/django-easy-audit
 License: GPL3
 Author: Natán Calzolari
 Author-email: natancalzolari@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Plugins
```

