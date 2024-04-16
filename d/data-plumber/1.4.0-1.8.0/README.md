# Comparing `tmp/data-plumber-1.4.0.tar.gz` & `tmp/data-plumber-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data-plumber-1.4.0.tar", last modified: Thu Feb  1 22:39:11 2024, max compression
+gzip compressed data, was "data-plumber-1.8.0.tar", last modified: Sat Feb  3 16:25:04 2024, max compression
```

## Comparing `data-plumber-1.4.0.tar` & `data-plumber-1.8.0.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-01 22:39:11.685601 data-plumber-1.4.0/
--rwxrwxrwx   0 root         (0) root         (0)     1080 2024-01-22 19:31:33.000000 data-plumber-1.4.0/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)     2514 2024-02-01 22:39:11.685432 data-plumber-1.4.0/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     2053 2024-01-31 22:17:36.000000 data-plumber-1.4.0/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-01 22:39:11.683215 data-plumber-1.4.0/data_plumber/
--rwxrwxrwx   0 root         (0) root         (0)      335 2024-02-01 22:39:06.000000 data-plumber-1.4.0/data_plumber/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     2232 2024-01-31 22:17:36.000000 data-plumber-1.4.0/data_plumber/array.py
--rwxrwxrwx   0 root         (0) root         (0)     1007 2024-02-01 22:39:06.000000 data-plumber-1.4.0/data_plumber/context.py
--rwxrwxrwx   0 root         (0) root         (0)      184 2024-01-31 22:17:36.000000 data-plumber-1.4.0/data_plumber/error.py
--rwxrwxrwx   0 root         (0) root         (0)     2204 2024-02-01 22:39:06.000000 data-plumber-1.4.0/data_plumber/fork.py
--rwxrwxrwx   0 root         (0) root         (0)     1931 2024-02-01 22:39:06.000000 data-plumber-1.4.0/data_plumber/output.py
--rwxrwxrwx   0 root         (0) root         (0)    12049 2024-02-01 22:39:06.000000 data-plumber-1.4.0/data_plumber/pipeline.py
--rwxrwxrwx   0 root         (0) root         (0)     4188 2024-02-01 22:39:06.000000 data-plumber-1.4.0/data_plumber/ref.py
--rwxrwxrwx   0 root         (0) root         (0)     4552 2024-02-01 22:39:06.000000 data-plumber-1.4.0/data_plumber/stage.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-01 22:39:11.684967 data-plumber-1.4.0/data_plumber.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     2514 2024-02-01 22:39:11.000000 data-plumber-1.4.0/data_plumber.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      374 2024-02-01 22:39:11.000000 data-plumber-1.4.0/data_plumber.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2024-02-01 22:39:11.000000 data-plumber-1.4.0/data_plumber.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       13 2024-02-01 22:39:11.000000 data-plumber-1.4.0/data_plumber.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       38 2024-02-01 22:39:11.685693 data-plumber-1.4.0/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      994 2024-02-01 22:39:06.000000 data-plumber-1.4.0/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-03 16:25:04.931026 data-plumber-1.8.0/
+-rwxrwxrwx   0 root         (0) root         (0)     1080 2024-01-22 19:31:33.000000 data-plumber-1.8.0/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)       30 2024-02-03 16:24:40.000000 data-plumber-1.8.0/MANIFEST.in
+-rwxrwxrwx   0 root         (0) root         (0)     3882 2024-02-03 16:25:04.930871 data-plumber-1.8.0/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     2053 2024-01-31 22:17:36.000000 data-plumber-1.8.0/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-03 16:25:04.929172 data-plumber-1.8.0/data_plumber/
+-rwxrwxrwx   0 root         (0) root         (0)      483 2024-02-03 16:24:40.000000 data-plumber-1.8.0/data_plumber/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     2232 2024-01-31 22:17:36.000000 data-plumber-1.8.0/data_plumber/array.py
+-rwxrwxrwx   0 root         (0) root         (0)     1064 2024-02-03 16:24:40.000000 data-plumber-1.8.0/data_plumber/context.py
+-rwxrwxrwx   0 root         (0) root         (0)      184 2024-01-31 22:17:36.000000 data-plumber-1.8.0/data_plumber/error.py
+-rwxrwxrwx   0 root         (0) root         (0)     2508 2024-02-03 16:24:40.000000 data-plumber-1.8.0/data_plumber/fork.py
+-rwxrwxrwx   0 root         (0) root         (0)     2408 2024-02-03 16:24:40.000000 data-plumber-1.8.0/data_plumber/output.py
+-rwxrwxrwx   0 root         (0) root         (0)    12283 2024-02-03 16:24:40.000000 data-plumber-1.8.0/data_plumber/pipeline.py
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-02-03 16:24:40.000000 data-plumber-1.8.0/data_plumber/py.typed
+-rwxrwxrwx   0 root         (0) root         (0)     9360 2024-02-03 16:24:40.000000 data-plumber-1.8.0/data_plumber/ref.py
+-rwxrwxrwx   0 root         (0) root         (0)     5945 2024-02-03 16:24:40.000000 data-plumber-1.8.0/data_plumber/stage.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-03 16:25:04.930492 data-plumber-1.8.0/data_plumber.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     3882 2024-02-03 16:25:04.000000 data-plumber-1.8.0/data_plumber.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      408 2024-02-03 16:25:04.000000 data-plumber-1.8.0/data_plumber.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2024-02-03 16:25:04.000000 data-plumber-1.8.0/data_plumber.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       13 2024-02-03 16:25:04.000000 data-plumber-1.8.0/data_plumber.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       38 2024-02-03 16:25:04.931107 data-plumber-1.8.0/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1261 2024-02-03 16:24:40.000000 data-plumber-1.8.0/setup.py
```

### Comparing `data-plumber-1.4.0/LICENSE` & `data-plumber-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `data-plumber-1.4.0/PKG-INFO` & `data-plumber-1.8.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: data-plumber
-Version: 1.4.0
-Summary: lightweight but versatile python-framework for multi-stage information processing
-Home-page: https://pypi.org/project/data-plumber/
-Author: Steffen Richters-Finger
-Author-email: srichters@uni-muenster.de
-License: MIT
-Project-URL: Source, https://github.com/RichtersFinger/data-plumber
-Platform: UNKNOWN
-Requires-Python: >=3.10, <4
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ![Tests](https://github.com/RichtersFinger/data-plumber/actions/workflows/tests.yml/badge.svg?branch=main)
 
 # data-plumber
 `data-plumber` is a lightweight but versatile python-framework for multi-stage
 information processing. It allows to construct processing pipelines from both
 atomic building blocks and via recombination of existing pipelines. Forks
 enable more complex (i.e. non-linear) orders of execution. Pipelines can also
@@ -54,9 +40,7 @@
 >>> pipeline.run(**{"data": 1}).stages
 [('', 0), ('bad type', 1)]
 >>> pipeline.run(**{"data": [1, "2", 3]}).stages
 [('', 0), ('', 0), ('bad type in data', 1)]
 >>> pipeline.run(**{"data": [1, 2, 3]}).stages
 [('', 0), ('', 0), ('validation success', 0)]
 ```
