# Comparing `tmp/iotopen_py_lynx-1.0.3.tar.gz` & `tmp/iotopen_py_lynx-1.0.4.tar.gz`

## Comparing `iotopen_py_lynx-1.0.3.tar` & `iotopen_py_lynx-1.0.4.tar`

### file list

```diff
@@ -1,47 +1,46 @@
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.3/.idea/.gitignore
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.3/.idea/misc.xml
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.3/.idea/modules.xml
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.3/.idea/py-lynx.iml
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.3/.idea/vcs.xml
--rw-r--r--   0        0        0     7223 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.3/.idea/workspace.xml
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.3/.idea/codeStyles/codeStyleConfig.xml
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.3/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.3/src/iotopen-py-lynx/__init__.py
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.3/src/iotopen-py-lynx/api_client.py
--rw-r--r--   0        0        0    17893 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.3/src/iotopen-py-lynx/client.py
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.3/src/iotopen-py-lynx/controller/__init__.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.3/src/iotopen-py-lynx/controller/controller.py
--rw-r--r--   0        0        0     3036 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.3/src/iotopen-py-lynx/controller/device_controller.py
--rw-r--r--   0        0        0     4153 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.3/src/iotopen-py-lynx/controller/edge_app_controller.py
--rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.3/src/iotopen-py-lynx/controller/file_controller.py
--rw-r--r--   0        0        0     3112 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.3/src/iotopen-py-lynx/controller/function_controller.py
--rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.3/src/iotopen-py-lynx/controller/installation_controller.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.3/src/iotopen-py-lynx/controller/installation_info_controller.py
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.3/src/iotopen-py-lynx/controller/log_controller.py
--rw-r--r--   0        0        0     4389 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.3/src/iotopen-py-lynx/controller/notification_controller.py
--rw-r--r--   0        0        0     3265 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.3/src/iotopen-py-lynx/controller/organization_controller.py
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.3/src/iotopen-py-lynx/controller/schedule_controller.py
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.3/src/iotopen-py-lynx/controller/trace_controller.py
--rw-r--r--   0        0        0     2926 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.3/src/iotopen-py-lynx/controller/user_controller.py
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.3/src/iotopen-py-lynx/models/__init__.py
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.3/src/iotopen-py-lynx/models/constants.py
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.3/src/iotopen-py-lynx/models/device.py
--rw-r--r--   0        0        0     6023 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.3/src/iotopen-py-lynx/models/edge_app.py
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.3/src/iotopen-py-lynx/models/file.py
--rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.3/src/iotopen-py-lynx/models/function.py
--rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.3/src/iotopen-py-lynx/models/installation.py
--rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.3/src/iotopen-py-lynx/models/installation_info.py
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.3/src/iotopen-py-lynx/models/log.py
--rw-r--r--   0        0        0     4780 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.3/src/iotopen-py-lynx/models/notification.py
--rw-r--r--   0        0        0     3645 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.3/src/iotopen-py-lynx/models/organization.py
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.3/src/iotopen-py-lynx/models/publisher.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.3/src/iotopen-py-lynx/models/responses.py
--rw-r--r--   0        0        0     3604 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.3/src/iotopen-py-lynx/models/schedule.py
--rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.3/src/iotopen-py-lynx/models/shared.py
--rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.3/src/iotopen-py-lynx/models/trace.py
--rw-r--r--   0        0        0     3749 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.3/src/iotopen-py-lynx/models/user.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.3/.gitignore
--rw-r--r--   0        0        0    11345 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.3/LICENSE
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.3/README.md
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/.idea/.gitignore
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/.idea/misc.xml
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/.idea/modules.xml
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/.idea/py-lynx.iml
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/.idea/vcs.xml
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/.idea/codeStyles/codeStyleConfig.xml
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/src/lynx/__init__.py
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/src/lynx/api_client.py
+-rw-r--r--   0        0        0    17893 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/src/lynx/client.py
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/src/lynx/controller/__init__.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/src/lynx/controller/controller.py
+-rw-r--r--   0        0        0     3036 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/src/lynx/controller/device_controller.py
+-rw-r--r--   0        0        0     4153 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/src/lynx/controller/edge_app_controller.py
+-rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/src/lynx/controller/file_controller.py
+-rw-r--r--   0        0        0     3112 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/src/lynx/controller/function_controller.py
+-rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/src/lynx/controller/installation_controller.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/src/lynx/controller/installation_info_controller.py
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/src/lynx/controller/log_controller.py
+-rw-r--r--   0        0        0     4389 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/src/lynx/controller/notification_controller.py
+-rw-r--r--   0        0        0     3265 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/src/lynx/controller/organization_controller.py
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/src/lynx/controller/schedule_controller.py
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/src/lynx/controller/trace_controller.py
+-rw-r--r--   0        0        0     2926 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/src/lynx/controller/user_controller.py
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/src/lynx/models/__init__.py
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/src/lynx/models/constants.py
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/src/lynx/models/device.py
+-rw-r--r--   0        0        0     6023 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/src/lynx/models/edge_app.py
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/src/lynx/models/file.py
+-rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/src/lynx/models/function.py
+-rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/src/lynx/models/installation.py
+-rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/src/lynx/models/installation_info.py
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/src/lynx/models/log.py
+-rw-r--r--   0        0        0     4780 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/src/lynx/models/notification.py
+-rw-r--r--   0        0        0     3645 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/src/lynx/models/organization.py
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/src/lynx/models/publisher.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/src/lynx/models/responses.py
+-rw-r--r--   0        0        0     3604 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/src/lynx/models/schedule.py
+-rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/src/lynx/models/shared.py
+-rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/src/lynx/models/trace.py
+-rw-r--r--   0        0        0     3749 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/src/lynx/models/user.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/.gitignore
+-rw-r--r--   0        0        0    11345 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/LICENSE
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/README.md
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/PKG-INFO
```

