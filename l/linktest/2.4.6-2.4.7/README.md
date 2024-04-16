# Comparing `tmp/linktest-2.4.6.tar.gz` & `tmp/linktest-2.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linktest-2.4.6.tar", last modified: Mon Apr 15 15:07:24 2024, max compression
+gzip compressed data, was "linktest-2.4.7.tar", last modified: Tue Apr 16 05:22:50 2024, max compression
```

## Comparing `linktest-2.4.6.tar` & `linktest-2.4.7.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-15 15:07:24.951055 linktest-2.4.6/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-04-15 15:07:24.950725 linktest-2.4.6/PKG-INFO
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-15 15:07:24.945620 linktest-2.4.6/linktest/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       22 2024-04-15 15:04:31.000000 linktest-2.4.6/linktest/__init__.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      487 2024-04-15 14:20:10.000000 linktest-2.4.6/linktest/android_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      187 2024-04-15 14:20:10.000000 linktest-2.4.6/linktest/api_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10759 2024-04-15 14:20:10.000000 linktest-2.4.6/linktest/appium_utils.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    29054 2024-04-15 14:20:10.000000 linktest-2.4.6/linktest/auto_generate_testcase_list.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10302 2024-04-15 14:20:10.000000 linktest-2.4.6/linktest/auto_generate_testcase_list_from_csv.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9661 2024-04-15 14:20:10.000000 linktest-2.4.6/linktest/base_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1792 2024-04-15 14:20:10.000000 linktest-2.4.6/linktest/clean_data.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1403 2024-04-15 14:20:10.000000 linktest-2.4.6/linktest/conver_xml_into_db.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7260 2024-04-15 14:20:10.000000 linktest-2.4.6/linktest/database_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2471 2024-04-15 14:20:10.000000 linktest-2.4.6/linktest/date_utilities.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      232 2024-04-15 14:20:10.000000 linktest-2.4.6/linktest/detect_delimiter.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16523 2024-04-15 14:20:10.000000 linktest-2.4.6/linktest/doctor.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      959 2024-04-15 14:20:10.000000 linktest-2.4.6/linktest/framework_log.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     6233 2024-04-15 15:03:01.000000 linktest-2.4.6/linktest/generate_html_log.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      987 2024-04-15 14:20:10.000000 linktest-2.4.6/linktest/get_adb_devices.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      924 2024-04-15 14:20:10.000000 linktest-2.4.6/linktest/get_ios_devices_list.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1775 2024-04-15 14:20:10.000000 linktest-2.4.6/linktest/get_platform_info.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3137 2024-04-15 14:20:10.000000 linktest-2.4.6/linktest/get_project_info.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    34730 2024-04-15 14:20:10.000000 linktest-2.4.6/linktest/html_report.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      280 2024-04-15 14:20:10.000000 linktest-2.4.6/linktest/ios_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      195 2024-04-15 14:20:10.000000 linktest-2.4.6/linktest/linktest_setup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8745 2024-04-15 14:20:10.000000 linktest-2.4.6/linktest/logged_requests.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)   105356 2024-04-15 14:20:10.000000 linktest-2.4.6/linktest/main.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      982 2024-04-15 14:20:10.000000 linktest-2.4.6/linktest/memory_usage.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     4526 2024-04-15 14:20:10.000000 linktest-2.4.6/linktest/re_func.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1077 2024-04-15 14:20:10.000000 linktest-2.4.6/linktest/run.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1926 2024-04-15 14:20:10.000000 linktest-2.4.6/linktest/run_testcase_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1048 2024-04-15 14:20:10.000000 linktest-2.4.6/linktest/scp_report_to_specified_path.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8022 2024-04-15 14:20:10.000000 linktest-2.4.6/linktest/selenium_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      396 2024-04-15 14:20:10.000000 linktest-2.4.6/linktest/set_run_flag_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-04-15 15:04:40.000000 linktest-2.4.6/linktest/setup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      173 2024-04-15 14:20:10.000000 linktest-2.4.6/linktest/testcase_order.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      140 2024-04-15 14:20:10.000000 linktest-2.4.6/linktest/testcase_timeout_exception.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      801 2024-04-15 14:20:10.000000 linktest-2.4.6/linktest/timeout_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      931 2024-04-15 14:20:10.000000 linktest-2.4.6/linktest/ui_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3055 2024-04-15 14:20:10.000000 linktest-2.4.6/linktest/update_config.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    11186 2024-04-15 14:20:10.000000 linktest-2.4.6/linktest/webdriver_wrapper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      406 2024-04-15 14:20:10.000000 linktest-2.4.6/linktest/windows_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3544 2024-04-15 14:20:10.000000 linktest-2.4.6/linktest/xml_report.py
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-15 15:07:24.950332 linktest-2.4.6/linktest.egg-info/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-04-15 15:07:24.000000 linktest-2.4.6/linktest.egg-info/PKG-INFO
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1271 2024-04-15 15:07:24.000000 linktest-2.4.6/linktest.egg-info/SOURCES.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        1 2024-04-15 15:07:24.000000 linktest-2.4.6/linktest.egg-info/dependency_links.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      123 2024-04-15 15:07:24.000000 linktest-2.4.6/linktest.egg-info/requires.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        9 2024-04-15 15:07:24.000000 linktest-2.4.6/linktest.egg-info/top_level.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       38 2024-04-15 15:07:24.951119 linktest-2.4.6/setup.cfg
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-04-15 15:07:19.000000 linktest-2.4.6/setup.py
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-16 05:22:50.810490 linktest-2.4.7/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-04-16 05:22:50.810024 linktest-2.4.7/PKG-INFO
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-16 05:22:50.806121 linktest-2.4.7/linktest/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       22 2024-04-15 15:31:29.000000 linktest-2.4.7/linktest/__init__.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      487 2024-04-15 15:08:03.000000 linktest-2.4.7/linktest/android_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      187 2024-04-15 15:08:03.000000 linktest-2.4.7/linktest/api_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10759 2024-04-15 15:08:03.000000 linktest-2.4.7/linktest/appium_utils.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    29054 2024-04-15 15:08:03.000000 linktest-2.4.7/linktest/auto_generate_testcase_list.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10302 2024-04-15 15:08:03.000000 linktest-2.4.7/linktest/auto_generate_testcase_list_from_csv.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9940 2024-04-16 02:13:14.000000 linktest-2.4.7/linktest/base_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1792 2024-04-15 15:08:03.000000 linktest-2.4.7/linktest/clean_data.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1403 2024-04-15 15:08:03.000000 linktest-2.4.7/linktest/conver_xml_into_db.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7260 2024-04-15 15:08:03.000000 linktest-2.4.7/linktest/database_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2471 2024-04-15 15:08:03.000000 linktest-2.4.7/linktest/date_utilities.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      232 2024-04-15 15:08:03.000000 linktest-2.4.7/linktest/detect_delimiter.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16523 2024-04-15 15:08:03.000000 linktest-2.4.7/linktest/doctor.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      959 2024-04-15 15:08:03.000000 linktest-2.4.7/linktest/framework_log.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     6539 2024-04-15 15:30:06.000000 linktest-2.4.7/linktest/generate_html_log.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      987 2024-04-15 15:08:03.000000 linktest-2.4.7/linktest/get_adb_devices.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      924 2024-04-15 15:08:03.000000 linktest-2.4.7/linktest/get_ios_devices_list.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1775 2024-04-15 15:08:03.000000 linktest-2.4.7/linktest/get_platform_info.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3137 2024-04-15 15:08:03.000000 linktest-2.4.7/linktest/get_project_info.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    34730 2024-04-15 15:08:03.000000 linktest-2.4.7/linktest/html_report.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      280 2024-04-15 15:08:03.000000 linktest-2.4.7/linktest/ios_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      195 2024-04-15 15:08:03.000000 linktest-2.4.7/linktest/linktest_setup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8745 2024-04-15 15:08:03.000000 linktest-2.4.7/linktest/logged_requests.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)   105356 2024-04-15 15:08:03.000000 linktest-2.4.7/linktest/main.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      982 2024-04-15 15:08:03.000000 linktest-2.4.7/linktest/memory_usage.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     4526 2024-04-15 15:08:03.000000 linktest-2.4.7/linktest/re_func.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1077 2024-04-15 15:08:03.000000 linktest-2.4.7/linktest/run.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1926 2024-04-15 15:08:03.000000 linktest-2.4.7/linktest/run_testcase_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1048 2024-04-15 15:08:03.000000 linktest-2.4.7/linktest/scp_report_to_specified_path.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8022 2024-04-15 15:08:03.000000 linktest-2.4.7/linktest/selenium_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      396 2024-04-15 15:08:03.000000 linktest-2.4.7/linktest/set_run_flag_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-04-15 15:31:37.000000 linktest-2.4.7/linktest/setup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      173 2024-04-15 15:08:03.000000 linktest-2.4.7/linktest/testcase_order.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      140 2024-04-15 15:08:03.000000 linktest-2.4.7/linktest/testcase_timeout_exception.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      801 2024-04-15 15:08:03.000000 linktest-2.4.7/linktest/timeout_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      931 2024-04-15 15:08:03.000000 linktest-2.4.7/linktest/ui_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3055 2024-04-15 15:08:03.000000 linktest-2.4.7/linktest/update_config.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    11186 2024-04-15 15:08:03.000000 linktest-2.4.7/linktest/webdriver_wrapper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      406 2024-04-15 15:08:03.000000 linktest-2.4.7/linktest/windows_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3544 2024-04-15 15:08:03.000000 linktest-2.4.7/linktest/xml_report.py
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-16 05:22:50.809398 linktest-2.4.7/linktest.egg-info/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-04-16 05:22:50.000000 linktest-2.4.7/linktest.egg-info/PKG-INFO
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1271 2024-04-16 05:22:50.000000 linktest-2.4.7/linktest.egg-info/SOURCES.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        1 2024-04-16 05:22:50.000000 linktest-2.4.7/linktest.egg-info/dependency_links.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      123 2024-04-16 05:22:50.000000 linktest-2.4.7/linktest.egg-info/requires.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        9 2024-04-16 05:22:50.000000 linktest-2.4.7/linktest.egg-info/top_level.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       38 2024-04-16 05:22:50.810602 linktest-2.4.7/setup.cfg
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-04-16 05:22:44.000000 linktest-2.4.7/setup.py
```

### Comparing `linktest-2.4.6/linktest/appium_utils.py` & `linktest-2.4.7/linktest/appium_utils.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.6/linktest/auto_generate_testcase_list.py` & `linktest-2.4.7/linktest/auto_generate_testcase_list.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.6/linktest/auto_generate_testcase_list_from_csv.py` & `linktest-2.4.7/linktest/auto_generate_testcase_list_from_csv.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.6/linktest/base_testcase.py` & `linktest-2.4.7/linktest/base_testcase.py`

 * *Files 12% similar despite different names*

```diff
@@ -102,15 +102,15 @@
     def run_test(self):
         """
         this method must be implement by all backend test cases,
         each test case must encapsulate its business logic into a specific method which called run_test():
         def run_test(self):
             ...
         """
