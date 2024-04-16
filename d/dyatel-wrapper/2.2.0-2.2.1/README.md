# Comparing `tmp/dyatel-wrapper-2.2.0.tar.gz` & `tmp/dyatel-wrapper-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dyatel-wrapper-2.2.0.tar", last modified: Sun Mar  3 23:29:04 2024, max compression
+gzip compressed data, was "dyatel-wrapper-2.2.1.tar", last modified: Tue Apr 16 16:26:26 2024, max compression
```

## Comparing `dyatel-wrapper-2.2.0.tar` & `dyatel-wrapper-2.2.1.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 pvladimir   (502) staff       (20)        0 2024-03-03 23:29:04.080208 dyatel-wrapper-2.2.0/
--rw-r--r--   0 pvladimir   (502) staff       (20)    11347 2023-04-12 09:28:58.000000 dyatel-wrapper-2.2.0/LICENSE
--rw-r--r--   0 pvladimir   (502) staff       (20)     1451 2024-03-03 23:29:04.080003 dyatel-wrapper-2.2.0/PKG-INFO
--rw-r--r--   0 pvladimir   (502) staff       (20)      179 2023-01-16 08:38:34.000000 dyatel-wrapper-2.2.0/README.md
-drwxr-xr-x   0 pvladimir   (502) staff       (20)        0 2024-03-03 23:29:04.044607 dyatel-wrapper-2.2.0/dyatel/
-drwxr-xr-x   0 pvladimir   (502) staff       (20)        0 2024-03-03 23:29:04.047517 dyatel-wrapper-2.2.0/dyatel/abstraction/
--rw-r--r--   0 pvladimir   (502) staff       (20)    12082 2024-03-03 23:28:21.000000 dyatel-wrapper-2.2.0/dyatel/abstraction/driver_wrapper_abc.py
--rw-r--r--   0 pvladimir   (502) staff       (20)    17159 2024-03-03 23:28:21.000000 dyatel-wrapper-2.2.0/dyatel/abstraction/element_abc.py
--rw-r--r--   0 pvladimir   (502) staff       (20)     1427 2023-11-25 17:03:52.000000 dyatel-wrapper-2.2.0/dyatel/abstraction/mixin_abc.py
--rw-r--r--   0 pvladimir   (502) staff       (20)     2637 2023-09-07 07:44:45.000000 dyatel-wrapper-2.2.0/dyatel/abstraction/page_abc.py
-drwxr-xr-x   0 pvladimir   (502) staff       (20)        0 2024-03-03 23:29:04.053229 dyatel-wrapper-2.2.0/dyatel/base/
--rw-r--r--   0 pvladimir   (502) staff       (20)     8327 2024-03-03 23:28:21.000000 dyatel-wrapper-2.2.0/dyatel/base/driver_wrapper.py
--rw-r--r--   0 pvladimir   (502) staff       (20)    20667 2024-03-03 23:28:21.000000 dyatel-wrapper-2.2.0/dyatel/base/element.py
--rw-r--r--   0 pvladimir   (502) staff       (20)     2304 2023-09-07 07:44:45.000000 dyatel-wrapper-2.2.0/dyatel/base/group.py
--rw-r--r--   0 pvladimir   (502) staff       (20)     7062 2023-11-25 17:52:02.000000 dyatel-wrapper-2.2.0/dyatel/base/page.py
-drwxr-xr-x   0 pvladimir   (502) staff       (20)        0 2024-03-03 23:29:04.056764 dyatel-wrapper-2.2.0/dyatel/dyatel_play/
-drwxr-xr-x   0 pvladimir   (502) staff       (20)        0 2024-03-03 23:29:04.057894 dyatel-wrapper-2.2.0/dyatel/dyatel_play/helpers/
--rw-r--r--   0 pvladimir   (502) staff       (20)      283 2024-03-01 20:10:58.000000 dyatel-wrapper-2.2.0/dyatel/dyatel_play/helpers/Trace.py
--rw-r--r--   0 pvladimir   (502) staff       (20)     8670 2024-03-03 23:28:21.000000 dyatel-wrapper-2.2.0/dyatel/dyatel_play/play_driver.py
--rw-r--r--   0 pvladimir   (502) staff       (20)    13858 2024-03-03 23:28:21.000000 dyatel-wrapper-2.2.0/dyatel/dyatel_play/play_element.py
--rw-r--r--   0 pvladimir   (502) staff       (20)       52 2023-09-07 07:44:45.000000 dyatel-wrapper-2.2.0/dyatel/dyatel_play/play_page.py
-drwxr-xr-x   0 pvladimir   (502) staff       (20)        0 2024-03-03 23:29:04.058786 dyatel-wrapper-2.2.0/dyatel/dyatel_sel/
-drwxr-xr-x   0 pvladimir   (502) staff       (20)        0 2024-03-03 23:29:04.063572 dyatel-wrapper-2.2.0/dyatel/dyatel_sel/core/
--rw-r--r--   0 pvladimir   (502) staff       (20)     7975 2024-03-03 23:28:21.000000 dyatel-wrapper-2.2.0/dyatel/dyatel_sel/core/core_driver.py
--rw-r--r--   0 pvladimir   (502) staff       (20)    18747 2024-03-03 23:28:21.000000 dyatel-wrapper-2.2.0/dyatel/dyatel_sel/core/core_element.py
--rw-r--r--   0 pvladimir   (502) staff       (20)       52 2023-09-07 07:44:45.000000 dyatel-wrapper-2.2.0/dyatel/dyatel_sel/core/core_page.py
-drwxr-xr-x   0 pvladimir   (502) staff       (20)        0 2024-03-03 23:29:04.065407 dyatel-wrapper-2.2.0/dyatel/dyatel_sel/driver/
--rw-r--r--   0 pvladimir   (502) staff       (20)     9426 2024-03-03 23:28:21.000000 dyatel-wrapper-2.2.0/dyatel/dyatel_sel/driver/mobile_driver.py
--rw-r--r--   0 pvladimir   (502) staff       (20)     2269 2024-01-29 16:18:55.000000 dyatel-wrapper-2.2.0/dyatel/dyatel_sel/driver/web_driver.py
-drwxr-xr-x   0 pvladimir   (502) staff       (20)        0 2024-03-03 23:29:04.067522 dyatel-wrapper-2.2.0/dyatel/dyatel_sel/elements/
--rw-r--r--   0 pvladimir   (502) staff       (20)     5340 2024-03-03 23:28:21.000000 dyatel-wrapper-2.2.0/dyatel/dyatel_sel/elements/mobile_element.py
--rw-r--r--   0 pvladimir   (502) staff       (20)     2903 2024-03-03 23:28:21.000000 dyatel-wrapper-2.2.0/dyatel/dyatel_sel/elements/web_element.py
-drwxr-xr-x   0 pvladimir   (502) staff       (20)        0 2024-03-03 23:29:04.069650 dyatel-wrapper-2.2.0/dyatel/dyatel_sel/pages/
--rw-r--r--   0 pvladimir   (502) staff       (20)     1361 2023-11-25 17:03:52.000000 dyatel-wrapper-2.2.0/dyatel/dyatel_sel/pages/mobile_page.py
--rw-r--r--   0 pvladimir   (502) staff       (20)      116 2023-09-07 07:44:45.000000 dyatel-wrapper-2.2.0/dyatel/dyatel_sel/pages/web_page.py
--rw-r--r--   0 pvladimir   (502) staff       (20)      497 2023-04-12 09:28:58.000000 dyatel-wrapper-2.2.0/dyatel/dyatel_sel/sel_utils.py
--rw-r--r--   0 pvladimir   (502) staff       (20)     1638 2023-10-17 08:41:12.000000 dyatel-wrapper-2.2.0/dyatel/exceptions.py
--rw-r--r--   0 pvladimir   (502) staff       (20)     6007 2024-03-03 23:28:21.000000 dyatel-wrapper-2.2.0/dyatel/js_scripts.py
--rw-r--r--   0 pvladimir   (502) staff       (20)     1963 2023-09-07 07:44:45.000000 dyatel-wrapper-2.2.0/dyatel/keyboard_keys.py
-drwxr-xr-x   0 pvladimir   (502) staff       (20)        0 2024-03-03 23:29:04.070815 dyatel-wrapper-2.2.0/dyatel/mixins/
--rw-r--r--   0 pvladimir   (502) staff       (20)     1769 2023-11-25 17:03:56.000000 dyatel-wrapper-2.2.0/dyatel/mixins/driver_mixin.py
--rw-r--r--   0 pvladimir   (502) staff       (20)     2701 2023-11-25 17:03:56.000000 dyatel-wrapper-2.2.0/dyatel/mixins/internal_mixin.py
-drwxr-xr-x   0 pvladimir   (502) staff       (20)        0 2024-03-03 23:29:04.072847 dyatel-wrapper-2.2.0/dyatel/mixins/objects/
--rw-r--r--   0 pvladimir   (502) staff       (20)      261 2024-03-03 23:28:21.000000 dyatel-wrapper-2.2.0/dyatel/mixins/objects/box.py
--rw-r--r--   0 pvladimir   (502) staff       (20)      167 2024-03-03 23:28:21.000000 dyatel-wrapper-2.2.0/dyatel/mixins/objects/location.py
--rw-r--r--   0 pvladimir   (502) staff       (20)      172 2024-03-03 23:28:21.000000 dyatel-wrapper-2.2.0/dyatel/mixins/objects/size.py
--rw-r--r--   0 pvladimir   (502) staff       (20)     2999 2024-03-03 23:28:21.000000 dyatel-wrapper-2.2.0/dyatel/shared_utils.py
-drwxr-xr-x   0 pvladimir   (502) staff       (20)        0 2024-03-03 23:29:04.075291 dyatel-wrapper-2.2.0/dyatel/utils/
--rw-r--r--   0 pvladimir   (502) staff       (20)     8099 2024-03-03 23:28:21.000000 dyatel-wrapper-2.2.0/dyatel/utils/internal_utils.py
--rw-r--r--   0 pvladimir   (502) staff       (20)     2845 2023-11-25 17:03:52.000000 dyatel-wrapper-2.2.0/dyatel/utils/logs.py
--rw-r--r--   0 pvladimir   (502) staff       (20)     1515 2023-11-26 12:42:22.000000 dyatel-wrapper-2.2.0/dyatel/utils/previous_object_driver.py
--rw-r--r--   0 pvladimir   (502) staff       (20)     4034 2024-03-03 23:28:21.000000 dyatel-wrapper-2.2.0/dyatel/utils/selector_synchronizer.py
--rw-r--r--   0 pvladimir   (502) staff       (20)    17097 2024-03-03 23:28:21.000000 dyatel-wrapper-2.2.0/dyatel/visual_comparison.py
-drwxr-xr-x   0 pvladimir   (502) staff       (20)        0 2024-03-03 23:29:04.079271 dyatel-wrapper-2.2.0/dyatel_wrapper.egg-info/
--rw-r--r--   0 pvladimir   (502) staff       (20)     1451 2024-03-03 23:29:03.000000 dyatel-wrapper-2.2.0/dyatel_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 pvladimir   (502) staff       (20)     1382 2024-03-03 23:29:03.000000 dyatel-wrapper-2.2.0/dyatel_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 pvladimir   (502) staff       (20)        1 2024-03-03 23:29:03.000000 dyatel-wrapper-2.2.0/dyatel_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 pvladimir   (502) staff       (20)      136 2024-03-03 23:29:03.000000 dyatel-wrapper-2.2.0/dyatel_wrapper.egg-info/requires.txt
--rw-r--r--   0 pvladimir   (502) staff       (20)        7 2024-03-03 23:29:03.000000 dyatel-wrapper-2.2.0/dyatel_wrapper.egg-info/top_level.txt
--rw-r--r--   0 pvladimir   (502) staff       (20)       79 2024-03-03 23:29:04.081476 dyatel-wrapper-2.2.0/setup.cfg
--rw-r--r--   0 pvladimir   (502) staff       (20)     2334 2024-03-03 23:28:21.000000 dyatel-wrapper-2.2.0/setup.py
+drwxr-xr-x   0 pvladimir   (502) staff       (20)        0 2024-04-16 16:26:26.911593 dyatel-wrapper-2.2.1/
+-rw-r--r--   0 pvladimir   (502) staff       (20)    11347 2023-04-12 09:28:58.000000 dyatel-wrapper-2.2.1/LICENSE
+-rw-r--r--   0 pvladimir   (502) staff       (20)     1451 2024-04-16 16:26:26.911398 dyatel-wrapper-2.2.1/PKG-INFO
+-rw-r--r--   0 pvladimir   (502) staff       (20)      179 2023-01-16 08:38:34.000000 dyatel-wrapper-2.2.1/README.md
+drwxr-xr-x   0 pvladimir   (502) staff       (20)        0 2024-04-16 16:26:26.875964 dyatel-wrapper-2.2.1/dyatel/
+drwxr-xr-x   0 pvladimir   (502) staff       (20)        0 2024-04-16 16:26:26.879585 dyatel-wrapper-2.2.1/dyatel/abstraction/
+-rw-r--r--   0 pvladimir   (502) staff       (20)    12242 2024-04-16 16:24:57.000000 dyatel-wrapper-2.2.1/dyatel/abstraction/driver_wrapper_abc.py
+-rw-r--r--   0 pvladimir   (502) staff       (20)    17159 2024-03-03 23:28:21.000000 dyatel-wrapper-2.2.1/dyatel/abstraction/element_abc.py
+-rw-r--r--   0 pvladimir   (502) staff       (20)     1427 2023-11-25 17:03:52.000000 dyatel-wrapper-2.2.1/dyatel/abstraction/mixin_abc.py
+-rw-r--r--   0 pvladimir   (502) staff       (20)     2637 2023-09-07 07:44:45.000000 dyatel-wrapper-2.2.1/dyatel/abstraction/page_abc.py
+drwxr-xr-x   0 pvladimir   (502) staff       (20)        0 2024-04-16 16:26:26.884708 dyatel-wrapper-2.2.1/dyatel/base/
+-rw-r--r--   0 pvladimir   (502) staff       (20)     8635 2024-04-16 16:24:57.000000 dyatel-wrapper-2.2.1/dyatel/base/driver_wrapper.py
+-rw-r--r--   0 pvladimir   (502) staff       (20)    20667 2024-03-03 23:28:21.000000 dyatel-wrapper-2.2.1/dyatel/base/element.py
+-rw-r--r--   0 pvladimir   (502) staff       (20)     2304 2023-09-07 07:44:45.000000 dyatel-wrapper-2.2.1/dyatel/base/group.py
+-rw-r--r--   0 pvladimir   (502) staff       (20)     7062 2023-11-25 17:52:02.000000 dyatel-wrapper-2.2.1/dyatel/base/page.py
+drwxr-xr-x   0 pvladimir   (502) staff       (20)        0 2024-04-16 16:26:26.887090 dyatel-wrapper-2.2.1/dyatel/dyatel_play/
+drwxr-xr-x   0 pvladimir   (502) staff       (20)        0 2024-04-16 16:26:26.888049 dyatel-wrapper-2.2.1/dyatel/dyatel_play/helpers/
+-rw-r--r--   0 pvladimir   (502) staff       (20)      283 2024-03-01 20:10:58.000000 dyatel-wrapper-2.2.1/dyatel/dyatel_play/helpers/Trace.py
+-rw-r--r--   0 pvladimir   (502) staff       (20)     8790 2024-04-16 16:24:57.000000 dyatel-wrapper-2.2.1/dyatel/dyatel_play/play_driver.py
+-rw-r--r--   0 pvladimir   (502) staff       (20)    13858 2024-03-03 23:28:21.000000 dyatel-wrapper-2.2.1/dyatel/dyatel_play/play_element.py
+-rw-r--r--   0 pvladimir   (502) staff       (20)       52 2023-09-07 07:44:45.000000 dyatel-wrapper-2.2.1/dyatel/dyatel_play/play_page.py
+drwxr-xr-x   0 pvladimir   (502) staff       (20)        0 2024-04-16 16:26:26.889021 dyatel-wrapper-2.2.1/dyatel/dyatel_sel/
+drwxr-xr-x   0 pvladimir   (502) staff       (20)        0 2024-04-16 16:26:26.891926 dyatel-wrapper-2.2.1/dyatel/dyatel_sel/core/
+-rw-r--r--   0 pvladimir   (502) staff       (20)     7975 2024-03-03 23:28:21.000000 dyatel-wrapper-2.2.1/dyatel/dyatel_sel/core/core_driver.py
+-rw-r--r--   0 pvladimir   (502) staff       (20)    18716 2024-04-16 16:24:57.000000 dyatel-wrapper-2.2.1/dyatel/dyatel_sel/core/core_element.py
+-rw-r--r--   0 pvladimir   (502) staff       (20)       52 2023-09-07 07:44:45.000000 dyatel-wrapper-2.2.1/dyatel/dyatel_sel/core/core_page.py
+drwxr-xr-x   0 pvladimir   (502) staff       (20)        0 2024-04-16 16:26:26.893293 dyatel-wrapper-2.2.1/dyatel/dyatel_sel/driver/
+-rw-r--r--   0 pvladimir   (502) staff       (20)     9868 2024-04-16 16:24:57.000000 dyatel-wrapper-2.2.1/dyatel/dyatel_sel/driver/mobile_driver.py
+-rw-r--r--   0 pvladimir   (502) staff       (20)     2300 2024-04-16 16:24:57.000000 dyatel-wrapper-2.2.1/dyatel/dyatel_sel/driver/web_driver.py
+drwxr-xr-x   0 pvladimir   (502) staff       (20)        0 2024-04-16 16:26:26.894643 dyatel-wrapper-2.2.1/dyatel/dyatel_sel/elements/
+-rw-r--r--   0 pvladimir   (502) staff       (20)     5340 2024-03-03 23:28:21.000000 dyatel-wrapper-2.2.1/dyatel/dyatel_sel/elements/mobile_element.py
+-rw-r--r--   0 pvladimir   (502) staff       (20)     2903 2024-03-03 23:28:21.000000 dyatel-wrapper-2.2.1/dyatel/dyatel_sel/elements/web_element.py
+drwxr-xr-x   0 pvladimir   (502) staff       (20)        0 2024-04-16 16:26:26.896536 dyatel-wrapper-2.2.1/dyatel/dyatel_sel/pages/
+-rw-r--r--   0 pvladimir   (502) staff       (20)     1361 2023-11-25 17:03:52.000000 dyatel-wrapper-2.2.1/dyatel/dyatel_sel/pages/mobile_page.py
+-rw-r--r--   0 pvladimir   (502) staff       (20)      116 2023-09-07 07:44:45.000000 dyatel-wrapper-2.2.1/dyatel/dyatel_sel/pages/web_page.py
+-rw-r--r--   0 pvladimir   (502) staff       (20)      497 2023-04-12 09:28:58.000000 dyatel-wrapper-2.2.1/dyatel/dyatel_sel/sel_utils.py
+-rw-r--r--   0 pvladimir   (502) staff       (20)     1638 2023-10-17 08:41:12.000000 dyatel-wrapper-2.2.1/dyatel/exceptions.py
+-rw-r--r--   0 pvladimir   (502) staff       (20)     6007 2024-03-03 23:28:21.000000 dyatel-wrapper-2.2.1/dyatel/js_scripts.py
+-rw-r--r--   0 pvladimir   (502) staff       (20)     1963 2023-09-07 07:44:45.000000 dyatel-wrapper-2.2.1/dyatel/keyboard_keys.py
+drwxr-xr-x   0 pvladimir   (502) staff       (20)        0 2024-04-16 16:26:26.898892 dyatel-wrapper-2.2.1/dyatel/mixins/
+-rw-r--r--   0 pvladimir   (502) staff       (20)     1769 2023-11-25 17:03:56.000000 dyatel-wrapper-2.2.1/dyatel/mixins/driver_mixin.py
+-rw-r--r--   0 pvladimir   (502) staff       (20)     2701 2023-11-25 17:03:56.000000 dyatel-wrapper-2.2.1/dyatel/mixins/internal_mixin.py
+drwxr-xr-x   0 pvladimir   (502) staff       (20)        0 2024-04-16 16:26:26.902731 dyatel-wrapper-2.2.1/dyatel/mixins/objects/
+-rw-r--r--   0 pvladimir   (502) staff       (20)      261 2024-03-03 23:28:21.000000 dyatel-wrapper-2.2.1/dyatel/mixins/objects/box.py
+-rw-r--r--   0 pvladimir   (502) staff       (20)      167 2024-03-03 23:28:21.000000 dyatel-wrapper-2.2.1/dyatel/mixins/objects/location.py
+-rw-r--r--   0 pvladimir   (502) staff       (20)      172 2024-03-03 23:28:21.000000 dyatel-wrapper-2.2.1/dyatel/mixins/objects/size.py
+-rw-r--r--   0 pvladimir   (502) staff       (20)     2999 2024-03-03 23:28:21.000000 dyatel-wrapper-2.2.1/dyatel/shared_utils.py
+drwxr-xr-x   0 pvladimir   (502) staff       (20)        0 2024-04-16 16:26:26.906805 dyatel-wrapper-2.2.1/dyatel/utils/
+-rw-r--r--   0 pvladimir   (502) staff       (20)     8272 2024-04-16 16:24:57.000000 dyatel-wrapper-2.2.1/dyatel/utils/internal_utils.py
+-rw-r--r--   0 pvladimir   (502) staff       (20)     2845 2023-11-25 17:03:52.000000 dyatel-wrapper-2.2.1/dyatel/utils/logs.py
+-rw-r--r--   0 pvladimir   (502) staff       (20)     1515 2023-11-26 12:42:22.000000 dyatel-wrapper-2.2.1/dyatel/utils/previous_object_driver.py
+-rw-r--r--   0 pvladimir   (502) staff       (20)     4066 2024-04-16 16:24:57.000000 dyatel-wrapper-2.2.1/dyatel/utils/selector_synchronizer.py
+-rw-r--r--   0 pvladimir   (502) staff       (20)    17109 2024-04-16 16:24:57.000000 dyatel-wrapper-2.2.1/dyatel/visual_comparison.py
+drwxr-xr-x   0 pvladimir   (502) staff       (20)        0 2024-04-16 16:26:26.910687 dyatel-wrapper-2.2.1/dyatel_wrapper.egg-info/
+-rw-r--r--   0 pvladimir   (502) staff       (20)     1451 2024-04-16 16:26:26.000000 dyatel-wrapper-2.2.1/dyatel_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 pvladimir   (502) staff       (20)     1382 2024-04-16 16:26:26.000000 dyatel-wrapper-2.2.1/dyatel_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 pvladimir   (502) staff       (20)        1 2024-04-16 16:26:26.000000 dyatel-wrapper-2.2.1/dyatel_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 pvladimir   (502) staff       (20)      136 2024-04-16 16:26:26.000000 dyatel-wrapper-2.2.1/dyatel_wrapper.egg-info/requires.txt
+-rw-r--r--   0 pvladimir   (502) staff       (20)        7 2024-04-16 16:26:26.000000 dyatel-wrapper-2.2.1/dyatel_wrapper.egg-info/top_level.txt
+-rw-r--r--   0 pvladimir   (502) staff       (20)       79 2024-04-16 16:26:26.912246 dyatel-wrapper-2.2.1/setup.cfg
+-rw-r--r--   0 pvladimir   (502) staff       (20)     2334 2024-04-16 16:24:57.000000 dyatel-wrapper-2.2.1/setup.py
```

### Comparing `dyatel-wrapper-2.2.0/LICENSE` & `dyatel-wrapper-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dyatel-wrapper-2.2.0/PKG-INFO` & `dyatel-wrapper-2.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyatel-wrapper
-Version: 2.2.0
+Version: 2.2.1
 Summary: Wrapper of Selenium, Appium and Playwright with single API
 Home-page: https://github.com/EnvInc/dyatel
 Author: Podolian Vladimir
 Author-email: vladimir.podolyan64@gmail.com
 Project-URL: Source, https://github.com/EnvInc/dyatel
 Project-URL: Tracker, https://github.com/EnvInc/dyatel/issues
 Project-URL: Changelog, https://github.com/EnvInc/dyatel/blob/master/CHANGELOG.md
