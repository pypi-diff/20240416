# Comparing `tmp/social_interaction_cloud-1.2.5.tar.gz` & `tmp/social_interaction_cloud-1.2.6.tar.gz`

## Comparing `social_interaction_cloud-1.2.5.tar` & `social_interaction_cloud-1.2.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.5/src/social_interaction_cloud/__init__.py
--rw-r--r--   0        0        0    41602 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.5/src/social_interaction_cloud/abstract_connector.py
--rw-r--r--   0        0        0    45630 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.5/src/social_interaction_cloud/basic_connector.py
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.5/src/social_interaction_cloud/choregraphe_to_json.py
--rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.5/src/social_interaction_cloud/detection_result_pb2.py
--rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.5/src/social_interaction_cloud/tracking_result_pb2.py
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.5/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.5/LICENSE
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.5/README.md
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.5/pyproject.toml
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.5/PKG-INFO
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.6/src/social_interaction_cloud/__init__.py
+-rw-r--r--   0        0        0    42012 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.6/src/social_interaction_cloud/abstract_connector.py
+-rw-r--r--   0        0        0    46358 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.6/src/social_interaction_cloud/basic_connector.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.6/src/social_interaction_cloud/choregraphe_to_json.py
+-rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.6/src/social_interaction_cloud/detection_result_pb2.py
+-rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.6/src/social_interaction_cloud/tracking_result_pb2.py
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.6/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.6/LICENSE
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.6/README.md
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.6/pyproject.toml
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.6/PKG-INFO
```

### Comparing `social_interaction_cloud-1.2.5/src/social_interaction_cloud/abstract_connector.py` & `social_interaction_cloud-1.2.6/src/social_interaction_cloud/abstract_connector.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,14 +54,15 @@
                                          'action_play_motion', 'action_record_motion',  # 'action_motion_file',
                                          'action_led_color', 'action_led_animation',
                                          'memory_create_interactant', 'memory_set_session',
                                          'memory_set_entry', 'memory_get_entry', 'memory_delete_entry',
                                          'memory_get_entries', 'memory_delete_entries',
                                          'memory_get_all_entries',
                                          'memory_set_interactant_data', 'memory_get_interactant_data',
+                                         'memory_delete_interactant_data',
                                          'memory_get_interactant_data_all', 'memory_get_all_interactants',
                                          'memory_set_interactant', 'memory_set_dialog_history',
                                          'memory_get_dialog_history_all',
                                          'memory_delete_interactant', 'memory_delete_all_interactants',
                                          'memory_get_move_history', 'memory_set_move_history',
                                          'memory_get_topics_of_interest', 'memory_set_topics_of_interest',
                                          'llm_openai_prompt'],
@@ -640,20 +641,26 @@
 
     def delete_memory_entries(self, interactant_id: str, entry_type: str):
         self.__send('memory_delete_entries', f'{interactant_id};{entry_type}')
 
     def get_all_memory_entries(self, entry_type: str):
         self.__send('memory_get_all_entries', entry_type)
 
-    def set_interactant_data(self, interactant_id: str, key: str, value: str):
-        self.__send('memory_set_interactant_data', f'{interactant_id};{key};{value}')
+    def set_interactant_data(self, interactant_id: str, key: str = '', value: str = '', keyvalues: dict = None):
+        if keyvalues:
+            self.__send('memory_set_interactant_data', f'{interactant_id};{dumps(keyvalues)}')
+        elif key and value:
+            self.__send('memory_set_interactant_data', f'{interactant_id};{key};{value}')
 
     def get_interactant_data(self, interactant_id: str, key: str):
         self.__send('memory_get_interactant_data', f'{interactant_id};{key}')
 
+    def delete_interactant_data(self, interactant_id: str, key: str):
+        self.__send('memory_delete_interactant_data', f'{interactant_id};{key}')
+
     def get_interactant_data_all(self, interactant_id: str):
         self.__send('memory_get_interactant_data_all', interactant_id)
 
     def get_all_interactants(self):
         self.__send('memory_get_all_interactants', '')
 
     def set_interactant(self, interactant_id: str, data: dict):
```

### Comparing `social_interaction_cloud-1.2.5/src/social_interaction_cloud/basic_connector.py` & `social_interaction_cloud-1.2.6/src/social_interaction_cloud/basic_connector.py`

 * *Files 2% similar despite different names*

```diff
@@ -707,24 +707,34 @@
                               callback=callback, event='EntriesDeleted', sync=sync, load=load)
 
     def get_all_memory_entries(self, entry_type: str, callback: callable = None, sync: bool = True, load: bool = False):
         self.__process_action(super(BasicSICConnector, self).get_all_memory_entries, entry_type,
                               callback=callback, event=f'AllEntries_{entry_type}', sync=sync, load=load,
                               listener_type=ListenerType.MEMORY)
 