-
-
```

### Comparing `data-plumber-1.4.0/data_plumber/array.py` & `data-plumber-1.8.0/data_plumber/array.py`

 * *Files identical despite different names*

### Comparing `data-plumber-1.4.0/data_plumber/context.py` & `data-plumber-1.8.0/data_plumber/context.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,20 +18,22 @@
     `stage.StageRef` classes.
 
     Properties:
     stages -- list of string identifiers of `Pipeline`-components in
               order of their registration (= order of execution with
               `Fork`s)
     current_position -- index of current position in stages
+    loop -- `loop`-property of `Pipeline`
     records -- list of previous `_StageRecord`s for the current
                `Pipeline.run`
     kwargs -- kwargs passed to `Pipeline.run`
     out -- persistent data-object passed through a `Pipeline`
     count -- index of previously executed `Stage`s
     """
 
     stages: list[str]
     current_position: int
+    loop: bool
     records: list[_StageRecord]
     kwargs: dict[str, Any]
     out: Any
     count: int
```

### Comparing `data-plumber-1.4.0/data_plumber/fork.py` & `data-plumber-1.8.0/data_plumber/fork.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 in a `Pipeline.run`.
 """
 
 from typing import Callable, Optional
 from uuid import uuid4
 
 from .context import PipelineContext
