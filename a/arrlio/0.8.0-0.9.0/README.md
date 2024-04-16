# Comparing `tmp/arrlio-0.8.0.tar.gz` & `tmp/arrlio-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arrlio-0.8.0.tar", last modified: Sat Jan  1 15:44:29 2022, max compression
+gzip compressed data, was "arrlio-0.9.0.tar", last modified: Wed Jan 26 21:06:11 2022, max compression
```

## Comparing `arrlio-0.8.0.tar` & `arrlio-0.9.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 levsh      (501) staff       (20)        0 2022-01-01 15:44:29.453015 arrlio-0.8.0/
--rw-r--r--   0 levsh      (501) staff       (20)     1068 2022-01-01 15:15:23.000000 arrlio-0.8.0/LICENSE
--rw-r--r--   0 levsh      (501) staff       (20)      524 2022-01-01 15:44:29.452735 arrlio-0.8.0/PKG-INFO
--rw-r--r--   0 levsh      (501) staff       (20)     1218 2022-01-01 15:26:54.000000 arrlio-0.8.0/README.md
-drwxr-xr-x   0 levsh      (501) staff       (20)        0 2022-01-01 15:44:29.445005 arrlio-0.8.0/arrlio/
--rw-r--r--   0 levsh      (501) staff       (20)      587 2022-01-01 15:27:29.000000 arrlio-0.8.0/arrlio/__init__.py
-drwxr-xr-x   0 levsh      (501) staff       (20)        0 2022-01-01 15:44:29.450108 arrlio-0.8.0/arrlio/backend/
--rw-r--r--   0 levsh      (501) staff       (20)        0 2022-01-01 15:15:23.000000 arrlio-0.8.0/arrlio/backend/__init__.py
--rw-r--r--   0 levsh      (501) staff       (20)     2466 2022-01-01 15:18:48.000000 arrlio-0.8.0/arrlio/backend/base.py
--rw-r--r--   0 levsh      (501) staff       (20)     6676 2022-01-01 15:18:48.000000 arrlio-0.8.0/arrlio/backend/local.py
--rw-r--r--   0 levsh      (501) staff       (20)    21389 2022-01-01 15:18:48.000000 arrlio-0.8.0/arrlio/backend/rabbitmq.py
--rw-r--r--   0 levsh      (501) staff       (20)     8580 2022-01-01 15:18:48.000000 arrlio-0.8.0/arrlio/backend/redis.py
--rw-r--r--   0 levsh      (501) staff       (20)    16327 2022-01-01 15:18:48.000000 arrlio-0.8.0/arrlio/core.py
--rw-r--r--   0 levsh      (501) staff       (20)     2499 2022-01-01 15:15:23.000000 arrlio-0.8.0/arrlio/crypto.py
--rw-r--r--   0 levsh      (501) staff       (20)      222 2022-01-01 15:15:23.000000 arrlio-0.8.0/arrlio/exc.py
--rw-r--r--   0 levsh      (501) staff       (20)     6531 2022-01-01 15:18:48.000000 arrlio-0.8.0/arrlio/models.py
-drwxr-xr-x   0 levsh      (501) staff       (20)        0 2022-01-01 15:44:29.452123 arrlio-0.8.0/arrlio/serializer/
--rw-r--r--   0 levsh      (501) staff       (20)        0 2022-01-01 15:15:23.000000 arrlio-0.8.0/arrlio/serializer/__init__.py
--rw-r--r--   0 levsh      (501) staff       (20)      818 2022-01-01 15:15:23.000000 arrlio-0.8.0/arrlio/serializer/base.py
--rw-r--r--   0 levsh      (501) staff       (20)     4091 2022-01-01 15:18:48.000000 arrlio-0.8.0/arrlio/serializer/json.py
--rw-r--r--   0 levsh      (501) staff       (20)      661 2022-01-01 15:15:23.000000 arrlio-0.8.0/arrlio/serializer/nop.py
--rw-r--r--   0 levsh      (501) staff       (20)     2774 2022-01-01 15:18:48.000000 arrlio-0.8.0/arrlio/settings.py
--rw-r--r--   0 levsh      (501) staff       (20)     2263 2022-01-01 15:15:23.000000 arrlio-0.8.0/arrlio/tp.py
--rw-r--r--   0 levsh      (501) staff       (20)     3744 2022-01-01 15:18:48.000000 arrlio-0.8.0/arrlio/utils.py
-drwxr-xr-x   0 levsh      (501) staff       (20)        0 2022-01-01 15:44:29.447160 arrlio-0.8.0/arrlio.egg-info/
--rw-r--r--   0 levsh      (501) staff       (20)      524 2022-01-01 15:44:29.000000 arrlio-0.8.0/arrlio.egg-info/PKG-INFO
--rw-r--r--   0 levsh      (501) staff       (20)      537 2022-01-01 15:44:29.000000 arrlio-0.8.0/arrlio.egg-info/SOURCES.txt
--rw-r--r--   0 levsh      (501) staff       (20)       49 2022-01-01 15:44:29.000000 arrlio-0.8.0/arrlio.egg-info/dependency_links.txt
--rw-r--r--   0 levsh      (501) staff       (20)       72 2022-01-01 15:44:29.000000 arrlio-0.8.0/arrlio.egg-info/requires.txt
--rw-r--r--   0 levsh      (501) staff       (20)        7 2022-01-01 15:44:29.000000 arrlio-0.8.0/arrlio.egg-info/top_level.txt
--rw-r--r--   0 levsh      (501) staff       (20)       38 2022-01-01 15:44:29.453105 arrlio-0.8.0/setup.cfg
--rw-r--r--   0 levsh      (501) staff       (20)     1232 2022-01-01 15:26:54.000000 arrlio-0.8.0/setup.py
+drwxr-xr-x   0 levsh      (501) staff       (20)        0 2022-01-26 21:06:11.076310 arrlio-0.9.0/
+-rw-r--r--   0 levsh      (501) staff       (20)     1068 2022-01-01 15:15:23.000000 arrlio-0.9.0/LICENSE
+-rw-r--r--   0 levsh      (501) staff       (20)      471 2022-01-26 21:06:11.075989 arrlio-0.9.0/PKG-INFO
+-rw-r--r--   0 levsh      (501) staff       (20)     2149 2022-01-26 20:36:32.000000 arrlio-0.9.0/README.md
+drwxr-xr-x   0 levsh      (501) staff       (20)        0 2022-01-26 21:06:11.069702 arrlio-0.9.0/arrlio/
+-rw-r--r--   0 levsh      (501) staff       (20)      548 2022-01-26 21:02:46.000000 arrlio-0.9.0/arrlio/__init__.py
+drwxr-xr-x   0 levsh      (501) staff       (20)        0 2022-01-26 21:06:11.073654 arrlio-0.9.0/arrlio/backends/
+-rw-r--r--   0 levsh      (501) staff       (20)        0 2022-01-26 20:36:32.000000 arrlio-0.9.0/arrlio/backends/__init__.py
+-rw-r--r--   0 levsh      (501) staff       (20)     2867 2022-01-26 20:36:32.000000 arrlio-0.9.0/arrlio/backends/base.py
+-rw-r--r--   0 levsh      (501) staff       (20)     8669 2022-01-26 20:36:32.000000 arrlio-0.9.0/arrlio/backends/local.py
+-rw-r--r--   0 levsh      (501) staff       (20)    26240 2022-01-26 20:36:32.000000 arrlio-0.9.0/arrlio/backends/rabbitmq.py
+-rw-r--r--   0 levsh      (501) staff       (20)    11022 2022-01-26 20:36:32.000000 arrlio-0.9.0/arrlio/backends/redis.py
+-rw-r--r--   0 levsh      (501) staff       (20)    18564 2022-01-26 20:36:32.000000 arrlio-0.9.0/arrlio/core.py
+-rw-r--r--   0 levsh      (501) staff       (20)     2499 2022-01-01 15:15:23.000000 arrlio-0.9.0/arrlio/crypto.py
+-rw-r--r--   0 levsh      (501) staff       (20)      222 2022-01-01 15:15:23.000000 arrlio-0.9.0/arrlio/exc.py
+-rw-r--r--   0 levsh      (501) staff       (20)     7045 2022-01-26 20:36:32.000000 arrlio-0.9.0/arrlio/models.py
+drwxr-xr-x   0 levsh      (501) staff       (20)        0 2022-01-26 21:06:11.075275 arrlio-0.9.0/arrlio/serializer/
+-rw-r--r--   0 levsh      (501) staff       (20)        0 2022-01-01 15:15:23.000000 arrlio-0.9.0/arrlio/serializer/__init__.py
+-rw-r--r--   0 levsh      (501) staff       (20)     1036 2022-01-25 15:55:09.000000 arrlio-0.9.0/arrlio/serializer/base.py
+-rw-r--r--   0 levsh      (501) staff       (20)     4336 2022-01-26 20:36:32.000000 arrlio-0.9.0/arrlio/serializer/json.py
+-rw-r--r--   0 levsh      (501) staff       (20)      818 2022-01-25 15:56:57.000000 arrlio-0.9.0/arrlio/serializer/nop.py
+-rw-r--r--   0 levsh      (501) staff       (20)     2339 2022-01-26 20:36:32.000000 arrlio-0.9.0/arrlio/settings.py
+-rw-r--r--   0 levsh      (501) staff       (20)     2263 2022-01-01 15:15:23.000000 arrlio-0.9.0/arrlio/tp.py
+-rw-r--r--   0 levsh      (501) staff       (20)     3628 2022-01-25 14:35:27.000000 arrlio-0.9.0/arrlio/utils.py
+drwxr-xr-x   0 levsh      (501) staff       (20)        0 2022-01-26 21:06:11.071881 arrlio-0.9.0/arrlio.egg-info/
+-rw-r--r--   0 levsh      (501) staff       (20)      471 2022-01-26 21:06:11.000000 arrlio-0.9.0/arrlio.egg-info/PKG-INFO
+-rw-r--r--   0 levsh      (501) staff       (20)      542 2022-01-26 21:06:11.000000 arrlio-0.9.0/arrlio.egg-info/SOURCES.txt
+-rw-r--r--   0 levsh      (501) staff       (20)        1 2022-01-26 21:06:11.000000 arrlio-0.9.0/arrlio.egg-info/dependency_links.txt
+-rw-r--r--   0 levsh      (501) staff       (20)       72 2022-01-26 21:06:11.000000 arrlio-0.9.0/arrlio.egg-info/requires.txt
+-rw-r--r--   0 levsh      (501) staff       (20)        7 2022-01-26 21:06:11.000000 arrlio-0.9.0/arrlio.egg-info/top_level.txt
+-rw-r--r--   0 levsh      (501) staff       (20)       38 2022-01-26 21:06:11.076407 arrlio-0.9.0/setup.cfg
+-rw-r--r--   0 levsh      (501) staff       (20)     1090 2022-01-01 18:45:29.000000 arrlio-0.9.0/setup.py
```

### Comparing `arrlio-0.8.0/LICENSE` & `arrlio-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `arrlio-0.8.0/arrlio/__init__.py` & `arrlio-0.9.0/arrlio/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 log_hndl = logging.StreamHandler(stream=sys.stderr)
 log_hndl.setFormatter(log_frmt)
 logger = logging.getLogger("arrlio")
 logger.addHandler(log_hndl)
 logger.setLevel("INFO")
 
 
-__version__ = "0.8.0"
+__version__ = "0.9.0"
 
 __tasks__ = {}
 
 
-from arrlio.core import Consumer, Producer, logger, task  # noqa
+from arrlio.core import App, logger, task  # noqa
 from arrlio.exc import NotFoundError, TaskError, TaskNoResultError, TaskTimeoutError  # noqa
 from arrlio.models import Graph  # noqa
-from arrlio.settings import ConsumerConfig, ProducerConfig  # noqa
+from arrlio.settings import Config  # noqa
```

