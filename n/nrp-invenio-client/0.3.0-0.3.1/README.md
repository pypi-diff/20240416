# Comparing `tmp/nrp_invenio_client-0.3.0.tar.gz` & `tmp/nrp_invenio_client-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nrp_invenio_client-0.3.0.tar", last modified: Mon Apr 15 13:53:52 2024, max compression
+gzip compressed data, was "nrp_invenio_client-0.3.1.tar", last modified: Tue Apr 16 09:10:27 2024, max compression
```

## Comparing `nrp_invenio_client-0.3.0.tar` & `nrp_invenio_client-0.3.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:53:52.458612 nrp_invenio_client-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-15 13:53:52.458612 nrp_invenio_client-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-15 13:53:06.000000 nrp_invenio_client-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-15 13:53:06.000000 nrp_invenio_client-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 13:53:52.458612 nrp_invenio_client-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:53:52.450612 nrp_invenio_client-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:53:52.454612 nrp_invenio_client-0.3.0/src/nrp_invenio_client/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-15 13:53:06.000000 nrp_invenio_client-0.3.0/src/nrp_invenio_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12096 2024-04-15 13:53:06.000000 nrp_invenio_client-0.3.0/src/nrp_invenio_client/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:53:52.458612 nrp_invenio_client-0.3.0/src/nrp_invenio_client/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-15 13:53:06.000000 nrp_invenio_client-0.3.0/src/nrp_invenio_client/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-04-15 13:53:06.000000 nrp_invenio_client-0.3.0/src/nrp_invenio_client/cli/alias.py
--rw-r--r--   0 runner    (1001) docker     (127)     5562 2024-04-15 13:53:06.000000 nrp_invenio_client-0.3.0/src/nrp_invenio_client/cli/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-04-15 13:53:06.000000 nrp_invenio_client-0.3.0/src/nrp_invenio_client/cli/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-15 13:53:06.000000 nrp_invenio_client-0.3.0/src/nrp_invenio_client/cli/describe.py
--rw-r--r--   0 runner    (1001) docker     (127)     6200 2024-04-15 13:53:06.000000 nrp_invenio_client-0.3.0/src/nrp_invenio_client/cli/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-04-15 13:53:06.000000 nrp_invenio_client-0.3.0/src/nrp_invenio_client/cli/output.py
--rw-r--r--   0 runner    (1001) docker     (127)     8000 2024-04-15 13:53:06.000000 nrp_invenio_client-0.3.0/src/nrp_invenio_client/cli/record.py
--rw-r--r--   0 runner    (1001) docker     (127)     8149 2024-04-15 13:53:06.000000 nrp_invenio_client-0.3.0/src/nrp_invenio_client/cli/requests.py
--rw-r--r--   0 runner    (1001) docker     (127)     4126 2024-04-15 13:53:06.000000 nrp_invenio_client-0.3.0/src/nrp_invenio_client/cli/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-04-15 13:53:06.000000 nrp_invenio_client-0.3.0/src/nrp_invenio_client/cli/set.py
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-15 13:53:06.000000 nrp_invenio_client-0.3.0/src/nrp_invenio_client/cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:53:52.458612 nrp_invenio_client-0.3.0/src/nrp_invenio_client/config/
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-15 13:53:06.000000 nrp_invenio_client-0.3.0/src/nrp_invenio_client/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-15 13:53:06.000000 nrp_invenio_client-0.3.0/src/nrp_invenio_client/config/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-15 13:53:06.000000 nrp_invenio_client-0.3.0/src/nrp_invenio_client/config/repository_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-15 13:53:06.000000 nrp_invenio_client-0.3.0/src/nrp_invenio_client/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-04-15 13:53:06.000000 nrp_invenio_client-0.3.0/src/nrp_invenio_client/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-04-15 13:53:06.000000 nrp_invenio_client-0.3.0/src/nrp_invenio_client/info.py
--rw-r--r--   0 runner    (1001) docker     (127)    10924 2024-04-15 13:53:06.000000 nrp_invenio_client-0.3.0/src/nrp_invenio_client/records.py
--rw-r--r--   0 runner    (1001) docker     (127)     6321 2024-04-15 13:53:06.000000 nrp_invenio_client-0.3.0/src/nrp_invenio_client/requests.py
--rw-r--r--   0 runner    (1001) docker     (127)     6995 2024-04-15 13:53:06.000000 nrp_invenio_client-0.3.0/src/nrp_invenio_client/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     4560 2024-04-15 13:53:06.000000 nrp_invenio_client-0.3.0/src/nrp_invenio_client/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:53:52.458612 nrp_invenio_client-0.3.0/src/nrp_invenio_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-15 13:53:52.000000 nrp_invenio_client-0.3.0/src/nrp_invenio_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-15 13:53:52.000000 nrp_invenio_client-0.3.0/src/nrp_invenio_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 13:53:52.000000 nrp_invenio_client-0.3.0/src/nrp_invenio_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-15 13:53:52.000000 nrp_invenio_client-0.3.0/src/nrp_invenio_client.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-15 13:53:52.000000 nrp_invenio_client-0.3.0/src/nrp_invenio_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-15 13:53:52.000000 nrp_invenio_client-0.3.0/src/nrp_invenio_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:10:27.499879 nrp_invenio_client-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-16 09:10:27.499879 nrp_invenio_client-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-16 09:09:35.000000 nrp_invenio_client-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-16 09:09:35.000000 nrp_invenio_client-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 09:10:27.499879 nrp_invenio_client-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:10:27.491879 nrp_invenio_client-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:10:27.495879 nrp_invenio_client-0.3.1/src/nrp_invenio_client/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-16 09:09:35.000000 nrp_invenio_client-0.3.1/src/nrp_invenio_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12096 2024-04-16 09:09:35.000000 nrp_invenio_client-0.3.1/src/nrp_invenio_client/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:10:27.495879 nrp_invenio_client-0.3.1/src/nrp_invenio_client/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-16 09:09:35.000000 nrp_invenio_client-0.3.1/src/nrp_invenio_client/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-04-16 09:09:35.000000 nrp_invenio_client-0.3.1/src/nrp_invenio_client/cli/alias.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5618 2024-04-16 09:09:35.000000 nrp_invenio_client-0.3.1/src/nrp_invenio_client/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-04-16 09:09:35.000000 nrp_invenio_client-0.3.1/src/nrp_invenio_client/cli/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-16 09:09:35.000000 nrp_invenio_client-0.3.1/src/nrp_invenio_client/cli/describe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6200 2024-04-16 09:09:35.000000 nrp_invenio_client-0.3.1/src/nrp_invenio_client/cli/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-04-16 09:09:35.000000 nrp_invenio_client-0.3.1/src/nrp_invenio_client/cli/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8000 2024-04-16 09:09:35.000000 nrp_invenio_client-0.3.1/src/nrp_invenio_client/cli/record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8149 2024-04-16 09:09:35.000000 nrp_invenio_client-0.3.1/src/nrp_invenio_client/cli/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4126 2024-04-16 09:09:35.000000 nrp_invenio_client-0.3.1/src/nrp_invenio_client/cli/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-04-16 09:09:35.000000 nrp_invenio_client-0.3.1/src/nrp_invenio_client/cli/set.py
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-16 09:09:35.000000 nrp_invenio_client-0.3.1/src/nrp_invenio_client/cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:10:27.495879 nrp_invenio_client-0.3.1/src/nrp_invenio_client/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-16 09:09:35.000000 nrp_invenio_client-0.3.1/src/nrp_invenio_client/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-16 09:09:35.000000 nrp_invenio_client-0.3.1/src/nrp_invenio_client/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-16 09:09:35.000000 nrp_invenio_client-0.3.1/src/nrp_invenio_client/config/repository_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-16 09:09:35.000000 nrp_invenio_client-0.3.1/src/nrp_invenio_client/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-04-16 09:09:35.000000 nrp_invenio_client-0.3.1/src/nrp_invenio_client/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-04-16 09:09:35.000000 nrp_invenio_client-0.3.1/src/nrp_invenio_client/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10924 2024-04-16 09:09:35.000000 nrp_invenio_client-0.3.1/src/nrp_invenio_client/records.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6321 2024-04-16 09:09:35.000000 nrp_invenio_client-0.3.1/src/nrp_invenio_client/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6995 2024-04-16 09:09:35.000000 nrp_invenio_client-0.3.1/src/nrp_invenio_client/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4560 2024-04-16 09:09:35.000000 nrp_invenio_client-0.3.1/src/nrp_invenio_client/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:10:27.499879 nrp_invenio_client-0.3.1/src/nrp_invenio_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-16 09:10:27.000000 nrp_invenio_client-0.3.1/src/nrp_invenio_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-16 09:10:27.000000 nrp_invenio_client-0.3.1/src/nrp_invenio_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 09:10:27.000000 nrp_invenio_client-0.3.1/src/nrp_invenio_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-16 09:10:27.000000 nrp_invenio_client-0.3.1/src/nrp_invenio_client.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-16 09:10:27.000000 nrp_invenio_client-0.3.1/src/nrp_invenio_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-16 09:10:27.000000 nrp_invenio_client-0.3.1/src/nrp_invenio_client.egg-info/top_level.txt
```

### Comparing `nrp_invenio_client-0.3.0/PKG-INFO` & `nrp_invenio_client-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nrp-invenio-client
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python and commandline client for NRP Invenio API
 Author-email: Mirek Simek <miroslav.simek@cesnet.cz>
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: click>=8.1.7
 Requires-Dist: dacite>=1.8.1
