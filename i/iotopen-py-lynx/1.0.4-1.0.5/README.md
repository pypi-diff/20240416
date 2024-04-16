# Comparing `tmp/iotopen_py_lynx-1.0.4.tar.gz` & `tmp/iotopen_py_lynx-1.0.5.tar.gz`

## Comparing `iotopen_py_lynx-1.0.4.tar` & `iotopen_py_lynx-1.0.5.tar`

### file list

```diff
@@ -1,46 +1,47 @@
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/.idea/.gitignore
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/.idea/misc.xml
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/.idea/modules.xml
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/.idea/py-lynx.iml
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/.idea/vcs.xml
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/.idea/codeStyles/codeStyleConfig.xml
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/src/lynx/__init__.py
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/src/lynx/api_client.py
--rw-r--r--   0        0        0    17893 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/src/lynx/client.py
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/src/lynx/controller/__init__.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/src/lynx/controller/controller.py
--rw-r--r--   0        0        0     3036 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/src/lynx/controller/device_controller.py
--rw-r--r--   0        0        0     4153 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/src/lynx/controller/edge_app_controller.py
--rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/src/lynx/controller/file_controller.py
--rw-r--r--   0        0        0     3112 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/src/lynx/controller/function_controller.py
--rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/src/lynx/controller/installation_controller.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/src/lynx/controller/installation_info_controller.py
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/src/lynx/controller/log_controller.py
--rw-r--r--   0        0        0     4389 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/src/lynx/controller/notification_controller.py
--rw-r--r--   0        0        0     3265 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/src/lynx/controller/organization_controller.py
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/src/lynx/controller/schedule_controller.py
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/src/lynx/controller/trace_controller.py
--rw-r--r--   0        0        0     2926 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/src/lynx/controller/user_controller.py
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/src/lynx/models/__init__.py
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/src/lynx/models/constants.py
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/src/lynx/models/device.py
--rw-r--r--   0        0        0     6023 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/src/lynx/models/edge_app.py
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/src/lynx/models/file.py
--rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/src/lynx/models/function.py
--rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/src/lynx/models/installation.py
--rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/src/lynx/models/installation_info.py
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/src/lynx/models/log.py
--rw-r--r--   0        0        0     4780 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/src/lynx/models/notification.py
--rw-r--r--   0        0        0     3645 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/src/lynx/models/organization.py
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/src/lynx/models/publisher.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/src/lynx/models/responses.py
--rw-r--r--   0        0        0     3604 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/src/lynx/models/schedule.py
--rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/src/lynx/models/shared.py
--rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/src/lynx/models/trace.py
--rw-r--r--   0        0        0     3749 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/src/lynx/models/user.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/.gitignore
--rw-r--r--   0        0        0    11345 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/LICENSE
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/README.md
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/.idea/.gitignore
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/.idea/misc.xml
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/.idea/modules.xml
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/.idea/py-lynx.iml
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/.idea/vcs.xml
+-rw-r--r--   0        0        0     4233 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/.idea/workspace.xml
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/.idea/codeStyles/codeStyleConfig.xml
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/src/lynx/__init__.py
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/src/lynx/api_client.py
+-rw-r--r--   0        0        0    17893 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/src/lynx/client.py
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/src/lynx/controller/__init__.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/src/lynx/controller/controller.py
+-rw-r--r--   0        0        0     3036 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/src/lynx/controller/device_controller.py
+-rw-r--r--   0        0        0     4153 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/src/lynx/controller/edge_app_controller.py
+-rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/src/lynx/controller/file_controller.py
+-rw-r--r--   0        0        0     3112 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/src/lynx/controller/function_controller.py
+-rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/src/lynx/controller/installation_controller.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/src/lynx/controller/installation_info_controller.py
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/src/lynx/controller/log_controller.py
+-rw-r--r--   0        0        0     4389 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/src/lynx/controller/notification_controller.py
+-rw-r--r--   0        0        0     3265 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/src/lynx/controller/organization_controller.py
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/src/lynx/controller/schedule_controller.py
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/src/lynx/controller/trace_controller.py
+-rw-r--r--   0        0        0     2926 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/src/lynx/controller/user_controller.py
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/src/lynx/models/__init__.py
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/src/lynx/models/constants.py
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/src/lynx/models/device.py
+-rw-r--r--   0        0        0     6016 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/src/lynx/models/edge_app.py
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/src/lynx/models/file.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/src/lynx/models/function.py
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/src/lynx/models/installation.py
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/src/lynx/models/installation_info.py
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/src/lynx/models/log.py
+-rw-r--r--   0        0        0     4780 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/src/lynx/models/notification.py
+-rw-r--r--   0        0        0     3630 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/src/lynx/models/organization.py
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/src/lynx/models/publisher.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/src/lynx/models/responses.py
+-rw-r--r--   0        0        0     3604 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/src/lynx/models/schedule.py
+-rw-r--r--   0        0        0     3013 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/src/lynx/models/shared.py
+-rw-r--r--   0        0        0     2444 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/src/lynx/models/trace.py
+-rw-r--r--   0        0        0     3734 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/src/lynx/models/user.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/.gitignore
+-rw-r--r--   0        0        0    11345 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/LICENSE
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/README.md
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/PKG-INFO
```

