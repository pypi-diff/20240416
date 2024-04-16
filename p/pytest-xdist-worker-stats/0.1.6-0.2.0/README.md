# Comparing `tmp/pytest_xdist_worker_stats-0.1.6.tar.gz` & `tmp/pytest_xdist_worker_stats-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_xdist_worker_stats-0.1.6.tar", max compression
+gzip compressed data, was "pytest_xdist_worker_stats-0.2.0.tar", max compression
```

## Comparing `pytest_xdist_worker_stats-0.1.6.tar` & `pytest_xdist_worker_stats-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1071 2024-04-11 14:39:31.042688 pytest_xdist_worker_stats-0.1.6/LICENSE
--rw-r--r--   0        0        0     2305 2024-04-11 14:39:31.042688 pytest_xdist_worker_stats-0.1.6/README.md
--rw-r--r--   0        0        0     2963 2024-04-11 14:39:31.042688 pytest_xdist_worker_stats-0.1.6/pyproject.toml
--rw-r--r--   0        0        0       75 2024-04-11 14:39:31.042688 pytest_xdist_worker_stats-0.1.6/pytest_xdist_worker_stats/__init__.py
--rw-r--r--   0        0        0      937 2024-04-11 14:39:31.042688 pytest_xdist_worker_stats-0.1.6/pytest_xdist_worker_stats/options.py
--rw-r--r--   0        0        0     3639 2024-04-11 14:39:31.042688 pytest_xdist_worker_stats-0.1.6/pytest_xdist_worker_stats/plugin.py
--rw-r--r--   0        0        0     3400 1970-01-01 00:00:00.000000 pytest_xdist_worker_stats-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-04-16 21:35:55.873459 pytest_xdist_worker_stats-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3165 2024-04-16 21:35:55.873459 pytest_xdist_worker_stats-0.2.0/README.md
+-rw-r--r--   0        0        0     2963 2024-04-16 21:35:55.873459 pytest_xdist_worker_stats-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      118 2024-04-16 21:35:55.873459 pytest_xdist_worker_stats-0.2.0/pytest_xdist_worker_stats/__init__.py
+-rw-r--r--   0        0        0     1003 2024-04-16 21:35:55.873459 pytest_xdist_worker_stats-0.2.0/pytest_xdist_worker_stats/options.py
+-rw-r--r--   0        0        0     4433 2024-04-16 21:35:55.873459 pytest_xdist_worker_stats-0.2.0/pytest_xdist_worker_stats/plugin.py
+-rw-r--r--   0        0        0     4254 1970-01-01 00:00:00.000000 pytest_xdist_worker_stats-0.2.0/PKG-INFO
```

### Comparing `pytest_xdist_worker_stats-0.1.6/LICENSE` & `pytest_xdist_worker_stats-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_xdist_worker_stats-0.1.6/pyproject.toml` & `pytest_xdist_worker_stats-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytest-xdist-worker-stats"
-version = "0.1.6"
+version = "0.2.0"
 description = "A pytest plugin to list worker statistics after a xdist run."
 authors = ["Mikuláš Poul <mikulaspoul@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pytest_xdist_worker_stats"}]
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -25,16 +25,16 @@
 keywords = ["pytest", "xdist", "pytest-xdist"]
 
 [tool.poetry.plugins."pytest11"]
 pytest-xdist-worker-stats = "pytest_xdist_worker_stats"
 
 [tool.poetry.dependencies]
 python = ">=3.8"
