# Comparing `tmp/river_core-1.4.2.tar.gz` & `tmp/river_core-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/river_core-1.4.2.tar", last modified: Tue Mar 26 07:10:38 2024, max compression
+gzip compressed data, was "dist/river_core-1.4.3.tar", last modified: Tue Apr 16 05:21:32 2024, max compression
```

## Comparing `river_core-1.4.2.tar` & `river_core-1.4.3.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:10:38.000000 river_core-1.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-03-26 07:10:24.000000 river_core-1.4.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-03-26 07:10:24.000000 river_core-1.4.2/LICENSE.incore
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-03-26 07:10:24.000000 river_core-1.4.2/LICENSE.tessolve
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-03-26 07:10:24.000000 river_core-1.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-03-26 07:10:38.000000 river_core-1.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-03-26 07:10:24.000000 river_core-1.4.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:10:38.000000 river_core-1.4.2/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-03-26 07:10:24.000000 river_core-1.4.2/examples/sample-config.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:10:38.000000 river_core-1.4.2/river_core/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-03-26 07:10:24.000000 river_core-1.4.2/river_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-03-26 07:10:24.000000 river_core-1.4.2/river_core/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-03-26 07:10:24.000000 river_core-1.4.2/river_core/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     7498 2024-03-26 07:10:24.000000 river_core-1.4.2/river_core/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-03-26 07:10:24.000000 river_core-1.4.2/river_core/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)    42234 2024-03-26 07:10:24.000000 river_core-1.4.2/river_core/rivercore.py
--rw-r--r--   0 runner    (1001) docker     (127)     6401 2024-03-26 07:10:24.000000 river_core-1.4.2/river_core/sim_hookspecs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:10:38.000000 river_core-1.4.2/river_core/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-03-26 07:10:24.000000 river_core-1.4.2/river_core/templates/coverage_report.html
--rw-r--r--   0 runner    (1001) docker     (127)    14632 2024-03-26 07:10:24.000000 river_core-1.4.2/river_core/templates/report.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:10:38.000000 river_core-1.4.2/river_core/templates/setup/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:10:38.000000 river_core-1.4.2/river_core/templates/setup/dut/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:10:24.000000 river_core-1.4.2/river_core/templates/setup/dut/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:10:38.000000 river_core-1.4.2/river_core/templates/setup/dut/boot/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-26 07:10:24.000000 river_core-1.4.2/river_core/templates/setup/dut/boot/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-03-26 07:10:24.000000 river_core-1.4.2/river_core/templates/setup/dut/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-03-26 07:10:24.000000 river_core-1.4.2/river_core/templates/setup/dut/gen_framework.py
--rw-r--r--   0 runner    (1001) docker     (127)     8461 2024-03-26 07:10:24.000000 river_core-1.4.2/river_core/templates/setup/dut/sample_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:10:38.000000 river_core-1.4.2/river_core/templates/setup/generator/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:10:24.000000 river_core-1.4.2/river_core/templates/setup/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-03-26 07:10:24.000000 river_core-1.4.2/river_core/templates/setup/generator/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-03-26 07:10:24.000000 river_core-1.4.2/river_core/templates/setup/generator/gen_framework.py
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-03-26 07:10:24.000000 river_core-1.4.2/river_core/templates/setup/generator/sample_gen_config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6026 2024-03-26 07:10:24.000000 river_core-1.4.2/river_core/templates/setup/generator/sample_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:10:38.000000 river_core-1.4.2/river_core/templates/setup/reference/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:10:24.000000 river_core-1.4.2/river_core/templates/setup/reference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-03-26 07:10:24.000000 river_core-1.4.2/river_core/templates/setup/reference/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-03-26 07:10:24.000000 river_core-1.4.2/river_core/templates/setup/reference/gen_framework.py
--rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-03-26 07:10:24.000000 river_core-1.4.2/river_core/templates/setup/reference/sample_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4074 2024-03-26 07:10:24.000000 river_core-1.4.2/river_core/templates/style.css
--rw-r--r--   0 runner    (1001) docker     (127)    18588 2024-03-26 07:10:24.000000 river_core-1.4.2/river_core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:10:38.000000 river_core-1.4.2/river_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-03-26 07:10:38.000000 river_core-1.4.2/river_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-03-26 07:10:38.000000 river_core-1.4.2/river_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 07:10:38.000000 river_core-1.4.2/river_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-26 07:10:38.000000 river_core-1.4.2/river_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 07:10:38.000000 river_core-1.4.2/river_core.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-03-26 07:10:38.000000 river_core-1.4.2/river_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-26 07:10:38.000000 river_core-1.4.2/river_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-03-26 07:10:38.000000 river_core-1.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-03-26 07:10:24.000000 river_core-1.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:21:32.000000 river_core-1.4.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-04-16 05:21:18.000000 river_core-1.4.3/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-16 05:21:18.000000 river_core-1.4.3/LICENSE.incore
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-16 05:21:18.000000 river_core-1.4.3/LICENSE.tessolve
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-16 05:21:18.000000 river_core-1.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-16 05:21:32.000000 river_core-1.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-16 05:21:18.000000 river_core-1.4.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:21:32.000000 river_core-1.4.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-04-16 05:21:18.000000 river_core-1.4.3/examples/sample-config.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:21:32.000000 river_core-1.4.3/river_core/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-16 05:21:18.000000 river_core-1.4.3/river_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-04-16 05:21:18.000000 river_core-1.4.3/river_core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-04-16 05:21:18.000000 river_core-1.4.3/river_core/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7498 2024-04-16 05:21:18.000000 river_core-1.4.3/river_core/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-16 05:21:18.000000 river_core-1.4.3/river_core/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    42358 2024-04-16 05:21:18.000000 river_core-1.4.3/river_core/rivercore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6401 2024-04-16 05:21:18.000000 river_core-1.4.3/river_core/sim_hookspecs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:21:32.000000 river_core-1.4.3/river_core/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-04-16 05:21:18.000000 river_core-1.4.3/river_core/templates/coverage_report.html
+-rw-r--r--   0 runner    (1001) docker     (127)    14632 2024-04-16 05:21:18.000000 river_core-1.4.3/river_core/templates/report.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:21:32.000000 river_core-1.4.3/river_core/templates/setup/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:21:32.000000 river_core-1.4.3/river_core/templates/setup/dut/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 05:21:18.000000 river_core-1.4.3/river_core/templates/setup/dut/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:21:32.000000 river_core-1.4.3/river_core/templates/setup/dut/boot/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-16 05:21:18.000000 river_core-1.4.3/river_core/templates/setup/dut/boot/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-16 05:21:18.000000 river_core-1.4.3/river_core/templates/setup/dut/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-16 05:21:18.000000 river_core-1.4.3/river_core/templates/setup/dut/gen_framework.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8461 2024-04-16 05:21:18.000000 river_core-1.4.3/river_core/templates/setup/dut/sample_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:21:32.000000 river_core-1.4.3/river_core/templates/setup/generator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 05:21:18.000000 river_core-1.4.3/river_core/templates/setup/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-16 05:21:18.000000 river_core-1.4.3/river_core/templates/setup/generator/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-04-16 05:21:18.000000 river_core-1.4.3/river_core/templates/setup/generator/gen_framework.py
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-16 05:21:18.000000 river_core-1.4.3/river_core/templates/setup/generator/sample_gen_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6026 2024-04-16 05:21:18.000000 river_core-1.4.3/river_core/templates/setup/generator/sample_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:21:32.000000 river_core-1.4.3/river_core/templates/setup/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 05:21:18.000000 river_core-1.4.3/river_core/templates/setup/reference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-16 05:21:18.000000 river_core-1.4.3/river_core/templates/setup/reference/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-16 05:21:18.000000 river_core-1.4.3/river_core/templates/setup/reference/gen_framework.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-04-16 05:21:18.000000 river_core-1.4.3/river_core/templates/setup/reference/sample_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4074 2024-04-16 05:21:18.000000 river_core-1.4.3/river_core/templates/style.css
+-rw-r--r--   0 runner    (1001) docker     (127)    18760 2024-04-16 05:21:18.000000 river_core-1.4.3/river_core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:21:32.000000 river_core-1.4.3/river_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-16 05:21:32.000000 river_core-1.4.3/river_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-16 05:21:32.000000 river_core-1.4.3/river_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 05:21:32.000000 river_core-1.4.3/river_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-16 05:21:32.000000 river_core-1.4.3/river_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 05:21:32.000000 river_core-1.4.3/river_core.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-16 05:21:32.000000 river_core-1.4.3/river_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-16 05:21:32.000000 river_core-1.4.3/river_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-16 05:21:32.000000 river_core-1.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-04-16 05:21:18.000000 river_core-1.4.3/setup.py
```

### Comparing `river_core-1.4.2/CONTRIBUTING.rst` & `river_core-1.4.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `river_core-1.4.2/LICENSE.incore` & `river_core-1.4.3/LICENSE.incore`

 * *Files identical despite different names*