```

### Comparing `dyatel-wrapper-2.2.0/dyatel/abstraction/driver_wrapper_abc.py` & `dyatel-wrapper-2.2.1/dyatel/abstraction/driver_wrapper_abc.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,27 +10,37 @@
 
 
 class DriverWrapperABC(ABC):
     session = None
     label = None
     original_tab = None
 
-    driver = None
-    browser_name = None
+    anchor = None
 
     is_desktop = False
     is_selenium = False
     is_playwright = False
 
+    is_appium = False
     is_mobile = False
+    is_tablet = False
+
     is_ios = False
+    is_ios_tablet = False
+    is_ios_mobile = False
+
     is_android = False
+    is_android_tablet = False
+    is_android_mobile = False
+
     is_simulator = False
     is_real_device = False
 
+    browser_name = None
+
     def quit(self, silent: bool = False, trace_path: str = 'trace.zip'):
         """
         Quit the driver instance
 
         :param silent: erase log
         :param trace_path: Playwright only: path for the trace
         :return: None
```

### Comparing `dyatel-wrapper-2.2.0/dyatel/abstraction/element_abc.py` & `dyatel-wrapper-2.2.1/dyatel/abstraction/element_abc.py`

 * *Files identical despite different names*

### Comparing `dyatel-wrapper-2.2.0/dyatel/abstraction/mixin_abc.py` & `dyatel-wrapper-2.2.1/dyatel/abstraction/mixin_abc.py`

 * *Files identical despite different names*

### Comparing `dyatel-wrapper-2.2.0/dyatel/abstraction/page_abc.py` & `dyatel-wrapper-2.2.1/dyatel/abstraction/page_abc.py`

 * *Files identical despite different names*

### Comparing `dyatel-wrapper-2.2.0/dyatel/base/driver_wrapper.py` & `dyatel-wrapper-2.2.1/dyatel/base/driver_wrapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import Union, Type, List, Tuple, Any
+from typing import Union, Type, List, Tuple, Any, Optional
 
 from PIL import Image
 from appium.webdriver.webdriver import WebDriver as AppiumDriver
 from selenium.webdriver.remote.webdriver import WebDriver as SeleniumDriver
 from playwright.sync_api import (
     Browser as PlaywrightBrowser,
     BrowserContext as PlaywrightContext,
@@ -57,17 +57,26 @@
 
     anchor = None
 
     is_desktop = False
     is_selenium = False
     is_playwright = False
 
+    is_appium = False
     is_mobile = False
+    is_tablet = False
+
     is_ios = False
+    is_ios_tablet = False
+    is_ios_mobile = False
+
     is_android = False
+    is_android_tablet = False
+    is_android_mobile = False
+
     is_simulator = False
     is_real_device = False
 
     browser_name = None
 
     driver: Union[SeleniumDriver, AppiumDriver, PlaywrightDriver]
     instance: PlaywrightBrowser  # Only for playwright instance
@@ -91,24 +100,33 @@
         if cls.is_android:
             label = 'android'
         elif cls.is_ios:
             label = 'ios'
 
         return f'{cls.__name__}({self.label}={self.driver}) at {hex(id(self))}, platform={label}'
 
-    def __init__(self, driver: Union[PlaywrightBrowser, AppiumDriver, SeleniumDriver], *args, **kwargs):
+    def __init__(
+            self,
+            driver: Union[PlaywrightBrowser, AppiumDriver, SeleniumDriver],
+            mobile_resolution: Optional[bool] = False,
+            *args,
+            **kwargs
+    ):
         """
         Initializing of driver wrapper based on given driver source
 
         :param driver: appium or selenium or playwright driver to initialize
         """
         self.driver = driver
         self.session.add_session(self)
         self.label = f'{self.session.all_sessions.index(self) + 1}_driver'
         self.__init_base_class__(*args, **kwargs)
+        if mobile_resolution:
+            self.is_desktop = False
+            self.is_mobile = True
 
     def quit(self, silent: bool = False, trace_path: str = 'trace.zip'):
         """
         Quit the driver instance
 
         :param silent: erase log
         :param trace_path: Playwright only: path for the trace
