# Comparing `tmp/pyuniprotkb-0.2.0.tar.gz` & `tmp/pyuniprotkb-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyuniprotkb-0.2.0.tar", last modified: Wed Mar 13 01:42:26 2024, max compression
+gzip compressed data, was "pyuniprotkb-0.3.0.tar", last modified: Mon Apr 15 20:33:24 2024, max compression
```

## Comparing `pyuniprotkb-0.2.0.tar` & `pyuniprotkb-0.3.0.tar`

### file list

```diff
@@ -1,33 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 01:42:26.682778 pyuniprotkb-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-03-13 01:42:19.000000 pyuniprotkb-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-03-13 01:42:19.000000 pyuniprotkb-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-03-13 01:42:19.000000 pyuniprotkb-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-03-13 01:42:26.682778 pyuniprotkb-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-03-13 01:42:19.000000 pyuniprotkb-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-03-13 01:42:19.000000 pyuniprotkb-0.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 01:42:26.678778 pyuniprotkb-0.2.0/pyuniprot/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-13 01:42:19.000000 pyuniprotkb-0.2.0/pyuniprot/CC.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-03-13 01:42:19.000000 pyuniprotkb-0.2.0/pyuniprot/DB.py
--rw-r--r--   0 runner    (1001) docker     (127)    25902 2024-03-13 01:42:19.000000 pyuniprotkb-0.2.0/pyuniprot/Uniprot.py
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-03-13 01:42:19.000000 pyuniprotkb-0.2.0/pyuniprot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 01:42:19.000000 pyuniprotkb-0.2.0/pyuniprot/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 01:42:26.678778 pyuniprotkb-0.2.0/pyuniprot/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-03-13 01:42:19.000000 pyuniprotkb-0.2.0/pyuniprot/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9824 2024-03-13 01:42:19.000000 pyuniprotkb-0.2.0/pyuniprot/utils/isoforms.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-13 01:42:19.000000 pyuniprotkb-0.2.0/pyuniprot/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 01:42:26.682778 pyuniprotkb-0.2.0/pyuniprotkb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-03-13 01:42:26.000000 pyuniprotkb-0.2.0/pyuniprotkb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-03-13 01:42:26.000000 pyuniprotkb-0.2.0/pyuniprotkb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 01:42:26.000000 pyuniprotkb-0.2.0/pyuniprotkb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-13 01:42:26.000000 pyuniprotkb-0.2.0/pyuniprotkb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-13 01:42:26.000000 pyuniprotkb-0.2.0/pyuniprotkb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-13 01:42:19.000000 pyuniprotkb-0.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-03-13 01:42:19.000000 pyuniprotkb-0.2.0/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-03-13 01:42:26.682778 pyuniprotkb-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-03-13 01:42:19.000000 pyuniprotkb-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 01:42:26.682778 pyuniprotkb-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 01:42:19.000000 pyuniprotkb-0.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-03-13 01:42:19.000000 pyuniprotkb-0.2.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-03-13 01:42:19.000000 pyuniprotkb-0.2.0/tests/test_isoforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-03-13 01:42:19.000000 pyuniprotkb-0.2.0/tests/test_uniprot.py
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-03-13 01:42:19.000000 pyuniprotkb-0.2.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:33:24.622710 pyuniprotkb-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-15 20:33:13.000000 pyuniprotkb-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-15 20:33:13.000000 pyuniprotkb-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-15 20:33:13.000000 pyuniprotkb-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4574 2024-04-15 20:33:24.622710 pyuniprotkb-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3832 2024-04-15 20:33:13.000000 pyuniprotkb-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-15 20:33:13.000000 pyuniprotkb-0.3.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:33:24.618710 pyuniprotkb-0.3.0/pyuniprot/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-15 20:33:13.000000 pyuniprotkb-0.3.0/pyuniprot/CC.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-15 20:33:13.000000 pyuniprotkb-0.3.0/pyuniprot/DB.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9087 2024-04-15 20:33:13.000000 pyuniprotkb-0.3.0/pyuniprot/UniRef.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25902 2024-04-15 20:33:13.000000 pyuniprotkb-0.3.0/pyuniprot/Uniprot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-15 20:33:13.000000 pyuniprotkb-0.3.0/pyuniprot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 20:33:13.000000 pyuniprotkb-0.3.0/pyuniprot/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:33:24.618710 pyuniprotkb-0.3.0/pyuniprot/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-15 20:33:13.000000 pyuniprotkb-0.3.0/pyuniprot/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9824 2024-04-15 20:33:13.000000 pyuniprotkb-0.3.0/pyuniprot/utils/isoforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-15 20:33:13.000000 pyuniprotkb-0.3.0/pyuniprot/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:33:24.618710 pyuniprotkb-0.3.0/pyuniprotkb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4574 2024-04-15 20:33:24.000000 pyuniprotkb-0.3.0/pyuniprotkb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-15 20:33:24.000000 pyuniprotkb-0.3.0/pyuniprotkb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 20:33:24.000000 pyuniprotkb-0.3.0/pyuniprotkb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-15 20:33:24.000000 pyuniprotkb-0.3.0/pyuniprotkb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-15 20:33:24.000000 pyuniprotkb-0.3.0/pyuniprotkb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-15 20:33:13.000000 pyuniprotkb-0.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-15 20:33:13.000000 pyuniprotkb-0.3.0/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-15 20:33:24.622710 pyuniprotkb-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-15 20:33:13.000000 pyuniprotkb-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:33:24.618710 pyuniprotkb-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 20:33:13.000000 pyuniprotkb-0.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-15 20:33:13.000000 pyuniprotkb-0.3.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-04-15 20:33:13.000000 pyuniprotkb-0.3.0/tests/test_isoforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-04-15 20:33:13.000000 pyuniprotkb-0.3.0/tests/test_uniprot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-04-15 20:33:13.000000 pyuniprotkb-0.3.0/tests/test_uniref.py
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-15 20:33:13.000000 pyuniprotkb-0.3.0/tox.ini
```

### Comparing `pyuniprotkb-0.2.0/.pre-commit-config.yaml` & `pyuniprotkb-0.3.0/.pre-commit-config.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0
+    rev: v4.6.0
     hooks:
       - id: check-builtin-literals
       - id: check-added-large-files
       - id: check-case-conflict
       - id: check-toml
       - id: check-yaml
       - id: debug-statements
       - id: end-of-file-fixer
         exclude: tests/test_files
       - id: forbid-new-submodules
       - id: trailing-whitespace
         exclude: tests/test_files
 
   - repo: https://github.com/psf/black
