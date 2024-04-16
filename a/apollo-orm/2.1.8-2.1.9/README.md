# Comparing `tmp/apollo-orm-2.1.8.tar.gz` & `tmp/apollo_orm-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apollo-orm-2.1.8.tar", last modified: Fri Apr 12 13:27:26 2024, max compression
+gzip compressed data, was "apollo_orm-2.1.9.tar", last modified: Fri Apr 12 16:49:13 2024, max compression
```

## Comparing `apollo-orm-2.1.8.tar` & `apollo_orm-2.1.9.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 13:27:26.098870 apollo-orm-2.1.8/
--rw-rw-rw-   0        0        0     1092 2024-02-28 16:34:21.000000 apollo-orm-2.1.8/LICENSE
--rw-rw-rw-   0        0        0     3273 2024-04-12 13:27:26.098870 apollo-orm-2.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     2608 2024-03-06 22:36:21.000000 apollo-orm-2.1.8/README.md
-drwxrwxrwx   0        0        0        0 2024-04-12 13:27:26.051597 apollo-orm-2.1.8/apollo_orm/
--rw-rw-rw-   0        0        0        0 2024-02-27 18:26:45.000000 apollo-orm-2.1.8/apollo_orm/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 13:27:26.067221 apollo-orm-2.1.8/apollo_orm/domains/
--rw-rw-rw-   0        0        0        0 2024-02-27 18:30:22.000000 apollo-orm-2.1.8/apollo_orm/domains/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 13:27:26.067221 apollo-orm-2.1.8/apollo_orm/domains/models/
--rw-rw-rw-   0        0        0        0 2024-02-26 14:26:38.000000 apollo-orm-2.1.8/apollo_orm/domains/models/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 13:27:26.067221 apollo-orm-2.1.8/apollo_orm/domains/models/entities/
--rw-rw-rw-   0        0        0        0 2024-02-26 14:35:42.000000 apollo-orm-2.1.8/apollo_orm/domains/models/entities/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 13:27:26.067221 apollo-orm-2.1.8/apollo_orm/domains/models/entities/column/
--rw-rw-rw-   0        0        0        0 2024-02-26 18:06:33.000000 apollo-orm-2.1.8/apollo_orm/domains/models/entities/column/__init__.py
--rw-rw-rw-   0        0        0      390 2024-02-26 18:50:38.000000 apollo-orm-2.1.8/apollo_orm/domains/models/entities/column/entity.py
-drwxrwxrwx   0        0        0        0 2024-04-12 13:27:26.067221 apollo-orm-2.1.8/apollo_orm/domains/models/entities/concurrent/
--rw-rw-rw-   0        0        0        0 2024-03-22 22:10:36.000000 apollo-orm-2.1.8/apollo_orm/domains/models/entities/concurrent/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 13:27:26.067221 apollo-orm-2.1.8/apollo_orm/domains/models/entities/concurrent/pre_processed_insert/
--rw-rw-rw-   0        0        0        0 2024-03-24 02:19:02.000000 apollo-orm-2.1.8/apollo_orm/domains/models/entities/concurrent/pre_processed_insert/__init__.py
--rw-rw-rw-   0        0        0      566 2024-03-24 02:46:24.000000 apollo-orm-2.1.8/apollo_orm/domains/models/entities/concurrent/pre_processed_insert/entity.py
-drwxrwxrwx   0        0        0        0 2024-04-12 13:27:26.077229 apollo-orm-2.1.8/apollo_orm/domains/models/entities/concurrent/result_list/
--rw-rw-rw-   0        0        0        0 2024-03-24 02:18:47.000000 apollo-orm-2.1.8/apollo_orm/domains/models/entities/concurrent/result_list/__init__.py
--rw-rw-rw-   0        0        0      300 2024-03-24 02:54:01.000000 apollo-orm-2.1.8/apollo_orm/domains/models/entities/concurrent/result_list/entity.py
-drwxrwxrwx   0        0        0        0 2024-04-12 13:27:26.077229 apollo-orm-2.1.8/apollo_orm/domains/models/entities/concurrent/result_process/
--rw-rw-rw-   0        0        0        0 2024-03-24 02:27:03.000000 apollo-orm-2.1.8/apollo_orm/domains/models/entities/concurrent/result_process/__init__.py
--rw-rw-rw-   0        0        0      401 2024-03-24 03:37:47.000000 apollo-orm-2.1.8/apollo_orm/domains/models/entities/concurrent/result_process/entity.py
-drwxrwxrwx   0        0        0        0 2024-04-12 13:27:26.077229 apollo-orm-2.1.8/apollo_orm/domains/models/entities/connection_config/
--rw-rw-rw-   0        0        0        0 2024-02-26 18:07:14.000000 apollo-orm-2.1.8/apollo_orm/domains/models/entities/connection_config/__init__.py
--rw-rw-rw-   0        0        0      589 2024-03-20 15:01:55.000000 apollo-orm-2.1.8/apollo_orm/domains/models/entities/connection_config/entity.py
-drwxrwxrwx   0        0        0        0 2024-04-12 13:27:26.083236 apollo-orm-2.1.8/apollo_orm/domains/models/entities/credentials/
--rw-rw-rw-   0        0        0        0 2024-02-26 18:07:23.000000 apollo-orm-2.1.8/apollo_orm/domains/models/entities/credentials/__init__.py
--rw-rw-rw-   0        0        0      688 2024-03-20 15:01:55.000000 apollo-orm-2.1.8/apollo_orm/domains/models/entities/credentials/entity.py
-drwxrwxrwx   0        0        0        0 2024-04-12 13:27:26.083236 apollo-orm-2.1.8/apollo_orm/domains/models/entities/table_config/
--rw-rw-rw-   0        0        0        0 2024-02-26 18:07:52.000000 apollo-orm-2.1.8/apollo_orm/domains/models/entities/table_config/__init__.py
--rw-rw-rw-   0        0        0      319 2024-02-28 18:35:47.000000 apollo-orm-2.1.8/apollo_orm/domains/models/entities/table_config/entity.py
-drwxrwxrwx   0        0        0        0 2024-04-12 13:27:26.083236 apollo-orm-2.1.8/apollo_orm/orm/
--rw-rw-rw-   0        0        0        0 2024-02-27 18:28:09.000000 apollo-orm-2.1.8/apollo_orm/orm/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 13:27:26.083236 apollo-orm-2.1.8/apollo_orm/orm/abstracts/
--rw-rw-rw-   0        0        0        0 2024-02-27 18:29:25.000000 apollo-orm-2.1.8/apollo_orm/orm/abstracts/__init__.py
--rw-rw-rw-   0        0        0      477 2024-02-28 18:35:47.000000 apollo-orm-2.1.8/apollo_orm/orm/abstracts/icredential.py
--rw-rw-rw-   0        0        0     2372 2024-03-02 19:23:03.000000 apollo-orm-2.1.8/apollo_orm/orm/abstracts/idatabase.py
--rw-rw-rw-   0        0        0    22982 2024-04-12 13:24:16.000000 apollo-orm-2.1.8/apollo_orm/orm/core.py
-drwxrwxrwx   0        0        0        0 2024-04-12 13:27:26.083236 apollo-orm-2.1.8/apollo_orm/orm/credentials/
--rw-rw-rw-   0        0        0        0 2024-02-23 15:44:41.000000 apollo-orm-2.1.8/apollo_orm/orm/credentials/__init__.py
--rw-rw-rw-   0        0        0      822 2024-03-04 13:10:50.000000 apollo-orm-2.1.8/apollo_orm/orm/credentials/credential_service.py
--rw-rw-rw-   0        0        0      629 2024-02-28 18:38:15.000000 apollo-orm-2.1.8/apollo_orm/orm/credentials/json_credential_service.py
--rw-rw-rw-   0        0        0      994 2024-02-28 20:04:09.000000 apollo-orm-2.1.8/apollo_orm/orm/credentials/secrets_manager_credential_service.py
-drwxrwxrwx   0        0        0        0 2024-04-12 13:27:26.083236 apollo-orm-2.1.8/apollo_orm/utils/
--rw-rw-rw-   0        0        0        0 2024-02-23 16:01:29.000000 apollo-orm-2.1.8/apollo_orm/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 13:27:26.083236 apollo-orm-2.1.8/apollo_orm/utils/exceptions/
--rw-rw-rw-   0        0        0     1028 2024-02-28 18:38:15.000000 apollo-orm-2.1.8/apollo_orm/utils/exceptions/CommonBaseException.py
--rw-rw-rw-   0        0        0        0 2024-02-23 16:01:47.000000 apollo-orm-2.1.8/apollo_orm/utils/exceptions/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 13:27:26.098870 apollo-orm-2.1.8/apollo_orm/utils/logger/
--rw-rw-rw-   0        0        0        0 2024-02-23 16:02:34.000000 apollo-orm-2.1.8/apollo_orm/utils/logger/__init__.py
--rw-rw-rw-   0        0        0     2037 2024-03-07 13:30:15.000000 apollo-orm-2.1.8/apollo_orm/utils/logger/logger.py
-drwxrwxrwx   0        0        0        0 2024-04-12 13:27:26.098870 apollo-orm-2.1.8/apollo_orm.egg-info/
--rw-rw-rw-   0        0        0     3273 2024-04-12 13:27:26.000000 apollo-orm-2.1.8/apollo_orm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1860 2024-04-12 13:27:26.000000 apollo-orm-2.1.8/apollo_orm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 13:27:26.000000 apollo-orm-2.1.8/apollo_orm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-04-12 13:27:26.000000 apollo-orm-2.1.8/apollo_orm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      731 2024-04-12 13:26:47.000000 apollo-orm-2.1.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-12 13:27:26.098870 apollo-orm-2.1.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-12 13:27:26.098870 apollo-orm-2.1.8/tests/
--rw-rw-rw-   0        0        0    13794 2024-04-03 21:42:11.000000 apollo-orm-2.1.8/tests/test_full_process.py
+drwxrwxrwx   0        0        0        0 2024-04-12 16:49:13.638353 apollo_orm-2.1.9/
+-rw-rw-rw-   0        0        0     1092 2024-02-28 16:34:21.000000 apollo_orm-2.1.9/LICENSE
+-rw-rw-rw-   0        0        0     3273 2024-04-12 16:49:13.637355 apollo_orm-2.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2608 2024-03-06 22:36:21.000000 apollo_orm-2.1.9/README.md
+drwxrwxrwx   0        0        0        0 2024-04-12 16:49:13.542818 apollo_orm-2.1.9/apollo_orm/
+-rw-rw-rw-   0        0        0        0 2024-02-27 18:26:45.000000 apollo_orm-2.1.9/apollo_orm/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 16:49:13.584836 apollo_orm-2.1.9/apollo_orm/domains/
+-rw-rw-rw-   0        0        0        0 2024-02-27 18:30:22.000000 apollo_orm-2.1.9/apollo_orm/domains/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 16:49:13.586836 apollo_orm-2.1.9/apollo_orm/domains/models/
+-rw-rw-rw-   0        0        0        0 2024-02-26 14:26:38.000000 apollo_orm-2.1.9/apollo_orm/domains/models/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 16:49:13.588832 apollo_orm-2.1.9/apollo_orm/domains/models/entities/
+-rw-rw-rw-   0        0        0        0 2024-02-26 14:35:42.000000 apollo_orm-2.1.9/apollo_orm/domains/models/entities/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 16:49:13.593359 apollo_orm-2.1.9/apollo_orm/domains/models/entities/column/
+-rw-rw-rw-   0        0        0        0 2024-02-26 18:06:33.000000 apollo_orm-2.1.9/apollo_orm/domains/models/entities/column/__init__.py
+-rw-rw-rw-   0        0        0      390 2024-02-26 18:50:38.000000 apollo_orm-2.1.9/apollo_orm/domains/models/entities/column/entity.py
+drwxrwxrwx   0        0        0        0 2024-04-12 16:49:13.595357 apollo_orm-2.1.9/apollo_orm/domains/models/entities/concurrent/
+-rw-rw-rw-   0        0        0        0 2024-03-22 22:10:36.000000 apollo_orm-2.1.9/apollo_orm/domains/models/entities/concurrent/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 16:49:13.597355 apollo_orm-2.1.9/apollo_orm/domains/models/entities/concurrent/pre_processed_insert/
+-rw-rw-rw-   0        0        0        0 2024-03-24 02:19:02.000000 apollo_orm-2.1.9/apollo_orm/domains/models/entities/concurrent/pre_processed_insert/__init__.py
+-rw-rw-rw-   0        0        0      566 2024-03-24 02:46:24.000000 apollo_orm-2.1.9/apollo_orm/domains/models/entities/concurrent/pre_processed_insert/entity.py
+drwxrwxrwx   0        0        0        0 2024-04-12 16:49:13.602358 apollo_orm-2.1.9/apollo_orm/domains/models/entities/concurrent/result_list/
+-rw-rw-rw-   0        0        0        0 2024-03-24 02:18:47.000000 apollo_orm-2.1.9/apollo_orm/domains/models/entities/concurrent/result_list/__init__.py
+-rw-rw-rw-   0        0        0      300 2024-03-24 02:54:01.000000 apollo_orm-2.1.9/apollo_orm/domains/models/entities/concurrent/result_list/entity.py
+drwxrwxrwx   0        0        0        0 2024-04-12 16:49:13.605353 apollo_orm-2.1.9/apollo_orm/domains/models/entities/concurrent/result_process/
+-rw-rw-rw-   0        0        0        0 2024-03-24 02:27:03.000000 apollo_orm-2.1.9/apollo_orm/domains/models/entities/concurrent/result_process/__init__.py
+-rw-rw-rw-   0        0        0      401 2024-03-24 03:37:47.000000 apollo_orm-2.1.9/apollo_orm/domains/models/entities/concurrent/result_process/entity.py
+drwxrwxrwx   0        0        0        0 2024-04-12 16:49:13.611356 apollo_orm-2.1.9/apollo_orm/domains/models/entities/connection_config/
+-rw-rw-rw-   0        0        0        0 2024-02-26 18:07:14.000000 apollo_orm-2.1.9/apollo_orm/domains/models/entities/connection_config/__init__.py
+-rw-rw-rw-   0        0        0      589 2024-03-20 15:01:55.000000 apollo_orm-2.1.9/apollo_orm/domains/models/entities/connection_config/entity.py
+drwxrwxrwx   0        0        0        0 2024-04-12 16:49:13.613355 apollo_orm-2.1.9/apollo_orm/domains/models/entities/credentials/
+-rw-rw-rw-   0        0        0        0 2024-02-26 18:07:23.000000 apollo_orm-2.1.9/apollo_orm/domains/models/entities/credentials/__init__.py
+-rw-rw-rw-   0        0        0      688 2024-03-20 15:01:55.000000 apollo_orm-2.1.9/apollo_orm/domains/models/entities/credentials/entity.py
+drwxrwxrwx   0        0        0        0 2024-04-12 16:49:13.615356 apollo_orm-2.1.9/apollo_orm/domains/models/entities/table_config/
+-rw-rw-rw-   0        0        0        0 2024-02-26 18:07:52.000000 apollo_orm-2.1.9/apollo_orm/domains/models/entities/table_config/__init__.py
+-rw-rw-rw-   0        0        0      319 2024-02-28 18:35:47.000000 apollo_orm-2.1.9/apollo_orm/domains/models/entities/table_config/entity.py
+drwxrwxrwx   0        0        0        0 2024-04-12 16:49:13.617357 apollo_orm-2.1.9/apollo_orm/orm/
+-rw-rw-rw-   0        0        0        0 2024-02-27 18:28:09.000000 apollo_orm-2.1.9/apollo_orm/orm/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 16:49:13.621358 apollo_orm-2.1.9/apollo_orm/orm/abstracts/
+-rw-rw-rw-   0        0        0        0 2024-02-27 18:29:25.000000 apollo_orm-2.1.9/apollo_orm/orm/abstracts/__init__.py
+-rw-rw-rw-   0        0        0      477 2024-02-28 18:35:47.000000 apollo_orm-2.1.9/apollo_orm/orm/abstracts/icredential.py
+-rw-rw-rw-   0        0        0     2372 2024-03-02 19:23:03.000000 apollo_orm-2.1.9/apollo_orm/orm/abstracts/idatabase.py
+-rw-rw-rw-   0        0        0    22995 2024-04-12 16:48:38.000000 apollo_orm-2.1.9/apollo_orm/orm/core.py
+drwxrwxrwx   0        0        0        0 2024-04-12 16:49:13.629357 apollo_orm-2.1.9/apollo_orm/orm/credentials/
+-rw-rw-rw-   0        0        0        0 2024-02-23 15:44:41.000000 apollo_orm-2.1.9/apollo_orm/orm/credentials/__init__.py
+-rw-rw-rw-   0        0        0      822 2024-03-04 13:10:50.000000 apollo_orm-2.1.9/apollo_orm/orm/credentials/credential_service.py
+-rw-rw-rw-   0        0        0      629 2024-02-28 18:38:15.000000 apollo_orm-2.1.9/apollo_orm/orm/credentials/json_credential_service.py
+-rw-rw-rw-   0        0        0      994 2024-02-28 20:04:09.000000 apollo_orm-2.1.9/apollo_orm/orm/credentials/secrets_manager_credential_service.py
+drwxrwxrwx   0        0        0        0 2024-04-12 16:49:13.630357 apollo_orm-2.1.9/apollo_orm/utils/
+-rw-rw-rw-   0        0        0        0 2024-02-23 16:01:29.000000 apollo_orm-2.1.9/apollo_orm/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 16:49:13.633355 apollo_orm-2.1.9/apollo_orm/utils/exceptions/
+-rw-rw-rw-   0        0        0     1028 2024-02-28 18:38:15.000000 apollo_orm-2.1.9/apollo_orm/utils/exceptions/CommonBaseException.py
+-rw-rw-rw-   0        0        0        0 2024-02-23 16:01:47.000000 apollo_orm-2.1.9/apollo_orm/utils/exceptions/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 16:49:13.634355 apollo_orm-2.1.9/apollo_orm/utils/logger/
+-rw-rw-rw-   0        0        0        0 2024-02-23 16:02:34.000000 apollo_orm-2.1.9/apollo_orm/utils/logger/__init__.py
+-rw-rw-rw-   0        0        0     2037 2024-03-07 13:30:15.000000 apollo_orm-2.1.9/apollo_orm/utils/logger/logger.py
+drwxrwxrwx   0        0        0        0 2024-04-12 16:49:13.636355 apollo_orm-2.1.9/apollo_orm.egg-info/
+-rw-rw-rw-   0        0        0     3273 2024-04-12 16:49:13.000000 apollo_orm-2.1.9/apollo_orm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1860 2024-04-12 16:49:13.000000 apollo_orm-2.1.9/apollo_orm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 16:49:13.000000 apollo_orm-2.1.9/apollo_orm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-04-12 16:49:13.000000 apollo_orm-2.1.9/apollo_orm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      731 2024-04-12 16:48:38.000000 apollo_orm-2.1.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-12 16:49:13.639353 apollo_orm-2.1.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-12 16:49:13.635355 apollo_orm-2.1.9/tests/
+-rw-rw-rw-   0        0        0    13794 2024-04-03 21:42:11.000000 apollo_orm-2.1.9/tests/test_full_process.py
```

### Comparing `apollo-orm-2.1.8/LICENSE` & `apollo_orm-2.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `apollo-orm-2.1.8/PKG-INFO` & `apollo_orm-2.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apollo-orm
-Version: 2.1.8
+Version: 2.1.9
 Summary: ORM Cassandra/Scylla Stable Version (2.x.x)
 Author-email: Danilo Rodrigues <daniloarodrigues@outlook.com>
 Project-URL: Homepage, https://github.com/daniloarodrigues/apollo-orm
 Project-URL: Issues, https://github.com/daniloarodrigues/apollo-orm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `apollo-orm-2.1.8/README.md` & `apollo_orm-2.1.9/README.md`

 * *Files identical despite different names*

### Comparing `apollo-orm-2.1.8/apollo_orm/domains/models/entities/concurrent/pre_processed_insert/entity.py` & `apollo_orm-2.1.9/apollo_orm/domains/models/entities/concurrent/pre_processed_insert/entity.py`

 * *Files identical despite different names*

### Comparing `apollo-orm-2.1.8/apollo_orm/domains/models/entities/connection_config/entity.py` & `apollo_orm-2.1.9/apollo_orm/domains/models/entities/connection_config/entity.py`

 * *Files identical despite different names*

### Comparing `apollo-orm-2.1.8/apollo_orm/domains/models/entities/credentials/entity.py` & `apollo_orm-2.1.9/apollo_orm/domains/models/entities/credentials/entity.py`

 * *Files identical despite different names*

### Comparing `apollo-orm-2.1.8/apollo_orm/orm/abstracts/idatabase.py` & `apollo_orm-2.1.9/apollo_orm/orm/abstracts/idatabase.py`

 * *Files identical despite different names*

### Comparing `apollo-orm-2.1.8/apollo_orm/orm/core.py` & `apollo_orm-2.1.9/apollo_orm/orm/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -388,15 +388,15 @@
             self.reconnect()
             return self.session.execute(statement, values)
 
     def _prepare_dynamic_statement(self, columns: Dict[str, Column], table_name: str,
                                    query_type: str) -> PreparedStatement:
         keyspace = self._connection_config.credential.keyspace_name
         ordered_columns = sorted(columns.values(), key=lambda x: x.name)