@@ -211,21 +229,19 @@
         """
         Get driver wrapper class in according to given driver source, and set him as base class
 
         :return: None
         """
         if isinstance(self.driver, PlaywrightBrowser):
             self.is_playwright = True
-            self.is_desktop = True
             self._base_cls = PlayDriver
         elif isinstance(self.driver, AppiumDriver):
-            self.is_mobile = True
+            self.is_appium = True
             self._base_cls = MobileDriver
         elif isinstance(self.driver, SeleniumDriver):
-            self.is_desktop = True
             self.is_selenium = True
             self._base_cls = WebDriver
         else:
             raise DriverWrapperException(f'Cant specify {self.__class__.__name__}')
 
         self._set_static(self._base_cls)
         self._base_cls.__init__(self, driver=self.driver, *args, **kwargs)
```

### Comparing `dyatel-wrapper-2.2.0/dyatel/base/element.py` & `dyatel-wrapper-2.2.1/dyatel/base/element.py`

 * *Files identical despite different names*

### Comparing `dyatel-wrapper-2.2.0/dyatel/base/group.py` & `dyatel-wrapper-2.2.1/dyatel/base/group.py`

 * *Files identical despite different names*

### Comparing `dyatel-wrapper-2.2.0/dyatel/base/page.py` & `dyatel-wrapper-2.2.1/dyatel/base/page.py`

 * *Files identical despite different names*

### Comparing `dyatel-wrapper-2.2.0/dyatel/dyatel_play/play_driver.py` & `dyatel-wrapper-2.2.1/dyatel/dyatel_play/play_driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
     def __init__(self, driver: Browser, trace: Trace = None, *args, **kwargs):
         """
         Initializing of desktop web driver with playwright
 
         :param driver: playwright driver to initialize
         """
