# Comparing `tmp/astro_extras-0.0.8.tar.gz` & `tmp/astro_extras-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astro_extras-0.0.8.tar", last modified: Mon Apr  8 07:18:12 2024, max compression
+gzip compressed data, was "astro_extras-0.0.9.tar", last modified: Mon Apr 15 17:00:57 2024, max compression
```

## Comparing `astro_extras-0.0.8.tar` & `astro_extras-0.0.9.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-04-08 07:18:12.487523 astro_extras-0.0.8/
--rw-rw-r--   0 kol       (1000) kol       (1000)     1074 2023-11-17 10:43:31.000000 astro_extras-0.0.8/LICENSE
--rw-rw-r--   0 kol       (1000) kol       (1000)       24 2023-10-26 14:10:20.000000 astro_extras-0.0.8/MANIFEST.in
--rw-r--r--   0 kol       (1000) kol       (1000)     7878 2024-04-08 07:18:12.487523 astro_extras-0.0.8/PKG-INFO
--rw-rw-r--   0 kol       (1000) kol       (1000)     7444 2023-11-20 09:59:52.000000 astro_extras-0.0.8/README.md
--rw-rw-r--   0 kol       (1000) kol       (1000)      352 2023-10-26 14:10:20.000000 astro_extras-0.0.8/pyproject.toml
--rw-rw-r--   0 kol       (1000) kol       (1000)      260 2024-03-11 13:15:33.000000 astro_extras-0.0.8/requirements.txt
--rw-rw-r--   0 kol       (1000) kol       (1000)       38 2024-04-08 07:18:12.487523 astro_extras-0.0.8/setup.cfg
--rw-rw-r--   0 kol       (1000) kol       (1000)     1109 2024-04-06 11:02:14.000000 astro_extras-0.0.8/setup.py
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-04-08 07:18:12.467523 astro_extras-0.0.8/src/
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-04-08 07:18:12.471523 astro_extras-0.0.8/src/astro_extras/
--rw-rw-r--   0 kol       (1000) kol       (1000)      963 2024-04-06 11:01:44.000000 astro_extras-0.0.8/src/astro_extras/__init__.py
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-04-08 07:18:12.483523 astro_extras-0.0.8/src/astro_extras/hooks/
--rw-rw-r--   0 kol       (1000) kol       (1000)       45 2023-10-26 14:10:20.000000 astro_extras-0.0.8/src/astro_extras/hooks/__init__.py
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-04-08 07:18:12.483523 astro_extras-0.0.8/src/astro_extras/operators/
--rw-rw-r--   0 kol       (1000) kol       (1000)       45 2023-10-26 14:10:20.000000 astro_extras-0.0.8/src/astro_extras/operators/__init__.py
--rw-rw-r--   0 kol       (1000) kol       (1000)     3861 2024-04-06 11:05:12.000000 astro_extras-0.0.8/src/astro_extras/operators/direct.py
--rw-rw-r--   0 kol       (1000) kol       (1000)    18057 2023-11-20 09:48:16.000000 astro_extras-0.0.8/src/astro_extras/operators/session.py
--rw-rw-r--   0 kol       (1000) kol       (1000)    24723 2024-04-06 11:01:05.000000 astro_extras-0.0.8/src/astro_extras/operators/table.py
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-04-08 07:18:12.483523 astro_extras-0.0.8/src/astro_extras/sensors/
--rw-rw-r--   0 kol       (1000) kol       (1000)       45 2024-04-02 07:09:42.000000 astro_extras-0.0.8/src/astro_extras/sensors/__init__.py
--rw-rw-r--   0 kol       (1000) kol       (1000)     5536 2024-04-06 11:03:48.000000 astro_extras-0.0.8/src/astro_extras/sensors/file.py
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-04-08 07:18:12.487523 astro_extras-0.0.8/src/astro_extras/utils/
--rw-rw-r--   0 kol       (1000) kol       (1000)       45 2023-10-26 14:10:20.000000 astro_extras-0.0.8/src/astro_extras/utils/__init__.py
--rw-rw-r--   0 kol       (1000) kol       (1000)    10650 2024-04-06 10:39:43.000000 astro_extras-0.0.8/src/astro_extras/utils/data_compare.py
--rw-rw-r--   0 kol       (1000) kol       (1000)     1675 2024-03-11 13:15:59.000000 astro_extras-0.0.8/src/astro_extras/utils/datetime_local.py
--rw-rw-r--   0 kol       (1000) kol       (1000)     5378 2024-03-11 14:28:15.000000 astro_extras-0.0.8/src/astro_extras/utils/template.py
--rw-rw-r--   0 kol       (1000) kol       (1000)     2029 2024-04-06 10:45:20.000000 astro_extras-0.0.8/src/astro_extras/utils/utils.py
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-04-08 07:18:12.487523 astro_extras-0.0.8/src/astro_extras.egg-info/
--rw-r--r--   0 kol       (1000) kol       (1000)     7878 2024-04-08 07:18:12.000000 astro_extras-0.0.8/src/astro_extras.egg-info/PKG-INFO
--rw-rw-r--   0 kol       (1000) kol       (1000)      821 2024-04-08 07:18:12.000000 astro_extras-0.0.8/src/astro_extras.egg-info/SOURCES.txt
--rw-rw-r--   0 kol       (1000) kol       (1000)        1 2024-04-08 07:18:12.000000 astro_extras-0.0.8/src/astro_extras.egg-info/dependency_links.txt
--rw-rw-r--   0 kol       (1000) kol       (1000)      112 2024-04-08 07:18:12.000000 astro_extras-0.0.8/src/astro_extras.egg-info/requires.txt
--rw-rw-r--   0 kol       (1000) kol       (1000)       13 2024-04-08 07:18:12.000000 astro_extras-0.0.8/src/astro_extras.egg-info/top_level.txt
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-04-08 07:18:12.487523 astro_extras-0.0.8/tests/
--rw-rw-r--   0 kol       (1000) kol       (1000)     4172 2023-11-17 09:41:29.000000 astro_extras-0.0.8/tests/test_session.py
--rw-rw-r--   0 kol       (1000) kol       (1000)     6158 2023-11-17 10:36:18.000000 astro_extras-0.0.8/tests/test_table.py
--rw-rw-r--   0 kol       (1000) kol       (1000)     1295 2023-11-17 09:42:18.000000 astro_extras-0.0.8/tests/test_templates.py
--rw-rw-r--   0 kol       (1000) kol       (1000)     5772 2024-03-11 14:20:58.000000 astro_extras-0.0.8/tests/test_utils.py
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-04-15 17:00:57.045239 astro_extras-0.0.9/
+-rw-rw-r--   0 kol       (1000) kol       (1000)     1074 2023-11-17 10:43:31.000000 astro_extras-0.0.9/LICENSE
+-rw-rw-r--   0 kol       (1000) kol       (1000)       24 2023-10-26 14:10:20.000000 astro_extras-0.0.9/MANIFEST.in
+-rw-r--r--   0 kol       (1000) kol       (1000)     7878 2024-04-15 17:00:57.045239 astro_extras-0.0.9/PKG-INFO
+-rw-rw-r--   0 kol       (1000) kol       (1000)     7444 2023-11-20 09:59:52.000000 astro_extras-0.0.9/README.md
+-rw-rw-r--   0 kol       (1000) kol       (1000)      352 2023-10-26 14:10:20.000000 astro_extras-0.0.9/pyproject.toml
+-rw-rw-r--   0 kol       (1000) kol       (1000)      260 2024-03-11 13:15:33.000000 astro_extras-0.0.9/requirements.txt
+-rw-rw-r--   0 kol       (1000) kol       (1000)       38 2024-04-15 17:00:57.045239 astro_extras-0.0.9/setup.cfg
+-rw-rw-r--   0 kol       (1000) kol       (1000)     1114 2024-04-15 17:00:54.000000 astro_extras-0.0.9/setup.py
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-04-15 17:00:57.005240 astro_extras-0.0.9/src/
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-04-15 17:00:57.013239 astro_extras-0.0.9/src/astro_extras/
+-rw-rw-r--   0 kol       (1000) kol       (1000)      963 2024-04-15 16:59:07.000000 astro_extras-0.0.9/src/astro_extras/__init__.py
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-04-15 17:00:57.029239 astro_extras-0.0.9/src/astro_extras/hooks/
+-rw-rw-r--   0 kol       (1000) kol       (1000)       45 2023-10-26 14:10:20.000000 astro_extras-0.0.9/src/astro_extras/hooks/__init__.py
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-04-15 17:00:57.033239 astro_extras-0.0.9/src/astro_extras/operators/
+-rw-rw-r--   0 kol       (1000) kol       (1000)       45 2023-10-26 14:10:20.000000 astro_extras-0.0.9/src/astro_extras/operators/__init__.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)     3861 2024-04-06 11:05:12.000000 astro_extras-0.0.9/src/astro_extras/operators/direct.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)    18308 2024-04-15 16:59:36.000000 astro_extras-0.0.9/src/astro_extras/operators/session.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)    24781 2024-04-15 15:17:52.000000 astro_extras-0.0.9/src/astro_extras/operators/table.py
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-04-15 17:00:57.037239 astro_extras-0.0.9/src/astro_extras/sensors/
+-rw-rw-r--   0 kol       (1000) kol       (1000)       45 2024-04-02 07:09:42.000000 astro_extras-0.0.9/src/astro_extras/sensors/__init__.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)     5536 2024-04-06 11:03:48.000000 astro_extras-0.0.9/src/astro_extras/sensors/file.py
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-04-15 17:00:57.037239 astro_extras-0.0.9/src/astro_extras/utils/
+-rw-rw-r--   0 kol       (1000) kol       (1000)       45 2023-10-26 14:10:20.000000 astro_extras-0.0.9/src/astro_extras/utils/__init__.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)    10650 2024-04-06 10:39:43.000000 astro_extras-0.0.9/src/astro_extras/utils/data_compare.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)     1675 2024-03-11 13:15:59.000000 astro_extras-0.0.9/src/astro_extras/utils/datetime_local.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)     5378 2024-03-11 14:28:15.000000 astro_extras-0.0.9/src/astro_extras/utils/template.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)     2199 2024-04-15 14:31:16.000000 astro_extras-0.0.9/src/astro_extras/utils/utils.py
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-04-15 17:00:57.045239 astro_extras-0.0.9/src/astro_extras.egg-info/
+-rw-r--r--   0 kol       (1000) kol       (1000)     7878 2024-04-15 17:00:56.000000 astro_extras-0.0.9/src/astro_extras.egg-info/PKG-INFO
+-rw-rw-r--   0 kol       (1000) kol       (1000)      821 2024-04-15 17:00:57.000000 astro_extras-0.0.9/src/astro_extras.egg-info/SOURCES.txt
+-rw-rw-r--   0 kol       (1000) kol       (1000)        1 2024-04-15 17:00:56.000000 astro_extras-0.0.9/src/astro_extras.egg-info/dependency_links.txt
+-rw-rw-r--   0 kol       (1000) kol       (1000)      112 2024-04-15 17:00:56.000000 astro_extras-0.0.9/src/astro_extras.egg-info/requires.txt
+-rw-rw-r--   0 kol       (1000) kol       (1000)       13 2024-04-15 17:00:56.000000 astro_extras-0.0.9/src/astro_extras.egg-info/top_level.txt
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-04-15 17:00:57.045239 astro_extras-0.0.9/tests/
+-rw-rw-r--   0 kol       (1000) kol       (1000)     4172 2023-11-17 09:41:29.000000 astro_extras-0.0.9/tests/test_session.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)     6158 2023-11-17 10:36:18.000000 astro_extras-0.0.9/tests/test_table.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)     1295 2023-11-17 09:42:18.000000 astro_extras-0.0.9/tests/test_templates.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)     5772 2024-03-11 14:20:58.000000 astro_extras-0.0.9/tests/test_utils.py
```

### Comparing `astro_extras-0.0.8/LICENSE` & `astro_extras-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `astro_extras-0.0.8/PKG-INFO` & `astro_extras-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro_extras
-Version: 0.0.8
+Version: 0.0.9
 Summary: Additional Astro SDK operators
 Home-page: https://github.com/skolchin/astro-extras
 Author: Kol
 Author-email: skolchin@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Apache Airflow
```

