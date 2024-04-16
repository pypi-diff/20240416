# Comparing `tmp/uk_election_ids-0.7.5.tar.gz` & `tmp/uk_election_ids-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uk_election_ids-0.7.5.tar", last modified: Fri Aug  4 08:03:29 2023, max compression
+gzip compressed data, was "uk_election_ids-0.8.0.tar", last modified: Tue Apr 16 06:59:27 2024, max compression
```

## Comparing `uk_election_ids-0.7.5.tar` & `uk_election_ids-0.8.0.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:03:29.630542 uk_election_ids-0.7.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-04 08:03:14.000000 uk_election_ids-0.7.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-04 08:03:14.000000 uk_election_ids-0.7.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-08-04 08:03:29.630542 uk_election_ids-0.7.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-08-04 08:03:14.000000 uk_election_ids-0.7.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 08:03:29.630542 uk_election_ids-0.7.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-08-04 08:03:14.000000 uk_election_ids-0.7.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:03:29.626542 uk_election_ids-0.7.5/uk_election_ids/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 08:03:14.000000 uk_election_ids-0.7.5/uk_election_ids/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:03:29.630542 uk_election_ids-0.7.5/uk_election_ids/data/
--rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-08-04 08:03:14.000000 uk_election_ids-0.7.5/uk_election_ids/data/id_requirements.json
--rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-08-04 08:03:14.000000 uk_election_ids-0.7.5/uk_election_ids/data/voting_systems.json
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-08-04 08:03:14.000000 uk_election_ids-0.7.5/uk_election_ids/datapackage.py
--rw-r--r--   0 runner    (1001) docker     (123)    13999 2023-08-04 08:03:14.000000 uk_election_ids-0.7.5/uk_election_ids/election_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     4580 2023-08-04 08:03:14.000000 uk_election_ids-0.7.5/uk_election_ids/metadata_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-08-04 08:03:14.000000 uk_election_ids-0.7.5/uk_election_ids/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-08-04 08:03:14.000000 uk_election_ids-0.7.5/uk_election_ids/slugger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:03:29.630542 uk_election_ids-0.7.5/uk_election_ids.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-08-04 08:03:29.000000 uk_election_ids-0.7.5/uk_election_ids.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-08-04 08:03:29.000000 uk_election_ids-0.7.5/uk_election_ids.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 08:03:29.000000 uk_election_ids-0.7.5/uk_election_ids.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-08-04 08:03:29.000000 uk_election_ids-0.7.5/uk_election_ids.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-04 08:03:29.000000 uk_election_ids-0.7.5/uk_election_ids.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:59:27.672234 uk_election_ids-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-16 06:59:22.000000 uk_election_ids-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-16 06:59:22.000000 uk_election_ids-0.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-04-16 06:59:27.672234 uk_election_ids-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-16 06:59:22.000000 uk_election_ids-0.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-16 06:59:22.000000 uk_election_ids-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 06:59:27.672234 uk_election_ids-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-04-16 06:59:22.000000 uk_election_ids-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:59:27.668234 uk_election_ids-0.8.0/uk_election_ids/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 06:59:22.000000 uk_election_ids-0.8.0/uk_election_ids/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:59:27.668234 uk_election_ids-0.8.0/uk_election_ids/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-04-16 06:59:22.000000 uk_election_ids-0.8.0/uk_election_ids/data/id_requirements.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-04-16 06:59:22.000000 uk_election_ids-0.8.0/uk_election_ids/data/postal_votes.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-04-16 06:59:22.000000 uk_election_ids-0.8.0/uk_election_ids/data/voting_systems.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-04-16 06:59:22.000000 uk_election_ids-0.8.0/uk_election_ids/datapackage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13999 2024-04-16 06:59:22.000000 uk_election_ids-0.8.0/uk_election_ids/election_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5216 2024-04-16 06:59:22.000000 uk_election_ids-0.8.0/uk_election_ids/metadata_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-16 06:59:22.000000 uk_election_ids-0.8.0/uk_election_ids/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-16 06:59:22.000000 uk_election_ids-0.8.0/uk_election_ids/slugger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:59:27.668234 uk_election_ids-0.8.0/uk_election_ids.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-04-16 06:59:27.000000 uk_election_ids-0.8.0/uk_election_ids.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-16 06:59:27.000000 uk_election_ids-0.8.0/uk_election_ids.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 06:59:27.000000 uk_election_ids-0.8.0/uk_election_ids.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-16 06:59:27.000000 uk_election_ids-0.8.0/uk_election_ids.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-16 06:59:27.000000 uk_election_ids-0.8.0/uk_election_ids.egg-info/top_level.txt
```

### Comparing `uk_election_ids-0.7.5/LICENSE` & `uk_election_ids-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `uk_election_ids-0.7.5/PKG-INFO` & `uk_election_ids-0.8.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 Metadata-Version: 2.1
 Name: uk_election_ids
-Version: 0.7.5
+Version: 0.8.0
 Summary: Create Democracy Club Election Identifiers
 Home-page: https://github.com/DemocracyClub/uk-election-ids/
 Author: chris48s
 License: MIT
 Project-URL: Documentation, https://democracyclub.github.io/uk-election-ids/
 Project-URL: Source, https://github.com/DemocracyClub/uk-election-ids/
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Provides-Extra: testing
+Requires-Dist: coveralls; extra == "testing"
 Provides-Extra: development
-License-File: LICENSE
+Requires-Dist: sphinx; extra == "development"
+Requires-Dist: sphinx_rtd_theme; extra == "development"
+Requires-Dist: ghp-import; extra == "development"
+Requires-Dist: pydantic; extra == "development"
+Requires-Dist: black==23.3.0; extra == "development"
+Requires-Dist: ruff==0.0.261; extra == "development"
 
 # UK Election IDs
 
 Create and validate Democracy Club Election Identifiers.
 
 ---
```