### Comparing `iotopen_py_lynx-1.0.3/src/iotopen-py-lynx/api_client.py` & `iotopen_py_lynx-1.0.4/src/lynx/api_client.py`

 * *Files identical despite different names*

### Comparing `iotopen_py_lynx-1.0.3/src/iotopen-py-lynx/client.py` & `iotopen_py_lynx-1.0.4/src/lynx/client.py`

 * *Files identical despite different names*

### Comparing `iotopen_py_lynx-1.0.3/src/iotopen-py-lynx/controller/__init__.py` & `iotopen_py_lynx-1.0.4/src/lynx/controller/__init__.py`

 * *Files identical despite different names*

### Comparing `iotopen_py_lynx-1.0.3/src/iotopen-py-lynx/controller/device_controller.py` & `iotopen_py_lynx-1.0.4/src/lynx/controller/device_controller.py`

 * *Files identical despite different names*

### Comparing `iotopen_py_lynx-1.0.3/src/iotopen-py-lynx/controller/edge_app_controller.py` & `iotopen_py_lynx-1.0.4/src/lynx/controller/edge_app_controller.py`

 * *Files identical despite different names*

### Comparing `iotopen_py_lynx-1.0.3/src/iotopen-py-lynx/controller/file_controller.py` & `iotopen_py_lynx-1.0.4/src/lynx/controller/file_controller.py`

 * *Files identical despite different names*

### Comparing `iotopen_py_lynx-1.0.3/src/iotopen-py-lynx/controller/function_controller.py` & `iotopen_py_lynx-1.0.4/src/lynx/controller/function_controller.py`

 * *Files identical despite different names*

### Comparing `iotopen_py_lynx-1.0.3/src/iotopen-py-lynx/controller/installation_controller.py` & `iotopen_py_lynx-1.0.4/src/lynx/controller/installation_controller.py`

 * *Files identical despite different names*

### Comparing `iotopen_py_lynx-1.0.3/src/iotopen-py-lynx/controller/installation_info_controller.py` & `iotopen_py_lynx-1.0.4/src/lynx/controller/installation_info_controller.py`

 * *Files identical despite different names*

### Comparing `iotopen_py_lynx-1.0.3/src/iotopen-py-lynx/controller/log_controller.py` & `iotopen_py_lynx-1.0.4/src/lynx/controller/log_controller.py`

 * *Files identical despite different names*

### Comparing `iotopen_py_lynx-1.0.3/src/iotopen-py-lynx/controller/notification_controller.py` & `iotopen_py_lynx-1.0.4/src/lynx/controller/notification_controller.py`

 * *Files identical despite different names*

### Comparing `iotopen_py_lynx-1.0.3/src/iotopen-py-lynx/controller/organization_controller.py` & `iotopen_py_lynx-1.0.4/src/lynx/controller/organization_controller.py`

 * *Files identical despite different names*

### Comparing `iotopen_py_lynx-1.0.3/src/iotopen-py-lynx/controller/schedule_controller.py` & `iotopen_py_lynx-1.0.4/src/lynx/controller/schedule_controller.py`

 * *Files identical despite different names*

### Comparing `iotopen_py_lynx-1.0.3/src/iotopen-py-lynx/controller/trace_controller.py` & `iotopen_py_lynx-1.0.4/src/lynx/controller/trace_controller.py`

 * *Files identical despite different names*

### Comparing `iotopen_py_lynx-1.0.3/src/iotopen-py-lynx/controller/user_controller.py` & `iotopen_py_lynx-1.0.4/src/lynx/controller/user_controller.py`

 * *Files identical despite different names*

### Comparing `iotopen_py_lynx-1.0.3/src/iotopen-py-lynx/models/__init__.py` & `iotopen_py_lynx-1.0.4/src/lynx/models/__init__.py`

 * *Files identical despite different names*

### Comparing `iotopen_py_lynx-1.0.3/src/iotopen-py-lynx/models/constants.py` & `iotopen_py_lynx-1.0.4/src/lynx/models/constants.py`

 * *Files identical despite different names*

### Comparing `iotopen_py_lynx-1.0.3/src/iotopen-py-lynx/models/device.py` & `iotopen_py_lynx-1.0.4/src/lynx/models/device.py`

 * *Files identical despite different names*

