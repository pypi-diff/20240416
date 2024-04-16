# Comparing `tmp/linktest-2.4.9.tar.gz` & `tmp/linktest-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linktest-2.4.9.tar", last modified: Tue Apr 16 06:04:45 2024, max compression
+gzip compressed data, was "linktest-2.5.1.tar", last modified: Tue Apr 16 07:14:44 2024, max compression
```

## Comparing `linktest-2.4.9.tar` & `linktest-2.5.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-16 06:04:45.208546 linktest-2.4.9/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-04-16 06:04:45.208205 linktest-2.4.9/PKG-INFO
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-16 06:04:45.206120 linktest-2.4.9/linktest/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       22 2024-04-16 06:02:56.000000 linktest-2.4.9/linktest/__init__.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      487 2024-04-16 05:51:00.000000 linktest-2.4.9/linktest/android_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      187 2024-04-16 05:51:00.000000 linktest-2.4.9/linktest/api_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10759 2024-04-16 05:51:00.000000 linktest-2.4.9/linktest/appium_utils.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    29054 2024-04-16 05:51:00.000000 linktest-2.4.9/linktest/auto_generate_testcase_list.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10302 2024-04-16 05:51:00.000000 linktest-2.4.9/linktest/auto_generate_testcase_list_from_csv.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9940 2024-04-16 05:51:00.000000 linktest-2.4.9/linktest/base_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1792 2024-04-16 05:51:00.000000 linktest-2.4.9/linktest/clean_data.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1403 2024-04-16 05:51:00.000000 linktest-2.4.9/linktest/conver_xml_into_db.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7260 2024-04-16 05:51:00.000000 linktest-2.4.9/linktest/database_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2471 2024-04-16 05:51:00.000000 linktest-2.4.9/linktest/date_utilities.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      232 2024-04-16 05:51:00.000000 linktest-2.4.9/linktest/detect_delimiter.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16523 2024-04-16 05:51:00.000000 linktest-2.4.9/linktest/doctor.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      959 2024-04-16 05:51:00.000000 linktest-2.4.9/linktest/framework_log.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7003 2024-04-16 06:02:41.000000 linktest-2.4.9/linktest/generate_html_log.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      987 2024-04-16 05:51:00.000000 linktest-2.4.9/linktest/get_adb_devices.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      924 2024-04-16 05:51:00.000000 linktest-2.4.9/linktest/get_ios_devices_list.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1775 2024-04-16 05:51:00.000000 linktest-2.4.9/linktest/get_platform_info.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3137 2024-04-16 05:51:00.000000 linktest-2.4.9/linktest/get_project_info.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    34730 2024-04-16 05:51:00.000000 linktest-2.4.9/linktest/html_report.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      280 2024-04-16 05:51:00.000000 linktest-2.4.9/linktest/ios_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      195 2024-04-16 05:51:00.000000 linktest-2.4.9/linktest/linktest_setup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8745 2024-04-16 05:51:00.000000 linktest-2.4.9/linktest/logged_requests.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)   105356 2024-04-16 05:51:00.000000 linktest-2.4.9/linktest/main.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      982 2024-04-16 05:51:00.000000 linktest-2.4.9/linktest/memory_usage.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     4526 2024-04-16 05:51:00.000000 linktest-2.4.9/linktest/re_func.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1077 2024-04-16 05:51:00.000000 linktest-2.4.9/linktest/run.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1926 2024-04-16 05:51:00.000000 linktest-2.4.9/linktest/run_testcase_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1048 2024-04-16 05:51:00.000000 linktest-2.4.9/linktest/scp_report_to_specified_path.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8022 2024-04-16 05:51:00.000000 linktest-2.4.9/linktest/selenium_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      396 2024-04-16 05:51:00.000000 linktest-2.4.9/linktest/set_run_flag_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-04-16 06:03:01.000000 linktest-2.4.9/linktest/setup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      173 2024-04-16 05:51:00.000000 linktest-2.4.9/linktest/testcase_order.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      140 2024-04-16 05:51:00.000000 linktest-2.4.9/linktest/testcase_timeout_exception.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      801 2024-04-16 05:51:00.000000 linktest-2.4.9/linktest/timeout_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      931 2024-04-16 05:51:00.000000 linktest-2.4.9/linktest/ui_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3055 2024-04-16 05:51:00.000000 linktest-2.4.9/linktest/update_config.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    11186 2024-04-16 05:51:00.000000 linktest-2.4.9/linktest/webdriver_wrapper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      406 2024-04-16 05:51:00.000000 linktest-2.4.9/linktest/windows_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3544 2024-04-16 05:51:00.000000 linktest-2.4.9/linktest/xml_report.py
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-16 06:04:45.207937 linktest-2.4.9/linktest.egg-info/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-04-16 06:04:44.000000 linktest-2.4.9/linktest.egg-info/PKG-INFO
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1271 2024-04-16 06:04:44.000000 linktest-2.4.9/linktest.egg-info/SOURCES.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        1 2024-04-16 06:04:44.000000 linktest-2.4.9/linktest.egg-info/dependency_links.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      123 2024-04-16 06:04:44.000000 linktest-2.4.9/linktest.egg-info/requires.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        9 2024-04-16 06:04:44.000000 linktest-2.4.9/linktest.egg-info/top_level.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       38 2024-04-16 06:04:45.208583 linktest-2.4.9/setup.cfg
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-04-16 06:04:40.000000 linktest-2.4.9/setup.py
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-16 07:14:44.652739 linktest-2.5.1/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-04-16 07:14:44.652369 linktest-2.5.1/PKG-INFO
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-16 07:14:44.646861 linktest-2.5.1/linktest/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       22 2024-04-16 07:12:22.000000 linktest-2.5.1/linktest/__init__.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      487 2024-04-16 06:05:20.000000 linktest-2.5.1/linktest/android_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      187 2024-04-16 06:05:20.000000 linktest-2.5.1/linktest/api_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10759 2024-04-16 06:05:20.000000 linktest-2.5.1/linktest/appium_utils.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    29054 2024-04-16 06:05:20.000000 linktest-2.5.1/linktest/auto_generate_testcase_list.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10302 2024-04-16 06:05:20.000000 linktest-2.5.1/linktest/auto_generate_testcase_list_from_csv.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9940 2024-04-16 06:05:20.000000 linktest-2.5.1/linktest/base_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1792 2024-04-16 06:05:20.000000 linktest-2.5.1/linktest/clean_data.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1403 2024-04-16 06:05:20.000000 linktest-2.5.1/linktest/conver_xml_into_db.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7260 2024-04-16 06:05:20.000000 linktest-2.5.1/linktest/database_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2471 2024-04-16 06:05:20.000000 linktest-2.5.1/linktest/date_utilities.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      232 2024-04-16 06:05:20.000000 linktest-2.5.1/linktest/detect_delimiter.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16523 2024-04-16 06:05:20.000000 linktest-2.5.1/linktest/doctor.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      959 2024-04-16 06:05:20.000000 linktest-2.5.1/linktest/framework_log.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8530 2024-04-16 06:43:54.000000 linktest-2.5.1/linktest/generate_html_log.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      987 2024-04-16 06:05:20.000000 linktest-2.5.1/linktest/get_adb_devices.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      924 2024-04-16 06:05:20.000000 linktest-2.5.1/linktest/get_ios_devices_list.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1775 2024-04-16 06:05:20.000000 linktest-2.5.1/linktest/get_platform_info.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3137 2024-04-16 06:05:20.000000 linktest-2.5.1/linktest/get_project_info.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    34730 2024-04-16 07:10:16.000000 linktest-2.5.1/linktest/html_report.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      280 2024-04-16 06:05:20.000000 linktest-2.5.1/linktest/ios_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      195 2024-04-16 06:05:20.000000 linktest-2.5.1/linktest/linktest_setup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8745 2024-04-16 06:05:20.000000 linktest-2.5.1/linktest/logged_requests.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)   105356 2024-04-16 06:05:20.000000 linktest-2.5.1/linktest/main.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      982 2024-04-16 06:05:20.000000 linktest-2.5.1/linktest/memory_usage.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     4526 2024-04-16 06:05:20.000000 linktest-2.5.1/linktest/re_func.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1077 2024-04-16 06:05:20.000000 linktest-2.5.1/linktest/run.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1926 2024-04-16 06:05:20.000000 linktest-2.5.1/linktest/run_testcase_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1048 2024-04-16 06:05:20.000000 linktest-2.5.1/linktest/scp_report_to_specified_path.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8022 2024-04-16 06:05:20.000000 linktest-2.5.1/linktest/selenium_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      396 2024-04-16 06:05:20.000000 linktest-2.5.1/linktest/set_run_flag_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-04-16 07:12:31.000000 linktest-2.5.1/linktest/setup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      173 2024-04-16 06:05:20.000000 linktest-2.5.1/linktest/testcase_order.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      140 2024-04-16 06:05:20.000000 linktest-2.5.1/linktest/testcase_timeout_exception.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      801 2024-04-16 06:05:20.000000 linktest-2.5.1/linktest/timeout_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      931 2024-04-16 06:05:20.000000 linktest-2.5.1/linktest/ui_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3055 2024-04-16 06:05:20.000000 linktest-2.5.1/linktest/update_config.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    11186 2024-04-16 06:05:20.000000 linktest-2.5.1/linktest/webdriver_wrapper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      406 2024-04-16 06:05:20.000000 linktest-2.5.1/linktest/windows_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3544 2024-04-16 06:05:20.000000 linktest-2.5.1/linktest/xml_report.py
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-16 07:14:44.651735 linktest-2.5.1/linktest.egg-info/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-04-16 07:14:44.000000 linktest-2.5.1/linktest.egg-info/PKG-INFO
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1271 2024-04-16 07:14:44.000000 linktest-2.5.1/linktest.egg-info/SOURCES.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        1 2024-04-16 07:14:44.000000 linktest-2.5.1/linktest.egg-info/dependency_links.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      123 2024-04-16 07:14:44.000000 linktest-2.5.1/linktest.egg-info/requires.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        9 2024-04-16 07:14:44.000000 linktest-2.5.1/linktest.egg-info/top_level.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       38 2024-04-16 07:14:44.652809 linktest-2.5.1/setup.cfg
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-04-16 07:14:35.000000 linktest-2.5.1/setup.py
```

### Comparing `linktest-2.4.9/linktest/appium_utils.py` & `linktest-2.5.1/linktest/appium_utils.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.9/linktest/auto_generate_testcase_list.py` & `linktest-2.5.1/linktest/auto_generate_testcase_list.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.9/linktest/auto_generate_testcase_list_from_csv.py` & `linktest-2.5.1/linktest/auto_generate_testcase_list_from_csv.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.9/linktest/base_testcase.py` & `linktest-2.5.1/linktest/base_testcase.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.9/linktest/clean_data.py` & `linktest-2.5.1/linktest/clean_data.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.9/linktest/conver_xml_into_db.py` & `linktest-2.5.1/linktest/conver_xml_into_db.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.9/linktest/database_helper.py` & `linktest-2.5.1/linktest/database_helper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.9/linktest/date_utilities.py` & `linktest-2.5.1/linktest/date_utilities.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.9/linktest/doctor.py` & `linktest-2.5.1/linktest/doctor.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.9/linktest/framework_log.py` & `linktest-2.5.1/linktest/framework_log.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.9/linktest/generate_html_log.py` & `linktest-2.5.1/linktest/generate_html_log.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 import os
-
 import re
