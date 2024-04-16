# Comparing `tmp/linktest-2.4.7.tar.gz` & `tmp/linktest-2.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linktest-2.4.7.tar", last modified: Tue Apr 16 05:22:50 2024, max compression
+gzip compressed data, was "linktest-2.4.8.tar", last modified: Tue Apr 16 05:50:19 2024, max compression
```

## Comparing `linktest-2.4.7.tar` & `linktest-2.4.8.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-16 05:22:50.810490 linktest-2.4.7/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-04-16 05:22:50.810024 linktest-2.4.7/PKG-INFO
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-16 05:22:50.806121 linktest-2.4.7/linktest/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       22 2024-04-15 15:31:29.000000 linktest-2.4.7/linktest/__init__.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      487 2024-04-15 15:08:03.000000 linktest-2.4.7/linktest/android_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      187 2024-04-15 15:08:03.000000 linktest-2.4.7/linktest/api_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10759 2024-04-15 15:08:03.000000 linktest-2.4.7/linktest/appium_utils.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    29054 2024-04-15 15:08:03.000000 linktest-2.4.7/linktest/auto_generate_testcase_list.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10302 2024-04-15 15:08:03.000000 linktest-2.4.7/linktest/auto_generate_testcase_list_from_csv.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9940 2024-04-16 02:13:14.000000 linktest-2.4.7/linktest/base_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1792 2024-04-15 15:08:03.000000 linktest-2.4.7/linktest/clean_data.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1403 2024-04-15 15:08:03.000000 linktest-2.4.7/linktest/conver_xml_into_db.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7260 2024-04-15 15:08:03.000000 linktest-2.4.7/linktest/database_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2471 2024-04-15 15:08:03.000000 linktest-2.4.7/linktest/date_utilities.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      232 2024-04-15 15:08:03.000000 linktest-2.4.7/linktest/detect_delimiter.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16523 2024-04-15 15:08:03.000000 linktest-2.4.7/linktest/doctor.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      959 2024-04-15 15:08:03.000000 linktest-2.4.7/linktest/framework_log.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     6539 2024-04-15 15:30:06.000000 linktest-2.4.7/linktest/generate_html_log.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      987 2024-04-15 15:08:03.000000 linktest-2.4.7/linktest/get_adb_devices.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      924 2024-04-15 15:08:03.000000 linktest-2.4.7/linktest/get_ios_devices_list.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1775 2024-04-15 15:08:03.000000 linktest-2.4.7/linktest/get_platform_info.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3137 2024-04-15 15:08:03.000000 linktest-2.4.7/linktest/get_project_info.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    34730 2024-04-15 15:08:03.000000 linktest-2.4.7/linktest/html_report.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      280 2024-04-15 15:08:03.000000 linktest-2.4.7/linktest/ios_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      195 2024-04-15 15:08:03.000000 linktest-2.4.7/linktest/linktest_setup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8745 2024-04-15 15:08:03.000000 linktest-2.4.7/linktest/logged_requests.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)   105356 2024-04-15 15:08:03.000000 linktest-2.4.7/linktest/main.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      982 2024-04-15 15:08:03.000000 linktest-2.4.7/linktest/memory_usage.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     4526 2024-04-15 15:08:03.000000 linktest-2.4.7/linktest/re_func.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1077 2024-04-15 15:08:03.000000 linktest-2.4.7/linktest/run.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1926 2024-04-15 15:08:03.000000 linktest-2.4.7/linktest/run_testcase_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1048 2024-04-15 15:08:03.000000 linktest-2.4.7/linktest/scp_report_to_specified_path.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8022 2024-04-15 15:08:03.000000 linktest-2.4.7/linktest/selenium_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      396 2024-04-15 15:08:03.000000 linktest-2.4.7/linktest/set_run_flag_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-04-15 15:31:37.000000 linktest-2.4.7/linktest/setup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      173 2024-04-15 15:08:03.000000 linktest-2.4.7/linktest/testcase_order.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      140 2024-04-15 15:08:03.000000 linktest-2.4.7/linktest/testcase_timeout_exception.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      801 2024-04-15 15:08:03.000000 linktest-2.4.7/linktest/timeout_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      931 2024-04-15 15:08:03.000000 linktest-2.4.7/linktest/ui_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3055 2024-04-15 15:08:03.000000 linktest-2.4.7/linktest/update_config.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    11186 2024-04-15 15:08:03.000000 linktest-2.4.7/linktest/webdriver_wrapper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      406 2024-04-15 15:08:03.000000 linktest-2.4.7/linktest/windows_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3544 2024-04-15 15:08:03.000000 linktest-2.4.7/linktest/xml_report.py
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-16 05:22:50.809398 linktest-2.4.7/linktest.egg-info/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-04-16 05:22:50.000000 linktest-2.4.7/linktest.egg-info/PKG-INFO
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1271 2024-04-16 05:22:50.000000 linktest-2.4.7/linktest.egg-info/SOURCES.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        1 2024-04-16 05:22:50.000000 linktest-2.4.7/linktest.egg-info/dependency_links.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      123 2024-04-16 05:22:50.000000 linktest-2.4.7/linktest.egg-info/requires.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        9 2024-04-16 05:22:50.000000 linktest-2.4.7/linktest.egg-info/top_level.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       38 2024-04-16 05:22:50.810602 linktest-2.4.7/setup.cfg
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-04-16 05:22:44.000000 linktest-2.4.7/setup.py
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-16 05:50:19.135415 linktest-2.4.8/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-04-16 05:50:19.134847 linktest-2.4.8/PKG-INFO
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-16 05:50:19.130441 linktest-2.4.8/linktest/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       22 2024-04-16 05:46:37.000000 linktest-2.4.8/linktest/__init__.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      487 2024-04-16 05:24:13.000000 linktest-2.4.8/linktest/android_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      187 2024-04-16 05:24:13.000000 linktest-2.4.8/linktest/api_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10759 2024-04-16 05:24:13.000000 linktest-2.4.8/linktest/appium_utils.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    29054 2024-04-16 05:24:13.000000 linktest-2.4.8/linktest/auto_generate_testcase_list.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10302 2024-04-16 05:24:13.000000 linktest-2.4.8/linktest/auto_generate_testcase_list_from_csv.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9940 2024-04-16 05:24:13.000000 linktest-2.4.8/linktest/base_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1792 2024-04-16 05:24:13.000000 linktest-2.4.8/linktest/clean_data.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1403 2024-04-16 05:24:13.000000 linktest-2.4.8/linktest/conver_xml_into_db.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7260 2024-04-16 05:24:13.000000 linktest-2.4.8/linktest/database_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2471 2024-04-16 05:24:13.000000 linktest-2.4.8/linktest/date_utilities.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      232 2024-04-16 05:24:13.000000 linktest-2.4.8/linktest/detect_delimiter.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16523 2024-04-16 05:24:13.000000 linktest-2.4.8/linktest/doctor.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      959 2024-04-16 05:24:13.000000 linktest-2.4.8/linktest/framework_log.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     6849 2024-04-16 05:47:46.000000 linktest-2.4.8/linktest/generate_html_log.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      987 2024-04-16 05:24:13.000000 linktest-2.4.8/linktest/get_adb_devices.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      924 2024-04-16 05:24:13.000000 linktest-2.4.8/linktest/get_ios_devices_list.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1775 2024-04-16 05:24:13.000000 linktest-2.4.8/linktest/get_platform_info.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3137 2024-04-16 05:24:13.000000 linktest-2.4.8/linktest/get_project_info.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    34730 2024-04-16 05:24:13.000000 linktest-2.4.8/linktest/html_report.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      280 2024-04-16 05:24:13.000000 linktest-2.4.8/linktest/ios_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      195 2024-04-16 05:24:13.000000 linktest-2.4.8/linktest/linktest_setup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8745 2024-04-16 05:24:13.000000 linktest-2.4.8/linktest/logged_requests.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)   105356 2024-04-16 05:24:13.000000 linktest-2.4.8/linktest/main.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      982 2024-04-16 05:24:13.000000 linktest-2.4.8/linktest/memory_usage.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     4526 2024-04-16 05:24:13.000000 linktest-2.4.8/linktest/re_func.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1077 2024-04-16 05:24:13.000000 linktest-2.4.8/linktest/run.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1926 2024-04-16 05:24:13.000000 linktest-2.4.8/linktest/run_testcase_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1048 2024-04-16 05:24:13.000000 linktest-2.4.8/linktest/scp_report_to_specified_path.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8022 2024-04-16 05:24:13.000000 linktest-2.4.8/linktest/selenium_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      396 2024-04-16 05:24:13.000000 linktest-2.4.8/linktest/set_run_flag_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-04-16 05:46:46.000000 linktest-2.4.8/linktest/setup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      173 2024-04-16 05:24:13.000000 linktest-2.4.8/linktest/testcase_order.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      140 2024-04-16 05:24:13.000000 linktest-2.4.8/linktest/testcase_timeout_exception.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      801 2024-04-16 05:24:13.000000 linktest-2.4.8/linktest/timeout_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      931 2024-04-16 05:24:13.000000 linktest-2.4.8/linktest/ui_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3055 2024-04-16 05:24:13.000000 linktest-2.4.8/linktest/update_config.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    11186 2024-04-16 05:24:13.000000 linktest-2.4.8/linktest/webdriver_wrapper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      406 2024-04-16 05:24:13.000000 linktest-2.4.8/linktest/windows_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3544 2024-04-16 05:24:13.000000 linktest-2.4.8/linktest/xml_report.py
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-16 05:50:19.134238 linktest-2.4.8/linktest.egg-info/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-04-16 05:50:18.000000 linktest-2.4.8/linktest.egg-info/PKG-INFO
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1271 2024-04-16 05:50:18.000000 linktest-2.4.8/linktest.egg-info/SOURCES.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        1 2024-04-16 05:50:18.000000 linktest-2.4.8/linktest.egg-info/dependency_links.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      123 2024-04-16 05:50:18.000000 linktest-2.4.8/linktest.egg-info/requires.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        9 2024-04-16 05:50:18.000000 linktest-2.4.8/linktest.egg-info/top_level.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       38 2024-04-16 05:50:19.135551 linktest-2.4.8/setup.cfg
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-04-16 05:50:13.000000 linktest-2.4.8/setup.py
```

### Comparing `linktest-2.4.7/linktest/appium_utils.py` & `linktest-2.4.8/linktest/appium_utils.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.7/linktest/auto_generate_testcase_list.py` & `linktest-2.4.8/linktest/auto_generate_testcase_list.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.7/linktest/auto_generate_testcase_list_from_csv.py` & `linktest-2.4.8/linktest/auto_generate_testcase_list_from_csv.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.7/linktest/base_testcase.py` & `linktest-2.4.8/linktest/base_testcase.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.7/linktest/clean_data.py` & `linktest-2.4.8/linktest/clean_data.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.7/linktest/conver_xml_into_db.py` & `linktest-2.4.8/linktest/conver_xml_into_db.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.7/linktest/database_helper.py` & `linktest-2.4.8/linktest/database_helper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.7/linktest/date_utilities.py` & `linktest-2.4.8/linktest/date_utilities.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.7/linktest/doctor.py` & `linktest-2.4.8/linktest/doctor.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.7/linktest/framework_log.py` & `linktest-2.4.8/linktest/framework_log.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.7/linktest/generate_html_log.py` & `linktest-2.4.8/linktest/generate_html_log.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,24 @@
     # 使用 re.match 检查字符串开头是否匹配该模式
     if re.match(pattern, input_string):
         return True
     else:
         return False
 
 