+        self.is_desktop = True
         self.trace = trace
         self.instance = driver
         self.context = driver.new_context(*args, **kwargs)
 
         if trace:
             self.context.tracing.start(**trace.__dict__)
 
@@ -113,23 +114,25 @@
         self.log('Going back')
         self.driver.go_back()
         return self
 
     def quit(self, silent: bool = False, trace_path: str = 'trace.zip'):
         """
         Quit the driver instance
+        Note: you should close browser instance by yourself
 
         :param silent: erase log
         :param trace_path: Playwright only: path for the trace
         :return: None
         """
         if self.trace and trace_path:
             self.context.tracing.stop(path=trace_path)
 
         self.driver.close()
+        self.context.close()
 
     def set_cookie(self, cookies: List[dict]) -> PlayDriver:
         """
         Adds a list of cookie dictionaries to current session
 
         domain: should be ".google.com" for url "https://google.com/some/url/"
```

### Comparing `dyatel-wrapper-2.2.0/dyatel/dyatel_play/play_element.py` & `dyatel-wrapper-2.2.1/dyatel/dyatel_play/play_element.py`

 * *Files identical despite different names*

### Comparing `dyatel-wrapper-2.2.0/dyatel/dyatel_sel/core/core_driver.py` & `dyatel-wrapper-2.2.1/dyatel/dyatel_sel/core/core_driver.py`

 * *Files identical despite different names*

### Comparing `dyatel-wrapper-2.2.0/dyatel/dyatel_sel/core/core_element.py` & `dyatel-wrapper-2.2.1/dyatel/dyatel_sel/core/core_element.py`

 * *Files 1% similar despite different names*

```diff
@@ -510,15 +510,15 @@
         :return: driver
         """
         base = self.driver
 
         if not base:
             raise DriverWrapperException("Can't find driver")
 
