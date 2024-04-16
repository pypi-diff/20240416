# Comparing `tmp/efootprint-2.0.3.tar.gz` & `tmp/efootprint-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "efootprint-2.0.3.tar", max compression
+gzip compressed data, was "efootprint-2.0.4.tar", max compression
```

## Comparing `efootprint-2.0.3.tar` & `efootprint-2.0.4.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0    34522 2023-10-17 09:49:47.557993 efootprint-2.0.3/LICENSE
--rw-r--r--   0        0        0     3456 2024-04-06 12:40:51.663763 efootprint-2.0.3/README.md
--rw-r--r--   0        0        0        0 2024-04-06 12:40:52.150404 efootprint-2.0.3/efootprint/__init__.py
--rw-r--r--   0        0        0        0 2023-10-26 17:58:06.648138 efootprint-2.0.3/efootprint/abstract_modeling_classes/__init__.py
--rw-r--r--   0        0        0    11880 2024-04-06 12:40:52.160479 efootprint-2.0.3/efootprint/abstract_modeling_classes/explainable_object_base_class.py
--rw-r--r--   0        0        0     2240 2024-04-06 12:40:52.168353 efootprint-2.0.3/efootprint/abstract_modeling_classes/explainable_object_dict.py
--rw-r--r--   0        0        0    12607 2024-04-06 12:40:52.173001 efootprint-2.0.3/efootprint/abstract_modeling_classes/explainable_objects.py
--rw-r--r--   0        0        0    17481 2024-04-12 11:51:41.746811 efootprint-2.0.3/efootprint/abstract_modeling_classes/modeling_object.py
--rw-r--r--   0        0        0      754 2024-03-04 16:54:55.210288 efootprint-2.0.3/efootprint/abstract_modeling_classes/source_objects.py
--rw-r--r--   0        0        0        0 2024-03-04 16:55:00.126280 efootprint-2.0.3/efootprint/api_utils/__init__.py
--rw-r--r--   0        0        0     6206 2024-04-15 15:44:04.537262 efootprint-2.0.3/efootprint/api_utils/json_to_system.py
--rw-r--r--   0        0        0     1306 2024-04-06 17:14:03.492802 efootprint-2.0.3/efootprint/api_utils/system_to_json.py
--rw-r--r--   0        0        0        0 2024-03-04 16:54:53.623840 efootprint-2.0.3/efootprint/builders/__init__.py
--rw-r--r--   0        0        0        0 2024-03-04 16:54:54.164118 efootprint-2.0.3/efootprint/builders/hardware/__init__.py
--rw-r--r--   0        0        0     2076 2024-03-04 16:54:55.218246 efootprint-2.0.3/efootprint/builders/hardware/devices_defaults.py
--rw-r--r--   0        0        0      743 2024-03-04 16:54:55.222924 efootprint-2.0.3/efootprint/builders/hardware/network_defaults.py
--rw-r--r--   0        0        0     8980 2024-04-06 12:40:52.200652 efootprint-2.0.3/efootprint/builders/hardware/servers_boaviztapi.py
--rw-r--r--   0        0        0     2898 2024-03-04 16:54:57.077899 efootprint-2.0.3/efootprint/builders/hardware/servers_defaults.py
--rw-r--r--   0        0        0     1876 2024-03-04 16:54:55.236944 efootprint-2.0.3/efootprint/builders/hardware/storage_defaults.py
--rw-r--r--   0        0        0        0 2024-04-06 17:14:03.495913 efootprint-2.0.3/efootprint/builders/usage/__init__.py
--rw-r--r--   0        0        0       39 2024-04-06 17:14:03.499539 efootprint-2.0.3/efootprint/builders/usage/job_ecobenchmark/.gitignore
--rw-r--r--   0        0        0        0 2024-04-06 17:14:03.500532 efootprint-2.0.3/efootprint/builders/usage/job_ecobenchmark/__init__.py
--rw-r--r--   0        0        0     2556 2024-04-06 17:14:03.502889 efootprint-2.0.3/efootprint/builders/usage/job_ecobenchmark/ecobenchmark_data_analysis.py
--rw-r--r--   0        0        0     3888 2024-04-15 15:53:51.780232 efootprint-2.0.3/efootprint/builders/usage/job_ecobenchmark/ecobenchmark_data_for_job_defaults.csv
--rw-r--r--   0        0        0     1827 2024-04-06 17:14:03.506424 efootprint-2.0.3/efootprint/builders/usage/job_ecobenchmark/ecobenchmark_job_builder.py
--rw-r--r--   0        0        0    67861 2024-04-06 17:14:03.511270 efootprint-2.0.3/efootprint/builders/usage/job_ecobenchmark/ecobenchmark_results__raw.csv
--rw-r--r--   0        0        0        0 2023-10-26 17:58:06.656189 efootprint-2.0.3/efootprint/constants/__init__.py
--rw-r--r--   0        0        0     4182 2024-04-06 12:40:52.207602 efootprint-2.0.3/efootprint/constants/countries.py
--rw-r--r--   0        0        0      100 2023-10-26 17:58:06.658280 efootprint-2.0.3/efootprint/constants/custom_units.txt
--rw-r--r--   0        0        0      284 2023-11-13 13:05:11.080734 efootprint-2.0.3/efootprint/constants/files.py
--rw-r--r--   0        0        0     1660 2024-03-04 16:54:55.243478 efootprint-2.0.3/efootprint/constants/sources.py
--rw-r--r--   0        0        0      173 2023-10-26 17:58:06.666143 efootprint-2.0.3/efootprint/constants/units.py
--rw-r--r--   0        0        0        0 2023-10-26 17:58:06.666706 efootprint-2.0.3/efootprint/core/__init__.py
--rw-r--r--   0        0        0        0 2023-10-26 17:58:06.667254 efootprint-2.0.3/efootprint/core/hardware/__init__.py
--rw-r--r--   0        0        0     6034 2024-04-06 12:40:52.212747 efootprint-2.0.3/efootprint/core/hardware/device_population.py
--rw-r--r--   0        0        0     5707 2024-04-06 12:40:52.215226 efootprint-2.0.3/efootprint/core/hardware/hardware_base_classes.py
--rw-r--r--   0        0        0     3367 2024-04-06 12:40:52.219470 efootprint-2.0.3/efootprint/core/hardware/network.py
--rw-r--r--   0        0        0        0 2023-10-26 17:58:06.671292 efootprint-2.0.3/efootprint/core/hardware/servers/__init__.py
--rw-r--r--   0        0        0     3135 2024-03-04 16:54:57.120650 efootprint-2.0.3/efootprint/core/hardware/servers/autoscaling.py
--rw-r--r--   0        0        0     3766 2024-04-06 12:40:52.222595 efootprint-2.0.3/efootprint/core/hardware/servers/on_premise.py
--rw-r--r--   0        0        0     3464 2024-03-04 16:54:59.121266 efootprint-2.0.3/efootprint/core/hardware/servers/server_base_class.py
--rw-r--r--   0        0        0     1972 2024-03-04 16:54:57.211287 efootprint-2.0.3/efootprint/core/hardware/servers/serverless.py
--rw-r--r--   0        0        0     5491 2024-03-04 16:54:59.146307 efootprint-2.0.3/efootprint/core/hardware/storage.py
--rw-r--r--   0        0        0     5312 2024-04-06 17:14:03.514666 efootprint-2.0.3/efootprint/core/service.py
--rw-r--r--   0        0        0    10359 2024-04-06 17:14:03.517635 efootprint-2.0.3/efootprint/core/system.py
--rw-r--r--   0        0        0        0 2023-10-26 17:58:06.688562 efootprint-2.0.3/efootprint/core/usage/__init__.py
--rw-r--r--   0        0        0     3995 2024-04-06 17:14:03.519960 efootprint-2.0.3/efootprint/core/usage/job.py
--rw-r--r--   0        0        0     3890 2024-04-06 12:40:52.233601 efootprint-2.0.3/efootprint/core/usage/usage_pattern.py
--rw-r--r--   0        0        0     2723 2024-04-06 17:14:03.529290 efootprint-2.0.3/efootprint/core/usage/user_journey.py
--rw-r--r--   0        0        0     1510 2024-04-06 17:14:03.531224 efootprint-2.0.3/efootprint/core/usage/user_journey_step.py
--rw-r--r--   0        0        0      805 2023-11-13 13:05:11.082835 efootprint-2.0.3/efootprint/logger.py
--rw-r--r--   0        0        0        0 2023-10-26 17:58:06.698150 efootprint-2.0.3/efootprint/utils/__init__.py
--rw-r--r--   0        0        0     3055 2024-04-06 12:40:52.240288 efootprint-2.0.3/efootprint/utils/calculus_graph.py
--rw-r--r--   0        0        0      146 2023-11-03 15:44:18.031433 efootprint-2.0.3/efootprint/utils/dev_utils/README.md
--rw-r--r--   0        0        0        0 2023-11-03 15:44:18.033655 efootprint-2.0.3/efootprint/utils/dev_utils/__init__.py
--rw-r--r--   0        0        0        0 2023-11-03 15:44:18.035244 efootprint-2.0.3/efootprint/utils/dev_utils/page_weights.py
--rw-r--r--   0        0        0      830 2023-11-03 15:44:18.039040 efootprint-2.0.3/efootprint/utils/dev_utils/selenium_screenshot.py
--rw-r--r--   0        0        0     1407 2024-04-06 12:40:52.242646 efootprint-2.0.3/efootprint/utils/graph_tools.py
--rw-r--r--   0        0        0     2390 2024-04-06 17:14:03.536199 efootprint-2.0.3/efootprint/utils/object_relationships_graphs.py
--rw-r--r--   0        0        0     7612 2024-04-06 17:14:03.543621 efootprint-2.0.3/efootprint/utils/plot_emission_diffs.py
--rw-r--r--   0        0        0     1702 2024-03-04 16:54:53.701197 efootprint-2.0.3/efootprint/utils/tools.py
--rw-r--r--   0        0        0     1258 2024-04-15 15:51:52.143807 efootprint-2.0.3/pyproject.toml
--rw-r--r--   0        0        0     4149 1970-01-01 00:00:00.000000 efootprint-2.0.3/PKG-INFO
+-rw-r--r--   0        0        0    34522 2023-10-17 09:49:47.557993 efootprint-2.0.4/LICENSE
+-rw-r--r--   0        0        0     3456 2024-04-06 12:40:51.663763 efootprint-2.0.4/README.md
+-rw-r--r--   0        0        0        0 2024-04-06 12:40:52.150404 efootprint-2.0.4/efootprint/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-26 17:58:06.648138 efootprint-2.0.4/efootprint/abstract_modeling_classes/__init__.py
+-rw-r--r--   0        0        0    11880 2024-04-06 12:40:52.160479 efootprint-2.0.4/efootprint/abstract_modeling_classes/explainable_object_base_class.py
+-rw-r--r--   0        0        0     2240 2024-04-06 12:40:52.168353 efootprint-2.0.4/efootprint/abstract_modeling_classes/explainable_object_dict.py
+-rw-r--r--   0        0        0    12607 2024-04-06 12:40:52.173001 efootprint-2.0.4/efootprint/abstract_modeling_classes/explainable_objects.py
+-rw-r--r--   0        0        0    17481 2024-04-12 11:51:41.746811 efootprint-2.0.4/efootprint/abstract_modeling_classes/modeling_object.py
+-rw-r--r--   0        0        0      754 2024-03-04 16:54:55.210288 efootprint-2.0.4/efootprint/abstract_modeling_classes/source_objects.py
+-rw-r--r--   0        0        0        0 2024-03-04 16:55:00.126280 efootprint-2.0.4/efootprint/api_utils/__init__.py
+-rw-r--r--   0        0        0     6256 2024-04-16 12:25:06.576552 efootprint-2.0.4/efootprint/api_utils/json_to_system.py
+-rw-r--r--   0        0        0     1306 2024-04-06 17:14:03.492802 efootprint-2.0.4/efootprint/api_utils/system_to_json.py
+-rw-r--r--   0        0        0        0 2024-03-04 16:54:53.623840 efootprint-2.0.4/efootprint/builders/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-04 16:54:54.164118 efootprint-2.0.4/efootprint/builders/hardware/__init__.py
+-rw-r--r--   0        0        0     2076 2024-03-04 16:54:55.218246 efootprint-2.0.4/efootprint/builders/hardware/devices_defaults.py
+-rw-r--r--   0        0        0      743 2024-03-04 16:54:55.222924 efootprint-2.0.4/efootprint/builders/hardware/network_defaults.py
+-rw-r--r--   0        0        0     8980 2024-04-06 12:40:52.200652 efootprint-2.0.4/efootprint/builders/hardware/servers_boaviztapi.py
+-rw-r--r--   0        0        0     2898 2024-03-04 16:54:57.077899 efootprint-2.0.4/efootprint/builders/hardware/servers_defaults.py
+-rw-r--r--   0        0        0     1876 2024-03-04 16:54:55.236944 efootprint-2.0.4/efootprint/builders/hardware/storage_defaults.py
+-rw-r--r--   0        0        0        0 2024-04-06 17:14:03.495913 efootprint-2.0.4/efootprint/builders/usage/__init__.py
+-rw-r--r--   0        0        0       39 2024-04-06 17:14:03.499539 efootprint-2.0.4/efootprint/builders/usage/job_ecobenchmark/.gitignore
+-rw-r--r--   0        0        0        0 2024-04-06 17:14:03.500532 efootprint-2.0.4/efootprint/builders/usage/job_ecobenchmark/__init__.py
+-rw-r--r--   0        0        0     2556 2024-04-06 17:14:03.502889 efootprint-2.0.4/efootprint/builders/usage/job_ecobenchmark/ecobenchmark_data_analysis.py
+-rw-r--r--   0        0        0     3888 2024-04-16 12:26:23.586197 efootprint-2.0.4/efootprint/builders/usage/job_ecobenchmark/ecobenchmark_data_for_job_defaults.csv
+-rw-r--r--   0        0        0     1827 2024-04-06 17:14:03.506424 efootprint-2.0.4/efootprint/builders/usage/job_ecobenchmark/ecobenchmark_job_builder.py
+-rw-r--r--   0        0        0    67861 2024-04-06 17:14:03.511270 efootprint-2.0.4/efootprint/builders/usage/job_ecobenchmark/ecobenchmark_results__raw.csv
+-rw-r--r--   0        0        0        0 2023-10-26 17:58:06.656189 efootprint-2.0.4/efootprint/constants/__init__.py
+-rw-r--r--   0        0        0     4182 2024-04-06 12:40:52.207602 efootprint-2.0.4/efootprint/constants/countries.py
+-rw-r--r--   0        0        0      100 2023-10-26 17:58:06.658280 efootprint-2.0.4/efootprint/constants/custom_units.txt
+-rw-r--r--   0        0        0      284 2023-11-13 13:05:11.080734 efootprint-2.0.4/efootprint/constants/files.py
+-rw-r--r--   0        0        0     1660 2024-03-04 16:54:55.243478 efootprint-2.0.4/efootprint/constants/sources.py
+-rw-r--r--   0        0        0      173 2023-10-26 17:58:06.666143 efootprint-2.0.4/efootprint/constants/units.py
+-rw-r--r--   0        0        0        0 2023-10-26 17:58:06.666706 efootprint-2.0.4/efootprint/core/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-26 17:58:06.667254 efootprint-2.0.4/efootprint/core/hardware/__init__.py
+-rw-r--r--   0        0        0     6034 2024-04-06 12:40:52.212747 efootprint-2.0.4/efootprint/core/hardware/device_population.py
+-rw-r--r--   0        0        0     5707 2024-04-06 12:40:52.215226 efootprint-2.0.4/efootprint/core/hardware/hardware_base_classes.py
+-rw-r--r--   0        0        0     3367 2024-04-06 12:40:52.219470 efootprint-2.0.4/efootprint/core/hardware/network.py
+-rw-r--r--   0        0        0        0 2023-10-26 17:58:06.671292 efootprint-2.0.4/efootprint/core/hardware/servers/__init__.py
+-rw-r--r--   0        0        0     3135 2024-03-04 16:54:57.120650 efootprint-2.0.4/efootprint/core/hardware/servers/autoscaling.py
+-rw-r--r--   0        0        0     3766 2024-04-06 12:40:52.222595 efootprint-2.0.4/efootprint/core/hardware/servers/on_premise.py
+-rw-r--r--   0        0        0     3464 2024-03-04 16:54:59.121266 efootprint-2.0.4/efootprint/core/hardware/servers/server_base_class.py
+-rw-r--r--   0        0        0     1972 2024-03-04 16:54:57.211287 efootprint-2.0.4/efootprint/core/hardware/servers/serverless.py
+-rw-r--r--   0        0        0     5491 2024-03-04 16:54:59.146307 efootprint-2.0.4/efootprint/core/hardware/storage.py
+-rw-r--r--   0        0        0     5312 2024-04-06 17:14:03.514666 efootprint-2.0.4/efootprint/core/service.py
+-rw-r--r--   0        0        0    10359 2024-04-06 17:14:03.517635 efootprint-2.0.4/efootprint/core/system.py
+-rw-r--r--   0        0        0        0 2023-10-26 17:58:06.688562 efootprint-2.0.4/efootprint/core/usage/__init__.py
+-rw-r--r--   0        0        0     3995 2024-04-06 17:14:03.519960 efootprint-2.0.4/efootprint/core/usage/job.py
+-rw-r--r--   0        0        0     3890 2024-04-06 12:40:52.233601 efootprint-2.0.4/efootprint/core/usage/usage_pattern.py
+-rw-r--r--   0        0        0     2723 2024-04-06 17:14:03.529290 efootprint-2.0.4/efootprint/core/usage/user_journey.py
+-rw-r--r--   0        0        0     1510 2024-04-06 17:14:03.531224 efootprint-2.0.4/efootprint/core/usage/user_journey_step.py
+-rw-r--r--   0        0        0      805 2023-11-13 13:05:11.082835 efootprint-2.0.4/efootprint/logger.py
+-rw-r--r--   0        0        0        0 2023-10-26 17:58:06.698150 efootprint-2.0.4/efootprint/utils/__init__.py
+-rw-r--r--   0        0        0     3055 2024-04-06 12:40:52.240288 efootprint-2.0.4/efootprint/utils/calculus_graph.py
+-rw-r--r--   0        0        0      146 2023-11-03 15:44:18.031433 efootprint-2.0.4/efootprint/utils/dev_utils/README.md
+-rw-r--r--   0        0        0        0 2023-11-03 15:44:18.033655 efootprint-2.0.4/efootprint/utils/dev_utils/__init__.py
+-rw-r--r--   0        0        0        0 2023-11-03 15:44:18.035244 efootprint-2.0.4/efootprint/utils/dev_utils/page_weights.py
+-rw-r--r--   0        0        0      830 2023-11-03 15:44:18.039040 efootprint-2.0.4/efootprint/utils/dev_utils/selenium_screenshot.py
+-rw-r--r--   0        0        0     1407 2024-04-06 12:40:52.242646 efootprint-2.0.4/efootprint/utils/graph_tools.py
+-rw-r--r--   0        0        0     2390 2024-04-06 17:14:03.536199 efootprint-2.0.4/efootprint/utils/object_relationships_graphs.py
+-rw-r--r--   0        0        0     7612 2024-04-06 17:14:03.543621 efootprint-2.0.4/efootprint/utils/plot_emission_diffs.py
+-rw-r--r--   0        0        0     1702 2024-03-04 16:54:53.701197 efootprint-2.0.4/efootprint/utils/tools.py
+-rw-r--r--   0        0        0     1258 2024-04-16 12:27:43.249720 efootprint-2.0.4/pyproject.toml
+-rw-r--r--   0        0        0     4149 1970-01-01 00:00:00.000000 efootprint-2.0.4/PKG-INFO
```

### Comparing `efootprint-2.0.3/LICENSE` & `efootprint-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.3/README.md` & `efootprint-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.3/efootprint/abstract_modeling_classes/explainable_object_base_class.py` & `efootprint-2.0.4/efootprint/abstract_modeling_classes/explainable_object_base_class.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.3/efootprint/abstract_modeling_classes/explainable_object_dict.py` & `efootprint-2.0.4/efootprint/abstract_modeling_classes/explainable_object_dict.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.3/efootprint/abstract_modeling_classes/explainable_objects.py` & `efootprint-2.0.4/efootprint/abstract_modeling_classes/explainable_objects.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.3/efootprint/abstract_modeling_classes/modeling_object.py` & `efootprint-2.0.4/efootprint/abstract_modeling_classes/modeling_object.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.3/efootprint/abstract_modeling_classes/source_objects.py` & `efootprint-2.0.4/efootprint/abstract_modeling_classes/source_objects.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.3/efootprint/api_utils/json_to_system.py` & `efootprint-2.0.4/efootprint/api_utils/json_to_system.py`

 * *Files 6% similar despite different names*

```diff
@@ -101,15 +101,16 @@
                 if len(mod_obj.systems) == 0:
                     logger.warning(
                         f"{mod_obj.class_as_simple_str} {mod_obj.name} is not linked to any existing system so needs "
                         f"to compute its own calculated attributes")
                     mod_obj.compute_calculated_attributes()
 
     for system in class_obj_dict["System"].values():