### Comparing `arrlio-0.8.0/arrlio/backend/base.py` & `arrlio-0.9.0/arrlio/backends/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import asyncio
 import logging
 from types import MethodType
 from typing import List, Optional
 
 from pydantic import BaseSettings
 
-from arrlio.models import Message, TaskInstance, TaskResult
+from arrlio.models import Event, Message, TaskInstance, TaskResult
 from arrlio.serializer.base import Serializer
 from arrlio.tp import AsyncCallableT, SerializerT, TimeoutT
 
 
 logger = logging.getLogger("arrlio")
 
 
@@ -28,14 +28,15 @@
         self._tasks: set = set()
 
     def __repr__(self):
         return self.__str__()
 
     def _cancel_tasks(self):
         for task in self._tasks:
+            logger.debug("Cancel task %s", task)
             task.cancel()
 
     def task(method: MethodType):
         async def wrap(self, *args, **kwds):
             if self._closed.done():
                 raise Exception(f"Call {method} on closed {self}")
             task = asyncio.create_task(method(self, *args, **kwds))
@@ -54,14 +55,15 @@
     async def close(self):
         if self.is_closed:
             return
         self._closed.set_result(None)
         self._cancel_tasks()
         await self.stop_consume_tasks()
         await self.stop_consume_messages()
+        await self.stop_consume_events()
 
     @abc.abstractmethod
     async def send_task(self, task_instance: TaskInstance, **kwds):
         pass
 
     @abc.abstractmethod
     async def consume_tasks(self, queues: List[str], on_task: AsyncCallableT):
@@ -76,14 +78,26 @@
         pass
 
     @abc.abstractmethod
     async def pop_task_result(self, task_instance: TaskInstance) -> TaskResult:
         pass
 
     @abc.abstractmethod
+    async def push_event(self, task_instance: TaskInstance, event: Event):
+        pass
+
+    # @abc.abstractmethod
+    # async def consume_events(self, on_event: AsyncCallableT):
+    #     pass
+
+    # @abc.abstractmethod
+    # async def stop_consume_events(self):
+    #     pass
+
+    @abc.abstractmethod
     async def send_message(self, message: Message, encrypt: bool = None, **kwds):
         pass
 
     @abc.abstractmethod
     async def consume_messages(self, queues: List[str], on_message: AsyncCallableT):
         pass
```

### Comparing `arrlio-0.8.0/arrlio/backend/rabbitmq.py` & `arrlio-0.9.0/arrlio/backends/rabbitmq.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,48 +8,58 @@
 from uuid import UUID
 
 import aiormq
 import yarl
 from pydantic import Field
 
 from arrlio import core
-from arrlio.backend import base
+from arrlio.backends import base
 from arrlio.exc import TaskNoResultError
-from arrlio.models import Message, TaskInstance, TaskResult
+from arrlio.models import Event, Message, TaskInstance, TaskResult
 from arrlio.tp import AsyncCallableT, ExceptionFilterT, PositiveIntT, PriorityT, RMQDsn, SerializerT, TimeoutT
 from arrlio.utils import retry
 
 
 logger = logging.getLogger("arrlio")
 
 
 BACKEND_NAME: str = "arrlio"
 SERIALIZER: str = "arrlio.serializer.json.Json"
 URL: str = "amqp://guest:guest@localhost"
 TIMEOUT: int = 10
 RETRY_TIMEOUTS: Iterable[int] = None
 VERIFY_SSL: bool = True
-TASK_EXCHANGE: str = "arrlio"
-TASK_QUEUE_DURABLE: bool = False
-TASK_QUEUE_TTL: int = None
-TASK_PREFETCH_COUNT: int = 1
+TASKS_EXCHANGE: str = "arrlio"
+TASKS_QUEUE_DURABLE: bool = False
+TASKS_QUEUE_TTL: int = None
+TASKS_PREFETCH_COUNT: int = 1
+EVENTS_EXCHANGE: str = "arrlio"
+EVENTS_QUEUE_DURABLE: bool = False
+EVENTS_QUEUE: str = "arrlio.events"
+EVENTS_QUEUE_TTL: int = None
+EVENTS_PREFETCH_COUNT: int = 1
 MESSAGE_PREFETCH_COUNT: int = 1
 
 
 class BackendConfig(base.BackendConfig):
     name: Optional[str] = Field(default_factory=lambda: BACKEND_NAME)
     serializer: SerializerT = Field(default_factory=lambda: SERIALIZER)
     url: RMQDsn = Field(default_factory=lambda: URL)
     timeout: Optional[TimeoutT] = Field(default_factory=lambda: TIMEOUT)
     retry_timeouts: Optional[List] = Field(default_factory=lambda: RETRY_TIMEOUTS)
     verify_ssl: Optional[bool] = Field(default_factory=lambda: True)
-    task_exchange: str = Field(default_factory=lambda: TASK_EXCHANGE)
-    task_queue_durable: bool = Field(default_factory=lambda: TASK_QUEUE_DURABLE)
-    task_queue_ttl: Optional[PositiveIntT] = Field(default_factory=lambda: TASK_QUEUE_TTL)
-    task_prefetch_count: Optional[PositiveIntT] = Field(default_factory=lambda: TASK_PREFETCH_COUNT)
+    tasks_exchange: str = Field(default_factory=lambda: TASKS_EXCHANGE)
+    tasks_queue_durable: bool = Field(default_factory=lambda: TASKS_QUEUE_DURABLE)
+    tasks_queue_ttl: Optional[PositiveIntT] = Field(default_factory=lambda: TASKS_QUEUE_TTL)
+    tasks_prefetch_count: Optional[PositiveIntT] = Field(default_factory=lambda: TASKS_PREFETCH_COUNT)
+    events_exchange: str = Field(default_factory=lambda: EVENTS_EXCHANGE)
+    events_queue_durable: bool = Field(default_factory=lambda: EVENTS_QUEUE_DURABLE)
+    events_queue: str = Field(default_factory=lambda: EVENTS_QUEUE)
+    events_queue_ttl: Optional[PositiveIntT] = Field(default_factory=lambda: EVENTS_QUEUE_TTL)
+    events_prefetch_count: Optional[PositiveIntT] = Field(default_factory=lambda: EVENTS_PREFETCH_COUNT)
     message_prefetch_count: Optional[PositiveIntT] = Field(default_factory=lambda: MESSAGE_PREFETCH_COUNT)
 
     class Config:
         validate_assignment = True
         env_prefix = "ARRLIO_RMQ_BACKEND_"
 
 
@@ -168,14 +178,16 @@
         if self.is_open:
             return
 
         if self._on_open_callbacks_lock.locked():
             raise ConnectionError()
 
         async with self._conn_lock:
+            if self.is_open:
+                return
             if self.is_closed:
                 raise Exception("Can't reopen closed connection")
 
             if self._conn is None or self._conn.is_closed:
 
                 @retry(retry_timeouts=self._retry_timeouts, exc_filter=self._exc_filter)
                 async def connect():
