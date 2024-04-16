# Comparing `tmp/fab-react-toolkit-0.4.1.tar.gz` & `tmp/fab_react_toolkit-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fab-react-toolkit-0.4.1.tar", last modified: Fri Apr 12 13:39:00 2024, max compression
+gzip compressed data, was "fab_react_toolkit-0.4.2.tar", last modified: Tue Apr 16 14:46:44 2024, max compression
```

## Comparing `fab-react-toolkit-0.4.1.tar` & `fab_react_toolkit-0.4.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:39:00.427953 fab-react-toolkit-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-12 13:38:50.000000 fab-react-toolkit-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-12 13:39:00.423953 fab-react-toolkit-0.4.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:39:00.419953 fab-react-toolkit-0.4.1/example/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:39:00.419953 fab-react-toolkit-0.4.1/example/app/
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-12 13:38:50.000000 fab-react-toolkit-0.4.1/example/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-04-12 13:38:50.000000 fab-react-toolkit-0.4.1/example/app/apis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-04-12 13:38:50.000000 fab-react-toolkit-0.4.1/example/app/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-12 13:38:50.000000 fab-react-toolkit-0.4.1/example/app/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-12 13:38:50.000000 fab-react-toolkit-0.4.1/example/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-12 13:38:50.000000 fab-react-toolkit-0.4.1/example/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-12 13:38:50.000000 fab-react-toolkit-0.4.1/example/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:39:00.423953 fab-react-toolkit-0.4.1/fab_react_toolkit/
--rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-04-12 13:38:50.000000 fab-react-toolkit-0.4.1/fab_react_toolkit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:39:00.423953 fab-react-toolkit-0.4.1/fab_react_toolkit/api/
--rw-r--r--   0 runner    (1001) docker     (127)    21804 2024-04-12 13:38:50.000000 fab-react-toolkit-0.4.1/fab_react_toolkit/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10043 2024-04-12 13:38:50.000000 fab-react-toolkit-0.4.1/fab_react_toolkit/api/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-12 13:38:50.000000 fab-react-toolkit-0.4.1/fab_react_toolkit/api/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-12 13:38:50.000000 fab-react-toolkit-0.4.1/fab_react_toolkit/api/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    29186 2024-04-12 13:38:50.000000 fab-react-toolkit-0.4.1/fab_react_toolkit/apis.py
--rw-r--r--   0 runner    (1001) docker     (127)    12522 2024-04-12 13:38:50.000000 fab-react-toolkit-0.4.1/fab_react_toolkit/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-12 13:38:50.000000 fab-react-toolkit-0.4.1/fab_react_toolkit/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-12 13:38:50.000000 fab-react-toolkit-0.4.1/fab_react_toolkit/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:39:00.423953 fab-react-toolkit-0.4.1/fab_react_toolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-12 13:39:00.000000 fab-react-toolkit-0.4.1/fab_react_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-12 13:39:00.000000 fab-react-toolkit-0.4.1/fab_react_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 13:39:00.000000 fab-react-toolkit-0.4.1/fab_react_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-12 13:39:00.000000 fab-react-toolkit-0.4.1/fab_react_toolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-12 13:39:00.000000 fab-react-toolkit-0.4.1/fab_react_toolkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-12 13:38:50.000000 fab-react-toolkit-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-12 13:38:50.000000 fab-react-toolkit-0.4.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 13:39:00.427953 fab-react-toolkit-0.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:46:44.778872 fab_react_toolkit-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-16 14:46:36.000000 fab_react_toolkit-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-16 14:46:44.774872 fab_react_toolkit-0.4.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:46:44.774872 fab_react_toolkit-0.4.2/example/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:46:44.774872 fab_react_toolkit-0.4.2/example/app/
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-16 14:46:36.000000 fab_react_toolkit-0.4.2/example/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-04-16 14:46:36.000000 fab_react_toolkit-0.4.2/example/app/apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-04-16 14:46:36.000000 fab_react_toolkit-0.4.2/example/app/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-16 14:46:36.000000 fab_react_toolkit-0.4.2/example/app/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-16 14:46:36.000000 fab_react_toolkit-0.4.2/example/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-16 14:46:36.000000 fab_react_toolkit-0.4.2/example/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-16 14:46:36.000000 fab_react_toolkit-0.4.2/example/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:46:44.774872 fab_react_toolkit-0.4.2/fab_react_toolkit/
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-04-16 14:46:36.000000 fab_react_toolkit-0.4.2/fab_react_toolkit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:46:44.774872 fab_react_toolkit-0.4.2/fab_react_toolkit/api/
+-rw-r--r--   0 runner    (1001) docker     (127)    21803 2024-04-16 14:46:36.000000 fab_react_toolkit-0.4.2/fab_react_toolkit/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10043 2024-04-16 14:46:36.000000 fab_react_toolkit-0.4.2/fab_react_toolkit/api/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-16 14:46:36.000000 fab_react_toolkit-0.4.2/fab_react_toolkit/api/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-16 14:46:36.000000 fab_react_toolkit-0.4.2/fab_react_toolkit/api/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29186 2024-04-16 14:46:36.000000 fab_react_toolkit-0.4.2/fab_react_toolkit/apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12522 2024-04-16 14:46:36.000000 fab_react_toolkit-0.4.2/fab_react_toolkit/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-16 14:46:36.000000 fab_react_toolkit-0.4.2/fab_react_toolkit/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-16 14:46:36.000000 fab_react_toolkit-0.4.2/fab_react_toolkit/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:46:44.774872 fab_react_toolkit-0.4.2/fab_react_toolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-16 14:46:44.000000 fab_react_toolkit-0.4.2/fab_react_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-16 14:46:44.000000 fab_react_toolkit-0.4.2/fab_react_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 14:46:44.000000 fab_react_toolkit-0.4.2/fab_react_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-16 14:46:44.000000 fab_react_toolkit-0.4.2/fab_react_toolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-16 14:46:44.000000 fab_react_toolkit-0.4.2/fab_react_toolkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-16 14:46:36.000000 fab_react_toolkit-0.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-16 14:46:36.000000 fab_react_toolkit-0.4.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 14:46:44.778872 fab_react_toolkit-0.4.2/setup.cfg
```

### Comparing `fab-react-toolkit-0.4.1/LICENSE` & `fab_react_toolkit-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fab-react-toolkit-0.4.1/PKG-INFO` & `fab_react_toolkit-0.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fab-react-toolkit
-Version: 0.4.1
+Version: 0.4.2
 Summary: A small example package
 Author-email: Matthias Leinweber <m.leinweber@datatactics.de>
 Project-URL: Homepage, https://github.com/dttctcs/fab-react-toolkit
 Project-URL: Issues, https://github.com/dttctcs/fab-react-toolkit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fab-react-toolkit-0.4.1/example/app/__init__.py` & `fab_react_toolkit-0.4.2/example/app/__init__.py`

 * *Files identical despite different names*

