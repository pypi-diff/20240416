# Comparing `tmp/rate_control-1.1.0.tar.gz` & `tmp/rate_control-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rate_control-1.1.0.tar", max compression
+gzip compressed data, was "rate_control-2.0.0.tar", max compression
```

## Comparing `rate_control-1.1.0.tar` & `rate_control-2.0.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1101 2024-03-31 06:43:45.993707 rate_control-1.1.0/LICENSE
--rw-r--r--   0        0        0     3822 2024-03-31 06:43:45.993707 rate_control-1.1.0/README.rst
--rw-r--r--   0        0        0     2812 2024-03-31 06:43:52.909777 rate_control-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      423 2024-03-31 06:43:45.997707 rate_control-1.1.0/rate_control/__init__.py
--rw-r--r--   0        0        0     3484 2024-03-31 06:43:45.997707 rate_control-1.1.0/rate_control/_bucket_group.py
--rw-r--r--   0        0        0      119 2024-03-31 06:43:45.997707 rate_control-1.1.0/rate_control/_controllers/__init__.py
--rw-r--r--   0        0        0     2797 2024-03-31 06:43:45.997707 rate_control-1.1.0/rate_control/_controllers/_base.py
--rw-r--r--   0        0        0      885 2024-03-31 06:43:45.997707 rate_control-1.1.0/rate_control/_controllers/_limiter.py
--rw-r--r--   0        0        0     8300 2024-03-31 06:43:45.997707 rate_control-1.1.0/rate_control/_controllers/_scheduler.py
--rw-r--r--   0        0        0      111 2024-03-31 06:43:45.997707 rate_control-1.1.0/rate_control/_enums/__init__.py
--rw-r--r--   0        0        0      262 2024-03-31 06:43:45.997707 rate_control-1.1.0/rate_control/_enums/_duration.py
--rw-r--r--   0        0        0      350 2024-03-31 06:43:45.997707 rate_control-1.1.0/rate_control/_enums/_priority.py
--rw-r--r--   0        0        0      297 2024-03-31 06:43:45.997707 rate_control-1.1.0/rate_control/_errors.py
--rw-r--r--   0        0        0      105 2024-03-31 06:43:45.997707 rate_control-1.1.0/rate_control/_helpers/__init__.py
--rw-r--r--   0        0        0      781 2024-03-31 06:43:45.997707 rate_control-1.1.0/rate_control/_helpers/_mk_repr.py
--rw-r--r--   0        0        0      472 2024-03-31 06:43:45.997707 rate_control-1.1.0/rate_control/_helpers/_protocols.py
--rw-r--r--   0        0        0     1502 2024-03-31 06:43:45.997707 rate_control-1.1.0/rate_control/_helpers/_request.py
--rw-r--r--   0        0        0     2167 2024-03-31 06:43:45.997707 rate_control-1.1.0/rate_control/_helpers/_validation.py
--rw-r--r--   0        0        0      330 2024-03-31 06:43:45.997707 rate_control-1.1.0/rate_control/buckets/__init__.py
--rw-r--r--   0        0        0      345 2024-03-31 06:43:45.997707 rate_control-1.1.0/rate_control/buckets/_base/__init__.py
--rw-r--r--   0        0        0     1946 2024-03-31 06:43:45.997707 rate_control-1.1.0/rate_control/buckets/_base/_abc.py
--rw-r--r--   0        0        0     2478 2024-03-31 06:43:45.997707 rate_control-1.1.0/rate_control/buckets/_base/_base_rate.py
--rw-r--r--   0        0        0      804 2024-03-31 06:43:45.997707 rate_control-1.1.0/rate_control/buckets/_base/_capacity_updating.py
--rw-r--r--   0        0        0      905 2024-03-31 06:43:45.997707 rate_control-1.1.0/rate_control/buckets/_base/_token_based.py
--rw-r--r--   0        0        0      976 2024-03-31 06:43:45.997707 rate_control-1.1.0/rate_control/buckets/_base/_windowed.py
--rw-r--r--   0        0        0     1033 2024-03-31 06:43:45.997707 rate_control-1.1.0/rate_control/buckets/_fixed_window_counter.py
--rw-r--r--   0        0        0     1371 2024-03-31 06:43:45.997707 rate_control-1.1.0/rate_control/buckets/_leaky_bucket.py
--rw-r--r--   0        0        0      658 2024-03-31 06:43:45.997707 rate_control-1.1.0/rate_control/buckets/_sliding_window_log.py
--rw-r--r--   0        0        0      657 2024-03-31 06:43:45.997707 rate_control-1.1.0/rate_control/buckets/_unlimited.py
--rw-r--r--   0        0        0        0 2024-03-31 06:43:45.997707 rate_control-1.1.0/rate_control/py.typed
--rw-r--r--   0        0        0      202 2024-03-31 06:43:45.997707 rate_control-1.1.0/rate_control/queues/__init__.py
--rw-r--r--   0        0        0     1540 2024-03-31 06:43:45.997707 rate_control-1.1.0/rate_control/queues/_abc.py
--rw-r--r--   0        0        0     1336 2024-03-31 06:43:45.997707 rate_control-1.1.0/rate_control/queues/_fifo.py
--rw-r--r--   0        0        0     1311 2024-03-31 06:43:45.997707 rate_control-1.1.0/rate_control/queues/_lifo.py
--rw-r--r--   0        0        0     1658 2024-03-31 06:43:45.997707 rate_control-1.1.0/rate_control/queues/_priority.py
--rw-r--r--   0        0        0     5030 1970-01-01 00:00:00.000000 rate_control-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1101 2024-04-16 18:30:46.785962 rate_control-2.0.0/LICENSE
+-rw-r--r--   0        0        0     3822 2024-04-16 18:30:46.785962 rate_control-2.0.0/README.rst
+-rw-r--r--   0        0        0     2872 2024-04-16 18:31:01.737882 rate_control-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0      622 2024-04-16 18:30:46.789962 rate_control-2.0.0/rate_control/__init__.py
+-rw-r--r--   0        0        0     3718 2024-04-16 18:30:46.789962 rate_control-2.0.0/rate_control/_bucket_group.py
+-rw-r--r--   0        0        0      330 2024-04-16 18:30:46.789962 rate_control-2.0.0/rate_control/_buckets/__init__.py
+-rw-r--r--   0        0        0      344 2024-04-16 18:30:46.789962 rate_control-2.0.0/rate_control/_buckets/_base/__init__.py
+-rw-r--r--   0        0        0     1942 2024-04-16 18:30:46.789962 rate_control-2.0.0/rate_control/_buckets/_base/_abc.py
+-rw-r--r--   0        0        0     2479 2024-04-16 18:30:46.789962 rate_control-2.0.0/rate_control/_buckets/_base/_base_rate.py
+-rw-r--r--   0        0        0      805 2024-04-16 18:30:46.789962 rate_control-2.0.0/rate_control/_buckets/_base/_capacity_updating.py
+-rw-r--r--   0        0        0      906 2024-04-16 18:30:46.789962 rate_control-2.0.0/rate_control/_buckets/_base/_token_based.py
+-rw-r--r--   0        0        0      977 2024-04-16 18:30:46.789962 rate_control-2.0.0/rate_control/_buckets/_base/_windowed.py
+-rw-r--r--   0        0        0     1034 2024-04-16 18:30:46.789962 rate_control-2.0.0/rate_control/_buckets/_fixed_window_counter.py
+-rw-r--r--   0        0        0     1372 2024-04-16 18:30:46.789962 rate_control-2.0.0/rate_control/_buckets/_leaky_bucket.py
+-rw-r--r--   0        0        0      659 2024-04-16 18:30:46.789962 rate_control-2.0.0/rate_control/_buckets/_sliding_window_log.py
+-rw-r--r--   0        0        0      653 2024-04-16 18:30:46.789962 rate_control-2.0.0/rate_control/_buckets/_unlimited.py
+-rw-r--r--   0        0        0      179 2024-04-16 18:30:46.789962 rate_control-2.0.0/rate_control/_controllers/__init__.py
+-rw-r--r--   0        0        0     4657 2024-04-16 18:30:46.789962 rate_control-2.0.0/rate_control/_controllers/_abc.py
+-rw-r--r--   0        0        0     1046 2024-04-16 18:30:46.789962 rate_control-2.0.0/rate_control/_controllers/_rate_limiter.py
+-rw-r--r--   0        0        0     8709 2024-04-16 18:30:46.789962 rate_control-2.0.0/rate_control/_controllers/_scheduler.py
+-rw-r--r--   0        0        0      111 2024-04-16 18:30:46.789962 rate_control-2.0.0/rate_control/_enums/__init__.py
+-rw-r--r--   0        0        0      262 2024-04-16 18:30:46.789962 rate_control-2.0.0/rate_control/_enums/_duration.py
+-rw-r--r--   0        0        0      350 2024-04-16 18:30:46.789962 rate_control-2.0.0/rate_control/_enums/_priority.py
+-rw-r--r--   0        0        0      297 2024-04-16 18:30:46.789962 rate_control-2.0.0/rate_control/_errors.py
+-rw-r--r--   0        0        0      105 2024-04-16 18:30:46.789962 rate_control-2.0.0/rate_control/_helpers/__init__.py
+-rw-r--r--   0        0        0      781 2024-04-16 18:30:46.789962 rate_control-2.0.0/rate_control/_helpers/_mk_repr.py
+-rw-r--r--   0        0        0      472 2024-04-16 18:30:46.789962 rate_control-2.0.0/rate_control/_helpers/_protocols.py
+-rw-r--r--   0        0        0     1502 2024-04-16 18:30:46.789962 rate_control-2.0.0/rate_control/_helpers/_request.py
+-rw-r--r--   0        0        0     2162 2024-04-16 18:30:46.789962 rate_control-2.0.0/rate_control/_helpers/_validation.py
+-rw-r--r--   0        0        0        0 2024-04-16 18:30:46.789962 rate_control-2.0.0/rate_control/py.typed
+-rw-r--r--   0        0        0      202 2024-04-16 18:30:46.789962 rate_control-2.0.0/rate_control/queues/__init__.py
+-rw-r--r--   0        0        0     1540 2024-04-16 18:30:46.789962 rate_control-2.0.0/rate_control/queues/_abc.py
+-rw-r--r--   0        0        0     1336 2024-04-16 18:30:46.789962 rate_control-2.0.0/rate_control/queues/_fifo.py
+-rw-r--r--   0        0        0     1311 2024-04-16 18:30:46.789962 rate_control-2.0.0/rate_control/queues/_lifo.py
+-rw-r--r--   0        0        0     1658 2024-04-16 18:30:46.789962 rate_control-2.0.0/rate_control/queues/_priority.py
+-rw-r--r--   0        0        0     5042 1970-01-01 00:00:00.000000 rate_control-2.0.0/PKG-INFO
```

### Comparing `rate_control-1.1.0/LICENSE` & `rate_control-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rate_control-1.1.0/README.rst` & `rate_control-2.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `rate_control-1.1.0/pyproject.toml` & `rate_control-2.0.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rate-control"
-version = "1.1.0"
+version = "2.0.0"
 description = "Versatile rate controlling in Python"
 authors = ["Corentin Régent <corentin.regent.pro@gmail.com>"]
 license = "MIT"
 
 homepage = "https://github.com/corentin-regent/rate-control"
 repository = "https://github.com/corentin-regent/rate-control"
 documentation = "https://rate-control.readthedocs.io/"
@@ -36,55 +36,56 @@
 ]
 
 [tool.poetry.urls]
 Changelog = "https://rate-control.readthedocs.io/en/latest/changelog.html"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-anyio = "^4"
-typing_extensions = {version = "^4.4", python = "<3.12"}
+anyio = "^4.0.0"
+typing_extensions = {version = "^4.4.0", python = "<3.12"}
 
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 anyio = {version = "*", extras = ["trio"]}
 mypy = "^1.6"
-ruff = "^0.2"
+ruff = "^0.3.0"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
 aiofastforward = "^0.0.26"
 anyio = {version = "*", extras = ["trio"]}
-coverage = {version = "^7", extras = ["toml"]}
-pytest = "^8"
-pytest-subtests = "^0.11"
+coverage = {version = "^7.0.0", extras = ["toml"]}
+pytest = "^8.0.0"
+pytest-subtests = "^0.11.0"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
-enum_tools = {version = "^0.11", extras=["sphinx"]}
+enum_tools = {version = "^0.11.0", extras=["sphinx"]}
 furo = "==2024.01.29"
-sphinx = "^7"
-sphinx-autodoc-typehints = "^1.21.2"
+sphinx = "^7.0.0"
+sphinx-autodoc-typehints = "^2.0.0"
 sphinx-tabs = "^3.4.2"
 
 
 [tool.coverage.run]
 branch = true
 
 [tool.coverage.report]
 show_missing = true
 skip_covered = true
 exclude_also = [
-    "if TYPE_CHECKING:"
+    "if TYPE_CHECKING:",
+    "^ +\\.{3}$",  # Lone ellipsis
 ]
 
 [tool.mypy]
 strict = true
 enable_error_code = "explicit-override"
 
 [[tool.mypy.overrides]]
```

