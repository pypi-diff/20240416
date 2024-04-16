# Comparing `tmp/rosny-0.0.6.tar.gz` & `tmp/rosny-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rosny-0.0.6.tar", last modified: Mon Oct 17 17:53:42 2022, max compression
+gzip compressed data, was "rosny-0.1.0.tar", last modified: Tue Apr 16 16:17:23 2024, max compression
```

## Comparing `rosny-0.0.6.tar` & `rosny-0.1.0.tar`

### file list

```diff
@@ -1,23 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 17:53:42.810592 rosny-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (121)     1072 2022-10-17 17:53:28.000000 rosny-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3248 2022-10-17 17:53:42.810592 rosny-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2289 2022-10-17 17:53:28.000000 rosny-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 17:53:42.810592 rosny-0.0.6/rosny/
--rw-r--r--   0 runner    (1001) docker     (121)      177 2022-10-17 17:53:28.000000 rosny-0.0.6/rosny/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2863 2022-10-17 17:53:28.000000 rosny-0.0.6/rosny/abstract.py
--rw-r--r--   0 runner    (1001) docker     (121)     2453 2022-10-17 17:53:28.000000 rosny-0.0.6/rosny/compose.py
--rw-r--r--   0 runner    (1001) docker     (121)     3370 2022-10-17 17:53:28.000000 rosny-0.0.6/rosny/loop.py
--rw-r--r--   0 runner    (1001) docker     (121)     1591 2022-10-17 17:53:28.000000 rosny-0.0.6/rosny/process.py
--rw-r--r--   0 runner    (1001) docker     (121)      878 2022-10-17 17:53:28.000000 rosny-0.0.6/rosny/signal.py
--rw-r--r--   0 runner    (1001) docker     (121)      791 2022-10-17 17:53:28.000000 rosny-0.0.6/rosny/state.py
--rw-r--r--   0 runner    (1001) docker     (121)     1369 2022-10-17 17:53:28.000000 rosny-0.0.6/rosny/thread.py
--rw-r--r--   0 runner    (1001) docker     (121)     3355 2022-10-17 17:53:28.000000 rosny-0.0.6/rosny/timing.py
--rw-r--r--   0 runner    (1001) docker     (121)      580 2022-10-17 17:53:28.000000 rosny-0.0.6/rosny/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 17:53:42.810592 rosny-0.0.6/rosny.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3248 2022-10-17 17:53:42.000000 rosny-0.0.6/rosny.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      338 2022-10-17 17:53:42.000000 rosny-0.0.6/rosny.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-17 17:53:42.000000 rosny-0.0.6/rosny.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-10-17 17:53:42.000000 rosny-0.0.6/rosny.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-17 17:53:42.000000 rosny-0.0.6/rosny.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      274 2022-10-17 17:53:42.810592 rosny-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1706 2022-10-17 17:53:28.000000 rosny-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:17:23.695213 rosny-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-16 16:17:19.000000 rosny-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5040 2024-04-16 16:17:23.695213 rosny-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-04-16 16:17:19.000000 rosny-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-04-16 16:17:19.000000 rosny-0.1.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:17:23.691213 rosny-0.1.0/rosny/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-16 16:17:19.000000 rosny-0.1.0/rosny/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-04-16 16:17:19.000000 rosny-0.1.0/rosny/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-04-16 16:17:19.000000 rosny-0.1.0/rosny/compose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-04-16 16:17:19.000000 rosny-0.1.0/rosny/loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-16 16:17:19.000000 rosny-0.1.0/rosny/process.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-16 16:17:19.000000 rosny-0.1.0/rosny/signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-16 16:17:19.000000 rosny-0.1.0/rosny/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-16 16:17:19.000000 rosny-0.1.0/rosny/thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-04-16 16:17:19.000000 rosny-0.1.0/rosny/timing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-16 16:17:19.000000 rosny-0.1.0/rosny/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:17:23.691213 rosny-0.1.0/rosny.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5040 2024-04-16 16:17:23.000000 rosny-0.1.0/rosny.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-16 16:17:23.000000 rosny-0.1.0/rosny.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 16:17:23.000000 rosny-0.1.0/rosny.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-16 16:17:23.000000 rosny-0.1.0/rosny.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-16 16:17:23.000000 rosny-0.1.0/rosny.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 16:17:23.695213 rosny-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:17:23.691213 rosny-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-16 16:17:19.000000 rosny-0.1.0/tests/test_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-16 16:17:19.000000 rosny-0.1.0/tests/test_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-04-16 16:17:19.000000 rosny-0.1.0/tests/test_compose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7937 2024-04-16 16:17:19.000000 rosny-0.1.0/tests/test_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-16 16:17:19.000000 rosny-0.1.0/tests/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-04-16 16:17:19.000000 rosny-0.1.0/tests/test_timing.py
```

### Comparing `rosny-0.0.6/LICENSE` & `rosny-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rosny-0.0.6/README.md` & `rosny-0.1.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 rosny is a lightweight library for building concurrent systems.
 
 ## Installation
 
 Tested on:
 
 * Linux
