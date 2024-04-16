# Comparing `tmp/aas-core3.0-1.0.3.tar.gz` & `tmp/aas_core3_0-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aas-core3.0-1.0.3.tar", last modified: Fri Mar 22 22:30:17 2024, max compression
+gzip compressed data, was "aas_core3_0-1.0.4.tar", last modified: Tue Apr 16 17:48:35 2024, max compression
```

## Comparing `aas-core3.0-1.0.3.tar` & `aas_core3_0-1.0.4.tar`

### file list

```diff
@@ -1,52 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 22:30:17.085826 aas-core3.0-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-03-22 22:30:08.000000 aas-core3.0-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-03-22 22:30:17.085826 aas-core3.0-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-03-22 22:30:08.000000 aas-core3.0-1.0.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 22:30:17.077826 aas-core3.0-1.0.3/aas_core3/
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-03-22 22:30:08.000000 aas-core3.0-1.0.3/aas_core3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-03-22 22:30:08.000000 aas-core3.0-1.0.3/aas_core3/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     6674 2024-03-22 22:30:08.000000 aas-core3.0-1.0.3/aas_core3/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)   341761 2024-03-22 22:30:08.000000 aas-core3.0-1.0.3/aas_core3/jsonization.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-22 22:30:08.000000 aas-core3.0-1.0.3/aas_core3/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    13216 2024-03-22 22:30:08.000000 aas-core3.0-1.0.3/aas_core3/stringification.py
--rw-r--r--   0 runner    (1001) docker     (127)   276794 2024-03-22 22:30:08.000000 aas-core3.0-1.0.3/aas_core3/types.py
--rw-r--r--   0 runner    (1001) docker     (127)   229409 2024-03-22 22:30:08.000000 aas-core3.0-1.0.3/aas_core3/verification.py
--rw-r--r--   0 runner    (1001) docker     (127)   950728 2024-03-22 22:30:08.000000 aas-core3.0-1.0.3/aas_core3/xmlization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 22:30:17.085826 aas-core3.0-1.0.3/aas_core3.0.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-03-22 22:30:17.000000 aas-core3.0-1.0.3/aas_core3.0.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-03-22 22:30:17.000000 aas-core3.0-1.0.3/aas_core3.0.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 22:30:17.000000 aas-core3.0-1.0.3/aas_core3.0.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-22 22:30:17.000000 aas-core3.0-1.0.3/aas_core3.0.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 22:30:17.073826 aas-core3.0-1.0.3/dev_scripts/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 22:30:17.081826 aas-core3.0-1.0.3/dev_scripts/test_codegen/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-22 22:30:08.000000 aas-core3.0-1.0.3/dev_scripts/test_codegen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-03-22 22:30:08.000000 aas-core3.0-1.0.3/dev_scripts/test_codegen/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-03-22 22:30:08.000000 aas-core3.0-1.0.3/dev_scripts/test_codegen/generate_all.py
--rw-r--r--   0 runner    (1001) docker     (127)    10953 2024-03-22 22:30:08.000000 aas-core3.0-1.0.3/dev_scripts/test_codegen/generate_common_jsonization.py
--rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-03-22 22:30:08.000000 aas-core3.0-1.0.3/dev_scripts/test_codegen/generate_test_for_descend_and_pass_through_visitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-03-22 22:30:08.000000 aas-core3.0-1.0.3/dev_scripts/test_codegen/generate_test_for_descend_once.py
--rw-r--r--   0 runner    (1001) docker     (127)     4675 2024-03-22 22:30:08.000000 aas-core3.0-1.0.3/dev_scripts/test_codegen/generate_test_for_jsonization_of_classes_with_descendants.py
--rw-r--r--   0 runner    (1001) docker     (127)    13346 2024-03-22 22:30:08.000000 aas-core3.0-1.0.3/dev_scripts/test_codegen/generate_test_for_jsonization_of_concrete_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-03-22 22:30:08.000000 aas-core3.0-1.0.3/dev_scripts/test_codegen/generate_test_for_jsonization_of_concrete_classes_outside_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-03-22 22:30:08.000000 aas-core3.0-1.0.3/dev_scripts/test_codegen/generate_test_for_jsonization_of_enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     7073 2024-03-22 22:30:08.000000 aas-core3.0-1.0.3/dev_scripts/test_codegen/generate_test_for_over_X_or_empty.py
--rw-r--r--   0 runner    (1001) docker     (127)     5632 2024-03-22 22:30:08.000000 aas-core3.0-1.0.3/dev_scripts/test_codegen/generate_test_for_x_or_default.py
--rw-r--r--   0 runner    (1001) docker     (127)     6109 2024-03-22 22:30:08.000000 aas-core3.0-1.0.3/dev_scripts/test_codegen/generate_test_for_xmlization_of_classes_with_descendants.py
--rw-r--r--   0 runner    (1001) docker     (127)    10711 2024-03-22 22:30:08.000000 aas-core3.0-1.0.3/dev_scripts/test_codegen/generate_test_for_xmlization_of_concrete_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-03-22 22:30:08.000000 aas-core3.0-1.0.3/dev_scripts/test_codegen/generate_test_for_xmlization_of_concrete_classes_outside_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-03-22 22:30:08.000000 aas-core3.0-1.0.3/dev_scripts/test_codegen/test_data_io.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-22 22:30:17.085826 aas-core3.0-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-03-22 22:30:08.000000 aas-core3.0-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 22:30:17.085826 aas-core3.0-1.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    32877 2024-03-22 22:30:09.000000 aas-core3.0-1.0.3/tests/test_descend_and_pass_through_visitor.py
--rw-r--r--   0 runner    (1001) docker     (127)    22650 2024-03-22 22:30:09.000000 aas-core3.0-1.0.3/tests/test_descend_once.py
--rw-r--r--   0 runner    (1001) docker     (127)    37646 2024-03-22 22:30:09.000000 aas-core3.0-1.0.3/tests/test_jsonization_of_classes_with_descendants.py
--rw-r--r--   0 runner    (1001) docker     (127)   183209 2024-03-22 22:30:09.000000 aas-core3.0-1.0.3/tests/test_jsonization_of_concrete_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)    24646 2024-03-22 22:30:09.000000 aas-core3.0-1.0.3/tests/test_jsonization_of_concrete_classes_outside_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-03-22 22:30:09.000000 aas-core3.0-1.0.3/tests/test_jsonization_of_enums.py
--rw-r--r--   0 runner    (1001) docker     (127)   201748 2024-03-22 22:30:09.000000 aas-core3.0-1.0.3/tests/test_over_x_or_empty.py
--rw-r--r--   0 runner    (1001) docker     (127)    13298 2024-03-22 22:30:09.000000 aas-core3.0-1.0.3/tests/test_x_or_default.py
--rw-r--r--   0 runner    (1001) docker     (127)   232372 2024-03-22 22:30:09.000000 aas-core3.0-1.0.3/tests/test_xmlization_of_classes_with_descendants.py
--rw-r--r--   0 runner    (1001) docker     (127)   254466 2024-03-22 22:30:09.000000 aas-core3.0-1.0.3/tests/test_xmlization_of_concrete_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)    33293 2024-03-22 22:30:09.000000 aas-core3.0-1.0.3/tests/test_xmlization_of_concrete_classes_outside_container.py
--rw-r--r--   0 runner    (1001) docker     (127)    34698 2024-03-22 22:30:09.000000 aas-core3.0-1.0.3/tests/test_xmlization_when_text_attached_to_end_element.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:48:35.511688 aas_core3_0-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-16 17:48:27.000000 aas_core3_0-1.0.4/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-16 17:48:27.000000 aas_core3_0-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-04-16 17:48:35.511688 aas_core3_0-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-16 17:48:27.000000 aas_core3_0-1.0.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:48:35.499688 aas_core3_0-1.0.4/aas_core3/
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-16 17:48:27.000000 aas_core3_0-1.0.4/aas_core3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-16 17:48:27.000000 aas_core3_0-1.0.4/aas_core3/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6674 2024-04-16 17:48:27.000000 aas_core3_0-1.0.4/aas_core3/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)   341653 2024-04-16 17:48:27.000000 aas_core3_0-1.0.4/aas_core3/jsonization.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-16 17:48:27.000000 aas_core3_0-1.0.4/aas_core3/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    13216 2024-04-16 17:48:27.000000 aas_core3_0-1.0.4/aas_core3/stringification.py
+-rw-r--r--   0 runner    (1001) docker     (127)   276929 2024-04-16 17:48:27.000000 aas_core3_0-1.0.4/aas_core3/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)   229469 2024-04-16 17:48:27.000000 aas_core3_0-1.0.4/aas_core3/verification.py
+-rw-r--r--   0 runner    (1001) docker     (127)   950617 2024-04-16 17:48:27.000000 aas_core3_0-1.0.4/aas_core3/xmlization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:48:35.507688 aas_core3_0-1.0.4/aas_core3.0.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-04-16 17:48:35.000000 aas_core3_0-1.0.4/aas_core3.0.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-04-16 17:48:35.000000 aas_core3_0-1.0.4/aas_core3.0.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 17:48:35.000000 aas_core3_0-1.0.4/aas_core3.0.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-16 17:48:35.000000 aas_core3_0-1.0.4/aas_core3.0.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:48:35.495688 aas_core3_0-1.0.4/dev_scripts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:48:35.503688 aas_core3_0-1.0.4/dev_scripts/test_codegen/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-16 17:48:27.000000 aas_core3_0-1.0.4/dev_scripts/test_codegen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-04-16 17:48:27.000000 aas_core3_0-1.0.4/dev_scripts/test_codegen/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-16 17:48:27.000000 aas_core3_0-1.0.4/dev_scripts/test_codegen/generate_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10953 2024-04-16 17:48:27.000000 aas_core3_0-1.0.4/dev_scripts/test_codegen/generate_common_jsonization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-04-16 17:48:27.000000 aas_core3_0-1.0.4/dev_scripts/test_codegen/generate_test_for_descend_and_pass_through_visitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-04-16 17:48:27.000000 aas_core3_0-1.0.4/dev_scripts/test_codegen/generate_test_for_descend_once.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4675 2024-04-16 17:48:27.000000 aas_core3_0-1.0.4/dev_scripts/test_codegen/generate_test_for_jsonization_of_classes_with_descendants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13346 2024-04-16 17:48:27.000000 aas_core3_0-1.0.4/dev_scripts/test_codegen/generate_test_for_jsonization_of_concrete_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-04-16 17:48:27.000000 aas_core3_0-1.0.4/dev_scripts/test_codegen/generate_test_for_jsonization_of_concrete_classes_outside_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-04-16 17:48:27.000000 aas_core3_0-1.0.4/dev_scripts/test_codegen/generate_test_for_jsonization_of_enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7073 2024-04-16 17:48:27.000000 aas_core3_0-1.0.4/dev_scripts/test_codegen/generate_test_for_over_X_or_empty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5632 2024-04-16 17:48:27.000000 aas_core3_0-1.0.4/dev_scripts/test_codegen/generate_test_for_x_or_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6109 2024-04-16 17:48:27.000000 aas_core3_0-1.0.4/dev_scripts/test_codegen/generate_test_for_xmlization_of_classes_with_descendants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10711 2024-04-16 17:48:27.000000 aas_core3_0-1.0.4/dev_scripts/test_codegen/generate_test_for_xmlization_of_concrete_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-04-16 17:48:27.000000 aas_core3_0-1.0.4/dev_scripts/test_codegen/generate_test_for_xmlization_of_concrete_classes_outside_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-04-16 17:48:27.000000 aas_core3_0-1.0.4/dev_scripts/test_codegen/test_data_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 17:48:35.511688 aas_core3_0-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-16 17:48:27.000000 aas_core3_0-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:48:35.507688 aas_core3_0-1.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    32877 2024-04-16 17:48:27.000000 aas_core3_0-1.0.4/tests/test_descend_and_pass_through_visitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22650 2024-04-16 17:48:27.000000 aas_core3_0-1.0.4/tests/test_descend_once.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37646 2024-04-16 17:48:27.000000 aas_core3_0-1.0.4/tests/test_jsonization_of_classes_with_descendants.py
+-rw-r--r--   0 runner    (1001) docker     (127)   183209 2024-04-16 17:48:27.000000 aas_core3_0-1.0.4/tests/test_jsonization_of_concrete_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24646 2024-04-16 17:48:27.000000 aas_core3_0-1.0.4/tests/test_jsonization_of_concrete_classes_outside_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-04-16 17:48:27.000000 aas_core3_0-1.0.4/tests/test_jsonization_of_enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)   201748 2024-04-16 17:48:27.000000 aas_core3_0-1.0.4/tests/test_over_x_or_empty.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13298 2024-04-16 17:48:27.000000 aas_core3_0-1.0.4/tests/test_x_or_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)   232372 2024-04-16 17:48:27.000000 aas_core3_0-1.0.4/tests/test_xmlization_of_classes_with_descendants.py
+-rw-r--r--   0 runner    (1001) docker     (127)   254466 2024-04-16 17:48:27.000000 aas_core3_0-1.0.4/tests/test_xmlization_of_concrete_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33293 2024-04-16 17:48:27.000000 aas_core3_0-1.0.4/tests/test_xmlization_of_concrete_classes_outside_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34698 2024-04-16 17:48:27.000000 aas_core3_0-1.0.4/tests/test_xmlization_when_text_attached_to_end_element.py
```

### Comparing `aas-core3.0-1.0.3/PKG-INFO` & `aas_core3_0-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: aas-core3.0
-Version: 1.0.3
+Version: 1.0.4
 Summary: Manipulate, verify and de/serialize Asset Administration Shells.
 Home-page: https://github.com/aas-core-works/aas-core3.0-python
 Author: Marko Ristin
 Author-email: marko@ristin.ch
 License: License :: OSI Approved :: MIT License
 Keywords: asset administration shell sdk industry 4.0 industrie i4.0 industry iot iiot
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 License-File: LICENSE
+License-File: AUTHORS
 
 **********************
 aas-core3.0-python
 **********************
 
 .. image:: https://github.com/aas-core-works/aas-core3.0-python/actions/workflows/ci.yml/badge.svg
     :target: https://github.com/aas-core-works/aas-core3.0-python/actions/workflows/ci.yml