### Comparing `rate_control-1.1.0/rate_control/_bucket_group.py` & `rate_control-2.0.0/rate_control/_bucket_group.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,38 @@
 __all__ = [
     'BucketGroup',
 ]
 
 import sys
 from contextlib import AsyncExitStack, suppress
-from typing import Any
+from typing import Any, Iterator
 
 from anyio import WouldBlock, create_memory_object_stream, create_task_group
 
+from rate_control._buckets import Bucket
 from rate_control._helpers import mk_repr
 from rate_control._helpers._validation import validate_buckets
-from rate_control.buckets import Bucket
+
+if sys.version_info >= (3, 9):
+    from collections.abc import Iterable
+else:
+    from typing import Iterable
 
 if sys.version_info >= (3, 11):
     from typing import Self
 else:
     from typing_extensions import Self
 
 if sys.version_info >= (3, 12):
     from typing import override
 else:
     from typing_extensions import override
 
 
-class BucketGroup(Bucket):
+class BucketGroup(Bucket, Iterable[Bucket]):
     """Bucket that aggregates other buckets."""
 
     def __init__(self, *buckets: Bucket, should_enter_context: bool = True, **kwargs: Any) -> None:
         """
         Args:
             buckets: The buckets to aggregate within this bucket group.
             should_enter_context: Whether entering the context of the bucket group
@@ -52,14 +57,18 @@
         return self
 
     @override
     async def __aexit__(self, *exc_info: Any) -> bool:
         self._task_group.cancel_scope.cancel()
         return await self._stack.__aexit__(*exc_info)
 
+    @override
+    def __iter__(self) -> Iterator[Bucket]:
+        return iter(self._buckets)
+
     async def _init_buckets(self) -> None:
         for bucket in self._buckets:
             if self._should_enter_context:
                 await self._stack.enter_async_context(bucket)
             self._listen_for_refill(bucket)
 
     def _listen_for_refill(self, bucket: Bucket) -> None:
```

### Comparing `rate_control-1.1.0/rate_control/_controllers/_limiter.py` & `rate_control-2.0.0/rate_control/_controllers/_rate_limiter.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 __all__ = [
     'RateLimiter',
 ]
 
 import sys
-from contextlib import contextmanager
+from contextlib import asynccontextmanager
 
-from rate_control._controllers._base import RateController
+from rate_control._controllers._abc import RateController
 
 if sys.version_info >= (3, 9):
-    from collections.abc import Iterator
+    from collections.abc import AsyncIterator
 else:
-    from typing import Iterator
+    from typing import AsyncIterator
+
+if sys.version_info >= (3, 12):
+    from typing import override
+else:
+    from typing_extensions import override
 
 
 class RateLimiter(RateController):
     """Rate controller that raises an error if a request cannot be fulfilled instantly."""
 
-    @contextmanager
-    def hold(self, tokens: float = 1) -> Iterator[None]:
+    @asynccontextmanager
+    @override
+    async def request(self, tokens: float = 1) -> AsyncIterator[None]:
         """Context manager that acquires the given amount of tokens while holding concurrency.
 
         Args:
             tokens: The number of tokens to acquire.
                 Defaults to `1`.
         Raises:
             RateLimit: The request cannot be fulfilled instantly.
