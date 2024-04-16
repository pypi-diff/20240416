# Comparing `tmp/gpp_components-0.0.9.tar.gz` & `tmp/gpp_components-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpp_components-0.0.9.tar", last modified: Tue Dec 26 06:01:20 2023, max compression
+gzip compressed data, was "gpp_components-0.1.0.tar", last modified: Tue Apr 16 01:09:36 2024, max compression
```

## Comparing `gpp_components-0.0.9.tar` & `gpp_components-0.1.0.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-12-26 06:01:20.132431 gpp_components-0.0.9/
--rw-rw-rw-   0        0        0     1097 2023-11-13 03:12:05.000000 gpp_components-0.0.9/LICENSE
--rw-rw-rw-   0        0        0      386 2023-12-26 06:01:20.126373 gpp_components-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0       58 2023-11-13 03:12:05.000000 gpp_components-0.0.9/README.md
-drwxrwxrwx   0        0        0        0 2023-12-26 06:01:20.073129 gpp_components-0.0.9/gpp_components/
--rw-rw-rw-   0        0        0       19 2023-12-26 05:13:21.000000 gpp_components-0.0.9/gpp_components/__init__.py
--rw-rw-rw-   0        0        0     1076 2023-12-26 05:13:21.000000 gpp_components-0.0.9/gpp_components/aes.py
--rw-rw-rw-   0        0        0       67 2023-12-26 05:13:21.000000 gpp_components-0.0.9/gpp_components/constant.py
--rw-rw-rw-   0        0        0     4442 2023-12-26 05:13:21.000000 gpp_components-0.0.9/gpp_components/dbConfig.py
--rw-rw-rw-   0        0        0     6755 2023-12-26 05:13:21.000000 gpp_components-0.0.9/gpp_components/handleData.py
--rw-rw-rw-   0        0        0     1629 2023-12-26 05:13:21.000000 gpp_components-0.0.9/gpp_components/lazyImport.py
--rw-rw-rw-   0        0        0      960 2023-12-26 05:13:21.000000 gpp_components-0.0.9/gpp_components/response.py
--rw-rw-rw-   0        0        0     2621 2023-12-26 06:00:55.000000 gpp_components-0.0.9/gpp_components/runOracle.py
--rw-rw-rw-   0        0        0     2880 2023-12-26 05:13:21.000000 gpp_components-0.0.9/gpp_components/sendMail.py
-drwxrwxrwx   0        0        0        0 2023-12-26 06:01:20.114063 gpp_components-0.0.9/gpp_components.egg-info/
--rw-rw-rw-   0        0        0      386 2023-12-26 06:01:19.000000 gpp_components-0.0.9/gpp_components.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      458 2023-12-26 06:01:19.000000 gpp_components-0.0.9/gpp_components.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-26 06:01:19.000000 gpp_components-0.0.9/gpp_components.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-12-26 06:01:19.000000 gpp_components-0.0.9/gpp_components.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-12-26 06:01:19.000000 gpp_components-0.0.9/gpp_components.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-12-26 06:01:20.132431 gpp_components-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0      697 2023-12-26 06:01:09.000000 gpp_components-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 01:09:36.489777 gpp_components-0.1.0/
+-rw-rw-rw-   0        0        0     1097 2023-11-13 03:12:05.000000 gpp_components-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0      412 2024-04-16 01:09:36.480260 gpp_components-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0       58 2023-11-13 03:12:05.000000 gpp_components-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-16 01:09:36.412983 gpp_components-0.1.0/gpp_components/
+-rw-rw-rw-   0        0        0       19 2023-12-26 05:13:21.000000 gpp_components-0.1.0/gpp_components/__init__.py
+-rw-rw-rw-   0        0        0     1076 2023-12-26 05:13:21.000000 gpp_components-0.1.0/gpp_components/aes.py
+-rw-rw-rw-   0        0        0      239 2024-02-22 03:46:53.000000 gpp_components-0.1.0/gpp_components/constant.py
+-rw-rw-rw-   0        0        0     4442 2023-12-26 05:13:21.000000 gpp_components-0.1.0/gpp_components/dbConfig.py
+-rw-rw-rw-   0        0        0     2535 2024-04-16 01:08:29.000000 gpp_components-0.1.0/gpp_components/decorator.py
+-rw-rw-rw-   0        0        0     9380 2024-04-16 01:08:22.000000 gpp_components-0.1.0/gpp_components/fileImporter.py
+-rw-rw-rw-   0        0        0     7696 2024-04-16 01:08:29.000000 gpp_components-0.1.0/gpp_components/handleData.py
+-rw-rw-rw-   0        0        0     1629 2023-12-26 05:13:21.000000 gpp_components-0.1.0/gpp_components/lazyImport.py
+-rw-rw-rw-   0        0        0     1422 2024-03-20 05:27:27.000000 gpp_components-0.1.0/gpp_components/response.py
+-rw-rw-rw-   0        0        0     5181 2024-04-16 01:08:22.000000 gpp_components-0.1.0/gpp_components/runOracle.py
+-rw-rw-rw-   0        0        0     2880 2023-12-26 05:13:21.000000 gpp_components-0.1.0/gpp_components/sendMail.py
+drwxrwxrwx   0        0        0        0 2024-04-16 01:09:36.462565 gpp_components-0.1.0/gpp_components.egg-info/
+-rw-rw-rw-   0        0        0      412 2024-04-16 01:09:35.000000 gpp_components-0.1.0/gpp_components.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      517 2024-04-16 01:09:36.000000 gpp_components-0.1.0/gpp_components.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 01:09:35.000000 gpp_components-0.1.0/gpp_components.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-04-16 01:09:35.000000 gpp_components-0.1.0/gpp_components.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-16 01:09:35.000000 gpp_components-0.1.0/gpp_components.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-16 01:09:36.491030 gpp_components-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      825 2024-04-16 01:09:10.000000 gpp_components-0.1.0/setup.py
```

### Comparing `gpp_components-0.0.9/LICENSE` & `gpp_components-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gpp_components-0.0.9/gpp_components/aes.py` & `gpp_components-0.1.0/gpp_components/aes.py`

 * *Files identical despite different names*

### Comparing `gpp_components-0.0.9/gpp_components/dbConfig.py` & `gpp_components-0.1.0/gpp_components/dbConfig.py`

 * *Files identical despite different names*

### Comparing `gpp_components-0.0.9/gpp_components/handleData.py` & `gpp_components-0.1.0/gpp_components/handleData.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,56 @@
 from .constant import Constant
 from .response import Response
 from django.apps import apps
 from copy import deepcopy
 from django.db.models import Q  # 不要拿掉
 from jsonpath import jsonpath