```

### Comparing `aas-core3.0-1.0.3/README.rst` & `aas_core3_0-1.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `aas-core3.0-1.0.3/aas_core3/common.py` & `aas_core3_0-1.0.4/aas_core3/common.py`

 * *Files identical despite different names*

### Comparing `aas-core3.0-1.0.3/aas_core3/constants.py` & `aas_core3_0-1.0.4/aas_core3/constants.py`

 * *Files identical despite different names*

### Comparing `aas-core3.0-1.0.3/aas_core3/jsonization.py` & `aas_core3_0-1.0.4/aas_core3/jsonization.py`

 * *Files 0% similar despite different names*

```diff
@@ -6541,41 +6541,41 @@
 
 
 class _SetterForEmbeddedDataSpecification:
     """Provide de-serialization-setters for properties."""
 
     def __init__(self) -> None:
         """Initialize with all the properties unset."""
-        self.data_specification: Optional[aas_types.Reference] = None
         self.data_specification_content: Optional[
             aas_types.DataSpecificationContent
         ] = None
+        self.data_specification: Optional[aas_types.Reference] = None
 
     def ignore(self, jsonable: Jsonable) -> None:
         """Ignore :paramref:`jsonable` and do not set anything."""
         pass
 
-    def set_data_specification_from_jsonable(self, jsonable: Jsonable) -> None:
-        """
-        Parse :paramref:`jsonable` as the value of :py:attr:`~data_specification`.
-
-        :param jsonable: input to be parsed
-        """
-        self.data_specification = reference_from_jsonable(jsonable)
-
     def set_data_specification_content_from_jsonable(self, jsonable: Jsonable) -> None:
         """
         Parse :paramref:`jsonable` as the value of :py:attr:`~data_specification_content`.
 
         :param jsonable: input to be parsed
         """
         self.data_specification_content = data_specification_content_from_jsonable(
             jsonable
         )
 
+    def set_data_specification_from_jsonable(self, jsonable: Jsonable) -> None:
+        """
+        Parse :paramref:`jsonable` as the value of :py:attr:`~data_specification`.
+
+        :param jsonable: input to be parsed
+        """
+        self.data_specification = reference_from_jsonable(jsonable)
+
 
 def embedded_data_specification_from_jsonable(
     jsonable: Jsonable,
 ) -> aas_types.EmbeddedDataSpecification:
     """
     Parse an instance of :py:class:`.types.EmbeddedDataSpecification` from the JSON-able
     structure :paramref:`jsonable`.
@@ -6596,26 +6596,21 @@
 
         try:
             setter_method(setter, jsonable_value)
         except DeserializationException as exception:
             exception.path._prepend(PropertySegment(jsonable_value, key))
             raise exception
 
-    if setter.data_specification is None:
-        raise DeserializationException(
-            "The required property 'dataSpecification' is missing"
-        )
-
     if setter.data_specification_content is None:
         raise DeserializationException(
             "The required property 'dataSpecificationContent' is missing"
         )
 
     return aas_types.EmbeddedDataSpecification(
-        setter.data_specification, setter.data_specification_content
+        setter.data_specification_content, setter.data_specification
     )
 
 
 def data_type_iec_61360_from_jsonable(jsonable: Jsonable) -> aas_types.DataTypeIEC61360:
     """
     Convert the JSON-able structure :paramref:`jsonable` to a literal of
     :py:class:`.types.DataTypeIEC61360`.
@@ -7922,16 +7917,16 @@
     "DataSpecificationIec61360": data_specification_iec_61360_from_jsonable,
 }
 
 
 _SETTER_MAP_FOR_EMBEDDED_DATA_SPECIFICATION: Mapping[
     str, Callable[[_SetterForEmbeddedDataSpecification, Jsonable], None]
 ] = {
-    "dataSpecification": _SetterForEmbeddedDataSpecification.set_data_specification_from_jsonable,
     "dataSpecificationContent": _SetterForEmbeddedDataSpecification.set_data_specification_content_from_jsonable,
+    "dataSpecification": _SetterForEmbeddedDataSpecification.set_data_specification_from_jsonable,
     "modelType": _SetterForEmbeddedDataSpecification.ignore,
 }
 
 
 _SETTER_MAP_FOR_LEVEL_TYPE: Mapping[
     str, Callable[[_SetterForLevelType, Jsonable], None]
 ] = {
@@ -9150,20 +9145,21 @@
 
     def transform_embedded_data_specification(
         self, that: aas_types.EmbeddedDataSpecification
     ) -> MutableJsonable:
         """Serialize :paramref:`that` to a JSON-able representation."""
         jsonable: MutableMapping[str, MutableJsonable] = dict()
 
-        jsonable["dataSpecification"] = self.transform(that.data_specification)
-
         jsonable["dataSpecificationContent"] = self.transform(
             that.data_specification_content
         )
 
+        if that.data_specification is not None:
+            jsonable["dataSpecification"] = self.transform(that.data_specification)
+
         return jsonable
 
     # noinspection PyMethodMayBeStatic
     def transform_level_type(self, that: aas_types.LevelType) -> MutableJsonable:
         """Serialize :paramref:`that` to a JSON-able representation."""
         jsonable: MutableMapping[str, MutableJsonable] = dict()
```