+import json
+
+def format_json(json_string):
+    try:
+        parsed_json = json.loads(json_string)
+        formatted_json = json.dumps(parsed_json, indent=2)
+        return formatted_json.replace(" ", "&nbsp;").replace("\n", "<br>")
+    except json.JSONDecodeError:
+        return json_string
+
 def generate_html_log(executing_testcase):
     # executing_testcase.logfile_full_name 是日志文件的完整路径
     # executing_testcase.full_tc_folder 是存放生成的HTML文件的目录
 
     # 读取日志文件内容
     with open(executing_testcase.logfile_full_name, "r") as logfile:
         execution_log = logfile.readlines()
@@ -142,15 +152,15 @@
 
 
         if line == "\n":
             continue
 
         if starts_with_date(line):
             if single_line_flag:
-                html_content += f'<div class="{class_name}"><p>{lines}</p></div>'
+                html_content += f'<div class="{class_name}"><pre>{format_json(lines)}</pre></div>'
                 lines = ""
                 single_line_flag = False
 
             timestamp = line.split(" ")[0] + " " + line.split(" ")[1]
             html_content += f'<div class="{class_name}"><span class="timestamp">{timestamp}</span><p>{line[len(timestamp):].strip()}</p></div>'
         else:
             lines += line.replace("\n", "<br>")