-        if self.driver_wrapper.is_ios or self.driver_wrapper.is_android:
+        if self.driver_wrapper.is_appium:
             if self.driver_wrapper.is_native_context:
                 return base
 
         if self.parent:
             base = self.parent._get_element(wait=wait)
 
         return base
```

### Comparing `dyatel-wrapper-2.2.0/dyatel/dyatel_sel/driver/mobile_driver.py` & `dyatel-wrapper-2.2.1/dyatel/dyatel_sel/driver/mobile_driver.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,56 +1,46 @@
 from __future__ import annotations
 
-from typing import Union, List
+from typing import Union, List, Optional
 
 from appium.webdriver.applicationstate import ApplicationState
 from appium.webdriver.common.touch_action import TouchAction
 from appium.webdriver.webdriver import WebDriver as AppiumDriver
 
 from dyatel.dyatel_sel.core.core_driver import CoreDriver
 
 
 class MobileDriver(CoreDriver):
 
+    bundle_id: Optional[str]
+
     def __init__(self, driver: AppiumDriver, *args, **kwargs):  # noqa
         """
         Initializing of mobile driver with appium
 
         :param driver: appium driver to initialize
         """
         self.caps = driver.capabilities
-
         self.browser_name = self.caps.get('browserName', None)
         self.is_web = bool(self.browser_name) or False
         self.is_app = self.caps.get('app', False)
 