-    def set_interactant_data(self, interactant_id: str, key: str, value: str, callback: callable = None,
-                             sync: bool = True, load: bool = False):
-        self.__process_action(super(BasicSICConnector, self).set_interactant_data, interactant_id, key, value,
-                              callback=callback, event='InteractantDataSet', sync=sync, load=load)
+    def set_interactant_data(self, interactant_id: str, key: str = '', value: str = '', keyvalues: dict = None,
+                             callback: callable = None, sync: bool = True, load: bool = False):
+        if keyvalues:
+            self.__process_action(super(BasicSICConnector, self).set_interactant_data, interactant_id,
+                                  keyvalues=keyvalues,
+                                  callback=callback, event='InteractantDataSet', sync=sync, load=load)
+        elif key and value:
+            self.__process_action(super(BasicSICConnector, self).set_interactant_data, interactant_id, key, value,
+                                  callback=callback, event='InteractantDataSet', sync=sync, load=load)
 
     def get_interactant_data(self, interactant_id: str, key: str, callback: callable = None,
                              sync: bool = True, load: bool = False):
         self.__process_action(super(BasicSICConnector, self).get_interactant_data, interactant_id, key,
                               callback=callback, event=key, sync=sync, load=load, listener_type=ListenerType.MEMORY)
 
+    def delete_interactant_data(self, interactant_id: str, key: str, callback: callable = None,
+                             sync: bool = True, load: bool = False):
+        self.__process_action(super(BasicSICConnector, self).delete_interactant_data, interactant_id, key,
+                              callback=callback, event='InteractantDataDeleted', sync=sync, load=load)
+
     def get_interactant_data_all(self, interactant_id: str, callback: callable = None,
                                  sync: bool = True, load: bool = False):
         self.__process_action(super(BasicSICConnector, self).get_interactant_data_all, interactant_id,
                               callback=callback, event=f'InteractantData_{interactant_id}', sync=sync, load=load,
                               listener_type=ListenerType.MEMORY)
 
     def get_all_interactants(self, callback: callable = None, sync: bool = True, load: bool = False):
@@ -783,15 +793,14 @@
 
     def llm_openai_prompt(self, params: dict,
                           callback: callable = None, sync: bool = True, load: bool = False) -> None:
         self.__process_action(super(BasicSICConnector, self).llm_openai_prompt, params,
                               callback=callback, event=params['prompt_id'], sync=sync, load=load,
                               listener_type=ListenerType.LLM)
 
-
     ###########################
     # Listeners Management  #
     ###########################
     def __register_action_listener(self, event: str, callback: callable) -> None:
         self.__action_listeners[event] = callback
 
     def __unregister_action_listener(self, event: str) -> None:
```

### Comparing `social_interaction_cloud-1.2.5/src/social_interaction_cloud/choregraphe_to_json.py` & `social_interaction_cloud-1.2.6/src/social_interaction_cloud/choregraphe_to_json.py`

 * *Files identical despite different names*

### Comparing `social_interaction_cloud-1.2.5/src/social_interaction_cloud/detection_result_pb2.py` & `social_interaction_cloud-1.2.6/src/social_interaction_cloud/detection_result_pb2.py`

 * *Files identical despite different names*

### Comparing `social_interaction_cloud-1.2.5/src/social_interaction_cloud/tracking_result_pb2.py` & `social_interaction_cloud-1.2.6/src/social_interaction_cloud/tracking_result_pb2.py`

 * *Files identical despite different names*

### Comparing `social_interaction_cloud-1.2.5/LICENSE` & `social_interaction_cloud-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `social_interaction_cloud-1.2.5/pyproject.toml` & `social_interaction_cloud-1.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "social_interaction_cloud"
-version = "1.2.5"
+version = "1.2.6"
 authors = [
   { name="Mike Ligthart", email="m.e.u.ligthart@vu.nl" },
 ]
 description = "Connector to the Social Interaction Cloud"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `social_interaction_cloud-1.2.5/PKG-INFO` & `social_interaction_cloud-1.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: social_interaction_cloud
-Version: 1.2.5
+Version: 1.2.6
 Summary: Connector to the Social Interaction Cloud
 Project-URL: Source, https://bitbucket.org/socialroboticshub/connectors/src/master/python/sic/
 Project-URL: Wiki, https://socialrobotics.atlassian.net/wiki/spaces/CBSR/overview
 Author-email: Mike Ligthart <m.e.u.ligthart@vu.nl>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

