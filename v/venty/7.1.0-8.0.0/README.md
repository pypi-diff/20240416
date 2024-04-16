# Comparing `tmp/venty-7.1.0.tar.gz` & `tmp/venty-8.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "venty-7.1.0.tar", last modified: Sat Apr 13 20:58:53 2024, max compression
+gzip compressed data, was "venty-8.0.0.tar", last modified: Tue Apr 16 20:20:53 2024, max compression
```

## Comparing `venty-7.1.0.tar` & `venty-8.0.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxrwx   0        0        0        0 2024-04-13 20:58:53.252396 venty-7.1.0/
--rw-rw-rw-   0        0        0    11558 2022-08-05 14:38:16.000000 venty-7.1.0/LICENSE
--rw-rw-rw-   0        0        0      167 2024-03-15 16:24:05.000000 venty-7.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2189 2024-04-13 20:58:53.251354 venty-7.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1127 2024-04-08 17:56:19.000000 venty-7.1.0/README.md
--rw-rw-rw-   0        0        0       47 2024-03-26 20:12:48.000000 venty-7.1.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-04-13 20:58:53.252396 venty-7.1.0/setup.cfg
--rw-rw-rw-   0        0        0     2017 2024-04-12 14:26:40.000000 venty-7.1.0/setup.py
--rw-rw-rw-   0        0        0      159 2024-03-16 16:56:05.000000 venty-7.1.0/test_requirements.txt
--rw-rw-rw-   0        0        0      665 2024-03-27 06:50:13.000000 venty-7.1.0/tox.ini
-drwxrwxrwx   0        0        0        0 2024-04-13 20:58:53.238346 venty-7.1.0/venty/
--rw-rw-rw-   0        0        0      257 2024-03-16 01:45:41.000000 venty-7.1.0/venty/__init__.py
--rw-rw-rw-   0        0        0      245 2024-03-15 20:16:30.000000 venty-7.1.0/venty/_dummy.py
--rw-rw-rw-   0        0        0      439 2024-04-12 14:47:07.000000 venty-7.1.0/venty/aggregate_channel.py
--rw-rw-rw-   0        0        0     1858 2024-04-08 17:52:38.000000 venty-7.1.0/venty/aggregate_root.py
--rw-rw-rw-   0        0        0     1390 2024-04-13 12:03:00.000000 venty-7.1.0/venty/aggregate_store.py
--rw-rw-rw-   0        0        0     2084 2024-04-12 14:22:50.000000 venty-7.1.0/venty/aggregate_store_test.py
--rw-rw-rw-   0        0        0      999 2024-04-12 13:16:52.000000 venty-7.1.0/venty/auth_event_producer.py
--rw-rw-rw-   0        0        0      886 2024-04-13 10:07:54.000000 venty-7.1.0/venty/classification.py
--rw-rw-rw-   0        0        0     1478 2024-04-13 10:08:57.000000 venty-7.1.0/venty/classification_test.py
--rw-rw-rw-   0        0        0     1234 2024-04-12 14:26:00.000000 venty-7.1.0/venty/cloudevent.py
--rw-rw-rw-   0        0        0     1315 2024-03-16 17:12:53.000000 venty-7.1.0/venty/event_channel.py
--rw-rw-rw-   0        0        0      517 2024-04-12 14:22:40.000000 venty-7.1.0/venty/event_channel_test.py
--rw-rw-rw-   0        0        0     5032 2024-04-12 14:22:40.000000 venty-7.1.0/venty/event_logger.py
--rw-rw-rw-   0        0        0     3521 2024-04-12 13:16:52.000000 venty-7.1.0/venty/event_producer.py
--rw-rw-rw-   0        0        0     1724 2024-04-12 14:23:14.000000 venty-7.1.0/venty/event_producer_stack.py
--rw-rw-rw-   0        0        0     1580 2024-04-12 14:22:40.000000 venty-7.1.0/venty/event_producer_stack_test.py
--rw-rw-rw-   0        0        0     1533 2024-04-12 14:22:40.000000 venty-7.1.0/venty/event_producer_test.py
--rw-rw-rw-   0        0        0     7087 2024-04-13 09:34:29.000000 venty-7.1.0/venty/event_store.py
--rw-rw-rw-   0        0        0      713 2024-04-13 09:35:17.000000 venty-7.1.0/venty/event_stream_channel.py
--rw-rw-rw-   0        0        0     1327 2024-03-16 17:12:15.000000 venty-7.1.0/venty/http_event_channel.py
--rw-rw-rw-   0        0        0     1846 2024-04-12 14:22:40.000000 venty-7.1.0/venty/http_event_channel_test.py
--rw-rw-rw-   0        0        0      604 2024-03-16 17:00:49.000000 venty-7.1.0/venty/in_memory_event_channel.py
--rw-rw-rw-   0        0        0      338 2024-03-16 17:01:54.000000 venty-7.1.0/venty/in_memory_event_channel_test.py
--rw-rw-rw-   0        0        0     4492 2024-03-16 17:02:22.000000 venty-7.1.0/venty/in_memory_event_store.py
--rw-rw-rw-   0        0        0     6706 2024-03-16 00:47:54.000000 venty-7.1.0/venty/in_memory_event_store_test.py
--rw-rw-rw-   0        0        0      277 2024-04-12 15:22:15.000000 venty-7.1.0/venty/null_event_channel.py
--rw-rw-rw-   0        0        0      781 2024-04-08 17:48:30.000000 venty-7.1.0/venty/object_storage.py
--rw-rw-rw-   0        0        0      301 2024-04-08 18:03:19.000000 venty-7.1.0/venty/optional.py
--rw-rw-rw-   0        0        0        0 2023-01-06 20:34:35.000000 venty-7.1.0/venty/py.typed
--rw-rw-rw-   0        0        0      294 2024-04-05 09:27:44.000000 venty-7.1.0/venty/settings.py
--rw-rw-rw-   0        0        0      589 2024-03-16 16:02:34.000000 venty-7.1.0/venty/settings_test.py
--rw-rw-rw-   0        0        0     8293 2024-04-12 14:25:34.000000 venty-7.1.0/venty/sql_event_store.py
--rw-rw-rw-   0        0        0     6817 2024-04-12 14:22:40.000000 venty-7.1.0/venty/sql_event_store_test.py
--rw-rw-rw-   0        0        0      395 2024-04-12 14:22:40.000000 venty-7.1.0/venty/strong_types.py
--rw-rw-rw-   0        0        0      996 2024-04-12 14:23:35.000000 venty-7.1.0/venty/strong_types_test.py
--rw-rw-rw-   0        0        0      958 2024-03-16 16:40:05.000000 venty-7.1.0/venty/timing.py
--rw-rw-rw-   0        0        0      961 2024-03-15 18:40:30.000000 venty-7.1.0/venty/timing_test.py
-drwxrwxrwx   0        0        0        0 2024-04-13 20:58:53.251354 venty-7.1.0/venty.egg-info/
--rw-rw-rw-   0        0        0     2189 2024-04-13 20:58:52.000000 venty-7.1.0/venty.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1179 2024-04-13 20:58:52.000000 venty-7.1.0/venty.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-13 20:58:52.000000 venty-7.1.0/venty.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      102 2024-04-13 20:58:52.000000 venty-7.1.0/venty.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-13 20:58:52.000000 venty-7.1.0/venty.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-16 20:20:53.860136 venty-8.0.0/
+-rw-rw-rw-   0        0        0    11558 2022-08-05 14:38:16.000000 venty-8.0.0/LICENSE
+-rw-rw-rw-   0        0        0      167 2024-03-15 16:24:05.000000 venty-8.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2189 2024-04-16 20:20:53.860136 venty-8.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1127 2024-04-08 17:56:19.000000 venty-8.0.0/README.md
+-rw-rw-rw-   0        0        0       47 2024-03-26 20:12:48.000000 venty-8.0.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-04-16 20:20:53.860136 venty-8.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     2017 2024-04-16 20:20:27.000000 venty-8.0.0/setup.py
+-rw-rw-rw-   0        0        0      159 2024-03-16 16:56:05.000000 venty-8.0.0/test_requirements.txt
+-rw-rw-rw-   0        0        0      665 2024-03-27 06:50:13.000000 venty-8.0.0/tox.ini
+drwxrwxrwx   0        0        0        0 2024-04-16 20:20:53.840135 venty-8.0.0/venty/
+-rw-rw-rw-   0        0        0      257 2024-03-16 01:45:41.000000 venty-8.0.0/venty/__init__.py
+-rw-rw-rw-   0        0        0      245 2024-03-15 20:16:30.000000 venty-8.0.0/venty/_dummy.py
+-rw-rw-rw-   0        0        0      439 2024-04-12 14:47:07.000000 venty-8.0.0/venty/aggregate_channel.py
+-rw-rw-rw-   0        0        0     1858 2024-04-08 17:52:38.000000 venty-8.0.0/venty/aggregate_root.py
+-rw-rw-rw-   0        0        0     1390 2024-04-15 21:25:40.000000 venty-8.0.0/venty/aggregate_store.py
+-rw-rw-rw-   0        0        0     2084 2024-04-12 14:22:50.000000 venty-8.0.0/venty/aggregate_store_test.py
+-rw-rw-rw-   0        0        0      995 2024-04-16 19:56:20.000000 venty-8.0.0/venty/auth_event_producer.py
+-rw-rw-rw-   0        0        0      886 2024-04-13 10:07:54.000000 venty-8.0.0/venty/classification.py
+-rw-rw-rw-   0        0        0     1478 2024-04-13 10:08:57.000000 venty-8.0.0/venty/classification_test.py
+-rw-rw-rw-   0        0        0     1234 2024-04-12 14:26:00.000000 venty-8.0.0/venty/cloudevent.py
+-rw-rw-rw-   0        0        0     1315 2024-03-16 17:12:53.000000 venty-8.0.0/venty/event_channel.py
+-rw-rw-rw-   0        0        0      517 2024-04-12 14:22:40.000000 venty-8.0.0/venty/event_channel_test.py
+-rw-rw-rw-   0        0        0     5032 2024-04-12 14:22:40.000000 venty-8.0.0/venty/event_logger.py
+-rw-rw-rw-   0        0        0     3521 2024-04-16 19:06:07.000000 venty-8.0.0/venty/event_producer.py
+-rw-rw-rw-   0        0        0     1724 2024-04-12 14:23:14.000000 venty-8.0.0/venty/event_producer_stack.py
+-rw-rw-rw-   0        0        0     1580 2024-04-12 14:22:40.000000 venty-8.0.0/venty/event_producer_stack_test.py
+-rw-rw-rw-   0        0        0     1533 2024-04-12 14:22:40.000000 venty-8.0.0/venty/event_producer_test.py
+-rw-rw-rw-   0        0        0     7087 2024-04-16 19:17:08.000000 venty-8.0.0/venty/event_store.py
+-rw-rw-rw-   0        0        0      713 2024-04-13 09:35:17.000000 venty-8.0.0/venty/event_stream_channel.py
+-rw-rw-rw-   0        0        0     1327 2024-03-16 17:12:15.000000 venty-8.0.0/venty/http_event_channel.py
+-rw-rw-rw-   0        0        0     1846 2024-04-12 14:22:40.000000 venty-8.0.0/venty/http_event_channel_test.py
+-rw-rw-rw-   0        0        0      604 2024-03-16 17:00:49.000000 venty-8.0.0/venty/in_memory_event_channel.py
+-rw-rw-rw-   0        0        0      338 2024-03-16 17:01:54.000000 venty-8.0.0/venty/in_memory_event_channel_test.py
+-rw-rw-rw-   0        0        0     4492 2024-04-16 19:17:34.000000 venty-8.0.0/venty/in_memory_event_store.py
+-rw-rw-rw-   0        0        0     6706 2024-03-16 00:47:54.000000 venty-8.0.0/venty/in_memory_event_store_test.py
+-rw-rw-rw-   0        0        0      277 2024-04-12 15:22:15.000000 venty-8.0.0/venty/null_event_channel.py
+-rw-rw-rw-   0        0        0      781 2024-04-08 17:48:30.000000 venty-8.0.0/venty/object_storage.py
+-rw-rw-rw-   0        0        0      301 2024-04-08 18:03:19.000000 venty-8.0.0/venty/optional.py
+-rw-rw-rw-   0        0        0        0 2023-01-06 20:34:35.000000 venty-8.0.0/venty/py.typed
+-rw-rw-rw-   0        0        0      294 2024-04-05 09:27:44.000000 venty-8.0.0/venty/settings.py
+-rw-rw-rw-   0        0        0      589 2024-03-16 16:02:34.000000 venty-8.0.0/venty/settings_test.py
+-rw-rw-rw-   0        0        0     8293 2024-04-12 14:25:34.000000 venty-8.0.0/venty/sql_event_store.py
+-rw-rw-rw-   0        0        0     6817 2024-04-12 14:22:40.000000 venty-8.0.0/venty/sql_event_store_test.py
+-rw-rw-rw-   0        0        0      395 2024-04-12 14:22:40.000000 venty-8.0.0/venty/strong_types.py
+-rw-rw-rw-   0        0        0      996 2024-04-12 14:23:35.000000 venty-8.0.0/venty/strong_types_test.py
+-rw-rw-rw-   0        0        0      958 2024-03-16 16:40:05.000000 venty-8.0.0/venty/timing.py
+-rw-rw-rw-   0        0        0      961 2024-03-15 18:40:30.000000 venty-8.0.0/venty/timing_test.py
+drwxrwxrwx   0        0        0        0 2024-04-16 20:20:53.859138 venty-8.0.0/venty.egg-info/
+-rw-rw-rw-   0        0        0     2189 2024-04-16 20:20:53.000000 venty-8.0.0/venty.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1179 2024-04-16 20:20:53.000000 venty-8.0.0/venty.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 20:20:53.000000 venty-8.0.0/venty.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      102 2024-04-16 20:20:53.000000 venty-8.0.0/venty.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-16 20:20:53.000000 venty-8.0.0/venty.egg-info/top_level.txt
```

### Comparing `venty-7.1.0/LICENSE` & `venty-8.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `venty-7.1.0/PKG-INFO` & `venty-8.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: venty
-Version: 7.1.0
+Version: 8.0.0
 Summary: Venty
 Home-page: https://github.com/sasha-tkachev/venty
 Author: Sasha Tkachev
 Author-email: sasha64sasha@gmail.com
 License: UNKNOWN
 Keywords: cloudevents,cloudevents[pydantic],ce,cloud,events,event,rest
 Platform: UNKNOWN
```

