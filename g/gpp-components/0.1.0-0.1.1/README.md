# Comparing `tmp/gpp_components-0.1.0.tar.gz` & `tmp/gpp_components-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpp_components-0.1.0.tar", last modified: Tue Apr 16 01:09:36 2024, max compression
+gzip compressed data, was "gpp_components-0.1.1.tar", last modified: Tue Apr 16 01:34:12 2024, max compression
```

## Comparing `gpp_components-0.1.0.tar` & `gpp_components-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 01:09:36.489777 gpp_components-0.1.0/
--rw-rw-rw-   0        0        0     1097 2023-11-13 03:12:05.000000 gpp_components-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      412 2024-04-16 01:09:36.480260 gpp_components-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       58 2023-11-13 03:12:05.000000 gpp_components-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-16 01:09:36.412983 gpp_components-0.1.0/gpp_components/
--rw-rw-rw-   0        0        0       19 2023-12-26 05:13:21.000000 gpp_components-0.1.0/gpp_components/__init__.py
--rw-rw-rw-   0        0        0     1076 2023-12-26 05:13:21.000000 gpp_components-0.1.0/gpp_components/aes.py
--rw-rw-rw-   0        0        0      239 2024-02-22 03:46:53.000000 gpp_components-0.1.0/gpp_components/constant.py
--rw-rw-rw-   0        0        0     4442 2023-12-26 05:13:21.000000 gpp_components-0.1.0/gpp_components/dbConfig.py
--rw-rw-rw-   0        0        0     2535 2024-04-16 01:08:29.000000 gpp_components-0.1.0/gpp_components/decorator.py
--rw-rw-rw-   0        0        0     9380 2024-04-16 01:08:22.000000 gpp_components-0.1.0/gpp_components/fileImporter.py
--rw-rw-rw-   0        0        0     7696 2024-04-16 01:08:29.000000 gpp_components-0.1.0/gpp_components/handleData.py
--rw-rw-rw-   0        0        0     1629 2023-12-26 05:13:21.000000 gpp_components-0.1.0/gpp_components/lazyImport.py
--rw-rw-rw-   0        0        0     1422 2024-03-20 05:27:27.000000 gpp_components-0.1.0/gpp_components/response.py
--rw-rw-rw-   0        0        0     5181 2024-04-16 01:08:22.000000 gpp_components-0.1.0/gpp_components/runOracle.py
--rw-rw-rw-   0        0        0     2880 2023-12-26 05:13:21.000000 gpp_components-0.1.0/gpp_components/sendMail.py
-drwxrwxrwx   0        0        0        0 2024-04-16 01:09:36.462565 gpp_components-0.1.0/gpp_components.egg-info/
--rw-rw-rw-   0        0        0      412 2024-04-16 01:09:35.000000 gpp_components-0.1.0/gpp_components.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      517 2024-04-16 01:09:36.000000 gpp_components-0.1.0/gpp_components.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 01:09:35.000000 gpp_components-0.1.0/gpp_components.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-04-16 01:09:35.000000 gpp_components-0.1.0/gpp_components.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-16 01:09:35.000000 gpp_components-0.1.0/gpp_components.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-16 01:09:36.491030 gpp_components-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      825 2024-04-16 01:09:10.000000 gpp_components-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 01:34:12.204173 gpp_components-0.1.1/
+-rw-rw-rw-   0        0        0     1097 2023-11-13 03:12:05.000000 gpp_components-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      412 2024-04-16 01:34:12.197196 gpp_components-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       58 2023-11-13 03:12:05.000000 gpp_components-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-16 01:34:12.108817 gpp_components-0.1.1/gpp_components/
+-rw-rw-rw-   0        0        0       19 2023-12-26 05:13:21.000000 gpp_components-0.1.1/gpp_components/__init__.py
+-rw-rw-rw-   0        0        0     1076 2023-12-26 05:13:21.000000 gpp_components-0.1.1/gpp_components/aes.py
+-rw-rw-rw-   0        0        0      239 2024-02-22 03:46:53.000000 gpp_components-0.1.1/gpp_components/constant.py
+-rw-rw-rw-   0        0        0     4442 2023-12-26 05:13:21.000000 gpp_components-0.1.1/gpp_components/dbConfig.py
+-rw-rw-rw-   0        0        0     2535 2024-04-16 01:08:29.000000 gpp_components-0.1.1/gpp_components/decorator.py
+-rw-rw-rw-   0        0        0     9380 2024-04-16 01:08:22.000000 gpp_components-0.1.1/gpp_components/fileImporter.py
+-rw-rw-rw-   0        0        0     7696 2024-04-16 01:08:29.000000 gpp_components-0.1.1/gpp_components/handleData.py
+-rw-rw-rw-   0        0        0     1629 2023-12-26 05:13:21.000000 gpp_components-0.1.1/gpp_components/lazyImport.py
+-rw-rw-rw-   0        0        0     1422 2024-03-20 05:27:27.000000 gpp_components-0.1.1/gpp_components/response.py
+-rw-rw-rw-   0        0        0     5115 2024-04-16 01:33:35.000000 gpp_components-0.1.1/gpp_components/runOracle.py
+-rw-rw-rw-   0        0        0     2880 2023-12-26 05:13:21.000000 gpp_components-0.1.1/gpp_components/sendMail.py
+drwxrwxrwx   0        0        0        0 2024-04-16 01:34:12.165610 gpp_components-0.1.1/gpp_components.egg-info/
+-rw-rw-rw-   0        0        0      412 2024-04-16 01:34:11.000000 gpp_components-0.1.1/gpp_components.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      517 2024-04-16 01:34:11.000000 gpp_components-0.1.1/gpp_components.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 01:34:11.000000 gpp_components-0.1.1/gpp_components.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-04-16 01:34:11.000000 gpp_components-0.1.1/gpp_components.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-16 01:34:11.000000 gpp_components-0.1.1/gpp_components.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-16 01:34:12.206180 gpp_components-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      877 2024-04-16 01:34:07.000000 gpp_components-0.1.1/setup.py
```

### Comparing `gpp_components-0.1.0/LICENSE` & `gpp_components-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gpp_components-0.1.0/gpp_components/aes.py` & `gpp_components-0.1.1/gpp_components/aes.py`

 * *Files identical despite different names*

### Comparing `gpp_components-0.1.0/gpp_components/dbConfig.py` & `gpp_components-0.1.1/gpp_components/dbConfig.py`

 * *Files identical despite different names*

### Comparing `gpp_components-0.1.0/gpp_components/decorator.py` & `gpp_components-0.1.1/gpp_components/decorator.py`

 * *Files identical despite different names*

### Comparing `gpp_components-0.1.0/gpp_components/fileImporter.py` & `gpp_components-0.1.1/gpp_components/fileImporter.py`

 * *Files identical despite different names*

### Comparing `gpp_components-0.1.0/gpp_components/handleData.py` & `gpp_components-0.1.1/gpp_components/handleData.py`

 * *Files identical despite different names*

### Comparing `gpp_components-0.1.0/gpp_components/lazyImport.py` & `gpp_components-0.1.1/gpp_components/lazyImport.py`

 * *Files identical despite different names*

### Comparing `gpp_components-0.1.0/gpp_components/response.py` & `gpp_components-0.1.1/gpp_components/response.py`

 * *Files identical despite different names*

### Comparing `gpp_components-0.1.0/gpp_components/runOracle.py` & `gpp_components-0.1.1/gpp_components/runOracle.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,17 +22,15 @@
         service_name = self.tns_config.get("service_name")
         dsn = self.tns_config.get("dsn")
 
         conn_str = f"{user}/{password}@{host}/{service_name}"  # ('system/system@172.24.0.64:1521/helowinXDB')
 
         try:
             # self.conn = oracledb.connect(conn_str)
