# Comparing `tmp/maxwell_utils-0.6.4.tar.gz` & `tmp/maxwell_utils-0.6.5.tar.gz`

## Comparing `maxwell_utils-0.6.4.tar` & `maxwell_utils-0.6.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 maxwell_utils-0.6.4/.git
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 maxwell_utils-0.6.4/Makefile
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 maxwell_utils-0.6.4/requirements.txt
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 maxwell_utils-0.6.4/setup.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 maxwell_utils-0.6.4/maxwell/__init__.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 maxwell_utils-0.6.4/maxwell/utils/__init__.py
--rw-r--r--   0        0        0    14173 2020-02-02 00:00:00.000000 maxwell_utils-0.6.4/maxwell/utils/connection.py
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 maxwell_utils-0.6.4/maxwell/utils/listenable.py
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 maxwell_utils-0.6.4/maxwell/utils/logger.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 maxwell_utils-0.6.4/test/__init__.py
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 maxwell_utils-0.6.4/test/test_connection.py
--rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 maxwell_utils-0.6.4/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 maxwell_utils-0.6.4/LICENSE
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 maxwell_utils-0.6.4/README.md
--rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 maxwell_utils-0.6.4/pyproject.toml
--rw-r--r--   0        0        0    13789 2020-02-02 00:00:00.000000 maxwell_utils-0.6.4/PKG-INFO
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 maxwell_utils-0.6.5/.git
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 maxwell_utils-0.6.5/Makefile
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 maxwell_utils-0.6.5/requirements.txt
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 maxwell_utils-0.6.5/setup.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 maxwell_utils-0.6.5/maxwell/__init__.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 maxwell_utils-0.6.5/maxwell/utils/__init__.py
+-rw-r--r--   0        0        0    14185 2020-02-02 00:00:00.000000 maxwell_utils-0.6.5/maxwell/utils/connection.py
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 maxwell_utils-0.6.5/maxwell/utils/listenable.py
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 maxwell_utils-0.6.5/maxwell/utils/logger.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 maxwell_utils-0.6.5/test/__init__.py
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 maxwell_utils-0.6.5/test/test_connection.py
+-rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 maxwell_utils-0.6.5/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 maxwell_utils-0.6.5/LICENSE
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 maxwell_utils-0.6.5/README.md
+-rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 maxwell_utils-0.6.5/pyproject.toml
+-rw-r--r--   0        0        0    13789 2020-02-02 00:00:00.000000 maxwell_utils-0.6.5/PKG-INFO
```

### Comparing `maxwell_utils-0.6.4/Makefile` & `maxwell_utils-0.6.5/Makefile`

 * *Files identical despite different names*

### Comparing `maxwell_utils-0.6.4/maxwell/utils/connection.py` & `maxwell_utils-0.6.5/maxwell/utils/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import asyncio
 import enum
-import websockets
 from abc import ABC, abstractmethod
-from typing import Callable
-import maxwell.protocol.maxwell_protocol_pb2 as protocol_types
+from typing import Callable, Awaitable
+
 import maxwell.protocol.maxwell_protocol as protocol
+import maxwell.protocol.maxwell_protocol_pb2 as protocol_types
+import websockets
+
 from .listenable import Listenable
 from .logger import get_logger
 
 logger = get_logger(__name__)
 
 
 class Event(enum.Enum):
@@ -320,28 +322,28 @@
 
 class MultiAltEndpointsConnection(AbstractConnection):
     # ===========================================
     # apis
     # ===========================================
     def __init__(
         self,
-        pick_endpoint: Callable[[], str],
+        pick_endpoint: Callable[[], Awaitable[str]],
         options={},
         event_handler=None,
         loop=None,
     ):
         super().__init__()
 
         self.__pick_endpoint = pick_endpoint
         self.__options = self._build_options(options)
         self.__event_handler = event_handler if event_handler else EventHandler()
         self.__loop = loop if loop else asyncio.get_event_loop()
 
         self.__should_run = True