-
+import json
 
 def starts_with_date(input_string):
     # 正则表达式匹配 YYYY-MM-DD 格式的日期
     pattern = r'^\d{4}-\d{2}-\d{2}'
 
     # 使用 re.match 检查字符串开头是否匹配该模式
     if re.match(pattern, input_string):
         return True
     else:
         return False
 
 
-import json
+def is_logged_requests_line(line):
+    pattern = r"logged_requests\.py \d+:$"
+    return bool(re.search(pattern, line))
+
 
 def format_json(json_string):
     try:
         parsed_json = json.loads(json_string)
         formatted_json = json.dumps(parsed_json, indent=2)
         return formatted_json.replace(" ", "&nbsp;").replace("\n", "<br>")
     except json.JSONDecodeError:
         return json_string
 
+
 def generate_html_log(executing_testcase):
     # executing_testcase.logfile_full_name 是日志文件的完整路径
     # executing_testcase.full_tc_folder 是存放生成的HTML文件的目录
 
     # 读取日志文件内容
     with open(executing_testcase.logfile_full_name, "r") as logfile:
         execution_log = logfile.readlines()
@@ -61,14 +64,22 @@
             .log-entry {
                 margin-bottom: 10px;
                 padding: 10px;
                 background-color: #f9f9f9;
                 border-left: 5px solid #2196F3;
                 font-size: 16px;
             }