-            self.conn = oracledb.connect(
-                user=user, password=password, dsn=dsn, encoding="UTF-8"
-            )
+            self.conn = oracledb.connect(user=user, password=password, dsn=dsn)
         except Exception as e:
             return Response(False, "tns is not correct, connection fail !")
 
     def closeConnection(self):
         if self.cursor:
             self.cursor.close()
         if self.conn:
@@ -68,15 +66,15 @@
                 return Response(data=[])
             else:
                 return Response(False, f"No Connenct Found !")
         except oracledb.DatabaseError as e:
             return Response(False, f"Problem in excuteSql: {e}")
         finally:
             self.closeConnection()
-        
+
     def runProc(self, sp_name, jsonStr):
         try:
             if self.conn:
                 # user = self.tns_config.get("user")
                 # password = self.tns_config.get("password")
                 # host = self.tns_config.get("host")
                 # service_name = self.tns_config.get("service_name")
@@ -100,15 +98,15 @@
     def getTNS(self, dbJson):
         host_name = dbJson.get("host_name")
         port = dbJson.get("port")
         container = dbJson.get("container")
         tb_space = dbJson.get("tb_space")
 
         # sqlStr = f"SELECT user_name, user_pwd, tns_content FROM DB_CONFIG WHERE host_name = '{host_name}' AND port = {port} AND container = '{container}' AND tb_space = '{tb_space}'"
-        
+
         sqlStr = f"WITH tmp_data AS (SELECT pid, user_name, user_pwd, tns_content FROM DB_CONFIG WHERE host_name = '{host_name}' AND port = {port} AND container = '{container}' AND tb_space = '{tb_space}'),tmp_root AS (SELECT tns_content FROM DB_CONFIG WHERE ID = (SELECT pid FROM tmp_data)) SELECT a.user_name, a.user_pwd, NVL(a.tns_content, b.tns_content) AS tns_content FROM tmp_data a LEFT JOIN tmp_root b ON 1 = 1"
 
         try:
             rsp = self.runSql(sqlStr)
             if isinstance(rsp, Response):
                 return rsp
             else:
```

### Comparing `gpp_components-0.1.0/gpp_components/sendMail.py` & `gpp_components-0.1.1/gpp_components/sendMail.py`

 * *Files identical despite different names*

### Comparing `gpp_components-0.1.0/gpp_components.egg-info/SOURCES.txt` & `gpp_components-0.1.1/gpp_components.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gpp_components-0.1.0/setup.py` & `gpp_components-0.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="gpp_components",
-    version="0.1.0",
+    version = '0.1.1',
+    # version="0.0.36", # last version for Py310
     #
     author="L",
     description="for internal use",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT Licence",
     #
```