```

### Comparing `nrp_invenio_client-0.3.0/README.md` & `nrp_invenio_client-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `nrp_invenio_client-0.3.0/pyproject.toml` & `nrp_invenio_client-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nrp-invenio-client"
-version = "0.3.0"
+version = "0.3.1"
 description = "Python and commandline client for NRP Invenio API"
 authors = [
     {name = "Mirek Simek", email = "miroslav.simek@cesnet.cz"},
 ]
 dependencies = [
     "click>=8.1.7",
     "dacite>=1.8.1",
```

### Comparing `nrp_invenio_client-0.3.0/src/nrp_invenio_client/base.py` & `nrp_invenio_client-0.3.1/src/nrp_invenio_client/base.py`

 * *Files identical despite different names*

### Comparing `nrp_invenio_client-0.3.0/src/nrp_invenio_client/cli/alias.py` & `nrp_invenio_client-0.3.1/src/nrp_invenio_client/cli/alias.py`

 * *Files identical despite different names*

### Comparing `nrp_invenio_client-0.3.0/src/nrp_invenio_client/cli/base.py` & `nrp_invenio_client-0.3.1/src/nrp_invenio_client/cli/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 """,
         fg="yellow",
     )
 
     click.secho(
         """
 nrp-cmd search records       - search for records
-nrp-cmd get record           - 
+nrp-cmd get record           - get a record from the repository, potentially with files
 nrp-cmd describe models      - show information about the models in a repository
     """,
         fg="green",
     )
 
 
 def with_config():