-* Python >= 3.6
+* Python >= 3.8
 
 From pip:
 
 ```bash
 pip install rosny
 ```
 
@@ -31,49 +31,49 @@
 pip install git+https://github.com/lRomul/rosny.git@master
 ```
 
 ## Example
 
 ```python
 from multiprocessing import Queue
-from rosny import ThreadStream, ProcessStream, ComposeStream
+from rosny import ThreadNode, ProcessNode, ComposeNode
 
 
-class SenderStream(ThreadStream):  # using threading.Thread
+class SenderNode(ThreadNode):  # using threading.Thread
     def __init__(self, queue: Queue):
         super().__init__(loop_rate=30)
         self.queue = queue
         self.count = 0
 
     # run the method in a loop in a separate thread
     def work(self):
         self.queue.put(self.count)
         self.logger.info(f'put {self.count}')
         self.count += 1
 
 
-class ReceiverStream(ProcessStream):  # using multiprocessing.Process
+class ReceiverNode(ProcessNode):  # using multiprocessing.Process
     def __init__(self, queue: Queue):
         super().__init__()
         self.queue = queue
 
     # run the method in a loop in a separate process
     def work(self):
         value = self.queue.get(timeout=1)
         self.logger.info(f'get {value}')
 
 
-class MainStream(ComposeStream):  # merging several streams
+class MainNode(ComposeNode):  # merging several nodes
     def __init__(self):
         super().__init__()
         queue = Queue()
-        self.sender = SenderStream(queue)
-        self.receiver = ReceiverStream(queue)
+        self.sender = SenderNode(queue)
+        self.receiver = ReceiverNode(queue)
 
 
 if __name__ == "__main__":
-    stream = MainStream()
-    stream.start()
-    stream.wait(5)
-    stream.stop()
-    stream.join()
+    node = MainNode()
+    node.start()
+    node.wait(5)
+    node.stop()
+    node.join()
 ```
```

### Comparing `rosny-0.0.6/rosny/abstract.py` & `rosny-0.1.0/rosny/abstract.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Optional
 
 from rosny.state import CommonState
 from rosny.utils import setup_logger, default_object_name
 from rosny.signal import start_signals, stop_signals
 
 
-class AbstractStream(metaclass=abc.ABCMeta):
+class AbstractNode(metaclass=abc.ABCMeta):
     def on_compile_begin(self):
         pass
 
     def on_compile_end(self):
         pass
 
     @abc.abstractmethod
@@ -63,15 +63,15 @@
         pass
 
     @abc.abstractmethod
     def joined(self) -> bool:
         pass
 
 
-class BaseStream(AbstractStream, metaclass=abc.ABCMeta):
+class BaseNode(AbstractNode, metaclass=abc.ABCMeta):
     def __init__(self):
         self.name = default_object_name(self)
         self.logger = setup_logger(self.name)
         self.common_state = CommonState()
         self._compiled = False
         self.handle_signals = True
 
@@ -83,15 +83,15 @@
         self.logger = setup_logger(self.name)
         if common_state is not None:
             self.common_state = common_state
         self.handle_signals = handle_signals
         self._compiled = True
 
     def wait(self, timeout: Optional[float] = None):
-        self.logger.info(f"Waiting stream with timeout {timeout}")
+        self.logger.info(f"Waiting node with timeout {timeout}")
         self.common_state.wait_exit(timeout=timeout)
         if self.common_state.exit_is_set():
             self.logger.info("Waiting ended, exit event is set")
         else:
             self.logger.info("Waiting ended, timeout exceeded")
 
     def _actions_before_start(self):
```

### Comparing `rosny-0.0.6/rosny/compose.py` & `rosny-0.1.0/rosny/loop.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,76 +1,108 @@
 import abc
-import time
-from typing import Optional, Dict
+from typing import Optional, Union, Any
 
-from rosny.abstract import BaseStream, AbstractStream
 from rosny.state import CommonState