-        hashed_name = _text_to_hash(f"{query_type}".join([column.name for column in ordered_columns]))
+        hashed_name = _text_to_hash(f"{query_type}-{table_name}".join([column.name for column in ordered_columns]))
         if hashed_name not in self._prepared_statements:
             try:
                 if query_type == "select":
                     self._prepare_read(hashed_name, ordered_columns, keyspace, table_name)
                 elif query_type == "insert":
                     self._prepare_insert(hashed_name, ordered_columns, keyspace, table_name, columns)
                 elif query_type == "delete":
```

### Comparing `apollo-orm-2.1.8/apollo_orm/orm/credentials/credential_service.py` & `apollo_orm-2.1.9/apollo_orm/orm/credentials/credential_service.py`

 * *Files identical despite different names*

### Comparing `apollo-orm-2.1.8/apollo_orm/orm/credentials/json_credential_service.py` & `apollo_orm-2.1.9/apollo_orm/orm/credentials/json_credential_service.py`

 * *Files identical despite different names*

### Comparing `apollo-orm-2.1.8/apollo_orm/orm/credentials/secrets_manager_credential_service.py` & `apollo_orm-2.1.9/apollo_orm/orm/credentials/secrets_manager_credential_service.py`

 * *Files identical despite different names*

### Comparing `apollo-orm-2.1.8/apollo_orm/utils/exceptions/CommonBaseException.py` & `apollo_orm-2.1.9/apollo_orm/utils/exceptions/CommonBaseException.py`

 * *Files identical despite different names*

### Comparing `apollo-orm-2.1.8/apollo_orm/utils/logger/logger.py` & `apollo_orm-2.1.9/apollo_orm/utils/logger/logger.py`

 * *Files identical despite different names*

### Comparing `apollo-orm-2.1.8/apollo_orm.egg-info/PKG-INFO` & `apollo_orm-2.1.9/apollo_orm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apollo-orm
-Version: 2.1.8
+Version: 2.1.9
 Summary: ORM Cassandra/Scylla Stable Version (2.x.x)
 Author-email: Danilo Rodrigues <daniloarodrigues@outlook.com>
 Project-URL: Homepage, https://github.com/daniloarodrigues/apollo-orm
 Project-URL: Issues, https://github.com/daniloarodrigues/apollo-orm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `apollo-orm-2.1.8/apollo_orm.egg-info/SOURCES.txt` & `apollo_orm-2.1.9/apollo_orm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apollo-orm-2.1.8/pyproject.toml` & `apollo_orm-2.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "apollo-orm"
-version = "2.1.8"
+version = "2.1.9"
 authors = [
     { name="Danilo Rodrigues", email="daniloarodrigues@outlook.com" },
 ]
 description = "ORM Cassandra/Scylla Stable Version (2.x.x)"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `apollo-orm-2.1.8/tests/test_full_process.py` & `apollo_orm-2.1.9/tests/test_full_process.py`

 * *Files identical despite different names*