### Comparing `aas-core3.0-1.0.3/aas_core3/stringification.py` & `aas_core3_0-1.0.4/aas_core3/stringification.py`

 * *Files identical despite different names*

### Comparing `aas-core3.0-1.0.3/aas_core3/types.py` & `aas_core3_0-1.0.4/aas_core3/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -5276,46 +5276,48 @@
         https://admin-shell.io/DataSpecificationTemplates/DataSpecificationIEC61360/3/0
     """
 
 
 class EmbeddedDataSpecification(Class):
     """Embed the content of a data specification."""
 
-    #: Reference to the data specification
-    data_specification: "Reference"
-
     #: Actual content of the data specification
     data_specification_content: "DataSpecificationContent"
 
+    #: Reference to the data specification
+    data_specification: Optional["Reference"]
+
     def descend_once(self) -> Iterator[Class]:
         """
         Iterate over the instances referenced from this instance.
 
         We do not recurse into the referenced instance.
 
         :yield: instances directly referenced from this instance
         """
-        yield self.data_specification
-
         yield self.data_specification_content
 
+        if self.data_specification is not None:
+            yield self.data_specification
+
     def descend(self) -> Iterator[Class]:
         """
         Iterate recursively over the instances referenced from this one.
 
         :yield: instances recursively referenced from this instance
         """
-        yield self.data_specification
-
-        yield from self.data_specification.descend()
-
         yield self.data_specification_content
 
         yield from self.data_specification_content.descend()
 
+        if self.data_specification is not None:
+            yield self.data_specification
+
+            yield from self.data_specification.descend()
+
     def accept(self, visitor: "AbstractVisitor") -> None:
         """Dispatch the :paramref:`visitor` on this instance."""
         visitor.visit_embedded_data_specification(self)
 
     def accept_with_context(
         self, visitor: "AbstractVisitorWithContext[ContextT]", context: ContextT
     ) -> None:
@@ -5336,20 +5338,20 @@
         """
         return transformer.transform_embedded_data_specification_with_context(
             self, context
         )
 
     def __init__(
         self,
-        data_specification: "Reference",
         data_specification_content: "DataSpecificationContent",
+        data_specification: Optional["Reference"] = None,
     ) -> None:
         """Initialize with the given values."""