### Comparing `fab-react-toolkit-0.4.1/example/app/apis.py` & `fab_react_toolkit-0.4.2/example/app/apis.py`

 * *Files identical despite different names*

### Comparing `fab-react-toolkit-0.4.1/example/app/config.py` & `fab_react_toolkit-0.4.2/example/app/config.py`

 * *Files identical despite different names*

### Comparing `fab-react-toolkit-0.4.1/example/app/models.py` & `fab_react_toolkit-0.4.2/example/app/models.py`

 * *Files identical despite different names*

### Comparing `fab-react-toolkit-0.4.1/example/run.py` & `fab_react_toolkit-0.4.2/example/run.py`

 * *Files identical despite different names*

### Comparing `fab-react-toolkit-0.4.1/fab_react_toolkit/__init__.py` & `fab_react_toolkit-0.4.2/fab_react_toolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `fab-react-toolkit-0.4.1/fab_react_toolkit/api/__init__.py` & `fab_react_toolkit-0.4.2/fab_react_toolkit/api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -414,15 +414,15 @@
                 The response from the bulk operation.
 
             """
             id_list = request.get_json()
             bulk_func = getattr(self, f"bulk_{handler}")
             return bulk_func(id_list)
     
-    @expose("/download", methods=["POST"])
+    @expose("/download", methods=["PUT"])
     @protect(allow_browser_login=True)
     @safe
     def download(self):
         query_params = request.json.get("queryParams", "")
 
         query = self.datamodel.session.query(self.datamodel.obj)
```

### Comparing `fab-react-toolkit-0.4.1/fab_react_toolkit/api/convert.py` & `fab_react_toolkit-0.4.2/fab_react_toolkit/api/convert.py`

 * *Files identical despite different names*

### Comparing `fab-react-toolkit-0.4.1/fab_react_toolkit/api/utils.py` & `fab_react_toolkit-0.4.2/fab_react_toolkit/api/utils.py`

 * *Files identical despite different names*

### Comparing `fab-react-toolkit-0.4.1/fab_react_toolkit/apis.py` & `fab_react_toolkit-0.4.2/fab_react_toolkit/apis.py`

 * *Files identical despite different names*

### Comparing `fab-react-toolkit-0.4.1/fab_react_toolkit/filters.py` & `fab_react_toolkit-0.4.2/fab_react_toolkit/filters.py`

 * *Files identical despite different names*

### Comparing `fab-react-toolkit-0.4.1/fab_react_toolkit/views.py` & `fab_react_toolkit-0.4.2/fab_react_toolkit/views.py`

 * *Files identical despite different names*

### Comparing `fab-react-toolkit-0.4.1/fab_react_toolkit.egg-info/PKG-INFO` & `fab_react_toolkit-0.4.2/fab_react_toolkit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fab-react-toolkit
-Version: 0.4.1
+Version: 0.4.2
 Summary: A small example package
 Author-email: Matthias Leinweber <m.leinweber@datatactics.de>
 Project-URL: Homepage, https://github.com/dttctcs/fab-react-toolkit
 Project-URL: Issues, https://github.com/dttctcs/fab-react-toolkit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fab-react-toolkit-0.4.1/fab_react_toolkit.egg-info/SOURCES.txt` & `fab_react_toolkit-0.4.2/fab_react_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fab-react-toolkit-0.4.1/pyproject.toml` & `fab_react_toolkit-0.4.2/pyproject.toml`

 * *Files identical despite different names*

