# Comparing `tmp/xcloud_client-3.2.tar.gz` & `tmp/xcloud_client-3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xcloud_client-3.2.tar", last modified: Mon Apr 15 04:56:56 2024, max compression
+gzip compressed data, was "xcloud_client-3.3.tar", last modified: Tue Apr 16 09:48:42 2024, max compression
```

## Comparing `xcloud_client-3.2.tar` & `xcloud_client-3.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 04:56:56.411308 xcloud_client-3.2/
--rw-rw-rw-   0        0        0       19 2024-04-14 06:52:25.000000 xcloud_client-3.2/MANIFEST.in
--rw-rw-rw-   0        0        0      126 2024-04-15 04:56:56.409308 xcloud_client-3.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-15 04:56:56.382305 xcloud_client-3.2/resources/
--rw-rw-rw-   0        0        0  1358472 2021-10-15 08:05:30.000000 xcloud_client-3.2/resources/XCloudJDBC-2.10.6.7.jar
--rw-rw-rw-   0        0        0   275539 2021-10-15 08:05:26.000000 xcloud_client-3.2/resources/XCloudJDBC_SP_Procedure_Parser-0.1.3.jar
--rw-rw-rw-   0        0        0   227712 2019-07-16 09:51:20.000000 xcloud_client-3.2/resources/libthrift-0.9.2.jar
--rw-rw-rw-   0        0        0   489884 2019-07-16 09:51:20.000000 xcloud_client-3.2/resources/log4j-1.2.17.jar
--rw-rw-rw-   0        0        0   236880 2019-07-16 09:51:20.000000 xcloud_client-3.2/resources/lz4-1.3.0.jar
--rw-rw-rw-   0        0        0  1555682 2023-08-17 03:30:59.000000 xcloud_client-3.2/resources/ojdbc14-10.2.0.4.0.jar
--rw-rw-rw-   0        0        0    23445 2019-09-11 10:52:32.000000 xcloud_client-3.2/resources/slf4j-api-1.5.8.jar
--rw-rw-rw-   0        0        0    26084 2018-10-10 07:16:32.000000 xcloud_client-3.2/resources/slf4j-api-1.7.5.jar
--rw-rw-rw-   0        0        0     8869 2021-10-15 08:05:28.000000 xcloud_client-3.2/resources/slf4j-log4j12-1.7.5.jar
--rw-rw-rw-   0        0        0    10680 2019-09-11 10:52:28.000000 xcloud_client-3.2/resources/slf4j-simple-1.7.5.jar
--rw-rw-rw-   0        0        0       42 2024-04-15 04:56:56.411308 xcloud_client-3.2/setup.cfg
--rw-rw-rw-   0        0        0      309 2024-04-15 04:56:37.000000 xcloud_client-3.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-15 04:56:56.389308 xcloud_client-3.2/xcloud_client/
--rw-rw-rw-   0        0        0       23 2024-04-15 03:30:26.000000 xcloud_client-3.2/xcloud_client/__init__.py
--rw-rw-rw-   0        0        0     2656 2024-04-15 04:56:18.000000 xcloud_client-3.2/xcloud_client/xCloud_client.py
-drwxrwxrwx   0        0        0        0 2024-04-15 04:56:56.405307 xcloud_client-3.2/xcloud_client.egg-info/
--rw-rw-rw-   0        0        0      126 2024-04-15 04:56:55.000000 xcloud_client-3.2/xcloud_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      587 2024-04-15 04:56:56.000000 xcloud_client-3.2/xcloud_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 04:56:55.000000 xcloud_client-3.2/xcloud_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-04-15 04:56:55.000000 xcloud_client-3.2/xcloud_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-15 04:56:55.000000 xcloud_client-3.2/xcloud_client.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-16 09:48:42.553707 xcloud_client-3.3/
+-rw-rw-rw-   0        0        0       19 2024-04-14 06:52:25.000000 xcloud_client-3.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      126 2024-04-16 09:48:42.552707 xcloud_client-3.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-16 09:48:42.520586 xcloud_client-3.3/resources/
+-rw-rw-rw-   0        0        0  1358472 2021-10-15 08:05:30.000000 xcloud_client-3.3/resources/XCloudJDBC-2.10.6.7.jar
+-rw-rw-rw-   0        0        0   275539 2021-10-15 08:05:26.000000 xcloud_client-3.3/resources/XCloudJDBC_SP_Procedure_Parser-0.1.3.jar
+-rw-rw-rw-   0        0        0   227712 2019-07-16 09:51:20.000000 xcloud_client-3.3/resources/libthrift-0.9.2.jar
+-rw-rw-rw-   0        0        0   489884 2019-07-16 09:51:20.000000 xcloud_client-3.3/resources/log4j-1.2.17.jar
+-rw-rw-rw-   0        0        0   236880 2019-07-16 09:51:20.000000 xcloud_client-3.3/resources/lz4-1.3.0.jar
+-rw-rw-rw-   0        0        0  1555682 2023-08-17 03:30:59.000000 xcloud_client-3.3/resources/ojdbc14-10.2.0.4.0.jar
+-rw-rw-rw-   0        0        0    23445 2019-09-11 10:52:32.000000 xcloud_client-3.3/resources/slf4j-api-1.5.8.jar
+-rw-rw-rw-   0        0        0    26084 2018-10-10 07:16:32.000000 xcloud_client-3.3/resources/slf4j-api-1.7.5.jar
+-rw-rw-rw-   0        0        0     8869 2021-10-15 08:05:28.000000 xcloud_client-3.3/resources/slf4j-log4j12-1.7.5.jar
+-rw-rw-rw-   0        0        0    10680 2019-09-11 10:52:28.000000 xcloud_client-3.3/resources/slf4j-simple-1.7.5.jar
+-rw-rw-rw-   0        0        0       42 2024-04-16 09:48:42.554723 xcloud_client-3.3/setup.cfg
+-rw-rw-rw-   0        0        0      309 2024-04-16 09:47:07.000000 xcloud_client-3.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 09:48:42.527526 xcloud_client-3.3/xcloud_client/
+-rw-rw-rw-   0        0        0       23 2024-04-16 09:46:56.000000 xcloud_client-3.3/xcloud_client/__init__.py
+-rw-rw-rw-   0        0        0     2656 2024-04-15 04:56:18.000000 xcloud_client-3.3/xcloud_client/xCloud_client.py
+drwxrwxrwx   0        0        0        0 2024-04-16 09:48:42.546735 xcloud_client-3.3/xcloud_client.egg-info/
+-rw-rw-rw-   0        0        0      126 2024-04-16 09:48:41.000000 xcloud_client-3.3/xcloud_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      587 2024-04-16 09:48:42.000000 xcloud_client-3.3/xcloud_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 09:48:41.000000 xcloud_client-3.3/xcloud_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-04-16 09:48:41.000000 xcloud_client-3.3/xcloud_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-16 09:48:41.000000 xcloud_client-3.3/xcloud_client.egg-info/top_level.txt
```

### Comparing `xcloud_client-3.2/resources/XCloudJDBC-2.10.6.7.jar` & `xcloud_client-3.3/resources/XCloudJDBC-2.10.6.7.jar`

 * *Files identical despite different names*

### Comparing `xcloud_client-3.2/resources/XCloudJDBC_SP_Procedure_Parser-0.1.3.jar` & `xcloud_client-3.3/resources/XCloudJDBC_SP_Procedure_Parser-0.1.3.jar`

 * *Files identical despite different names*

### Comparing `xcloud_client-3.2/resources/libthrift-0.9.2.jar` & `xcloud_client-3.3/resources/libthrift-0.9.2.jar`

 * *Files identical despite different names*

### Comparing `xcloud_client-3.2/resources/log4j-1.2.17.jar` & `xcloud_client-3.3/resources/log4j-1.2.17.jar`

 * *Files identical despite different names*

### Comparing `xcloud_client-3.2/resources/lz4-1.3.0.jar` & `xcloud_client-3.3/resources/lz4-1.3.0.jar`

 * *Files identical despite different names*

### Comparing `xcloud_client-3.2/resources/ojdbc14-10.2.0.4.0.jar` & `xcloud_client-3.3/resources/ojdbc14-10.2.0.4.0.jar`

 * *Files identical despite different names*

### Comparing `xcloud_client-3.2/resources/slf4j-api-1.5.8.jar` & `xcloud_client-3.3/resources/slf4j-api-1.5.8.jar`

 * *Files identical despite different names*

### Comparing `xcloud_client-3.2/resources/slf4j-api-1.7.5.jar` & `xcloud_client-3.3/resources/slf4j-api-1.7.5.jar`

 * *Files identical despite different names*

### Comparing `xcloud_client-3.2/resources/slf4j-log4j12-1.7.5.jar` & `xcloud_client-3.3/resources/slf4j-log4j12-1.7.5.jar`

 * *Files identical despite different names*

### Comparing `xcloud_client-3.2/resources/slf4j-simple-1.7.5.jar` & `xcloud_client-3.3/resources/slf4j-simple-1.7.5.jar`

 * *Files identical despite different names*

### Comparing `xcloud_client-3.2/xcloud_client/xCloud_client.py` & `xcloud_client-3.3/xcloud_client/xCloud_client.py`

 * *Files identical despite different names*

### Comparing `xcloud_client-3.2/xcloud_client.egg-info/SOURCES.txt` & `xcloud_client-3.3/xcloud_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

