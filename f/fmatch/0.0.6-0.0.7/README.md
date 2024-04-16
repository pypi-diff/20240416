# Comparing `tmp/fmatch-0.0.6.tar.gz` & `tmp/fmatch-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fmatch-0.0.6.tar", last modified: Wed Mar 27 16:19:43 2024, max compression
+gzip compressed data, was "fmatch-0.0.7.tar", last modified: Tue Apr 16 16:37:47 2024, max compression
```

## Comparing `fmatch-0.0.6.tar` & `fmatch-0.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:19:43.284663 fmatch-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-27 16:19:27.000000 fmatch-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-03-27 16:19:43.280663 fmatch-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-03-27 16:19:27.000000 fmatch-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:19:43.280663 fmatch-0.0.6/fmatch/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-03-27 16:19:27.000000 fmatch-0.0.6/fmatch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9610 2024-03-27 16:19:27.000000 fmatch-0.0.6/fmatch/matcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-03-27 16:19:27.000000 fmatch-0.0.6/fmatch/test_fmatch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:19:43.280663 fmatch-0.0.6/fmatch/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-27 16:19:27.000000 fmatch-0.0.6/fmatch/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9323 2024-03-27 16:19:27.000000 fmatch-0.0.6/fmatch/tests/test_matcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:19:43.280663 fmatch-0.0.6/fmatch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-03-27 16:19:43.000000 fmatch-0.0.6/fmatch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-03-27 16:19:43.000000 fmatch-0.0.6/fmatch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 16:19:43.000000 fmatch-0.0.6/fmatch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-27 16:19:43.000000 fmatch-0.0.6/fmatch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-27 16:19:43.000000 fmatch-0.0.6/fmatch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 16:19:43.284663 fmatch-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-03-27 16:19:27.000000 fmatch-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:37:47.140995 fmatch-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-16 16:37:33.000000 fmatch-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-16 16:37:47.140995 fmatch-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-16 16:37:33.000000 fmatch-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:37:47.140995 fmatch-0.0.7/fmatch/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-16 16:37:33.000000 fmatch-0.0.7/fmatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9655 2024-04-16 16:37:33.000000 fmatch-0.0.7/fmatch/matcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-04-16 16:37:33.000000 fmatch-0.0.7/fmatch/test_fmatch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:37:47.140995 fmatch-0.0.7/fmatch/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-16 16:37:33.000000 fmatch-0.0.7/fmatch/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9339 2024-04-16 16:37:33.000000 fmatch-0.0.7/fmatch/tests/test_matcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:37:47.140995 fmatch-0.0.7/fmatch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-16 16:37:47.000000 fmatch-0.0.7/fmatch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-16 16:37:47.000000 fmatch-0.0.7/fmatch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 16:37:47.000000 fmatch-0.0.7/fmatch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-16 16:37:47.000000 fmatch-0.0.7/fmatch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-16 16:37:47.000000 fmatch-0.0.7/fmatch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 16:37:47.140995 fmatch-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-16 16:37:33.000000 fmatch-0.0.7/setup.py
```

### Comparing `fmatch-0.0.6/LICENSE` & `fmatch-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fmatch-0.0.6/PKG-INFO` & `fmatch-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fmatch
-Version: 0.0.6
+Version: 0.0.7
 Summary: Common package for matching runs with provided metadata
 Author: sboyapal
 Author-email: sboyapal@redhat.com
 Keywords: python,matching,red hat,perf-scale,matcher,orion
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fmatch-0.0.6/fmatch/matcher.py` & `fmatch-0.0.7/fmatch/matcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,18 @@
 from elasticsearch_dsl import Search, Q
 
 
 class Matcher:
     """Matcher"""
 
     def __init__(
-        self, index="perf_scale_ci", level=logging.INFO, ES_URL=os.getenv("ES_SERVER")
+        self, index="ospst-perf-scale-ci",
+        level=logging.INFO,
+        ES_URL=os.getenv("ES_SERVER"),
+        verify_certs=True
     ):
         self.index = index
         self.es_url = ES_URL
         self.search_size = 10000
         self.logger = logging.getLogger("Matcher")
         self.logger.setLevel(level)
         handler = logging.StreamHandler(sys.stdout)
@@ -31,15 +34,15 @@
         formatter = logging.Formatter(
             "%(asctime)s - %(name)s - %(levelname)s - %(message)s"
         )
         handler.setFormatter(formatter)
         self.logger.addHandler(handler)
         # We can set the ES logging higher if we want additional debugging
         logging.getLogger("elasticsearch").setLevel(logging.WARN)
-        self.es = Elasticsearch([self.es_url], timeout=30)
+        self.es = Elasticsearch([self.es_url], timeout=30, verify_certs=verify_certs)
         self.data = None
 
     def get_metadata_by_uuid(self, uuid, index=None):
         """Returns back metadata when uuid is given
 
         Args:
             uuid (str): uuid of the run
@@ -92,22 +95,21 @@
         s = Search(using=self.es, index=index).query(query).extra(size=self.search_size)
         result = self.query_index(index, s)
         hits = result.hits.hits
         uuids_docs = [{ "uuid":hit.to_dict()["_source"]["uuid"],
                         "buildUrl":hit.to_dict()["_source"]["buildUrl"]} for hit in hits]
         return uuids_docs
 
-    def match_kube_burner(self, uuids):
+    def match_kube_burner(self, uuids, index):
         """match kube burner runs
         Args:
             uuids (list): list of uuids
         Returns:
             list : list of runs
         """
-        index = "ripsaw-kube-burner*"
         query = Q(
             "bool",
             filter=[
                 Q("terms", **{"uuid.keyword": uuids}),
                 Q("match", metricName="jobSummary"),
                 ~Q("match", **{"jobConfig.name": "garbage-collection"}),
             ],
```

### Comparing `fmatch-0.0.6/fmatch/test_fmatch.py` & `fmatch-0.0.7/fmatch/test_fmatch.py`

 * *Files identical despite different names*

### Comparing `fmatch-0.0.6/fmatch/tests/test_matcher.py` & `fmatch-0.0.7/fmatch/tests/test_matcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
                 "buildUrl":"buildUrl1"},
                 {"uuid": "uuid2",
                 "buildUrl":"buildUrl1"}]
     assert result == expected
 
 
 def test_match_kube_burner(matcher_instance):
-    result = matcher_instance.match_kube_burner(["uuid1"])
+    result = matcher_instance.match_kube_burner(["uuid1"],index="ospst-*")
     expected = [
         {"uuid": "uuid1", "field1": "value1"},
         {"uuid": "uuid2", "field1": "value2"},
     ]
     assert result == expected
```

### Comparing `fmatch-0.0.6/fmatch.egg-info/PKG-INFO` & `fmatch-0.0.7/fmatch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fmatch
-Version: 0.0.6
+Version: 0.0.7
 Summary: Common package for matching runs with provided metadata
 Author: sboyapal
 Author-email: sboyapal@redhat.com
 Keywords: python,matching,red hat,perf-scale,matcher,orion
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fmatch-0.0.6/setup.py` & `fmatch-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 setup file for fmatch package
 """
 from setuptools import setup, find_packages
 
 
-VERSION = '0.0.6'
+VERSION = '0.0.7'
 DESCRIPTION = 'Common package for matching runs with provided metadata'
 # pylint: disable= line-too-long
 LONG_DESCRIPTION = "A package that allows to match metadata and get runs and create csv files with queried metrics"
 
 # Setting up
 setup(
     name="fmatch",
```