### Comparing `river_core-1.4.2/LICENSE.tessolve` & `river_core-1.4.3/LICENSE.tessolve`

 * *Files identical despite different names*

### Comparing `river_core-1.4.2/PKG-INFO` & `river_core-1.4.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: river_core
-Version: 1.4.2
+Version: 1.4.3
 Summary: RiVer Core Verification Framework
 Home-page: https://github.com/incoresemi/river_core
 Author: InCore Semiconductors Pvt. Ltd.; Tessolve
 Author-email: neelgala@incoresemi.com
 License: BSD-3-Clause
 Description: **RiVer Core** : RISC-V Core Verification Framework 
         ###################################################################################
```

### Comparing `river_core-1.4.2/examples/sample-config.ini` & `river_core-1.4.3/examples/sample-config.ini`

 * *Files identical despite different names*

### Comparing `river_core-1.4.2/river_core/constants.py` & `river_core-1.4.3/river_core/constants.py`

 * *Files identical despite different names*

### Comparing `river_core-1.4.2/river_core/log.py` & `river_core-1.4.3/river_core/log.py`

 * *Files identical despite different names*

### Comparing `river_core-1.4.2/river_core/main.py` & `river_core-1.4.3/river_core/main.py`

 * *Files identical despite different names*

### Comparing `river_core-1.4.2/river_core/rivercore.py` & `river_core-1.4.3/river_core/rivercore.py`

 * *Files 0% similar despite different names*

```diff
@@ -609,15 +609,16 @@
         if compare:
             test_dict = utils.load_yaml(test_list)
             gen_json_data = []
             target_json_data = []
             ref_json_data = []
             for test, attr in test_dict.items():
                 test_wd = attr['work_dir']