+from rosny.abstract import BaseNode
+from rosny.timing import LoopRateManager, Profiler
 
 
-class ComposeStream(BaseStream, metaclass=abc.ABCMeta):
-    @abc.abstractmethod
-    def __init__(self):
+class LoopNode(BaseNode, metaclass=abc.ABCMeta):
+    def __init__(self,
+                 loop_rate: Optional[float] = None,
+                 min_sleep: float = 1e-9,
+                 profile_interval: Optional[float] = None,
+                 daemon: bool = False):
         super().__init__()
-        self._streams: Dict[str, AbstractStream] = dict()
+        self.daemon = daemon
+        self._driver: Optional[Any] = None
+        self.rate_manager = LoopRateManager(loop_rate=loop_rate,
+                                            min_sleep=min_sleep)
+        self.profiler = Profiler(node=self, interval=profile_interval)
+
+    @abc.abstractmethod
+    def work(self):
+        pass
+
+    def loop(self):
+        try:
+            self.on_loop_begin()
+            self.rate_manager.reset()
+            self.profiler.reset(self)
+            while not self.stopped():
+                self.work()
+                self.rate_manager.timing()
+                self.profiler.profile()
+        except (Exception, KeyboardInterrupt) as exception:
+            self.on_catch_exception(exception)
+        finally:
+            self.on_loop_end()
+
+    def on_catch_exception(self, exception: Union[Exception, KeyboardInterrupt]):
+        self.logger.exception(exception)
+        self.common_state.set_exit()
+
+    def on_loop_begin(self):
+        pass
+
+    def on_loop_end(self):
+        pass
 
-    def __setattr__(self, name, value):
-        if isinstance(value, AbstractStream):
-            self._streams[name] = value
-        object.__setattr__(self, name, value)
+    @abc.abstractmethod
+    def _start_driver(self):
+        pass
+
+    @abc.abstractmethod
+    def _stop_driver(self):
+        pass
+
+    @abc.abstractmethod
+    def _join_driver(self, timeout: Optional[float] = None):
+        pass
 
     def compile(self,
                 common_state: Optional[CommonState] = None,
                 name: Optional[str] = None,
                 handle_signals: bool = True):
         self.on_compile_begin()
         super().compile(common_state=common_state,
                         name=name,
                         handle_signals=handle_signals)
-        for stream_name, stream in self._streams.items():
-            stream.compile(
-                common_state=self.common_state,
-                name=f"{self.name}/{stream_name}",
-                handle_signals=False
-            )
         self.on_compile_end()
 
     def start(self):
-        self.logger.info("Starting stream")
-        self._actions_before_start()
-        self.on_start_begin()
-        for stream in self._streams.values():
-            stream.start()
-        self.on_start_end()
-        self.logger.info("Stream started")
+        self.logger.info("Starting node")
+        if self.stopped():
+            if self.joined():
+                self._actions_before_start()
+                self.on_start_begin()
+                self._start_driver()
+                self.on_start_end()
+                self.logger.info("Node started")
+            else:
+                self.logger.error("Node stopped but not joined")
+        else:
+            self.logger.error("Node is already started")
 
     def stop(self):
-        self.logger.info("Stopping stream")
-        self.on_stop_begin()
-        for stream in self._streams.values():
-            stream.stop()
-        self.on_stop_end()
-        self._actions_after_stop()
-        self.logger.info("Stream stopped")
+        self.logger.info("Stopping node")
+        if not self.stopped():
+            self.on_stop_begin()
+            self._stop_driver()
+            self.on_stop_end()
+            self._actions_after_stop()
+            self.logger.info("Node stopped")
+        else:
+            self.logger.error("Node is already stopped")
 
     def join(self, timeout: Optional[float] = None):
-        self.logger.info("Joining stream")
-        self.on_join_begin()
-        for stream in self._streams.values():
-            start = time.perf_counter()
-            stream.join(timeout=timeout)
-            if timeout is not None:
-                timeout -= time.perf_counter() - start
-                timeout = max(timeout, 0)
-        self.on_join_end()
-        self.logger.info("Stream joined")
-
-    def stopped(self) -> bool:
-        for stream in self._streams.values():
-            if not stream.stopped():
-                return False
-        return True
+        self.logger.info("Joining node")
+        if not self.joined():
+            self.on_join_begin()
+            self._join_driver(timeout=timeout)
+            self.on_join_end()
+            self.logger.info("Node joined")
+        else:
+            self.logger.error("Node is already joined")
 
     def joined(self) -> bool:
