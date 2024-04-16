# Comparing `tmp/twinn-ml-interface-0.3.1.dev0.tar.gz` & `tmp/twinn_ml_interface-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twinn-ml-interface-0.3.1.dev0.tar", last modified: Mon Mar 11 08:46:09 2024, max compression
+gzip compressed data, was "twinn_ml_interface-0.3.2.tar", last modified: Tue Apr 16 08:40:52 2024, max compression
```

## Comparing `twinn-ml-interface-0.3.1.dev0.tar` & `twinn_ml_interface-0.3.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 08:46:09.484867 twinn-ml-interface-0.3.1.dev0/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-03-11 08:46:05.000000 twinn-ml-interface-0.3.1.dev0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-03-11 08:46:09.484867 twinn-ml-interface-0.3.1.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3515 2024-03-11 08:46:05.000000 twinn-ml-interface-0.3.1.dev0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-03-11 08:46:05.000000 twinn-ml-interface-0.3.1.dev0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-11 08:46:09.484867 twinn-ml-interface-0.3.1.dev0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 08:46:09.480867 twinn-ml-interface-0.3.1.dev0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-03-11 08:46:05.000000 twinn-ml-interface-0.3.1.dev0/tests/test_input_data_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-03-11 08:46:05.000000 twinn-ml-interface-0.3.1.dev0/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-03-11 08:46:05.000000 twinn-ml-interface-0.3.1.dev0/tests/test_mocks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 08:46:09.480867 twinn-ml-interface-0.3.1.dev0/twinn_ml_interface/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 08:46:05.000000 twinn-ml-interface-0.3.1.dev0/twinn_ml_interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-11 08:46:05.000000 twinn-ml-interface-0.3.1.dev0/twinn_ml_interface/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 08:46:09.480867 twinn-ml-interface-0.3.1.dev0/twinn_ml_interface/input_data/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-11 08:46:05.000000 twinn-ml-interface-0.3.1.dev0/twinn_ml_interface/input_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4753 2024-03-11 08:46:05.000000 twinn-ml-interface-0.3.1.dev0/twinn_ml_interface/input_data/input_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-03-11 08:46:05.000000 twinn-ml-interface-0.3.1.dev0/twinn_ml_interface/input_data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 08:46:09.480867 twinn-ml-interface-0.3.1.dev0/twinn_ml_interface/interface/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-03-11 08:46:05.000000 twinn-ml-interface-0.3.1.dev0/twinn_ml_interface/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5741 2024-03-11 08:46:05.000000 twinn-ml-interface-0.3.1.dev0/twinn_ml_interface/interface/model_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-03-11 08:46:05.000000 twinn-ml-interface-0.3.1.dev0/twinn_ml_interface/interface/model_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 08:46:09.480867 twinn-ml-interface-0.3.1.dev0/twinn_ml_interface/interface_validation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 08:46:05.000000 twinn-ml-interface-0.3.1.dev0/twinn_ml_interface/interface_validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-11 08:46:05.000000 twinn-ml-interface-0.3.1.dev0/twinn_ml_interface/interface_validation/mock_predict_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-11 08:46:05.000000 twinn-ml-interface-0.3.1.dev0/twinn_ml_interface/interface_validation/mock_train_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-03-11 08:46:05.000000 twinn-ml-interface-0.3.1.dev0/twinn_ml_interface/interface_validation/test_model_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 08:46:09.480867 twinn-ml-interface-0.3.1.dev0/twinn_ml_interface/mocks/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-03-11 08:46:05.000000 twinn-ml-interface-0.3.1.dev0/twinn_ml_interface/mocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7145 2024-03-11 08:46:05.000000 twinn-ml-interface-0.3.1.dev0/twinn_ml_interface/mocks/mocks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 08:46:09.484867 twinn-ml-interface-0.3.1.dev0/twinn_ml_interface/objectmodels/
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-03-11 08:46:05.000000 twinn-ml-interface-0.3.1.dev0/twinn_ml_interface/objectmodels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-03-11 08:46:05.000000 twinn-ml-interface-0.3.1.dev0/twinn_ml_interface/objectmodels/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-03-11 08:46:05.000000 twinn-ml-interface-0.3.1.dev0/twinn_ml_interface/objectmodels/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-03-11 08:46:05.000000 twinn-ml-interface-0.3.1.dev0/twinn_ml_interface/objectmodels/hierarchy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5574 2024-03-11 08:46:05.000000 twinn-ml-interface-0.3.1.dev0/twinn_ml_interface/objectmodels/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-03-11 08:46:05.000000 twinn-ml-interface-0.3.1.dev0/twinn_ml_interface/objectmodels/model_flags.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 08:46:09.484867 twinn-ml-interface-0.3.1.dev0/twinn_ml_interface.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-03-11 08:46:09.000000 twinn-ml-interface-0.3.1.dev0/twinn_ml_interface.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-03-11 08:46:09.000000 twinn-ml-interface-0.3.1.dev0/twinn_ml_interface.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 08:46:09.000000 twinn-ml-interface-0.3.1.dev0/twinn_ml_interface.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-11 08:46:09.000000 twinn-ml-interface-0.3.1.dev0/twinn_ml_interface.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-11 08:46:09.000000 twinn-ml-interface-0.3.1.dev0/twinn_ml_interface.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:40:52.891383 twinn_ml_interface-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-16 08:40:46.000000 twinn_ml_interface-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-04-16 08:40:52.891383 twinn_ml_interface-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3515 2024-04-16 08:40:46.000000 twinn_ml_interface-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-16 08:40:46.000000 twinn_ml_interface-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 08:40:52.891383 twinn_ml_interface-0.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:40:52.887383 twinn_ml_interface-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-04-16 08:40:46.000000 twinn_ml_interface-0.3.2/tests/test_input_data_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-04-16 08:40:46.000000 twinn_ml_interface-0.3.2/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-16 08:40:46.000000 twinn_ml_interface-0.3.2/tests/test_mocks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:40:52.887383 twinn_ml_interface-0.3.2/twinn_ml_interface/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 08:40:46.000000 twinn_ml_interface-0.3.2/twinn_ml_interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-16 08:40:46.000000 twinn_ml_interface-0.3.2/twinn_ml_interface/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:40:52.891383 twinn_ml_interface-0.3.2/twinn_ml_interface/input_data/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-16 08:40:46.000000 twinn_ml_interface-0.3.2/twinn_ml_interface/input_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4753 2024-04-16 08:40:46.000000 twinn_ml_interface-0.3.2/twinn_ml_interface/input_data/input_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-16 08:40:46.000000 twinn_ml_interface-0.3.2/twinn_ml_interface/input_data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:40:52.891383 twinn_ml_interface-0.3.2/twinn_ml_interface/interface/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-16 08:40:46.000000 twinn_ml_interface-0.3.2/twinn_ml_interface/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5741 2024-04-16 08:40:46.000000 twinn_ml_interface-0.3.2/twinn_ml_interface/interface/model_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-16 08:40:46.000000 twinn_ml_interface-0.3.2/twinn_ml_interface/interface/model_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:40:52.891383 twinn_ml_interface-0.3.2/twinn_ml_interface/interface_validation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 08:40:46.000000 twinn_ml_interface-0.3.2/twinn_ml_interface/interface_validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-16 08:40:46.000000 twinn_ml_interface-0.3.2/twinn_ml_interface/interface_validation/mock_predict_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-16 08:40:46.000000 twinn_ml_interface-0.3.2/twinn_ml_interface/interface_validation/mock_train_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-16 08:40:46.000000 twinn_ml_interface-0.3.2/twinn_ml_interface/interface_validation/test_model_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:40:52.891383 twinn_ml_interface-0.3.2/twinn_ml_interface/mocks/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-16 08:40:46.000000 twinn_ml_interface-0.3.2/twinn_ml_interface/mocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7145 2024-04-16 08:40:46.000000 twinn_ml_interface-0.3.2/twinn_ml_interface/mocks/mocks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:40:52.891383 twinn_ml_interface-0.3.2/twinn_ml_interface/objectmodels/
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-16 08:40:46.000000 twinn_ml_interface-0.3.2/twinn_ml_interface/objectmodels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-16 08:40:46.000000 twinn_ml_interface-0.3.2/twinn_ml_interface/objectmodels/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-04-16 08:40:46.000000 twinn_ml_interface-0.3.2/twinn_ml_interface/objectmodels/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4220 2024-04-16 08:40:46.000000 twinn_ml_interface-0.3.2/twinn_ml_interface/objectmodels/hierarchy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5574 2024-04-16 08:40:46.000000 twinn_ml_interface-0.3.2/twinn_ml_interface/objectmodels/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-16 08:40:46.000000 twinn_ml_interface-0.3.2/twinn_ml_interface/objectmodels/model_flags.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:40:52.891383 twinn_ml_interface-0.3.2/twinn_ml_interface.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-04-16 08:40:52.000000 twinn_ml_interface-0.3.2/twinn_ml_interface.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-04-16 08:40:52.000000 twinn_ml_interface-0.3.2/twinn_ml_interface.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 08:40:52.000000 twinn_ml_interface-0.3.2/twinn_ml_interface.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 08:40:52.000000 twinn_ml_interface-0.3.2/twinn_ml_interface.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-16 08:40:52.000000 twinn_ml_interface-0.3.2/twinn_ml_interface.egg-info/top_level.txt
```

### Comparing `twinn-ml-interface-0.3.1.dev0/LICENSE` & `twinn_ml_interface-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `twinn-ml-interface-0.3.1.dev0/PKG-INFO` & `twinn_ml_interface-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twinn-ml-interface
-Version: 0.3.1.dev0
+Version: 0.3.2
 Summary: Machine learning model contracts with machine learning infrastructure
 License: MIT
 Project-URL: homepage, https://github.com/RoyalHaskoningDHV/twinn-ml-interface
 Project-URL: issues, https://github.com/RoyalHaskoningDHV/twinn-ml-interface/issues
 Project-URL: discussions, https://github.com/RoyalHaskoningDHV/twinn-ml-interface/discussions
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `twinn-ml-interface-0.3.1.dev0/README.md` & `twinn_ml_interface-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `twinn-ml-interface-0.3.1.dev0/pyproject.toml` & `twinn_ml_interface-0.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `twinn-ml-interface-0.3.1.dev0/tests/test_input_data_class.py` & `twinn_ml_interface-0.3.2/tests/test_input_data_class.py`

 * *Files identical despite different names*

### Comparing `twinn-ml-interface-0.3.1.dev0/tests/test_logging.py` & `twinn_ml_interface-0.3.2/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `twinn-ml-interface-0.3.1.dev0/twinn_ml_interface/input_data/input_data.py` & `twinn_ml_interface-0.3.2/twinn_ml_interface/input_data/input_data.py`

 * *Files identical despite different names*