-pytest = ">7.3.2"
-pytest-xdist = "^3.3"
+pytest = ">=7.0.0"
+pytest-xdist = ">=3"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.9.1"
 ruff = "^0.0.291"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `pytest_xdist_worker_stats-0.1.6/pytest_xdist_worker_stats/plugin.py` & `pytest_xdist_worker_stats-0.2.0/pytest_xdist_worker_stats/plugin.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,101 +1,113 @@
 import os
 import time
 from typing import NamedTuple
 
 import pytest
+from _pytest.terminal import TerminalReporter
+
+ARGPARSE_PARSER_GROUP = "pytest-xdist-worker-stats"
+ARGPARSE_REPORT_WORKER_RUNTIMES_OPTION_NAME = "pytest_xdist_worker_stats_report_worker_runtimes"
+ARGPARSE_REPORT_TEST_BREAKDOWN_OPTION_NAME = "pytest_xdist_worker_stats_report_test_breakdown"
 
 SHARED_WORKER_INFO = "worker_info"
 
 
-class RunStatistics(NamedTuple):
+class RuntimeStats(NamedTuple):
     mininum_tests: int
     maximum_tests: int
     average_tests: float
     mininum_runtime: float
     maximum_runtime: float
     average_runtime: float
 
 
 class XdistWorkerStatsPlugin:
-    def __init__(self, config):
+    def __init__(self, config: pytest.Config):
         self.config = config
         self.test_stats = {}
-        self.worker_test_times = {}
+        self.worker_stats = {}
+        self.report_worker_runtimes = config.getoption(ARGPARSE_REPORT_WORKER_RUNTIMES_OPTION_NAME, False)
+        self.report_test_breakdown = config.getoption(ARGPARSE_REPORT_TEST_BREAKDOWN_OPTION_NAME, False)
 
     def add(self, name):
         self.test_stats[name] = self.test_stats.get(name) or {}
         return self.test_stats[name]
 
     def pytest_runtest_setup(self, item):
         self.add(item.nodeid)["start"] = time.time()
 
     @pytest.hookimpl(hookwrapper=True)
     def pytest_runtest_call(self, item):
         yield
-        end = time.time()
-        self.add(item.nodeid)["diff"] = end - self.add(item.nodeid)["start"]
+        runtime = time.time() - self.add(item.nodeid)["start"]
+        self.add(item.nodeid)["runtime"] = runtime
 
-        if (worker := os.environ.get("PYTEST_XDIST_WORKER", "primary")) not in self.worker_test_times:
-            self.worker_test_times[worker] = []
+        if (worker := os.environ.get("PYTEST_XDIST_WORKER", "primary")) not in self.worker_stats:
+            self.worker_stats[worker] = {}
 
-        self.worker_test_times[worker].append(self.add(item.nodeid)["diff"])
+        self.worker_stats[worker][item.nodeid] = runtime
 
-    def get_statistics(self) -> RunStatistics:
-        workers = self.worker_test_times.keys()
-        tests = [len(self.worker_test_times[worker]) for worker in workers]
-        runtimes = [sum(self.worker_test_times[worker]) for worker in workers]
-
-        return RunStatistics(
-            mininum_tests=min(tests),
-            maximum_tests=max(tests),
-            average_tests=sum(tests) / len(tests),
-            mininum_runtime=min(runtimes),
-            maximum_runtime=max(runtimes),
-            average_runtime=sum(runtimes) / len(runtimes),
+    def get_runtime_stats(self) -> RuntimeStats:
+        test_counts = [len(stats) for stats in self.worker_stats.values()]
+        test_runtimes = [sum(stats.values()) for stats in self.worker_stats.values()]
+
+        return RuntimeStats(
+            mininum_tests=min(test_counts),
+            maximum_tests=max(test_counts),
+            average_tests=sum(test_counts) / len(test_counts),
+            mininum_runtime=min(test_runtimes),
+            maximum_runtime=max(test_runtimes),
+            average_runtime=sum(test_runtimes) / len(test_runtimes),
         )
 
-    def pytest_terminal_summary(self, terminalreporter):
+    def pytest_terminal_summary(self, terminalreporter: TerminalReporter):
         """
         If there's multiple workers, report on number of tests and total runtime.
         """
         tr = terminalreporter
-        if self.worker_test_times and len(self.worker_test_times) > 1:
+        if self.worker_stats and len(self.worker_stats) > 1:
             tr._tw.sep("=", "Worker statistics", yellow=True)
-            workers = sorted(self.worker_test_times.keys(), key=lambda x: int(x.lstrip("gw")))
-            statistics = self.get_statistics()
+            worker_columns = len(max(self.worker_stats.keys(), key=len)) + 2
 
-            for worker in workers:
-                worker_times = self.worker_test_times[worker]
-                tr._tw.line(f"worker {worker: <5}: {len(worker_times): >4} tests {sum(worker_times):10.2f}s runtime")
+            if self.report_worker_runtimes:
+                for worker, stats in sorted(self.worker_stats.items()):
+                    runtimes = stats.values()
+                    tr._tw.line(
+                        f"worker {worker: <{worker_columns}}: {len(runtimes): >4} tests {sum(runtimes):10.2f}s runtime"
+                    )
+                    if self.report_test_breakdown:
+                        for nodeid in sorted(stats.keys()):
+                            tr._tw.line(f"    {nodeid}")
+                tr._tw.line("")
 
-            tr._tw.line("")
+            runtime_stats = self.get_runtime_stats()
             tr._tw.line(
-                f"Tests   : min {statistics.mininum_tests: >8}, "
-                f"max {statistics.maximum_tests: >8}, "
-                f"average {statistics.average_tests:.1f}"
+                f"Tests   : min {runtime_stats.mininum_tests: >8}, "
+                f"max {runtime_stats.maximum_tests: >8}, "
+                f"average {runtime_stats.average_tests:.1f}"
             )
             tr._tw.line(
-                f"Runtime : min {statistics.mininum_runtime:7.2f}s, "
-                f"max {statistics.maximum_runtime:7.2f}s, "
-                f"average {statistics.average_runtime:.2f}s"
+                f"Runtime : min {runtime_stats.mininum_runtime:7.2f}s, "
+                f"max {runtime_stats.maximum_runtime:7.2f}s, "
+                f"average {runtime_stats.average_runtime:.2f}s"
             )
 
     def pytest_testnodedown(self, node, error):
         """
         Get statistic about worker usage for test cases from xdist nodes and merge to primary stats.
         """
         if (
             hasattr(node, "workeroutput")
             and (node_worker_stats := node.workeroutput.get(SHARED_WORKER_INFO)) is not None
         ):
-            self.worker_test_times.update(dict(node_worker_stats))
+            self.worker_stats.update(dict(node_worker_stats))
 
     @pytest.hookimpl(hookwrapper=True, trylast=True)
     def pytest_sessionfinish(self, session, exitstatus):
         """
         Dump worker usage statistics to `workeroutput`.
         Executed once per node if with xdist and will gen from primary node.
         """
         yield
         if hasattr(self.config, "workeroutput"):
-            self.config.workeroutput[SHARED_WORKER_INFO] = self.worker_test_times
+            self.config.workeroutput[SHARED_WORKER_INFO] = self.worker_stats
```