@@ -228,23 +240,26 @@
 
 class Backend(base.Backend):
     def __init__(self, config: BackendConfig):
         super().__init__(config)
 
         self._task_consumers: Dict[str, Tuple[aiormq.Channel, aiormq.spec.Basic.ConsumeOk]] = {}
         self._message_consumers: Dict[str, Tuple[aiormq.Channel, aiormq.spec.Basic.ConsumeOk]] = {}
+        self._events_consumer: Tuple[aiormq.Channel, aiormq.spec.Basic.ConsumeOk] = []
         self._consume_lock: asyncio.Lock = asyncio.Lock()
 
         self.__conn: RMQConnection = RMQConnection(config.url, retry_timeouts=config.retry_timeouts)
 
         self.__conn.add_callback("on_open", id(self), "declare", self.declare)
         self.__conn.add_callback("on_lost", id(self), "cleanup", self._task_consumers.clear)
         self.__conn.add_callback("on_lost", id(self), "cleanup", self._message_consumers.clear)
-        self.__conn.add_callback("on_close", id(self), "cleanup", self.stop_consume_messages)
+        self.__conn.add_callback("on_lost", id(self), "cleanup", self._events_consumer.clear)
         self.__conn.add_callback("on_close", id(self), "cleanup", self.stop_consume_tasks)
+        self.__conn.add_callback("on_close", id(self), "cleanup", self.stop_consume_messages)
+        self.__conn.add_callback("on_close", id(self), "cleanup", self.stop_consume_events)
 
     def __del__(self):
         if not self.is_closed:
             logger.warning("Unclosed %s", self)
 
     def __str__(self):
         return f"[RMQBackend[{self.__conn}]]"
@@ -268,48 +283,71 @@
         await self.__conn.remove_callback_group(id(self))
         await self.__conn.close()
 
     @base.Backend.task
     async def declare(self):
         async with self._conn.channel_ctx() as channel:
             await channel.exchange_declare(
-                self.config.task_exchange,
+                self.config.tasks_exchange,
+                exchange_type="direct",
+                durable=False,
+                auto_delete=False,
+                timeout=self.config.timeout,
+            )
+            await channel.exchange_declare(
+                self.config.events_exchange,
                 exchange_type="direct",
                 durable=False,
                 auto_delete=False,
                 timeout=self.config.timeout,
             )
+            arguments = {}
+            if self.config.events_queue_ttl is not None:
+                arguments["x-message-ttl"] = self.config.events_queue_ttl * 1000
+            await channel.queue_declare(
+                self.config.events_queue,
+                durable=self.config.events_queue_durable,
+                auto_delete=not self.config.events_queue_durable,
+                arguments=arguments,
+                timeout=self.config.timeout,
+            )
+            await channel.queue_bind(
+                self.config.events_queue,
+                self.config.events_exchange,
+                routing_key=self.config.events_queue,
+                timeout=self.config.timeout,
+            )
 
     @base.Backend.task
     async def declare_task_queue(self, queue: str):
         async with self._conn.channel_ctx() as channel:
             arguments = {}
             arguments["x-max-priority"] = PriorityT.le
-            if self.config.task_queue_ttl is not None:
-                arguments["x-message-ttl"] = self.config.task_queue_ttl * 1000
-            durable = self.config.task_queue_durable
+            if self.config.tasks_queue_ttl is not None:
+                arguments["x-message-ttl"] = self.config.tasks_queue_ttl * 1000
+            durable = self.config.tasks_queue_durable
             await channel.queue_declare(
                 queue,
                 durable=durable,
                 auto_delete=not durable,
                 arguments=arguments,
                 timeout=self.config.timeout,
             )
