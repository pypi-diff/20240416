# Comparing `tmp/pyuniprotkb-0.4.0.tar.gz` & `tmp/pyuniprotkb-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyuniprotkb-0.4.0.tar", last modified: Tue Apr 16 16:09:57 2024, max compression
+gzip compressed data, was "pyuniprotkb-0.4.1.tar", last modified: Tue Apr 16 16:17:51 2024, max compression
```

## Comparing `pyuniprotkb-0.4.0.tar` & `pyuniprotkb-0.4.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:09:57.469540 pyuniprotkb-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-16 16:09:49.000000 pyuniprotkb-0.4.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-16 16:09:49.000000 pyuniprotkb-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-16 16:09:49.000000 pyuniprotkb-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4574 2024-04-16 16:09:57.469540 pyuniprotkb-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3832 2024-04-16 16:09:49.000000 pyuniprotkb-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-16 16:09:49.000000 pyuniprotkb-0.4.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:09:57.465540 pyuniprotkb-0.4.0/pyuniprot/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-16 16:09:49.000000 pyuniprotkb-0.4.0/pyuniprot/CC.py
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-16 16:09:49.000000 pyuniprotkb-0.4.0/pyuniprot/DB.py
--rw-r--r--   0 runner    (1001) docker     (127)     9087 2024-04-16 16:09:49.000000 pyuniprotkb-0.4.0/pyuniprot/UniRef.py
--rw-r--r--   0 runner    (1001) docker     (127)    30664 2024-04-16 16:09:49.000000 pyuniprotkb-0.4.0/pyuniprot/Uniprot.py
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-16 16:09:49.000000 pyuniprotkb-0.4.0/pyuniprot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 16:09:49.000000 pyuniprotkb-0.4.0/pyuniprot/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:09:57.465540 pyuniprotkb-0.4.0/pyuniprot/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-16 16:09:49.000000 pyuniprotkb-0.4.0/pyuniprot/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9824 2024-04-16 16:09:49.000000 pyuniprotkb-0.4.0/pyuniprot/utils/isoforms.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-16 16:09:49.000000 pyuniprotkb-0.4.0/pyuniprot/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:09:57.469540 pyuniprotkb-0.4.0/pyuniprotkb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4574 2024-04-16 16:09:57.000000 pyuniprotkb-0.4.0/pyuniprotkb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-16 16:09:57.000000 pyuniprotkb-0.4.0/pyuniprotkb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 16:09:57.000000 pyuniprotkb-0.4.0/pyuniprotkb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-16 16:09:57.000000 pyuniprotkb-0.4.0/pyuniprotkb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-16 16:09:57.000000 pyuniprotkb-0.4.0/pyuniprotkb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-16 16:09:49.000000 pyuniprotkb-0.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-16 16:09:49.000000 pyuniprotkb-0.4.0/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-16 16:09:57.469540 pyuniprotkb-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-16 16:09:49.000000 pyuniprotkb-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:09:57.469540 pyuniprotkb-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 16:09:49.000000 pyuniprotkb-0.4.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-16 16:09:49.000000 pyuniprotkb-0.4.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-04-16 16:09:49.000000 pyuniprotkb-0.4.0/tests/test_isoforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     4045 2024-04-16 16:09:49.000000 pyuniprotkb-0.4.0/tests/test_uniprot.py
--rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-04-16 16:09:49.000000 pyuniprotkb-0.4.0/tests/test_uniref.py
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-16 16:09:49.000000 pyuniprotkb-0.4.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:17:51.453887 pyuniprotkb-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-16 16:17:42.000000 pyuniprotkb-0.4.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-16 16:17:42.000000 pyuniprotkb-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-16 16:17:42.000000 pyuniprotkb-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4538 2024-04-16 16:17:51.453887 pyuniprotkb-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3832 2024-04-16 16:17:42.000000 pyuniprotkb-0.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-16 16:17:42.000000 pyuniprotkb-0.4.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:17:51.449887 pyuniprotkb-0.4.1/pyuniprot/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-16 16:17:42.000000 pyuniprotkb-0.4.1/pyuniprot/CC.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-16 16:17:42.000000 pyuniprotkb-0.4.1/pyuniprot/DB.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9087 2024-04-16 16:17:42.000000 pyuniprotkb-0.4.1/pyuniprot/UniRef.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30664 2024-04-16 16:17:42.000000 pyuniprotkb-0.4.1/pyuniprot/Uniprot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-16 16:17:42.000000 pyuniprotkb-0.4.1/pyuniprot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 16:17:42.000000 pyuniprotkb-0.4.1/pyuniprot/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:17:51.449887 pyuniprotkb-0.4.1/pyuniprot/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-16 16:17:42.000000 pyuniprotkb-0.4.1/pyuniprot/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9824 2024-04-16 16:17:42.000000 pyuniprotkb-0.4.1/pyuniprot/utils/isoforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-16 16:17:42.000000 pyuniprotkb-0.4.1/pyuniprot/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:17:51.453887 pyuniprotkb-0.4.1/pyuniprotkb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4538 2024-04-16 16:17:51.000000 pyuniprotkb-0.4.1/pyuniprotkb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-16 16:17:51.000000 pyuniprotkb-0.4.1/pyuniprotkb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 16:17:51.000000 pyuniprotkb-0.4.1/pyuniprotkb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-16 16:17:51.000000 pyuniprotkb-0.4.1/pyuniprotkb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-16 16:17:51.000000 pyuniprotkb-0.4.1/pyuniprotkb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 16:17:42.000000 pyuniprotkb-0.4.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-16 16:17:42.000000 pyuniprotkb-0.4.1/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-16 16:17:51.453887 pyuniprotkb-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-16 16:17:42.000000 pyuniprotkb-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:17:51.453887 pyuniprotkb-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 16:17:42.000000 pyuniprotkb-0.4.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-16 16:17:42.000000 pyuniprotkb-0.4.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-04-16 16:17:42.000000 pyuniprotkb-0.4.1/tests/test_isoforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4045 2024-04-16 16:17:42.000000 pyuniprotkb-0.4.1/tests/test_uniprot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-04-16 16:17:42.000000 pyuniprotkb-0.4.1/tests/test_uniref.py
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-16 16:17:42.000000 pyuniprotkb-0.4.1/tox.ini
```

### Comparing `pyuniprotkb-0.4.0/.pre-commit-config.yaml` & `pyuniprotkb-0.4.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pyuniprotkb-0.4.0/LICENSE` & `pyuniprotkb-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyuniprotkb-0.4.0/PKG-INFO` & `pyuniprotkb-0.4.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: pyuniprotkb
-Version: 0.4.0
+Version: 0.4.1
 Summary: A python package to retrieve bioinformatics given Uniprot IDs.
 Home-page: https://github.com/Ruibin-Liu/pyuniprot
 Author: Ruibin Liu
 Author-email: ruibinliuphd@gmail.com
 Project-URL: Bug Tracker, https://github.com/Ruibin-Liu/pyuniprot/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: beautifulsoup4>=4.12
 Provides-Extra: testing
 Requires-Dist: tox>=3.24; extra == "testing"
 Requires-Dist: pytest>=7.0; extra == "testing"
 Requires-Dist: pytest-cov>=3.0; extra == "testing"
 
 # pyuniprot
 `pyuniprot` parses a UniProt text file given a Uniprot ID into a python object. All information is made programmatically accessible when programming in python, the most used programming language in bioinformatics.
