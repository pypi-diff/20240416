# Comparing `tmp/energiinfo-1.0.1.tar.gz` & `tmp/energiinfo-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "energiinfo-1.0.1.tar", last modified: Tue Apr 16 13:30:59 2024, max compression
+gzip compressed data, was "energiinfo-1.0.2.tar", last modified: Tue Apr 16 13:34:06 2024, max compression
```

## Comparing `energiinfo-1.0.1.tar` & `energiinfo-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 veulsan  (2037719458) 1135428931        0 2024-04-16 13:30:59.273381 energiinfo-1.0.1/
--rw-r--r--   0 veulsan  (2037719458) 1135428931    35149 2024-04-16 12:42:03.000000 energiinfo-1.0.1/LICENSE
--rw-r--r--   0 veulsan  (2037719458) 1135428931     1917 2024-04-16 13:30:59.272691 energiinfo-1.0.1/PKG-INFO
--rw-r--r--   0 veulsan  (2037719458) 1135428931     1359 2024-04-16 12:42:03.000000 energiinfo-1.0.1/README.md
--rw-r--r--   0 veulsan  (2037719458) 1135428931       87 2024-04-16 13:30:50.000000 energiinfo-1.0.1/pyproject.toml
--rw-r--r--   0 veulsan  (2037719458) 1135428931      685 2024-04-16 13:30:59.285241 energiinfo-1.0.1/setup.cfg
-drwxr-xr-x   0 veulsan  (2037719458) 1135428931        0 2024-04-16 13:30:59.224506 energiinfo-1.0.1/src/
-drwxr-xr-x   0 veulsan  (2037719458) 1135428931        0 2024-04-16 13:30:59.245622 energiinfo-1.0.1/src/energiinfo/
--rw-r--r--   0 veulsan  (2037719458) 1135428931       85 2024-04-16 13:26:33.000000 energiinfo-1.0.1/src/energiinfo/__init__.py
--rw-r--r--   0 veulsan  (2037719458) 1135428931     8812 2024-04-16 13:13:32.000000 energiinfo-1.0.1/src/energiinfo/api.py
--rw-r--r--   0 veulsan  (2037719458) 1135428931     1009 2024-04-16 13:18:42.000000 energiinfo-1.0.1/src/energiinfo/const.py
-drwxr-xr-x   0 veulsan  (2037719458) 1135428931        0 2024-04-16 13:30:59.271359 energiinfo-1.0.1/src/energiinfo.egg-info/
--rw-r--r--   0 veulsan  (2037719458) 1135428931     1917 2024-04-16 13:30:59.000000 energiinfo-1.0.1/src/energiinfo.egg-info/PKG-INFO
--rw-r--r--   0 veulsan  (2037719458) 1135428931      267 2024-04-16 13:30:59.000000 energiinfo-1.0.1/src/energiinfo.egg-info/SOURCES.txt
--rw-r--r--   0 veulsan  (2037719458) 1135428931        1 2024-04-16 13:30:59.000000 energiinfo-1.0.1/src/energiinfo.egg-info/dependency_links.txt
--rw-r--r--   0 veulsan  (2037719458) 1135428931       11 2024-04-16 13:30:59.000000 energiinfo-1.0.1/src/energiinfo.egg-info/top_level.txt
+drwxr-xr-x   0 veulsan  (2037719458) 1135428931        0 2024-04-16 13:34:06.740697 energiinfo-1.0.2/
+-rw-r--r--   0 veulsan  (2037719458) 1135428931    35149 2024-04-16 12:42:03.000000 energiinfo-1.0.2/LICENSE
+-rw-r--r--   0 veulsan  (2037719458) 1135428931     1917 2024-04-16 13:34:06.740475 energiinfo-1.0.2/PKG-INFO
+-rw-r--r--   0 veulsan  (2037719458) 1135428931     1359 2024-04-16 12:42:03.000000 energiinfo-1.0.2/README.md
+-rw-r--r--   0 veulsan  (2037719458) 1135428931       87 2024-04-16 13:30:50.000000 energiinfo-1.0.2/pyproject.toml
+-rw-r--r--   0 veulsan  (2037719458) 1135428931      685 2024-04-16 13:34:06.742312 energiinfo-1.0.2/setup.cfg
+drwxr-xr-x   0 veulsan  (2037719458) 1135428931        0 2024-04-16 13:34:06.721684 energiinfo-1.0.2/src/
+drwxr-xr-x   0 veulsan  (2037719458) 1135428931        0 2024-04-16 13:34:06.728154 energiinfo-1.0.2/src/energiinfo/
+-rw-r--r--   0 veulsan  (2037719458) 1135428931       85 2024-04-16 13:33:42.000000 energiinfo-1.0.2/src/energiinfo/__init__.py
+-rw-r--r--   0 veulsan  (2037719458) 1135428931     8812 2024-04-16 13:32:22.000000 energiinfo-1.0.2/src/energiinfo/api.py
+-rw-r--r--   0 veulsan  (2037719458) 1135428931     1009 2024-04-16 13:18:42.000000 energiinfo-1.0.2/src/energiinfo/const.py
+drwxr-xr-x   0 veulsan  (2037719458) 1135428931        0 2024-04-16 13:34:06.739956 energiinfo-1.0.2/src/energiinfo.egg-info/
+-rw-r--r--   0 veulsan  (2037719458) 1135428931     1917 2024-04-16 13:34:06.000000 energiinfo-1.0.2/src/energiinfo.egg-info/PKG-INFO
+-rw-r--r--   0 veulsan  (2037719458) 1135428931      267 2024-04-16 13:34:06.000000 energiinfo-1.0.2/src/energiinfo.egg-info/SOURCES.txt
+-rw-r--r--   0 veulsan  (2037719458) 1135428931        1 2024-04-16 13:34:06.000000 energiinfo-1.0.2/src/energiinfo.egg-info/dependency_links.txt
+-rw-r--r--   0 veulsan  (2037719458) 1135428931       11 2024-04-16 13:34:06.000000 energiinfo-1.0.2/src/energiinfo.egg-info/top_level.txt
```

### Comparing `energiinfo-1.0.1/LICENSE` & `energiinfo-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `energiinfo-1.0.1/PKG-INFO` & `energiinfo-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: energiinfo
-Version: 1.0.1
+Version: 1.0.2
 Summary: Energiinfo API package
 Home-page: https://gitlab.com/veulsan/energiinfo
 Author: Ulrik Sannsell
 Author-email: ulrik@sannsell.se
 Project-URL: Bug Tracker, https://gitlab.com/veulsan/energiinfo/-/issues
 Project-URL: repository, https://gitlab.com/veulsan/energiinfo
 Classifier: Programming Language :: Python :: 3
```