### Comparing `venty-7.1.0/README.md` & `venty-8.0.0/README.md`

 * *Files identical despite different names*

### Comparing `venty-7.1.0/setup.py` & `venty-8.0.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 here = Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 if __name__ == "__main__":
     setuptools.setup(
         name="venty",
-        version="7.1.0",
+        version="8.0.0",
         author="Sasha Tkachev",
         author_email="sasha64sasha@gmail.com",
         description="Venty",
         long_description_content_type="text/markdown",
         long_description=long_description,
         home_page="https://github.com/sasha-tkachev/venty",
         url="https://github.com/sasha-tkachev/venty",
```

### Comparing `venty-7.1.0/tox.ini` & `venty-8.0.0/tox.ini`

 * *Files identical despite different names*

### Comparing `venty-7.1.0/venty/aggregate_root.py` & `venty-8.0.0/venty/aggregate_root.py`

 * *Files identical despite different names*

### Comparing `venty-7.1.0/venty/aggregate_store.py` & `venty-8.0.0/venty/aggregate_store.py`

 * *Files identical despite different names*

### Comparing `venty-7.1.0/venty/aggregate_store_test.py` & `venty-8.0.0/venty/aggregate_store_test.py`

 * *Files identical despite different names*

### Comparing `venty-7.1.0/venty/auth_event_producer.py` & `venty-8.0.0/venty/auth_event_producer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from typing import Optional, Any, Type, Dict
 from venty.event_producer import EventProducer, AttributeValue
 from venty.strong_types import CloudEventT
 
 
 class AuthEventProducer(EventProducer):
-    def __init__(self, authoid: str, authtype: str, parent: EventProducer):
-        self._authoid = authoid
+    def __init__(self, authid: str, authtype: str, parent: EventProducer):
+        self._authid = authid
         self._authtype = authtype
         self._parent = parent
 
     def produce_event(
         self,
         type_: Type[CloudEventT],
         data: Optional[Any],
         *,
         attributes: Optional[Dict[str, AttributeValue]] = None
     ) -> CloudEventT:
         if attributes is None:
             attributes = {}
         if ("authid" not in attributes) and ("authtype" not in attributes):
             # https://github.com/cloudevents/spec/blob/main/cloudevents/extensions/authcontext.md
-            attributes["authid"] = self._authoid
+            attributes["authid"] = self._authid
             attributes["authtype"] = self._authtype
         return self._parent.produce_event(type_, data, attributes=attributes)
```

### Comparing `venty-7.1.0/venty/classification.py` & `venty-8.0.0/venty/classification.py`

 * *Files identical despite different names*

### Comparing `venty-7.1.0/venty/classification_test.py` & `venty-8.0.0/venty/classification_test.py`

 * *Files identical despite different names*

### Comparing `venty-7.1.0/venty/cloudevent.py` & `venty-8.0.0/venty/cloudevent.py`

 * *Files identical despite different names*

### Comparing `venty-7.1.0/venty/event_channel.py` & `venty-8.0.0/venty/event_channel.py`

 * *Files identical despite different names*

### Comparing `venty-7.1.0/venty/event_channel_test.py` & `venty-8.0.0/venty/event_channel_test.py`

 * *Files identical despite different names*

### Comparing `venty-7.1.0/venty/event_logger.py` & `venty-8.0.0/venty/event_logger.py`

 * *Files identical despite different names*

### Comparing `venty-7.1.0/venty/event_producer.py` & `venty-8.0.0/venty/event_producer.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -88,18 +88,18 @@
         data: Optional[Any],
         *,
         attributes: Optional[Dict[str, AttributeValue]] = None,
     ) -> CloudEventT:
         if attributes is None:
             attributes = {}
         actual_attributes = self._default_attributes.copy()