-        self.__connection: Connection = None
+        self.__connection = None
         self.__open_event = asyncio.Event()
         self.__connect_task = None
 
         self.__toggle_to_close()
         self.__add_connect_task()
 
     async def close(self):
```

### Comparing `maxwell_utils-0.6.4/maxwell/utils/listenable.py` & `maxwell_utils-0.6.5/maxwell/utils/listenable.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 
 class Listenable(object):
     def __init__(self):
         self.__listeners = collections.OrderedDict()
 
     def add_listener(self, event, callback):
         callbacks = self.__listeners.get(event)
-        if callbacks == None:
+        if callbacks is None:
             callbacks = []
             self.__listeners[event] = callbacks
         callbacks.append(callback)
 
     def delete_listener(self, event, callback):
         callbacks = self.__listeners.get(event)
-        if callbacks == None:
+        if callbacks is None:
             return
         try:
             callbacks.remove(callback)
         except Exception:
             pass
 
     def notify(self, event, *argv, **kwargs):
```

### Comparing `maxwell_utils-0.6.4/maxwell/utils/logger.py` & `maxwell_utils-0.6.5/maxwell/utils/logger.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,28 @@
-import os
 import json
 import logging
 import logging.config
+import os
 from distutils.sysconfig import get_python_lib
 
 inited = False
 
 
+def __get_root_dir():
+    """Get the root directory of the project."""
+    root_dir = os.environ.get("APP_ROOT_DIR")
+    if root_dir:
+        return root_dir
+    return os.path.abspath(os.path.join(get_python_lib(), "..", "..", "..", ".."))
+
+
 def __init(
     default_path="logging.json", default_level=logging.INFO, env_var_key="LOG_CFG_FILE"
 ):
-    root_dir = os.path.abspath(os.path.join(get_python_lib(), "..", "..", "..", ".."))
+    root_dir = __get_root_dir()
 
     specified_config_path = os.getenv(env_var_key, None)
     if specified_config_path:
         config_path = specified_config_path
     else:
         config_path = os.path.join(root_dir, "config", default_path)
```

### Comparing `maxwell_utils-0.6.4/test/test_connection.py` & `maxwell_utils-0.6.5/test/test_connection.py`

 * *Files identical despite different names*

### Comparing `maxwell_utils-0.6.4/.gitignore` & `maxwell_utils-0.6.5/.gitignore`

 * *Files 7% similar despite different names*

```diff
@@ -153,10 +153,10 @@
 cython_debug/
 
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
-#.idea/
+.idea/
 
 log
```

### Comparing `maxwell_utils-0.6.4/LICENSE` & `maxwell_utils-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `maxwell_utils-0.6.4/pyproject.toml` & `maxwell_utils-0.6.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
   "maxwell-protocol == 0.7.3",
 ]
 description = "The maxwell utils implementation for python."
 license = {file = "LICENSE"}
 name = "maxwell-utils"
 readme = "README.md"
 requires-python = ">=3.7"
-version = "0.6.4"
+version = "0.6.5"
 
 [project.optional-dependencies]
 test = ["pytest >= 8.1.1", "pytest-asyncio >= 0.23.6", "pytest-cov >= 4.1.0"]
 
 [project.urls]
 changelog = "https://github.com/maxwell-dev/maxwell-utils-python/CHANGELOG.md"
 repository = "https://github.com/maxwell-dev/maxwell-utils-python"
```

### Comparing `maxwell_utils-0.6.4/PKG-INFO` & `maxwell_utils-0.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: maxwell-utils
-Version: 0.6.4
+Version: 0.6.5
 Summary: The maxwell utils implementation for python.
 Project-URL: changelog, https://github.com/maxwell-dev/maxwell-utils-python/CHANGELOG.md
 Project-URL: repository, https://github.com/maxwell-dev/maxwell-utils-python
 Author-email: Xu Chaoqian <chaoranxu@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