```

### Comparing `pyuniprotkb-0.4.0/README.md` & `pyuniprotkb-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pyuniprotkb-0.4.0/pyuniprot/DB.py` & `pyuniprotkb-0.4.1/pyuniprot/DB.py`

 * *Files identical despite different names*

### Comparing `pyuniprotkb-0.4.0/pyuniprot/UniRef.py` & `pyuniprotkb-0.4.1/pyuniprot/UniRef.py`

 * *Files identical despite different names*

### Comparing `pyuniprotkb-0.4.0/pyuniprot/Uniprot.py` & `pyuniprotkb-0.4.1/pyuniprot/Uniprot.py`

 * *Files identical despite different names*

### Comparing `pyuniprotkb-0.4.0/pyuniprot/utils/isoforms.py` & `pyuniprotkb-0.4.1/pyuniprot/utils/isoforms.py`

 * *Files identical despite different names*

### Comparing `pyuniprotkb-0.4.0/pyuniprotkb.egg-info/PKG-INFO` & `pyuniprotkb-0.4.1/pyuniprotkb.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: pyuniprotkb
-Version: 0.4.0
+Version: 0.4.1
 Summary: A python package to retrieve bioinformatics given Uniprot IDs.
 Home-page: https://github.com/Ruibin-Liu/pyuniprot
 Author: Ruibin Liu
 Author-email: ruibinliuphd@gmail.com
 Project-URL: Bug Tracker, https://github.com/Ruibin-Liu/pyuniprot/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: beautifulsoup4>=4.12
 Provides-Extra: testing
 Requires-Dist: tox>=3.24; extra == "testing"
 Requires-Dist: pytest>=7.0; extra == "testing"
 Requires-Dist: pytest-cov>=3.0; extra == "testing"
 
 # pyuniprot
 `pyuniprot` parses a UniProt text file given a Uniprot ID into a python object. All information is made programmatically accessible when programming in python, the most used programming language in bioinformatics.
```

### Comparing `pyuniprotkb-0.4.0/pyuniprotkb.egg-info/SOURCES.txt` & `pyuniprotkb-0.4.1/pyuniprotkb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyuniprotkb-0.4.0/setup.py` & `pyuniprotkb-0.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `pyuniprotkb-0.4.0/tests/test_isoforms.py` & `pyuniprotkb-0.4.1/tests/test_isoforms.py`

 * *Files identical despite different names*

### Comparing `pyuniprotkb-0.4.0/tests/test_uniprot.py` & `pyuniprotkb-0.4.1/tests/test_uniprot.py`

 * *Files identical despite different names*

### Comparing `pyuniprotkb-0.4.0/tests/test_uniref.py` & `pyuniprotkb-0.4.1/tests/test_uniref.py`

 * *Files identical despite different names*