-        self.is_android = self.caps.get('platformName').lower() == 'android'
-        self.is_ios = self.caps.get('platformName').lower() == 'ios'
-        self.is_simulator = self.caps.get('useSimulator')
-        self.is_real_device = not self.caps.get('useSimulator')
+        _set_static(self)
 
         self.native_context_name = 'NATIVE_APP'
         self.web_context_name = self.get_web_view_context() if self.is_ios else 'CHROMIUM'
         self.__is_native_context = None
         self.__is_web_context = None
 
         self.top_bar_height = None
         self.bottom_bar_height = None
 
         self.original_tab = None
         self.page_box = None
 
-        if self.is_app:
-            if self.is_ios:
-                self.bundle_id = self.caps.get('bundleId', 'undefined: bundleId')
-            elif self.is_android:
-                self.bundle_id = self.caps.get('appPackage', 'undefined: appPackage')
-            else:
-                raise Exception('Make sure that correct "platformName" capability specified')
-
         CoreDriver.__init__(self, driver=driver)
 
     def is_app_installed(self) -> bool:
         """
         Is app running checking
 
         :return: True if the app running
@@ -290,7 +280,36 @@
 
         if self.is_ios:
             TouchAction(self.driver).tap(x=x, y=y).perform()
         elif self.is_android:
             CoreDriver.click_by_coordinates(self, x=x, y=y, silent=True)
 
         return self
+
+
+def _set_static(obj) -> None:
+    """
+    Set static attributes for Appium driver wrapper
+
+    :return: None
+    """
+    obj.is_tablet = obj.caps.get('is_tablet', False)
+    obj.is_mobile = not obj.is_tablet
+
+    obj.is_ios = obj.caps.get('platformName').lower() == 'ios'
+    obj.is_ios_tablet = obj.is_ios and obj.is_tablet
+    obj.is_ios_mobile = obj.is_ios and obj.is_mobile
+
+    obj.is_android = obj.caps.get('platformName').lower() == 'android'
+    obj.is_android_tablet = obj.is_android and obj.is_tablet
+    obj.is_android_mobile = obj.is_android and obj.is_mobile
+
+    obj.is_simulator = obj.caps.get('useSimulator', False)
+    obj.is_real_device = not obj.is_simulator
+
+    if obj.is_app:
+        if obj.is_ios:
+            obj.bundle_id = obj.caps.get('bundleId', 'undefined: bundleId')
+        elif obj.is_android:
+            obj.bundle_id = obj.caps.get('appPackage', 'undefined: appPackage')
+        else:
+            raise Exception('Make sure that correct "platformName" capability specified')
```

### Comparing `dyatel-wrapper-2.2.0/dyatel/dyatel_sel/driver/web_driver.py` & `dyatel-wrapper-2.2.1/dyatel/dyatel_sel/driver/web_driver.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
     def __init__(self, driver: SeleniumWebDriver, *args, **kwargs):  # noqa
         """
         Initializing of desktop web driver with selenium
 
         :param driver: selenium driver to initialize
         """
+        self.is_desktop = True
         self.original_tab = driver.current_window_handle
         self.browser_name = driver.caps.get('browserName', None)
 
         CoreDriver.__init__(self, driver=driver)
 
     def set_window_size(self, width: int, height: int) -> CoreDriver:
         """
