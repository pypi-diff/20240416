# Comparing `tmp/project-utils-django-0.3.19.tar.gz` & `tmp/project-utils-django-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "project-utils-django-0.3.19.tar", last modified: Tue Apr 16 10:22:51 2024, max compression
+gzip compressed data, was "project-utils-django-1.0.1.tar", last modified: Tue Apr 16 10:29:45 2024, max compression
```

## Comparing `project-utils-django-0.3.19.tar` & `project-utils-django-1.0.1.tar`

### file list

```diff
@@ -1,147 +1,147 @@
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-16 10:22:51.685680 project-utils-django-0.3.19/
--rw-r--r--   0 mylx2014   (501) staff       (20)        0 2023-10-13 07:03:44.000000 project-utils-django-0.3.19/LICENSE
--rw-r--r--   0 mylx2014   (501) staff       (20)     1674 2024-04-16 10:22:51.684412 project-utils-django-0.3.19/PKG-INFO
--rw-r--r--   0 mylx2014   (501) staff       (20)     1289 2023-11-24 01:16:34.000000 project-utils-django-0.3.19/README.md
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-16 10:22:51.671299 project-utils-django-0.3.19/project_utils/
--rw-r--r--   0 mylx2014   (501) staff       (20)        0 2023-10-13 02:35:45.000000 project-utils-django-0.3.19/project_utils/__init__.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-16 10:22:51.671512 project-utils-django-0.3.19/project_utils/collection/
--rw-r--r--   0 mylx2014   (501) staff       (20)      140 2023-10-14 01:51:03.000000 project-utils-django-0.3.19/project_utils/collection/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      596 2023-10-13 02:35:45.000000 project-utils-django-0.3.19/project_utils/collection/list_util.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-16 10:22:51.671816 project-utils-django-0.3.19/project_utils/config/
--rw-r--r--   0 mylx2014   (501) staff       (20)      155 2023-10-14 01:51:03.000000 project-utils-django-0.3.19/project_utils/config/__init__.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-16 10:22:51.672421 project-utils-django-0.3.19/project_utils/config/addr_config/
--rw-r--r--   0 mylx2014   (501) staff       (20)      652 2023-10-14 01:51:03.000000 project-utils-django-0.3.19/project_utils/config/addr_config/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      739 2023-11-24 01:16:34.000000 project-utils-django-0.3.19/project_utils/config/addr_config/base_config.py
--rw-r--r--   0 mylx2014   (501) staff       (20)       86 2023-10-14 01:51:03.000000 project-utils-django-0.3.19/project_utils/config/addr_config/hbase_config.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      777 2023-10-14 01:51:03.000000 project-utils-django-0.3.19/project_utils/config/addr_config/kafka_config.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      695 2023-10-14 01:51:03.000000 project-utils-django-0.3.19/project_utils/config/addr_config/mysql_config.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      825 2023-11-24 01:16:34.000000 project-utils-django-0.3.19/project_utils/config/addr_config/redis_config.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     1039 2023-10-14 01:51:03.000000 project-utils-django-0.3.19/project_utils/config/base_config.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-16 10:22:51.672623 project-utils-django-0.3.19/project_utils/config/path_config/
--rw-r--r--   0 mylx2014   (501) staff       (20)      130 2023-10-14 01:51:03.000000 project-utils-django-0.3.19/project_utils/config/path_config/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      970 2023-10-13 02:35:45.000000 project-utils-django-0.3.19/project_utils/config/path_config/path_config.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     1977 2023-10-14 01:51:03.000000 project-utils-django-0.3.19/project_utils/config/template.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-16 10:22:51.672721 project-utils-django-0.3.19/project_utils/db/
--rw-r--r--   0 mylx2014   (501) staff       (20)      164 2023-10-14 01:57:29.000000 project-utils-django-0.3.19/project_utils/db/__init__.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-16 10:22:51.673278 project-utils-django-0.3.19/project_utils/db/mysql/
--rw-r--r--   0 mylx2014   (501) staff       (20)      257 2023-10-14 01:57:29.000000 project-utils-django-0.3.19/project_utils/db/mysql/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     3484 2023-11-28 08:48:43.000000 project-utils-django-0.3.19/project_utils/db/mysql/_collection.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     2291 2023-12-15 01:39:50.000000 project-utils-django-0.3.19/project_utils/db/mysql/_pool.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      832 2023-11-24 01:16:34.000000 project-utils-django-0.3.19/project_utils/db/mysql/_result.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      107 2023-10-13 02:35:45.000000 project-utils-django-0.3.19/project_utils/db/mysql/_types.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-16 10:22:51.674036 project-utils-django-0.3.19/project_utils/exception/
--rw-r--r--   0 mylx2014   (501) staff       (20)      811 2023-10-14 02:37:02.000000 project-utils-django-0.3.19/project_utils/exception/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      148 2023-10-14 02:37:02.000000 project-utils-django-0.3.19/project_utils/exception/collection_exception.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      144 2023-10-14 02:37:02.000000 project-utils-django-0.3.19/project_utils/exception/config_exception.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-16 10:22:51.674354 project-utils-django-0.3.19/project_utils/exception/db_exception/
--rw-r--r--   0 mylx2014   (501) staff       (20)      141 2023-10-14 02:37:02.000000 project-utils-django-0.3.19/project_utils/exception/db_exception/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      118 2023-10-14 02:37:02.000000 project-utils-django-0.3.19/project_utils/exception/db_exception/mysql_exception.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      507 2023-10-13 02:35:45.000000 project-utils-django-0.3.19/project_utils/exception/my_base_exception.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-16 10:22:51.674483 project-utils-django-0.3.19/project_utils/exception/web_exception/
--rw-r--r--   0 mylx2014   (501) staff       (20)      142 2023-10-14 02:37:02.000000 project-utils-django-0.3.19/project_utils/exception/web_exception/__init__.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-16 10:22:51.674694 project-utils-django-0.3.19/project_utils/exception/web_exception/django_exception/
--rw-r--r--   0 mylx2014   (501) staff       (20)      125 2023-10-14 02:37:02.000000 project-utils-django-0.3.19/project_utils/exception/web_exception/django_exception/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      127 2023-10-14 02:37:02.000000 project-utils-django-0.3.19/project_utils/exception/web_exception/django_exception/model_exception.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-16 10:22:51.674920 project-utils-django-0.3.19/project_utils/exception/web_exception/django_exception/view_exception/
--rw-r--r--   0 mylx2014   (501) staff       (20)      275 2023-10-18 02:20:38.000000 project-utils-django-0.3.19/project_utils/exception/web_exception/django_exception/view_exception/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      120 2023-10-14 02:37:02.000000 project-utils-django-0.3.19/project_utils/exception/web_exception/django_exception/view_exception/response_exception.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     1255 2023-10-13 02:35:45.000000 project-utils-django-0.3.19/project_utils/io.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-16 10:22:51.675140 project-utils-django-0.3.19/project_utils/os/
--rw-r--r--   0 mylx2014   (501) staff       (20)       98 2023-10-14 02:37:02.000000 project-utils-django-0.3.19/project_utils/os/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      760 2023-10-13 02:35:45.000000 project-utils-django-0.3.19/project_utils/os/dir.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     2029 2024-01-16 07:43:03.000000 project-utils-django-0.3.19/project_utils/time.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-16 10:22:51.675237 project-utils-django-0.3.19/project_utils/web/
--rw-r--r--   0 mylx2014   (501) staff       (20)        0 2023-10-13 02:35:45.000000 project-utils-django-0.3.19/project_utils/web/__init__.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-16 10:22:51.675320 project-utils-django-0.3.19/project_utils/web/aiohttp/
--rw-r--r--   0 mylx2014   (501) staff       (20)        0 2023-10-13 02:35:45.000000 project-utils-django-0.3.19/project_utils/web/aiohttp/__init__.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-16 10:22:51.675502 project-utils-django-0.3.19/project_utils/web/django/
--rw-r--r--   0 mylx2014   (501) staff       (20)      463 2023-10-14 02:37:02.000000 project-utils-django-0.3.19/project_utils/web/django/__init__.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-16 10:22:51.675691 project-utils-django-0.3.19/project_utils/web/django/celery/
--rw-r--r--   0 mylx2014   (501) staff       (20)       84 2023-10-14 02:37:02.000000 project-utils-django-0.3.19/project_utils/web/django/celery/__init__.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-16 10:22:51.675911 project-utils-django-0.3.19/project_utils/web/django/celery/_conf/
--rw-r--r--   0 mylx2014   (501) staff       (20)      142 2023-10-14 02:37:02.000000 project-utils-django-0.3.19/project_utils/web/django/celery/_conf/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     1061 2023-11-24 01:16:34.000000 project-utils-django-0.3.19/project_utils/web/django/celery/_conf/_celery_config.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      334 2023-10-18 01:14:46.000000 project-utils-django-0.3.19/project_utils/web/django/celery/create_app.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-16 10:22:51.676108 project-utils-django-0.3.19/project_utils/web/django/conf/
--rw-r--r--   0 mylx2014   (501) staff       (20)      155 2023-10-14 02:37:02.000000 project-utils-django-0.3.19/project_utils/web/django/conf/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     2145 2023-11-24 01:16:34.000000 project-utils-django-0.3.19/project_utils/web/django/conf/_django_config.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-16 10:22:51.676305 project-utils-django-0.3.19/project_utils/web/django/middle/
--rw-r--r--   0 mylx2014   (501) staff       (20)      124 2023-10-14 02:37:02.000000 project-utils-django-0.3.19/project_utils/web/django/middle/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     1161 2023-11-24 01:16:34.000000 project-utils-django-0.3.19/project_utils/web/django/middle/_base_middle.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-16 10:22:51.676816 project-utils-django-0.3.19/project_utils/web/django/model/
--rw-r--r--   0 mylx2014   (501) staff       (20)      434 2024-01-15 14:04:29.000000 project-utils-django-0.3.19/project_utils/web/django/model/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      106 2023-12-10 05:49:34.000000 project-utils-django-0.3.19/project_utils/web/django/model/_base_meta.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     1511 2024-01-15 14:04:29.000000 project-utils-django-0.3.19/project_utils/web/django/model/_base_model.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      487 2023-12-08 06:57:16.000000 project-utils-django-0.3.19/project_utils/web/django/model/_id_model.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      461 2024-01-15 14:04:29.000000 project-utils-django-0.3.19/project_utils/web/django/model/_model_type.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-16 10:22:51.677017 project-utils-django-0.3.19/project_utils/web/django/pagination/
--rw-r--r--   0 mylx2014   (501) staff       (20)      197 2023-10-14 02:37:02.000000 project-utils-django-0.3.19/project_utils/web/django/pagination/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     1011 2023-11-24 01:16:34.000000 project-utils-django-0.3.19/project_utils/web/django/pagination/_base_pagination.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-16 10:22:51.677235 project-utils-django-0.3.19/project_utils/web/django/request/
--rw-r--r--   0 mylx2014   (501) staff       (20)      102 2023-10-14 02:37:02.000000 project-utils-django-0.3.19/project_utils/web/django/request/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     1379 2023-11-24 01:16:34.000000 project-utils-django-0.3.19/project_utils/web/django/request/_request.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-16 10:22:51.677540 project-utils-django-0.3.19/project_utils/web/django/response/
--rw-r--r--   0 mylx2014   (501) staff       (20)      153 2023-10-14 02:37:02.000000 project-utils-django-0.3.19/project_utils/web/django/response/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     1291 2023-10-14 02:37:02.000000 project-utils-django-0.3.19/project_utils/web/django/response/_response_model.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      213 2023-11-24 01:16:34.000000 project-utils-django-0.3.19/project_utils/web/django/response/_response_types.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-16 10:22:51.677856 project-utils-django-0.3.19/project_utils/web/django/serializer/
--rw-r--r--   0 mylx2014   (501) staff       (20)      130 2023-10-14 02:37:02.000000 project-utils-django-0.3.19/project_utils/web/django/serializer/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      284 2023-10-13 02:35:45.000000 project-utils-django-0.3.19/project_utils/web/django/serializer/_base_meta.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      418 2023-10-14 02:37:02.000000 project-utils-django-0.3.19/project_utils/web/django/serializer/_base_serializer.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-16 10:22:51.678050 project-utils-django-0.3.19/project_utils/web/django/swagger/
--rw-r--r--   0 mylx2014   (501) staff       (20)      499 2023-12-10 07:02:32.000000 project-utils-django-0.3.19/project_utils/web/django/swagger/__init__.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-16 10:22:51.678770 project-utils-django-0.3.19/project_utils/web/django/swagger/_params/
--rw-r--r--   0 mylx2014   (501) staff       (20)      675 2023-12-10 07:02:32.000000 project-utils-django-0.3.19/project_utils/web/django/swagger/_params/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      307 2023-12-10 07:02:32.000000 project-utils-django-0.3.19/project_utils/web/django/swagger/_params/_base.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     1025 2023-12-10 07:02:32.000000 project-utils-django-0.3.19/project_utils/web/django/swagger/_params/_form.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     1164 2023-12-10 07:02:32.000000 project-utils-django-0.3.19/project_utils/web/django/swagger/_params/_params.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      978 2023-12-10 07:02:32.000000 project-utils-django-0.3.19/project_utils/web/django/swagger/_params/_query.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     2065 2023-12-10 07:17:18.000000 project-utils-django-0.3.19/project_utils/web/django/swagger/_params/_response.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      412 2023-12-10 07:02:32.000000 project-utils-django-0.3.19/project_utils/web/django/swagger/_params/_types.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      268 2023-12-10 07:15:26.000000 project-utils-django-0.3.19/project_utils/web/django/swagger/_urls.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-16 10:22:51.679299 project-utils-django-0.3.19/project_utils/web/django/swagger/config/
--rw-r--r--   0 mylx2014   (501) staff       (20)       69 2023-12-10 07:02:32.000000 project-utils-django-0.3.19/project_utils/web/django/swagger/config/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      488 2023-12-10 07:15:01.000000 project-utils-django-0.3.19/project_utils/web/django/swagger/config/_config.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     1274 2023-12-10 07:15:01.000000 project-utils-django-0.3.19/project_utils/web/django/swagger/config/_swagger.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-16 10:22:51.679919 project-utils-django-0.3.19/project_utils/web/django/swagger/document/
--rw-r--r--   0 mylx2014   (501) staff       (20)      256 2023-12-10 07:02:32.000000 project-utils-django-0.3.19/project_utils/web/django/swagger/document/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     1169 2023-12-10 07:15:01.000000 project-utils-django-0.3.19/project_utils/web/django/swagger/document/_document.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      273 2023-12-10 07:02:32.000000 project-utils-django-0.3.19/project_utils/web/django/swagger/document/_types.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      678 2023-11-24 01:16:34.000000 project-utils-django-0.3.19/project_utils/web/django/utils.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-16 10:22:51.680632 project-utils-django-0.3.19/project_utils/web/django/view/
--rw-r--r--   0 mylx2014   (501) staff       (20)      478 2023-12-10 07:02:32.000000 project-utils-django-0.3.19/project_utils/web/django/view/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     3840 2023-12-10 07:02:32.000000 project-utils-django-0.3.19/project_utils/web/django/view/_async_view.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     2086 2023-12-10 15:11:23.000000 project-utils-django-0.3.19/project_utils/web/django/view/_base.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-16 10:22:51.681085 project-utils-django-0.3.19/project_utils/web/django/view/_base_api/
--rw-r--r--   0 mylx2014   (501) staff       (20)       57 2023-12-10 07:02:32.000000 project-utils-django-0.3.19/project_utils/web/django/view/_base_api/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     3277 2023-12-10 15:07:50.000000 project-utils-django-0.3.19/project_utils/web/django/view/_base_api/api.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      908 2023-12-10 15:07:50.000000 project-utils-django-0.3.19/project_utils/web/django/view/_base_api/api_util.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-16 10:22:51.681613 project-utils-django-0.3.19/project_utils/web/django/view/_rest_api/
--rw-r--r--   0 mylx2014   (501) staff       (20)      296 2023-12-10 07:02:32.000000 project-utils-django-0.3.19/project_utils/web/django/view/_rest_api/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     1921 2023-12-10 15:07:50.000000 project-utils-django-0.3.19/project_utils/web/django/view/_rest_api/api.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      480 2023-12-10 15:08:55.000000 project-utils-django-0.3.19/project_utils/web/django/view/_rest_api/api_utils.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     2020 2023-12-10 15:08:55.000000 project-utils-django-0.3.19/project_utils/web/django/view/_rest_api/async_api.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-16 10:22:51.682235 project-utils-django-0.3.19/project_utils/web/django/view/_rest_view/
--rw-r--r--   0 mylx2014   (501) staff       (20)      307 2023-12-10 07:02:32.000000 project-utils-django-0.3.19/project_utils/web/django/view/_rest_view/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)    12607 2023-12-10 15:16:37.000000 project-utils-django-0.3.19/project_utils/web/django/view/_rest_view/_async_base_view.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     3840 2023-12-10 15:11:23.000000 project-utils-django-0.3.19/project_utils/web/django/view/_rest_view/_async_view.py
--rw-r--r--   0 mylx2014   (501) staff       (20)    12432 2023-12-10 15:11:23.000000 project-utils-django-0.3.19/project_utils/web/django/view/_rest_view/_base_view.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     1243 2023-12-10 15:11:23.000000 project-utils-django-0.3.19/project_utils/web/django/view/_rest_view/_swagger_base.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     1243 2023-12-10 07:27:29.000000 project-utils-django-0.3.19/project_utils/web/django/view/_swagger_base.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      750 2023-12-10 07:02:32.000000 project-utils-django-0.3.19/project_utils/web/django/view/_types.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-16 10:22:51.682613 project-utils-django-0.3.19/project_utils/web/django/view/_user_view/
--rw-r--r--   0 mylx2014   (501) staff       (20)      185 2023-12-10 07:02:32.000000 project-utils-django-0.3.19/project_utils/web/django/view/_user_view/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      239 2023-12-10 15:11:23.000000 project-utils-django-0.3.19/project_utils/web/django/view/_user_view/_model.py
--rw-r--r--   0 mylx2014   (501) staff       (20)    11333 2023-12-10 15:11:23.000000 project-utils-django-0.3.19/project_utils/web/django/view/_user_view/_view.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-16 10:22:51.682764 project-utils-django-0.3.19/project_utils/web/fastapi/
--rw-r--r--   0 mylx2014   (501) staff       (20)        0 2023-10-13 02:35:45.000000 project-utils-django-0.3.19/project_utils/web/fastapi/__init__.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-16 10:22:51.682874 project-utils-django-0.3.19/project_utils/web/flask/
--rw-r--r--   0 mylx2014   (501) staff       (20)        0 2023-10-13 02:35:45.000000 project-utils-django-0.3.19/project_utils/web/flask/__init__.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-16 10:22:51.683668 project-utils-django-0.3.19/project_utils_django.egg-info/
--rw-r--r--   0 mylx2014   (501) staff       (20)     1674 2024-04-16 10:22:51.000000 project-utils-django-0.3.19/project_utils_django.egg-info/PKG-INFO
--rw-r--r--   0 mylx2014   (501) staff       (20)     4854 2024-04-16 10:22:51.000000 project-utils-django-0.3.19/project_utils_django.egg-info/SOURCES.txt
--rw-r--r--   0 mylx2014   (501) staff       (20)        1 2024-04-16 10:22:51.000000 project-utils-django-0.3.19/project_utils_django.egg-info/dependency_links.txt
--rw-r--r--   0 mylx2014   (501) staff       (20)       76 2024-04-16 10:22:51.000000 project-utils-django-0.3.19/project_utils_django.egg-info/requires.txt
--rw-r--r--   0 mylx2014   (501) staff       (20)       14 2024-04-16 10:22:51.000000 project-utils-django-0.3.19/project_utils_django.egg-info/top_level.txt
--rw-r--r--   0 mylx2014   (501) staff       (20)       38 2024-04-16 10:22:51.685730 project-utils-django-0.3.19/setup.cfg
--rw-r--r--   0 mylx2014   (501) staff       (20)      823 2024-04-16 10:22:35.000000 project-utils-django-0.3.19/setup.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-16 10:29:45.425403 project-utils-django-1.0.1/
+-rw-r--r--   0 mylx2014   (501) staff       (20)        0 2023-10-13 07:03:44.000000 project-utils-django-1.0.1/LICENSE
+-rw-r--r--   0 mylx2014   (501) staff       (20)     1876 2024-04-16 10:29:45.425153 project-utils-django-1.0.1/PKG-INFO
+-rw-r--r--   0 mylx2014   (501) staff       (20)     1289 2023-11-24 01:16:34.000000 project-utils-django-1.0.1/README.md
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-16 10:29:45.405182 project-utils-django-1.0.1/project_utils/
+-rw-r--r--   0 mylx2014   (501) staff       (20)        0 2023-10-13 02:35:45.000000 project-utils-django-1.0.1/project_utils/__init__.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-16 10:29:45.405725 project-utils-django-1.0.1/project_utils/collection/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      140 2023-10-14 01:51:03.000000 project-utils-django-1.0.1/project_utils/collection/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      596 2023-10-13 02:35:45.000000 project-utils-django-1.0.1/project_utils/collection/list_util.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-16 10:29:45.406522 project-utils-django-1.0.1/project_utils/config/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      155 2023-10-14 01:51:03.000000 project-utils-django-1.0.1/project_utils/config/__init__.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-16 10:29:45.407915 project-utils-django-1.0.1/project_utils/config/addr_config/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      652 2023-10-14 01:51:03.000000 project-utils-django-1.0.1/project_utils/config/addr_config/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      739 2023-11-24 01:16:34.000000 project-utils-django-1.0.1/project_utils/config/addr_config/base_config.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)       86 2023-10-14 01:51:03.000000 project-utils-django-1.0.1/project_utils/config/addr_config/hbase_config.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      777 2023-10-14 01:51:03.000000 project-utils-django-1.0.1/project_utils/config/addr_config/kafka_config.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      695 2023-10-14 01:51:03.000000 project-utils-django-1.0.1/project_utils/config/addr_config/mysql_config.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      825 2023-11-24 01:16:34.000000 project-utils-django-1.0.1/project_utils/config/addr_config/redis_config.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     1039 2023-10-14 01:51:03.000000 project-utils-django-1.0.1/project_utils/config/base_config.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-16 10:29:45.408406 project-utils-django-1.0.1/project_utils/config/path_config/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      130 2023-10-14 01:51:03.000000 project-utils-django-1.0.1/project_utils/config/path_config/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      970 2023-10-13 02:35:45.000000 project-utils-django-1.0.1/project_utils/config/path_config/path_config.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     1977 2023-10-14 01:51:03.000000 project-utils-django-1.0.1/project_utils/config/template.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-16 10:29:45.408596 project-utils-django-1.0.1/project_utils/db/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      164 2023-10-14 01:57:29.000000 project-utils-django-1.0.1/project_utils/db/__init__.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-16 10:29:45.409724 project-utils-django-1.0.1/project_utils/db/mysql/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      257 2023-10-14 01:57:29.000000 project-utils-django-1.0.1/project_utils/db/mysql/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     3484 2023-11-28 08:48:43.000000 project-utils-django-1.0.1/project_utils/db/mysql/_collection.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     2291 2023-12-15 01:39:50.000000 project-utils-django-1.0.1/project_utils/db/mysql/_pool.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      832 2023-11-24 01:16:34.000000 project-utils-django-1.0.1/project_utils/db/mysql/_result.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      107 2023-10-13 02:35:45.000000 project-utils-django-1.0.1/project_utils/db/mysql/_types.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-16 10:29:45.410306 project-utils-django-1.0.1/project_utils/exception/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      811 2023-10-14 02:37:02.000000 project-utils-django-1.0.1/project_utils/exception/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      148 2023-10-14 02:37:02.000000 project-utils-django-1.0.1/project_utils/exception/collection_exception.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      144 2023-10-14 02:37:02.000000 project-utils-django-1.0.1/project_utils/exception/config_exception.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-16 10:29:45.410580 project-utils-django-1.0.1/project_utils/exception/db_exception/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      141 2023-10-14 02:37:02.000000 project-utils-django-1.0.1/project_utils/exception/db_exception/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      118 2023-10-14 02:37:02.000000 project-utils-django-1.0.1/project_utils/exception/db_exception/mysql_exception.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      507 2023-10-13 02:35:45.000000 project-utils-django-1.0.1/project_utils/exception/my_base_exception.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-16 10:29:45.410718 project-utils-django-1.0.1/project_utils/exception/web_exception/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      142 2023-10-14 02:37:02.000000 project-utils-django-1.0.1/project_utils/exception/web_exception/__init__.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-16 10:29:45.411125 project-utils-django-1.0.1/project_utils/exception/web_exception/django_exception/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      125 2023-10-14 02:37:02.000000 project-utils-django-1.0.1/project_utils/exception/web_exception/django_exception/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      127 2023-10-14 02:37:02.000000 project-utils-django-1.0.1/project_utils/exception/web_exception/django_exception/model_exception.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-16 10:29:45.411397 project-utils-django-1.0.1/project_utils/exception/web_exception/django_exception/view_exception/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      275 2023-10-18 02:20:38.000000 project-utils-django-1.0.1/project_utils/exception/web_exception/django_exception/view_exception/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      120 2023-10-14 02:37:02.000000 project-utils-django-1.0.1/project_utils/exception/web_exception/django_exception/view_exception/response_exception.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     1255 2023-10-13 02:35:45.000000 project-utils-django-1.0.1/project_utils/io.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-16 10:29:45.411672 project-utils-django-1.0.1/project_utils/os/
+-rw-r--r--   0 mylx2014   (501) staff       (20)       98 2023-10-14 02:37:02.000000 project-utils-django-1.0.1/project_utils/os/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      760 2023-10-13 02:35:45.000000 project-utils-django-1.0.1/project_utils/os/dir.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     2029 2024-01-16 07:43:03.000000 project-utils-django-1.0.1/project_utils/time.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-16 10:29:45.411806 project-utils-django-1.0.1/project_utils/web/
+-rw-r--r--   0 mylx2014   (501) staff       (20)        0 2023-10-13 02:35:45.000000 project-utils-django-1.0.1/project_utils/web/__init__.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-16 10:29:45.411889 project-utils-django-1.0.1/project_utils/web/aiohttp/
+-rw-r--r--   0 mylx2014   (501) staff       (20)        0 2023-10-13 02:35:45.000000 project-utils-django-1.0.1/project_utils/web/aiohttp/__init__.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-16 10:29:45.412116 project-utils-django-1.0.1/project_utils/web/django/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      463 2023-10-14 02:37:02.000000 project-utils-django-1.0.1/project_utils/web/django/__init__.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-16 10:29:45.412535 project-utils-django-1.0.1/project_utils/web/django/celery/
+-rw-r--r--   0 mylx2014   (501) staff       (20)       84 2023-10-14 02:37:02.000000 project-utils-django-1.0.1/project_utils/web/django/celery/__init__.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-16 10:29:45.412805 project-utils-django-1.0.1/project_utils/web/django/celery/_conf/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      142 2023-10-14 02:37:02.000000 project-utils-django-1.0.1/project_utils/web/django/celery/_conf/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     1061 2023-11-24 01:16:34.000000 project-utils-django-1.0.1/project_utils/web/django/celery/_conf/_celery_config.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      334 2023-10-18 01:14:46.000000 project-utils-django-1.0.1/project_utils/web/django/celery/create_app.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-16 10:29:45.413074 project-utils-django-1.0.1/project_utils/web/django/conf/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      155 2023-10-14 02:37:02.000000 project-utils-django-1.0.1/project_utils/web/django/conf/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     2145 2023-11-24 01:16:34.000000 project-utils-django-1.0.1/project_utils/web/django/conf/_django_config.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-16 10:29:45.413401 project-utils-django-1.0.1/project_utils/web/django/middle/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      124 2023-10-14 02:37:02.000000 project-utils-django-1.0.1/project_utils/web/django/middle/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     1161 2023-11-24 01:16:34.000000 project-utils-django-1.0.1/project_utils/web/django/middle/_base_middle.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-16 10:29:45.414545 project-utils-django-1.0.1/project_utils/web/django/model/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      434 2024-01-15 14:04:29.000000 project-utils-django-1.0.1/project_utils/web/django/model/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      106 2023-12-10 05:49:34.000000 project-utils-django-1.0.1/project_utils/web/django/model/_base_meta.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     1511 2024-01-15 14:04:29.000000 project-utils-django-1.0.1/project_utils/web/django/model/_base_model.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      487 2023-12-08 06:57:16.000000 project-utils-django-1.0.1/project_utils/web/django/model/_id_model.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      461 2024-01-15 14:04:29.000000 project-utils-django-1.0.1/project_utils/web/django/model/_model_type.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-16 10:29:45.415146 project-utils-django-1.0.1/project_utils/web/django/pagination/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      197 2023-10-14 02:37:02.000000 project-utils-django-1.0.1/project_utils/web/django/pagination/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     1011 2023-11-24 01:16:34.000000 project-utils-django-1.0.1/project_utils/web/django/pagination/_base_pagination.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-16 10:29:45.415583 project-utils-django-1.0.1/project_utils/web/django/request/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      102 2023-10-14 02:37:02.000000 project-utils-django-1.0.1/project_utils/web/django/request/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     1379 2023-11-24 01:16:34.000000 project-utils-django-1.0.1/project_utils/web/django/request/_request.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-16 10:29:45.416207 project-utils-django-1.0.1/project_utils/web/django/response/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      153 2023-10-14 02:37:02.000000 project-utils-django-1.0.1/project_utils/web/django/response/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     1291 2023-10-14 02:37:02.000000 project-utils-django-1.0.1/project_utils/web/django/response/_response_model.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      213 2023-11-24 01:16:34.000000 project-utils-django-1.0.1/project_utils/web/django/response/_response_types.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-16 10:29:45.416694 project-utils-django-1.0.1/project_utils/web/django/serializer/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      130 2023-10-14 02:37:02.000000 project-utils-django-1.0.1/project_utils/web/django/serializer/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      284 2023-10-13 02:35:45.000000 project-utils-django-1.0.1/project_utils/web/django/serializer/_base_meta.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      418 2023-10-14 02:37:02.000000 project-utils-django-1.0.1/project_utils/web/django/serializer/_base_serializer.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-16 10:29:45.417152 project-utils-django-1.0.1/project_utils/web/django/swagger/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      499 2023-12-10 07:02:32.000000 project-utils-django-1.0.1/project_utils/web/django/swagger/__init__.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-16 10:29:45.418577 project-utils-django-1.0.1/project_utils/web/django/swagger/_params/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      675 2023-12-10 07:02:32.000000 project-utils-django-1.0.1/project_utils/web/django/swagger/_params/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      307 2023-12-10 07:02:32.000000 project-utils-django-1.0.1/project_utils/web/django/swagger/_params/_base.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     1025 2023-12-10 07:02:32.000000 project-utils-django-1.0.1/project_utils/web/django/swagger/_params/_form.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     1164 2023-12-10 07:02:32.000000 project-utils-django-1.0.1/project_utils/web/django/swagger/_params/_params.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      978 2023-12-10 07:02:32.000000 project-utils-django-1.0.1/project_utils/web/django/swagger/_params/_query.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     2065 2023-12-10 07:17:18.000000 project-utils-django-1.0.1/project_utils/web/django/swagger/_params/_response.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      412 2023-12-10 07:02:32.000000 project-utils-django-1.0.1/project_utils/web/django/swagger/_params/_types.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      268 2023-12-10 07:15:26.000000 project-utils-django-1.0.1/project_utils/web/django/swagger/_urls.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-16 10:29:45.419012 project-utils-django-1.0.1/project_utils/web/django/swagger/config/
+-rw-r--r--   0 mylx2014   (501) staff       (20)       69 2023-12-10 07:02:32.000000 project-utils-django-1.0.1/project_utils/web/django/swagger/config/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      488 2023-12-10 07:15:01.000000 project-utils-django-1.0.1/project_utils/web/django/swagger/config/_config.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     1274 2023-12-10 07:15:01.000000 project-utils-django-1.0.1/project_utils/web/django/swagger/config/_swagger.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-16 10:29:45.419545 project-utils-django-1.0.1/project_utils/web/django/swagger/document/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      256 2023-12-10 07:02:32.000000 project-utils-django-1.0.1/project_utils/web/django/swagger/document/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     1169 2023-12-10 07:15:01.000000 project-utils-django-1.0.1/project_utils/web/django/swagger/document/_document.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      273 2023-12-10 07:02:32.000000 project-utils-django-1.0.1/project_utils/web/django/swagger/document/_types.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      678 2023-11-24 01:16:34.000000 project-utils-django-1.0.1/project_utils/web/django/utils.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-16 10:29:45.420678 project-utils-django-1.0.1/project_utils/web/django/view/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      478 2023-12-10 07:02:32.000000 project-utils-django-1.0.1/project_utils/web/django/view/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     3840 2023-12-10 07:02:32.000000 project-utils-django-1.0.1/project_utils/web/django/view/_async_view.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     2086 2023-12-10 15:11:23.000000 project-utils-django-1.0.1/project_utils/web/django/view/_base.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-16 10:29:45.421331 project-utils-django-1.0.1/project_utils/web/django/view/_base_api/
+-rw-r--r--   0 mylx2014   (501) staff       (20)       57 2023-12-10 07:02:32.000000 project-utils-django-1.0.1/project_utils/web/django/view/_base_api/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     3277 2023-12-10 15:07:50.000000 project-utils-django-1.0.1/project_utils/web/django/view/_base_api/api.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      908 2023-12-10 15:07:50.000000 project-utils-django-1.0.1/project_utils/web/django/view/_base_api/api_util.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-16 10:29:45.422109 project-utils-django-1.0.1/project_utils/web/django/view/_rest_api/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      296 2023-12-10 07:02:32.000000 project-utils-django-1.0.1/project_utils/web/django/view/_rest_api/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     1921 2023-12-10 15:07:50.000000 project-utils-django-1.0.1/project_utils/web/django/view/_rest_api/api.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      480 2023-12-10 15:08:55.000000 project-utils-django-1.0.1/project_utils/web/django/view/_rest_api/api_utils.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     2020 2023-12-10 15:08:55.000000 project-utils-django-1.0.1/project_utils/web/django/view/_rest_api/async_api.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-16 10:29:45.423232 project-utils-django-1.0.1/project_utils/web/django/view/_rest_view/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      307 2023-12-10 07:02:32.000000 project-utils-django-1.0.1/project_utils/web/django/view/_rest_view/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)    12607 2023-12-10 15:16:37.000000 project-utils-django-1.0.1/project_utils/web/django/view/_rest_view/_async_base_view.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     3840 2023-12-10 15:11:23.000000 project-utils-django-1.0.1/project_utils/web/django/view/_rest_view/_async_view.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)    12432 2023-12-10 15:11:23.000000 project-utils-django-1.0.1/project_utils/web/django/view/_rest_view/_base_view.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     1243 2023-12-10 15:11:23.000000 project-utils-django-1.0.1/project_utils/web/django/view/_rest_view/_swagger_base.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     1243 2023-12-10 07:27:29.000000 project-utils-django-1.0.1/project_utils/web/django/view/_swagger_base.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      750 2023-12-10 07:02:32.000000 project-utils-django-1.0.1/project_utils/web/django/view/_types.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-16 10:29:45.423830 project-utils-django-1.0.1/project_utils/web/django/view/_user_view/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      185 2023-12-10 07:02:32.000000 project-utils-django-1.0.1/project_utils/web/django/view/_user_view/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      239 2023-12-10 15:11:23.000000 project-utils-django-1.0.1/project_utils/web/django/view/_user_view/_model.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)    11333 2023-12-10 15:11:23.000000 project-utils-django-1.0.1/project_utils/web/django/view/_user_view/_view.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-16 10:29:45.424121 project-utils-django-1.0.1/project_utils/web/fastapi/
+-rw-r--r--   0 mylx2014   (501) staff       (20)        0 2023-10-13 02:35:45.000000 project-utils-django-1.0.1/project_utils/web/fastapi/__init__.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-16 10:29:45.424239 project-utils-django-1.0.1/project_utils/web/flask/
+-rw-r--r--   0 mylx2014   (501) staff       (20)        0 2023-10-13 02:35:45.000000 project-utils-django-1.0.1/project_utils/web/flask/__init__.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-04-16 10:29:45.424877 project-utils-django-1.0.1/project_utils_django.egg-info/
+-rw-r--r--   0 mylx2014   (501) staff       (20)     1876 2024-04-16 10:29:45.000000 project-utils-django-1.0.1/project_utils_django.egg-info/PKG-INFO
+-rw-r--r--   0 mylx2014   (501) staff       (20)     4854 2024-04-16 10:29:45.000000 project-utils-django-1.0.1/project_utils_django.egg-info/SOURCES.txt
+-rw-r--r--   0 mylx2014   (501) staff       (20)        1 2024-04-16 10:29:45.000000 project-utils-django-1.0.1/project_utils_django.egg-info/dependency_links.txt
+-rw-r--r--   0 mylx2014   (501) staff       (20)       83 2024-04-16 10:29:45.000000 project-utils-django-1.0.1/project_utils_django.egg-info/requires.txt
+-rw-r--r--   0 mylx2014   (501) staff       (20)       14 2024-04-16 10:29:45.000000 project-utils-django-1.0.1/project_utils_django.egg-info/top_level.txt
+-rw-r--r--   0 mylx2014   (501) staff       (20)       38 2024-04-16 10:29:45.425444 project-utils-django-1.0.1/setup.cfg
+-rw-r--r--   0 mylx2014   (501) staff       (20)      829 2024-04-16 10:29:17.000000 project-utils-django-1.0.1/setup.py
```

### Comparing `project-utils-django-0.3.19/README.md` & `project-utils-django-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `project-utils-django-0.3.19/project_utils/collection/list_util.py` & `project-utils-django-1.0.1/project_utils/collection/list_util.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-0.3.19/project_utils/config/addr_config/__init__.py` & `project-utils-django-1.0.1/project_utils/config/addr_config/__init__.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-0.3.19/project_utils/config/addr_config/base_config.py` & `project-utils-django-1.0.1/project_utils/config/addr_config/base_config.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-0.3.19/project_utils/config/addr_config/kafka_config.py` & `project-utils-django-1.0.1/project_utils/config/addr_config/kafka_config.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-0.3.19/project_utils/config/addr_config/mysql_config.py` & `project-utils-django-1.0.1/project_utils/config/addr_config/mysql_config.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-0.3.19/project_utils/config/addr_config/redis_config.py` & `project-utils-django-1.0.1/project_utils/config/addr_config/redis_config.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-0.3.19/project_utils/config/base_config.py` & `project-utils-django-1.0.1/project_utils/config/base_config.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-0.3.19/project_utils/config/path_config/path_config.py` & `project-utils-django-1.0.1/project_utils/config/path_config/path_config.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-0.3.19/project_utils/config/template.py` & `project-utils-django-1.0.1/project_utils/config/template.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-0.3.19/project_utils/db/mysql/_collection.py` & `project-utils-django-1.0.1/project_utils/db/mysql/_collection.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-0.3.19/project_utils/db/mysql/_pool.py` & `project-utils-django-1.0.1/project_utils/db/mysql/_pool.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-0.3.19/project_utils/db/mysql/_result.py` & `project-utils-django-1.0.1/project_utils/db/mysql/_result.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-0.3.19/project_utils/exception/__init__.py` & `project-utils-django-1.0.1/project_utils/exception/__init__.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-0.3.19/project_utils/io.py` & `project-utils-django-1.0.1/project_utils/io.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-0.3.19/project_utils/os/dir.py` & `project-utils-django-1.0.1/project_utils/os/dir.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-0.3.19/project_utils/time.py` & `project-utils-django-1.0.1/project_utils/time.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-0.3.19/project_utils/web/django/celery/_conf/_celery_config.py` & `project-utils-django-1.0.1/project_utils/web/django/celery/_conf/_celery_config.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-0.3.19/project_utils/web/django/conf/_django_config.py` & `project-utils-django-1.0.1/project_utils/web/django/conf/_django_config.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-0.3.19/project_utils/web/django/middle/_base_middle.py` & `project-utils-django-1.0.1/project_utils/web/django/middle/_base_middle.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-0.3.19/project_utils/web/django/model/_base_model.py` & `project-utils-django-1.0.1/project_utils/web/django/model/_base_model.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-0.3.19/project_utils/web/django/pagination/_base_pagination.py` & `project-utils-django-1.0.1/project_utils/web/django/pagination/_base_pagination.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-0.3.19/project_utils/web/django/request/_request.py` & `project-utils-django-1.0.1/project_utils/web/django/request/_request.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-0.3.19/project_utils/web/django/response/_response_model.py` & `project-utils-django-1.0.1/project_utils/web/django/response/_response_model.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-0.3.19/project_utils/web/django/swagger/_params/__init__.py` & `project-utils-django-1.0.1/project_utils/web/django/swagger/_params/__init__.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-0.3.19/project_utils/web/django/swagger/_params/_form.py` & `project-utils-django-1.0.1/project_utils/web/django/swagger/_params/_form.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-0.3.19/project_utils/web/django/swagger/_params/_params.py` & `project-utils-django-1.0.1/project_utils/web/django/swagger/_params/_params.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-0.3.19/project_utils/web/django/swagger/_params/_query.py` & `project-utils-django-1.0.1/project_utils/web/django/swagger/_params/_query.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-0.3.19/project_utils/web/django/swagger/_params/_response.py` & `project-utils-django-1.0.1/project_utils/web/django/swagger/_params/_response.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-0.3.19/project_utils/web/django/swagger/config/_swagger.py` & `project-utils-django-1.0.1/project_utils/web/django/swagger/config/_swagger.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-0.3.19/project_utils/web/django/swagger/document/_document.py` & `project-utils-django-1.0.1/project_utils/web/django/swagger/document/_document.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-0.3.19/project_utils/web/django/utils.py` & `project-utils-django-1.0.1/project_utils/web/django/utils.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-0.3.19/project_utils/web/django/view/_async_view.py` & `project-utils-django-1.0.1/project_utils/web/django/view/_async_view.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-0.3.19/project_utils/web/django/view/_base.py` & `project-utils-django-1.0.1/project_utils/web/django/view/_base.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-0.3.19/project_utils/web/django/view/_base_api/api.py` & `project-utils-django-1.0.1/project_utils/web/django/view/_base_api/api.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-0.3.19/project_utils/web/django/view/_base_api/api_util.py` & `project-utils-django-1.0.1/project_utils/web/django/view/_base_api/api_util.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-0.3.19/project_utils/web/django/view/_rest_api/api.py` & `project-utils-django-1.0.1/project_utils/web/django/view/_rest_api/api.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-0.3.19/project_utils/web/django/view/_rest_api/async_api.py` & `project-utils-django-1.0.1/project_utils/web/django/view/_rest_api/async_api.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-0.3.19/project_utils/web/django/view/_rest_view/_async_base_view.py` & `project-utils-django-1.0.1/project_utils/web/django/view/_rest_view/_async_base_view.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-0.3.19/project_utils/web/django/view/_rest_view/_async_view.py` & `project-utils-django-1.0.1/project_utils/web/django/view/_rest_view/_async_view.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-0.3.19/project_utils/web/django/view/_rest_view/_base_view.py` & `project-utils-django-1.0.1/project_utils/web/django/view/_rest_view/_base_view.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-0.3.19/project_utils/web/django/view/_rest_view/_swagger_base.py` & `project-utils-django-1.0.1/project_utils/web/django/view/_rest_view/_swagger_base.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-0.3.19/project_utils/web/django/view/_swagger_base.py` & `project-utils-django-1.0.1/project_utils/web/django/view/_swagger_base.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-0.3.19/project_utils/web/django/view/_types.py` & `project-utils-django-1.0.1/project_utils/web/django/view/_types.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-0.3.19/project_utils/web/django/view/_user_view/_view.py` & `project-utils-django-1.0.1/project_utils/web/django/view/_user_view/_view.py`

 * *Files identical despite different names*

### Comparing `project-utils-django-0.3.19/project_utils_django.egg-info/SOURCES.txt` & `project-utils-django-1.0.1/project_utils_django.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `project-utils-django-0.3.19/setup.py` & `project-utils-django-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.3.19"
+VERSION = "1.0.1"
 DESCRIPTION = "python project_utils tools"
 setup(
     name="project-utils-django",
     version=VERSION,
     author="mylx2014",
     author_email="mylx2014@163.com",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=open('README.md', encoding="UTF8").read(),
     packages=find_packages(),
-    install_requires=['loguru', 'dbutils', 'pymysql', "django", "djangorestframework", "drf-yasg", "asyncio",
+    install_requires=['loguru', 'dbutils', 'pymysql', "django==3.0.0", "djangorestframework", "drf-yasg", "asyncio",
                       "aiofiles"],
     keywords=['python', 'utils', 'project utils', "aiofiles"],
     data_files=[],
     entry_points={},
     license="MIT",
     url="https://gitee.com/mylx2014/project-utils-django.git",
     scripts=[],
```