### Comparing `twinn-ml-interface-0.3.1.dev0/twinn_ml_interface/input_data/utils.py` & `twinn_ml_interface-0.3.2/twinn_ml_interface/input_data/utils.py`

 * *Files identical despite different names*

### Comparing `twinn-ml-interface-0.3.1.dev0/twinn_ml_interface/interface/model_interfaces.py` & `twinn_ml_interface-0.3.2/twinn_ml_interface/interface/model_interfaces.py`

 * *Files identical despite different names*

### Comparing `twinn-ml-interface-0.3.1.dev0/twinn_ml_interface/interface/model_test.py` & `twinn_ml_interface-0.3.2/twinn_ml_interface/interface/model_test.py`

 * *Files identical despite different names*

### Comparing `twinn-ml-interface-0.3.1.dev0/twinn_ml_interface/mocks/mocks.py` & `twinn_ml_interface-0.3.2/twinn_ml_interface/mocks/mocks.py`

 * *Files identical despite different names*

### Comparing `twinn-ml-interface-0.3.1.dev0/twinn_ml_interface/objectmodels/__init__.py` & `twinn_ml_interface-0.3.2/twinn_ml_interface/objectmodels/__init__.py`

 * *Files identical despite different names*

### Comparing `twinn-ml-interface-0.3.1.dev0/twinn_ml_interface/objectmodels/configuration.py` & `twinn_ml_interface-0.3.2/twinn_ml_interface/objectmodels/configuration.py`

 * *Files identical despite different names*