### Comparing `iotopen_py_lynx-1.0.4/src/lynx/api_client.py` & `iotopen_py_lynx-1.0.5/src/lynx/api_client.py`

 * *Files identical despite different names*

### Comparing `iotopen_py_lynx-1.0.4/src/lynx/client.py` & `iotopen_py_lynx-1.0.5/src/lynx/client.py`

 * *Files identical despite different names*

### Comparing `iotopen_py_lynx-1.0.4/src/lynx/controller/__init__.py` & `iotopen_py_lynx-1.0.5/src/lynx/controller/__init__.py`

 * *Files identical despite different names*

### Comparing `iotopen_py_lynx-1.0.4/src/lynx/controller/device_controller.py` & `iotopen_py_lynx-1.0.5/src/lynx/controller/device_controller.py`

 * *Files identical despite different names*

### Comparing `iotopen_py_lynx-1.0.4/src/lynx/controller/edge_app_controller.py` & `iotopen_py_lynx-1.0.5/src/lynx/controller/edge_app_controller.py`

 * *Files identical despite different names*

### Comparing `iotopen_py_lynx-1.0.4/src/lynx/controller/file_controller.py` & `iotopen_py_lynx-1.0.5/src/lynx/controller/file_controller.py`

 * *Files identical despite different names*

### Comparing `iotopen_py_lynx-1.0.4/src/lynx/controller/function_controller.py` & `iotopen_py_lynx-1.0.5/src/lynx/controller/function_controller.py`

 * *Files identical despite different names*

### Comparing `iotopen_py_lynx-1.0.4/src/lynx/controller/installation_controller.py` & `iotopen_py_lynx-1.0.5/src/lynx/controller/installation_controller.py`

 * *Files identical despite different names*

### Comparing `iotopen_py_lynx-1.0.4/src/lynx/controller/installation_info_controller.py` & `iotopen_py_lynx-1.0.5/src/lynx/controller/installation_info_controller.py`

 * *Files identical despite different names*

### Comparing `iotopen_py_lynx-1.0.4/src/lynx/controller/log_controller.py` & `iotopen_py_lynx-1.0.5/src/lynx/controller/log_controller.py`

 * *Files identical despite different names*

### Comparing `iotopen_py_lynx-1.0.4/src/lynx/controller/notification_controller.py` & `iotopen_py_lynx-1.0.5/src/lynx/controller/notification_controller.py`

 * *Files identical despite different names*

### Comparing `iotopen_py_lynx-1.0.4/src/lynx/controller/organization_controller.py` & `iotopen_py_lynx-1.0.5/src/lynx/controller/organization_controller.py`

 * *Files identical despite different names*

### Comparing `iotopen_py_lynx-1.0.4/src/lynx/controller/schedule_controller.py` & `iotopen_py_lynx-1.0.5/src/lynx/controller/schedule_controller.py`

 * *Files identical despite different names*

### Comparing `iotopen_py_lynx-1.0.4/src/lynx/controller/trace_controller.py` & `iotopen_py_lynx-1.0.5/src/lynx/controller/trace_controller.py`

 * *Files identical despite different names*