-        actual_attributes.update(attributes)
         actual_attributes["source"] = self._source
         actual_attributes["id"] = self._id_selection_algorithm()
         actual_attributes["time"] = self._time_selection_algorithm()
+        actual_attributes.update(attributes)
         return type_.create(_normalize_attributes(actual_attributes), data)
 
 
 def testing_event_producer(
     *,
     source: Optional[EventSource] = EventSource("fake-source"),
     default_attributes: Optional[Dict[str, Any]] = None,
```

### Comparing `venty-7.1.0/venty/event_producer_stack.py` & `venty-8.0.0/venty/event_producer_stack.py`

 * *Files identical despite different names*

### Comparing `venty-7.1.0/venty/event_producer_stack_test.py` & `venty-8.0.0/venty/event_producer_stack_test.py`

 * *Files identical despite different names*

### Comparing `venty-7.1.0/venty/event_producer_test.py` & `venty-8.0.0/venty/event_producer_test.py`

 * *Files identical despite different names*

### Comparing `venty-7.1.0/venty/event_store.py` & `venty-8.0.0/venty/event_store.py`

 * *Files identical despite different names*

### Comparing `venty-7.1.0/venty/event_stream_channel.py` & `venty-8.0.0/venty/event_stream_channel.py`

 * *Files identical despite different names*

### Comparing `venty-7.1.0/venty/http_event_channel.py` & `venty-8.0.0/venty/http_event_channel.py`

 * *Files identical despite different names*

### Comparing `venty-7.1.0/venty/http_event_channel_test.py` & `venty-8.0.0/venty/http_event_channel_test.py`

 * *Files identical despite different names*

### Comparing `venty-7.1.0/venty/in_memory_event_channel.py` & `venty-8.0.0/venty/in_memory_event_channel.py`

 * *Files identical despite different names*

### Comparing `venty-7.1.0/venty/in_memory_event_store.py` & `venty-8.0.0/venty/in_memory_event_store.py`

 * *Files identical despite different names*

### Comparing `venty-7.1.0/venty/in_memory_event_store_test.py` & `venty-8.0.0/venty/in_memory_event_store_test.py`

 * *Files identical despite different names*

### Comparing `venty-7.1.0/venty/object_storage.py` & `venty-8.0.0/venty/object_storage.py`

 * *Files identical despite different names*

### Comparing `venty-7.1.0/venty/settings_test.py` & `venty-8.0.0/venty/settings_test.py`

 * *Files identical despite different names*

### Comparing `venty-7.1.0/venty/sql_event_store.py` & `venty-8.0.0/venty/sql_event_store.py`

 * *Files identical despite different names*

### Comparing `venty-7.1.0/venty/sql_event_store_test.py` & `venty-8.0.0/venty/sql_event_store_test.py`

 * *Files identical despite different names*

### Comparing `venty-7.1.0/venty/strong_types_test.py` & `venty-8.0.0/venty/strong_types_test.py`

 * *Files identical despite different names*

### Comparing `venty-7.1.0/venty/timing.py` & `venty-8.0.0/venty/timing.py`

 * *Files identical despite different names*

### Comparing `venty-7.1.0/venty/timing_test.py` & `venty-8.0.0/venty/timing_test.py`

 * *Files identical despite different names*

### Comparing `venty-7.1.0/venty.egg-info/PKG-INFO` & `venty-8.0.0/venty.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: venty
-Version: 7.1.0
+Version: 8.0.0
 Summary: Venty
 Home-page: https://github.com/sasha-tkachev/venty
 Author: Sasha Tkachev
 Author-email: sasha64sasha@gmail.com
 License: UNKNOWN
 Keywords: cloudevents,cloudevents[pydantic],ce,cloud,events,event,rest
 Platform: UNKNOWN
```

### Comparing `venty-7.1.0/venty.egg-info/SOURCES.txt` & `venty-8.0.0/venty.egg-info/SOURCES.txt`

 * *Files identical despite different names*