-        raise NotImplementedError("---subclass: %s must implement this method: run_test(self)!" % self)
+        raise NotImplementedError(" - subclass: %s must implement this method: run_test(self)!" % self)
 
     def teardown(self):
         """
         def teardown(self):
             ...
         """
         pass
@@ -121,69 +121,67 @@
             ...
         """
         pass
 
     def assert_equals(self, actual_val, expect_val):
         try:
             assert actual_val == expect_val
-            self.logger.info("assert actual_val: %s == expect_val: %s  ====== Passed" % (actual_val, expect_val))
+            self.logger.info("Assertion Passed: actual_val(%s) == expect_val(%s)", actual_val, expect_val)
+
         except AssertionError as e:
             e.args += ('expected value is %s' % expect_val, 'actual_val is %s' % actual_val)
-            self.logger.info("assert_equals(%s, %s)  ------ Failed" % (actual_val, expect_val))
+            self.logger.info("Assertion Failed: actual_val(%s) == expect_val(%s)", actual_val, expect_val)
             raise
 
     def assert_contains(self, source_val, target_val):
         try:
             if (
                     (type(source_val) == type(target_val)) and
                     (
                             type(source_val) == str or type(source_val) == int or type(source_val) == float
                     )
             ):
                 source_val_str = str(source_val)
                 target_val_str = str(target_val)
                 if source_val_str.__contains__(target_val_str):
                     self.logger.info(
-                        "assert_contains => source_val: %s, target_val: %s    => Passed" % (source_val, target_val))
+                        "assert_contains Passed => source_val: %s, target_val: %s" % (source_val, target_val))
                 else:
                     self.logger.error(
-                        "assert_contains => source_val: %s, target_val: %s    -------------------------> Failed" % (
-                            source_val, target_val))
+                        "assert_contains Failed => source_val: %s, target_val: %s " % (source_val, target_val))
                     raise RuntimeError(
-                        "assert_contains => source_val: %s, target_val: %s    -------------------------> Failed" % (
-                            source_val, target_val))
+                        "assert_contains Failed => source_val: %s, target_val: %s " % (source_val, target_val))
             else:
                 self.logger.error(
-                    "assert_contains => source_val: %s, target_val: %s     -------------------------> Failed, "
+                    "assert_contains Failed => source_val: %s, target_val: %s, "
                     "the type of params should be on of [str, int, float] " % (source_val, target_val))
                 raise RuntimeError(
-                    "assert_contains => source_val: %s, target_val: %s     -------------------------> Failed, "
+                    "assert_contains Failed => source_val: %s, target_val: %s , "
                     "the type of params should be on of [str, int, float] " % (source_val, target_val))
 
         except AssertionError as e:
             e.args += ('assert_contains => source_val is %s' % source_val, 'target_val is %s' % target_val)
             self.logger.error(
-                "assert_contains => source_val: %s, target_val: %s      -------------------------> Failed" % (
-                    source_val, target_val))
+                "assert_contains Failed => source_val: %s, target_val: %s " % (source_val, target_val))
             raise RuntimeError(
-                "assert_contains => source_val: %s, target_val: %s      -------------------------> Failed" % (
-                    source_val, target_val))
+                "assert_contains Failed => source_val: %s, target_val: %s " % (source_val, target_val))
 
     def assert_is_not_none(self, actual_val):
         try:
             assert actual_val is not None
-            self.logger.info("assert %s is not None      ====== Passed" % (actual_val))
+            self.logger.info("assert Passed %s is not None" % (actual_val))
         except AssertionError as e:
             e.args += ('expected value is not None', 'actual_val is %s' % actual_val)
-            self.logger.info("assert_is_not_none(%s)  -- Failed" % (actual_val))
+            self.logger.info("assert_is_not_none Failed => assert_is_not_none(%s)" % (actual_val))
             raise
 
     def compare_json_and_return_diff(self, expected_json, actual_json, rules=None):
         """