```

### Comparing `linktest-2.4.7/linktest/get_adb_devices.py` & `linktest-2.4.8/linktest/get_adb_devices.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.7/linktest/get_ios_devices_list.py` & `linktest-2.4.8/linktest/get_ios_devices_list.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.7/linktest/get_platform_info.py` & `linktest-2.4.8/linktest/get_platform_info.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.7/linktest/get_project_info.py` & `linktest-2.4.8/linktest/get_project_info.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.7/linktest/html_report.py` & `linktest-2.4.8/linktest/html_report.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.7/linktest/logged_requests.py` & `linktest-2.4.8/linktest/logged_requests.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.7/linktest/main.py` & `linktest-2.4.8/linktest/main.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.7/linktest/memory_usage.py` & `linktest-2.4.8/linktest/memory_usage.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.7/linktest/re_func.py` & `linktest-2.4.8/linktest/re_func.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.7/linktest/run.py` & `linktest-2.4.8/linktest/run.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.7/linktest/run_testcase_thread.py` & `linktest-2.4.8/linktest/run_testcase_thread.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.7/linktest/scp_report_to_specified_path.py` & `linktest-2.4.8/linktest/scp_report_to_specified_path.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.7/linktest/selenium_helper.py` & `linktest-2.4.8/linktest/selenium_helper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.7/linktest/timeout_thread.py` & `linktest-2.4.8/linktest/timeout_thread.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.7/linktest/ui_testcase.py` & `linktest-2.4.8/linktest/ui_testcase.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.7/linktest/update_config.py` & `linktest-2.4.8/linktest/update_config.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.7/linktest/webdriver_wrapper.py` & `linktest-2.4.8/linktest/webdriver_wrapper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.7/linktest/xml_report.py` & `linktest-2.4.8/linktest/xml_report.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.7/linktest.egg-info/SOURCES.txt` & `linktest-2.4.8/linktest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

