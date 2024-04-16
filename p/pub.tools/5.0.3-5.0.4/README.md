# Comparing `tmp/pub_tools-5.0.3.tar.gz` & `tmp/pub_tools-5.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pub_tools-5.0.3.tar", last modified: Mon Apr 15 17:24:07 2024, max compression
+gzip compressed data, was "pub_tools-5.0.4.tar", last modified: Tue Apr 16 20:22:40 2024, max compression
```

## Comparing `pub_tools-5.0.3.tar` & `pub_tools-5.0.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:24:07.481336 pub_tools-5.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-15 17:24:03.000000 pub_tools-5.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-15 17:24:07.481336 pub_tools-5.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-15 17:24:03.000000 pub_tools-5.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:24:07.473336 pub_tools-5.0.3/pub/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 17:24:03.000000 pub_tools-5.0.3/pub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:24:07.477336 pub_tools-5.0.3/pub/tools/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-15 17:24:03.000000 pub_tools-5.0.3/pub/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17304 2024-04-15 17:24:03.000000 pub_tools-5.0.3/pub/tools/citations.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-15 17:24:03.000000 pub_tools-5.0.3/pub/tools/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-04-15 17:24:03.000000 pub_tools-5.0.3/pub/tools/cooking.py
--rw-r--r--   0 runner    (1001) docker     (127)    22472 2024-04-15 17:24:03.000000 pub_tools-5.0.3/pub/tools/entrez.py
--rw-r--r--   0 runner    (1001) docker     (127)     8431 2024-04-15 17:24:03.000000 pub_tools-5.0.3/pub/tools/formatting.py
--rw-r--r--   0 runner    (1001) docker     (127)     5380 2024-04-15 17:24:03.000000 pub_tools-5.0.3/pub/tools/isbn.py
--rw-r--r--   0 runner    (1001) docker     (127)  1443107 2024-04-15 17:24:03.000000 pub_tools-5.0.3/pub/tools/journals.json
--rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-04-15 17:24:03.000000 pub_tools-5.0.3/pub/tools/journals.py
--rw-r--r--   0 runner    (1001) docker     (127)     8659 2024-04-15 17:24:03.000000 pub_tools-5.0.3/pub/tools/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:24:07.481336 pub_tools-5.0.3/pub/tools/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-15 17:24:03.000000 pub_tools-5.0.3/pub/tools/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24651 2024-04-15 17:24:03.000000 pub_tools-5.0.3/pub/tools/tests/test_citations.py
--rw-r--r--   0 runner    (1001) docker     (127)    17851 2024-04-15 17:24:03.000000 pub_tools-5.0.3/pub/tools/tests/test_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (127)    25839 2024-04-15 17:24:03.000000 pub_tools-5.0.3/pub/tools/tests/test_entrez.py
--rw-r--r--   0 runner    (1001) docker     (127)     7902 2024-04-15 17:24:03.000000 pub_tools-5.0.3/pub/tools/tests/test_formatting.py
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-15 17:24:03.000000 pub_tools-5.0.3/pub/tools/tests/test_journals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:24:07.481336 pub_tools-5.0.3/pub.tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-15 17:24:07.000000 pub_tools-5.0.3/pub.tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-15 17:24:07.000000 pub_tools-5.0.3/pub.tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 17:24:07.000000 pub_tools-5.0.3/pub.tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-15 17:24:07.000000 pub_tools-5.0.3/pub.tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-15 17:24:07.000000 pub_tools-5.0.3/pub.tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-15 17:24:03.000000 pub_tools-5.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 17:24:07.481336 pub_tools-5.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:22:40.679309 pub_tools-5.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-16 20:22:36.000000 pub_tools-5.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-16 20:22:40.679309 pub_tools-5.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-16 20:22:36.000000 pub_tools-5.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:22:40.671309 pub_tools-5.0.4/pub/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 20:22:36.000000 pub_tools-5.0.4/pub/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:22:40.675309 pub_tools-5.0.4/pub/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-16 20:22:36.000000 pub_tools-5.0.4/pub/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17304 2024-04-16 20:22:36.000000 pub_tools-5.0.4/pub/tools/citations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-16 20:22:36.000000 pub_tools-5.0.4/pub/tools/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-04-16 20:22:36.000000 pub_tools-5.0.4/pub/tools/cooking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22480 2024-04-16 20:22:36.000000 pub_tools-5.0.4/pub/tools/entrez.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8431 2024-04-16 20:22:36.000000 pub_tools-5.0.4/pub/tools/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5380 2024-04-16 20:22:36.000000 pub_tools-5.0.4/pub/tools/isbn.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1443107 2024-04-16 20:22:36.000000 pub_tools-5.0.4/pub/tools/journals.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-04-16 20:22:36.000000 pub_tools-5.0.4/pub/tools/journals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8659 2024-04-16 20:22:36.000000 pub_tools-5.0.4/pub/tools/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:22:40.675309 pub_tools-5.0.4/pub/tools/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-16 20:22:36.000000 pub_tools-5.0.4/pub/tools/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24651 2024-04-16 20:22:36.000000 pub_tools-5.0.4/pub/tools/tests/test_citations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17851 2024-04-16 20:22:36.000000 pub_tools-5.0.4/pub/tools/tests/test_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25839 2024-04-16 20:22:36.000000 pub_tools-5.0.4/pub/tools/tests/test_entrez.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7902 2024-04-16 20:22:36.000000 pub_tools-5.0.4/pub/tools/tests/test_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-16 20:22:36.000000 pub_tools-5.0.4/pub/tools/tests/test_journals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:22:40.675309 pub_tools-5.0.4/pub.tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-16 20:22:40.000000 pub_tools-5.0.4/pub.tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-16 20:22:40.000000 pub_tools-5.0.4/pub.tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 20:22:40.000000 pub_tools-5.0.4/pub.tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-16 20:22:40.000000 pub_tools-5.0.4/pub.tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-16 20:22:40.000000 pub_tools-5.0.4/pub.tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-16 20:22:36.000000 pub_tools-5.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 20:22:40.679309 pub_tools-5.0.4/setup.cfg
```

### Comparing `pub_tools-5.0.3/PKG-INFO` & `pub_tools-5.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pub.tools
-Version: 5.0.3
+Version: 5.0.4
 Summary: Get publication metadata from NCBI's eUtils and generate citations.
 Author-email: Eric Wohnlich <wohnlice@imsweb.com>
 License: GPL
 Project-URL: homepage, https://github.com/imsweb/pub.tools
 Project-URL: documentation, https://imsweb.github.io/pub.tools
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `pub_tools-5.0.3/README.md` & `pub_tools-5.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pub_tools-5.0.3/pub/tools/citations.py` & `pub_tools-5.0.4/pub/tools/citations.py`

 * *Files identical despite different names*