-from .ref import StageRef
+from .ref import StageRef, StageById, StageByIncrement
 
 
 class Fork:
     """
     A `Fork` can be inserted into a `Pipeline` to control flow/execution
     order of a `Pipeline.run(...)`-command. This class is not indended
     for direct use, but taylored to be integrated into a `Pipeline`. It
@@ -52,20 +52,27 @@
         self._id = str(uuid4())
 
     @property
     def id(self) -> str:
         """Returns a `Stage`'s `id`."""
         return self._id
 
-    def eval(self, context: PipelineContext) \
-            -> Optional[StageRef | str | int]:
+    def eval(self, context: PipelineContext) -> Optional[StageRef]:
         """
-        Returns the value from evaluation of the `Fork`s conditional
+        Returns a `StageRef` or `None` as given with `Fork`s conditional
         function.
 
         Keyword arguments:
         context -- `Pipeline` execution context
         """
 
-        return self._fork(
+        result = self._fork(
             **context.kwargs, out=context.out, count=context.count
         )
+
+        # replace int or string by corresponding StageRef.
+        if isinstance(result, str):
+            return StageById(result)
+        if isinstance(result, int):
+            return StageByIncrement(result)
+        # otherwise it is either a StageRef already or None
+        return result
```

### Comparing `data-plumber-1.4.0/data_plumber/output.py` & `data-plumber-1.8.0/data_plumber/output.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,16 +5,38 @@
 `Pipeline.run`.
 """
 
 from typing import TypeAlias, Any, Optional
 from dataclasses import dataclass
 
 
-_StageRecord: TypeAlias = tuple[str, str, int]
-"""Tuple of `Stage`-identifier and evaluated message and status."""
+@dataclass
+class _StageRecord:
+    """
+    Record of a `Stage`'s execution result.
+
+    Keyword arguments:
+    index -- position in `Pipeline`'s list of `Stage`s
+    id_ -- `Stage` identifier (in `Pipeline`)
+    message -- string returned by `Stage`'s `message`-`Callable`
+    status -- int returned by `Stage`'s `status`-`Callable`
+    """
+    index: int
+    id_: str
+    message: str
+    status: int
+
+    def prune(self) -> "StageRecord":
+        """
+        Returns pruned `_StageRecord` containing only message and
+        status.
+        """
+        return (self.message, self.status)
+
+
 StageRecord: TypeAlias = tuple[str, int]
 """Tuple of message and status from a `Stage`'s-evaluation."""
 
 
 @dataclass
 class PipelineOutput:
     """
```

### Comparing `data-plumber-1.4.0/data_plumber/pipeline.py` & `data-plumber-1.8.0/data_plumber/pipeline.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 # data_plumber/pipeline.py
 
 The `pipeline`-module defines the `Pipeline`-class as the core-component
 of the data-plumber-framework.
 """
 
 from typing import Optional, Callable, Any, Iterator
+from functools import wraps
 from uuid import uuid4
 
 from .context import PipelineContext
 from .error import PipelineError
 from .output import _StageRecord, PipelineOutput
 from .fork import Fork
-from .ref import StageRef
 from .stage import Stage
 
 
 class Pipeline:
     """
     A `Pipeline` provides the core-functionality of the `data-plumber`-
     framework. `Pipeline`s can be defined either with (explicitly) named
@@ -89,40 +89,31 @@
             if isinstance(s, str):
                 continue
             self._stage_catalog.update({str(s): s})
 
     def _meets_requirements(self, _s: str, context: PipelineContext) -> bool:
         s = self._stage_catalog[_s]
         for ref, req in s.requires.items():  # type: ignore[union-attr]
-            match_status = None
-            if isinstance(ref, str):  # by identifier
-                # find latest status of Stage with this identifier
-                ref_record = next(
-                    (stage for _, stage in enumerate(reversed(context.records))
-                        if stage[0] == ref),
-                    None
-                )
-                if ref_record is None:
-                    # this Stage has not been executed
-                    raise PipelineError(
-                        f"Referenced Stage '{ref}' (required by Stage"
-                        + f" '{_s}') has not been executed yet."
-                    )
-                match_status = ref_record[2]
-            else:  # by StageRef
-                ref_output = ref.get(
-                    context
+            # get target Stage from StageRef
+            ref_output = ref.get(
+                context
+            )
+            # get latest status of that Stage
+            match_status = next(
+                (stage.status for stage in reversed(context.records)
+                    if stage.id_ == ref_output.stage),
+                None
+            )
+            if match_status is None:
+                # this Stage does not exist or has not been executed
+                raise PipelineError(
+                    f"Referenced Stage '{ref_output.stage}' (required by Stage"
+                    + f" '{_s}') has not been executed yet. "
+                    + f"Records until error: {context.records}"
                 )
-                if ref_output is None or ref_output.status is None:
-                    # this Stage has not been executed
-                    raise PipelineError(
-                        f"Referenced Stage '{str(ref)}' (required by Stage"
-                        + f" '{_s}') has not been executed yet."
-                    )
-                match_status = ref_output.status
             if callable(req):
                 if not req(status=match_status):  # type: ignore[call-arg]
                     # requirement not met
                     return False
             else:
                 if match_status != req:
                     # requirement not met
@@ -130,14 +121,25 @@
         return True
 
     def _loop_index(self, index: int) -> int:
         if self._loop:  # loop by truncating index
             return index % len(self._pipeline)
         return index
 
+    def _validate_external_kwargs(self, **kwargs):
+        reserved_words = ["out", "primer", "status", "count"]
+        # check for reserved kwargs
+        if (bad_kwarg := next(
+            (p for p in kwargs if p in reserved_words),
+            None
+        )):
+            raise PipelineError(
+                f"Keyword '{bad_kwarg}' is reserved in the context of a "
+                + f"'Pipeline.run'-command. (Reserved words: {reserved_words})"
+            )
 
     @property
     def id(self) -> str:
         """Returns a `Pipeline`'s `id`."""
         return self._id
 
     @property
@@ -154,23 +156,15 @@
         """
         Trigger `Pipeline` execution.
 
         Keyword arguments:
         kwargs -- keyword arguments that are forwarded into `Stage`s
         """
 
-        # check for reserved kwargs
-        if (bad_kwarg := next(
-            (p for p in kwargs if p in ["out", "primer", "status", "count"]),
-            None
-        )):
-            raise PipelineError(
-                f"Keyword '{bad_kwarg}' is reserved in the context of a "
-                + "'Pipeline.run'-command."
-            )
+        self._validate_external_kwargs(**kwargs)
 
         records: list[_StageRecord] = []  # record of results
         data = self._initialize_output()  # output data
 
         stage_count = -1
         index = 0
         while True:
@@ -179,62 +173,46 @@
                 break
 
             _s = self._pipeline[index]
             try:
                 s = self._stage_catalog[_s]
             except KeyError as exc:
                 raise PipelineError(
-                    f"Unable to resolve reference to Stage '{_s}' at stage #{str(stage_count)}. "
-                    + f"Records until error: {', '.join(map(str, records))}"
+                    f"Unable to resolve reference to Stage id '{_s}' in Pipeline with " \
+                    + f"stages {self._pipeline}. Records until error: {records}"
                 ) from exc
             if isinstance(s, Fork):
                 # ##########
                 # Fork
-                fork_target = s.eval(
+                # get StageRef
+                stage_ref = s.eval(
                     PipelineContext(
-                        self._pipeline, index, records, kwargs, data, stage_count
+                        self._pipeline, index, self._loop, records, kwargs,
+                        data, stage_count
                     )
                 )
-                if fork_target is None:  # exit pipeline on request
+                if stage_ref is None:  # exit pipeline on request
                     break
-                if isinstance(fork_target, str):  # new index via index()
-                    try:
-                        index = self._pipeline.index(fork_target)
-                    except ValueError as exc:
-                        raise PipelineError(
-                            f"Unable to resolve reference to '{str(fork_target)}' at stage #{str(stage_count)}. "
-                            + f"Records until error: {', '.join(map(str, records))}"
-                        ) from exc
-                elif isinstance(fork_target, int):  # new index via addition
-                    index = self._loop_index(index + fork_target)
-                    if index < 0 or index >= len(self._pipeline):
-                        raise PipelineError(
-                            "Unable to resolve Fork reference (out of bounds). "
-                            + f"Records until error: {', '.join(map(str, records))}"
-                        )
-                else:  # new index via StageRef.get
-                    ref = fork_target.get(
-                        PipelineContext(
-                            self._pipeline, index, records, kwargs, data, stage_count
-                        )
+                # get target of StageRef
+                ref = stage_ref.get(
+                    PipelineContext(
+                        self._pipeline, index, self._loop, records, kwargs,
+                        data, stage_count
                     )
-                    if ref is None:
-                        raise PipelineError(
-                            f"Unable to resolve fork's StageRef '{str(ref)}' at stage #{str(stage_count)}. "
-                            + f"Records until error: {', '.join(map(str, records))}"
-                        )
-                    index = self._loop_index(index + ref.relative_index)
+                )
+                index = ref.index
                 continue
             # ##########
             # Stage
             # requires
             if s.requires is not None:
                 if not self._meets_requirements(
                     _s, PipelineContext(
-                        self._pipeline, index, records, kwargs, data, stage_count
+                        self._pipeline, index, self._loop, records, kwargs,
+                        data, stage_count
                     )
                 ):
                     index = index + 1
                     continue
             # all requirements met
             stage_count = stage_count + 1
             # primer
@@ -242,41 +220,84 @@
             # action
             s.action(
                 **kwargs,
                 out=data,
                 primer=primer,
                 count=stage_count
             )
+            exported_kwargs = s.export(
+                **kwargs,
+                out=data,
+                primer=primer,
+                count=stage_count
+            )
+            self._validate_external_kwargs(**exported_kwargs)
+            kwargs.update(exported_kwargs)
             # status/message
             status = s.status(
                 **kwargs,
                 out=data,
                 primer=primer,
                 count=stage_count
             )
             msg = s.message(
                 **kwargs,
                 out=data,
                 primer=primer,
                 count=stage_count,
                 status=status
             )
-            records.append((_s, msg, status))
+            records.append(_StageRecord(index, _s, msg, status))
             if self._exit_on_status(status):
                 break
             index = index + 1
 
         if self._finalize_output is not None:
             self._finalize_output(data=data, **kwargs)
         return PipelineOutput(
-            list(map(lambda x: x[1:], records)),  # trim _StageRecord
+            [r.prune() for r in records],  # prune `_StageRecord`s
             kwargs,
             data
         )
 
+    def run_for_kwargs(self, **kwargs):
+        """
+        Returns a decorator that can be used to generate kwargs for the
+        decorated function based on the output of a `Pipeline.run`. This
+        requires for the persistent data-object (`PipelineOutput.data`)
+        to be a mapping that can be unpacked as `**PipelineOutput.data`.
+
+        Using this decorator on a function and calling that function
+         >>> @pipeline.run_for_kwargs(...)
+             def f(...): ...
+         >>> f()
+        is equivalent to
+         >>> f(**pipeline.run(...).data)
+
+        Note that it is also possible to only generate a subset of all
+        keyword arguments to a target function or have the target also
+        require positional arguments (which then still have to be
+        provided explicitly to the decorated function). When makign a
+        call to the decorated function with kwargs that are also output
+        from the `Pipeline.run`, the explicitly given arguments take
+        priority.
+
+        Keyword arguments:
+        kwargs -- keyword arguments that are forwarded into
+                  `Pipeline.run`
+        """
+
+        def decorator(function):
+            @wraps(function)
+            def wrapped(*args, **_kwargs):
+                output = self.run(**kwargs)
+                return function(*args, **(output.data | _kwargs))
+            return wrapped
+        return decorator
+
     def append(self, element: "str | Stage | Fork | Pipeline") -> None:
         """Append `element` to the `Pipeline`."""
         if isinstance(element, Pipeline):
             self._update_catalog(**element.catalog)
             self._pipeline = self._pipeline + element.stages
             return
         self._update_catalog(element)
```

### Comparing `data-plumber-1.4.0/data_plumber/stage.py` & `data-plumber-1.8.0/data_plumber/stage.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 This module defines the `Stage`-class, a single data-processing unit of
 a `Pipeline`.
 """
 
 from typing import Optional, Callable, Any
 from uuid import uuid4
 
-from .ref import StageRef
+from .ref import StageRef, StageById, StageByIncrement
 
 
 class Stage:
     """
     A `Stage` represents a single building block in the processing logic
     of a `Pipeline`. The set of arguments which are passed to a
     `Stage`'s `Callable` kwargs are given by (for actual arguments
@@ -22,73 +22,101 @@
     * `out` (an object that is passed through the entire `Pipeline`; its
       initial value is generated by the `Pipeline`'s `initialize_output`
       kwarg),
     * `primer` (output of `Stage.primer`),
     * `status` (output of `Stage.status`),
     * `count` (index of `Stage` in execution of `Pipeline`)
 
+    `Callable`s are executed in the order:
+    `primer` > `action` > `export` > `status` > `message`
+
     Example usage:
      >>> from data_plumber import Stage
      >>> Stage(
              primer=lambda **kwargs: "data" in kwargs,
              status=lambda primer, **kwargs: int(primer),
              message=lambda primer, **kwargs:
                  "missing 'data'-argument" if not primer else ""
          )
      <data_plumber.stage.Stage object at ...>
 
     Keyword arguments:
-    requires -- requirements for `Stage`-execution; dictionary with keys
-                being either `None`, a `StageRef`, or `str` (identifier
-                of a `Stage` in the context of a `Pipeline`; uses most
-                recent evaluation) and values being either an integer
-                (required output status of the keyed `Stage`) or a
-                `Callable` taking the status as an argument and
-                returning a `bool` (if it evaluates to `True`, the
-                `Stage`-requirement is met); `PipelineError` is raised
-                if references `Stage` has not yet been executed
+    requires -- requirements for `Stage`-execution being either `None`
+                or a dictionary with pairs of some reference to a `Stage`
+                and the required status (uses most recent evaluation);
+
+                key types are either `StageRef`, `str` (identifier of a
+                `Stage` in the context of a `Pipeline`), or `int`
+                (relative index in `Pipeline` stage arrangement);
+
+                values are either an integer value or a `Callable`
+                taking the status as an argument and returning a `bool`
+                (if it evaluates to `True`, the `Stage`-requirement is
+                met); `PipelineError` is raised if referenced `Stage`
+                has not yet been executed
     primer -- `Callable` for pre-processing data
               (kwargs: `out`, `count`)
               (default `lambda **kwargs: None`)
     action -- `Callable` for main-step of processing
               (kwargs: `out`, `primer`, `count`)
               (default `lambda **kwargs: None`)
+    export -- `Callable` that returns a dictionary of additional kwargs
+              to be exported to the parent `Pipeline`; in the following
+              `Stage`s, these kwargs are then available as if they were
+              provided with the `Pipeline.run`-command
+              (kwargs: `out`, `primer`, `count`)
+              (default `lambda **kwargs: None`)
     status -- `Callable` for generation of `Stage`'s integer exit status
               (kwargs: `out`, `primer`, `count`)
               (default `lambda **kwargs: 0`)
     message -- `Callable` for generation of `Stage`'s exit message
                (kwargs: `out`, `primer`, `count`, `status`)
                (default `lambda **kwargs: ""`)
     """
 
     def __init__(
         self,
         requires: Optional[
-            dict[StageRef | str, int | Callable[[int], bool]]
+            dict[StageRef | str | int, int | Callable[[int], bool]]
         ] = None,
         primer: Callable[..., Any] = lambda **kwargs: None,
         action: Callable[..., Any] = lambda **kwargs: None,
+        export: Optional[Callable[..., Optional[dict[str, Any]]]] = None,
         status: Callable[..., int] = lambda **kwargs: 0,
         message: Callable[..., str] = lambda **kwargs: ""
     ) -> None:
-        self._requires = requires
+        if requires is None:
+            self._requires = None
+        else:
+            self._requires = {}
+            for k, v in requires.items():
+                if isinstance(k, str):
+                    self._requires[StageById(k)] = v
+                elif isinstance(k, int):
+                    self._requires[StageByIncrement(k)] = v
+                else:
+                    self._requires[k] = v
         self._primer = primer
         self._action = action
+        if export is None:
+            self._export: Callable[..., dict[str, Any]] = lambda **kwargs: {}
+        else:
+            self._export = export  # type: ignore[assignment]
         self._status = status
         self._message = message
         self._id = str(uuid4())
 
     @property
     def id(self) -> str:
         """Returns a `Stage`'s `id`."""
         return self._id
 
     @property
     def requires(self) -> Optional[
-        dict[StageRef | str, int | Callable[[int], bool]]
+        dict[StageRef, int | Callable[[int], bool]]
     ]:
         """Returns a `Stage`'s requirements."""
         return self._requires
 
     @property
     def primer(self) -> Callable[..., Any]:
         """Returns a `Stage`'s `primer` callable."""
@@ -96,14 +124,19 @@
 
     @property
     def action(self) -> Callable[..., Any]:
         """Returns a `Stage`'s `action` callable."""
         return self._action
 
     @property
+    def export(self) -> Callable[..., Any]:
+        """Returns a `Stage`'s `export` callable."""
+        return self._export
+
+    @property
     def status(self) -> Callable[..., int]:
         """Returns a `Stage`'s `status` callable."""
         return self._status
 
     @property
     def message(self) -> Callable[..., str]:
         """Returns a `Stage`'s `message` callable."""
```

### Comparing `data-plumber-1.4.0/data_plumber.egg-info/PKG-INFO` & `data-plumber-1.8.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-plumber
-Version: 1.4.0
+Version: 1.8.0
 Summary: lightweight but versatile python-framework for multi-stage information processing
 Home-page: https://pypi.org/project/data-plumber/
 Author: Steffen Richters-Finger
 Author-email: srichters@uni-muenster.de
 License: MIT
 Project-URL: Source, https://github.com/RichtersFinger/data-plumber
 Platform: UNKNOWN
@@ -56,7 +56,55 @@
 >>> pipeline.run(**{"data": [1, "2", 3]}).stages
 [('', 0), ('', 0), ('bad type in data', 1)]
 >>> pipeline.run(**{"data": [1, 2, 3]}).stages
 [('', 0), ('', 0), ('validation success', 0)]
 ```
 
 
+# Changelog
+
+## [1.8.0] - 2024-02-03
+
+### Changed
+
+- refactored `Fork` and `Stage` to transform string/integer-references to `Stage`s into `StageRef`s (`7ba677b`)
+
+### Added
+
+- added decorator-factory `Pipeline.run_for_kwargs` to generate kwargs for function calls (`fe616b2`)
+- added optional `Stage`-callable to export kwargs into `Pipeline.run` (`8eca1bc`)
+- added even more types of `StageRef`s: `PreviousN`, `NextN` (`576820c`)
+- added `py.typed`-marker to package (`04a2e1d`)
+- added more types of `StageRef`s: `StageById`, `StageByIndex`, `StageByIncrement` (`92d57ad`)
+
+## [1.4.0] - 2024-02-01
+
+### Changed
+
+- refactored internal modules (`cf7045f`)
+
+### Added
+
+- added `StageRefs` `Next`, `Last`, and `Skip` (`14abaa7`)
+- added optional finalizer-`Callable` to `Pipeline` (`d95e5b6`)
+- added support for `Callable` in `Pipeline`-argument `exit_on_status` (`154c67b`)
+
+### Fixed
+
+- `PipelineOutput.last_X`-methods now return `None` in case of empty records (``)
+
+## [1.0.0] - 2024-01-31
+
+### Changed
+
+- **Breaking:** refactor `PipelineOutput` and related types (`1436ca1`)
+- **Breaking:** replaced forwarding kwargs of `Pipeline.run` as dictionary `in_` into `Stage`/`Fork`-`Callable`s by forwarding directly (`f2710fa`, `b569bb9`)
+
+### Added
+
+- added missing information in module- and class-docstrings (`7896742`)
+
+## [0.1.0] - 2024-01-31
+
+initial release
+
+
```

### Comparing `data-plumber-1.4.0/setup.py` & `data-plumber-1.8.0/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,34 +1,43 @@
 from pathlib import Path
 from setuptools import setup
 
 # read contents of README
 long_description = \
     (Path(__file__).parent / "README.md").read_text(encoding="utf8")
+# read contents of CHANGELOG
+changelog = \
+    (Path(__file__).parent / "CHANGELOG.md").read_text(encoding="utf8")
 
 # read contents of requirements.txt
 requirements = \
     (Path(__file__).parent / "requirements.txt") \
         .read_text(encoding="utf8") \
         .strip() \
         .split("\n")
 
 setup(
-    version="1.4.0",
+    version="1.8.0",
     name="data-plumber",
     description="lightweight but versatile python-framework for multi-stage information processing",
-    long_description=long_description,
+    long_description=long_description + "\n\n" + changelog,
     long_description_content_type="text/markdown",
     author="Steffen Richters-Finger",
     author_email="srichters@uni-muenster.de",
     license="MIT",
     license_files=("LICENSE",),
     url="https://pypi.org/project/data-plumber/",
     project_urls={
         "Source": "https://github.com/RichtersFinger/data-plumber"
     },
     python_requires=">=3.10, <4",
     install_requires=requirements,
     packages=[
         "data_plumber",
     ],
+    package_data={
+        "data_plumber": [
+            "data_plumber/py.typed",
+        ],
+    },
+    include_package_data=True,
 )
```