### Comparing `twinn-ml-interface-0.3.1.dev0/twinn_ml_interface/objectmodels/exceptions.py` & `twinn_ml_interface-0.3.2/twinn_ml_interface/objectmodels/exceptions.py`

 * *Files identical despite different names*

### Comparing `twinn-ml-interface-0.3.1.dev0/twinn_ml_interface/objectmodels/hierarchy.py` & `twinn_ml_interface-0.3.2/twinn_ml_interface/objectmodels/hierarchy.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,15 @@
         unit, tag = unit_tag.split(separator)
         return cls(Unit(unit, "UNKNOWN", True), Tag(tag))
 
     def __str__(self) -> str:
         return f"{self.unit.unit_code}:{self.tag.to_string(self.unit.unit_type_code)}"
 
     def __hash__(self):
-        return hash(f"{self.unit}:{self.tag}")
+        return hash(self.__str__())
 
 
 @dataclass
 class UnitTagTemplate:
     relative_path: list[RelativeType]
     tags: list[Tag]
```

### Comparing `twinn-ml-interface-0.3.1.dev0/twinn_ml_interface/objectmodels/logging.py` & `twinn_ml_interface-0.3.2/twinn_ml_interface/objectmodels/logging.py`

 * *Files identical despite different names*

### Comparing `twinn-ml-interface-0.3.1.dev0/twinn_ml_interface.egg-info/PKG-INFO` & `twinn_ml_interface-0.3.2/twinn_ml_interface.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twinn-ml-interface
-Version: 0.3.1.dev0
+Version: 0.3.2
 Summary: Machine learning model contracts with machine learning infrastructure
 License: MIT
 Project-URL: homepage, https://github.com/RoyalHaskoningDHV/twinn-ml-interface
 Project-URL: issues, https://github.com/RoyalHaskoningDHV/twinn-ml-interface/issues
 Project-URL: discussions, https://github.com/RoyalHaskoningDHV/twinn-ml-interface/discussions
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `twinn-ml-interface-0.3.1.dev0/twinn_ml_interface.egg-info/SOURCES.txt` & `twinn_ml_interface-0.3.2/twinn_ml_interface.egg-info/SOURCES.txt`

 * *Files identical despite different names*