-            await channel.queue_bind(queue, self.config.task_exchange, routing_key=queue, timeout=self.config.timeout)
+            await channel.queue_bind(queue, self.config.tasks_exchange, routing_key=queue, timeout=self.config.timeout)
 
     @base.Backend.task
     async def send_task(self, task_instance: TaskInstance, result_queue_durable: bool = False, **kwds):
         task_data = task_instance.data
         task_data.extra["result_queue_durable"] = result_queue_durable
         await self.declare_task_queue(task_data.queue)
         logger.debug("%s: put %s", self, task_instance)
         async with self._conn.channel_ctx() as channel:
             await channel.basic_publish(
                 self.serializer.dumps_task_instance(task_instance),
-                exchange=self.config.task_exchange,
+                exchange=self.config.tasks_exchange,
                 routing_key=task_data.queue,
                 properties=aiormq.spec.Basic.Properties(
                     delivery_mode=2,
                     message_id=str(task_data.task_id.hex),
                     timestamp=datetime.datetime.now(tz=datetime.timezone.utc),
                     expiration=str(int(task_data.ttl * 1000)) if task_data.ttl is not None else None,
                     priority=task_data.priority,
@@ -331,44 +369,41 @@
                         await channel.basic_ack(msg.delivery.delivery_tag)
                     await asyncio.shield(on_task(task_instance))
                     if ack_late:
                         await channel.basic_ack(msg.delivery.delivery_tag)
                 except Exception:
                     logger.exception("Internal error")
 
-            async with self._conn.channel_ctx() as channel:
-                await channel.basic_qos(prefetch_count=self.config.task_prefetch_count, timeout=timeout)
-
             for queue in queues:
                 if queue in self._task_consumers and not self._task_consumers[queue][0].is_closed:
                     continue
                 await self.declare_task_queue(queue)
                 channel = await self._conn.channel()
+                await channel.basic_qos(prefetch_count=self.config.tasks_prefetch_count, timeout=timeout)
                 self._task_consumers[queue] = [
                     channel,
                     await channel.basic_consume(queue, functools.partial(on_msg, channel), timeout=timeout),
                 ]
                 logger.debug("%s: consuming queue '%s'", self, queue)
 
             async def _consume_tasks():
                 await self.consume_tasks(list(self._task_consumers.keys()), on_task)
 
             self._conn.add_callback("on_lost", id(self), "consume_tasks", _consume_tasks)
 
     async def stop_consume_tasks(self):
         await self.__conn.remove_callback("on_lost", id(self), "consume_tasks")
+        await self.__conn.remove_callback("on_close", id(self), "consume_tasks")
         async with self._consume_lock:
-            try:
-                for queue, (channel, consume_ok) in self._task_consumers.items():
-                    if not self.__conn.is_closed and not channel.is_closed:
-                        logger.debug("%s: stop consuming queue '%s'", self, queue)
-                        await channel.basic_cancel(consume_ok.consumer_tag, timeout=self.config.timeout)
-                        await channel.close()
-            finally:
-                self._task_consumers = {}
+            for queue, (channel, consume_ok) in self._task_consumers.items():
+                if not self.__conn.is_closed and not channel.is_closed:
+                    logger.debug("%s: stop consuming queue '%s'", self, queue)
+                    await channel.basic_cancel(consume_ok.consumer_tag, timeout=self.config.timeout)
+                    await channel.close()
+            self._task_consumers = {}
 
     @base.Backend.task
     async def declare_result_queue(self, task_instance: TaskInstance):
         task_id = task_instance.data.task_id
         result_ttl = task_instance.data.result_ttl
         queue = routing_key = f"result.{task_id}"
         durable = task_instance.data.extra.get("result_queue_durable")
@@ -378,30 +413,30 @@
                 durable=durable,
                 auto_delete=not durable,
                 arguments={"x-expires": result_ttl * 1000} if result_ttl is not None else None,
                 timeout=self.config.timeout,
             )
             await channel.queue_bind(
                 queue,
-                self.config.task_exchange,
+                self.config.tasks_exchange,
                 routing_key=routing_key,
                 timeout=self.config.timeout,
             )
         return queue
 
     @base.Backend.task
     async def push_task_result(self, task_instance: core.TaskInstance, task_result: TaskResult):
         if not task_instance.task.result_return:
             raise TaskNoResultError(task_instance.data.task_id)
         routing_key = await self.declare_result_queue(task_instance)
         logger.debug("%s: push result for %s", self, task_instance)
         async with self._conn.channel_ctx() as channel:
             await channel.basic_publish(
                 self.serializer.dumps_task_result(task_result, encrypt=task_instance.data.result_encrypt),
-                exchange=self.config.task_exchange,
+                exchange=self.config.tasks_exchange,
                 routing_key=routing_key,
                 properties=aiormq.spec.Basic.Properties(
                     delivery_mode=2,
                     timestamp=datetime.datetime.now(tz=datetime.timezone.utc),
                 ),
                 timeout=self.config.timeout,
             )
@@ -499,36 +534,101 @@
                         await channel.basic_ack(msg.delivery.delivery_tag)
                     await asyncio.shield(on_message(message))
                     if ack_late:
                         await channel.basic_ack(msg.delivery.delivery_tag)
                 except Exception:
                     logger.exception("Internal error")
 
-            async with self._conn.channel_ctx() as channel:
-                await channel.basic_qos(prefetch_count=self.config.message_prefetch_count, timeout=timeout)
-
             for queue in queues:
                 if queue in self._message_consumers and not self._message_consumers[queue][0].is_closed:
                     continue
                 channel = await self._conn.channel()
+                await channel.basic_qos(prefetch_count=self.config.message_prefetch_count, timeout=timeout)
                 self._message_consumers[queue] = [
                     channel,
                     await channel.basic_consume(queue, functools.partial(on_msg, channel), timeout=timeout),
                 ]
                 logger.debug("%s: consuming messages queue '%s'", self, queue)
 
             async def _consume_messages():
                 await self.consume_messages(list(self._message_consumers.keys()), on_message)
 
             self._conn.add_callback("on_lost", id(self), "consume_messages", _consume_messages)
 
     async def stop_consume_messages(self):
         await self.__conn.remove_callback("on_lost", id(self), "consume_messages")
+        await self.__conn.remove_callback("on_close", id(self), "consume_messages")
         async with self._consume_lock:
-            try:
-                for queue, (channel, consume_ok) in self._message_consumers.items():
-                    if not self.__conn.is_closed and not channel.is_closed:
-                        logger.debug("%s: stop consuming messages queue '%s'", self, queue)
-                        await channel.basic_cancel(consume_ok.consumer_tag, timeout=self.config.timeout)
-                        await channel.close()
-            finally:
-                self._message_consumers = {}
+            for queue, (channel, consume_ok) in self._message_consumers.items():
+                if not self.__conn.is_closed and not channel.is_closed:
+                    logger.debug("%s: stop consuming messages queue '%s'", self, queue)
+                    await channel.basic_cancel(consume_ok.consumer_tag, timeout=self.config.timeout)
+                    await channel.close()
+            self._message_consumers = {}
+
+    @base.Backend.task
+    async def push_event(self, task_instance: TaskInstance, event: Event):
+        if not task_instance.data.events:
+            return
+        async with self._conn.channel_ctx() as channel:
+            await channel.basic_publish(
+                self.serializer.dumps_event(event),
+                exchange=self.config.events_exchange,
+                routing_key=self.config.events_queue,
+                properties=aiormq.spec.Basic.Properties(
+                    delivery_mode=2,
+                    timestamp=datetime.datetime.now(tz=datetime.timezone.utc),
+                ),
+                timeout=self.config.timeout,
+            )
+
+    @base.Backend.task
+    async def consume_events(self, on_event: AsyncCallableT):
+        async with self._consume_lock:
+            timeout = self.config.timeout
+
+            async def on_msg(channel: aiormq.Channel, msg):
+                try:
+                    event = self.serializer.loads_event(msg.body)
+                    logger.debug("%s: got %s", self, event)
+                    # ack_late = event.ack_late
+                    ack_late = False
+                    if not ack_late:
+                        await channel.basic_ack(msg.delivery.delivery_tag)
+                    await asyncio.shield(on_event(event))
+                    if ack_late:
+                        await channel.basic_ack(msg.delivery.delivery_tag)
+                except Exception:
+                    logger.exception("Internal error")
+
+                if self._events_consumer and not self._events_consumer[0].is_closed:
+                    return
+
+            channel = await self._conn.channel()
+            await channel.basic_qos(prefetch_count=self.config.events_prefetch_count, timeout=timeout)
+            self._events_consumer = [
+                channel,
+                await channel.basic_consume(
+                    self.config.events_queue,
+                    functools.partial(on_msg, channel),
+                    timeout=timeout,
+                ),
+            ]
+            logger.debug("%s: consuming events queue '%s'", self, self.config.events_queue)
+
+            async def _consume_events():
+                await self.consume_events(on_event)
+
+            self._conn.add_callback("on_lost", id(self), "consume_events", _consume_events)
+
+    async def stop_consume_events(self):
+        await self.__conn.remove_callback("on_lost", id(self), "consume_events")
+        await self.__conn.remove_callback("on_close", id(self), "consume_events")
+        async with self._consume_lock:
+            if not self._events_consumer:
+                return
+            channel, consume_ok = self._events_consumer
+            if not self.__conn.is_closed and not channel.is_closed:
+                logger.debug("%s: stop consuming events queue '%s'", self, self.config.events_queue)
+                await channel.basic_cancel(consume_ok.consumer_tag, timeout=self.config.timeout)
+                await channel.close()
+            self._events_consumer = []
```

### Comparing `arrlio-0.8.0/arrlio/backend/redis.py` & `arrlio-0.9.0/arrlio/backends/redis.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import asyncio
 import dataclasses
 import itertools
 import logging
-from typing import Iterable, List, Optional
+from typing import Dict, Iterable, List, Optional
 
 import siderpy
 from pydantic import Field
 
 from arrlio import core
-from arrlio.backend import base
+from arrlio.backends import base
 from arrlio.exc import TaskNoResultError
-from arrlio.models import Message, TaskInstance, TaskResult
+from arrlio.models import Event, Message, TaskInstance, TaskResult
 from arrlio.tp import AsyncCallableT, PositiveIntT, RedisDsn, SerializerT, TimeoutT
 
 
 logger = logging.getLogger("arrlio")
 
 
 BACKEND_NAME: str = "arrlio"
@@ -47,16 +47,17 @@
         super().__init__(config)
         self.redis_pool = siderpy.RedisPool(
             config.url.get_secret_value(),
             connect_timeout=config.connect_timeout,
             timeout=config.timeout,
             size=config.pool_size,
         )
-        self._task_consumers = {}
-        self._message_consumers = {}
+        self._task_consumers: Dict[str, asyncio.Task] = {}
+        self._message_consumers: Dict[str, asyncio.Task] = {}
+        self._events_consumer: asyncio.Task = None
 
     def __str__(self):
         return f"[RedisBackend[{self.redis_pool}]]"
 
     async def close(self):
         await super().close()
         await self.redis_pool.close()
@@ -88,15 +89,15 @@
 
     @base.Backend.task
     async def consume_tasks(self, queues: List[str], on_task: AsyncCallableT):
         async def consume_queue(queue):
             queue_key = self._make_task_queue_key(queue)
             while True:
                 try:
-                    logger.debug("%s: consuming task queue '%s'", self, queue)
+                    logger.debug("%s: consuming tasks queue '%s'", self, queue)
                     _, queue_value = await self.redis_pool.blpop(queue_key, 0)
                     priority, task_id = queue_value.decode().split("|")
                     serialized_data = await self.redis_pool.get(task_id)
                     if serialized_data is None:
                         continue
                     task_instance = self.serializer.loads_task_instance(serialized_data)
                     await asyncio.shield(on_task(task_instance))
@@ -115,16 +116,16 @@
                 except Exception:
                     logger.exception("Internal error")
 
         for queue in queues:
             self._task_consumers[queue] = asyncio.create_task(consume_queue(queue))
 
     async def stop_consume_tasks(self):
-        for queue, task in self._task_consumers.items():
-            task.cancel()
+        for queue in self._task_consumers.keys():
+            self._task_consumers[queue].cancel()
         self._task_consumers = {}
 
     @base.Backend.task
     async def push_task_result(self, task_instance: core.TaskInstance, task_result: TaskResult):
         if not task_instance.task.result_return:
             raise TaskNoResultError(task_instance.data.task_id)
         result_key = self._make_result_key(task_instance.data.task_id)
@@ -164,15 +165,15 @@
 
     @base.Backend.task
     async def consume_messages(self, queues: List[str], on_message: AsyncCallableT):
         async def consume_queue(queue):
             queue_key = self._make_message_queue_key(queue)
             while True:
                 try:
-                    logger.debug("%s: consuming message queue '%s'", self, queue)
+                    logger.debug("%s: consuming messages queue '%s'", self, queue)
                     _, queue_value = await self.redis_pool.blpop(queue_key, 0)
                     priority, message_id = queue_value.decode().split("|")
                     serialized_data = await self.redis_pool.get(message_id)
                     if serialized_data is None:
                         continue
                     data = self.serializer.loads(serialized_data)
                     message = Message(**data)
@@ -193,10 +194,63 @@
                 except Exception:
                     logger.exception("Internal error")
 
         for queue in queues:
             self._message_consumers[queue] = asyncio.create_task(consume_queue(queue))
 
     async def stop_consume_messages(self):
-        for queue, task in self._message_consumers.items():
-            task.cancel()
+        for queue in self._message_consumers.keys():
+            self._message_consumers[queue].cancel()
         self._message_consumers = {}
+
+    @base.Backend.task
+    async def push_event(self, task_instance: core.TaskInstance, event: Event):
+        if not task_instance.data.events:
+            return
+
+        queue_key = "arrlio.events"
+        data = self.serializer.dumps_event(event)
+
+        async with self.redis_pool.get_redis() as redis:
+            with redis.pipeline():
+                await redis.multi()
+                await redis.setex(f"{event.event_id}", task_instance.data.event_ttl, data)
+                await redis.rpush(queue_key, f"{event.event_id}")
+                await redis.execute()
+                await redis.pipeline_execute()
+
+    @base.Backend.task
+    async def consume_events(self, on_event: AsyncCallableT):
+        async def consume_queue():
+            queue_key = "arrlio.events"
+            while True:
+                try:
+                    logger.debug("%s: consuming events")
+                    _, queue_value = await self.redis_pool.blpop(queue_key, 0)
+                    event_id = queue_value.decode()
+                    serialized_data = await self.redis_pool.get(event_id)
+                    if serialized_data is None:
+                        continue
+                    event = self.serializer.loads_event(serialized_data)
+                    logger.debug("%s: got %s", self, event)
+                    await asyncio.shield(on_event(event))
+                except asyncio.CancelledError:
+                    logger.info("%s: stop consume events")
+                    break
+                except (ConnectionError, TimeoutError) as e:
+                    logger.error("%s: %s %s", self, e.__class__, e)
+                    retry_timeouts = (
+                        iter(self.config.retry_timeouts) if self.config.retry_timeouts else itertools.repeat(1)
+                    )
+                    seconds = next(retry_timeouts, None)
+                    if seconds is None:
+                        raise e
+                    await asyncio.sleep(seconds)
+                except Exception:
+                    logger.exception("Internal error")
+
+        self._events_consumer = asyncio.create_task(consume_queue())
+
+    async def stop_consume_events(self):
+        if self._events_consumer:
+            self._events_consumer.cancel()
+        self._events_consumer = None
```

### Comparing `arrlio-0.8.0/arrlio/core.py` & `arrlio-0.9.0/arrlio/core.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import asyncio
+import copy
+import datetime
 import inspect
 import logging
 import sys
 import threading
 import time
 from types import FunctionType, MethodType
-from typing import Any, Dict, List, Tuple, Union
+from typing import Any, List, Tuple, Union
 from uuid import UUID
 
 from arrlio import __tasks__, settings
 from arrlio.exc import NotFoundError, TaskError, TaskNoResultError, TaskTimeoutError
-from arrlio.models import Graph, Message, Task, TaskData, TaskInstance, TaskResult
-from arrlio.settings import ConsumerConfig, ProducerConfig
+from arrlio.models import Event, Graph, Message, Task, TaskData, TaskInstance, TaskResult
+from arrlio.settings import Config
 
 
 logger = logging.getLogger("arrlio")
 
 
 def task(
     func: FunctionType = None,
@@ -27,14 +29,16 @@
     timeout: int = None,
     ttl: int = None,
     ack_late: bool = None,
     result_ttl: int = None,
     result_return: bool = None,
     result_encrypt: bool = None,
     thread: bool = None,
+    events: bool = None,
+    event_ttl: int = None,
 ) -> Task:
 
     if bind is None:
         bind = settings.TASK_BIND
     if base is None:
         base = Task
     if queue is None:
@@ -44,19 +48,21 @@
     if timeout is None:
         timeout = settings.TASK_TIMEOUT
     if ttl is None:
         ttl = settings.TASK_TTL
     if ack_late is None:
         ack_late = settings.TASK_ACK_LATE
     if result_ttl is None:
-        result_ttl = settings.RESULT_TTL
+        result_ttl = settings.TASK_RESULT_TTL
     if result_return is None:
-        result_return = settings.RESULT_RETURN
-    if result_encrypt is None:
-        result_encrypt = settings.RESULT_ENCRYPT
+        result_return = settings.TASK_RESULT_RETURN
+    if events is None:
+        events = settings.EVENTS
+    if event_ttl is None:
+        event_ttl = settings.EVENT_TTL
 
     if func is not None:
         if not isinstance(func, (FunctionType, MethodType)):
             raise TypeError("Argument 'func' does not a function or method")
         if name is None:
             name = f"{func.__module__}.{func.__name__}"
         if name in __tasks__:
@@ -70,14 +76,16 @@
             timeout=timeout,
             ttl=ttl,
             ack_late=ack_late,
             result_ttl=result_ttl,
             result_return=result_return,
             result_encrypt=result_encrypt,
             thread=thread,
+            events=events,
+            event_ttl=event_ttl,
         )
         __tasks__[name] = t
         logger.info("Register %s", t)
         return t
     else:
 
         def wrapper(func):