-        self.data_specification = data_specification
         self.data_specification_content = data_specification_content
+        self.data_specification = data_specification
 
 
 class DataTypeIEC61360(enum.Enum):
     # pylint: disable=missing-class-docstring
 
     #: values containing a calendar date, conformant to ISO 8601:2004 Format yyyy-mm-dd
     #: Example from IEC 61360-1:2017: "1999-05-31" is the [DATE] representation of:
```

### Comparing `aas-core3.0-1.0.3/aas_core3/verification.py` & `aas_core3_0-1.0.4/aas_core3/verification.py`

 * *Files 0% similar despite different names*

```diff
@@ -5583,22 +5583,23 @@
                     error.path._prepend(PropertySegment(that, "concept_descriptions"))
                     yield error
 
     # noinspection PyMethodMayBeStatic
     def transform_embedded_data_specification(
         self, that: aas_types.EmbeddedDataSpecification
     ) -> Iterator[Error]:
-        for error in self.transform(that.data_specification):
-            error.path._prepend(PropertySegment(that, "data_specification"))
-            yield error
-
         for error in self.transform(that.data_specification_content):
             error.path._prepend(PropertySegment(that, "data_specification_content"))
             yield error
 
+        if that.data_specification is not None:
+            for error in self.transform(that.data_specification):
+                error.path._prepend(PropertySegment(that, "data_specification"))
+                yield error
+
     # noinspection PyMethodMayBeStatic
     def transform_level_type(self, that: aas_types.LevelType) -> Iterator[Error]:
         # No verification has been defined for LevelType.
         return
         # For this uncommon return-yield construction, see:
         # https://stackoverflow.com/questions/13243766/how-to-define-an-empty-generator-function
         # noinspection PyUnreachableCode