-                if not attr['self_checking']:
+                is_self_checking = attr['self_checking']
+                if not is_self_checking:
                   if not os.path.isfile(test_wd + '/dut.dump'):
                       logger.error(f'{test:<30} : DUT dump is missing')
                       test_dict[test]['result'] = 'Unavailable'
                       test_dict[test]['log'] = "DUT dump is missing"
                       success = False
                       continue
                   if not os.path.isfile(test_wd + '/ref.dump'):
@@ -631,17 +632,18 @@
                   if not os.path.isfile(test_wd + '/dut.signature'):
                       logger.error(f'{test:<30} : DUT signature is missing')
                       test_dict[test]['result'] = 'Unavailable'
                       test_dict[test]['log'] = "DUT signature is missing"
                       success = False
                       continue
                   result, log = utils.self_check(test_wd + '/dut.signature')
+                  insnsize = utils.get_file_size(test_wd + '/dut.dump')
+                test_dict[test]['num_instr'] = insnsize
                 test_dict[test]['result'] = result
                 test_dict[test]['log'] = log
-                test_dict[test]['num_instr'] = insnsize
                 if result == 'Passed':
                     logger.info(f"{test:<30} : TEST {result.upper()}")
                 else:
                     success = False
                     logger.error(f"{test:<30} : TEST {result.upper()}")
 
             utils.save_yaml(test_dict, output_dir+'/result_list.yaml')