### Comparing `pub_tools-5.0.3/pub/tools/cooking.py` & `pub_tools-5.0.4/pub/tools/cooking.py`

 * *Files identical despite different names*

### Comparing `pub_tools-5.0.3/pub/tools/entrez.py` & `pub_tools-5.0.4/pub/tools/entrez.py`

 * *Files 1% similar despite different names*

```diff
@@ -231,16 +231,16 @@
     article_ids = {}
     for aid in articleids:
         article_ids[aid.attributes['IdType']] = aid
 
     grants = []
     for grant in article.get('GrantList', []):
         grants.append(Grant(
-            grantid=grant.get('GrantID'),
-            acronym=grant.get('Acronym'),
+            grantid=grant.get('GrantID', ''),
+            acronym=grant.get('Acronym', ''),
             agency=grant.get('Agency', ''))
         )
     mesh = []
     for meshHeader in medline.get('MeshHeadingList', []):
         mesh.append(meshHeader['DescriptorName'])
     pubtypelist = [ptl for ptl in article.get('PublicationTypeList', [])]
     edate = ''
```

### Comparing `pub_tools-5.0.3/pub/tools/formatting.py` & `pub_tools-5.0.4/pub/tools/formatting.py`

 * *Files identical despite different names*

### Comparing `pub_tools-5.0.3/pub/tools/isbn.py` & `pub_tools-5.0.4/pub/tools/isbn.py`

 * *Files identical despite different names*

### Comparing `pub_tools-5.0.3/pub/tools/journals.json` & `pub_tools-5.0.4/pub/tools/journals.json`

 * *Files identical despite different names*

### Comparing `pub_tools-5.0.3/pub/tools/journals.py` & `pub_tools-5.0.4/pub/tools/journals.py`

 * *Files identical despite different names*

### Comparing `pub_tools-5.0.3/pub/tools/schema.py` & `pub_tools-5.0.4/pub/tools/schema.py`

 * *Files identical despite different names*

### Comparing `pub_tools-5.0.3/pub/tools/tests/test_citations.py` & `pub_tools-5.0.4/pub/tools/tests/test_citations.py`

 * *Files identical despite different names*

### Comparing `pub_tools-5.0.3/pub/tools/tests/test_compatibility.py` & `pub_tools-5.0.4/pub/tools/tests/test_compatibility.py`

 * *Files identical despite different names*

### Comparing `pub_tools-5.0.3/pub/tools/tests/test_entrez.py` & `pub_tools-5.0.4/pub/tools/tests/test_entrez.py`

 * *Files identical despite different names*

### Comparing `pub_tools-5.0.3/pub/tools/tests/test_formatting.py` & `pub_tools-5.0.4/pub/tools/tests/test_formatting.py`

 * *Files identical despite different names*

### Comparing `pub_tools-5.0.3/pub/tools/tests/test_journals.py` & `pub_tools-5.0.4/pub/tools/tests/test_journals.py`

 * *Files identical despite different names*

### Comparing `pub_tools-5.0.3/pub.tools.egg-info/PKG-INFO` & `pub_tools-5.0.4/pub.tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pub.tools
-Version: 5.0.3
+Version: 5.0.4
 Summary: Get publication metadata from NCBI's eUtils and generate citations.
 Author-email: Eric Wohnlich <wohnlice@imsweb.com>
 License: GPL
 Project-URL: homepage, https://github.com/imsweb/pub.tools
 Project-URL: documentation, https://imsweb.github.io/pub.tools
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `pub_tools-5.0.3/pub.tools.egg-info/SOURCES.txt` & `pub_tools-5.0.4/pub.tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pub_tools-5.0.3/pyproject.toml` & `pub_tools-5.0.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pub.tools"
-version = "5.0.3"
+version = "5.0.4"
 readme = "README.md"
 requires-python = ">=3.11"
 description = "Get publication metadata from NCBI's eUtils and generate citations."
 classifiers = [
           "Programming Language :: Python :: 3",
           "Topic :: Scientific/Engineering",
           "Topic :: Scientific/Engineering :: Bio-Informatics",
```

