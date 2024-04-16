# Comparing `tmp/pygradflow-0.3.8.tar.gz` & `tmp/pygradflow-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygradflow-0.3.8.tar", max compression
+gzip compressed data, was "pygradflow-0.3.9.tar", max compression
```

## Comparing `pygradflow-0.3.8.tar` & `pygradflow-0.3.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0    10847 2024-01-23 13:10:51.093788 pygradflow-0.3.8/LICENSE
--rw-r--r--   0        0        0      984 2024-01-23 13:10:51.093788 pygradflow-0.3.8/README.md
--rw-r--r--   0        0        0        0 2024-01-23 13:10:51.093788 pygradflow-0.3.8/pygradflow/__init__.py
--rw-r--r--   0        0        0      872 2024-01-23 13:10:51.093788 pygradflow-0.3.8/pygradflow/active_set.py
--rw-r--r--   0        0        0     4458 2024-01-23 13:10:51.093788 pygradflow-0.3.8/pygradflow/cons_problem.py
--rw-r--r--   0        0        0     1749 2024-01-23 13:10:51.093788 pygradflow-0.3.8/pygradflow/controller.py
--rw-r--r--   0        0        0     2455 2024-01-23 13:10:51.093788 pygradflow-0.3.8/pygradflow/deriv_check.py
--rw-r--r--   0        0        0     3179 2024-01-23 13:10:51.093788 pygradflow-0.3.8/pygradflow/display.py
--rw-r--r--   0        0        0     4839 2024-01-23 13:10:51.093788 pygradflow-0.3.8/pygradflow/eval.py
--rw-r--r--   0        0        0     6308 2024-01-23 13:10:51.093788 pygradflow-0.3.8/pygradflow/implicit_func.py
--rw-r--r--   0        0        0     4701 2024-01-23 13:10:51.093788 pygradflow-0.3.8/pygradflow/iterate.py
--rw-r--r--   0        0        0       55 2024-01-23 13:10:51.093788 pygradflow-0.3.8/pygradflow/log.py
--rw-r--r--   0        0        0     6570 2024-01-23 13:10:51.093788 pygradflow-0.3.8/pygradflow/newton.py
--rw-r--r--   0        0        0     5061 2024-01-23 13:10:51.093788 pygradflow-0.3.8/pygradflow/params.py
--rw-r--r--   0        0        0     5104 2024-01-23 13:10:51.093788 pygradflow-0.3.8/pygradflow/penalty.py
--rw-r--r--   0        0        0     5850 2024-01-23 13:10:51.093788 pygradflow-0.3.8/pygradflow/problem.py
--rw-r--r--   0        0        0        0 2024-01-23 13:10:51.093788 pygradflow-0.3.8/pygradflow/py.typed
--rw-r--r--   0        0        0     3437 2024-01-23 13:10:51.093788 pygradflow-0.3.8/pygradflow/runners/cutest_runner.py
--rw-r--r--   0        0        0      366 2024-01-23 13:10:51.093788 pygradflow-0.3.8/pygradflow/runners/instance.py
--rw-r--r--   0        0        0     2045 2024-01-23 13:10:51.093788 pygradflow-0.3.8/pygradflow/runners/qplib_runner.py
--rw-r--r--   0        0        0     7240 2024-01-23 13:10:51.093788 pygradflow-0.3.8/pygradflow/runners/runner.py
--rw-r--r--   0        0        0    14696 2024-01-23 13:10:51.093788 pygradflow-0.3.8/pygradflow/solver.py
--rw-r--r--   0        0        0     1284 2024-01-23 13:10:51.093788 pygradflow-0.3.8/pygradflow/step/__init__.py
--rw-r--r--   0        0        0     4145 2024-01-23 13:10:51.093788 pygradflow-0.3.8/pygradflow/step/asymmetric_step_solver.py
--rw-r--r--   0        0        0     2696 2024-01-23 13:10:51.093788 pygradflow-0.3.8/pygradflow/step/cond_estimate.py
--rw-r--r--   0        0        0     2873 2024-01-23 13:10:51.097788 pygradflow-0.3.8/pygradflow/step/extended_step_solver.py
--rw-r--r--   0        0        0     2458 2024-01-23 13:10:51.097788 pygradflow-0.3.8/pygradflow/step/linear_solver.py
--rw-r--r--   0        0        0     2384 2024-01-23 13:10:51.097788 pygradflow-0.3.8/pygradflow/step/scaled_step_solver.py
--rw-r--r--   0        0        0     2147 2024-01-23 13:10:51.097788 pygradflow-0.3.8/pygradflow/step/standard_step_solver.py
--rw-r--r--   0        0        0     6966 2024-01-23 13:10:51.097788 pygradflow-0.3.8/pygradflow/step/step_control.py
--rw-r--r--   0        0        0     1819 2024-01-23 13:10:51.097788 pygradflow-0.3.8/pygradflow/step/step_solver.py
--rw-r--r--   0        0        0     3887 2024-01-23 13:10:51.097788 pygradflow-0.3.8/pygradflow/step/symmetric_step_solver.py
--rw-r--r--   0        0        0      232 2024-01-23 13:10:51.097788 pygradflow-0.3.8/pygradflow/util.py
--rw-r--r--   0        0        0      858 2024-01-23 13:10:51.097788 pygradflow-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     1767 1970-01-01 00:00:00.000000 pygradflow-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0    10847 2024-01-23 18:13:18.723216 pygradflow-0.3.9/LICENSE
+-rw-r--r--   0        0        0      984 2024-01-23 18:13:18.723216 pygradflow-0.3.9/README.md
+-rw-r--r--   0        0        0        0 2024-01-23 18:13:18.723216 pygradflow-0.3.9/pygradflow/__init__.py
+-rw-r--r--   0        0        0      872 2024-01-23 18:13:18.723216 pygradflow-0.3.9/pygradflow/active_set.py
+-rw-r--r--   0        0        0     4458 2024-01-23 18:13:18.723216 pygradflow-0.3.9/pygradflow/cons_problem.py
+-rw-r--r--   0        0        0     1749 2024-01-23 18:13:18.723216 pygradflow-0.3.9/pygradflow/controller.py
+-rw-r--r--   0        0        0     2455 2024-01-23 18:13:18.723216 pygradflow-0.3.9/pygradflow/deriv_check.py
+-rw-r--r--   0        0        0     3179 2024-01-23 18:13:18.723216 pygradflow-0.3.9/pygradflow/display.py
+-rw-r--r--   0        0        0     4839 2024-01-23 18:13:18.723216 pygradflow-0.3.9/pygradflow/eval.py
+-rw-r--r--   0        0        0     6308 2024-01-23 18:13:18.723216 pygradflow-0.3.9/pygradflow/implicit_func.py
+-rw-r--r--   0        0        0     4701 2024-01-23 18:13:18.727216 pygradflow-0.3.9/pygradflow/iterate.py
+-rw-r--r--   0        0        0       55 2024-01-23 18:13:18.727216 pygradflow-0.3.9/pygradflow/log.py
+-rw-r--r--   0        0        0     6570 2024-01-23 18:13:18.727216 pygradflow-0.3.9/pygradflow/newton.py
+-rw-r--r--   0        0        0     5099 2024-01-23 18:13:18.727216 pygradflow-0.3.9/pygradflow/params.py
+-rw-r--r--   0        0        0     5104 2024-01-23 18:13:18.727216 pygradflow-0.3.9/pygradflow/penalty.py
+-rw-r--r--   0        0        0     5850 2024-01-23 18:13:18.727216 pygradflow-0.3.9/pygradflow/problem.py
+-rw-r--r--   0        0        0        0 2024-01-23 18:13:18.727216 pygradflow-0.3.9/pygradflow/py.typed
+-rw-r--r--   0        0        0     3437 2024-01-23 18:13:18.727216 pygradflow-0.3.9/pygradflow/runners/cutest_runner.py
+-rw-r--r--   0        0        0      366 2024-01-23 18:13:18.727216 pygradflow-0.3.9/pygradflow/runners/instance.py
+-rw-r--r--   0        0        0     2045 2024-01-23 18:13:18.727216 pygradflow-0.3.9/pygradflow/runners/qplib_runner.py
+-rw-r--r--   0        0        0     7417 2024-01-23 18:13:18.727216 pygradflow-0.3.9/pygradflow/runners/runner.py
+-rw-r--r--   0        0        0    14851 2024-01-23 18:13:18.727216 pygradflow-0.3.9/pygradflow/solver.py
+-rw-r--r--   0        0        0     1284 2024-01-23 18:13:18.727216 pygradflow-0.3.9/pygradflow/step/__init__.py
+-rw-r--r--   0        0        0     4145 2024-01-23 18:13:18.727216 pygradflow-0.3.9/pygradflow/step/asymmetric_step_solver.py
+-rw-r--r--   0        0        0     2696 2024-01-23 18:13:18.727216 pygradflow-0.3.9/pygradflow/step/cond_estimate.py
+-rw-r--r--   0        0        0     2873 2024-01-23 18:13:18.727216 pygradflow-0.3.9/pygradflow/step/extended_step_solver.py
+-rw-r--r--   0        0        0     2458 2024-01-23 18:13:18.727216 pygradflow-0.3.9/pygradflow/step/linear_solver.py
+-rw-r--r--   0        0        0     2384 2024-01-23 18:13:18.727216 pygradflow-0.3.9/pygradflow/step/scaled_step_solver.py
+-rw-r--r--   0        0        0     2147 2024-01-23 18:13:18.727216 pygradflow-0.3.9/pygradflow/step/standard_step_solver.py
+-rw-r--r--   0        0        0     6966 2024-01-23 18:13:18.727216 pygradflow-0.3.9/pygradflow/step/step_control.py
+-rw-r--r--   0        0        0     1819 2024-01-23 18:13:18.727216 pygradflow-0.3.9/pygradflow/step/step_solver.py
+-rw-r--r--   0        0        0     3887 2024-01-23 18:13:18.727216 pygradflow-0.3.9/pygradflow/step/symmetric_step_solver.py
+-rw-r--r--   0        0        0      232 2024-01-23 18:13:18.727216 pygradflow-0.3.9/pygradflow/util.py
+-rw-r--r--   0        0        0      858 2024-01-23 18:13:18.727216 pygradflow-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0     1767 1970-01-01 00:00:00.000000 pygradflow-0.3.9/PKG-INFO
```

### Comparing `pygradflow-0.3.8/LICENSE` & `pygradflow-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pygradflow-0.3.8/README.md` & `pygradflow-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `pygradflow-0.3.8/pygradflow/active_set.py` & `pygradflow-0.3.9/pygradflow/active_set.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.3.8/pygradflow/cons_problem.py` & `pygradflow-0.3.9/pygradflow/cons_problem.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.3.8/pygradflow/controller.py` & `pygradflow-0.3.9/pygradflow/controller.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.3.8/pygradflow/deriv_check.py` & `pygradflow-0.3.9/pygradflow/deriv_check.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.3.8/pygradflow/display.py` & `pygradflow-0.3.9/pygradflow/display.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.3.8/pygradflow/eval.py` & `pygradflow-0.3.9/pygradflow/eval.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.3.8/pygradflow/implicit_func.py` & `pygradflow-0.3.9/pygradflow/implicit_func.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.3.8/pygradflow/iterate.py` & `pygradflow-0.3.9/pygradflow/iterate.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.3.8/pygradflow/newton.py` & `pygradflow-0.3.9/pygradflow/newton.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.3.8/pygradflow/params.py` & `pygradflow-0.3.9/pygradflow/params.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import dataclasses
 import enum
 from dataclasses import dataclass
 from enum import Enum, Flag, auto
+from typing import Optional
 
 import numpy as np
 
 
 class NewtonType(Enum):
     """
     The Newton method to be used to solve the semi-smooth systems.
@@ -163,15 +164,15 @@
     deriv_pert: float = 1e-8
     deriv_tol: float = 1e-4
 
     precision: Precision = Precision.Double
 
     validate_input: bool = True
 
-    iteration_limit: int = 1000
+    iteration_limit: Optional[int] = None
     time_limit: float = np.inf
     display_interval: float = 0.1
 
     # lower bound on objective function value,
     # used to detect unbounded problems
     obj_lower_limit: float = -1e10
```