+            .only-time-Log-entry {
+                margin-bottom: 1px;
+                margin-top: -8px;
+                padding: 8px;
+                background-color: #f9f9f9;
+                border-left: 5px solid #2196F3;
+                font-size: 12px;
+            }
             .error {
                 border-left-color: #f44336;
             }
             .info {
                 border-left-color: #4CAF50;
             }
             .timestamp {
@@ -85,18 +96,21 @@
     lines = ""
     single_line_flag = False
 
     # 将日志行转换为HTML元素
     for line in execution_log:
         line = line.replace("<", "&lt;").replace(">", "&gt;")
         class_name = "log-entry"
+        cls_name_only_time_Log_entry = "only-time-Log-entry"
         if "ERROR" in line:
             class_name += " error"
+            cls_name_only_time_Log_entry += " error"
         elif "INFO" in line:
             class_name += " info"
+            cls_name_only_time_Log_entry += " info"
 
         if "WebDriver Action:" in line:
             action_name = line.split("'")[1]
             line = line.replace("WebDriver Action:", "<span style='color:#0066CC'>WebDriver Action:</span>")
             line = line.replace(f"'{action_name}'", f"<b style='color:#006600'>'{action_name}'</b>")
             if "args" in line:
                 line = line.replace("args", "<b style='color:#333333'>args</b>")
@@ -146,29 +160,42 @@
 
         if "Assertion Passed:" in line:
             line = line.replace("Assertion Passed:", "<strong style='color:green'>Assertion Passed:</strong>")
 
         if "Assertion Failed:" in line:
             line = line.replace("Assertion Failed:", "<strong style='color:red'>Assertion Failed:</strong>")
 
+        if "logged_requests.py" in line:
+            if "URL:" in line and "logged_requests.py" in line.split("URL:")[0]:
+                line = line.replace("URL:", f"<strong style='color:#0066CC'>URL:</strong>")
+            if "JSON:" in line and "logged_requests.py" in line.split("JSON:")[0]:
+                line = line.replace("JSON:",f"<strong style='color:#0066CC'>JSON:</strong>")
+            if "kwargs:" in line and "logged_requests.py" in line.split("kwargs:")[0]:
+                line = line.replace("kwargs:",f"<strong style='color:#0066CC'>kwargs:</strong>")
 
         if line == "\n":
             continue
 
         if starts_with_date(line):
             if single_line_flag:
                 if lines.startswith("{"):
                     html_content += f'<div class="{class_name}"><pre>{format_json(lines)}</pre></div>'
                 else:
-                    html_content += f'<div class="{class_name}"><p>{lines}</p></div>'
+                    if lines.startswith("curl "):
+                        html_content += f'<div class="{class_name}"><b style="color: darkorange;">{lines}</b></div>'
+                    else:
+                        html_content += f'<div class="{class_name}"><pre>{lines}</pre></div>'
                 lines = ""
                 single_line_flag = False
 
             timestamp = line.split(" ")[0] + " " + line.split(" ")[1]
-            html_content += f'<div class="{class_name}"><span class="timestamp">{timestamp}</span><p>{line[len(timestamp):].strip()}</p></div>'
+            if is_logged_requests_line(line[len(timestamp):].strip()):
+                html_content += f'<div class="{cls_name_only_time_Log_entry}">{line.strip()}</div>'
+            else:
+                html_content += f'<div class="{class_name}"><span class="timestamp">{timestamp}</span><p>{line[len(timestamp):].strip()}</p></div>'
         else:
             lines += line.replace("\n", "<br>")
             single_line_flag = True
             continue
 
     html_content += """
         </div>
```

### Comparing `linktest-2.4.9/linktest/get_adb_devices.py` & `linktest-2.5.1/linktest/get_adb_devices.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.9/linktest/get_ios_devices_list.py` & `linktest-2.5.1/linktest/get_ios_devices_list.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.9/linktest/get_platform_info.py` & `linktest-2.5.1/linktest/get_platform_info.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.9/linktest/get_project_info.py` & `linktest-2.5.1/linktest/get_project_info.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.9/linktest/html_report.py` & `linktest-2.5.1/linktest/html_report.py`

 * *Files 0% similar despite different names*

```diff
@@ -312,44 +312,44 @@
                     testcase_filter_tag = testcase.__module__[0:testcase.__module__.rfind(".")]
                     map_testcases_package(all_testcases_package, tc_map_tag, testcase_filter_tag, testcase)
 
             # generate the drop down list for all the different tags
             # 判断是不需要显示 'show Global Data List' button
             if create_global_data_list_flag:
                 html_drop_down_list = """
-                            <table border='0' align='center' width='1080'>
+                            <table border='0' align='center' width='1050'>
                                 <tr>
                                     <td width='280'><font style='color: black; font-size: 18; margin-left: -30'><a class="btn btn-success" target='_blank' role='button'
                                          href='%s'>View Global Data</a></font></td>
                                     
                                 </tr>
                             </table>
                             
-                            <table border='0' align='center' width='1080'>
+                            <table border='0' align='center' width='1050'>
                                 <tr>
-                                    <td width='280'><font style='color: black; font-size: 18; margin-left: -30'>Filter Cases By Package: </font></td>
+                                    <td width='285'><font style='color: black; font-size: 18; margin-left: -30'>Filter Cases By Package: </font></td>
                                     <td>
                             """ % (output_folder + os.sep + "global_data_list.py")
             else:
                 html_drop_down_list = """
             <br>
-            <table border='0' align='center' width='1020'>
+            <table border='0' align='center' width='1050'>
                 <tr>
-                    <td width='285'><strong style='color: #555555; font-size: 18; margin-left: -50'>Filter Cases By Package: </strong></td>
+                    <td width='285'><strong style='color: #555555; font-size: 18; margin-left: -30'>Filter Cases By Package: </strong></td>
                     <td>
             """
 
             report_file_handler.write(html_drop_down_list)
 
             all_testcases_package_list = []
             for testcase in all_testcases_package:
                 all_testcases_package_list.append(testcase)
 
             all_testcases_package_list.sort()
-            report_file_handler.write("<select class='form-select' style='margin-left: -120px; overflow: hidden; text-overflow: ellipsis; width: 650;' id=\"testcase_tag\" onchange=\"changeTag()\">")
+            report_file_handler.write("<select class='form-select' style='margin-left: -100px; overflow: hidden; text-overflow: ellipsis; width: 650;' id=\"testcase_tag\" onchange=\"changeTag()\">")
             for testcase in all_testcases_package_list:
                 report_file_handler.write("<option value='%s'>" % testcase)
                 report_file_handler.write("%s" % testcase)
                 report_file_handler.write("</option>")
             report_file_handler.write("</select>")
             report_file_handler.write("</td><td align='left'><p id='copy_status_info'></p></td><td>")
```

### Comparing `linktest-2.4.9/linktest/logged_requests.py` & `linktest-2.5.1/linktest/logged_requests.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.9/linktest/main.py` & `linktest-2.5.1/linktest/main.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.9/linktest/memory_usage.py` & `linktest-2.5.1/linktest/memory_usage.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.9/linktest/re_func.py` & `linktest-2.5.1/linktest/re_func.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.9/linktest/run.py` & `linktest-2.5.1/linktest/run.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.9/linktest/run_testcase_thread.py` & `linktest-2.5.1/linktest/run_testcase_thread.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.9/linktest/scp_report_to_specified_path.py` & `linktest-2.5.1/linktest/scp_report_to_specified_path.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.9/linktest/selenium_helper.py` & `linktest-2.5.1/linktest/selenium_helper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.9/linktest/timeout_thread.py` & `linktest-2.5.1/linktest/timeout_thread.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.9/linktest/ui_testcase.py` & `linktest-2.5.1/linktest/ui_testcase.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.9/linktest/update_config.py` & `linktest-2.5.1/linktest/update_config.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.9/linktest/webdriver_wrapper.py` & `linktest-2.5.1/linktest/webdriver_wrapper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.9/linktest/xml_report.py` & `linktest-2.5.1/linktest/xml_report.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.9/linktest.egg-info/SOURCES.txt` & `linktest-2.5.1/linktest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