```

### Comparing `nrp_invenio_client-0.3.0/src/nrp_invenio_client/cli/commands.py` & `nrp_invenio_client-0.3.1/src/nrp_invenio_client/cli/commands.py`

 * *Files identical despite different names*

### Comparing `nrp_invenio_client-0.3.0/src/nrp_invenio_client/cli/describe.py` & `nrp_invenio_client-0.3.1/src/nrp_invenio_client/cli/describe.py`

 * *Files identical despite different names*

### Comparing `nrp_invenio_client-0.3.0/src/nrp_invenio_client/cli/files.py` & `nrp_invenio_client-0.3.1/src/nrp_invenio_client/cli/files.py`

 * *Files identical despite different names*

### Comparing `nrp_invenio_client-0.3.0/src/nrp_invenio_client/cli/output.py` & `nrp_invenio_client-0.3.1/src/nrp_invenio_client/cli/output.py`

 * *Files identical despite different names*

### Comparing `nrp_invenio_client-0.3.0/src/nrp_invenio_client/cli/record.py` & `nrp_invenio_client-0.3.1/src/nrp_invenio_client/cli/record.py`

 * *Files identical despite different names*

### Comparing `nrp_invenio_client-0.3.0/src/nrp_invenio_client/cli/requests.py` & `nrp_invenio_client-0.3.1/src/nrp_invenio_client/cli/requests.py`

 * *Files identical despite different names*

### Comparing `nrp_invenio_client-0.3.0/src/nrp_invenio_client/cli/search.py` & `nrp_invenio_client-0.3.1/src/nrp_invenio_client/cli/search.py`

 * *Files identical despite different names*

### Comparing `nrp_invenio_client-0.3.0/src/nrp_invenio_client/cli/set.py` & `nrp_invenio_client-0.3.1/src/nrp_invenio_client/cli/set.py`

 * *Files identical despite different names*

### Comparing `nrp_invenio_client-0.3.0/src/nrp_invenio_client/cli/utils.py` & `nrp_invenio_client-0.3.1/src/nrp_invenio_client/cli/utils.py`

 * *Files identical despite different names*

### Comparing `nrp_invenio_client-0.3.0/src/nrp_invenio_client/config/config.py` & `nrp_invenio_client-0.3.1/src/nrp_invenio_client/config/config.py`

 * *Files identical despite different names*

### Comparing `nrp_invenio_client-0.3.0/src/nrp_invenio_client/errors.py` & `nrp_invenio_client-0.3.1/src/nrp_invenio_client/errors.py`

 * *Files identical despite different names*

### Comparing `nrp_invenio_client-0.3.0/src/nrp_invenio_client/files.py` & `nrp_invenio_client-0.3.1/src/nrp_invenio_client/files.py`

 * *Files identical despite different names*

### Comparing `nrp_invenio_client-0.3.0/src/nrp_invenio_client/info.py` & `nrp_invenio_client-0.3.1/src/nrp_invenio_client/info.py`

 * *Files identical despite different names*

### Comparing `nrp_invenio_client-0.3.0/src/nrp_invenio_client/records.py` & `nrp_invenio_client-0.3.1/src/nrp_invenio_client/records.py`

 * *Files identical despite different names*

### Comparing `nrp_invenio_client-0.3.0/src/nrp_invenio_client/requests.py` & `nrp_invenio_client-0.3.1/src/nrp_invenio_client/requests.py`

 * *Files identical despite different names*

### Comparing `nrp_invenio_client-0.3.0/src/nrp_invenio_client/search.py` & `nrp_invenio_client-0.3.1/src/nrp_invenio_client/search.py`

 * *Files identical despite different names*

### Comparing `nrp_invenio_client-0.3.0/src/nrp_invenio_client/utils.py` & `nrp_invenio_client-0.3.1/src/nrp_invenio_client/utils.py`

 * *Files identical despite different names*

### Comparing `nrp_invenio_client-0.3.0/src/nrp_invenio_client.egg-info/PKG-INFO` & `nrp_invenio_client-0.3.1/src/nrp_invenio_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nrp-invenio-client
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python and commandline client for NRP Invenio API
 Author-email: Mirek Simek <miroslav.simek@cesnet.cz>
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: click>=8.1.7
 Requires-Dist: dacite>=1.8.1
```

### Comparing `nrp_invenio_client-0.3.0/src/nrp_invenio_client.egg-info/SOURCES.txt` & `nrp_invenio_client-0.3.1/src/nrp_invenio_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

