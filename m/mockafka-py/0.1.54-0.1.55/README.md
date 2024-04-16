# Comparing `tmp/mockafka_py-0.1.54.tar.gz` & `tmp/mockafka_py-0.1.55.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mockafka_py-0.1.54.tar", max compression
+gzip compressed data, was "mockafka_py-0.1.55.tar", max compression
```

## Comparing `mockafka_py-0.1.54.tar` & `mockafka_py-0.1.55.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1067 2024-04-10 08:04:55.410152 mockafka_py-0.1.54/LICENSE
--rw-r--r--   0        0        0     6491 2024-04-10 08:04:55.410152 mockafka_py-0.1.54/README.md
--rw-r--r--   0        0        0      465 2024-04-10 08:04:55.414152 mockafka_py-0.1.54/mockafka/__init__.py
--rw-r--r--   0        0        0     7147 2024-04-10 08:04:55.414152 mockafka_py-0.1.54/mockafka/admin_client.py
--rw-r--r--   0        0        0      252 2024-04-10 08:04:55.414152 mockafka_py-0.1.54/mockafka/aiokafka/__init__.py
--rw-r--r--   0        0        0     2425 2024-04-10 08:04:55.414152 mockafka_py-0.1.54/mockafka/aiokafka/aiokafka_admin_client.py
--rw-r--r--   0        0        0     3434 2024-04-10 08:04:55.414152 mockafka_py-0.1.54/mockafka/aiokafka/aiokafka_consumer.py
--rw-r--r--   0        0        0     2050 2024-04-10 08:04:55.414152 mockafka_py-0.1.54/mockafka/aiokafka/aiokafka_producer.py
--rw-r--r--   0        0        0      522 2024-04-10 08:04:55.414152 mockafka_py-0.1.54/mockafka/broker_metadata.py
--rw-r--r--   0        0        0     1282 2024-04-10 08:04:55.414152 mockafka_py-0.1.54/mockafka/cluster_metadata.py
--rw-r--r--   0        0        0    11791 2024-04-10 08:04:55.414152 mockafka_py-0.1.54/mockafka/conumser.py
--rw-r--r--   0        0        0      376 2024-04-10 08:04:55.414152 mockafka_py-0.1.54/mockafka/decorators/__init__.py
--rw-r--r--   0        0        0     1825 2024-04-10 08:04:55.414152 mockafka_py-0.1.54/mockafka/decorators/aconsumer.py
--rw-r--r--   0        0        0     1769 2024-04-10 08:04:55.414152 mockafka_py-0.1.54/mockafka/decorators/aproducer.py
--rw-r--r--   0        0        0     1620 2024-04-10 08:04:55.414152 mockafka_py-0.1.54/mockafka/decorators/asetup_kafka.py
--rw-r--r--   0        0        0     1956 2024-04-10 08:04:55.414152 mockafka_py-0.1.54/mockafka/decorators/bulk_producer.py
--rw-r--r--   0        0        0     1366 2024-04-10 08:04:55.414152 mockafka_py-0.1.54/mockafka/decorators/consumer.py
--rw-r--r--   0        0        0     1524 2024-04-10 08:04:55.414152 mockafka_py-0.1.54/mockafka/decorators/producer.py
--rw-r--r--   0        0        0     1373 2024-04-10 08:04:55.414152 mockafka_py-0.1.54/mockafka/decorators/setup_kafka.py
--rw-r--r--   0        0        0     6283 2024-04-10 08:04:55.414152 mockafka_py-0.1.54/mockafka/kafka_store.py
--rw-r--r--   0        0        0     1643 2024-04-10 08:04:55.414152 mockafka_py-0.1.54/mockafka/message.py
--rw-r--r--   0        0        0     1579 2024-04-10 08:04:55.414152 mockafka_py-0.1.54/mockafka/producer.py
--rw-r--r--   0        0        0      798 2024-04-10 08:04:55.414152 mockafka_py-0.1.54/mockafka/topic_metadata.py
--rw-r--r--   0        0        0      879 2024-04-10 08:04:55.414152 mockafka_py-0.1.54/pyproject.toml
--rw-r--r--   0        0        0     7414 1970-01-01 00:00:00.000000 mockafka_py-0.1.54/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-16 13:50:56.026616 mockafka_py-0.1.55/LICENSE
+-rw-r--r--   0        0        0     6868 2024-04-16 13:50:56.026616 mockafka_py-0.1.55/README.md
+-rw-r--r--   0        0        0      498 2024-04-16 13:50:56.030616 mockafka_py-0.1.55/mockafka/__init__.py
+-rw-r--r--   0        0        0     7183 2024-04-16 13:50:56.030616 mockafka_py-0.1.55/mockafka/admin_client.py
+-rw-r--r--   0        0        0      238 2024-04-16 13:50:56.030616 mockafka_py-0.1.55/mockafka/aiokafka/__init__.py
+-rw-r--r--   0        0        0     2491 2024-04-16 13:50:56.030616 mockafka_py-0.1.55/mockafka/aiokafka/aiokafka_admin_client.py
+-rw-r--r--   0        0        0     3720 2024-04-16 13:50:56.030616 mockafka_py-0.1.55/mockafka/aiokafka/aiokafka_consumer.py
+-rw-r--r--   0        0        0     1843 2024-04-16 13:50:56.030616 mockafka_py-0.1.55/mockafka/aiokafka/aiokafka_producer.py
+-rw-r--r--   0        0        0      522 2024-04-16 13:50:56.030616 mockafka_py-0.1.55/mockafka/broker_metadata.py
+-rw-r--r--   0        0        0     1357 2024-04-16 13:50:56.030616 mockafka_py-0.1.55/mockafka/cluster_metadata.py
+-rw-r--r--   0        0        0    12919 2024-04-16 13:50:56.030616 mockafka_py-0.1.55/mockafka/conumser.py
+-rw-r--r--   0        0        0      376 2024-04-16 13:50:56.030616 mockafka_py-0.1.55/mockafka/decorators/__init__.py
+-rw-r--r--   0        0        0     1825 2024-04-16 13:50:56.030616 mockafka_py-0.1.55/mockafka/decorators/aconsumer.py
+-rw-r--r--   0        0        0     1705 2024-04-16 13:50:56.030616 mockafka_py-0.1.55/mockafka/decorators/aproducer.py
+-rw-r--r--   0        0        0     1737 2024-04-16 13:50:56.030616 mockafka_py-0.1.55/mockafka/decorators/asetup_kafka.py
+-rw-r--r--   0        0        0     1957 2024-04-16 13:50:56.030616 mockafka_py-0.1.55/mockafka/decorators/bulk_producer.py
+-rw-r--r--   0        0        0     1368 2024-04-16 13:50:56.030616 mockafka_py-0.1.55/mockafka/decorators/consumer.py
+-rw-r--r--   0        0        0     1460 2024-04-16 13:50:56.030616 mockafka_py-0.1.55/mockafka/decorators/producer.py
+-rw-r--r--   0        0        0     1411 2024-04-16 13:50:56.030616 mockafka_py-0.1.55/mockafka/decorators/setup_kafka.py
+-rw-r--r--   0        0        0     6414 2024-04-16 13:50:56.030616 mockafka_py-0.1.55/mockafka/kafka_store.py
+-rw-r--r--   0        0        0     1717 2024-04-16 13:50:56.030616 mockafka_py-0.1.55/mockafka/message.py
+-rw-r--r--   0        0        0     1543 2024-04-16 13:50:56.030616 mockafka_py-0.1.55/mockafka/producer.py
+-rw-r--r--   0        0        0      798 2024-04-16 13:50:56.030616 mockafka_py-0.1.55/mockafka/topic_metadata.py
+-rw-r--r--   0        0        0      879 2024-04-16 13:50:56.030616 mockafka_py-0.1.55/pyproject.toml
+-rw-r--r--   0        0        0     7791 1970-01-01 00:00:00.000000 mockafka_py-0.1.55/PKG-INFO
```

### Comparing `mockafka_py-0.1.54/LICENSE` & `mockafka_py-0.1.55/LICENSE`

 * *Files identical despite different names*

### Comparing `mockafka_py-0.1.54/README.md` & `mockafka_py-0.1.55/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,42 @@
 ![Alt text](banner.png)
 <p align="center">
     <em>Mockafka-py is a Python library designed for in-memory mocking of Kafka.</em>
 </p>
 
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/mockafka-py)
+![Codecov](https://img.shields.io/codecov/c/github/alm0ra/mockafka-py)
+[![CodeFactor](https://www.codefactor.io/repository/github/alm0ra/mockafka-py/badge)](https://www.codefactor.io/repository/github/alm0ra/mockafka-py)
+[![codebeat badge](https://codebeat.co/badges/9cda14cf-3aac-438f-a6f7-c67517d7d74f)](https://codebeat.co/projects/github-com-alm0ra-mockafka-py-main)
 ![GitHub Workflow Status (with event)](https://img.shields.io/github/actions/workflow/status/alm0ra/mockafka-py/python-app.yml)
 ![GitHub](https://img.shields.io/github/license/alm0ra/mockafka-py)
-![Codecov](https://img.shields.io/codecov/c/github/alm0ra/mockafka-py)
 ![GitHub release (with filter)](https://img.shields.io/github/v/release/alm0ra/mockafka-py)
 ![GitHub repo size](https://img.shields.io/github/repo-size/alm0ra/mockafka-py)
 
 # Mockafka: Fake Version for confluent-kafka-python & aiokafka
 
 # Features
 
 - Compatible with confluent-kafka
-- Compatible with aiokafka
+- Compatible with aiokafka (async support)
 - Supports Produce, Consume, and AdminClient operations with ease.
 
-# TODO
 
 # Getting Start
 
-### Installing via pip
+### Installing via pip or poetry
 
 ```bash
 pip install mockafka-py
+
+# or using poetry
+poetry add mockafka-py
 ```
 
+
 # Usage
 
 ## Multi-Decorator Examples for `confluent-kafka-python`
 
 In the following examples, we showcase the usage of multiple decorators to simulate different scenarios in a Mockafka
 environment. These scenarios include producing, consuming, and setting up Kafka topics using the provided decorators.
 
@@ -179,15 +184,15 @@
 <mockafka.message.Message object at 0x7fe84b4c31f0>
 <mockafka.message.Message object at 0x7fe84b4c32b0>
 <mockafka.message.Message object at 0x7fe84b4c3400>
 <mockafka.message.Message object at 0x7fe84b4c3340>
 None
 """
 ```
-
+# Async support
 ## Multi-Decorator Examples for `aiokafka`
 
 ### Example 1: Using `@aproduce` and `@aconsume` and `@asetup_kafka` Decorators
 
 #### Test Case: `test_produce_and_consume_with_decorator`
 
 ```python
```

### Comparing `mockafka_py-0.1.54/mockafka/admin_client.py` & `mockafka_py-0.1.55/mockafka/admin_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,17 @@
     def create_partition(self, partition: NewPartitions):
         """
         Create a single partition in the in-memory Kafka store.
 
         Parameters:
         - partition (NewPartitions): The partition object to be created.
         """
-        self.kafka.create_partition(topic=partition.topic, partitions=partition.new_total_count)
+        self.kafka.create_partition(
+            topic=partition.topic, partitions=partition.new_total_count
+        )
 
     def create_topics(self, topics: list[NewTopic]):
         """
         Create topics in the in-memory Kafka store.
 
         Parameters:
         - topics (List[NewTopic]): List of topic objects to be created.
@@ -74,15 +76,17 @@
 
         Parameters:
         - topic (NewTopic): The topic object to be created.
         """
         self.kafka.create_topic(topic.topic)
         self.create_partitions([NewPartitions(topic.topic, topic.num_partitions)])
 
-    def delete_topics(self, topics, future=None, request_timeout=None, operation_timeout=None):
+    def delete_topics(
+        self, topics, future=None, request_timeout=None, operation_timeout=None
+    ):
         """
         Delete topics from the in-memory Kafka store.
 
         Parameters:
         - topics: Topics to be deleted.
         - future: Unused parameter (for compatibility).
         - request_timeout: Unused parameter (for compatibility).
```

### Comparing `mockafka_py-0.1.54/mockafka/aiokafka/aiokafka_admin_client.py` & `mockafka_py-0.1.55/mockafka/aiokafka/aiokafka_admin_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,17 @@
         pass
 
     async def start(self):
         pass
 
     async def _create_topic(self, topic: NewTopic) -> None:
         self.kafka.create_topic(topic.name)
-        await self._create_partition(topic=topic.name, partition_count=topic.num_partitions)
+        await self._create_partition(
+            topic=topic.name, partition_count=topic.num_partitions
+        )
 
     async def _remove_topic(self, topic: str):
         self.kafka.remove_topic(topic=topic)
 
     async def create_topics(self, new_topics: list[NewTopic], *args, **kwargs):
         for topic in new_topics:
             await self._create_topic(topic=topic)
@@ -52,10 +54,14 @@
     async def delete_topics(self, topics: list[str], **kwargs) -> None:
         for topic in topics:
             await self._remove_topic(topic=topic)
 
     async def _create_partition(self, topic: str, partition_count: int):
         self.kafka.create_partition(topic=topic, partitions=partition_count)
 
-    async def create_partitions(self, topic_partitions: Dict[str, NewPartitions], *args, **kwargs):
+    async def create_partitions(
+        self, topic_partitions: Dict[str, NewPartitions], *args, **kwargs
+    ):
         for topic, partition in topic_partitions.items():
-            await self._create_partition(topic=topic, partition_count=partition.total_count)
+            await self._create_partition(
+                topic=topic, partition_count=partition.total_count
+            )
```

### Comparing `mockafka_py-0.1.54/mockafka/aiokafka/aiokafka_consumer.py` & `mockafka_py-0.1.55/mockafka/aiokafka/aiokafka_consumer.py`

 * *Files 25% similar despite different names*

```diff
@@ -40,17 +40,22 @@
 
     async def stop(self):
         self.consumer_store = {}
         self.subscribed_topic: list = []
 
     async def commit(self):
         for item in self.consumer_store:
-            topic, partition = item.split('*')
-            if self.kafka.get_partition_first_offset(topic, partition) <= self.consumer_store[item]:
-                self.kafka.set_first_offset(topic=topic, partition=partition, value=self.consumer_store[item])
+            topic, partition = item.split("*")
+            if (
+                self.kafka.get_partition_first_offset(topic, partition)
+                <= self.consumer_store[item]
+            ):
+                self.kafka.set_first_offset(
+                    topic=topic, partition=partition, value=self.consumer_store[item]
+                )
 
         self.consumer_store = {}
 
     async def topics(self):
         return self.subscribed_topic
 
     def subscribe(self, topics: list[str]):
@@ -64,33 +69,43 @@
     def subscribtion(self) -> list[str]:
         return self.subscribed_topic
 
     def unsubscribe(self):
         self.subscribed_topic = []
 
     def _get_key(self, topic, partition) -> str:
-        return f'{topic}*{partition}'
+        return f"{topic}*{partition}"
 
     async def getone(self):
         for topic in self.subscribed_topic:
             for partition in self.kafka.partition_list(topic=topic):
-                first_offset = self.kafka.get_partition_first_offset(topic=topic, partition=partition)
-                next_offset = self.kafka.get_partition_next_offset(topic=topic, partition=partition)
-                consumer_amount = self.consumer_store.get(self._get_key(topic, partition))
+                first_offset = self.kafka.get_partition_first_offset(
+                    topic=topic, partition=partition
+                )
+                next_offset = self.kafka.get_partition_next_offset(
+                    topic=topic, partition=partition
+                )
+                consumer_amount = self.consumer_store.get(
+                    self._get_key(topic, partition)
+                )
                 if first_offset == next_offset:
                     continue
 
                 if consumer_amount == next_offset:
                     continue
 
                 if consumer_amount is not None:
                     self.consumer_store[self._get_key(topic, partition)] += 1
                 else:
-                    self.consumer_store[self._get_key(topic, partition)] = first_offset + 1
-
-                return self.kafka.get_message(topic=topic, partition=partition, offset=first_offset)
+                    self.consumer_store[self._get_key(topic, partition)] = (
+                        first_offset + 1
+                    )
+
+                return self.kafka.get_message(
+                    topic=topic, partition=partition, offset=first_offset
+                )
 
         return None
 
     async def getmany(self):
         # FIXME: must impelement
         return await self.getone()
```

### Comparing `mockafka_py-0.1.54/mockafka/aiokafka/aiokafka_producer.py` & `mockafka_py-0.1.55/mockafka/aiokafka/aiokafka_producer.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,44 +24,46 @@
 
     def __init__(self, *args, **kwargs) -> None:
         self.kafka = KafkaStore()
 
     async def _produce(self, topic, value=None, *args, **kwargs) -> None:
         # create a message and call produce kafka
         message = Message(value=value, topic=topic, *args, **kwargs)
-        self.kafka.produce(message=message, topic=topic, partition=kwargs['partition'])
+        self.kafka.produce(message=message, topic=topic, partition=kwargs["partition"])
 
     async def start(self) -> None:
         pass
 
-    async def send(self,
-                   topic,
-                   value=None,
-                   key=None,
-                   partition=0,
-                   timestamp_ms=None,
-                   headers=None,
-                   ) -> None:
+    async def send(
+        self,
+        topic,
+        value=None,
+        key=None,
+        partition=0,
+        timestamp_ms=None,
+        headers=None,
+    ) -> None:
         await self._produce(
             topic=topic,
             value=value,
             key=key,
             partition=partition,
             headers=headers,
             timestamp_ms=timestamp_ms,
         )
 
-    async def send_and_wait(self,
-                            topic,
-                            value=None,
-                            key=None,
-                            partition=0,
-                            timestamp_ms=None,
-                            headers=None,
-                            ) -> None:
+    async def send_and_wait(
+        self,
+        topic,
+        value=None,
+        key=None,
+        partition=0,
+        timestamp_ms=None,
+        headers=None,
+    ) -> None:
         await self._produce(
             topic=topic,
             value=value,
             key=key,
             partition=partition,
             headers=headers,
             timestamp_ms=timestamp_ms,
```

### Comparing `mockafka_py-0.1.54/mockafka/broker_metadata.py` & `mockafka_py-0.1.55/mockafka/broker_metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
     This class is typically not user instantiated.
     """
 
     def __init__(self):
         self.id = 1
         """Broker id"""
-        self.host = 'fakebroker'
+        self.host = "fakebroker"
         """Broker hostname"""
         self.port = 9091
         """Broker port"""
 
     def __repr__(self):
         return "BrokerMetadata({}, {}:{})".format(self.id, self.host, self.port)
```

### Comparing `mockafka_py-0.1.54/mockafka/cluster_metadata.py` & `mockafka_py-0.1.55/mockafka/cluster_metadata.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,25 +9,29 @@
     Returned by list_topics().
 
     This class is typically not user instantiated.
     """
 
     def __init__(self, topic: str = None):
         self.kafka = KafkaStore()
-        self.cluster_id = 'test'
+        self.cluster_id = "test"
         self.controller_id = 1
         self.brokers = {1: BrokerMetadata()}
         self.topics = CustomDict()
         if topic:
             if self.kafka.is_topic_exist(topic=topic):
-                self.topics[topic] = TopicMetadata(topic, self.kafka.partition_list(topic=topic))
+                self.topics[topic] = TopicMetadata(
+                    topic, self.kafka.partition_list(topic=topic)
+                )
 
         else:
             for topic in self.kafka.topic_list():
-                self.topics[topic] = TopicMetadata(topic, self.kafka.partition_list(topic=topic))
+                self.topics[topic] = TopicMetadata(
+                    topic, self.kafka.partition_list(topic=topic)
+                )
 
         self.orig_broker_id = -1
         self.orig_broker_name = None
 
     def __repr__(self):
         return "ClusterMetadata({})".format(self.cluster_id)
 
@@ -37,8 +41,7 @@
 
 class CustomDict(dict):
     def __getitem__(self, key):
         try:
             return super().__getitem__(key)
         except KeyError:
             return
-
```

### Comparing `mockafka_py-0.1.54/mockafka/conumser.py` & `mockafka_py-0.1.55/mockafka/conumser.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-import warnings
+import random
+from copy import deepcopy
 
 from mockafka.cluster_metadata import ClusterMetadata
+from mockafka.kafka_store import KafkaStore
 from mockafka.message import Message
-from mockafka.kafka_store import KafkaStore, KafkaException
 
 __all__ = ["FakeConsumer"]
 
 
 class FakeConsumer(object):
     """
     Mock implementation of the Confluent Kafka Consumer for testing purposes.
@@ -45,27 +46,33 @@
         - args: Additional arguments (unused).
         - kwargs: Additional keyword arguments (unused).
         """
         self.kafka = KafkaStore()
         self.consumer_store = {}
         self.subscribed_topic: list = []
 
-    def consume(self, num_messages=1, *args, **kwargs):
+    def consume(self, num_messages=1, *args, **kwargs) -> list[Message]:
         """
         Consume messages from subscribed topics.
 
         Parameters:
         - num_messages (int): Number of messages to consume.
         - args: Additional arguments (unused).
         - kwargs: Additional keyword arguments (unused).
 
         Returns:
         - Message or None: Consumed message or None if no message is available.
         """
-        return self.poll()
+        consumed_messages = []
+        for count in range(num_messages):
+            message = self.poll()
+            if message:
+                consumed_messages.append(self.poll())
+
+        return consumed_messages
 
     def close(self, *args, **kwargs):
         """
         Close the consumer and reset state.
 
         Parameters:
         - args: Additional arguments (unused).
@@ -80,23 +87,40 @@
 
         Parameters:
         - message (Message): Consumed message (unused).
         - args: Additional arguments (unused).
         - kwargs: Additional keyword arguments (unused).
         """
         if message:
-            warnings.warn("commit a specific message is not yet implemented in mockafka and it act like commit a "
-                          "consumer entire messages ")
-
-        for item in self.consumer_store:
-            topic, partition = item.split('*')
-            if self.kafka.get_partition_first_offset(topic, partition) <= self.consumer_store[item]:
-                self.kafka.set_first_offset(topic=topic, partition=partition, value=self.consumer_store[item])
+            topic = message.topic()
+            partition = message.partition()
+            key = self._get_key(topic=topic, partition=partition)
+            if (
+                self.kafka.get_partition_first_offset(topic, partition)
+                <= self.consumer_store[key]
+            ):
+                self.kafka.set_first_offset(
+                    topic=topic, partition=partition, value=self.consumer_store[key]
+                )
+            del self.consumer_store[key]
+
+        else:
+            for item in self.consumer_store:
+                topic, partition = item.split("*")
+                if (
+                    self.kafka.get_partition_first_offset(topic, partition)
+                    <= self.consumer_store[item]
+                ):
+                    self.kafka.set_first_offset(
+                        topic=topic,
+                        partition=partition,
+                        value=self.consumer_store[item],
+                    )
 
-        self.consumer_store = {}
+            self.consumer_store = {}
 
     def list_topics(self, topic=None, *args, **kwargs):
         """
         List topics (returns ClusterMetadata).
 
         Parameters:
         - topic: Topic name (unused).
@@ -117,47 +141,60 @@
 
         Returns:
         - Message or None: Consumed message or None if no message is available.
         """
         if timeout:
             pass
             # sleep(timeout)
-
-        for topic in self.subscribed_topic:
-            for partition in self.kafka.partition_list(topic=topic):
-                first_offset = self.kafka.get_partition_first_offset(topic=topic, partition=partition)
-                next_offset = self.kafka.get_partition_next_offset(topic=topic, partition=partition)
-                consumer_amount = self.consumer_store.get(self._get_key(topic, partition))
+        topics_to_consume = deepcopy(self.subscribed_topic)
+        random.shuffle(topics_to_consume)
+        for topic in topics_to_consume:
+            partition_to_consume = deepcopy(self.kafka.partition_list(topic=topic))
+            random.shuffle(topics_to_consume)
+            for partition in partition_to_consume:
+                first_offset = self.kafka.get_partition_first_offset(
+                    topic=topic, partition=partition
+                )
+                next_offset = self.kafka.get_partition_next_offset(
+                    topic=topic, partition=partition
+                )
+                consumer_amount = self.consumer_store.get(
+                    self._get_key(topic, partition)
+                )
                 if first_offset == next_offset:
                     continue
 
                 if consumer_amount == next_offset:
                     continue
 
                 if consumer_amount is not None:
                     self.consumer_store[self._get_key(topic, partition)] += 1
                 else:
-                    self.consumer_store[self._get_key(topic, partition)] = first_offset + 1
-
-                return self.kafka.get_message(topic=topic, partition=partition, offset=first_offset)
+                    self.consumer_store[self._get_key(topic, partition)] = (
+                        first_offset + 1
+                    )
+
+                return self.kafka.get_message(
+                    topic=topic, partition=partition, offset=first_offset
+                )
 
         return None
 
     def _get_key(self, topic, partition) -> str:
         """
         Generate a unique key for a topic-partition pair.
 
         Parameters:
         - topic: Topic name.
         - partition: Partition number.
 
         Returns:
         - str: Unique key for the topic-partition pair.
         """
-        return f'{topic}*{partition}'
+        return f"{topic}*{partition}"
 
     def subscribe(self, topics, on_assign=None, *args, **kwargs):
         """
         Subscribe to one or more topics.
 
         Parameters:
         - topics (list): List of topics to subscribe to.
@@ -182,15 +219,15 @@
         Parameters:
         - args: Additional arguments (unused).
         - kwargs: Additional keyword arguments.
 
         Raises:
         - ValueError: If no 'topics' keyword argument is provided.
         """
-        topics = kwargs.get('topics', [])
+        topics = kwargs.get("topics", [])
         for topic in topics:
             if topic in self.subscribed_topic:
                 self.subscribed_topic.remove(topic)
 
     def assign(self, partitions):
         """
         Assign partitions to the consumer (unsupported in mockafka).
```

### Comparing `mockafka_py-0.1.54/mockafka/decorators/aconsumer.py` & `mockafka_py-0.1.55/mockafka/decorators/aconsumer.py`

 * *Files identical despite different names*

### Comparing `mockafka_py-0.1.54/mockafka/decorators/aproducer.py` & `mockafka_py-0.1.55/mockafka/decorators/aproducer.py`

 * *Files 13% similar despite different names*

```diff
@@ -30,28 +30,24 @@
 
     """
 
     def decorator(func):
         @wraps(func)
         async def wrapper(*args, **kwargs):
             # Extract parameters from the decorator_args
-            topic = decorator_args.get('topic', None)
-            value = decorator_args.get('value', None)
-            key = decorator_args.get('key', None)
-            headers = decorator_args.get('headers', None)
-            partition = decorator_args.get('partition', None)
+            topic = decorator_args.get("topic", None)
+            value = decorator_args.get("value", None)
+            key = decorator_args.get("key", None)
+            headers = decorator_args.get("headers", None)
+            partition = decorator_args.get("partition", None)
 
             # Create a FakeProducer instance and produce the message
             fake_producer = FakeAIOKafkaProducer()
             await fake_producer.send(
-                topic=topic,
-                partition=partition,
-                value=value,
-                key=key,
-                headers=headers
+                topic=topic, partition=partition, value=value, key=key, headers=headers
             )
 
             # Call the original function
             result = await func(*args, **kwargs)
             return result
 
         return wrapper
```

### Comparing `mockafka_py-0.1.54/mockafka/decorators/asetup_kafka.py` & `mockafka_py-0.1.55/mockafka/decorators/asetup_kafka.py`

 * *Files 16% similar despite different names*

```diff
@@ -33,18 +33,23 @@
         @wraps(func)
         async def wrapper(*args, **kwargs):
             # Create a FakeAdminClient instance with the specified clean option
             fake_admin = FakeAIOKafkaAdmin(clean=clean)
 
             # Create specified topics using the FakeAdminClient
             for item in topics:
-                topic = item.get('topic', None)
-                partition = item.get('partition', None)
+                topic = item.get("topic", None)
+                partition = item.get("partition", None)
                 await fake_admin.create_topics(
-                    new_topics=[NewTopic(name=topic, num_partitions=partition, replication_factor=1)])
+                    new_topics=[
+                        NewTopic(
+                            name=topic, num_partitions=partition, replication_factor=1
+                        )
+                    ]
+                )
 
             # Call the original function
             result = await func(*args, **kwargs)
             return result
 
         return wrapper
```

### Comparing `mockafka_py-0.1.54/mockafka/decorators/bulk_producer.py` & `mockafka_py-0.1.55/mockafka/decorators/bulk_producer.py`

 * *Files 13% similar despite different names*

```diff
@@ -30,29 +30,29 @@
         @wraps(func)
         def wrapper(*args, **kwargs):
             # Create a FakeProducer instance for producing messages
             fake_producer = FakeProducer()
 
             # Extract parameters from each message dictionary and produce messages
             for item in list_of_messages:
-                value = item.get('value', None)
-                key = item.get('key', None)
-                topic = item.get('topic', None)
-                partition = item.get('partition', None)
-                timestamp = item.get('timestamp', None)
-                headers = item.get('headers', None)
+                value = item.get("value", None)
+                key = item.get("key", None)
+                topic = item.get("topic", None)
+                partition = item.get("partition", None)
+                timestamp = item.get("timestamp", None)
+                headers = item.get("headers", None)
 
                 # Produce the message using the FakeProducer
                 fake_producer.produce(
                     topic=topic,
                     partition=partition,
                     value=value,
                     key=key,
                     timestamp=timestamp,
-                    headers=headers
+                    headers=headers,
                 )
 
             # Call the original function
             result = func(*args, **kwargs)
             return result
 
         return wrapper
```

### Comparing `mockafka_py-0.1.54/mockafka/decorators/consumer.py` & `mockafka_py-0.1.55/mockafka/decorators/consumer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from functools import wraps
 from mockafka import FakeConsumer
 
+
 def consume(topics: list[str], auto_commit: bool = True):
     """
     A decorator for simulating message consumption using a FakeConsumer.
 
     Parameters:
     - topics (list[str]): A list of topics to subscribe to.
     - auto_commit (bool): Whether to automatically commit offsets after consuming messages.
@@ -12,14 +13,15 @@
     Example Usage:
     ```python
     @consume(topics=['test_topic'], auto_commit=False)
     def test_function(message):
         # Your test logic for processing the consumed message here
     ```
     """
+
     def decorator(func):
         @wraps(func)
         def wrapper(*args, **kwargs):
             # Create a FakeConsumer instance and subscribe to specified topics
             fake_consumer = FakeConsumer()
             fake_consumer.subscribe(topics=topics)
```

### Comparing `mockafka_py-0.1.54/mockafka/decorators/setup_kafka.py` & `mockafka_py-0.1.55/mockafka/decorators/setup_kafka.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,17 +23,19 @@
         @wraps(func)
         def wrapper(*args, **kwargs):
             # Create a FakeAdminClient instance with the specified clean option
             fake_admin = FakeAdminClientImpl(clean=clean)
 
             # Create specified topics using the FakeAdminClient
             for item in topics:
-                topic = item.get('topic', None)
-                partition = item.get('partition', None)
-                fake_admin.create_topics(topics=[NewTopic(topic=topic, num_partitions=partition)])
+                topic = item.get("topic", None)
+                partition = item.get("partition", None)
+                fake_admin.create_topics(
+                    topics=[NewTopic(topic=topic, num_partitions=partition)]
+                )
 
             # Call the original function
             result = func(*args, **kwargs)
             return result
 
         return wrapper
```

### Comparing `mockafka_py-0.1.54/mockafka/kafka_store.py` & `mockafka_py-0.1.55/mockafka/kafka_store.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 offset_store = {
     'sample_topic_1': {
         'first_offset': 0,
         'next_offset': 0,
     }
 }
 """
+
 from confluent_kafka import KafkaException
 from .message import Message
 from copy import deepcopy
 
 mock_topics: dict[str, dict[int, list[Message]]] = {}
 
 offset_store: dict[str, dict[str, int]] = {}
@@ -26,69 +27,70 @@
 __all__ = ["KafkaStore"]
 
 
 class SingletonMeta(type):
     _instances = {}
 
     def __call__(cls, *args, **kwargs):
-        if cls not in cls._instances or 'clean' in kwargs.keys():
+        if cls not in cls._instances or "clean" in kwargs.keys():
             instance = super().__call__(*args, **kwargs)
             cls._instances[cls] = instance
         return cls._instances[cls]
 
 
 class KafkaStore(metaclass=SingletonMeta):
     """
     In memory kafka store
     """
-    FIRST_OFFSET = 'first_offset'
-    NEXT_OFFSET = 'next_offset'
+
+    FIRST_OFFSET = "first_offset"
+    NEXT_OFFSET = "next_offset"
 
     def __init__(self, clean: bool = False):
         if clean:
             mock_topics.clear()
             offset_store.clear()
 
     @staticmethod
     def is_topic_exist(topic: str) -> bool:
         return topic in mock_topics.keys()
 
     @classmethod
     def is_partition_exist_on_topic(cls, topic: str, partition_num: int) -> bool:
         if not cls.is_topic_exist(topic=topic):
-            raise KafkaException('Topic Does not exist')
+            raise KafkaException("Topic Does not exist")
 
         return mock_topics[topic].get(partition_num, None) is not None
 
     @staticmethod
     def get_number_of_partition(topic: str) -> int:
         return len(mock_topics[topic].keys())
 
     @staticmethod
     def create_topic(topic: str):
         if mock_topics.get(topic, None) is not None:
-            raise KafkaException(f'{topic} exist is fake kafka')
+            raise KafkaException(f"{topic} exist is fake kafka")
 
         mock_topics[topic] = {}
 
     def create_partition(self, topic: str, partitions: int):
         if not self.is_topic_exist(topic=topic):
             self.create_topic(topic=topic)
 
         len_of_current_partition = len(mock_topics[topic].keys())
         if partitions >= len_of_current_partition:
             for i in range(len_of_current_partition, partitions):
                 mock_topics[topic][i] = []
                 offset_store[self.get_offset_store_key(topic, i)] = {
                     self.FIRST_OFFSET: 0,
-                    self.NEXT_OFFSET: 0
+                    self.NEXT_OFFSET: 0,
                 }
 
         else:
-            raise KafkaException('can not decrease partition of topic')
+            raise KafkaException("can not decrease partition of topic")
 
     def remove_topic(self, topic: str):
         if not self.is_topic_exist(topic=topic):
             return
 
         mock_topics.pop(topic)
 
@@ -106,30 +108,34 @@
             offset_store[offset_store_key][self.FIRST_OFFSET] = value
 
     def _add_next_offset(self, topic: str, partition: int):
         offset_store_key = self.get_offset_store_key(topic=topic, partition=partition)
         offset_store[offset_store_key][self.NEXT_OFFSET] += 1
 
     def get_offset_store_key(self, topic: str, partition: int):
-        return f'{topic}*{partition}'
+        return f"{topic}*{partition}"
 
     def produce(self, message: Message, topic: str, partition: int):
         if not topic:
             return
 
         if partition is None:
-            raise KafkaException('you must assign partition when you want to produce message')
+            raise KafkaException(
+                "you must assign partition when you want to produce message"
+            )
 
         if not self.is_topic_exist(topic=topic):
             if partition == 0:
                 partition = 1
             self.create_partition(topic=topic, partitions=partition)
 
         if mock_topics[topic].get(partition, None) is None:
-            raise KafkaException(f'can not produce on partition {partition} of {topic}, partition does not exist')
+            raise KafkaException(
+                f"can not produce on partition {partition} of {topic}, partition does not exist"
+            )
 
         # add message to topic
         mock_topics[topic][partition].append(message)
 
         self._add_next_offset(topic=topic, partition=partition)
 
     def get_message(self, topic: str, partition: int, offset: int) -> Message:
@@ -154,33 +160,37 @@
     @staticmethod
     def get_messages_in_partition(topic: str, partition: int) -> list[Message]:
         return mock_topics[topic][partition]
 
     def number_of_message_in_topic(self, topic: str) -> int:
         count_of_messages = 0
         for partition in self.partition_list(topic=topic):
-            count_of_messages += len(self.get_messages_in_partition(topic=topic, partition=partition))
+            count_of_messages += len(
+                self.get_messages_in_partition(topic=topic, partition=partition)
+            )
 
         return count_of_messages
 
     def clear_topic_messages(self, topic: str):
         for partition in self.partition_list(topic=topic):
             self.clear_partition_messages(topic=topic, partition=partition)
 
     @staticmethod
     def clear_partition_messages(topic: str, partition: int):
         mock_topics[topic][partition] = []
 
-    def reset_offset(self, topic: str, strategy: str = 'latest'):
+    def reset_offset(self, topic: str, strategy: str = "latest"):
         for partition in self.partition_list(topic=topic):
             key = self.get_offset_store_key(topic, partition)
 
-            if strategy == 'latest':
-                offset_store[key][self.FIRST_OFFSET] = offset_store[key][self.NEXT_OFFSET]
+            if strategy == "latest":
+                offset_store[key][self.FIRST_OFFSET] = offset_store[key][
+                    self.NEXT_OFFSET
+                ]
 
-            elif strategy == 'earliest':
+            elif strategy == "earliest":
                 offset_store[key][self.FIRST_OFFSET] = 0
 
     @staticmethod
     def fresh():
         mock_topics.clear()
         offset_store.clear()
```

### Comparing `mockafka_py-0.1.54/mockafka/message.py` & `mockafka_py-0.1.55/mockafka/message.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from typing import Optional
 
 from confluent_kafka import KafkaError
 
 
 class Message:
     def __init__(self, *args, **kwargs):
-        self._headers: Optional[dict] = kwargs.get('headers', None)
-        self._key: Optional[str] = kwargs.get('key', None)
-        self._value: Optional[str] = kwargs.get('value', None)
-        self._topic: Optional[str] = kwargs.get('topic', None)
-        self._offset: Optional[int] = kwargs.get('offset', None)
-        self._error: Optional[KafkaError] = kwargs.get('error', None)
-        self._latency: Optional[float] = kwargs.get('latency', None)
-        self._leader_epoch: Optional[int] = kwargs.get('leader_epoch', None)
-        self._partition: Optional[int] = kwargs.get('partition', None)
-        self._timestamp: int = kwargs.get('timestamp', None)
+        self._headers: Optional[dict] = kwargs.get("headers", None)
+        self._key: Optional[str] = kwargs.get("key", None)
+        self._value: Optional[str] = kwargs.get("value", None)
+        self._topic: Optional[str] = kwargs.get("topic", None)
+        self._offset: Optional[int] = kwargs.get("offset", None)
+        self._error: Optional[KafkaError] = kwargs.get("error", None)
+        self._latency: Optional[float] = kwargs.get("latency", None)
+        self._leader_epoch: Optional[int] = kwargs.get("leader_epoch", None)
+        self._partition: Optional[int] = kwargs.get("partition", None)
+        self._timestamp: int = kwargs.get("timestamp", None)
 
     def offset(self, *args, **kwargs):
         return self._offset
 
     def latency(self, *args, **kwargs):
         return self._latency
 
@@ -36,14 +36,17 @@
 
     def timestamp(self, *args, **kwargs):
         return self._timestamp
 
     def topic(self, *args, **kwargs):
         return self._topic
 
+    def partition(self, *args, **kwargs):
+        return self._partition
+
     def error(self):
         return self._error
 
     def set_headers(self, *args, **kwargs):  # real signature unknown
         pass
 
     def set_key(self, *args, **kwargs):  # real signature unknown
```

### Comparing `mockafka_py-0.1.54/mockafka/producer.py` & `mockafka_py-0.1.55/mockafka/producer.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 class FakeProducer(object):
     def __init__(self, config: dict = None):
         self.kafka = KafkaStore()
 
     def produce(self, topic, value=None, *args, **kwargs):
         # create a message and call produce kafka
         message = Message(value=value, topic=topic, *args, **kwargs)
-        self.kafka.produce(message=message, topic=topic, partition=kwargs['partition'])
+        self.kafka.produce(message=message, topic=topic, partition=kwargs["partition"])
 
     def list_topics(self, topic=None, *args, **kwargs):
         return ClusterMetadata(topic)
 
     def abort_transaction(self, timeout=None):
         # This method Does not support in mockafka
         pass
@@ -41,11 +41,10 @@
         # This method Does not support in mockafka
         return 0
 
     def purge(self, in_queue=True, *args, **kwargs):
         # This method Does not support in mockafka
         pass
 
-    def send_offsets_to_transaction(self, positions, group_metadata,
-                                    timeout=None):
+    def send_offsets_to_transaction(self, positions, group_metadata, timeout=None):
         # This method Does not support in mockafka
         pass
```

### Comparing `mockafka_py-0.1.54/mockafka/topic_metadata.py` & `mockafka_py-0.1.55/mockafka/topic_metadata.py`

 * *Files identical despite different names*

### Comparing `mockafka_py-0.1.54/pyproject.toml` & `mockafka_py-0.1.55/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mockafka-py"
-version = "0.1.54"
+version = "0.1.55"
 authors = ["alm0ra <ali.mrd318@gmail.com>"]
 repository = "https://github.com/alm0ra/mockafka-py"
 documentation = "https://github.com/alm0ra/mockafka-py/docs"
 
 
 description = "A mock library for confluent kafka"
 readme = "README.md"
```

### Comparing `mockafka_py-0.1.54/PKG-INFO` & `mockafka_py-0.1.55/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mockafka-py
-Version: 0.1.54
+Version: 0.1.55
 Summary: A mock library for confluent kafka
 Home-page: https://github.com/alm0ra/mockafka-py
 Author: alm0ra
 Author-email: ali.mrd318@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -23,38 +23,43 @@
 
 ![Alt text](banner.png)
 <p align="center">
     <em>Mockafka-py is a Python library designed for in-memory mocking of Kafka.</em>
 </p>
 
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/mockafka-py)
+![Codecov](https://img.shields.io/codecov/c/github/alm0ra/mockafka-py)
+[![CodeFactor](https://www.codefactor.io/repository/github/alm0ra/mockafka-py/badge)](https://www.codefactor.io/repository/github/alm0ra/mockafka-py)
+[![codebeat badge](https://codebeat.co/badges/9cda14cf-3aac-438f-a6f7-c67517d7d74f)](https://codebeat.co/projects/github-com-alm0ra-mockafka-py-main)
 ![GitHub Workflow Status (with event)](https://img.shields.io/github/actions/workflow/status/alm0ra/mockafka-py/python-app.yml)
 ![GitHub](https://img.shields.io/github/license/alm0ra/mockafka-py)
-![Codecov](https://img.shields.io/codecov/c/github/alm0ra/mockafka-py)
 ![GitHub release (with filter)](https://img.shields.io/github/v/release/alm0ra/mockafka-py)
 ![GitHub repo size](https://img.shields.io/github/repo-size/alm0ra/mockafka-py)
 
 # Mockafka: Fake Version for confluent-kafka-python & aiokafka
 
 # Features
 
 - Compatible with confluent-kafka
-- Compatible with aiokafka
+- Compatible with aiokafka (async support)
 - Supports Produce, Consume, and AdminClient operations with ease.
 
-# TODO
 
 # Getting Start
 
-### Installing via pip
+### Installing via pip or poetry
 
 ```bash
 pip install mockafka-py
+
+# or using poetry
+poetry add mockafka-py
 ```
 
+
 # Usage
 
 ## Multi-Decorator Examples for `confluent-kafka-python`
 
 In the following examples, we showcase the usage of multiple decorators to simulate different scenarios in a Mockafka
 environment. These scenarios include producing, consuming, and setting up Kafka topics using the provided decorators.
 
@@ -202,15 +207,15 @@
 <mockafka.message.Message object at 0x7fe84b4c31f0>
 <mockafka.message.Message object at 0x7fe84b4c32b0>
 <mockafka.message.Message object at 0x7fe84b4c3400>
 <mockafka.message.Message object at 0x7fe84b4c3340>
 None
 """
 ```
-
+# Async support
 ## Multi-Decorator Examples for `aiokafka`
 
 ### Example 1: Using `@aproduce` and `@aconsume` and `@asetup_kafka` Decorators
 
 #### Test Case: `test_produce_and_consume_with_decorator`
 
 ```python
```