```

### Comparing `aas-core3.0-1.0.3/aas_core3/xmlization.py` & `aas_core3_0-1.0.4/aas_core3/xmlization.py`

 * *Files 0% similar despite different names*

```diff
@@ -21095,27 +21095,18 @@
     The properties correspond to the constructor arguments of
     :py:class:`EmbeddedDataSpecification`. We use this buffer to facilitate dispatching when
     parsing the properties in a streaming fashion.
     """
 
     def __init__(self) -> None:
         """Initialize with all the properties unset."""
-        self.data_specification: Optional[aas_types.Reference] = None
         self.data_specification_content: Optional[
             aas_types.DataSpecificationContent
         ] = None
-
-    def read_and_set_data_specification(
-        self, element: Element, iterator: Iterator[Tuple[str, Element]]
-    ) -> None:
-        """
-        Read :paramref:`element` as the property
-        :py:attr:`.types.EmbeddedDataSpecification.data_specification` and set it.
-        """
-        self.data_specification = _read_reference_as_sequence(element, iterator)
+        self.data_specification: Optional[aas_types.Reference] = None
 
     def read_and_set_data_specification_content(
         self, element: Element, iterator: Iterator[Tuple[str, Element]]
     ) -> None:
         """
         Read :paramref:`element` as the property
         :py:attr:`.types.EmbeddedDataSpecification.data_specification_content` and set it.