```

### Comparing `rate_control-1.1.0/rate_control/_controllers/_scheduler.py` & `rate_control-2.0.0/rate_control/_controllers/_scheduler.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 import sys
 from contextlib import asynccontextmanager, contextmanager, suppress
 from typing import Any, NoReturn, Optional
 
 from anyio import create_task_group, get_cancelled_exc_class
 from anyio.lowlevel import checkpoint
 
-from rate_control._controllers._base import RateController
+from rate_control._buckets import Bucket
+from rate_control._controllers._abc import RateController
 from rate_control._enums import Priority
 from rate_control._errors import RateLimit, ReachedMaxPending
 from rate_control._helpers import Request, mk_repr
 from rate_control._helpers._validation import validate_max_pending
-from rate_control.buckets import Bucket
 from rate_control.queues import PriorityQueue, Queue
 
 if sys.version_info >= (3, 9):
     from collections.abc import AsyncIterator, Callable, Iterator
 else:
     from typing import AsyncIterator, Callable, Iterator
 
@@ -30,80 +30,90 @@
 if sys.version_info >= (3, 12):
     from typing import override
 else:
     from typing_extensions import override
 
 
 class Scheduler(RateController):
-    """Rate controller that schedule requests for later processing."""
+    """Rate controller that schedules requests for later processing."""
 
     def __init__(
         self,
-        bucket: Bucket,
+        *buckets: Bucket,
+        should_enter_context: bool = True,
         max_concurrency: Optional[int] = None,
         max_pending: Optional[int] = None,
         queue_factory: Callable[[], Queue[Request]] = PriorityQueue,
         **kwargs: Any,
     ) -> None:
         """
         Args:
-            bucket: The bucket that will be managed by the rate controller.
+            buckets: The buckets that will be managed by the rate controller.
+            should_enter_context: Whether entering the context of the rate controller
+                should also enter the context of the underlying buckets.
+                Defaults to True.
             max_concurrency: The maximum amount of concurrent requests allowed.
                 Defaults to `None` (no limit).
             max_pending: The maximum amount of requests waiting to be processed.
                 Defaults to `None` (no limit).
             queue_factory: The factory for initializing the request queues.
                 Defaults to :class:`.PriorityQueue`: requests are processed by ascending weight.
         """