```

### Comparing `dyatel-wrapper-2.2.0/dyatel/dyatel_sel/elements/mobile_element.py` & `dyatel-wrapper-2.2.1/dyatel/dyatel_sel/elements/mobile_element.py`

 * *Files identical despite different names*

### Comparing `dyatel-wrapper-2.2.0/dyatel/dyatel_sel/elements/web_element.py` & `dyatel-wrapper-2.2.1/dyatel/dyatel_sel/elements/web_element.py`

 * *Files identical despite different names*

### Comparing `dyatel-wrapper-2.2.0/dyatel/dyatel_sel/pages/mobile_page.py` & `dyatel-wrapper-2.2.1/dyatel/dyatel_sel/pages/mobile_page.py`

 * *Files identical despite different names*

### Comparing `dyatel-wrapper-2.2.0/dyatel/exceptions.py` & `dyatel-wrapper-2.2.1/dyatel/exceptions.py`

 * *Files identical despite different names*

### Comparing `dyatel-wrapper-2.2.0/dyatel/js_scripts.py` & `dyatel-wrapper-2.2.1/dyatel/js_scripts.py`

 * *Files identical despite different names*

### Comparing `dyatel-wrapper-2.2.0/dyatel/keyboard_keys.py` & `dyatel-wrapper-2.2.1/dyatel/keyboard_keys.py`

 * *Files identical despite different names*

### Comparing `dyatel-wrapper-2.2.0/dyatel/mixins/driver_mixin.py` & `dyatel-wrapper-2.2.1/dyatel/mixins/driver_mixin.py`

 * *Files identical despite different names*

### Comparing `dyatel-wrapper-2.2.0/dyatel/mixins/internal_mixin.py` & `dyatel-wrapper-2.2.1/dyatel/mixins/internal_mixin.py`

 * *Files identical despite different names*

### Comparing `dyatel-wrapper-2.2.0/dyatel/shared_utils.py` & `dyatel-wrapper-2.2.1/dyatel/shared_utils.py`

 * *Files identical despite different names*

### Comparing `dyatel-wrapper-2.2.0/dyatel/utils/internal_utils.py` & `dyatel-wrapper-2.2.1/dyatel/utils/internal_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -232,22 +232,26 @@
 
     return items
 
 
 def is_target_on_screen(x: int, y: int, possible_range: dict):
     """
     Check is given coordinates fit into given range
+    An safe value will be applied:
+      1 - Due to usage of range
+      2 - Due to rounding a number when get size/location of element
 
     :param x: x coordinate
     :param y: y coordinate
     :param possible_range: possible range
     :return: bool
     """
