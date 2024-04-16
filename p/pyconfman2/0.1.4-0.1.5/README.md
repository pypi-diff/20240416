# Comparing `tmp/pyconfman2-0.1.4.tar.gz` & `tmp/pyconfman2-0.1.5.tar.gz`

## Comparing `pyconfman2-0.1.4.tar` & `pyconfman2-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 pyconfman2-0.1.4/Devs.md
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 pyconfman2-0.1.4/setup.py
--rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 pyconfman2-0.1.4/.github/workflows/build-and-publish-to-pypi.yml
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 pyconfman2-0.1.4/src/pyconfman2/Exceptions.py
--rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 pyconfman2-0.1.4/src/pyconfman2/Schema.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyconfman2-0.1.4/src/pyconfman2/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyconfman2-0.1.4/tests/__init__.py
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 pyconfman2-0.1.4/tests/config.yaml
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyconfman2-0.1.4/tests/config.yml
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyconfman2-0.1.4/tests/test_default_config.yml
--rw-r--r--   0        0        0     7398 2020-02-02 00:00:00.000000 pyconfman2-0.1.4/tests/test_schema.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 pyconfman2-0.1.4/tests/test_schema_config.yml
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 pyconfman2-0.1.4/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 pyconfman2-0.1.4/LICENSE
--rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 pyconfman2-0.1.4/README.md
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 pyconfman2-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 pyconfman2-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 pyconfman2-0.1.5/Devs.md
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 pyconfman2-0.1.5/setup.py
+-rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 pyconfman2-0.1.5/.github/workflows/build-and-publish-to-pypi.yml
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 pyconfman2-0.1.5/src/pyconfman2/Exceptions.py
+-rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 pyconfman2-0.1.5/src/pyconfman2/Schema.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyconfman2-0.1.5/src/pyconfman2/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyconfman2-0.1.5/tests/__init__.py
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 pyconfman2-0.1.5/tests/config.yaml
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyconfman2-0.1.5/tests/config.yml
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyconfman2-0.1.5/tests/test_default_config.yml
+-rw-r--r--   0        0        0     7398 2020-02-02 00:00:00.000000 pyconfman2-0.1.5/tests/test_schema.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 pyconfman2-0.1.5/tests/test_schema_config.yml
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 pyconfman2-0.1.5/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 pyconfman2-0.1.5/LICENSE
+-rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 pyconfman2-0.1.5/README.md
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 pyconfman2-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 pyconfman2-0.1.5/PKG-INFO
```

### Comparing `pyconfman2-0.1.4/.github/workflows/build-and-publish-to-pypi.yml` & `pyconfman2-0.1.5/.github/workflows/build-and-publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pyconfman2-0.1.4/src/pyconfman2/Schema.py` & `pyconfman2-0.1.5/src/pyconfman2/Schema.py`

 * *Files 11% similar despite different names*

```diff
@@ -57,7 +57,10 @@
         if not os.path.exists(filepath):
             raise FileNotFoundException
         
         with open(filepath, "r") as fh:
             config_file = yaml.safe_load(fh)
         
         self.add(config_file)
+    
+    def items(self):
+        return self.properties.items()
```

### Comparing `pyconfman2-0.1.4/tests/test_schema.py` & `pyconfman2-0.1.5/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `pyconfman2-0.1.4/LICENSE` & `pyconfman2-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyconfman2-0.1.4/README.md` & `pyconfman2-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `pyconfman2-0.1.4/pyproject.toml` & `pyconfman2-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pyconfman2"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
   { name="Phillyp Henning", email="phillyp.henning@gmail.com" },
 ]
 description = "A python package for managing YAML configuration"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `pyconfman2-0.1.4/PKG-INFO` & `pyconfman2-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyconfman2
-Version: 0.1.4
+Version: 0.1.5
 Summary: A python package for managing YAML configuration
 Project-URL: Homepage, https://github.com/PhillypHenning/python-config-parser
 Project-URL: Issues, https://github.com/PhillypHenning/python-config-parser/issues
 Author-email: Phillyp Henning <phillyp.henning@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