@@ -91,272 +99,304 @@
                 timeout=timeout,
                 ttl=ttl,
                 ack_late=ack_late,
                 result_ttl=result_ttl,
                 result_return=result_return,
                 result_encrypt=result_encrypt,
                 thread=thread,
+                events=events,
+                event_ttl=event_ttl,
             )
 
         return wrapper
 
 
-class Base:
-    def __init__(self, config: Union[ProducerConfig, ConsumerConfig], backend_config_kwds: dict = None):
+class Executor:
+    def __str__(self):
+        return f"[{self.__class__.__name__}]"
+
+    def __repr__(self):
+        return self.__str__()
+
+    async def __call__(self, task_instance: TaskInstance) -> TaskResult:
+        task_data: TaskData = task_instance.data
+        task: Task = task_instance.task
+
+        res, exc, trb = None, None, None
+        t0 = time.monotonic()
+
+        logger.info("%s: execute task %s(%s)", self, task.name, task_data.task_id)
+
+        try:
+            if task_instance.task.func is None:
+                raise NotFoundError(f"Task '{task_instance.task.name}' not found")
+            try:
+                if inspect.iscoroutinefunction(task_instance.task.func):
+                    res = await asyncio.wait_for(task_instance(), task_data.timeout)
+                else:
+                    res = task_instance()
+            except asyncio.TimeoutError:
+                raise TaskTimeoutError(task_data.timeout)
+        except Exception as e:
+            exc_info = sys.exc_info()
+            exc = exc_info[1]
+            trb = exc_info[2]
+            if isinstance(e, TaskTimeoutError):
+                logger.error("Task timeout for %s", task_instance)
+            else:
+                logger.exception("%s: %s", self, task_instance)
+
+        logger.info(
+            "%s: task %s(%s) done in %.2f second(s)",
+            self,
+            task.name,
+            task_data.task_id,
+            time.monotonic() - t0,
+        )
+
+        return TaskResult(res=res, exc=exc, trb=trb)
+
+
+class ThreadExecutor(Executor):
+    async def __call__(self, task_instance: TaskInstance) -> TaskResult:
+        root_loop = asyncio.get_running_loop()
+        done_ev: asyncio.Event = asyncio.Event()
+        task_result: TaskResult = None
+
+        def thread():
+            nonlocal done_ev
+            nonlocal task_result
+            loop = asyncio.new_event_loop()
+            try:
+                asyncio.set_event_loop(loop)
+                task_result = loop.run_until_complete(super(ThreadExecutor, self).__call__(task_instance))
+            finally:
+                loop.run_until_complete(loop.shutdown_asyncgens())
+                loop.close()
+                root_loop.call_soon_threadsafe(lambda: done_ev.set())
+
+        th = threading.Thread(target=thread)
+        th.start()
+
+        await done_ev.wait()
+
+        return task_result
+
+
+class App:
+    def __init__(self, config: Config, backend_config_kwds: dict = None):
         self.config = config
-        backend_config_kwds = backend_config_kwds or {}
-        self.backend = self.config.backend.Backend(self.config.backend.BackendConfig(**(backend_config_kwds)))
+        self._backend = self.config.backend.Backend(self.config.backend.BackendConfig(**(backend_config_kwds or {})))
         self._closed: asyncio.Future = asyncio.Future()
+        self._running_tasks: dict = {}
+        self._running_messages: dict = {}
+        self._lock: asyncio.Lock = asyncio.Lock()
 
     def __str__(self):
-        return f"[{self.__class__.__name__}{self.backend}]"
+        return f"[{self.__class__.__name__}{self._backend}]"
 
     def __repr__(self):
         return self.__str__()
 
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.close()
 
     @property
+    def backend(self):
+        return self._backend
+
+    @property
     def is_closed(self):
         return self._closed.done()
 
     async def close(self):
-        await self.backend.close()
+        await self.stop_consume_tasks()
+        await self.stop_consume_messages()
+        await self.stop_consume_events()
+        await self._backend.close()
         self._closed.set_result(None)
 
