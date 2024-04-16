# Comparing `tmp/midas-util-1.1.1.tar.gz` & `tmp/midas-util-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "midas-util-1.1.1.tar", last modified: Wed Nov 29 08:18:59 2023, max compression
+gzip compressed data, was "midas-util-1.1.2.tar", last modified: Tue Apr 16 06:20:14 2024, max compression
```

## Comparing `midas-util-1.1.1.tar` & `midas-util-1.1.2.tar`

### file list

```diff
@@ -1,28 +1,30 @@
-drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2023-11-29 08:18:59.153863 midas-util-1.1.1/
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     7648 2023-07-12 12:36:58.000000 midas-util-1.1.1/LICENSE
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     1988 2023-11-29 08:18:59.153863 midas-util-1.1.1/PKG-INFO
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     1019 2023-07-12 12:36:58.000000 midas-util-1.1.1/README.md
-drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2023-11-29 08:18:59.150529 midas-util-1.1.1/midas/
-drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2023-11-29 08:18:59.153863 midas-util-1.1.1/midas/util/
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)       50 2023-07-12 12:36:58.000000 midas-util-1.1.1/midas/util/__init__.py
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     7182 2023-07-12 12:36:58.000000 midas-util-1.1.1/midas/util/base_data_model.py
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     6230 2023-07-12 12:36:58.000000 midas-util-1.1.1/midas/util/base_data_module.py
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     6138 2023-07-12 12:36:58.000000 midas-util-1.1.1/midas/util/base_data_simulator.py
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     1199 2023-07-12 12:36:58.000000 midas-util-1.1.1/midas/util/compute_q.py
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     4440 2023-07-12 12:36:58.000000 midas-util-1.1.1/midas/util/config_util.py
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)       87 2023-07-12 12:36:58.000000 midas-util-1.1.1/midas/util/dateformat.py
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     3610 2023-07-12 12:36:58.000000 midas-util-1.1.1/midas/util/dict_util.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     9151 2023-07-12 12:36:58.000000 midas-util-1.1.1/midas/util/forecast_data_model.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     1869 2023-07-12 12:36:58.000000 midas-util-1.1.1/midas/util/logging.py
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)      225 2023-07-12 12:36:58.000000 midas-util-1.1.1/midas/util/print_format.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     2198 2023-07-12 12:36:58.000000 midas-util-1.1.1/midas/util/report_util.py
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)    16196 2023-11-29 07:58:53.000000 midas-util-1.1.1/midas/util/runtime_config.py
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)    12588 2023-09-22 09:32:49.000000 midas-util-1.1.1/midas/util/upgrade_module.py
-drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2023-11-29 08:18:59.153863 midas-util-1.1.1/midas_util.egg-info/
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     1988 2023-11-29 08:18:59.000000 midas-util-1.1.1/midas_util.egg-info/PKG-INFO
--rw-r--r--   0 sbalduin  (1000) wheel      (998)      579 2023-11-29 08:18:59.000000 midas-util-1.1.1/midas_util.egg-info/SOURCES.txt
--rw-r--r--   0 sbalduin  (1000) wheel      (998)        1 2023-11-29 08:18:59.000000 midas-util-1.1.1/midas_util.egg-info/dependency_links.txt
--rw-r--r--   0 sbalduin  (1000) wheel      (998)      124 2023-11-29 08:18:59.000000 midas-util-1.1.1/midas_util.egg-info/requires.txt
--rw-r--r--   0 sbalduin  (1000) wheel      (998)        6 2023-11-29 08:18:59.000000 midas-util-1.1.1/midas_util.egg-info/top_level.txt
--rw-r--r--   0 sbalduin  (1000) wheel      (998)       38 2023-11-29 08:18:59.153863 midas-util-1.1.1/setup.cfg
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     1603 2023-07-12 12:36:58.000000 midas-util-1.1.1/setup.py
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2024-04-16 06:20:14.909225 midas-util-1.1.2/
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     7648 2023-07-12 12:36:58.000000 midas-util-1.1.2/LICENSE
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     1988 2024-04-16 06:20:14.905892 midas-util-1.1.2/PKG-INFO
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     1019 2023-07-12 12:36:58.000000 midas-util-1.1.2/README.md
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2024-04-16 06:20:14.905892 midas-util-1.1.2/midas/
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2024-04-16 06:20:14.905892 midas-util-1.1.2/midas/util/
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)       50 2023-07-12 12:36:58.000000 midas-util-1.1.2/midas/util/__init__.py
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     7182 2023-07-12 12:36:58.000000 midas-util-1.1.2/midas/util/base_data_model.py
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     6230 2023-07-12 12:36:58.000000 midas-util-1.1.2/midas/util/base_data_module.py
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     6138 2023-07-12 12:36:58.000000 midas-util-1.1.2/midas/util/base_data_simulator.py
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     1199 2023-07-12 12:36:58.000000 midas-util-1.1.2/midas/util/compute_q.py
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     4440 2023-07-12 12:36:58.000000 midas-util-1.1.2/midas/util/config_util.py
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)       87 2023-07-12 12:36:58.000000 midas-util-1.1.2/midas/util/dateformat.py
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     3610 2023-07-12 12:36:58.000000 midas-util-1.1.2/midas/util/dict_util.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     9151 2023-07-12 12:36:58.000000 midas-util-1.1.2/midas/util/forecast_data_model.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     1869 2023-07-12 12:36:58.000000 midas-util-1.1.2/midas/util/logging.py
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)      225 2023-07-12 12:36:58.000000 midas-util-1.1.2/midas/util/print_format.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     2198 2023-07-12 12:36:58.000000 midas-util-1.1.2/midas/util/report_util.py
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)    16196 2023-11-29 09:54:18.000000 midas-util-1.1.2/midas/util/runtime_config.py
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)    12741 2024-04-16 06:19:32.000000 midas-util-1.1.2/midas/util/upgrade_module.py
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2024-04-16 06:20:14.905892 midas-util-1.1.2/midas_util.egg-info/
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     1988 2024-04-16 06:20:14.000000 midas-util-1.1.2/midas_util.egg-info/PKG-INFO
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)      609 2024-04-16 06:20:14.000000 midas-util-1.1.2/midas_util.egg-info/SOURCES.txt
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)        1 2024-04-16 06:20:14.000000 midas-util-1.1.2/midas_util.egg-info/dependency_links.txt
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)      124 2024-04-16 06:20:14.000000 midas-util-1.1.2/midas_util.egg-info/requires.txt
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)        6 2024-04-16 06:20:14.000000 midas-util-1.1.2/midas_util.egg-info/top_level.txt
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)       38 2024-04-16 06:20:14.909225 midas-util-1.1.2/setup.cfg
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     1603 2023-07-12 12:36:58.000000 midas-util-1.1.2/setup.py
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2024-04-16 06:20:14.905892 midas-util-1.1.2/tests/
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     4624 2023-07-12 12:36:58.000000 midas-util-1.1.2/tests/test_base_data_model.py
```

### Comparing `midas-util-1.1.1/LICENSE` & `midas-util-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `midas-util-1.1.1/PKG-INFO` & `midas-util-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: midas-util
-Version: 1.1.1
+Version: 1.1.2
 Summary: A collection of utility functions for MIDAS.
 Home-page: https://gitlab.com/midas-mosaik/midas-util
 Author: Stephan Balduin
 Author-email: stephan.balduin@offis.de
 License: LGPL
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `midas-util-1.1.1/README.md` & `midas-util-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `midas-util-1.1.1/midas/util/base_data_model.py` & `midas-util-1.1.2/midas/util/base_data_model.py`

 * *Files identical despite different names*