### Comparing `iotopen_py_lynx-1.0.3/src/iotopen-py-lynx/models/edge_app.py` & `iotopen_py_lynx-1.0.4/src/lynx/models/edge_app.py`

 * *Files identical despite different names*

### Comparing `iotopen_py_lynx-1.0.3/src/iotopen-py-lynx/models/file.py` & `iotopen_py_lynx-1.0.4/src/lynx/models/file.py`

 * *Files identical despite different names*

### Comparing `iotopen_py_lynx-1.0.3/src/iotopen-py-lynx/models/function.py` & `iotopen_py_lynx-1.0.4/src/lynx/models/function.py`

 * *Files identical despite different names*

### Comparing `iotopen_py_lynx-1.0.3/src/iotopen-py-lynx/models/installation.py` & `iotopen_py_lynx-1.0.4/src/lynx/models/installation.py`

 * *Files identical despite different names*

### Comparing `iotopen_py_lynx-1.0.3/src/iotopen-py-lynx/models/installation_info.py` & `iotopen_py_lynx-1.0.4/src/lynx/models/installation_info.py`

 * *Files identical despite different names*

### Comparing `iotopen_py_lynx-1.0.3/src/iotopen-py-lynx/models/log.py` & `iotopen_py_lynx-1.0.4/src/lynx/models/log.py`

 * *Files identical despite different names*

### Comparing `iotopen_py_lynx-1.0.3/src/iotopen-py-lynx/models/notification.py` & `iotopen_py_lynx-1.0.4/src/lynx/models/notification.py`

 * *Files identical despite different names*

### Comparing `iotopen_py_lynx-1.0.3/src/iotopen-py-lynx/models/organization.py` & `iotopen_py_lynx-1.0.4/src/lynx/models/organization.py`

 * *Files identical despite different names*

### Comparing `iotopen_py_lynx-1.0.3/src/iotopen-py-lynx/models/publisher.py` & `iotopen_py_lynx-1.0.4/src/lynx/models/publisher.py`

 * *Files identical despite different names*

### Comparing `iotopen_py_lynx-1.0.3/src/iotopen-py-lynx/models/schedule.py` & `iotopen_py_lynx-1.0.4/src/lynx/models/schedule.py`

 * *Files identical despite different names*

### Comparing `iotopen_py_lynx-1.0.3/src/iotopen-py-lynx/models/shared.py` & `iotopen_py_lynx-1.0.4/src/lynx/models/shared.py`

 * *Files identical despite different names*

### Comparing `iotopen_py_lynx-1.0.3/src/iotopen-py-lynx/models/trace.py` & `iotopen_py_lynx-1.0.4/src/lynx/models/trace.py`

 * *Files identical despite different names*

### Comparing `iotopen_py_lynx-1.0.3/src/iotopen-py-lynx/models/user.py` & `iotopen_py_lynx-1.0.4/src/lynx/models/user.py`

 * *Files identical despite different names*

### Comparing `iotopen_py_lynx-1.0.3/LICENSE` & `iotopen_py_lynx-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `iotopen_py_lynx-1.0.3/README.md` & `iotopen_py_lynx-1.0.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 ```
 
 ## Usage
 
 Create a Lynx client and use the functions on it to make API-calls.
 
 ```python
-from iotopen-py-lynx import Client
+from lynx import Client
 
 cli = Client("https://lynx.iotopen.se", "abcdef123456789abcdef123456789")
 
 installations = cli.get_installations()
 print(installations)
 ```
 
-[0]: https://iotopen.io/developers
+[0]: https://iotopen.io/developers
```

### Comparing `iotopen_py_lynx-1.0.3/pyproject.toml` & `iotopen_py_lynx-1.0.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
-packages = ["src/iotopen-py-lynx"]
+packages = ["src/lynx"]
 
 [project]
 name = "iotopen-py-lynx"
-version = "1.0.3"
+version = "1.0.4"
 authors = [
     { name = "Jesper Falk", email = "jesper.falk@iotopen.se" },
 ]
 description = "A wrapper library for the IoT Open Lynx API"
 readme = "README.md"
 requires-python = ">3.8"
 classifiers = [
```

### Comparing `iotopen_py_lynx-1.0.3/PKG-INFO` & `iotopen_py_lynx-1.0.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: iotopen-py-lynx
-Version: 1.0.3
+Version: 1.0.4
 Summary: A wrapper library for the IoT Open Lynx API
 Project-URL: Homepage, https://github.com/IoTOpen/py-lynx
 Project-URL: Issues, https://github.com/IoTOpen/py-lynx/issues
 Author-email: Jesper Falk <jesper.falk@iotopen.se>
 License-File: LICENSE
 Keywords: api,iot,iot-open
 Classifier: Intended Audience :: Developers
@@ -29,16 +29,16 @@
 ```
 
 ## Usage
 
 Create a Lynx client and use the functions on it to make API-calls.
 
 ```python
-from iotopen-py-lynx import Client
+from lynx import Client
 
 cli = Client("https://lynx.iotopen.se", "abcdef123456789abcdef123456789")
 
 installations = cli.get_installations()
 print(installations)
 ```
 
-[0]: https://iotopen.io/developers
+[0]: https://iotopen.io/developers
```

