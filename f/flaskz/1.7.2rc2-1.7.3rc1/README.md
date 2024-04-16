# Comparing `tmp/flaskz-1.7.2rc2.tar.gz` & `tmp/flaskz-1.7.3rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flaskz-1.7.2rc2.tar", last modified: Fri Jan 26 02:56:58 2024, max compression
+gzip compressed data, was "flaskz-1.7.3rc1.tar", last modified: Tue Apr 16 02:00:09 2024, max compression
```

## Comparing `flaskz-1.7.2rc2.tar` & `flaskz-1.7.3rc1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2024-01-26 02:56:58.399527 flaskz-1.7.2rc2/
--rwxrwxrwx   0 taozh      (501) staff       (20)     1070 2023-12-29 07:22:00.000000 flaskz-1.7.2rc2/LICENSE
--rw-r--r--   0 taozh      (501) staff       (20)     9150 2024-01-26 02:56:58.399295 flaskz-1.7.2rc2/PKG-INFO
--rwxrwxrwx   0 taozh      (501) staff       (20)     8537 2024-01-26 02:35:46.000000 flaskz-1.7.2rc2/README.md
--rwxrwxrwx   0 taozh      (501) staff       (20)      108 2021-10-20 06:20:46.000000 flaskz-1.7.2rc2/pyproject.toml
--rwxrwxrwx   0 taozh      (501) staff       (20)      778 2024-01-26 02:56:58.400299 flaskz-1.7.2rc2/setup.cfg
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2024-01-26 02:56:58.361794 flaskz-1.7.2rc2/src/
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2024-01-26 02:56:58.367026 flaskz-1.7.2rc2/src/flaskz/
--rwxrwxrwx   0 taozh      (501) staff       (20)       25 2024-01-26 02:37:12.000000 flaskz-1.7.2rc2/src/flaskz/__init__.py
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2024-01-26 02:56:58.372136 flaskz-1.7.2rc2/src/flaskz/auth/
--rw-r--r--   0 taozh      (501) staff       (20)       20 2022-09-19 02:49:18.000000 flaskz-1.7.2rc2/src/flaskz/auth/__init__.py
--rw-r--r--   0 taozh      (501) staff       (20)     8563 2023-11-06 11:28:38.000000 flaskz-1.7.2rc2/src/flaskz/auth/_jws.py
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2024-01-26 02:56:58.375624 flaskz-1.7.2rc2/src/flaskz/ext/
--rw-r--r--   0 taozh      (501) staff       (20)      117 2023-04-27 10:17:39.000000 flaskz-1.7.2rc2/src/flaskz/ext/__init__.py
--rw-r--r--   0 taozh      (501) staff       (20)     8661 2023-12-11 08:39:54.000000 flaskz-1.7.2rc2/src/flaskz/ext/cypher.py
--rw-r--r--   0 taozh      (501) staff       (20)    21686 2023-12-31 10:16:20.000000 flaskz-1.7.2rc2/src/flaskz/ext/ssh.py
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2024-01-26 02:56:58.377430 flaskz-1.7.2rc2/src/flaskz/log/
--rwxrwxrwx   0 taozh      (501) staff       (20)     2395 2023-07-06 02:14:56.000000 flaskz-1.7.2rc2/src/flaskz/log/__init__.py
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2024-01-26 02:56:58.383233 flaskz-1.7.2rc2/src/flaskz/models/
--rwxrwxrwx   0 taozh      (501) staff       (20)     5909 2024-01-04 07:54:53.000000 flaskz-1.7.2rc2/src/flaskz/models/__init__.py
--rwxrwxrwx   0 taozh      (501) staff       (20)    31374 2024-01-22 02:47:13.000000 flaskz-1.7.2rc2/src/flaskz/models/_base.py
--rwxrwxrwx   0 taozh      (501) staff       (20)    11055 2024-01-22 02:47:13.000000 flaskz-1.7.2rc2/src/flaskz/models/_model.py
--rw-r--r--   0 taozh      (501) staff       (20)    19674 2024-01-22 02:47:13.000000 flaskz-1.7.2rc2/src/flaskz/models/_query_util.py
--rwxrwxrwx   0 taozh      (501) staff       (20)    11011 2024-01-04 03:49:56.000000 flaskz-1.7.2rc2/src/flaskz/models/_util.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     1316 2021-10-25 05:47:22.000000 flaskz-1.7.2rc2/src/flaskz/res_status_codes.py
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2024-01-26 02:56:58.386179 flaskz-1.7.2rc2/src/flaskz/rest/
--rwxrwxrwx   0 taozh      (501) staff       (20)    21363 2024-01-01 06:50:15.000000 flaskz-1.7.2rc2/src/flaskz/rest/__init__.py
--rwxrwxrwx   0 taozh      (501) staff       (20)      960 2023-04-26 02:54:40.000000 flaskz-1.7.2rc2/src/flaskz/rest/_mgmt.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     4173 2023-12-30 16:50:29.000000 flaskz-1.7.2rc2/src/flaskz/rest/_util.py
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2024-01-26 02:56:58.396722 flaskz-1.7.2rc2/src/flaskz/utils/
--rwxrwxrwx   0 taozh      (501) staff       (20)      251 2023-06-21 05:37:43.000000 flaskz-1.7.2rc2/src/flaskz/utils/__init__.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     2502 2023-12-30 16:37:35.000000 flaskz-1.7.2rc2/src/flaskz/utils/_app.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     2848 2023-12-30 16:37:56.000000 flaskz-1.7.2rc2/src/flaskz/utils/_cache.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     7039 2023-12-30 16:47:31.000000 flaskz-1.7.2rc2/src/flaskz/utils/_cls.py
--rwxrwxrwx   0 taozh      (501) staff       (20)    13669 2024-01-17 09:40:36.000000 flaskz-1.7.2rc2/src/flaskz/utils/_common.py
--rw-r--r--   0 taozh      (501) staff       (20)      860 2023-12-30 16:48:17.000000 flaskz-1.7.2rc2/src/flaskz/utils/_func.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     2785 2023-04-26 10:28:36.000000 flaskz-1.7.2rc2/src/flaskz/utils/_magic.py
--rw-r--r--   0 taozh      (501) staff       (20)     1020 2023-12-30 16:50:25.000000 flaskz-1.7.2rc2/src/flaskz/utils/_private.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     8044 2024-01-26 02:55:12.000000 flaskz-1.7.2rc2/src/flaskz/utils/_request_api.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     1201 2023-12-30 16:50:25.000000 flaskz-1.7.2rc2/src/flaskz/utils/_request_args.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     2734 2023-12-30 13:54:33.000000 flaskz-1.7.2rc2/src/flaskz/utils/_response.py
--rw-r--r--   0 taozh      (501) staff       (20)     4322 2023-12-30 13:56:42.000000 flaskz-1.7.2rc2/src/flaskz/utils/_timer.py
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2024-01-26 02:56:58.398091 flaskz-1.7.2rc2/src/flaskz.egg-info/
--rw-r--r--   0 taozh      (501) staff       (20)     9150 2024-01-26 02:56:58.000000 flaskz-1.7.2rc2/src/flaskz.egg-info/PKG-INFO
--rwxrwxrwx   0 taozh      (501) staff       (20)      981 2024-01-26 02:56:58.000000 flaskz-1.7.2rc2/src/flaskz.egg-info/SOURCES.txt
--rwxrwxrwx   0 taozh      (501) staff       (20)        1 2024-01-26 02:56:58.000000 flaskz-1.7.2rc2/src/flaskz.egg-info/dependency_links.txt
--rwxrwxrwx   0 taozh      (501) staff       (20)       87 2024-01-26 02:56:58.000000 flaskz-1.7.2rc2/src/flaskz.egg-info/requires.txt
--rwxrwxrwx   0 taozh      (501) staff       (20)        7 2024-01-26 02:56:58.000000 flaskz-1.7.2rc2/src/flaskz.egg-info/top_level.txt
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2024-04-16 02:00:09.550594 flaskz-1.7.3rc1/
+-rwxrwxrwx   0 taozh      (501) staff       (20)     1070 2023-12-29 07:22:00.000000 flaskz-1.7.3rc1/LICENSE
+-rw-r--r--   0 taozh      (501) staff       (20)     9710 2024-04-16 02:00:09.550215 flaskz-1.7.3rc1/PKG-INFO
+-rwxrwxrwx   0 taozh      (501) staff       (20)     9102 2024-04-15 11:36:23.000000 flaskz-1.7.3rc1/README.md
+-rwxrwxrwx   0 taozh      (501) staff       (20)      108 2021-10-20 06:20:46.000000 flaskz-1.7.3rc1/pyproject.toml
+-rwxrwxrwx   0 taozh      (501) staff       (20)      778 2024-04-16 02:00:09.551653 flaskz-1.7.3rc1/setup.cfg
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2024-04-16 02:00:09.506875 flaskz-1.7.3rc1/src/
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2024-04-16 02:00:09.512737 flaskz-1.7.3rc1/src/flaskz/
+-rwxrwxrwx   0 taozh      (501) staff       (20)       25 2024-04-14 04:30:05.000000 flaskz-1.7.3rc1/src/flaskz/__init__.py
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2024-04-16 02:00:09.516736 flaskz-1.7.3rc1/src/flaskz/auth/
+-rw-r--r--   0 taozh      (501) staff       (20)       20 2022-09-19 02:49:18.000000 flaskz-1.7.3rc1/src/flaskz/auth/__init__.py
+-rw-r--r--   0 taozh      (501) staff       (20)     8563 2023-11-06 11:28:38.000000 flaskz-1.7.3rc1/src/flaskz/auth/_jws.py
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2024-04-16 02:00:09.520306 flaskz-1.7.3rc1/src/flaskz/ext/
+-rw-r--r--   0 taozh      (501) staff       (20)      117 2023-04-27 10:17:39.000000 flaskz-1.7.3rc1/src/flaskz/ext/__init__.py
+-rw-r--r--   0 taozh      (501) staff       (20)     8661 2023-12-11 08:39:54.000000 flaskz-1.7.3rc1/src/flaskz/ext/cypher.py
+-rw-r--r--   0 taozh      (501) staff       (20)    22378 2024-04-15 12:15:00.000000 flaskz-1.7.3rc1/src/flaskz/ext/ssh.py
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2024-04-16 02:00:09.520831 flaskz-1.7.3rc1/src/flaskz/log/
+-rwxrwxrwx   0 taozh      (501) staff       (20)     2395 2023-07-06 02:14:56.000000 flaskz-1.7.3rc1/src/flaskz/log/__init__.py
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2024-04-16 02:00:09.527060 flaskz-1.7.3rc1/src/flaskz/models/
+-rwxrwxrwx   0 taozh      (501) staff       (20)     6102 2024-02-02 04:22:48.000000 flaskz-1.7.3rc1/src/flaskz/models/__init__.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)    31531 2024-04-14 10:04:24.000000 flaskz-1.7.3rc1/src/flaskz/models/_base.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)    11055 2024-01-22 02:47:13.000000 flaskz-1.7.3rc1/src/flaskz/models/_model.py
+-rw-r--r--   0 taozh      (501) staff       (20)    20087 2024-04-07 02:45:01.000000 flaskz-1.7.3rc1/src/flaskz/models/_query_util.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)    11212 2024-04-14 09:19:30.000000 flaskz-1.7.3rc1/src/flaskz/models/_util.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     1316 2021-10-25 05:47:22.000000 flaskz-1.7.3rc1/src/flaskz/res_status_codes.py
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2024-04-16 02:00:09.531391 flaskz-1.7.3rc1/src/flaskz/rest/
+-rwxrwxrwx   0 taozh      (501) staff       (20)    21363 2024-01-01 06:50:15.000000 flaskz-1.7.3rc1/src/flaskz/rest/__init__.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)      960 2023-04-26 02:54:40.000000 flaskz-1.7.3rc1/src/flaskz/rest/_mgmt.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     4173 2023-12-30 16:50:29.000000 flaskz-1.7.3rc1/src/flaskz/rest/_util.py
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2024-04-16 02:00:09.547250 flaskz-1.7.3rc1/src/flaskz/utils/
+-rwxrwxrwx   0 taozh      (501) staff       (20)      251 2023-06-21 05:37:43.000000 flaskz-1.7.3rc1/src/flaskz/utils/__init__.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     2502 2023-12-30 16:37:35.000000 flaskz-1.7.3rc1/src/flaskz/utils/_app.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     2848 2023-12-30 16:37:56.000000 flaskz-1.7.3rc1/src/flaskz/utils/_cache.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     7248 2024-04-14 10:55:34.000000 flaskz-1.7.3rc1/src/flaskz/utils/_cls.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)    13669 2024-01-17 09:40:36.000000 flaskz-1.7.3rc1/src/flaskz/utils/_common.py
+-rw-r--r--   0 taozh      (501) staff       (20)      860 2023-12-30 16:48:17.000000 flaskz-1.7.3rc1/src/flaskz/utils/_func.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     2785 2023-04-26 10:28:36.000000 flaskz-1.7.3rc1/src/flaskz/utils/_magic.py
+-rw-r--r--   0 taozh      (501) staff       (20)     1020 2023-12-30 16:50:25.000000 flaskz-1.7.3rc1/src/flaskz/utils/_private.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     7933 2024-01-30 02:20:56.000000 flaskz-1.7.3rc1/src/flaskz/utils/_request_api.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     1201 2023-12-30 16:50:25.000000 flaskz-1.7.3rc1/src/flaskz/utils/_request_args.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     3045 2024-01-30 02:31:20.000000 flaskz-1.7.3rc1/src/flaskz/utils/_response.py
+-rw-r--r--   0 taozh      (501) staff       (20)     4322 2023-12-30 13:56:42.000000 flaskz-1.7.3rc1/src/flaskz/utils/_timer.py
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2024-04-16 02:00:09.548505 flaskz-1.7.3rc1/src/flaskz.egg-info/
+-rw-r--r--   0 taozh      (501) staff       (20)     9710 2024-04-16 02:00:09.000000 flaskz-1.7.3rc1/src/flaskz.egg-info/PKG-INFO
+-rwxrwxrwx   0 taozh      (501) staff       (20)      981 2024-04-16 02:00:09.000000 flaskz-1.7.3rc1/src/flaskz.egg-info/SOURCES.txt
+-rwxrwxrwx   0 taozh      (501) staff       (20)        1 2024-04-16 02:00:09.000000 flaskz-1.7.3rc1/src/flaskz.egg-info/dependency_links.txt
+-rwxrwxrwx   0 taozh      (501) staff       (20)       87 2024-04-16 02:00:09.000000 flaskz-1.7.3rc1/src/flaskz.egg-info/requires.txt
+-rwxrwxrwx   0 taozh      (501) staff       (20)        7 2024-04-16 02:00:09.000000 flaskz-1.7.3rc1/src/flaskz.egg-info/top_level.txt
```

### Comparing `flaskz-1.7.2rc2/LICENSE` & `flaskz-1.7.3rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `flaskz-1.7.2rc2/PKG-INFO` & `flaskz-1.7.3rc1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flaskz
-Version: 1.7.2rc2
+Version: 1.7.3rc1
 Summary: Flask and SQLAlchemy extensions for web applications
 Home-page: https://github.com/taozh1982/flaskz
 Author: Zhang Tao
 Author-email: taozh1982@gmail.com
 Project-URL: Bug Tracker, https://github.com/taozh1982/flaskz/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -30,35 +30,40 @@
 3. [☞API封装、访问权限控制和系统日志](http://zhangyiheng.com/blog/articles/py_flaskz_api.html)
 4. [☞常用函数](http://zhangyiheng.com/blog/articles/py_flaskz_utils.html)
 5. [☞基于Flaskz的管理系统开发模板 Flaskz-admin](http://zhangyiheng.com/blog/articles/py_flaskz_admin.html)
 6. [☞使用手册](http://zhangyiheng.com/blog/articles/py_flaskz_manual.html)
 
 ## 版本
 
-- **1.7.2rc2** `2024/01/26`
-    - [A] `flaskz.utils.api_request`函数添加`http_kwargs`参数，用于设置http请求参数
-- **1.7.2rc1** `2024/01/22`
-    - [A] `flaskz.models.parse_pss`函数支持`like_columns`参数, 用于定义模糊查询列(默认使用模型类的like_columns)
+- **1.7.3rc1** `2024/04/16`
+    - [C] `flaskz.utils.ins_to_dict`函数返回的dict中包含值为`None`的键值
+    - [A] `BaseModelMixin.to_dict`方法的`option`参数添加`relationships`选项，用于自定义是否查询关联关系
+    - [A] `FLASKZ_DATABASE_SESSION_KWARGS`配置参数添加`reusable_in_flask_g`选项, 用于设置是否在`flask.g`中缓存&复用`session`对象(默认启用)
+    - [C] `flaskz.ext.ssh`返回值保留文本两侧的空格
+    - [A] `flaskz.ext.ssh.SSH`添加`pre_commands`参数, 用于在命令执行之前预先执行控制相关命令
 
+- **1.7.2** `2024/02/01`
+    - [A] `flaskz.models.parse_pss`函数支持`like_columns`参数, 用于定义模糊查询列(默认使用模型类的like_columns)
+    - [A] `flaskz.utils.api_request`函数添加`http_kwargs`参数，用于设置http请求参数
 - **1.7.1** `2024/01/05`
     - [F] 修复SQLAlchemy<2.0.0版本时, `flaskz.models._util.py`中`BinaryExpression`类的导入问题
 - **1.7.0** `2024/01/01`
     - [C] `SQLAlchemy`依赖的版本从`>=1.3.13(EOL)`升级到`>=1.4.0(Maintenance)`
     - [A] `BaseModelMixin.query_pss`方法支持`relationship`的查询和排序
     - [A] `flaskz.models.parse_pss`函数支持`relationship`的查询和排序参数解析
 - **1.6.4** `2023/12/01`
     - [A] `BaseModelMixin`添加`refresh`方法, 用于更新当前模型对象
     - [A] 添加`flaskz.models.refresh_instance`函数, 用于更新模型对象/列表
     - [A] `model_to_dict`函数的`option`参数添加`filter`选项, 用于过滤模型对象列表
     - [A] `flaskz.rest.register_model_query_pss_route`路由生成函数添加`get_pss_config`参数, 用于自定义pss查询参数
     - [A] `flaskz.ext.ssh`添加`ssh_run_command`和`ssh_run_command_list`函数
     - [A] `flaskz.ext.ssh.SSH`添加`connect_kwargs`和`channel_kwargs`参数以自定义connect和channel参数
-    - [A] `flaskz.ext.ssh.SSH`添加`timeout`参数的默认值为`10`
+    - [A] `flaskz.ext.ssh.SSH`设置`timeout`参数的默认值为`10`
 - **1.6.3** `2023/09/01`
-    - [A] 添加`FLASKZ_DATABASE_SESSION_KWARGS`参数, 用于自定义`DBSession`参数
+    - [A] 添加`FLASKZ_DATABASE_SESSION_KWARGS`配置参数, 用于自定义`DBSession`参数
     - [C] `BaseModelMixin.add_db`和`BaseModelMixin.update_db`方法添加`refresh`操作, 以返回跟数据库同步的instance对象
     - [A] `flaskz.rest.register_model_*`路由生成函数添加路由`endpoint`参数
 - **1.6.2** `2023/07/06`
     - [F] 修复`flaskz.utils._request_args.py`中`import parse_pss as get_pss`的导入问题
 - **1.6.1** `2023/07/01`
     - [C] `flaskz.utils.get_pss`(`flaskz.models.parse_pss`)函数返回项由SQL字符串拼接改为参数化模式以预防SQL注入
     - [A] 添加`flaskz.utils.run_at`函数用于执行定时函数
```