### Comparing `energiinfo-1.0.1/README.md` & `energiinfo-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `energiinfo-1.0.1/setup.cfg` & `energiinfo-1.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = energiinfo
-version = 1.0.1
+version = 1.0.2
 author = Ulrik Sannsell
 author_email = ulrik@sannsell.se
 description = Energiinfo API package
 long_description = file: README.md, LICENSE.txt
 long_description_content_type = text/markdown
 url = https://gitlab.com/veulsan/energiinfo
 project_urls =
```

### Comparing `energiinfo-1.0.1/src/energiinfo/api.py` & `energiinfo-1.0.2/src/energiinfo/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     CMD_PROFILE,
     CMD_METERPOINTS,
     CMD_INVOICES,
     CMD_PERIOD,
     CMD_OBJECTSETTINGS,
     CMD_TEMPERATURE,
     CLIENT_HEADERS,
-    TOKEN_EXPRIATION,
+    TOKEN_EXPIRATION,
     USER_AGENT_TEMPLATE,
 )
 
 #https://api4.energiinfo.se/?access_token=none&cmd=login
 
 class EnergiinfoClient:
     """
```

### Comparing `energiinfo-1.0.1/src/energiinfo/const.py` & `energiinfo-1.0.2/src/energiinfo/const.py`

 * *Files identical despite different names*

### Comparing `energiinfo-1.0.1/src/energiinfo.egg-info/PKG-INFO` & `energiinfo-1.0.2/src/energiinfo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: energiinfo
-Version: 1.0.1
+Version: 1.0.2
 Summary: Energiinfo API package
 Home-page: https://gitlab.com/veulsan/energiinfo
 Author: Ulrik Sannsell
 Author-email: ulrik@sannsell.se
 Project-URL: Bug Tracker, https://gitlab.com/veulsan/energiinfo/-/issues
 Project-URL: repository, https://gitlab.com/veulsan/energiinfo
 Classifier: Programming Language :: Python :: 3
```