-        for stream in self._streams.values():
-            if not stream.joined():
-                return False
-        return True
+        return self._driver is None
```

### Comparing `rosny-0.0.6/rosny/process.py` & `rosny-0.1.0/rosny/process.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import abc
 from typing import Optional
 from multiprocessing import Process, Value
 
-from rosny.loop import LoopStream
+from rosny.loop import LoopNode
 from rosny.utils import setup_logger
 
 
-class ProcessStream(LoopStream, metaclass=abc.ABCMeta):
+class ProcessNode(LoopNode, metaclass=abc.ABCMeta):
     def __init__(self,
                  loop_rate: Optional[float] = None,
                  min_sleep: float = 1e-9,
                  profile_interval: Optional[float] = None,
                  daemon: bool = False):
         super().__init__(loop_rate=loop_rate,
                          min_sleep=min_sleep,
```

### Comparing `rosny-0.0.6/rosny/signal.py` & `rosny-0.1.0/rosny/signal.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,23 +8,23 @@
     def __init__(self, signum: signal.Signals, frame):
         message = f"Handle signal: {signal.Signals(signum).name}"
         super().__init__(message)
         self.signum = signum
         self.frame = frame
 
 
-def start_signals(stream):
+def start_signals(node):
     def signal_handler(signum: signal.Signals, frame):
         exception = SignalException(signum, frame)
-        stream.logger.error(exception)
-        stream.stop()
+        node.logger.error(exception)
+        node.stop()
         raise exception
 
     for sig in _signals:
         signal.signal(sig, signal_handler)
-    stream.logger.info("Start handling signals")
+    node.logger.info("Start handling signals")
 
 
-def stop_signals(stream):
+def stop_signals(node):
     for sig in _signals:
         signal.signal(sig, _default_handlers[sig])
-    stream.logger.info("Stop handling signals")
+    node.logger.info("Stop handling signals")
```

### Comparing `rosny-0.0.6/rosny/state.py` & `rosny-0.1.0/rosny/state.py`

 * *Files identical despite different names*

### Comparing `rosny-0.0.6/rosny/thread.py` & `rosny-0.1.0/rosny/thread.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import abc
 from threading import Thread
 from typing import Optional
 
-from rosny.loop import LoopStream
+from rosny.loop import LoopNode
 
 
-class ThreadStream(LoopStream, metaclass=abc.ABCMeta):
+class ThreadNode(LoopNode, metaclass=abc.ABCMeta):
     def __init__(self,
                  loop_rate: Optional[float] = None,
                  min_sleep: float = 1e-9,
                  profile_interval: Optional[float] = None,
                  daemon: bool = False):
         super().__init__(loop_rate=loop_rate,
                          min_sleep=min_sleep,
```

### Comparing `rosny-0.0.6/rosny/timing.py` & `rosny-0.1.0/rosny/timing.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import time
 from typing import Optional
 
-from rosny.abstract import BaseStream
+from rosny.abstract import BaseNode
 
 
 class LoopTimeMeter:
     def __init__(self):
         self.mean = 0.0
         self.count = 0
         self.last_time = time.perf_counter()
@@ -77,31 +77,31 @@
             sleep_time = max(self.min_sleep, sleep_time)
 
             time.sleep(sleep_time)
             self._prev_time = time.perf_counter()
 
 
 class Profiler:
-    def __init__(self, stream: BaseStream, interval: Optional[float] = None):
-        self._stream = stream
+    def __init__(self, node: BaseNode, interval: Optional[float] = None):
+        self._node = node
         self.interval = interval
         self._time_meter = LoopTimeMeter()
         self._last_profile_time = time.perf_counter()
 
-    def reset(self, stream: BaseStream):
-        self._stream = stream
+    def reset(self, node: BaseNode):
+        self._node = node
         self._time_meter.reset()
         self._last_profile_time = time.perf_counter()
 
     def profile(self):
         if self.interval is not None:
             self._time_meter.end()
             if self._time_meter.last_time - self._last_profile_time > self.interval:
                 loop_time = self._time_meter.mean
                 loop_rate = 1 / loop_time if loop_time else float('inf')
-                self._stream.common_state.profile_stats[self._stream.name] = loop_time
-                self._stream.logger.info(
+                self._node.common_state.profile_stats[self._node.name] = loop_time
+                self._node.logger.info(
                     f"Profile - loop time {loop_time:.6g}, loop rate {loop_rate:.4g}"
                 )
 
                 self._time_meter.reset()
                 self._last_profile_time = time.perf_counter()
```

### Comparing `rosny-0.0.6/rosny/utils.py` & `rosny-0.1.0/rosny/utils.py`

 * *Files identical despite different names*