-        super().__init__(bucket, max_concurrency, **kwargs)
+        super().__init__(*buckets, should_enter_context=should_enter_context, max_concurrency=max_concurrency, **kwargs)
         validate_max_pending(max_pending)
         self._max_pending = max_pending
         self._pending_requests = 0
         self._queues = [queue_factory() for _ in Priority]
         self._is_processing_requests = False
 
+    @override
     async def __aenter__(self) -> Self:
-        """Enter the scheduler's context.
-
-        Starts listening to the underlying bucket for replenishments.
-        """
+        await super().__aenter__()
         self._task_group = await create_task_group().__aenter__()
         self._task_group.start_soon(self._listen_to_refills)
         return self
 
     async def _listen_to_refills(self) -> NoReturn:
         """Process queued requests every time new tokens are available."""
         while True:
             await self._bucket.wait_for_refill()
             await self._process_queued_requests()
             await checkpoint()
 
-    async def __aexit__(self, *exc_info: Any) -> None:
-        """Exit the scheduler's context."""
+    @override
+    async def __aexit__(self, *exc_info: Any) -> Optional[bool]:
         self._task_group.cancel_scope.cancel()
         await self._task_group.__aexit__(*exc_info)
+        return await super().__aexit__(*exc_info)
 
     @override
     def __repr__(self) -> str:
-        return mk_repr(self, bucket=self._bucket, max_concurrency=self._max_concurrency, max_pending=self._max_pending)
+        return mk_repr(
+            self,
+            self._bucket,
+            should_enter_context=self._should_enter_context,
+            max_concurrency=self._max_concurrency,
+            max_pending=self._max_pending,
+        )
 
     @asynccontextmanager
-    async def schedule(
+    @override
+    async def request(
         self,
-        cost: float = 1,
+        tokens: float = 1,
         priority: Priority = Priority.NORMAL,
         fill_or_kill: bool = False,
     ) -> AsyncIterator[None]:
         """Asynchronous context manager that schedules the execution of the contained statements.
 
-        Waits until all the conditions of token disponibility and allowed concurrency are met,
+        Waits until all the conditions of token availability and allowed concurrency are met,
         before actually consuming tokens and holding a spot for the concurrency.
 
         Args:
-            cost: The number of tokens required for the request.
+            tokens: The number of tokens required for the request.
                 Defaults to `1`.
             priority: The priority of the request.
                 Requests with higher priority will be processed before the others.
                 Defaults to :py:enum:mem:`Priority.NORMAL`.
             fill_or_kill: Whether :exc:`RateLimit` should be raised
                 if the request cannot be process instantly.
                 Defaults to `False`.
@@ -111,20 +121,20 @@
         Raises:
             RateLimit: The request cannot be processed instantly
                 but the ``fill_or_kill`` flag was set to `True`.
             ReachedMaxPending: The limit of pending requests was reached.
         """
         if not hasattr(self, '_task_group'):
             raise RuntimeError(f"Make sure to enter the scheduler's context using 'async with {self}'")
-        if not self.can_acquire(cost):
+        if not self.can_acquire(tokens):
             if fill_or_kill:
-                raise RateLimit(f'Cannot process the request for {cost} tokens.')
+                raise RateLimit(f'Cannot process the request for {tokens} tokens.')
             else:
-                await self._request(cost, priority)
-        self._bucket.acquire(cost)
+                await self._perform_request(tokens, priority)
+        self._bucket.acquire(tokens)
         with self._hold_concurrency():
             yield
 
     @override
     def _on_concurrency_release(self) -> None:
         if self._max_concurrency is not None and self._concurrent_requests == self._max_concurrency - 1:
             self._task_group.start_soon(self._process_queued_requests)
@@ -159,15 +169,15 @@
         Tokens are not acquired directly in this method,
         in order to support request cancellation.
         """
         request = self._pop(queue)
         request.fire()
         await request.wait_for_ack()
 
-    async def _request(self, tokens: float, priority: Priority) -> None:
+    async def _perform_request(self, tokens: float, priority: Priority) -> None:
         """Perform a request to acquire the given amount of tokens, with the given priority.
 
         Args:
             tokens: The amount of tokens to acquire.
             priority: The request priority.
 
         Raises:
```

### Comparing `rate_control-1.1.0/rate_control/_helpers/_mk_repr.py` & `rate_control-2.0.0/rate_control/_helpers/_mk_repr.py`

 * *Files identical despite different names*

### Comparing `rate_control-1.1.0/rate_control/_helpers/_request.py` & `rate_control-2.0.0/rate_control/_helpers/_request.py`

 * *Files identical despite different names*

### Comparing `rate_control-1.1.0/rate_control/_helpers/_validation.py` & `rate_control-2.0.0/rate_control/_helpers/_validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 if sys.version_info >= (3, 9):
     from collections.abc import Collection
 else:
     from typing import Collection
 
 if TYPE_CHECKING:
-    from rate_control.buckets._base import Bucket
+    from rate_control._buckets import Bucket
 
 
 def validate_buckets(buckets: Collection[Bucket]) -> None:
     """
     Raises:
         ValueError: No bucket was provided.
     """
```

### Comparing `rate_control-1.1.0/rate_control/buckets/_base/_abc.py` & `rate_control-2.0.0/rate_control/_buckets/_base/_abc.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 if sys.version_info >= (3, 12):
     from typing import override
 else:
     from typing_extensions import override
 
 
 class Bucket(ABC):
-    """Abstract base class for all buckets."""
+    """Abstract base class for buckets."""
 
     async def __aenter__(self) -> Self:
         """Enter the bucket context.
 
         It may for example start scheduling replenishments.
         """
         return self
```

### Comparing `rate_control-1.1.0/rate_control/buckets/_base/_base_rate.py` & `rate_control-2.0.0/rate_control/_buckets/_base/_base_rate.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import sys
 from abc import ABC, abstractmethod
 from typing import Any, Optional
 
 from anyio import Event, create_task_group, sleep
 
+from rate_control._buckets._base._token_based import TokenBasedBucket
 from rate_control._helpers._validation import validate_delay
-from rate_control.buckets._base._token_based import TokenBasedBucket
 
 if sys.version_info >= (3, 11):
     from typing import Self
 else:
     from typing_extensions import Self
 
 if sys.version_info >= (3, 12):
```

### Comparing `rate_control-1.1.0/rate_control/buckets/_base/_capacity_updating.py` & `rate_control-2.0.0/rate_control/_buckets/_base/_capacity_updating.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 __all__ = [
     'CapacityUpdatingBucket',
 ]
 
+from rate_control._buckets._base._token_based import TokenBasedBucket
 from rate_control._helpers._validation import validate_capacity
-from rate_control.buckets._base._token_based import TokenBasedBucket
 
 
 class CapacityUpdatingBucket(TokenBasedBucket):
     """Mixin for buckets which token capacity can be updated."""
 
     def update_capacity(self, new_capacity: float) -> None:
         """Update the bucket's token capacity.
```

### Comparing `rate_control-1.1.0/rate_control/buckets/_base/_token_based.py` & `rate_control-2.0.0/rate_control/_buckets/_base/_token_based.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,16 +2,16 @@
     'TokenBasedBucket',
 ]
 
 import sys
 from abc import ABC
 from typing import Any
 
+from rate_control._buckets._base._abc import Bucket
 from rate_control._helpers._validation import validate_capacity, validate_tokens
-from rate_control.buckets._base._abc import Bucket
 
 if sys.version_info >= (3, 12):
     from typing import override
 else:
     from typing_extensions import override
```

### Comparing `rate_control-1.1.0/rate_control/buckets/_base/_windowed.py` & `rate_control-2.0.0/rate_control/_buckets/_base/_windowed.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,16 @@
     'BaseWindowedTokenBucket',
 ]
 
 import sys
 from abc import ABC
 from typing import Any
 
+from rate_control._buckets._base._base_rate import BaseRateBucket
 from rate_control._helpers import mk_repr
-from rate_control.buckets._base._base_rate import BaseRateBucket
 
 if sys.version_info >= (3, 12):
     from typing import override
 else:
     from typing_extensions import override
```

### Comparing `rate_control-1.1.0/rate_control/buckets/_fixed_window_counter.py` & `rate_control-2.0.0/rate_control/_buckets/_fixed_window_counter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 __all__ = [
     'FixedWindowCounter',
 ]
 
 import sys
 from typing import Any
 
-from rate_control.buckets._base import BaseWindowedTokenBucket, CapacityUpdatingBucket
+from rate_control._buckets._base import BaseWindowedTokenBucket, CapacityUpdatingBucket
 
 if sys.version_info >= (3, 12):
     from typing import override
 else:
     from typing_extensions import override
```

### Comparing `rate_control-1.1.0/rate_control/buckets/_leaky_bucket.py` & `rate_control-2.0.0/rate_control/_buckets/_leaky_bucket.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,17 +2,17 @@
     'LeakyBucket',
 ]
 
 import math
 import sys
 from typing import Any
 
+from rate_control._buckets._base import BaseRateBucket
 from rate_control._errors import RateLimit
 from rate_control._helpers import mk_repr
-from rate_control.buckets._base import BaseRateBucket
 
 if sys.version_info >= (3, 12):
     from typing import override
 else:
     from typing_extensions import override
```

### Comparing `rate_control-1.1.0/rate_control/buckets/_sliding_window_log.py` & `rate_control-2.0.0/rate_control/_buckets/_sliding_window_log.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 __all__ = [
     'SlidingWindowLog',
 ]
 
 import sys
 
-from rate_control.buckets._base import BaseWindowedTokenBucket, CapacityUpdatingBucket
+from rate_control._buckets._base import BaseWindowedTokenBucket, CapacityUpdatingBucket
 
 if sys.version_info >= (3, 12):
     from typing import override
 else:
     from typing_extensions import override
```

### Comparing `rate_control-1.1.0/rate_control/buckets/_unlimited.py` & `rate_control-2.0.0/rate_control/_buckets/_unlimited.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
     'UnlimitedBucket',
 ]
 
 import sys
 
 from anyio import sleep_forever
 
-from rate_control.buckets._base._abc import Bucket
+from rate_control._buckets._base import Bucket
 
 if sys.version_info >= (3, 12):
     from typing import override
 else:
     from typing_extensions import override
```

### Comparing `rate_control-1.1.0/rate_control/queues/_abc.py` & `rate_control-2.0.0/rate_control/queues/_abc.py`

 * *Files identical despite different names*

### Comparing `rate_control-1.1.0/rate_control/queues/_fifo.py` & `rate_control-2.0.0/rate_control/queues/_fifo.py`

 * *Files identical despite different names*

### Comparing `rate_control-1.1.0/rate_control/queues/_lifo.py` & `rate_control-2.0.0/rate_control/queues/_lifo.py`

 * *Files identical despite different names*

### Comparing `rate_control-1.1.0/rate_control/queues/_priority.py` & `rate_control-2.0.0/rate_control/queues/_priority.py`

 * *Files identical despite different names*

### Comparing `rate_control-1.1.0/PKG-INFO` & `rate_control-2.0.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rate-control
-Version: 1.1.0
+Version: 2.0.0
 Summary: Versatile rate controlling in Python
 Home-page: https://github.com/corentin-regent/rate-control
 License: MIT
 Keywords: async,rate limit,schedule,throttle,token bucket
 Author: Corentin Régent
 Author-email: corentin.regent.pro@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -18,16 +18,16 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
-Requires-Dist: anyio (>=4,<5)
-Requires-Dist: typing_extensions (>=4.4,<5.0) ; python_version < "3.12"
+Requires-Dist: anyio (>=4.0.0,<5.0.0)
+Requires-Dist: typing_extensions (>=4.4.0,<5.0.0) ; python_version < "3.12"
 Project-URL: Changelog, https://rate-control.readthedocs.io/en/latest/changelog.html
 Project-URL: Documentation, https://rate-control.readthedocs.io/
 Project-URL: Repository, https://github.com/corentin-regent/rate-control
 Description-Content-Type: text/x-rst
 
 ============
 Rate Control
```