### Comparing `midas-util-1.1.1/midas/util/base_data_module.py` & `midas-util-1.1.2/midas/util/base_data_module.py`

 * *Files identical despite different names*

### Comparing `midas-util-1.1.1/midas/util/base_data_simulator.py` & `midas-util-1.1.2/midas/util/base_data_simulator.py`

 * *Files identical despite different names*

### Comparing `midas-util-1.1.1/midas/util/compute_q.py` & `midas-util-1.1.2/midas/util/compute_q.py`

 * *Files identical despite different names*

### Comparing `midas-util-1.1.1/midas/util/config_util.py` & `midas-util-1.1.2/midas/util/config_util.py`

 * *Files identical despite different names*

### Comparing `midas-util-1.1.1/midas/util/dict_util.py` & `midas-util-1.1.2/midas/util/dict_util.py`

 * *Files identical despite different names*

### Comparing `midas-util-1.1.1/midas/util/forecast_data_model.py` & `midas-util-1.1.2/midas/util/forecast_data_model.py`

 * *Files identical despite different names*

### Comparing `midas-util-1.1.1/midas/util/logging.py` & `midas-util-1.1.2/midas/util/logging.py`

 * *Files identical despite different names*

### Comparing `midas-util-1.1.1/midas/util/report_util.py` & `midas-util-1.1.2/midas/util/report_util.py`

 * *Files identical despite different names*

### Comparing `midas-util-1.1.1/midas/util/runtime_config.py` & `midas-util-1.1.2/midas/util/runtime_config.py`

 * *Files identical despite different names*

### Comparing `midas-util-1.1.1/midas/util/upgrade_module.py` & `midas-util-1.1.2/midas/util/upgrade_module.py`

 * *Files 2% similar despite different names*

```diff
@@ -217,17 +217,21 @@
         self.sim_key = self.scenario.generate_sim_key(self)
 
         # Start the simulator if it was not started before
         if not self.scenario.sim_started(self.sim_key):
             self.scenario.add_sim(
                 self.sim_key, self.world.start(**self.sim_params)
             )
+            try:
+                sid = getattr(self.scenario.get_sim(self.sim_key), "_sid")
+            except AttributeError:
+                sid = getattr(self.scenario.get_sim(self.sim_key), "_sim").sid
             self.logger.debug(
                 "Started simulator %s (key: %s).",
-                getattr(self.scenario.get_sim(self.sim_key), "_sim").sid,
+                sid,
                 self.sim_key,
             )
             self.scenario.script.definitions.append(
                 f"{self.sim_key}_params = {self.sim_params}\n"
             )
             self.scenario.script.sim_start.append(
                 f"{self.sim_key} = world.start(**{self.sim_key}_params)\n"
```

### Comparing `midas-util-1.1.1/midas_util.egg-info/PKG-INFO` & `midas-util-1.1.2/midas_util.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: midas-util
-Version: 1.1.1
+Version: 1.1.2
 Summary: A collection of utility functions for MIDAS.
 Home-page: https://gitlab.com/midas-mosaik/midas-util
 Author: Stephan Balduin
 Author-email: stephan.balduin@offis.de
 License: LGPL
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `midas-util-1.1.1/midas_util.egg-info/SOURCES.txt` & `midas-util-1.1.2/midas_util.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -15,8 +15,9 @@
 midas/util/report_util.py
 midas/util/runtime_config.py
 midas/util/upgrade_module.py
 midas_util.egg-info/PKG-INFO
 midas_util.egg-info/SOURCES.txt
 midas_util.egg-info/dependency_links.txt
 midas_util.egg-info/requires.txt
-midas_util.egg-info/top_level.txt
+midas_util.egg-info/top_level.txt
+tests/test_base_data_model.py
```

### Comparing `midas-util-1.1.1/setup.py` & `midas-util-1.1.2/setup.py`

 * *Files identical despite different names*