@@ -21141,14 +21132,23 @@
             exception.path._prepend(ElementSegment(next_element))
             raise
 
         _read_end_element(element, iterator)
 
         self.data_specification_content = result
 
+    def read_and_set_data_specification(
+        self, element: Element, iterator: Iterator[Tuple[str, Element]]
+    ) -> None:
+        """
+        Read :paramref:`element` as the property
+        :py:attr:`.types.EmbeddedDataSpecification.data_specification` and set it.
+        """
+        self.data_specification = _read_reference_as_sequence(element, iterator)
+
 
 def _read_embedded_data_specification_as_sequence(
     element: Element, iterator: Iterator[Tuple[str, Element]]
 ) -> aas_types.EmbeddedDataSpecification:
     """
     Read an instance of :py:class:`.types.EmbeddedDataSpecification`
     as a sequence of XML-encoded properties.
@@ -21212,27 +21212,22 @@
 
         try:
             read_and_set_method(reader_and_setter, next_element, iterator)
         except DeserializationException as exception:
             exception.path._prepend(ElementSegment(next_element))
             raise
 
-    if reader_and_setter.data_specification is None:
-        raise DeserializationException(
-            "The required property 'dataSpecification' is missing"
-        )
-
     if reader_and_setter.data_specification_content is None:
         raise DeserializationException(
             "The required property 'dataSpecificationContent' is missing"
         )
 
     return aas_types.EmbeddedDataSpecification(
-        reader_and_setter.data_specification,
         reader_and_setter.data_specification_content,
+        reader_and_setter.data_specification,
     )
 
 
 def _read_embedded_data_specification_as_element(
     element: Element, iterator: Iterator[Tuple[str, Element]]
 ) -> aas_types.EmbeddedDataSpecification:
     """
