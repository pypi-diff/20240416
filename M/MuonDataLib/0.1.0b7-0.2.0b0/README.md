# Comparing `tmp/muondatalib-0.1.0b7.tar.gz` & `tmp/muondatalib-0.2.0b0.tar.gz`

## Comparing `muondatalib-0.1.0b7.tar` & `muondatalib-0.2.0b0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 muondatalib-0.1.0b7/.pre-commit-config.yaml
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 muondatalib-0.1.0b7/.readthedocs.yaml
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 muondatalib-0.1.0b7/MuonDataLib-dev.yml
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 muondatalib-0.1.0b7/MuonDataLib.yml
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 muondatalib-0.1.0b7/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 muondatalib-0.1.0b7/.github/release.yml
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 muondatalib-0.1.0b7/.github/workflows/flake8.yml
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 muondatalib-0.1.0b7/.github/workflows/label_merge_conflicts.yml
--rw-r--r--   0        0        0     3260 2020-02-02 00:00:00.000000 muondatalib-0.1.0b7/.github/workflows/merge.yml
--rw-r--r--   0        0        0     3441 2020-02-02 00:00:00.000000 muondatalib-0.1.0b7/.github/workflows/release_next.yml
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 muondatalib-0.1.0b7/.github/workflows/run_tests.yml
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 muondatalib-0.1.0b7/docs/source/api.rst
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 muondatalib-0.1.0b7/docs/source/conf.py
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 muondatalib-0.1.0b7/docs/source/index.rst
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 muondatalib-0.1.0b7/docs/source/intro.rst
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 muondatalib-0.1.0b7/docs/source/usage.rst
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 muondatalib-0.1.0b7/docs/source/dev/index.rst
--rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 muondatalib-0.1.0b7/docs/source/dev/setup.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 muondatalib-0.1.0b7/src/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 muondatalib-0.1.0b7/src/MuonDataLib/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 muondatalib-0.1.0b7/src/MuonDataLib/data/__init__.py
--rw-r--r--   0        0        0     4493 2020-02-02 00:00:00.000000 muondatalib-0.1.0b7/src/MuonDataLib/data/detector1.py
--rw-r--r--   0        0        0     4103 2020-02-02 00:00:00.000000 muondatalib-0.1.0b7/src/MuonDataLib/data/hdf5.py
--rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 muondatalib-0.1.0b7/src/MuonDataLib/data/muon_data.py
--rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 muondatalib-0.1.0b7/src/MuonDataLib/data/periods.py
--rw-r--r--   0        0        0     3607 2020-02-02 00:00:00.000000 muondatalib-0.1.0b7/src/MuonDataLib/data/raw_data.py
--rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 muondatalib-0.1.0b7/src/MuonDataLib/data/sample.py
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 muondatalib-0.1.0b7/src/MuonDataLib/data/source.py
--rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 muondatalib-0.1.0b7/src/MuonDataLib/data/user.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 muondatalib-0.1.0b7/src/MuonDataLib/data/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 muondatalib-0.1.0b7/src/MuonDataLib/data/loader/__init__.py
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 muondatalib-0.1.0b7/src/MuonDataLib/data/loader/load_nxs2.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 muondatalib-0.1.0b7/test/__init__.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 muondatalib-0.1.0b7/test/add_test.py
--rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 muondatalib-0.1.0b7/tools/conda_dict_to_yml.py
--rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 muondatalib-0.1.0b7/tools/create_conda_yml.py
--rw-r--r--   0        0        0     2005 2020-02-02 00:00:00.000000 muondatalib-0.1.0b7/tools/setup_helper.py
--rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 muondatalib-0.1.0b7/tools/version.py
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 muondatalib-0.1.0b7/README.md
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 muondatalib-0.1.0b7/pyproject.toml
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 muondatalib-0.1.0b7/PKG-INFO
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 muondatalib-0.2.0b0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 muondatalib-0.2.0b0/.readthedocs.yaml
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 muondatalib-0.2.0b0/MuonDataLib-dev.yml
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 muondatalib-0.2.0b0/MuonDataLib.yml
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 muondatalib-0.2.0b0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 muondatalib-0.2.0b0/.github/release.yml
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 muondatalib-0.2.0b0/.github/workflows/flake8.yml
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 muondatalib-0.2.0b0/.github/workflows/label_merge_conflicts.yml
+-rw-r--r--   0        0        0     3260 2020-02-02 00:00:00.000000 muondatalib-0.2.0b0/.github/workflows/merge.yml
+-rw-r--r--   0        0        0     3441 2020-02-02 00:00:00.000000 muondatalib-0.2.0b0/.github/workflows/release_next.yml
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 muondatalib-0.2.0b0/.github/workflows/run_tests.yml
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 muondatalib-0.2.0b0/docs/source/api.rst
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 muondatalib-0.2.0b0/docs/source/conf.py
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 muondatalib-0.2.0b0/docs/source/index.rst
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 muondatalib-0.2.0b0/docs/source/intro.rst
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 muondatalib-0.2.0b0/docs/source/usage.rst
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 muondatalib-0.2.0b0/docs/source/dev/index.rst
+-rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 muondatalib-0.2.0b0/docs/source/dev/setup.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 muondatalib-0.2.0b0/src/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 muondatalib-0.2.0b0/src/MuonDataLib/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 muondatalib-0.2.0b0/src/MuonDataLib/data/__init__.py
+-rw-r--r--   0        0        0     4493 2020-02-02 00:00:00.000000 muondatalib-0.2.0b0/src/MuonDataLib/data/detector1.py
+-rw-r--r--   0        0        0     4103 2020-02-02 00:00:00.000000 muondatalib-0.2.0b0/src/MuonDataLib/data/hdf5.py
+-rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 muondatalib-0.2.0b0/src/MuonDataLib/data/muon_data.py
+-rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 muondatalib-0.2.0b0/src/MuonDataLib/data/periods.py
+-rw-r--r--   0        0        0     3607 2020-02-02 00:00:00.000000 muondatalib-0.2.0b0/src/MuonDataLib/data/raw_data.py
+-rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 muondatalib-0.2.0b0/src/MuonDataLib/data/sample.py
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 muondatalib-0.2.0b0/src/MuonDataLib/data/source.py
+-rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 muondatalib-0.2.0b0/src/MuonDataLib/data/user.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 muondatalib-0.2.0b0/src/MuonDataLib/data/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 muondatalib-0.2.0b0/src/MuonDataLib/data/loader/__init__.py
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 muondatalib-0.2.0b0/src/MuonDataLib/data/loader/load_nxs2.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 muondatalib-0.2.0b0/test/__init__.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 muondatalib-0.2.0b0/test/add_test.py
+-rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 muondatalib-0.2.0b0/tools/conda_dict_to_yml.py
+-rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 muondatalib-0.2.0b0/tools/create_conda_yml.py
+-rw-r--r--   0        0        0     2005 2020-02-02 00:00:00.000000 muondatalib-0.2.0b0/tools/setup_helper.py
+-rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 muondatalib-0.2.0b0/tools/version.py
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 muondatalib-0.2.0b0/README.md
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 muondatalib-0.2.0b0/pyproject.toml
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 muondatalib-0.2.0b0/PKG-INFO
```

### Comparing `muondatalib-0.1.0b7/.pre-commit-config.yaml` & `muondatalib-0.2.0b0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `muondatalib-0.1.0b7/.github/PULL_REQUEST_TEMPLATE.md` & `muondatalib-0.2.0b0/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `muondatalib-0.1.0b7/.github/workflows/label_merge_conflicts.yml` & `muondatalib-0.2.0b0/.github/workflows/label_merge_conflicts.yml`

 * *Files identical despite different names*

### Comparing `muondatalib-0.1.0b7/.github/workflows/merge.yml` & `muondatalib-0.2.0b0/.github/workflows/merge.yml`

 * *Files identical despite different names*

### Comparing `muondatalib-0.1.0b7/.github/workflows/release_next.yml` & `muondatalib-0.2.0b0/.github/workflows/release_next.yml`

 * *Files identical despite different names*

### Comparing `muondatalib-0.1.0b7/.github/workflows/run_tests.yml` & `muondatalib-0.2.0b0/.github/workflows/run_tests.yml`

 * *Files identical despite different names*

### Comparing `muondatalib-0.1.0b7/docs/source/conf.py` & `muondatalib-0.2.0b0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `muondatalib-0.1.0b7/docs/source/index.rst` & `muondatalib-0.2.0b0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `muondatalib-0.1.0b7/docs/source/dev/setup.rst` & `muondatalib-0.2.0b0/docs/source/dev/setup.rst`

 * *Files identical despite different names*

### Comparing `muondatalib-0.1.0b7/src/MuonDataLib/data/detector1.py` & `muondatalib-0.2.0b0/src/MuonDataLib/data/detector1.py`

 * *Files identical despite different names*

### Comparing `muondatalib-0.1.0b7/src/MuonDataLib/data/hdf5.py` & `muondatalib-0.2.0b0/src/MuonDataLib/data/hdf5.py`

 * *Files identical despite different names*

### Comparing `muondatalib-0.1.0b7/src/MuonDataLib/data/muon_data.py` & `muondatalib-0.2.0b0/src/MuonDataLib/data/muon_data.py`

 * *Files identical despite different names*

### Comparing `muondatalib-0.1.0b7/src/MuonDataLib/data/periods.py` & `muondatalib-0.2.0b0/src/MuonDataLib/data/periods.py`

 * *Files identical despite different names*

### Comparing `muondatalib-0.1.0b7/src/MuonDataLib/data/raw_data.py` & `muondatalib-0.2.0b0/src/MuonDataLib/data/raw_data.py`

 * *Files identical despite different names*

### Comparing `muondatalib-0.1.0b7/src/MuonDataLib/data/sample.py` & `muondatalib-0.2.0b0/src/MuonDataLib/data/sample.py`

 * *Files identical despite different names*

### Comparing `muondatalib-0.1.0b7/src/MuonDataLib/data/source.py` & `muondatalib-0.2.0b0/src/MuonDataLib/data/source.py`

 * *Files identical despite different names*

### Comparing `muondatalib-0.1.0b7/src/MuonDataLib/data/user.py` & `muondatalib-0.2.0b0/src/MuonDataLib/data/user.py`

 * *Files identical despite different names*

### Comparing `muondatalib-0.1.0b7/src/MuonDataLib/data/utils.py` & `muondatalib-0.2.0b0/src/MuonDataLib/data/utils.py`

 * *Files identical despite different names*

### Comparing `muondatalib-0.1.0b7/src/MuonDataLib/data/loader/load_nxs2.py` & `muondatalib-0.2.0b0/src/MuonDataLib/data/loader/load_nxs2.py`

 * *Files identical despite different names*

### Comparing `muondatalib-0.1.0b7/tools/conda_dict_to_yml.py` & `muondatalib-0.2.0b0/tools/conda_dict_to_yml.py`

 * *Files identical despite different names*

### Comparing `muondatalib-0.1.0b7/tools/create_conda_yml.py` & `muondatalib-0.2.0b0/tools/create_conda_yml.py`

 * *Files identical despite different names*

### Comparing `muondatalib-0.1.0b7/tools/setup_helper.py` & `muondatalib-0.2.0b0/tools/setup_helper.py`

 * *Files identical despite different names*

### Comparing `muondatalib-0.1.0b7/tools/version.py` & `muondatalib-0.2.0b0/tools/version.py`

 * *Files identical despite different names*