### Comparing `pygradflow-0.3.8/pygradflow/penalty.py` & `pygradflow-0.3.9/pygradflow/penalty.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.3.8/pygradflow/problem.py` & `pygradflow-0.3.9/pygradflow/problem.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.3.8/pygradflow/runners/cutest_runner.py` & `pygradflow-0.3.9/pygradflow/runners/cutest_runner.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.3.8/pygradflow/runners/qplib_runner.py` & `pygradflow-0.3.9/pygradflow/runners/qplib_runner.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.3.8/pygradflow/runners/runner.py` & `pygradflow-0.3.9/pygradflow/runners/runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,19 @@
     try:
         handler = logging.FileHandler(log_filename)
         handler.setFormatter(formatter)
         logger.handlers.clear()
         logger.addHandler(handler)
         logger.setLevel(logging.INFO)
 
+        logging.captureWarnings(True)
+        warn_logger = logging.getLogger("py.warnings")
+        warn_logger.addHandler(handler)
+        warn_logger.setLevel(logging.WARN)
+
         def solve():
             return instance.solve(params)
 
         # No time limit
         if params.time_limit == np.inf:
             return solve()
```

### Comparing `pygradflow-0.3.8/pygradflow/solver.py` & `pygradflow-0.3.9/pygradflow/solver.py`

 * *Files 8% similar despite different names*

```diff
@@ -261,33 +261,33 @@
         iterate: Iterate,
         iterations: int,
         accepted_steps: int,
         dist_factor: float,
     ) -> None:
         rho = self.rho
 