-    is_x_on_screen = x in range(possible_range['width'] + 1)
-    is_y_on_screen = y in range(possible_range['height'] + 1)
+    safe_value = 2
+    is_x_on_screen = x in range(possible_range['width'] + safe_value)
+    is_y_on_screen = y in range(possible_range['height'] + safe_value)
     return is_x_on_screen and is_y_on_screen
 
 
 def calculate_coordinate_to_click(element: Any, x: int = 0, y: int = 0) -> tuple:
     """
     Calculate coordinates to click for element
     Examples:
```

### Comparing `dyatel-wrapper-2.2.0/dyatel/utils/logs.py` & `dyatel-wrapper-2.2.1/dyatel/utils/logs.py`

 * *Files identical despite different names*

### Comparing `dyatel-wrapper-2.2.0/dyatel/utils/previous_object_driver.py` & `dyatel-wrapper-2.2.1/dyatel/utils/previous_object_driver.py`

 * *Files identical despite different names*

### Comparing `dyatel-wrapper-2.2.0/dyatel/utils/selector_synchronizer.py` & `dyatel-wrapper-2.2.1/dyatel/utils/selector_synchronizer.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
     mobile_fallback_locator = data.get('mobile', locator)
 
     if obj.driver_wrapper.is_android:
         locator = data.get('android', mobile_fallback_locator)
     elif obj.driver_wrapper.is_ios:
         locator = data.get('ios', mobile_fallback_locator)
-    elif obj.driver_wrapper.is_mobile:
+    elif obj.driver_wrapper.is_mobile or obj.driver_wrapper.is_appium:
         locator = mobile_fallback_locator
     elif obj.driver_wrapper.is_desktop:
         locator = data.get('desktop', locator)
 
     return locator
```

### Comparing `dyatel-wrapper-2.2.0/dyatel/visual_comparison.py` & `dyatel-wrapper-2.2.1/dyatel/visual_comparison.py`

 * *Files 1% similar despite different names*

```diff
@@ -412,14 +412,15 @@
             pytest_rerun = importlib.import_module('pytest_rerunfailures')
         except ModuleNotFoundError:
             return None
 
         if hasattr(self.test_item, 'execution_count'):
             self.test_item.execution_count = pytest_rerun.get_reruns_count(self.test_item) + 1
 
-    def _remove_unexpected_underscores(self, text) -> str:
+    @staticmethod
+    def _remove_unexpected_underscores(text) -> str:
         """
         Remove multiple underscores from given text
 
         :return: test_screenshot__data___name -> test_screenshot_data_name
         """
         return re.sub(r'_{2,}', '_', text)
```

### Comparing `dyatel-wrapper-2.2.0/dyatel_wrapper.egg-info/PKG-INFO` & `dyatel-wrapper-2.2.1/dyatel_wrapper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyatel-wrapper
-Version: 2.2.0
+Version: 2.2.1
 Summary: Wrapper of Selenium, Appium and Playwright with single API
 Home-page: https://github.com/EnvInc/dyatel
 Author: Podolian Vladimir
 Author-email: vladimir.podolyan64@gmail.com
 Project-URL: Source, https://github.com/EnvInc/dyatel
 Project-URL: Tracker, https://github.com/EnvInc/dyatel/issues
 Project-URL: Changelog, https://github.com/EnvInc/dyatel/blob/master/CHANGELOG.md
```

### Comparing `dyatel-wrapper-2.2.0/dyatel_wrapper.egg-info/SOURCES.txt` & `dyatel-wrapper-2.2.1/dyatel_wrapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dyatel-wrapper-2.2.0/setup.py` & `dyatel-wrapper-2.2.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 
 cleanup()
 
 
 setup(
     name=pypi_name,
-    version='2.2.0',
+    version='2.2.1',
     url=f'https://github.com/EnvInc/{project_name}',
     packages=get_packages(project_name),
     install_requires=[
         'Appium-Python-Client>=2.1.2',
         'numpy>=1.18.1',
         'opencv-python==4.5.5.62',
         'Pillow>=6.2.2',
```