### Comparing `iotopen_py_lynx-1.0.4/src/lynx/controller/user_controller.py` & `iotopen_py_lynx-1.0.5/src/lynx/controller/user_controller.py`

 * *Files identical despite different names*

### Comparing `iotopen_py_lynx-1.0.4/src/lynx/models/__init__.py` & `iotopen_py_lynx-1.0.5/src/lynx/models/__init__.py`

 * *Files identical despite different names*

### Comparing `iotopen_py_lynx-1.0.4/src/lynx/models/constants.py` & `iotopen_py_lynx-1.0.5/src/lynx/models/constants.py`

 * *Files identical despite different names*

### Comparing `iotopen_py_lynx-1.0.4/src/lynx/models/device.py` & `iotopen_py_lynx-1.0.5/src/lynx/models/device.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pprint
 from typing import Optional
 
-from src.lynx.models.shared import Meta, WithMeta
+from .shared import Meta, WithMeta
 
 
 class Device(WithMeta):
     def __init__(self, installation_id: int, type: str, meta: Meta,
                  protected_meta: Optional[Meta] = None,
                  id: Optional[int] = None,
                  created: Optional[int] = None,
```

### Comparing `iotopen_py_lynx-1.0.4/src/lynx/models/edge_app.py` & `iotopen_py_lynx-1.0.5/src/lynx/models/edge_app.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 import pprint
 from typing import Optional, Any, TYPE_CHECKING
 
 if TYPE_CHECKING:
-    from src.lynx import Publisher
+    from . import Publisher
 
 
 class EdgeApp:
     def __init__(self, name: str, category: str, tags: list[str], short_description: str, description: str,
                  source_url: str, public: Optional[bool] = None, id: Optional[int] = None,
                  publisher: Optional[Publisher] = None, official: Optional[bool] = None, created: Optional[int] = None,
                  updated: Optional[int] = None):
```

### Comparing `iotopen_py_lynx-1.0.4/src/lynx/models/file.py` & `iotopen_py_lynx-1.0.5/src/lynx/models/file.py`

 * *Files identical despite different names*

### Comparing `iotopen_py_lynx-1.0.4/src/lynx/models/function.py` & `iotopen_py_lynx-1.0.5/src/lynx/models/function.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pprint
 from typing import Optional
 
-from src.lynx.models.shared import WithMeta, Meta
+from .shared import WithMeta, Meta
 
 
 class Function(WithMeta):
     def __init__(self, installation_id: int, type: str, meta: Meta,
                  protected_meta: Optional[Meta] = None,
                  id: Optional[int] = None,
                  created: Optional[int] = None,
```

### Comparing `iotopen_py_lynx-1.0.4/src/lynx/models/installation.py` & `iotopen_py_lynx-1.0.5/src/lynx/models/installation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pprint
 from typing import Optional
 
-from src.lynx.models.shared import WithMeta, Meta
+from .shared import WithMeta, Meta
 
 
 class Installation(WithMeta):
     def __init__(self, name: str, organization_id: int, notes: str, users: list[int], meta: Meta,
                  id: Optional[int] = None, client_id: Optional[int] = None, protected_meta: Optional[Meta] = None,
                  created: Optional[int] = None):
         super().__init__(meta, protected_meta)
```

### Comparing `iotopen_py_lynx-1.0.4/src/lynx/models/installation_info.py` & `iotopen_py_lynx-1.0.5/src/lynx/models/installation_info.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,8 @@
 import pprint
-from typing import Optional
-
-from src.lynx.models.shared import WithMeta, Meta
 
 
 class InstallationInfo:
     def __init__(self, name: str, organization_id: int, id: int, client_id: int, assigned: bool,
                  capabilities: list[str]):
         self._name = name
         self._organization_id = organization_id
```

### Comparing `iotopen_py_lynx-1.0.4/src/lynx/models/log.py` & `iotopen_py_lynx-1.0.5/src/lynx/models/log.py`

 * *Files identical despite different names*

### Comparing `iotopen_py_lynx-1.0.4/src/lynx/models/notification.py` & `iotopen_py_lynx-1.0.5/src/lynx/models/notification.py`

 * *Files identical despite different names*

### Comparing `iotopen_py_lynx-1.0.4/src/lynx/models/organization.py` & `iotopen_py_lynx-1.0.5/src/lynx/models/organization.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pprint
 from typing import Optional
 
-from src.lynx.models.shared import WithMeta, Meta, Address
+from .shared import WithMeta, Meta, Address
 
 
 class OrganizationChild:
     def __init__(self, id: int, name: str):
         self._id = id
         self._name = name
```

### Comparing `iotopen_py_lynx-1.0.4/src/lynx/models/publisher.py` & `iotopen_py_lynx-1.0.5/src/lynx/models/publisher.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 import pprint
 from typing import Optional, TYPE_CHECKING
 
 if TYPE_CHECKING:
-    from src.lynx import EdgeApp
+    from . import EdgeApp
 
 
 class Publisher:
     def __init__(self, name: str, id: int, apps: Optional[list[EdgeApp]] = None):
         self._name = name
         self._id = id
         self._apps = apps
```

### Comparing `iotopen_py_lynx-1.0.4/src/lynx/models/schedule.py` & `iotopen_py_lynx-1.0.5/src/lynx/models/schedule.py`

 * *Files identical despite different names*

### Comparing `iotopen_py_lynx-1.0.4/src/lynx/models/shared.py` & `iotopen_py_lynx-1.0.5/src/lynx/models/shared.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import pprint
-import urllib.parse
 from typing import Dict, Optional
 
 
 class MetaObject:
     def __init__(self, value: str, protected: Optional[bool] = False):
         self._value = value
         self._protected = protected
```

### Comparing `iotopen_py_lynx-1.0.4/src/lynx/models/trace.py` & `iotopen_py_lynx-1.0.5/src/lynx/models/trace.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pprint
 
-from src.lynx.models import TraceAction, TraceObjectType
+from . import TraceAction, TraceObjectType
 
 
 class TraceEntry:
     def __init__(self, id: str, path: str, method: str, timestamp: float, user_id: int, action: TraceAction,
                  object_type: TraceObjectType, object_id: int, description: str):
         self._id = id
         self._path = path
```

### Comparing `iotopen_py_lynx-1.0.4/src/lynx/models/user.py` & `iotopen_py_lynx-1.0.5/src/lynx/models/user.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pprint
 from typing import Optional
 
-from src.lynx.models.shared import WithMeta, Meta, Address
+from .shared import WithMeta, Meta, Address
 
 
 class User(WithMeta):
     def __init__(self, email: str, first_name: str, last_name: str, role: int, sms_login: bool, address: Address,
                  note: str, mobile: str, organisations: list[int], meta: Meta, assigned_installations: list[int],
                  expire_at: int, protected_meta: Optional[Meta] = None, id: Optional[int] = None):
         super().__init__(meta, protected_meta)
```

### Comparing `iotopen_py_lynx-1.0.4/LICENSE` & `iotopen_py_lynx-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `iotopen_py_lynx-1.0.4/README.md` & `iotopen_py_lynx-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `iotopen_py_lynx-1.0.4/pyproject.toml` & `iotopen_py_lynx-1.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/lynx"]
 
 [project]
 name = "iotopen-py-lynx"
-version = "1.0.4"
+version = "1.0.5"
 authors = [
     { name = "Jesper Falk", email = "jesper.falk@iotopen.se" },
 ]
 description = "A wrapper library for the IoT Open Lynx API"
 readme = "README.md"
 requires-python = ">3.8"
 classifiers = [
```

### Comparing `iotopen_py_lynx-1.0.4/PKG-INFO` & `iotopen_py_lynx-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: iotopen-py-lynx
-Version: 1.0.4
+Version: 1.0.5
 Summary: A wrapper library for the IoT Open Lynx API
 Project-URL: Homepage, https://github.com/IoTOpen/py-lynx
 Project-URL: Issues, https://github.com/IoTOpen/py-lynx/issues
 Author-email: Jesper Falk <jesper.falk@iotopen.se>
 License-File: LICENSE
 Keywords: api,iot,iot-open
 Classifier: Intended Audience :: Developers
```