### Comparing `astro_extras-0.0.8/README.md` & `astro_extras-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `astro_extras-0.0.8/setup.py` & `astro_extras-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # Astro SDK Extras project
-# (c) kol, 2023
+# (c) kol, 2023-2024
 """
 Setup routine for astro_extras package
 """
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 with open("requirements.txt", "r", encoding="utf-8") as fh:
     requirements = fh.readlines()
 
 setuptools.setup(
     name="astro_extras",
-    version="0.0.8",
+    version="0.0.9",
     author="Kol",
     author_email="skolchin@gmail.com",
     description="Additional Astro SDK operators",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/skolchin/astro-extras",
     classifiers=[
```

### Comparing `astro_extras-0.0.8/src/astro_extras/__init__.py` & `astro_extras-0.0.9/src/astro_extras/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Astro SDK Extras project
 # (c) kol, 2023-2024
 
-__version__ = '0.0.8'
+__version__ = '0.0.9'
 
 from .operators.session import (
     open_session, 
     close_session,
     ETLSession,
     get_current_session,
     get_session_period,
```

### Comparing `astro_extras-0.0.8/src/astro_extras/operators/direct.py` & `astro_extras-0.0.9/src/astro_extras/operators/direct.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.0.8/src/astro_extras/operators/session.py` & `astro_extras-0.0.9/src/astro_extras/operators/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,15 +99,20 @@
         return self._actual_sesssion
 
     def __exit__(self, type, value, traceback):
         dag = cast(DAG, DagContext.get_current_dag())
         if len(dag.tasks) > 1:
             t1, t2 = dag.tasks[0], dag.tasks[1]
             if t1.task_id == 'open-session' and 'open-session' not in t2.upstream_task_ids:
-                t2.set_upstream(t1)
+                if not t2.task_group:
+                    # stand-alone operator
+                    t2.set_upstream(t1)
+                else:
+                    t2.task_group.set_upstream(t1)
+
         close_session(self._actual_sesssion).set_downstream(aql.cleanup())
 
 class OpenSessionOperator(BaseOperator):
     """ Session opening operator. Normally is used within `open_session` function """
 
     def __init__(self,
                  *,
@@ -293,15 +298,15 @@
         source_conn_id=source_conn_id,
         destination_conn_id=destination_conn_id,
         session_conn_id=session_conn_id,
         **kwargs))
 
 def close_session(
         session: Union[ETLSession, XComArg], 
-        upstream_task: Optional[Any] = None,
+        upstream: Optional[Any] = None,
         dag: Optional[DAG] = None,
         **kwargs) -> XComArg:
     """ Closes the ETL session.
 
     Updates `public.sessions` table for currently running session
     saving completion time and state. If all tasks in a DAG run were successfull,
     session's state will be set to `success`, otherwise - to `error`. Note that 
@@ -323,21 +328,23 @@
         An `XComArg` object indicating the session was closed
 
     Examples:
         See `open_session` for examples
     """
     
     assert (dag := dag or DagContext.get_current_dag())
-    if upstream_task is None:
+    if not upstream:
         if not len(dag.tasks):
             raise ValueError('close_session must not be the first DAG operator')
-        upstream_task = dag.tasks[-1]
+        upstream = dag.tasks[-1]
+        if upstream.task_group and not upstream.task_group.is_root:
+            upstream = upstream.task_group
 
     op = CloseSessionOperator(dag=dag, session=session, **kwargs)
-    upstream_task.set_downstream(op)
+    op.set_upstream(upstream)
     return XComArg(op)
 
 def get_current_session(context: Optional[Context] = None) -> ETLSession:
     """ Retrieves current session from XCom.
     
     Args:
         context:    DAG execution context (optional)
```

### Comparing `astro_extras-0.0.8/src/astro_extras/operators/table.py` & `astro_extras-0.0.9/src/astro_extras/operators/table.py`

 * *Files 0% similar despite different names*

```diff
@@ -472,29 +472,35 @@
 
     if target_tables and len(target_tables) != len(source_tables):
         raise AirflowFailException(f'Source and target tables list size must be equal')
 
     target_tables = target_tables or source_tables
     op_cls = TableTransfer if not changes_only else ChangedTableTransfer
 
-    with TaskGroup(group_id or 'transfer-tables', add_suffix_on_collision=True) as tg:
+    with TaskGroup(
+        group_id or 'transfer-tables', 
+        add_suffix_on_collision=True,
+        prefix_group_id=False) as tg:
+
         ops_list = []
         for (source, target) in zip(source_tables, target_tables):
             source_table = ensure_table(source, source_conn_id)
             dest_table = ensure_table(target, destination_conn_id) or source_table
             op = op_cls(
                 source_table=source_table,
                 destination_table=dest_table,
                 session=session,
                 **kwargs_with_datasets(
                     kwargs=kwargs, 
                     input_datasets=source_table, 
                     output_datasets=dest_table))
             ops_list.append(op)
+
         schedule_ops(ops_list, num_parallel)
+
     return tg
 
 def compare_tables(
         source_tables: List[str | Table],
         target_tables: List[str | Table] | None = None,
         source_conn_id: str | None = None,
         destination_conn_id: str | None = None,
```

### Comparing `astro_extras-0.0.8/src/astro_extras/sensors/file.py` & `astro_extras-0.0.9/src/astro_extras/sensors/file.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.0.8/src/astro_extras/utils/data_compare.py` & `astro_extras-0.0.9/src/astro_extras/utils/data_compare.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.0.8/src/astro_extras/utils/datetime_local.py` & `astro_extras-0.0.9/src/astro_extras/utils/datetime_local.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.0.8/src/astro_extras/utils/template.py` & `astro_extras-0.0.9/src/astro_extras/utils/template.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.0.8/src/astro_extras.egg-info/PKG-INFO` & `astro_extras-0.0.9/src/astro_extras.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro_extras
-Version: 0.0.8
+Version: 0.0.9
 Summary: Additional Astro SDK operators
 Home-page: https://github.com/skolchin/astro-extras
 Author: Kol
 Author-email: skolchin@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Apache Airflow
```

### Comparing `astro_extras-0.0.8/src/astro_extras.egg-info/SOURCES.txt` & `astro_extras-0.0.9/src/astro_extras.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `astro_extras-0.0.8/tests/test_session.py` & `astro_extras-0.0.9/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.0.8/tests/test_table.py` & `astro_extras-0.0.9/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.0.8/tests/test_templates.py` & `astro_extras-0.0.9/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.0.8/tests/test_utils.py` & `astro_extras-0.0.9/tests/test_utils.py`

 * *Files identical despite different names*