+from django.core.paginator import Paginator
 
 
 class HandleData(Constant):
-    def get_(self, table_name, conditions={}):
+    def get_(
+        self, table_name, conditions={}, page_size=None, current_page=None, sort=None
+    ):
         # table_name = kwargs.get("table_name")
         # condition = {} if not kwargs.get("condition")
         name_type = "db_table" if not "." in table_name else "verbose_name"
 
         if len(list(conditions.keys())) == 0:
             conditions = {"data": [{}]}
 
         if "data" not in list(conditions.keys()):
             conditions = {"data": [conditions]}
-            
+
         condition = strConditions(formatConditions(conditions))
 
         for model in apps.get_models():
             if model._meta.app_label == self.app_name:
                 if model._meta.__getattribute__(name_type) == table_name:
-                    qs = model.objects.filter(eval(condition)).all().values()
-                    return Response(data=list(qs))
-        return Response(data=[])
+                    models = model.objects.filter(eval(condition))
+                    qs = models.all().values()
+                    if not sort == None:
+                        qs = qs.order_by(sort)
+                    if page_size == None:
+                        return Response(data=list(qs))
+                    else:
+                        # 创建Paginator对象并指定每页显示的记录数量
+                        paginator = Paginator(list(qs), per_page=page_size)
+                        page = paginator.get_page(current_page)
+
+                        return Response(
+                            data=list(page.object_list),
+                            page={
+                                "total_count": paginator.count,
+                                "num_pages": paginator.num_pages,
+                                "current_page": page.number,
+                            },
+                        )
+
+        return Response(False, "table is not found!", [])
 
     # {
     #   "action":"insert",
     #   "table_name":"TBL_USER",
     #   "data":[
     #     { user_name:"d1"},
     #     { user_name:"d2"},
```

### Comparing `gpp_components-0.0.9/gpp_components/lazyImport.py` & `gpp_components-0.1.0/gpp_components/lazyImport.py`

 * *Files identical despite different names*

### Comparing `gpp_components-0.0.9/gpp_components/response.py` & `gpp_components-0.1.0/gpp_components/response.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,53 @@
 import json
 from types import NoneType
 
 
 class Response:
     def __init__(
-        self, success: bool = True, msg: str or NoneType = None, data: list = []
+        self,
+        success: bool = True,
+        msg: str | NoneType = None,
+        data: list = [],
+        page: dict | NoneType = None,
     ):
         try:
             assert type(success) == bool, "success is not boolean"
             self.success = success
             assert (
                 a := type(msg)
             ) == str or a == NoneType, "msg is not string or None Type"
             self.msg = msg
             assert type(data) == list, "data is not list/array"
             self.data = data
+            assert (
+                a := type(page)
+            ) == dict or a == NoneType, "page is not dict(object)"
+            self.page = page
+
         except Exception as e:
             self.success = False
             self.msg = str(e)
             self.data = []
+            self.page = None
 
     def __str__(self):
-        return json.dumps({"success": self.success, "msg": self.msg, "data": self.data})
+        return json.dumps(
+            {
+                "success": self.success,
+                "msg": self.msg,
+                "data": self.data,
+                "page": self.page,
+            }
+        )
 
     @property
     def json(self):
-        return {
+        json = {
             "success": str(self.success).lower(),
             "msg": self.msg,
             "data": self.data,
         }
+        if self.page:
+            json["page"] = self.page
+
+        return json
```

### Comparing `gpp_components-0.0.9/gpp_components/sendMail.py` & `gpp_components-0.1.0/gpp_components/sendMail.py`

 * *Files identical despite different names*

### Comparing `gpp_components-0.0.9/setup.py` & `gpp_components-0.1.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,36 @@
 import os, shutil
 
 os.chdir(r"D:\Coding\GPP-Vue\gpp-py-components")
+# os.chdir(r"D:\gitLab\gpp-py-components")
 dir_list = ["./build", "./dist", "./gpp_components.egg-info"]
 for i in dir_list:
     if os.path.exists(i):
         shutil.rmtree(i)
 
 
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="gpp_components",
-    version="0.0.9",
+    version="0.1.0",
     #
     author="L",
     description="for internal use",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT Licence",
     #
     packages=find_packages(),
-    install_requires=["crypto", "django", "cx_Oracle", "pandas", "jsonpath", "rich"],
+    install_requires=[
+        "crypto",
+        "django",
+        "oracledb",
+        "pandas",
+        "jsonpath",
+        "rich",
+        "SQLAlchemy",
+    ],
 )
```