-        此方法 比较两个 json 时会忽略结构体内item的顺序,即如下 json1 & json2 会被认为是相同的
+        忽视JSON对象内部的键值对的顺序，即对象包含相同的键值对，即使顺序不同，也被视为相同的JSON对象。JSON对象的比较忽略键值对的顺序。
+        例如，以下两个JSON对象包含相同的键值对，即使顺序不同，也被视为相同的JSON对象：
         json1 = {
             "name": "linktest",
             "Company": {
                 "name": "IKEA",
                 "No": 1
             },
             "version": "1.0"
@@ -217,15 +215,25 @@
 
     def compare_json_and_assert_equal(self, expected_json, actual_json, rules=None):
         diff = self.compare_json_and_return_diff(expected_json, actual_json, rules)
         self.pprint(diff)
         assert diff == {}
 
     def compare_json_with_strict_mode(self, expected_json, actual_json):
-        """不会忽略json体内Item的顺序, 即: { "name": "linktest", "version": 1.0 } 和 {"version": 1.0, "name": "linktest" } 是不同的, 本质上就是当做字符串来比较"""
+        """
+        JSON对象内部的键值对顺序是有意义的，即使对象包含相同的键值对，但顺序不同，也应该被视为不同的对象。JSON对象的比较不应该忽略键值对的顺序。
+        例如，以下两个JSON对象虽然包含相同的键值对，但由于顺序不同，应该被视为不同的对象：
+        ```
+        { "name": "linktest", "version": 1.0 }
+        {"version": 1.0, "name": "linktest" }
+        ```
+        :param expected_json:
+        :param actual_json:
+        :return:
+        """
 
         self.logger.info("========================= Compare JSON Objects With Strict Mode =========================")
         v1 = json.dumps(expected_json, sort_keys=False)
         v2 = json.dumps(actual_json, sort_keys=False)
 
         self.logger.info("Expected JSON: ")
         self.logger.info(self.pformat(v1))
```

### Comparing `linktest-2.4.6/linktest/clean_data.py` & `linktest-2.4.7/linktest/clean_data.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.6/linktest/conver_xml_into_db.py` & `linktest-2.4.7/linktest/conver_xml_into_db.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.6/linktest/database_helper.py` & `linktest-2.4.7/linktest/database_helper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.6/linktest/date_utilities.py` & `linktest-2.4.7/linktest/date_utilities.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.6/linktest/doctor.py` & `linktest-2.4.7/linktest/doctor.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.6/linktest/framework_log.py` & `linktest-2.4.7/linktest/framework_log.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.6/linktest/generate_html_log.py` & `linktest-2.4.7/linktest/generate_html_log.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,16 +97,16 @@
             line = line.replace(f"'{action_name}'", f"<b style='color:#006600'>'{action_name}'</b>")
             if "args" in line:
                 line = line.replace("args", "<b style='color:#333333'>args</b>")
 
         if "WebDriver Action:</span> <b style='color:#006600'>'save_screenshot'</b> with <b style='color:#333333'>args</b>:" in line:
             line += "<img src='" + line.split("WebDriver Action:</span> <b style='color:#006600'>'save_screenshot'</b> with <b style='color:#333333'>args</b>:")[1].strip() + "' width='100%'>"
 
-        if "logged_requests.py" in line:
-            line = line.replace("logged_requests.py", "<span style='color:#0066CC'>logged_requests.py</span>")
+        # if "logged_requests.py" in line:
+        #     line = line.replace("logged_requests.py", "<span style='color:#0066CC'>logged_requests.py</span>")
 
         if "run_test() Start" in line:
             line = line.replace("run_test() Start", "<strong style='color:#0066CC'>run_test() Start</strong>")
 
         if " POST Request Started" in line:
             line = line.replace(" POST Request Started", "<strong style='color:#0066CC'> POST Request Started</strong>")
 
@@ -130,14 +130,20 @@
 
         if "Response [200]" in line:
             line = line.replace("Response [200]", "<strong style='color:green'>Response [200]</strong>")
 
         if "Response [500]" in line:
             line = line.replace("Response [500]", "<strong style='color:red'>Response [500]</strong>")
 
+        if "Assertion Passed:" in line:
+            line = line.replace("Assertion Passed:", "<strong style='color:green'>Assertion Passed:</strong>")
+
+        if "Assertion Failed:" in line:
+            line = line.replace("Assertion Failed:", "<strong style='color:red'>Assertion Failed:</strong>")
+
 
         if line == "\n":
             continue
 
         if starts_with_date(line):
             if single_line_flag:
                 html_content += f'<div class="{class_name}"><p>{lines}</p></div>'
```

### Comparing `linktest-2.4.6/linktest/get_adb_devices.py` & `linktest-2.4.7/linktest/get_adb_devices.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.6/linktest/get_ios_devices_list.py` & `linktest-2.4.7/linktest/get_ios_devices_list.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.6/linktest/get_platform_info.py` & `linktest-2.4.7/linktest/get_platform_info.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.6/linktest/get_project_info.py` & `linktest-2.4.7/linktest/get_project_info.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.6/linktest/html_report.py` & `linktest-2.4.7/linktest/html_report.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.6/linktest/logged_requests.py` & `linktest-2.4.7/linktest/logged_requests.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.6/linktest/main.py` & `linktest-2.4.7/linktest/main.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.6/linktest/memory_usage.py` & `linktest-2.4.7/linktest/memory_usage.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.6/linktest/re_func.py` & `linktest-2.4.7/linktest/re_func.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.6/linktest/run.py` & `linktest-2.4.7/linktest/run.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.6/linktest/run_testcase_thread.py` & `linktest-2.4.7/linktest/run_testcase_thread.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.6/linktest/scp_report_to_specified_path.py` & `linktest-2.4.7/linktest/scp_report_to_specified_path.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.6/linktest/selenium_helper.py` & `linktest-2.4.7/linktest/selenium_helper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.6/linktest/timeout_thread.py` & `linktest-2.4.7/linktest/timeout_thread.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.6/linktest/ui_testcase.py` & `linktest-2.4.7/linktest/ui_testcase.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.6/linktest/update_config.py` & `linktest-2.4.7/linktest/update_config.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.6/linktest/webdriver_wrapper.py` & `linktest-2.4.7/linktest/webdriver_wrapper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.6/linktest/xml_report.py` & `linktest-2.4.7/linktest/xml_report.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.6/linktest.egg-info/SOURCES.txt` & `linktest-2.4.7/linktest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