### Comparing `flaskz-1.7.2rc2/README.md` & `flaskz-1.7.3rc1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -9,35 +9,40 @@
 3. [☞API封装、访问权限控制和系统日志](http://zhangyiheng.com/blog/articles/py_flaskz_api.html)
 4. [☞常用函数](http://zhangyiheng.com/blog/articles/py_flaskz_utils.html)
 5. [☞基于Flaskz的管理系统开发模板 Flaskz-admin](http://zhangyiheng.com/blog/articles/py_flaskz_admin.html)
 6. [☞使用手册](http://zhangyiheng.com/blog/articles/py_flaskz_manual.html)
 
 ## 版本
 
-- **1.7.2rc2** `2024/01/26`
-    - [A] `flaskz.utils.api_request`函数添加`http_kwargs`参数，用于设置http请求参数
-- **1.7.2rc1** `2024/01/22`
-    - [A] `flaskz.models.parse_pss`函数支持`like_columns`参数, 用于定义模糊查询列(默认使用模型类的like_columns)
+- **1.7.3rc1** `2024/04/16`
+    - [C] `flaskz.utils.ins_to_dict`函数返回的dict中包含值为`None`的键值
+    - [A] `BaseModelMixin.to_dict`方法的`option`参数添加`relationships`选项，用于自定义是否查询关联关系
+    - [A] `FLASKZ_DATABASE_SESSION_KWARGS`配置参数添加`reusable_in_flask_g`选项, 用于设置是否在`flask.g`中缓存&复用`session`对象(默认启用)
+    - [C] `flaskz.ext.ssh`返回值保留文本两侧的空格
+    - [A] `flaskz.ext.ssh.SSH`添加`pre_commands`参数, 用于在命令执行之前预先执行控制相关命令
 
+- **1.7.2** `2024/02/01`
+    - [A] `flaskz.models.parse_pss`函数支持`like_columns`参数, 用于定义模糊查询列(默认使用模型类的like_columns)
+    - [A] `flaskz.utils.api_request`函数添加`http_kwargs`参数，用于设置http请求参数
 - **1.7.1** `2024/01/05`
     - [F] 修复SQLAlchemy<2.0.0版本时, `flaskz.models._util.py`中`BinaryExpression`类的导入问题
 - **1.7.0** `2024/01/01`
     - [C] `SQLAlchemy`依赖的版本从`>=1.3.13(EOL)`升级到`>=1.4.0(Maintenance)`
     - [A] `BaseModelMixin.query_pss`方法支持`relationship`的查询和排序
     - [A] `flaskz.models.parse_pss`函数支持`relationship`的查询和排序参数解析
 - **1.6.4** `2023/12/01`
     - [A] `BaseModelMixin`添加`refresh`方法, 用于更新当前模型对象
     - [A] 添加`flaskz.models.refresh_instance`函数, 用于更新模型对象/列表
     - [A] `model_to_dict`函数的`option`参数添加`filter`选项, 用于过滤模型对象列表
     - [A] `flaskz.rest.register_model_query_pss_route`路由生成函数添加`get_pss_config`参数, 用于自定义pss查询参数
     - [A] `flaskz.ext.ssh`添加`ssh_run_command`和`ssh_run_command_list`函数
     - [A] `flaskz.ext.ssh.SSH`添加`connect_kwargs`和`channel_kwargs`参数以自定义connect和channel参数
-    - [A] `flaskz.ext.ssh.SSH`添加`timeout`参数的默认值为`10`
+    - [A] `flaskz.ext.ssh.SSH`设置`timeout`参数的默认值为`10`
 - **1.6.3** `2023/09/01`
-    - [A] 添加`FLASKZ_DATABASE_SESSION_KWARGS`参数, 用于自定义`DBSession`参数
+    - [A] 添加`FLASKZ_DATABASE_SESSION_KWARGS`配置参数, 用于自定义`DBSession`参数
     - [C] `BaseModelMixin.add_db`和`BaseModelMixin.update_db`方法添加`refresh`操作, 以返回跟数据库同步的instance对象
     - [A] `flaskz.rest.register_model_*`路由生成函数添加路由`endpoint`参数
 - **1.6.2** `2023/07/06`
     - [F] 修复`flaskz.utils._request_args.py`中`import parse_pss as get_pss`的导入问题
 - **1.6.1** `2023/07/01`
     - [C] `flaskz.utils.get_pss`(`flaskz.models.parse_pss`)函数返回项由SQL字符串拼接改为参数化模式以预防SQL注入
     - [A] 添加`flaskz.utils.run_at`函数用于执行定时函数
```

### Comparing `flaskz-1.7.2rc2/setup.cfg` & `flaskz-1.7.3rc1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = flaskz
-version = 1.7.2rc2
+version = 1.7.3rc1
 author = Zhang Tao
 author_email = taozh1982@gmail.com
 description = Flask and SQLAlchemy extensions for web applications
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/taozh1982/flaskz
 project_urls =
```

### Comparing `flaskz-1.7.2rc2/src/flaskz/auth/_jws.py` & `flaskz-1.7.3rc1/src/flaskz/auth/_jws.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.7.2rc2/src/flaskz/ext/cypher.py` & `flaskz-1.7.3rc1/src/flaskz/ext/cypher.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.7.2rc2/src/flaskz/ext/ssh.py` & `flaskz-1.7.3rc1/src/flaskz/ext/ssh.py`

 * *Files 4% similar despite different names*

```diff
@@ -165,14 +165,23 @@
         if 'timeout' in kwargs:
             self._timeout = kwargs.pop('timeout', 0)
         else:
             self._timeout = 10
 
         if hostname is None and 'host' in kwargs:
             hostname = kwargs.pop('host', None)
+
+        self._pre_commands = None  # @2024-04-14 add
+        pre_commands = kwargs.pop('pre_commands', None)
+        if type(pre_commands) is str:
+            pre_commands = [pre_commands]
+        if type(pre_commands) is list and len(pre_commands) > 0:
+            self._pre_commands = pre_commands
+            self._pre_commands_run = False
+
         # self.transport = paramiko.Transport((hostname, port))
         self.transport = paramiko.Transport(_create_socket(hostname=hostname, port=port, timeout=self._timeout))
         _connect_kwargs = kwargs.pop('connect_kwargs', None) or {}  # kwargs for Transport.connect()
         self.transport.connect(username=username, password=password, **_connect_kwargs)
         if self.transport.is_authenticated() is not True:  # @2023-12-28 add(Oops, unhandled type 3 ('unimplemented'))
             raise AuthenticationException('Authentication failed.')
 
@@ -216,19 +225,25 @@
          :param command: the command to run.
          :param recv: wait for the result or not.
          :param clean: clean output info or not, default True(clean)
          :param prompt: the prompt of the command line
 
          :return: the output of the command
         """
-        command, recv, clean = _get_command_arg(command, recv, clean)
+
+        if self._pre_commands and self._pre_commands_run is False:
+            # self._run_command('', False)
+            for pre_command in self._pre_commands:
+                self._run_command(pre_command, False)
+            self._pre_commands_run = True
 
         if prompt is None:  # prompt is False for config
             prompt = self.get_prompt()  # 1.get prompt 2.remove welcome
 
+        command, recv, clean = _get_command_arg(command, recv, clean)
         output = self._run_command(command, recv, prompt)
         if output is None:
             return None
 
         if self._is_secondary_login(command, output):
             secondary_login_output = self._secondary_login(output)
             if secondary_login_output is False:
@@ -245,16 +260,14 @@
             return output
 
         if clean is not False:
             output = _clean_output(output, command, prompt)
 
         return output
 
-        # --------------------------------------------------------------
-
     def run_command_list(self, command_list: list, last_result: bool = False, **kwargs) -> Union[list, str]:
         """
         Run a command list.
         By default, returns the list of results , if last_result==True returns the result of the last command
 
         Example:
             ssh.run_command_list(['show version', 'show running-config'])
@@ -269,15 +282,15 @@
 
          :param command_list: the command list to run.
          :param last_result: if True, return the result of the last command, otherwise, return the result list
 
          :return: command output result(list/last)
         """
         re_list = []
-        prompt = kwargs.get('kwargs', None)
+        prompt = kwargs.get('prompt', None)  # @2024-03-26 kwargs.get('kwargs', None) --> kwargs.get('prompt', None)
         if prompt is None:
             kwargs['prompt'] = self.get_prompt()  # for reuse
         count = len(command_list)
         for index, command in enumerate(command_list):
             if last_result is True:
                 if index == count - 1:  # last
                     return self.run_command(command, **kwargs)
@@ -508,15 +521,15 @@
     - Path info         ex)[root@localhost ~]...
     - Command info      ex) [root@localhost ~] ls -l
     - Return prompt     ex) [root@localhost ~]
 
     """
     # remove the start command  ex) ls -l
     if output.startswith(command):
-        output = output[len(command):].lstrip()
+        output = output[len(command):].lstrip('\r\n')  # 2024-04-05 add '\r\n' to keep space
 
     prompt_matched = False
     if type(prompt) is str:  # for show
         # 1.remove text before command ex) [root@localhost ~]# ls -l
         cmd_prompt = prompt + command
         cmd_start = output.rfind(cmd_prompt)
         if cmd_start > -1:
@@ -539,15 +552,15 @@
         path_pattern = re.compile('.*[#$]( )?$')  # @2023-07-06 change '.*[#$] ' --> '.*[#$]( )?'
         path_match = path_pattern.search(output)  # @2023-10-26 change sub()-->search(), '.*[#$]( )?'-->'.*[#$]( )?$'
         if path_match:
             path_match_start, path_match_end = path_match.span()
             output = output[:path_match_start] + '' + output[path_match_end:]
         output = output.replace(command + '\r\n', '')
 
-    return output.strip()
+    return output.strip('\r\n')  # 2024-04-05 add '\r\n' to keep space
 
 
 def _remove_end_slash(path):
     """Remove ending slash """
     if path[-1] == '/':
         return path[0:-1]
     return path
```

### Comparing `flaskz-1.7.2rc2/src/flaskz/log/__init__.py` & `flaskz-1.7.3rc1/src/flaskz/log/__init__.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.7.2rc2/src/flaskz/models/__init__.py` & `flaskz-1.7.3rc1/src/flaskz/models/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,15 +45,17 @@
         for engine_key, config_key in {'echo': 'FLASKZ_DATABASE_ECHO',
                                        'pool_recycle': 'FLASKZ_DATABASE_POOL_RECYCLE',
                                        'pool_pre_ping': 'FLASKZ_DATABASE_POOL_PRE_PING'}.items():  # @2023-02-01: add pool_pre_ping config
             if config_key in app_config:
                 engine_kwargs[engine_key] = app_config.get(config_key)
 
         engine = create_engine(database_uri, **engine_kwargs)
-        session_kwargs = app_config.get('FLASKZ_DATABASE_SESSION_KWARGS') or {}  # @2023-08-25: add FLASKZ_DATABASE_SESSION_KWARGS config
+        session_kwargs = app_config.get('FLASKZ_DATABASE_SESSION_KWARGS') or {}  # @2023-08-25: add `FLASKZ_DATABASE_SESSION_KWARGS` config
+        if session_kwargs.pop('reusable_in_flask_g', None) is False:  # @2024-02-02: add `reusable_in_flask_g` to disable cache
+            setattr(DBSession, 'reusable_in_flask_g', False)
         DBSession.configure(binds={ModelBase: engine}, **session_kwargs)  # for multiple db
 
         with engine.connect():  # connect test
             flaskz_logger.info('Database ' + database_uri + ' is ready\n')
 
         # handle disconnect error
         engine_err_info = {}
```

### Comparing `flaskz-1.7.2rc2/src/flaskz/models/_base.py` & `flaskz-1.7.3rc1/src/flaskz/models/_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -222,17 +222,24 @@
             'include': lambda ins, key: ins.__class__.to_dict_field_filter(key),
         }
         if option:
             opt.update(option)
         return ins_to_dict(self, opt)
 
     @classmethod
-    def get_to_dict_attrs(cls, ins, cascade, *args):
+    def get_to_dict_attrs(cls, ins, cascade=0, relationships=None, *args, **kwargs):
         """to_dict attr """
         fields = [cls.get_column_field(col) for col in cls.get_columns()]
+
+        # @2024-04-14 add
+        if relationships:
+            for relationship in cls.get_relationships():
+                if relationship.key in relationships:
+                    fields.append(relationship.key)
+
         if cascade > 0:
             for relationship in cls.get_relationships():
                 lazy = relationship.lazy
                 if lazy != 'dynamic' and lazy != 'noload':
                     fields.append(relationship.key)
         items = {}
         for field in fields:
@@ -862,15 +869,13 @@
         cls = self.__class__
         attrs = []
         for col in cls.get_columns():
             field = cls.get_column_field(col)
             attrs.append(field + '=' + str(getattr(self, field, None)))
         return cls.get_class_name() + '(' + (', '.join(attrs)) + ')'
 
-    # -------------------------------------------new-------------------------------------------
-
 
 # must
 from ..utils._cls import ins_to_dict
 from ..utils._common import find_list, filter_list, is_str, is_dict, is_list, get_dict_value_by_type
 from ._util import create_instance, create_relationships, db_session, append_query_filter, _db_session, _session_get, _refresh_instance, _append_pss_query_filters
 from ._query_util import get_col_op
```

### Comparing `flaskz-1.7.2rc2/src/flaskz/models/_model.py` & `flaskz-1.7.3rc1/src/flaskz/models/_model.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.7.2rc2/src/flaskz/models/_query_util.py` & `flaskz-1.7.3rc1/src/flaskz/models/_query_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -262,14 +262,15 @@
         'like': lambda col, val: col.like(val),
         'ilike': lambda col, val: col.ilike(val),
         'notlike': lambda col, val: col.notlike(val),
         'notilike': lambda col, val: col.notilike(val),
 
         '==': lambda col, val: col.__eq__(val)
     }
+    value = _get_operator_value(operator, value)  # 2024-04-07 add
     if operator in op_func_mapping:
         return op_func_mapping.get(operator)(column, value)
     return column.op(operator)(value)
 
 
 def _get_parse_options(cls, pss_payload):
     search = pss_payload.get('search') or pss_payload.get('query') or {}
@@ -347,19 +348,20 @@
 
 
 def _gen_like_columns_filters(like_columns, like_op, like_value):
     """Generate the like filters"""
     if like_value is None or type(like_value) is not str or like_value == '':
         return []
 
-    if not (like_value.startswith('%') or like_value.startswith('%')):
-        like_value = "%" + like_value + "%"
-
+    # if not (like_value.startswith('%') or like_value.startswith('%')):
+    #     like_value = "%" + like_value + "%"
+    like_value = _get_operator_value(like_op, like_value)
     filters = []
     for col in like_columns:
+        # filters.append(get_col_op(col, like_op, like_value))
         filters.append(get_col_op(col, like_op, like_value))
     return filters
 
 
 def _merge_search_filter_likes(pss_options, parse_option):
     filters = []
     filter_likes = pss_options.pop('filter_likes', [])
@@ -376,14 +378,21 @@
         if parse_option.get('notlike_join') == 'or':
             filters.append(or_(*filter_notlikes))
         else:
             filters.append(and_(*filter_notlikes))
     pss_options['filter_likes'] = filters
 
 
+def _get_operator_value(operator, value):
+    if operator in ('like', 'ilike', 'notlike', 'notilike'):
+        if not (value.startswith('%') or value.endswith('%')):
+            return "%" + value + "%"
+    return value
+
+
 # -------------------------------------------sort+group-------------------------------------------
 def _parse_groups(cls, group):
     """
     Get group by list
     """
     groups = []
     if group:
```

### Comparing `flaskz-1.7.2rc2/src/flaskz/models/_util.py` & `flaskz-1.7.3rc1/src/flaskz/models/_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,23 +106,23 @@
     :return:If failed, returns the failed tuple, otherwise, returns the the data list.
     """
 
     return query_all_models(*cls_list)
 
 
 def append_debug_queries(query):
-    if _has_g_context():  # @2022-07-26 add,
+    if _has_flask_g_context():  # @2022-07-26 add,
         debug_queries = getattr(g, 'z_debug_queries', None)
         if debug_queries is None:
             g.z_debug_queries = debug_queries = []
         debug_queries.append(query)
 
 
 def get_debug_queries():
-    if _has_g_context():  # @2022-07-26 add,
+    if _has_flask_g_context():  # @2022-07-26 add,
         return getattr(g, 'z_debug_queries', [])
     return []
 
 
 def _append_pss_query_filters(query, pss_option):
     query = append_query_filter(query, pss_option.get('filter_likes', []), 'and')
     # query = append_query_filter(query, pss_option.get('filter_notlikes', []), 'and')
@@ -185,15 +185,17 @@
     Example:
         session = get_db_session()
         session.query(User).all()
         session.close()             # close session
 
     :return:
     """
-    if _has_g_context():  # @2022-07-26 add, make sure work without flask request
+    # @2022-07-26 add `_has_g_context` condition to make sure work without flask request,
+    # @2024-02-02 add `reusable_in_flask_g` condition to disable cache
+    if getattr(DBSession, 'reusable_in_flask_g', None) is not False and _has_flask_g_context():
         session = get_g_cache('_flaskz_db_session')
         if session is None:
             session = DBSession()
             set_g_cache('_flaskz_db_session', session)
     else:
         session = DBSession()
         setattr(session, '_temporary', True)  # @2022-08-22 add '_temporary' attr
@@ -202,15 +204,15 @@
 
 def close_db_session():
     """
     Close the cached session.
 
     :return:
     """
-    if _has_g_context():  # @2022-07-26 add
+    if _has_flask_g_context():  # @2022-07-26 add
         session = get_g_cache('_flaskz_db_session')
         if session is not None:
             remove_g_cache('_flaskz_db_session')
             session.close()
 
 
 def _close_temporary_session(session):
@@ -345,15 +347,15 @@
 
     :param obj:
     :return:
     """
     return isinstance(obj, BaseModelMixin)
 
 
-def _has_g_context():
+def _has_flask_g_context():
     # if has_request_context():  # If there is request context, g must exist
     #     return True
     if not g:  # @2022-11-28: change, (not g) != (g is None)
         return False
     return True
     # return has_request_context() or g is not None
```

### Comparing `flaskz-1.7.2rc2/src/flaskz/res_status_codes.py` & `flaskz-1.7.3rc1/src/flaskz/res_status_codes.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.7.2rc2/src/flaskz/rest/__init__.py` & `flaskz-1.7.3rc1/src/flaskz/rest/__init__.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.7.2rc2/src/flaskz/rest/_mgmt.py` & `flaskz-1.7.3rc1/src/flaskz/rest/_mgmt.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.7.2rc2/src/flaskz/rest/_util.py` & `flaskz-1.7.3rc1/src/flaskz/rest/_util.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.7.2rc2/src/flaskz/utils/_app.py` & `flaskz-1.7.3rc1/src/flaskz/utils/_app.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.7.2rc2/src/flaskz/utils/_cache.py` & `flaskz-1.7.3rc1/src/flaskz/utils/_cache.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.7.2rc2/src/flaskz/utils/_cls.py` & `flaskz-1.7.3rc1/src/flaskz/utils/_cls.py`

 * *Files 3% similar despite different names*

```diff
@@ -131,22 +131,26 @@
     if 'cascade' in item_option:
         item_cascade = item_option.get('cascade', 0)
     else:
         item_cascade = _get_option_key(option, path_keys, 'cascade')  # print('查找父option的cascade，直到找到根option')
         if type(item_cascade) == int:
             item_cascade -= len(path_keys)
 
-    if type(item_cascade) != int:
+    if type(item_cascade) is not int:
         item_cascade = 0
 
+    item_relationships = item_option.get('relationships', None)  # @2024-04-14 add
+    if type(item_relationships) is not list:
+        item_relationships = []
+
     item_recursion_value = _get_option_key(option, path_keys, 'recursion_value')
 
     item_getattrs = _get_option_key(option, path_keys, 'getattrs')
     if item_getattrs:
-        attrs = item_getattrs(ins, item_cascade, option, path_keys)
+        attrs = item_getattrs(ins, item_cascade, item_relationships, option, path_keys)
     else:
         attrs = ins.__dict__
 
     # with_none_value = item_option.get('with_none_value', False)
     attr_filter = _get_option_filter(item_option)
     result = {}
     for key, value in attrs.items():
@@ -174,16 +178,16 @@
                 if value not in path_items:
                     _value = _ins_to_dict(value, option, path_items, path_keys + [key])
                 elif item_recursion_value is not None:
                     _value = item_recursion_value
         else:
             _value = value
 
-        if _value is not None:
-            result[key] = _value
+        # if _value is not None:  # @2024-03-06 remove
+        result[key] = _value
         # elif with_none_value:
         #     result[key] = None
     return result
 
 
 def _get_option_key(option, key_list, key):
     """
```

### Comparing `flaskz-1.7.2rc2/src/flaskz/utils/_common.py` & `flaskz-1.7.3rc1/src/flaskz/utils/_common.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.7.2rc2/src/flaskz/utils/_func.py` & `flaskz-1.7.3rc1/src/flaskz/utils/_func.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.7.2rc2/src/flaskz/utils/_magic.py` & `flaskz-1.7.3rc1/src/flaskz/utils/_magic.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.7.2rc2/src/flaskz/utils/_private.py` & `flaskz-1.7.3rc1/src/flaskz/utils/_private.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.7.2rc2/src/flaskz/utils/_request_api.py` & `flaskz-1.7.3rc1/src/flaskz/utils/_request_api.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,27 +20,31 @@
     Request an api.
 
    .. versionupdated::
         1.7.2 - add `http_kwargs` param to set http request parameters(HTTPAdapter)
 
     Example
         # post request
-        api_request('http://flaskz_server/sys-mgmt/auth/token/', 'POST', json={'username': 'admin','password': 'admin'})
+        api_request('req_url', 'POST', json=payload)
+        api_request({'url': 'req_url', 'method': 'POST'}, json=payload)
 
         # get request
-        api_request('http://flaskz_server/sys-mgmt/auth/account/', headers={'Authorization': 'eyJhbGciOiJIUzUxMiIs......'})
+        api_request('req_url', headers={'Authorization': 'eyJhbGciOiJIUzUxMiIs......'})
+
+        # base url
+        api_request('req_url', base_url='base_url') # url --> 'base_url/req_url'
 
         # url_variables
-        api_request('http://flaskz_server/api/v1.0/ex-employees/{id}/', url_variables={'id': 1}) # url --> 'http://flaskz_server/api/v1.0/ex-employees/1/'
+        api_request('req_url/{id}/', url_variables={'id': 1}) # url --> 'req_url/1/'
 
         # url_search_params
-        api_request('http://flaskz_server/api/v1.0/ex-employees/', url_search_params={'id': 1}) # url --> 'http://flaskz_server/api/v1.0/ex-employees/?id=1'
+        api_request('req_url', url_search_params={'id': 1}) # url --> 'req_url?id=1'
 
         # http_kwargs
-        print(api_request('http://flaskz_server/api/v1.0/ex-employees/', http_kwargs={ # --> HTTPAdapter parameters
+        api_request('req_url', http_kwargs={ # --> HTTPAdapter parameters
             'pool_connections': 10, 'pool_maxsize': 100, 'max_retries': 10
         })
 
     :param url:
     :param method:
     :param url_params:
     :param raw_response:
```

### Comparing `flaskz-1.7.2rc2/src/flaskz/utils/_request_args.py` & `flaskz-1.7.3rc1/src/flaskz/utils/_request_args.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.7.2rc2/src/flaskz/utils/_response.py` & `flaskz-1.7.3rc1/src/flaskz/utils/_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,22 @@
 __all__ = ['create_response', 'get_status_msg', 'ResponseManager']
 
 
 def create_response(success, data, data_wrapped=False):
     """
     Create the response json result.
 
+    Example:
+        @api_bp.route('/users/add/', methods=['POST'])
+        def add():
+            request_json = request.json
+            success, data = User.add(request_json)
+            res_data = model_to_dict(data)
+            return create_response(success, res_data) # return response result
+
     :param success:
     :param data:
     :param data_wrapped:
     :return:
     """
     if success is True:
         return _create_success_response(data, data_wrapped)
@@ -58,15 +66,15 @@
         'message': str(msg),
     }
 
 
 def get_status_msg(status_code):
     """
     Get the specified message by status_code.
-    Can be used to return internationalized text, Local can be fixed, or get the local from request.
+    Can be used to return internationalized text, Locale can be fixed, or get the locale from request.
 
     :param status_code:
     :return:
     """
     response_callback = get_current_response_manager('get_response_callback')
     if response_callback:
         return response_callback(status_code)
```

### Comparing `flaskz-1.7.2rc2/src/flaskz/utils/_timer.py` & `flaskz-1.7.3rc1/src/flaskz/utils/_timer.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.7.2rc2/src/flaskz.egg-info/PKG-INFO` & `flaskz-1.7.3rc1/src/flaskz.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flaskz
-Version: 1.7.2rc2
+Version: 1.7.3rc1
 Summary: Flask and SQLAlchemy extensions for web applications
 Home-page: https://github.com/taozh1982/flaskz
 Author: Zhang Tao
 Author-email: taozh1982@gmail.com
 Project-URL: Bug Tracker, https://github.com/taozh1982/flaskz/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -30,35 +30,40 @@
 3. [☞API封装、访问权限控制和系统日志](http://zhangyiheng.com/blog/articles/py_flaskz_api.html)
 4. [☞常用函数](http://zhangyiheng.com/blog/articles/py_flaskz_utils.html)
 5. [☞基于Flaskz的管理系统开发模板 Flaskz-admin](http://zhangyiheng.com/blog/articles/py_flaskz_admin.html)
 6. [☞使用手册](http://zhangyiheng.com/blog/articles/py_flaskz_manual.html)
 
 ## 版本
 
-- **1.7.2rc2** `2024/01/26`
-    - [A] `flaskz.utils.api_request`函数添加`http_kwargs`参数，用于设置http请求参数
-- **1.7.2rc1** `2024/01/22`
-    - [A] `flaskz.models.parse_pss`函数支持`like_columns`参数, 用于定义模糊查询列(默认使用模型类的like_columns)
+- **1.7.3rc1** `2024/04/16`
+    - [C] `flaskz.utils.ins_to_dict`函数返回的dict中包含值为`None`的键值
+    - [A] `BaseModelMixin.to_dict`方法的`option`参数添加`relationships`选项，用于自定义是否查询关联关系
+    - [A] `FLASKZ_DATABASE_SESSION_KWARGS`配置参数添加`reusable_in_flask_g`选项, 用于设置是否在`flask.g`中缓存&复用`session`对象(默认启用)
+    - [C] `flaskz.ext.ssh`返回值保留文本两侧的空格
+    - [A] `flaskz.ext.ssh.SSH`添加`pre_commands`参数, 用于在命令执行之前预先执行控制相关命令
 
+- **1.7.2** `2024/02/01`
+    - [A] `flaskz.models.parse_pss`函数支持`like_columns`参数, 用于定义模糊查询列(默认使用模型类的like_columns)
+    - [A] `flaskz.utils.api_request`函数添加`http_kwargs`参数，用于设置http请求参数
 - **1.7.1** `2024/01/05`
     - [F] 修复SQLAlchemy<2.0.0版本时, `flaskz.models._util.py`中`BinaryExpression`类的导入问题
 - **1.7.0** `2024/01/01`
     - [C] `SQLAlchemy`依赖的版本从`>=1.3.13(EOL)`升级到`>=1.4.0(Maintenance)`
     - [A] `BaseModelMixin.query_pss`方法支持`relationship`的查询和排序
     - [A] `flaskz.models.parse_pss`函数支持`relationship`的查询和排序参数解析
 - **1.6.4** `2023/12/01`
     - [A] `BaseModelMixin`添加`refresh`方法, 用于更新当前模型对象
     - [A] 添加`flaskz.models.refresh_instance`函数, 用于更新模型对象/列表
     - [A] `model_to_dict`函数的`option`参数添加`filter`选项, 用于过滤模型对象列表
     - [A] `flaskz.rest.register_model_query_pss_route`路由生成函数添加`get_pss_config`参数, 用于自定义pss查询参数
     - [A] `flaskz.ext.ssh`添加`ssh_run_command`和`ssh_run_command_list`函数
     - [A] `flaskz.ext.ssh.SSH`添加`connect_kwargs`和`channel_kwargs`参数以自定义connect和channel参数
-    - [A] `flaskz.ext.ssh.SSH`添加`timeout`参数的默认值为`10`
+    - [A] `flaskz.ext.ssh.SSH`设置`timeout`参数的默认值为`10`
 - **1.6.3** `2023/09/01`
-    - [A] 添加`FLASKZ_DATABASE_SESSION_KWARGS`参数, 用于自定义`DBSession`参数
+    - [A] 添加`FLASKZ_DATABASE_SESSION_KWARGS`配置参数, 用于自定义`DBSession`参数
     - [C] `BaseModelMixin.add_db`和`BaseModelMixin.update_db`方法添加`refresh`操作, 以返回跟数据库同步的instance对象
     - [A] `flaskz.rest.register_model_*`路由生成函数添加路由`endpoint`参数
 - **1.6.2** `2023/07/06`
     - [F] 修复`flaskz.utils._request_args.py`中`import parse_pss as get_pss`的导入问题
 - **1.6.1** `2023/07/01`
     - [C] `flaskz.utils.get_pss`(`flaskz.models.parse_pss`)函数返回项由SQL字符串拼接改为参数化模式以预防SQL注入
     - [A] 添加`flaskz.utils.run_at`函数用于执行定时函数
```

### Comparing `flaskz-1.7.2rc2/src/flaskz.egg-info/SOURCES.txt` & `flaskz-1.7.3rc1/src/flaskz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