-    rev: 24.2.0
+    rev: 24.3.0
     hooks:
       - id: black
         language_version: python3.10
 
   - repo: https://github.com/PyCQA/flake8
     rev: 7.0.0
     hooks:
@@ -35,15 +35,15 @@
   - repo: https://github.com/PyCQA/isort
     rev: 5.13.2
     hooks:
       - id: isort
         files: \.py$
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.8.0
+    rev: v1.9.0
     hooks:
       - id: mypy
         exclude: tests/data
         args: ["--pretty", "--show-error-codes"]
         additional_dependencies:
           [
             "keyring==23.13.1",
```

### Comparing `pyuniprotkb-0.2.0/LICENSE` & `pyuniprotkb-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyuniprotkb-0.2.0/pyuniprot/DB.py` & `pyuniprotkb-0.3.0/pyuniprot/DB.py`

 * *Files identical despite different names*

### Comparing `pyuniprotkb-0.2.0/pyuniprot/Uniprot.py` & `pyuniprotkb-0.3.0/pyuniprot/Uniprot.py`

 * *Files identical despite different names*

### Comparing `pyuniprotkb-0.2.0/pyuniprot/utils/isoforms.py` & `pyuniprotkb-0.3.0/pyuniprot/utils/isoforms.py`

 * *Files identical despite different names*

### Comparing `pyuniprotkb-0.2.0/pyuniprotkb.egg-info/SOURCES.txt` & `pyuniprotkb-0.3.0/pyuniprotkb.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -6,22 +6,24 @@
 requirements.txt
 requirements_dev.txt
 setup.cfg
 setup.py
 tox.ini
 pyuniprot/CC.py
 pyuniprot/DB.py
+pyuniprot/UniRef.py
 pyuniprot/Uniprot.py
 pyuniprot/__init__.py
 pyuniprot/py.typed
 pyuniprot/version.py
 pyuniprot/utils/__init__.py
 pyuniprot/utils/isoforms.py
 pyuniprotkb.egg-info/PKG-INFO
 pyuniprotkb.egg-info/SOURCES.txt
 pyuniprotkb.egg-info/dependency_links.txt
 pyuniprotkb.egg-info/requires.txt
 pyuniprotkb.egg-info/top_level.txt
 tests/__init__.py
 tests/conftest.py
 tests/test_isoforms.py
-tests/test_uniprot.py
+tests/test_uniprot.py
+tests/test_uniref.py
```

### Comparing `pyuniprotkb-0.2.0/setup.py` & `pyuniprotkb-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `pyuniprotkb-0.2.0/tests/test_isoforms.py` & `pyuniprotkb-0.3.0/tests/test_isoforms.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import os
 
 import pytest
 
 from pyuniprot.utils import AA, get_alt_resids, get_isoforms
 
 CFD = os.path.dirname(__file__)
+CWD = os.getcwd()
 
 
 def test_get_isoforms_wrong_id():
     """
     Test the get_isoforms function when the uniprot_id str length is wrong
     """
     uniprot_id = "xxx"
@@ -26,28 +27,28 @@
     Test the get_isoforms function when the uniprot_id is obsolete
     """
     uniprot_id = "P00016"
     e_message = f"{uniprot_id} is obsolete"
     with pytest.raises(ValueError, match=e_message):
         get_isoforms(uniprot_id)
     try:
-        os.remove(f"{CFD}/{uniprot_id}.txt")
+        os.remove(f"{CWD}/{uniprot_id}.txt")
     except OSError:
         pass
 
 
 def test_get_isoforms_no_iso():
     """
     Test the get_isoforms function when there is no isoform
     """
     uniprot_id = "Q9H0H0"
     isoforms = get_isoforms(uniprot_id)
     assert isoforms == {"Q9H0H0": []}, "Q9H0H0 isoform is not empty."
     try:
-        os.remove(f"{CFD}/{uniprot_id}.txt")
+        os.remove(f"{CWD}/{uniprot_id}.txt")
     except OSError:
         pass
 
 
 def test_get_isoforms():
     """
     Test the get_isoforms function
@@ -63,15 +64,15 @@
         ],
         "Q92879-5": [(1, 17, "", "Missing"), (104, 104, "", "Missing")],
         "Q92879-6": [(104, 104, "", "Missing")],
     }
     isoforms = get_isoforms(uniprot_id)
     assert isoforms == expected, "Q92879 isoforms are wrong."
     try:
-        os.remove(f"{CFD}/{uniprot_id}.txt")
+        os.remove(f"{CWD}/{uniprot_id}.txt")
     except OSError:
         pass
 
 
 def test_get_alt_wrong_aa():
     """
     Test wrong AA names
@@ -92,15 +93,15 @@
     uniprot_resid = 12
     residue_type = "C"
     e_message = f"{uniprot_id} {uniprot_resid} is not {residue_type}"
     with pytest.raises(ValueError, match=e_message):
         get_alt_resids(uniprot_id, uniprot_resid, residue_type)
 
     try:
-        os.remove(f"{CFD}/{uniprot_id}.txt")
+        os.remove(f"{CWD}/{uniprot_id}.txt")
     except OSError:
         pass
 
 
 def test_get_alt_resids_oob():
     """
     Test out of bounds resids
@@ -109,15 +110,16 @@
     uniprot_resid = 200
     residue_type = "C"
 
     e_message = f"{uniprot_id} {uniprot_resid} is beyond the sequence of length 189"
     with pytest.raises(ValueError, match=e_message):
         get_alt_resids(uniprot_id, uniprot_resid, residue_type)
     try:
-        os.remove(f"{CFD}/{uniprot_id}.txt")
+        os.remove(f"{CWD}/{uniprot_id}.txt")
+        os.remove(f"{CWD}/{uniprot_id[:-2]}.txt")
     except OSError:
         pass
 
 
 def test_get_alt_resids():
     """
     Test different resid situations
@@ -135,19 +137,12 @@
         ("Q92879-6", 433),
     ]
     resids = get_alt_resids(uniprot_id, uniprot_resid, residue_type)
     assert (
         resids == expected
     ), f"{uniprot_id} {uniprot_resid} {residue_type} alt resids wrong"
     try:
-        os.remove(f"{CFD}/{uniprot_id}.txt")
+        os.remove(f"{CWD}/{uniprot_id}.txt")
+        os.remove(f"{CWD}/{uniprot_id[:-2]}.txt")
+        os.remove(f"{CWD}/{uniprot_id[:-2]}-1.txt")
     except OSError:
         pass
-
-
-# def test():
-#     """
-#     Test the get_isoforms function when there is no isoform
-#     """
-#     uniprot_id = "P01116"
-#     isoforms = get_isoforms(uniprot_id)
-#     print(isoforms)
```

### Comparing `pyuniprotkb-0.2.0/tests/test_uniprot.py` & `pyuniprotkb-0.3.0/tests/test_uniprot.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import sys
 from pathlib import Path
 
 from pyuniprot.Uniprot import Uniprot
 
 sys.path.append("..")
 CFD = os.path.dirname(__file__)
+CWD = os.getcwd()
 
 
 def test_get_properties():
     """
     Test class properties
     """
     uniprot_id = "P36952"
@@ -37,15 +38,15 @@
     assert uniprot.local_download_dir == Path(
         CFD, "test_files"
     ), "local_download_dir not pointing to test_files."
     assert uniprot.uniprot_txt_file == Path(
         CFD, "test_files", f"{uniprot.uniprot_id}.txt"
     ), "Uniprot TXT file path not right when existed."
     try:
-        os.remove(f"{CFD}/{uniprot_id}.txt")
+        os.remove(f"{CWD}/{uniprot_id}.txt")
     except OSError:
         pass
 
 
 def test_get_category_lines():
     """Test the _get_category_lines function."""
     uniprot_id = "P04637"
```