-        system.launch_attributes_computation_chain()
+        system.__init__(system.name, usage_patterns=system.usage_patterns)
+        system.after_init()
 
     return class_obj_dict, flat_obj_dict
 
 
 def get_obj_by_key_similarity(obj_container_dict, input_key):
     for key in obj_container_dict.keys():
         if input_key in key:
```

### Comparing `efootprint-2.0.3/efootprint/api_utils/system_to_json.py` & `efootprint-2.0.4/efootprint/api_utils/system_to_json.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.3/efootprint/builders/hardware/devices_defaults.py` & `efootprint-2.0.4/efootprint/builders/hardware/devices_defaults.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.3/efootprint/builders/hardware/network_defaults.py` & `efootprint-2.0.4/efootprint/builders/hardware/network_defaults.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.3/efootprint/builders/hardware/servers_boaviztapi.py` & `efootprint-2.0.4/efootprint/builders/hardware/servers_boaviztapi.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.3/efootprint/builders/hardware/servers_defaults.py` & `efootprint-2.0.4/efootprint/builders/hardware/servers_defaults.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.3/efootprint/builders/hardware/storage_defaults.py` & `efootprint-2.0.4/efootprint/builders/hardware/storage_defaults.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.3/efootprint/builders/usage/job_ecobenchmark/ecobenchmark_data_analysis.py` & `efootprint-2.0.4/efootprint/builders/usage/job_ecobenchmark/ecobenchmark_data_analysis.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.3/efootprint/builders/usage/job_ecobenchmark/ecobenchmark_data_for_job_defaults.csv` & `efootprint-2.0.4/efootprint/builders/usage/job_ecobenchmark/ecobenchmark_data_for_job_defaults.csv`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.3/efootprint/builders/usage/job_ecobenchmark/ecobenchmark_job_builder.py` & `efootprint-2.0.4/efootprint/builders/usage/job_ecobenchmark/ecobenchmark_job_builder.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.3/efootprint/builders/usage/job_ecobenchmark/ecobenchmark_results__raw.csv` & `efootprint-2.0.4/efootprint/builders/usage/job_ecobenchmark/ecobenchmark_results__raw.csv`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.3/efootprint/constants/countries.py` & `efootprint-2.0.4/efootprint/constants/countries.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.3/efootprint/constants/sources.py` & `efootprint-2.0.4/efootprint/constants/sources.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.3/efootprint/core/hardware/device_population.py` & `efootprint-2.0.4/efootprint/core/hardware/device_population.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.3/efootprint/core/hardware/hardware_base_classes.py` & `efootprint-2.0.4/efootprint/core/hardware/hardware_base_classes.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.3/efootprint/core/hardware/network.py` & `efootprint-2.0.4/efootprint/core/hardware/network.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.3/efootprint/core/hardware/servers/autoscaling.py` & `efootprint-2.0.4/efootprint/core/hardware/servers/autoscaling.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.3/efootprint/core/hardware/servers/on_premise.py` & `efootprint-2.0.4/efootprint/core/hardware/servers/on_premise.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.3/efootprint/core/hardware/servers/server_base_class.py` & `efootprint-2.0.4/efootprint/core/hardware/servers/server_base_class.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.3/efootprint/core/hardware/servers/serverless.py` & `efootprint-2.0.4/efootprint/core/hardware/servers/serverless.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.3/efootprint/core/hardware/storage.py` & `efootprint-2.0.4/efootprint/core/hardware/storage.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.3/efootprint/core/service.py` & `efootprint-2.0.4/efootprint/core/service.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.3/efootprint/core/system.py` & `efootprint-2.0.4/efootprint/core/system.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.3/efootprint/core/usage/job.py` & `efootprint-2.0.4/efootprint/core/usage/job.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.3/efootprint/core/usage/usage_pattern.py` & `efootprint-2.0.4/efootprint/core/usage/usage_pattern.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.3/efootprint/core/usage/user_journey.py` & `efootprint-2.0.4/efootprint/core/usage/user_journey.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.3/efootprint/core/usage/user_journey_step.py` & `efootprint-2.0.4/efootprint/core/usage/user_journey_step.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.3/efootprint/logger.py` & `efootprint-2.0.4/efootprint/logger.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.3/efootprint/utils/calculus_graph.py` & `efootprint-2.0.4/efootprint/utils/calculus_graph.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.3/efootprint/utils/dev_utils/selenium_screenshot.py` & `efootprint-2.0.4/efootprint/utils/dev_utils/selenium_screenshot.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.3/efootprint/utils/graph_tools.py` & `efootprint-2.0.4/efootprint/utils/graph_tools.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.3/efootprint/utils/object_relationships_graphs.py` & `efootprint-2.0.4/efootprint/utils/object_relationships_graphs.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.3/efootprint/utils/plot_emission_diffs.py` & `efootprint-2.0.4/efootprint/utils/plot_emission_diffs.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.3/efootprint/utils/tools.py` & `efootprint-2.0.4/efootprint/utils/tools.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.3/pyproject.toml` & `efootprint-2.0.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # NOTE: you have to use single-quoted strings in TOML for regular expressions.
 # It's the equivalent of r-strings in Python.  Multiline strings are treated as
 # verbose regular expressions by Black.  Use [ ] to denote a significant space
 # character.
 
 [tool.poetry]
 name = "efootprint"
-version = "2.0.3"
+version = "2.0.4"
 description = "Digital service environmental footprint model"
 authors = ["Vincent Villet for Publicis Sapient"]
 readme = "README.md"
 include = ["efootprint/constants/custom_units.txt"]
 
 [tool.black]
 line-length = 120
```

### Comparing `efootprint-2.0.3/PKG-INFO` & `efootprint-2.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: efootprint
-Version: 2.0.3
+Version: 2.0.4
 Summary: Digital service environmental footprint model
 Author: Vincent Villet for Publicis Sapient
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