-        desc = "{:>30s}".format(SolverStatus.description(status))
+        desc = "{:>45s}".format(SolverStatus.description(status))
 
         status_desc = Format.redgreen(desc, SolverStatus.success(status), bold=True)
-        status_name = Format.bold("{:>30s}".format("Status"))
+        status_name = Format.bold("{:>20s}".format("Status"))
 
-        logger.info("%30s: %30s", status_name, status_desc)
-        logger.info("%30s: %30s", "Time", f"{total_time:.2f}s")
-        logger.info("%30s: %30d", "Iterations", iterations)
-        logger.info("%30s: %30d", "Accepted steps", accepted_steps)
-
-        logger.info("%30s: %30e", "Distance factor", dist_factor)
-
-        logger.info("%30s: %30e", "Objective", iterate.obj)
-        logger.info("%30s: %30e", "Aug Lag violation", iterate.aug_lag_violation(rho))
-        logger.info("%30s: %30e", "Aug Lag dual", iterate.aug_lag_dual())
-
-        logger.info("%30s: %30e", "Bound violation", iterate.bound_violation)
-        logger.info("%30s: %30e", "Constraint violation", iterate.cons_violation)
-        logger.info("%30s: %30e", "Dual violation", iterate.stat_res)
+        logger.info("%20s: %45s", status_name, status_desc)
+        logger.info("%20s: %45s", "Time", f"{total_time:.2f}s")
+        logger.info("%20s: %45d", "Iterations", iterations)
+        logger.info("%20s: %45d", "Accepted steps", accepted_steps)
+
+        logger.info("%20s: %45e", "Distance factor", dist_factor)
+
+        logger.info("%20s: %45e", "Objective", iterate.obj)
+        logger.info("%20s: %45e", "Aug Lag violation", iterate.aug_lag_violation(rho))
+        logger.info("%20s: %45e", "Aug Lag dual", iterate.aug_lag_dual())
+
+        logger.info("%20s: %45e", "Bound violation", iterate.bound_violation)
+        logger.info("%20s: %45e", "Constraint violation", iterate.cons_violation)
+        logger.info("%20s: %45e", "Dual violation", iterate.stat_res)
 
     def solve(
         self, x0: Optional[np.ndarray] = None, y0: Optional[np.ndarray] = None
     ) -> SolverResult:
         """
         Solves the problem starting from the given primal / dual point
 
@@ -352,16 +352,17 @@
         iteration = 0
 
         logger.info(display.header)
 
         path_dist = 0.0
         initial_iterate = iterate
         accepted_steps = 0
+        iteration = 0
 
-        for iteration in range(params.iteration_limit):
+        while True:
             if line_diff == header_interval:
                 line_diff = 0
                 logger.info(display.header)
 
             if iterate.total_res <= params.opt_tol:
                 logger.debug("Convergence achieved")
                 status = SolverStatus.Optimal
@@ -438,17 +439,22 @@
                 accepted_steps += 1
 
                 if (lamb <= params.lamb_term) and (delta <= params.opt_tol):
                     logger.debug("Convergence achieved")
                     status = SolverStatus.Optimal
                     break
 
-        else:
-            status = SolverStatus.IterationLimit
-            logger.debug("Iteration limit reached")
+            iteration += 1
+
+            if (params.iteration_limit is not None) and (
+                iteration >= params.iteration_limit
+            ):
+                status = SolverStatus.IterationLimit
+                logger.debug("Iteration limit reached")
+                break
 
         curr_time = time.time()
         total_time = curr_time - start_time
 
         direct_dist = iterate.dist(initial_iterate)
 
         assert path_dist >= direct_dist
```

### Comparing `pygradflow-0.3.8/pygradflow/step/__init__.py` & `pygradflow-0.3.9/pygradflow/step/__init__.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.3.8/pygradflow/step/asymmetric_step_solver.py` & `pygradflow-0.3.9/pygradflow/step/asymmetric_step_solver.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.3.8/pygradflow/step/cond_estimate.py` & `pygradflow-0.3.9/pygradflow/step/cond_estimate.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.3.8/pygradflow/step/extended_step_solver.py` & `pygradflow-0.3.9/pygradflow/step/extended_step_solver.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.3.8/pygradflow/step/linear_solver.py` & `pygradflow-0.3.9/pygradflow/step/linear_solver.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.3.8/pygradflow/step/scaled_step_solver.py` & `pygradflow-0.3.9/pygradflow/step/scaled_step_solver.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.3.8/pygradflow/step/standard_step_solver.py` & `pygradflow-0.3.9/pygradflow/step/standard_step_solver.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.3.8/pygradflow/step/step_control.py` & `pygradflow-0.3.9/pygradflow/step/step_control.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.3.8/pygradflow/step/step_solver.py` & `pygradflow-0.3.9/pygradflow/step/step_solver.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.3.8/pygradflow/step/symmetric_step_solver.py` & `pygradflow-0.3.9/pygradflow/step/symmetric_step_solver.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.3.8/pyproject.toml` & `pygradflow-0.3.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pygradflow"
-version = "0.3.8"
+version = "0.3.9"
 description = "PyGradFlow is a simple implementation of the sequential homotopy method to be used to solve general nonlinear programs."
 authors = ["Christoph Hansknecht <christoph.hansknecht@tu-clausthal.de>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.13"
 scipy = "^1.10.1"
```

### Comparing `pygradflow-0.3.8/PKG-INFO` & `pygradflow-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygradflow
-Version: 0.3.8
+Version: 0.3.9
 Summary: PyGradFlow is a simple implementation of the sequential homotopy method to be used to solve general nonlinear programs.
 Author: Christoph Hansknecht
 Author-email: christoph.hansknecht@tu-clausthal.de
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