-
-class Producer(Base):
-    def __init__(self, config: ProducerConfig, backend_config_kwds: dict = None):
-        super().__init__(config, backend_config_kwds=backend_config_kwds)
-
-    async def send_task(
+    async def run_task(
         self,
         task: Union[Task, str],
         args: tuple = None,
         kwds: dict = None,
         queue: str = None,
         priority: int = None,
         timeout: int = None,
         ttl: int = None,
         encrypt: bool = None,
         ack_late: bool = None,
         result_ttl: int = None,
         result_return: bool = None,
         result_encrypt: bool = None,
         thread: bool = None,
+        events: bool = None,
+        event_ttl: int = None,
         extra: dict = None,
         **kwargs,
     ) -> "AsyncResult":
         name = task
         if isinstance(task, Task):
             name = task.name
 
         if args is None:
             args = ()
         if kwds is None:
             kwds = {}
         if extra is None:
             extra = {}
 
+        settings = self.config.task.dict(exclude_unset=True)
+
+        if queue is None:
+            queue = settings.get("queue")
+        if priority is None:
+            priority = settings.get("priority")
+        if timeout is None:
+            timeout = settings.get("timeout")
+        if ttl is None:
+            ttl = settings.get("ttl")
+        if ack_late is None:
+            ack_late = settings.get("ack_late")
+        if result_ttl is None:
+            result_ttl = settings.get("result_ttl")
+        if result_return is None:
+            result_return = settings.get("result_return")
+        if events is None:
+            events = settings.get("events")
+        if event_ttl is None:
+            event_ttl = settings.get("event_ttl")
+
         task_data = TaskData(
             args=args,
             kwds=kwds,
             queue=queue,
             priority=priority,
             timeout=timeout,
             ttl=ttl,
             encrypt=encrypt,
             ack_late=ack_late,
             result_ttl=result_ttl,
             result_return=result_return,
             result_encrypt=result_encrypt,
             thread=thread,
+            events=events,
+            event_ttl=event_ttl,
             extra=extra,
         )
 
         if name in __tasks__:
             task_instance = __tasks__[name].instantiate(data=task_data)
         else:
             task_instance = Task(None, name).instantiate(data=task_data)
 
-        logger.info("%s: send %s", self, task_instance)
+        logger.info("%s: run %s", self, task_instance)
 
-        await self.backend.send_task(task_instance, **kwargs)
+        await self._backend.send_task(task_instance, **kwargs)
 
         return AsyncResult(self, task_instance)
 
-    async def send_graph(self, graph: Graph, args: Union[Tuple, List] = None, kwds: dict = None):
-        logger.info("%s: send %s with args: %s and kwds: %s", self, graph, args, kwds)
-
-        for root in graph.roots:
-            name, root_kwds = graph.nodes[root]
-
-            task_data = TaskData(**root_kwds)
-            task_data.args += tuple(args or ())
-            task_data.kwds.update(kwds or {})
-            task_data.graph = Graph(graph.id, nodes=graph.nodes, edges=graph.edges, roots={root})
-
-            if name in __tasks__:
-                task_instance = __tasks__[name].instantiate(data=task_data)
+    async def run_graph(self, graph: Graph, args: Union[Tuple, List] = None, kwds: dict = None):
+        nodes = copy.deepcopy(graph.nodes)
+        edges = graph.edges
+        roots = graph.roots
+
+        if not nodes or not roots:
+            return
+
+        logger.info("%s: run %s with args: %s and kwds: %s", self, graph, args, kwds)
+
+        task_instances = {}
+        for node_name, (task, node_kwds) in nodes.items():
+            task_data = TaskData(**node_kwds)
+            node_kwds["task_id"] = task_data.task_id
+            if task in __tasks__:
+                task_instance = __tasks__[task].instantiate(data=task_data)
             else:
-                task_instance = Task(None, name).instantiate(data=task_data)
+                task_instance = Task(None, task).instantiate(data=task_data)
+            task_instances[node_name] = task_instance
 
-            logger.info("%s: send %s", self, task_instance)
+        for root in roots:
+            task_instances[root].data.args += tuple(args or ())
+            task_instances[root].data.kwds.update(kwds or {})
+            task_instances[root].data.graph = Graph(graph.id, nodes=nodes, edges=edges, roots={root})
+            logger.info("%s: run %s", self, task_instances[root])
+            await self._backend.send_task(task_instances[root])
 
-            await self.backend.send_task(task_instance)
+        return {k: AsyncResult(self, task_instance) for k, task_instance in task_instances.items()}
 
     async def send_message(
         self,
         message: Any,
         exchange: str = None,
         routing_key: str = None,
         priority: int = None,
         ttl: int = None,
+        ack_late: bool = None,
         encrypt: bool = None,
     ):
-        message = Message(exchange=exchange, data=message, priority=priority, ttl=ttl)
+        settings = self.config.message.dict(exclude_unset=True)
+
+        if exchange is None:
+            exchange = settings.get("exchange")
+        if priority is None:
+            priority = settings.get("priority")
+        if ttl is None:
+            ttl = settings.get("ttl")
+        if ack_late is None:
+            ack_late = settings.get("ack_late")
+
+        message = Message(exchange=exchange, data=message, priority=priority, ttl=ttl, ack_late=ack_late)
         logger.info("%s: send %s", self, message)
-        await self.backend.send_message(message, routing_key=routing_key, encrypt=encrypt)
+        await self._backend.send_message(message, routing_key=routing_key, encrypt=encrypt)
 
     async def pop_result(self, task_instance: TaskInstance):
-        task_result = await self.backend.pop_task_result(task_instance)
+        task_result = await self._backend.pop_task_result(task_instance)
         if task_result.exc:
             if isinstance(task_result.exc, TaskError):
                 raise task_result.exc
             else:
                 raise TaskError(task_result.exc, task_result.trb)
         return task_result.res
 
-
-class Executor:
-    def __str__(self):
-        return f"[{self.__class__.__name__}]"
-
-    def __repr__(self):
-        return self.__str__()
-
-    async def __call__(self, task_instance: TaskInstance) -> TaskResult:
-        task_data: TaskData = task_instance.data
-        task: Task = task_instance.task
-
-        res, exc, trb = None, None, None
-        t0 = time.monotonic()
-
-        logger.info("%s: execute task %s(%s)", self, task.name, task_data.task_id)
-
-        try:
-            if task_instance.task.func is None:
-                raise NotFoundError(f"Task '{task_instance.task.name}' not found")
-            try:
-                if inspect.iscoroutinefunction(task_instance.task.func):
-                    res = await asyncio.wait_for(task_instance(), task_data.timeout)
-                else:
-                    res = task_instance()
-            except asyncio.TimeoutError:
-                raise TaskTimeoutError(task_data.timeout)
-        except Exception as e:
-            exc_info = sys.exc_info()
-            exc = exc_info[1]
-            trb = exc_info[2]
-            if isinstance(e, TaskTimeoutError):
-                logger.error("Task timeout for %s", task_instance)
-            else:
-                logger.exception("%s: %s", self, task_instance)
-
-        logger.info(
-            "%s: task %s(%s) done in %.2f second(s)",
-            self,
-            task.name,
-            task_data.task_id,
-            time.monotonic() - t0,
-        )
-
-        return TaskResult(res=res, exc=exc, trb=trb)
-
-
-class ThreadExecutor(Executor):
-    async def __call__(self, task_instance: TaskInstance) -> TaskResult:
-        root_loop = asyncio.get_running_loop()
-        done_ev: asyncio.Event = asyncio.Event()
-        task_result: TaskResult = None
-
-        def thread():
-            nonlocal done_ev
-            nonlocal task_result
-            loop = asyncio.new_event_loop()
-            try:
-                asyncio.set_event_loop(loop)
-                task_result = loop.run_until_complete(super(ThreadExecutor, self).__call__(task_instance))
-            finally:
-                loop.run_until_complete(loop.shutdown_asyncgens())
-                loop.close()
-                root_loop.call_soon_threadsafe(lambda: done_ev.set())
-
-        th = threading.Thread(target=thread)
-        th.start()
-
-        await done_ev.wait()
-
-        return task_result
-
-
-class Consumer(Base):
-    def __init__(self, config: ConsumerConfig, backend_config_kwds: dict = None, on_message=None):
-        super().__init__(config, backend_config_kwds=backend_config_kwds)
-        self.producer = Producer(
-            ProducerConfig(**{k: v for k, v in config.dict().items() if k in ProducerConfig.__fields__}),
-            backend_config_kwds=backend_config_kwds,
-        )
-
-        if on_message:
-            self.on_message = on_message
-
-        self._running_tasks: dict = {}
-        self._running_messages: dict = {}
-        self._lock: asyncio.Lock = asyncio.Lock()
-
-    async def close(self):
-        await self.stop_consume_tasks()
-        await self.stop_consume_messages()
-        await super().close()
-
     async def consume_tasks(self):
         if self.config.task_queues:
             logger.info("%s: consuming task queues %s", self, self.config.task_queues)
-            await self.backend.consume_tasks(self.config.task_queues, self._on_task)
+            await self._backend.consume_tasks(self.config.task_queues, self._on_task)
 
     async def stop_consume_tasks(self):
         async with self._lock:
+            await self._backend.stop_consume_tasks()
             for task_id, aio_task in self._running_tasks.items():
                 logger.debug("Cancel processing task '%s'", task_id)
                 aio_task.cancel()
             self._running_tasks = {}
 
     async def _on_task(self, task_instance: TaskInstance):
         try:
             task_id: UUID = task_instance.data.task_id
 
             async with self._lock:
                 if self.is_closed:
                     return
 
                 if len(self._running_tasks) + len(self._running_messages) + 1 >= self.config.pool_size:
-                    await self.backend.stop_consume_tasks()
+                    await self._backend.stop_consume_tasks()
                     try:
                         aio_task = asyncio.create_task(self._execute_task(task_instance))
                         aio_task.add_done_callback(lambda *args: self._running_tasks.pop(task_id, None))
                         self._running_tasks[task_id] = aio_task
                         await aio_task
                     finally:
                         if not self.is_closed:
-                            await self.backend.consume_tasks(self.config.task_queues, self._on_task)
+                            await self._backend.consume_tasks(self.config.task_queues, self._on_task)
                     return
 
             aio_task = asyncio.create_task(self._execute_task(task_instance))
             aio_task.add_done_callback(lambda *args: self._running_tasks.pop(task_id, None))
             self._running_tasks[task_id] = aio_task
 
         except Exception as e:
@@ -381,74 +421,94 @@
                         for child in graph.edges[root]:
                             graph: Graph = Graph(
                                 id=graph.id,
                                 nodes=graph.nodes,
                                 edges=graph.edges,
                                 roots={child},
                             )
-                            await self.producer.send_graph(
+                            await self.run_graph(
                                 graph,
                                 args=(task_result.res,),
                                 kwds={"graph_source_node": root},
                             )
 
             if task_instance.data.result_return:
                 try:
-                    await self.backend.push_task_result(task_instance, task_result)
+                    await self._backend.push_task_result(task_instance, task_result)
+                except Exception as e:
+                    logger.exception(e)
+
+            if task_instance.data.events:
+                event: Event = Event(
+                    type="task done",
+                    datetime=datetime.datetime.now(tz=datetime.timezone.utc),
+                    data={
+                        "task_id": task_instance.data.task_id,
+                        "status": task_result.exc is None,
+                    },
+                )
+                try:
+                    await self._backend.push_event(task_instance, event)
                 except Exception as e:
                     logger.exception(e)
 
         except asyncio.CancelledError:
             pass
         except Exception as e:
             logger.exception(e)
 
-    async def consume_messages(self):
+    async def consume_messages(self, on_message):
         if self.config.message_queues:
+
+            async def handle(message: Message):
+                try:
+                    message_id: UUID = message.message_id
+
+                    async with self._lock:
+                        if len(self._running_tasks) + len(self._running_messages) + 1 >= self.config.pool_size:
+                            await self._backend.stop_consume_messages()
+                            try:
+                                aio_task = asyncio.create_task(on_message(message.data))
+                                aio_task.add_done_callback(lambda *args: self._running_messages.pop(message_id, None))
+                                self._running_tasks[message_id] = aio_task
+                                await aio_task
+                            finally:
+                                if not self.is_closed:
+                                    await self._backend.consume_messages(self.config.message_queues, handle)
+                            return
+
+                    aio_task = asyncio.create_task(on_message(message.data))
+                    aio_task.add_done_callback(lambda *args: self._running_messages.pop(message_id, None))
+                    self._running_messages[message_id] = aio_task
+
+                except Exception as e:
+                    logger.exception(e)
+
             logger.info("%s: consuming message queues %s", self, self.config.message_queues)
-            await self.backend.consume_messages(self.config.message_queues, self._on_message)
+            await self._backend.consume_messages(self.config.message_queues, handle)
 
     async def stop_consume_messages(self):
         async with self._lock:
+            await self._backend.stop_consume_messages()
             for message_id, aio_task in self._running_messages.items():
                 logger.debug("Cancel processing message '%s'", message_id)
                 aio_task.cancel()
             self._running_messages = {}
 
-    async def on_message(self, message: Any):
-        pass
-
-    async def _on_message(self, message: Message):
-        try:
-            message_id: UUID = message.message_id
-
-            async with self._lock:
-                if len(self._running_tasks) + len(self._running_messages) + 1 >= self.config.pool_size:
-                    await self.backend.stop_consume_messages()
-                    try:
-                        aio_task = asyncio.create_task(self.on_message(message.data))
-                        aio_task.add_done_callback(lambda *args: self._running_tasks.pop(message_id, None))
-                        self._running_tasks[message_id] = aio_task
-                        await aio_task
-                    finally:
-                        if not self.is_closed:
-                            await self.backend.consume_messages(self.config.message_queues, self._on_message)
-                    return
+    async def consume_events(self, on_event):
+        logger.info("%s: consuming events", self)
+        await self._backend.consume_events(on_event)
 
-            aio_task = asyncio.create_task(self.on_message(message.data))
-            aio_task.add_done_callback(lambda *args: self._running_messages.pop(message_id, None))
-            self._running_messages[message_id] = aio_task
-
-        except Exception as e:
-            logger.exception(e)
+    async def stop_consume_events(self):
+        await self._backend.stop_consume_events()
 
 
 class AsyncResult:
-    def __init__(self, producer: Producer, task_instance: TaskInstance):
-        self._producer = producer
+    def __init__(self, app: App, task_instance: TaskInstance):
+        self._app = app
         self._task_instance = task_instance
         self._result = None
         self._exception: Exception = None
         self._ready: bool = False
 
     @property
     def task_instance(self) -> TaskInstance:
@@ -467,15 +527,15 @@
         return self._ready
 
     async def get(self):
         if not self._task_instance.data.result_return:
             raise TaskNoResultError(self._task_instance.data.task_id)
         if not self._ready:
             try:
-                self._result = await self._producer.pop_result(self._task_instance)
+                self._result = await self._app.pop_result(self._task_instance)
                 self._ready = True
             except TaskError as e:
                 self._exception = e
                 self._ready = True
         if self._exception:
             if isinstance(self._exception.args[0], Exception):
                 raise self._exception from self._exception.args[0]
```

### Comparing `arrlio-0.8.0/arrlio/crypto.py` & `arrlio-0.9.0/arrlio/crypto.py`

 * *Files identical despite different names*

### Comparing `arrlio-0.8.0/arrlio/models.py` & `arrlio-0.9.0/arrlio/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,28 @@
+import datetime
 from dataclasses import dataclass, field
 from types import FunctionType, TracebackType
 from typing import Any, Dict, List, Set, Tuple, Union
 from uuid import UUID, uuid4
 
 from roview import rodict, roset
 
 from arrlio.settings import (
+    EVENT_TTL,
+    EVENTS,
     MESSAGE_ACK_LATE,
     MESSAGE_EXCHANGE,
     MESSAGE_PRIORITY,
     MESSAGE_TTL,
-    RESULT_ENCRYPT,
-    RESULT_RETURN,
-    RESULT_TTL,
     TASK_ACK_LATE,
     TASK_BIND,
     TASK_PRIORITY,
     TASK_QUEUE,
+    TASK_RESULT_RETURN,
+    TASK_RESULT_TTL,
     TASK_TIMEOUT,
     TASK_TTL,
 )
 
 
 @dataclass
 class TaskData:
@@ -33,14 +35,16 @@
     ttl: int = None
     encrypt: bool = None
     ack_late: bool = None
     result_ttl: int = None
     result_return: bool = None
     result_encrypt: bool = None
     thread: bool = None
+    events: bool = None
+    event_ttl: int = None
     extra: dict = field(default_factory=dict)
     graph: "Graph" = None
 
 
 @dataclass(frozen=True)
 class Task:
     func: FunctionType
@@ -52,14 +56,16 @@
     ttl: int = None
     encrypt: bool = None
     ack_late: bool = None
     result_ttl: int = None
     result_return: bool = None
     result_encrypt: bool = None
     thread: bool = None
+    events: bool = None
+    event_ttl: int = None
 
     def __post_init__(self):
         if self.bind is None:
             object.__setattr__(self, "bind", TASK_BIND)
         if self.queue is None:
             object.__setattr__(self, "queue", TASK_QUEUE)
         if self.priority is None:
@@ -67,19 +73,21 @@
         if self.timeout is None:
             object.__setattr__(self, "timeout", TASK_TIMEOUT)
         if self.ttl is None:
             object.__setattr__(self, "ttl", TASK_TTL)
         if self.ack_late is None:
             object.__setattr__(self, "ack_late", TASK_ACK_LATE)
         if self.result_ttl is None:
-            object.__setattr__(self, "result_ttl", RESULT_TTL)
+            object.__setattr__(self, "result_ttl", TASK_RESULT_TTL)
         if self.result_return is None:
-            object.__setattr__(self, "result_return", RESULT_RETURN)
-        if self.result_encrypt is None:
-            object.__setattr__(self, "result_encrypt", RESULT_ENCRYPT)
+            object.__setattr__(self, "result_return", TASK_RESULT_RETURN)
+        if self.events is None:
+            object.__setattr__(self, "events", EVENTS)
+        if self.event_ttl is None:
+            object.__setattr__(self, "event_ttl", EVENT_TTL)
 
     def instantiate(self, data: TaskData = None) -> "TaskInstance":
         if data is None:
             data = TaskData()
         if isinstance(data.task_id, str):
             data.task_id = UUID(data.task_id)
         if isinstance(data.args, list):
@@ -100,14 +108,18 @@
             data.result_ttl = self.result_ttl
         if data.result_return is None:
             data.result_return = self.result_return
         if data.result_encrypt is None:
             data.result_encrypt = self.result_encrypt
         if data.thread is None:
             data.thread = self.thread
+        if data.events is None:
+            data.events = self.events
+        if data.event_ttl is None:
+            data.event_ttl = self.event_ttl
         return TaskInstance(task=self, data=data)
 
     def __call__(self, *args, **kwds) -> Any:
         return self.instantiate(TaskData(args=args, kwds=kwds))()
 
 
 @dataclass(frozen=True)
@@ -146,14 +158,22 @@
             object.__setattr__(self, "priority", MESSAGE_PRIORITY)
         if self.ttl is None:
             object.__setattr__(self, "ttl", MESSAGE_TTL)
         if self.ack_late is None:
             object.__setattr__(self, "ack_late", MESSAGE_ACK_LATE)
 
 
+@dataclass(frozen=True)
+class Event:
+    type: str
+    datetime: datetime.datetime
+    data: dict
+    event_id: UUID = field(default_factory=uuid4)
+
+
 class Graph:
     def __init__(
         self,
         id: str,
         nodes: Dict = None,
         edges: Dict = None,
         roots: Set = None,
```

### Comparing `arrlio-0.8.0/arrlio/serializer/base.py` & `arrlio-0.9.0/arrlio/serializer/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import abc
 from typing import Any, Union
 
-from arrlio.models import TaskInstance, TaskResult
+from arrlio.models import Event, TaskInstance, TaskResult
 
 
 class Serializer(abc.ABC):
     @abc.abstractmethod
     def dumps_task_instance(self, task_instance: TaskInstance, **kwds) -> Union[bytes, TaskInstance]:
         pass
 
@@ -18,13 +18,21 @@
         pass
 
     @abc.abstractmethod
     def loads_task_result(self, data: Union[bytes, TaskResult]) -> TaskResult:
         pass
 
     @abc.abstractmethod
+    def dumps_event(self, event: Event, **kwds) -> Union[bytes, Event]:
+        pass
+
+    @abc.abstractmethod
+    def loads_event(self, data: Union[bytes, Event]) -> Event:
+        pass
+
+    @abc.abstractmethod
     def dumps(self, data: Any, **kwds) -> Union[bytes, Any]:
         pass
 
     @abc.abstractmethod
     def loads(self, data: Union[bytes, Any]) -> Any:
         pass
```

### Comparing `arrlio-0.8.0/arrlio/serializer/json.py` & `arrlio-0.9.0/arrlio/serializer/json.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import logging
 import traceback
 from dataclasses import asdict
 from typing import Any, Callable
 
 from arrlio import __tasks__
-from arrlio.models import Graph, Task, TaskData, TaskInstance, TaskResult
+from arrlio.models import Event, Graph, Task, TaskData, TaskInstance, TaskResult
 from arrlio.serializer import base
 from arrlio.utils import ExtendedJSONEncoder
 
 
 logger = logging.getLogger("arrlio")
 
 
@@ -55,14 +55,21 @@
         else:
             data = (task_result.res, None, None)
         return json.dumps(data, cls=self.encoder).encode()
 
     def loads_task_result(self, data: bytes) -> TaskResult:
         return TaskResult(*json.loads(data))
 
+    def dumps_event(self, event: Event, **kwds) -> bytes:
+        data = asdict(event)
+        return json.dumps(data, cls=self.encoder).encode()
+
+    def loads_event(self, data: bytes) -> Event:
+        return Event(**json.loads(data))
+
     def dumps(self, data: Any, **kwds) -> bytes:
         return json.dumps(data, cls=self.encoder).encode()
 
     def loads(self, data: bytes) -> Any:
         return json.loads(data)
```

### Comparing `arrlio-0.8.0/arrlio/settings.py` & `arrlio-0.9.0/arrlio/settings.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,84 +1,70 @@
 from typing import List, Optional
 
 from pydantic import BaseSettings, Field
 
 from arrlio.tp import BackendT, PositiveIntT, PriorityT, TimeoutT
 
 
-BACKEND = "arrlio.backend.local"
+BACKEND = "arrlio.backends.local"
 
 TASK_BIND = False
 TASK_QUEUE = "arrlio.tasks"
 TASK_PRIORITY = 1
 TASK_TIMEOUT = 300
 TASK_TTL = 300
 TASK_ACK_LATE = False
 
-RESULT_TTL = 300
-RESULT_RETURN = True
-RESULT_ENCRYPT = False
+TASK_RESULT_TTL = 300
+TASK_RESULT_RETURN = True
+
+EVENTS = False
+EVENT_TTL = 300
 
 MESSAGE_EXCHANGE = "arrlio.messages"
 MESSAGE_PRIORITY = 1
 MESSAGE_TTL = 300
 MESSAGE_ACK_LATE = False
 
-CONSUMER_TASK_QUEUES = [TASK_QUEUE]
-CONSUMER_MESSAGE_QUEUES = [MESSAGE_EXCHANGE]
-CONSUMER_POOL_SIZE = 100
+TASK_QUEUES = [TASK_QUEUE]
+MESSAGE_QUEUES = [MESSAGE_EXCHANGE]
+POOL_SIZE = 100
 
 
 class TaskConfig(BaseSettings):
-    bind: bool = Field(default_factory=lambda: TASK_BIND)
     queue: str = Field(default_factory=lambda: TASK_QUEUE)
     priority: PriorityT = Field(default_factory=lambda: TASK_PRIORITY)
     timeout: Optional[TimeoutT] = Field(default_factory=lambda: TASK_TIMEOUT)
     ttl: Optional[PositiveIntT] = Field(default_factory=lambda: TASK_TTL)
     ack_late: Optional[bool] = Field(default_factory=lambda: TASK_ACK_LATE)
-    result_return: Optional[bool] = Field(default_factory=lambda: RESULT_RETURN)
-    result_encrypt: Optional[bool] = Field(default_factory=lambda: RESULT_ENCRYPT)
+    result_ttl: Optional[PositiveIntT] = Field(default_factory=lambda: TASK_RESULT_TTL)
+    result_return: Optional[bool] = Field(default_factory=lambda: TASK_RESULT_RETURN)
+    events: Optional[bool] = Field(default_factory=lambda: EVENTS)
+    event_ttl: Optional[PositiveIntT] = Field(default_factory=lambda: EVENT_TTL)
 
     class Config:
         validate_assignment = True
         env_prefix = "ARRLIO_TASK_"
 
 
-class ResultConfig(BaseSettings):
-    ttl: Optional[PositiveIntT] = Field(default_factory=lambda: RESULT_TTL)
-
-    class Config:
-        validate_assignment = True
-        env_prefix = "ARRLIO_RESULT_"
-
-
 class MessageConfig(BaseSettings):
     exchange: str = Field(default_factory=lambda: MESSAGE_EXCHANGE)
     priority: PriorityT = Field(default_factory=lambda: MESSAGE_PRIORITY)
     ttl: Optional[PositiveIntT] = Field(default_factory=lambda: MESSAGE_TTL)
     ack_late: Optional[bool] = Field(default_factory=lambda: MESSAGE_ACK_LATE)
 
     class Config:
         validate_assignment = True
         env_prefix = "ARRLIO_MESSAGE_"
 
 
-class ProducerConfig(BaseSettings):
+class Config(BaseSettings):
     backend: BackendT = Field(default_factory=lambda: BACKEND, env="ARRLIO_BACKEND")
     task: TaskConfig = Field(default_factory=TaskConfig)
-    result: ResultConfig = Field(default_factory=ResultConfig)
     message: MessageConfig = Field(default_factory=MessageConfig)
+    task_queues: List[str] = Field(default_factory=lambda: TASK_QUEUES)
+    message_queues: List[str] = Field(default_factory=lambda: MESSAGE_QUEUES)
+    pool_size: PositiveIntT = Field(default_factory=lambda: POOL_SIZE)
 
     class Config:
         validate_assignment = True
-        env_prefix = "ARRLIO_PRODUCER_"
-
-
-class ConsumerConfig(BaseSettings):
-    backend: BackendT = Field(default_factory=lambda: BACKEND, env="ARRLIO_BACKEND")
-    task_queues: List[str] = Field(default_factory=lambda: CONSUMER_TASK_QUEUES)
-    message_queues: List[str] = Field(default_factory=lambda: CONSUMER_MESSAGE_QUEUES)
-    pool_size: PositiveIntT = Field(default_factory=lambda: CONSUMER_POOL_SIZE)
-
-    class Config:
-        validate_assignment = True
-        env_prefix = "ARRLIO_CONSUMER_"
+        env_prefix = "ARRLIO_"
```

### Comparing `arrlio-0.8.0/arrlio/tp.py` & `arrlio-0.9.0/arrlio/tp.py`

 * *Files identical despite different names*

### Comparing `arrlio-0.8.0/arrlio/utils.py` & `arrlio-0.9.0/arrlio/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import asyncio
 import contextlib
-import inspect
 import itertools
 import json
 import logging
 from dataclasses import asdict
 from datetime import datetime
 from types import MethodType
 from typing import Iterable
@@ -39,20 +38,18 @@
     if exc_filter is None:
         exc_filter = lambda e: isinstance(e, (ConnectionError, TimeoutError, asyncio.TimeoutError))
 
     def decorator(fn):
         async def wrapper(*args, **kwds):
             while True:
                 try:
-                    if inspect.iscoroutinefunction(fn):
-                        return await fn(*args, **kwds)
-                    return fn(*args, **kwds)
+                    return await fn(*args, **kwds)
                 except Exception as e:
-                    logger.error(e)
                     if not exc_filter(e):
+                        logger.error(e)
                         raise e
                     try:
                         t = next(retry_timeouts)
                         logger.error("%s - retry in %s second(s)", e, t)
                         await asyncio.sleep(t)
                     except StopIteration:
                         raise e
```

### Comparing `arrlio-0.8.0/arrlio.egg-info/SOURCES.txt` & `arrlio-0.9.0/arrlio.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 arrlio/tp.py
 arrlio/utils.py
 arrlio.egg-info/PKG-INFO
 arrlio.egg-info/SOURCES.txt
 arrlio.egg-info/dependency_links.txt
 arrlio.egg-info/requires.txt
 arrlio.egg-info/top_level.txt
-arrlio/backend/__init__.py
-arrlio/backend/base.py
-arrlio/backend/local.py
-arrlio/backend/rabbitmq.py
-arrlio/backend/redis.py
+arrlio/backends/__init__.py
+arrlio/backends/base.py
+arrlio/backends/local.py
+arrlio/backends/rabbitmq.py
+arrlio/backends/redis.py
 arrlio/serializer/__init__.py
 arrlio/serializer/base.py
 arrlio/serializer/json.py
 arrlio/serializer/nop.py
```

### Comparing `arrlio-0.8.0/setup.py` & `arrlio-0.9.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -28,20 +28,16 @@
         "aiormq>=5.2.0",
         "cryptography",
         "pydantic>=1.9.0",
         "yarl",
         "roview",
         "siderpy[hiredis]",
     ],
-    dependency_links=[
-        "git+git://github.com/levsh/roview.git#egg=roview",
-    ],
     python_requires=">=3.8",
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3 :: Only",
-        "Topic :: System :: Distributed Computing",
         "Operating System :: POSIX :: Linux",
         "Operating System :: MacOS :: MacOS X",
     ],
 )
```