```

### Comparing `river_core-1.4.2/river_core/sim_hookspecs.py` & `river_core-1.4.3/river_core/sim_hookspecs.py`

 * *Files identical despite different names*

### Comparing `river_core-1.4.2/river_core/templates/coverage_report.html` & `river_core-1.4.3/river_core/templates/coverage_report.html`

 * *Files identical despite different names*

### Comparing `river_core-1.4.2/river_core/templates/report.html` & `river_core-1.4.3/river_core/templates/report.html`

 * *Files identical despite different names*

### Comparing `river_core-1.4.2/river_core/templates/setup/dut/gen_framework.py` & `river_core-1.4.3/river_core/templates/setup/dut/gen_framework.py`

 * *Files identical despite different names*

### Comparing `river_core-1.4.2/river_core/templates/setup/dut/sample_plugin.py` & `river_core-1.4.3/river_core/templates/setup/dut/sample_plugin.py`

 * *Files identical despite different names*

### Comparing `river_core-1.4.2/river_core/templates/setup/generator/gen_framework.py` & `river_core-1.4.3/river_core/templates/setup/generator/gen_framework.py`

 * *Files identical despite different names*

### Comparing `river_core-1.4.2/river_core/templates/setup/generator/sample_plugin.py` & `river_core-1.4.3/river_core/templates/setup/generator/sample_plugin.py`

 * *Files identical despite different names*

### Comparing `river_core-1.4.2/river_core/templates/setup/reference/gen_framework.py` & `river_core-1.4.3/river_core/templates/setup/reference/gen_framework.py`

 * *Files identical despite different names*

### Comparing `river_core-1.4.2/river_core/templates/setup/reference/sample_plugin.py` & `river_core-1.4.3/river_core/templates/setup/reference/sample_plugin.py`

 * *Files identical despite different names*

### Comparing `river_core-1.4.2/river_core/templates/style.css` & `river_core-1.4.3/river_core/templates/style.css`

 * *Files identical despite different names*

### Comparing `river_core-1.4.2/river_core/utils.py` & `river_core-1.4.3/river_core/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,22 @@
     for lineno, line in enumerate(f):
       line_val = f'0x{line}'
       if int(line_val,0) != 0:
         result = 'Failed'
         rout = f'\nLine:{lineno} has a non-zero value indicating a fail'
   return result, rout
 
+def get_file_size(file):
+    '''
+    Function to give the number of lines
+    '''
+    with open(f'{file}','r') as fd:
+      rcount = len(fd.readlines())
+    return rcount
+
 def compare_signature(file1, file2):
     '''
         Function to check whether two signature files are equivalent. This funcion uses the
         :py:mod:`difflib` to perform the comparision and obtain the difference.
         :param file1: The path to the first signature.
         :param file2: The path to the second signature.
         :type file1: str
```

### Comparing `river_core-1.4.2/river_core.egg-info/PKG-INFO` & `river_core-1.4.3/river_core.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: river-core
-Version: 1.4.2
+Version: 1.4.3
 Summary: RiVer Core Verification Framework
 Home-page: https://github.com/incoresemi/river_core
 Author: InCore Semiconductors Pvt. Ltd.; Tessolve
 Author-email: neelgala@incoresemi.com
 License: BSD-3-Clause
 Description: **RiVer Core** : RISC-V Core Verification Framework 
         ###################################################################################
```

### Comparing `river_core-1.4.2/river_core.egg-info/SOURCES.txt` & `river_core-1.4.3/river_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `river_core-1.4.2/setup.py` & `river_core-1.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,10 +58,10 @@
         ]
     },
     setup_requires=setup_requirements,
     test_suite='',
     tests_require=test_requirements,
     url=
     'https://github.com/incoresemi/river_core',
-    version='1.4.2',
+    version='1.4.3',
     zip_safe=False,
 )
```

