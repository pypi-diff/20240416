# Comparing `tmp/pythia_client-0.1.6.tar.gz` & `tmp/pythia_client-0.1.7.tar.gz`

## Comparing `pythia_client-0.1.6.tar` & `pythia_client-0.1.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 pythia_client-0.1.6/.python-version
--rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 pythia_client-0.1.6/CHANGELOG.md
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 pythia_client-0.1.6/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pythia_client-0.1.6/src/pythia_client/__init__.py
--rw-r--r--   0        0        0    20766 2020-02-02 00:00:00.000000 pythia_client-0.1.6/src/pythia_client/client.py
--rw-r--r--   0        0        0     6153 2020-02-02 00:00:00.000000 pythia_client-0.1.6/src/pythia_client/schema.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pythia_client-0.1.6/test/__init__.py
--rw-r--r--   0        0        0     8795 2020-02-02 00:00:00.000000 pythia_client-0.1.6/test/test_client.py
--rw-r--r--   0        0        0    26093 2020-02-02 00:00:00.000000 pythia_client-0.1.6/test/samples/sample1.pdf
--rw-r--r--   0        0        0   217237 2020-02-02 00:00:00.000000 pythia_client-0.1.6/test/samples/sample2.pdf
--rw-r--r--   0        0        0    21457 2020-02-02 00:00:00.000000 pythia_client-0.1.6/test/samples/sample3.pdf
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 pythia_client-0.1.6/.gitignore
--rw-r--r--   0        0        0    11343 2020-02-02 00:00:00.000000 pythia_client-0.1.6/LICENSE
--rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 pythia_client-0.1.6/README.md
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 pythia_client-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     3046 2020-02-02 00:00:00.000000 pythia_client-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 pythia_client-0.1.7/.python-version
+-rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 pythia_client-0.1.7/CHANGELOG.md
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 pythia_client-0.1.7/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pythia_client-0.1.7/src/pythia_client/__init__.py
+-rw-r--r--   0        0        0    20766 2020-02-02 00:00:00.000000 pythia_client-0.1.7/src/pythia_client/client.py
+-rw-r--r--   0        0        0     6221 2020-02-02 00:00:00.000000 pythia_client-0.1.7/src/pythia_client/schema.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pythia_client-0.1.7/test/__init__.py
+-rw-r--r--   0        0        0     8795 2020-02-02 00:00:00.000000 pythia_client-0.1.7/test/test_client.py
+-rw-r--r--   0        0        0    26093 2020-02-02 00:00:00.000000 pythia_client-0.1.7/test/samples/sample1.pdf
+-rw-r--r--   0        0        0   217237 2020-02-02 00:00:00.000000 pythia_client-0.1.7/test/samples/sample2.pdf
+-rw-r--r--   0        0        0    21457 2020-02-02 00:00:00.000000 pythia_client-0.1.7/test/samples/sample3.pdf
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 pythia_client-0.1.7/.gitignore
+-rw-r--r--   0        0        0    11343 2020-02-02 00:00:00.000000 pythia_client-0.1.7/LICENSE
+-rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 pythia_client-0.1.7/README.md
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 pythia_client-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     3046 2020-02-02 00:00:00.000000 pythia_client-0.1.7/PKG-INFO
```

### Comparing `pythia_client-0.1.6/CHANGELOG.md` & `pythia_client-0.1.7/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+#### v0.1.7
+- MetaJSON schema fix for Mistral models. Compatible with `haystack-api` v0.2.2
+
 #### v0.1.6
 - New intent functions: add_intent, predict_intent, delete_intent. Compatible with `haystack-api` v0.2.1
 
 #### v0.1.4
 - Minor ESR Ticket schema fix
 
 #### v0.1.3
```

### Comparing `pythia_client-0.1.6/src/pythia_client/client.py` & `pythia_client-0.1.7/src/pythia_client/client.py`

 * *Files identical despite different names*

### Comparing `pythia_client-0.1.6/src/pythia_client/schema.py` & `pythia_client-0.1.7/src/pythia_client/schema.py`

 * *Files 6% similar despite different names*

```diff
@@ -162,18 +162,18 @@
 
 class UsageJSON(BaseModel):
     input_tokens: int
     output_tokens: int
 
 
 class MetaJSON(BaseModel):
-    id: str
-    model: str
-    usage: UsageJSON
-    stop_reason: str
+    id: Optional[str] = None
+    model: Optional[str] = None
+    usage: Optional[UsageJSON] = None
+    stop_reason: Optional[str] = None
     stop_sequence: Optional[str] = None
 
 
 class ValidatedItem(BaseModel):
     content: str
     role: str = "assistant"
     name: Optional[str] = None
```

### Comparing `pythia_client-0.1.6/test/test_client.py` & `pythia_client-0.1.7/test/test_client.py`

 * *Files identical despite different names*

### Comparing `pythia_client-0.1.6/test/samples/sample1.pdf` & `pythia_client-0.1.7/test/samples/sample1.pdf`

 * *Files identical despite different names*

### Comparing `pythia_client-0.1.6/test/samples/sample2.pdf` & `pythia_client-0.1.7/test/samples/sample2.pdf`

 * *Files identical despite different names*

### Comparing `pythia_client-0.1.6/test/samples/sample3.pdf` & `pythia_client-0.1.7/test/samples/sample3.pdf`

 * *Files identical despite different names*

### Comparing `pythia_client-0.1.6/LICENSE` & `pythia_client-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pythia_client-0.1.6/README.md` & `pythia_client-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `pythia_client-0.1.6/pyproject.toml` & `pythia_client-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pythia-client"
-version = "0.1.6"
+version = "0.1.7"
 dependencies = [
     "requests>=2.31",
     "pydantic>=2.6",
 ]
 requires-python = ">=3.11"
 authors = [
   {name = "Corentin Meyer", email = "contact@cmeyer.fr"},
```

### Comparing `pythia_client-0.1.6/PKG-INFO` & `pythia_client-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pythia-client
-Version: 0.1.6
+Version: 0.1.7
 Summary: Client to interact with the Pythia API
 Project-URL: Homepage, https://gitlab.com/ale-gitlab/dto/data-science/cip-bot/project-pythia
 Project-URL: Documentation, https://gitlab.com/ale-gitlab/dto/data-science/cip-bot/project-pythia
 Project-URL: Repository, https://gitlab.com/ale-gitlab/dto/data-science/cip-bot/project-pythia
 Project-URL: Issues, https://gitlab.com/ale-gitlab/dto/data-science/cip-bot/project-pythia/-/issues
 Author-email: Corentin Meyer <contact@cmeyer.fr>
 Maintainer-email: Corentin Meyer <contact@cmeyer.fr>
```