@@ -23416,16 +23411,16 @@
             _ReaderAndSetterForEmbeddedDataSpecification,
             Element,
             Iterator[Tuple[str, Element]],
         ],
         None,
     ],
 ] = {
-    "dataSpecification": _ReaderAndSetterForEmbeddedDataSpecification.read_and_set_data_specification,
     "dataSpecificationContent": _ReaderAndSetterForEmbeddedDataSpecification.read_and_set_data_specification_content,
+    "dataSpecification": _ReaderAndSetterForEmbeddedDataSpecification.read_and_set_data_specification,
 }
 
 
 #: Dispatch XML property name to read & set method in
 #: :py:class:`_ReaderAndSetterForLevelType`
 _READ_AND_SET_DISPATCH_FOR_LEVEL_TYPE: Mapping[
     str,
@@ -26166,22 +26161,23 @@
         XML elements.
 
         Each element in the sequence corresponds to a property. If no properties
         are set, nothing is written to the :py:attr:`~stream`.
 
         :param that: instance to be serialized
         """
-        self._write_start_element("dataSpecification")
-        self._write_reference_as_sequence(that.data_specification)
-        self._write_end_element("dataSpecification")
-
         self._write_start_element("dataSpecificationContent")
         self.visit(that.data_specification_content)
         self._write_end_element("dataSpecificationContent")
 
+        if that.data_specification is not None:
+            self._write_start_element("dataSpecification")
+            self._write_reference_as_sequence(that.data_specification)
+            self._write_end_element("dataSpecification")
+
     def visit_embedded_data_specification(
         self, that: aas_types.EmbeddedDataSpecification
     ) -> None:
         """
         Serialize :paramref:`that` to :py:attr:`~stream` as an XML element.
 
         The enclosing XML element designates the class of the instance, where its
```

### Comparing `aas-core3.0-1.0.3/aas_core3.0.egg-info/PKG-INFO` & `aas_core3_0-1.0.4/aas_core3.0.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: aas-core3.0
-Version: 1.0.3
+Version: 1.0.4
 Summary: Manipulate, verify and de/serialize Asset Administration Shells.
 Home-page: https://github.com/aas-core-works/aas-core3.0-python
 Author: Marko Ristin
 Author-email: marko@ristin.ch
 License: License :: OSI Approved :: MIT License
 Keywords: asset administration shell sdk industry 4.0 industrie i4.0 industry iot iiot
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 License-File: LICENSE
+License-File: AUTHORS
 
 **********************
 aas-core3.0-python
 **********************
 
 .. image:: https://github.com/aas-core-works/aas-core3.0-python/actions/workflows/ci.yml/badge.svg
     :target: https://github.com/aas-core-works/aas-core3.0-python/actions/workflows/ci.yml
```

### Comparing `aas-core3.0-1.0.3/aas_core3.0.egg-info/SOURCES.txt` & `aas_core3_0-1.0.4/aas_core3.0.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+AUTHORS
 LICENSE
 README.rst
 setup.py
 aas_core3/__init__.py
 aas_core3/common.py
 aas_core3/constants.py
 aas_core3/jsonization.py
```

### Comparing `aas-core3.0-1.0.3/dev_scripts/test_codegen/common.py` & `aas_core3_0-1.0.4/dev_scripts/test_codegen/common.py`

 * *Files identical despite different names*

### Comparing `aas-core3.0-1.0.3/dev_scripts/test_codegen/generate_all.py` & `aas_core3_0-1.0.4/dev_scripts/test_codegen/generate_all.py`

 * *Files identical despite different names*

### Comparing `aas-core3.0-1.0.3/dev_scripts/test_codegen/generate_common_jsonization.py` & `aas_core3_0-1.0.4/dev_scripts/test_codegen/generate_common_jsonization.py`

 * *Files identical despite different names*

### Comparing `aas-core3.0-1.0.3/dev_scripts/test_codegen/generate_test_for_descend_and_pass_through_visitor.py` & `aas_core3_0-1.0.4/dev_scripts/test_codegen/generate_test_for_descend_and_pass_through_visitor.py`

 * *Files identical despite different names*

### Comparing `aas-core3.0-1.0.3/dev_scripts/test_codegen/generate_test_for_descend_once.py` & `aas_core3_0-1.0.4/dev_scripts/test_codegen/generate_test_for_descend_once.py`

 * *Files identical despite different names*

### Comparing `aas-core3.0-1.0.3/dev_scripts/test_codegen/generate_test_for_jsonization_of_classes_with_descendants.py` & `aas_core3_0-1.0.4/dev_scripts/test_codegen/generate_test_for_jsonization_of_classes_with_descendants.py`

 * *Files identical despite different names*

### Comparing `aas-core3.0-1.0.3/dev_scripts/test_codegen/generate_test_for_jsonization_of_concrete_classes.py` & `aas_core3_0-1.0.4/dev_scripts/test_codegen/generate_test_for_jsonization_of_concrete_classes.py`

 * *Files identical despite different names*

### Comparing `aas-core3.0-1.0.3/dev_scripts/test_codegen/generate_test_for_jsonization_of_concrete_classes_outside_container.py` & `aas_core3_0-1.0.4/dev_scripts/test_codegen/generate_test_for_jsonization_of_concrete_classes_outside_container.py`

 * *Files identical despite different names*

### Comparing `aas-core3.0-1.0.3/dev_scripts/test_codegen/generate_test_for_jsonization_of_enums.py` & `aas_core3_0-1.0.4/dev_scripts/test_codegen/generate_test_for_jsonization_of_enums.py`

 * *Files identical despite different names*

### Comparing `aas-core3.0-1.0.3/dev_scripts/test_codegen/generate_test_for_over_X_or_empty.py` & `aas_core3_0-1.0.4/dev_scripts/test_codegen/generate_test_for_over_X_or_empty.py`

 * *Files identical despite different names*

### Comparing `aas-core3.0-1.0.3/dev_scripts/test_codegen/generate_test_for_x_or_default.py` & `aas_core3_0-1.0.4/dev_scripts/test_codegen/generate_test_for_x_or_default.py`

 * *Files identical despite different names*

### Comparing `aas-core3.0-1.0.3/dev_scripts/test_codegen/generate_test_for_xmlization_of_classes_with_descendants.py` & `aas_core3_0-1.0.4/dev_scripts/test_codegen/generate_test_for_xmlization_of_classes_with_descendants.py`

 * *Files identical despite different names*

### Comparing `aas-core3.0-1.0.3/dev_scripts/test_codegen/generate_test_for_xmlization_of_concrete_classes.py` & `aas_core3_0-1.0.4/dev_scripts/test_codegen/generate_test_for_xmlization_of_concrete_classes.py`

 * *Files identical despite different names*

### Comparing `aas-core3.0-1.0.3/dev_scripts/test_codegen/generate_test_for_xmlization_of_concrete_classes_outside_container.py` & `aas_core3_0-1.0.4/dev_scripts/test_codegen/generate_test_for_xmlization_of_concrete_classes_outside_container.py`

 * *Files identical despite different names*

### Comparing `aas-core3.0-1.0.3/dev_scripts/test_codegen/test_data_io.py` & `aas_core3_0-1.0.4/dev_scripts/test_codegen/test_data_io.py`

 * *Files identical despite different names*

### Comparing `aas-core3.0-1.0.3/setup.py` & `aas_core3_0-1.0.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 with open(os.path.join(here, "README.rst"), encoding="utf-8") as fid:
     long_description = fid.read()
 
 setup(
     name="aas-core3.0",
     # Synchronize with __init__.py and changelog.rst!
-    version="1.0.3",
+    version="1.0.4",
     description="Manipulate, verify and de/serialize Asset Administration Shells.",
     long_description=long_description,
     url="https://github.com/aas-core-works/aas-core3.0-python",
     author="Marko Ristin",
     author_email="marko@ristin.ch",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
```

### Comparing `aas-core3.0-1.0.3/tests/test_descend_and_pass_through_visitor.py` & `aas_core3_0-1.0.4/tests/test_descend_and_pass_through_visitor.py`

 * *Files identical despite different names*

### Comparing `aas-core3.0-1.0.3/tests/test_descend_once.py` & `aas_core3_0-1.0.4/tests/test_descend_once.py`

 * *Files identical despite different names*

### Comparing `aas-core3.0-1.0.3/tests/test_jsonization_of_classes_with_descendants.py` & `aas_core3_0-1.0.4/tests/test_jsonization_of_classes_with_descendants.py`

 * *Files identical despite different names*

### Comparing `aas-core3.0-1.0.3/tests/test_jsonization_of_concrete_classes.py` & `aas_core3_0-1.0.4/tests/test_jsonization_of_concrete_classes.py`

 * *Files identical despite different names*

### Comparing `aas-core3.0-1.0.3/tests/test_jsonization_of_concrete_classes_outside_container.py` & `aas_core3_0-1.0.4/tests/test_jsonization_of_concrete_classes_outside_container.py`

 * *Files identical despite different names*

### Comparing `aas-core3.0-1.0.3/tests/test_jsonization_of_enums.py` & `aas_core3_0-1.0.4/tests/test_jsonization_of_enums.py`

 * *Files identical despite different names*

### Comparing `aas-core3.0-1.0.3/tests/test_over_x_or_empty.py` & `aas_core3_0-1.0.4/tests/test_over_x_or_empty.py`

 * *Files identical despite different names*

### Comparing `aas-core3.0-1.0.3/tests/test_x_or_default.py` & `aas_core3_0-1.0.4/tests/test_x_or_default.py`

 * *Files identical despite different names*

### Comparing `aas-core3.0-1.0.3/tests/test_xmlization_of_classes_with_descendants.py` & `aas_core3_0-1.0.4/tests/test_xmlization_of_classes_with_descendants.py`

 * *Files identical despite different names*

### Comparing `aas-core3.0-1.0.3/tests/test_xmlization_of_concrete_classes.py` & `aas_core3_0-1.0.4/tests/test_xmlization_of_concrete_classes.py`

 * *Files identical despite different names*

### Comparing `aas-core3.0-1.0.3/tests/test_xmlization_of_concrete_classes_outside_container.py` & `aas_core3_0-1.0.4/tests/test_xmlization_of_concrete_classes_outside_container.py`

 * *Files identical despite different names*

### Comparing `aas-core3.0-1.0.3/tests/test_xmlization_when_text_attached_to_end_element.py` & `aas_core3_0-1.0.4/tests/test_xmlization_when_text_attached_to_end_element.py`

 * *Files identical despite different names*