### Comparing `uk_election_ids-0.7.5/README.md` & `uk_election_ids-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `uk_election_ids-0.7.5/setup.py` & `uk_election_ids-0.8.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
             return f.read()
     except IOError:
         return ""
 
 
 setup(
     name="uk_election_ids",
-    version="0.7.5",
+    version="0.8.0",
     author="chris48s",
     license="MIT",
     url="https://github.com/DemocracyClub/uk-election-ids/",
     packages=["uk_election_ids"],
     package_data={"uk_election_ids": ["data/*.json"]},
     description="Create Democracy Club Election Identifiers",
     long_description=_get_description(),
```

### Comparing `uk_election_ids-0.7.5/uk_election_ids/data/id_requirements.json` & `uk_election_ids-0.8.0/uk_election_ids/data/id_requirements.json`

 * *Files identical despite different names*

### Comparing `uk_election_ids-0.7.5/uk_election_ids/data/voting_systems.json` & `uk_election_ids-0.8.0/uk_election_ids/data/voting_systems.json`

 * *Files identical despite different names*

### Comparing `uk_election_ids-0.7.5/uk_election_ids/datapackage.py` & `uk_election_ids-0.8.0/uk_election_ids/datapackage.py`

 * *Files identical despite different names*

### Comparing `uk_election_ids-0.7.5/uk_election_ids/election_ids.py` & `uk_election_ids-0.8.0/uk_election_ids/election_ids.py`

 * *Files identical despite different names*

### Comparing `uk_election_ids-0.7.5/uk_election_ids/metadata_tools.py` & `uk_election_ids-0.8.0/uk_election_ids/metadata_tools.py`

 * *Files 14% similar despite different names*

```diff
@@ -37,16 +37,15 @@
         \. represents a literal '.', always present at the start of a wildcard
         (\..*) captures a sequence of "[any characters]."
         ? captures a group between 0-1 times
         """
         id_part = id_part.replace(
             "-", r"\-"
         )  # prevent '-' from being interpreted as range indicator
-        id_part = id_part.replace(".*.", r"\.(.*\.)?")
-        return id_part
+        return id_part.replace(".*.", r"\.(.*\.)?")
 
     def match_id(self):
         """
         Match the most specific key to this ID
 
         """
         ids_with_defaults = self.DATA["defaults"].keys()
@@ -121,13 +120,33 @@
         id_part, data = self.match_id()
         if self.nation and self.nation in data.get("nations", {}):
             data = data["nations"][self.nation]
 
         if data.get("dates"):
             data = self.match_dates(data["dates"])
 
+        default = data.get("default", "")
+        if default == "":
+            required_keys = data.keys()
+            raise ValueError(f"{id_part} requires {' or '.join(required_keys)}")
+
+        return data["default"]
+
+
+class PostalVotingRequirementsMatcher(MetaDataMatcher):
+    path = Path(__file__).parent / "data" / "postal_votes.json"
+    DATA = json.load(path.open())
+
+    def get_postal_voting_requirements(self):
+        id_part, data = self.match_id()
+        if self.nation and self.nation in data.get("nations", {}):
+            data = data["nations"][self.nation]
+
+        if data.get("dates"):
+            data = self.match_dates(data["dates"])
+
         default = data.get("default", "")
         if default == "":
             required_keys = data.keys()
             raise ValueError(f"{id_part} requires {' or '.join(required_keys)}")
 
         return data["default"]
```

### Comparing `uk_election_ids-0.7.5/uk_election_ids/parser.py` & `uk_election_ids-0.8.0/uk_election_ids/parser.py`

 * *Files identical despite different names*

### Comparing `uk_election_ids-0.7.5/uk_election_ids/slugger.py` & `uk_election_ids-0.8.0/uk_election_ids/slugger.py`

 * *Files identical despite different names*

