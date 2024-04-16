# Comparing `tmp/surquest_split_balancer-0.0.4.tar.gz` & `tmp/surquest_split_balancer-0.0.5.tar.gz`

## Comparing `surquest_split_balancer-0.0.4.tar` & `surquest_split_balancer-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.4/app.base.dockerfile
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.4/package.base.dockerfile
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.4/vercel.json
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.4/.github/workflows/release.yml
--rw-r--r--   0        0        0     2646 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.4/.github/workflows/test.yml
--rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.4/app/main.py
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.4/app/requirements.txt
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.4/app/schemas.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.4/surquest/utils/split_balancer/__init__.py
--rw-r--r--   0        0        0     3349 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.4/surquest/utils/split_balancer/errors.py
--rw-r--r--   0        0        0    12354 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.4/surquest/utils/split_balancer/split_balancer.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.4/test/pytest.ini
--rw-r--r--   0        0        0     7545 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.4/test/surquest/utils/split_balancer/test_split_balancer.py
--rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.4/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.4/LICENSE
--rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.4/README.md
--rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     3604 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.5/app.base.dockerfile
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.5/package.base.dockerfile
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.5/vercel.json
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.5/.github/workflows/release.yml
+-rw-r--r--   0        0        0     2587 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.5/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.5/app/main.py
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.5/app/requirements.txt
+-rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.5/app/schemas.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.5/surquest/utils/split_balancer/__init__.py
+-rw-r--r--   0        0        0     3283 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.5/surquest/utils/split_balancer/errors.py
+-rw-r--r--   0        0        0    12038 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.5/surquest/utils/split_balancer/split_balancer.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.5/test/pytest.ini
+-rw-r--r--   0        0        0     7382 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.5/test/surquest/utils/split_balancer/test_split_balancer.py
+-rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.5/LICENSE
+-rw-r--r--   0        0        0     2970 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.5/README.md
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     3604 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.5/PKG-INFO
```

### Comparing `surquest_split_balancer-0.0.4/app.base.dockerfile` & `surquest_split_balancer-0.0.5/app.base.dockerfile`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-FROM python:3.12-slim AS base
-
-# Update the base image
-# RUN apt update && apt full-upgrade -y
-
-COPY /app/requirements.txt /tmp/requirements.txt
-
-# Install python packages
-RUN pip install --no-cache-dir -r /tmp/requirements.txt
-
-# Copy local code to the container image.
-ENV DIR_PROJECT /opt/project
-ENV DIR_SRC /opt/project/src
-ENV DIR_TEST /opt/project/test
-ENV HOME $DIR_PROJECT
-RUN mkdir -p $DIR_PROJECT
-WORKDIR $DIR_PROJECT
-
-# Allow statements and log messages to immediately appear in the Cloud Run logs
-ENV ENVIRONMENT DEV
-ENV PYTHONUNBUFFERED True
-ENV PYTHONPATH="${PYTHONPATH}:${DIR_PROJECT}:${DIR_SRC}:${DIR_TEST}"
-
-CMD ["uvicorn", "app.main:app", "--host", "0.0.0.0", "--port", "8080", "--reload"]
-
-FROM base AS test
-
-COPY /test/test.requirements.txt /tmp/test.requirements.txt
-RUN pip install --no-cache-dir -r /tmp/test.requirements.txt
-ENV ENVIRONMENT TEST
-WORKDIR $DIR_TEST
-
-
-FROM base AS app
-
-COPY src $DIR_PROJECT/src
-
-CMD ["uvicorn", "app.main:app", "--host", "0.0.0.0", "--port", "8080"]
+FROM python:3.12-slim AS base
+
+# Update the base image
+# RUN apt update && apt full-upgrade -y
+
+COPY /app/requirements.txt /tmp/requirements.txt
+
+# Install python packages
+RUN pip install --no-cache-dir -r /tmp/requirements.txt
+
+# Copy local code to the container image.
+ENV DIR_PROJECT /opt/project
+ENV DIR_SRC /opt/project/src
+ENV DIR_TEST /opt/project/test
+ENV HOME $DIR_PROJECT
+RUN mkdir -p $DIR_PROJECT
+WORKDIR $DIR_PROJECT
+
+# Allow statements and log messages to immediately appear in the Cloud Run logs
+ENV ENVIRONMENT DEV
+ENV PYTHONUNBUFFERED True
+ENV PYTHONPATH="${PYTHONPATH}:${DIR_PROJECT}:${DIR_SRC}:${DIR_TEST}"
+
+CMD ["uvicorn", "app.main:app", "--host", "0.0.0.0", "--port", "8080", "--reload"]
+
+FROM base AS test
+
+COPY /test/test.requirements.txt /tmp/test.requirements.txt
+RUN pip install --no-cache-dir -r /tmp/test.requirements.txt
+ENV ENVIRONMENT TEST
+WORKDIR $DIR_TEST
+
+
+FROM base AS app
+
+COPY src $DIR_PROJECT/src
+
+CMD ["uvicorn", "app.main:app", "--host", "0.0.0.0", "--port", "8080"]
```

### Comparing `surquest_split_balancer-0.0.4/package.base.dockerfile` & `surquest_split_balancer-0.0.5/package.base.dockerfile`

 * *Files identical despite different names*

### Comparing `surquest_split_balancer-0.0.4/.github/workflows/release.yml` & `surquest_split_balancer-0.0.5/.github/workflows/release.yml`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,33 @@
-# Gitlab action triggered by new release which builds and publish new python package to PyPi
-
-name: Release
-
-on:
-  release:
-    types: [published]
-
-jobs:
-  release:
-    runs-on: ubuntu-latest
-
-    steps:
-    - uses: actions/checkout@v3
-
-    - name: Set up Python
-      uses: actions/setup-python@v4
-
-    - name: Install dependencies
-      run: |
-        python -m pip install --upgrade pip
-        pip install build
-
-    - name: Build package
-      run: python -m build
-
-    - name: Publish package
-      uses: pypa/gh-action-pypi-publish@v1.8.3
-      with:
-        user: __token__
-        password: ${{ secrets.PYPI_API_TOKEN }}
+# Gitlab action triggered by new release which builds and publish new python package to PyPi
+
+name: Release
+
+on:
+  release:
+    types: [published]
+
+jobs:
+  release:
+    runs-on: ubuntu-latest
+
+    steps:
+    - uses: actions/checkout@v4
+
+    - name: Set up Python
+      uses: actions/setup-python@v5
+      with:
+        python-version: '3.11' 
+
+    - name: Install dependencies
+      run: |
+        python3 -m pip install --upgrade pip pkginfo==1.10.0 twine==5.0.0
+        pip install build==1.2.1
+
+    - name: Build package
+      run: python3 -m build
+
+    - name: Publish package
+      uses: pypa/gh-action-pypi-publish@v1.8.14
+      with:
+        user: __token__
+        password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `surquest_split_balancer-0.0.4/app/main.py` & `surquest_split_balancer-0.0.5/app/main.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,61 +1,61 @@
-
-"""File main.py with FastAPI app"""
-import os
-from fastapi.exceptions import RequestValidationError
-from starlette.exceptions import HTTPException
-from fastapi import FastAPI, Request, Query, Body
-
-from surquest.utils.split_balancer import SplitBalancer
-# import surquest modules and objects
-from surquest.fastapi.utils.route import Route  # custom routes for documentation and FavIcon
-from surquest.fastapi.utils.GCP.tracer import Tracer
-from surquest.fastapi.utils.GCP.logging import Logger
-from surquest.fastapi.schemas.responses import Response
-from surquest.fastapi.utils.GCP.middleware import LoggingMiddleware
-from surquest.fastapi.utils.GCP.catcher import (
-    catch_validation_exceptions,
-    catch_http_exceptions,
-)
-
-from .schemas import Split
-
-PATH_PREFIX = os.getenv('PATH_PREFIX','')
-
-app = FastAPI(
-    title="Split Balancer",
-    openapi_url=F"{PATH_PREFIX}/openapi.json"
-)
-
-# add middleware
-app.add_middleware(LoggingMiddleware)
-
-# exception handlers
-app.add_exception_handler(HTTPException, catch_http_exceptions)
-app.add_exception_handler(RequestValidationError, catch_validation_exceptions)
-
-# custom routes to documentation and favicon
-app.add_api_route(path=F"{PATH_PREFIX}/", endpoint=Route.get_documentation, include_in_schema=False)
-app.add_api_route(path=PATH_PREFIX, endpoint=Route.get_favicon, include_in_schema=False)
-
-
-@app.post(F"{PATH_PREFIX}/split_balancer")
-def split(
-    split: Split = Body(...),
-):
-    """
-    Split Balancer API
-    """
-    model = SplitBalancer(
-        pool=split.pool,
-        characteristics=split.characteristics,
-        target_group_size=split.target_group_size,
-        control_group_size=split.control_group_size,
-        in_target_group=split.in_target_group,
-        in_control_group=split.in_control_group,
-    )
-
-    results = model.solve()
-
-    return Response.set(
-        data=results
+
+"""File main.py with FastAPI app"""
+import os
+from fastapi.exceptions import RequestValidationError
+from starlette.exceptions import HTTPException
+from fastapi import FastAPI, Request, Query, Body
+
+from surquest.utils.split_balancer import SplitBalancer
+# import surquest modules and objects
+from surquest.fastapi.utils.route import Route  # custom routes for documentation and FavIcon
+from surquest.fastapi.utils.GCP.tracer import Tracer
+from surquest.fastapi.utils.GCP.logging import Logger
+from surquest.fastapi.schemas.responses import Response
+from surquest.fastapi.utils.GCP.middleware import LoggingMiddleware
+from surquest.fastapi.utils.GCP.catcher import (
+    catch_validation_exceptions,
+    catch_http_exceptions,
+)
+
+from .schemas import Split
+
+PATH_PREFIX = os.getenv('PATH_PREFIX','')
+
+app = FastAPI(
+    title="Split Balancer",
+    openapi_url=F"{PATH_PREFIX}/openapi.json"
+)
+
+# add middleware
+app.add_middleware(LoggingMiddleware)
+
+# exception handlers
+app.add_exception_handler(HTTPException, catch_http_exceptions)
+app.add_exception_handler(RequestValidationError, catch_validation_exceptions)
+
+# custom routes to documentation and favicon
+app.add_api_route(path=F"{PATH_PREFIX}/", endpoint=Route.get_documentation, include_in_schema=False)
+app.add_api_route(path=PATH_PREFIX, endpoint=Route.get_favicon, include_in_schema=False)
+
+
+@app.post(F"{PATH_PREFIX}/split_balancer")
+def split(
+    split: Split = Body(...),
+):
+    """
+    Split Balancer API
+    """
+    model = SplitBalancer(
+        pool=split.pool,
+        characteristics=split.characteristics,
+        target_group_size=split.target_group_size,
+        control_group_size=split.control_group_size,
+        in_target_group=split.in_target_group,
+        in_control_group=split.in_control_group,
+    )
+
+    results = model.solve()
+
+    return Response.set(
+        data=results
     )
```

### Comparing `surquest_split_balancer-0.0.4/surquest/utils/split_balancer/errors.py` & `surquest_split_balancer-0.0.5/surquest/utils/split_balancer/errors.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,67 +1,67 @@
-class SplitBalancerError(Exception):
-    """Base class for exceptions in the SplitBalancer package."""
-
-    def __init__(self, message):
-        self.message = message
-        super().__init__(self.message)
-
-
-class InsufficientUnitsError(SplitBalancerError):
-    """Exception raised when the size of the units pool is lower than the sum of target + control group sizes."""
-
-    def __init__(self, pool_size, target_size, control_size):
-        self.pool_size = pool_size
-        self.target_size = target_size
-        self.control_size = control_size
-        message = f"Insufficient units: pool size ({self.pool_size}) is lower than the sum of target ({self.target_size}) + control ({self.control_size}) group sizes."
-        super().__init__(message)
-
-
-class OverlappingUnitsError(SplitBalancerError):
-    """Exception raised when the same units are in both the target and control groups."""
-
-    def __init__(self, overlapping_units):
-        self.overlapping_units = overlapping_units
-        if len(self.overlapping_units) == 1:
-            message = f"Overlapping unit: The following unit is in both the target and control groups: {self.overlapping_units}"
-        elif len(self.overlapping_units) > 1 and len(self.overlapping_units) < 5:
-            message = f"Overlapping units: The following units are in both the target and control groups: {self.overlapping_units}"
-        else:
-            message = f"Overlapping units: The following units are in both the target and control groups: {self.overlapping_units[0:5]} and {len(self.overlapping_units) - 5} more"
-        super().__init__(message)
-
-
-class DuplicateUnitsError(SplitBalancerError):
-    """Exception raised when the same units are in and out of the target group."""
-
-    def __init__(self, duplicate_units, group_type="target"):
-        self.duplicate_units = duplicate_units
-        self.group_type = group_type 
-
-        if len(self.duplicate_units) == 1:
-            message = f"Duplicate unit: The following unit should be in and out of the {self.group_type} group: {self.duplicate_units}"
-
-        elif len(self.duplicate_units) > 1 and len(self.duplicate_units) < 5:
-            message = f"Duplicate units: The following units should be in and out of the {self.group_type} group: {self.duplicate_units}"
-
-        else:
-            message = f"Duplicate units: The following units should be in and out of the {self.group_type} group: {self.duplicate_units[0:5]} and {len(self.duplicate_units) - 5} more"
-
-        super().__init__(message)
-
-class InvalidGroupSizeError(SplitBalancerError):
-    """Exception raised when the group size is smaller than 1 or greater than the amount of units in the pool - 1."""
-
-    def __init__(self, group_size, pool_size):
-        self.group_size = group_size
-        self.pool_size = pool_size
-        message = f"Invalid group size: Group size ({self.group_size}) is smaller than 1 or greater than the amount of units in the pool ({self.pool_size}) - 1."
-        super().__init__(message)   
-
-
-class NoOptimalSolutionError(SplitBalancerError):
-    """Exception raised when there is no optimal solution to the split balancing problem."""
-
-    def __init__(self):
-
+class SplitBalancerError(Exception):
+    """Base class for exceptions in the SplitBalancer package."""
+
+    def __init__(self, message):
+        self.message = message
+        super().__init__(self.message)
+
+
+class InsufficientUnitsError(SplitBalancerError):
+    """Exception raised when the size of the units pool is lower than the sum of target + control group sizes."""
+
+    def __init__(self, pool_size, target_size, control_size):
+        self.pool_size = pool_size
+        self.target_size = target_size
+        self.control_size = control_size
+        message = f"Insufficient units: pool size ({self.pool_size}) is lower than the sum of target ({self.target_size}) + control ({self.control_size}) group sizes."
+        super().__init__(message)
+
+
+class OverlappingUnitsError(SplitBalancerError):
+    """Exception raised when the same units are in both the target and control groups."""
+
+    def __init__(self, overlapping_units):
+        self.overlapping_units = overlapping_units
+        if len(self.overlapping_units) == 1:
+            message = f"Overlapping unit: The following unit is in both the target and control groups: {self.overlapping_units}"
+        elif len(self.overlapping_units) > 1 and len(self.overlapping_units) < 5:
+            message = f"Overlapping units: The following units are in both the target and control groups: {self.overlapping_units}"
+        else:
+            message = f"Overlapping units: The following units are in both the target and control groups: {self.overlapping_units[0:5]} and {len(self.overlapping_units) - 5} more"
+        super().__init__(message)
+
+
+class DuplicateUnitsError(SplitBalancerError):
+    """Exception raised when the same units are in and out of the target group."""
+
+    def __init__(self, duplicate_units, group_type="target"):
+        self.duplicate_units = duplicate_units
+        self.group_type = group_type 
+
+        if len(self.duplicate_units) == 1:
+            message = f"Duplicate unit: The following unit should be in and out of the {self.group_type} group: {self.duplicate_units}"
+
+        elif len(self.duplicate_units) > 1 and len(self.duplicate_units) < 5:
+            message = f"Duplicate units: The following units should be in and out of the {self.group_type} group: {self.duplicate_units}"
+
+        else:
+            message = f"Duplicate units: The following units should be in and out of the {self.group_type} group: {self.duplicate_units[0:5]} and {len(self.duplicate_units) - 5} more"
+
+        super().__init__(message)
+
+class InvalidGroupSizeError(SplitBalancerError):
+    """Exception raised when the group size is smaller than 1 or greater than the amount of units in the pool - 1."""
+
+    def __init__(self, group_size, pool_size):
+        self.group_size = group_size
+        self.pool_size = pool_size
+        message = f"Invalid group size: Group size ({self.group_size}) is smaller than 1 or greater than the amount of units in the pool ({self.pool_size}) - 1."
+        super().__init__(message)   
+
+
+class NoOptimalSolutionError(SplitBalancerError):
+    """Exception raised when there is no optimal solution to the split balancing problem."""
+
+    def __init__(self):
+
         super().__init__("No optimal solution: There is no optimal solution to the split balancing problem.")
```

### Comparing `surquest_split_balancer-0.0.4/surquest/utils/split_balancer/split_balancer.py` & `surquest_split_balancer-0.0.5/surquest/utils/split_balancer/split_balancer.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,332 +1,332 @@
-"""
-
-"""
-
-from ortools.math_opt.python import mathopt
-from ortools.math_opt.python.ipc import remote_http_solve
-from datetime import datetime, timedelta
-from surquest.utils.split_balancer.errors import *
-import numpy as np
-import logging
-
-
-class SplitBalancer:
-    """Class to balance the split of units into two groups based on their characteristics. 
-    """
-
-    def __init__(
-        self,
-        pool: list,
-        characteristics: list,
-        target_group_size: int,
-        control_group_size: int,
-        in_target_group: list | None = None,
-        in_control_group: list | None = None,
-        out_target_group: list | None = None,
-        out_control_group: list | None = None
-        # model_type: str = "CP-SAT", # "SCIP", # "GLOP", #"CP-SAT",
-        # groups: list = ["target", "control", "unassigned"]
-    ):
-        """Initializes the SplitBalancer class.
-
-        Args:
-            pool (list): A list of the pool of units.
-            characteristics (list of list): An array of the characteristics of the units.
-            target_group_size (int): The size of the target group.
-            control_group_size (int): The size of the control group.
-            in_target_group (list): A list of the units that must be in the target group.
-            in_control_group (list): A list of the units that must be in the control group.
-            out_target_group (list): A list of the units that must be out ofthe target group.
-            out_control_group (list): A list of the units that must be out the control group.
-        """
-
-        # Validate the input
-
-        # Check if the pool has enough units
-        if len(pool) < target_group_size + control_group_size:
-
-            raise InsufficientUnitsError(
-                len(pool), target_group_size, control_group_size
-            )
-
-        # Check if the same units are in both the target and control groups
-        if in_target_group is not None and in_control_group is not None:
-
-            overlapping_units = list(set(in_target_group) & set(in_control_group))
-
-            if len(overlapping_units) > 0:
-
-                raise OverlappingUnitsError(overlapping_units)
-
-        # Check if the same units are required to be in as well as out of the target
-        if out_target_group is not None and in_target_group is not None:
-
-            overlapping_units = list(set(in_target_group) & set(out_target_group))
-
-            if len(overlapping_units) > 0:
-
-                raise DuplicateUnitsError(overlapping_units, "target")
-
-        # Check if the same units are required to be in as well as out of the control
-        if out_control_group is not None and in_control_group is not None:
-
-            overlapping_units = list(set(in_control_group) & set(out_control_group))
-
-            if len(overlapping_units) > 0:
-
-                raise DuplicateUnitsError(overlapping_units, "control")
-
-        # Check if the group size is smaller than 1 or greater than the amount of units in the pool - 1
-        if target_group_size < 1 or target_group_size > len(pool) - 1:
-
-            raise InvalidGroupSizeError(target_group_size, len(pool))
-
-        if control_group_size < 1 or control_group_size > len(pool) - 1:
-
-            raise InvalidGroupSizeError(control_group_size, len(pool))
-
-        self.pool = pool
-        self.characteristics = characteristics
-        self.target_group_size = target_group_size
-        self.control_group_size = control_group_size
-        self.in_target_group = in_target_group
-        self.in_control_group = in_control_group
-        self.out_target_group = out_target_group
-        self.out_control_group = out_control_group
-
-        # Log inputs
-        logging.info(f"Pool: {self.pool}")
-        logging.info(f"Characteristics: {self.characteristics}")
-        logging.info(f"Target group size: {self.target_group_size}")
-        logging.info(f"Control group size: {self.control_group_size}")
-        logging.info(f"In target group: {self.in_target_group}")
-        logging.info(f"In control group: {self.in_control_group}")
-        logging.info(f"Out target group: {self.out_target_group}")
-        logging.info(f"Out control group: {self.out_control_group}")
-
-        self.groups = ["target", "control", "unassigned"]
-
-
-    def _get_model(self, integer_only=False):
-        """Method to create the optimization model.
-
-        Returns:
-            pywraplp.Solver: The optimization model.
-        """
-
-        pool = self.pool
-        groups = self.groups
-        target_group_size = self.target_group_size
-        control_group_size = self.control_group_size
-        in_target_group = self.in_target_group
-        in_control_group = self.in_control_group
-        out_target_group = self.out_target_group
-        out_control_group = self.out_control_group
-
-        # Create the optimization model
-        model = mathopt.Model(name="split_balancer")
-
-        # Define variables
-
-        if integer_only is True:
-            b = model.add_variable(is_integer=True, name="b")
-        else:
-            b = model.add_variable(name="b")
-
-        x = {}
-        for i in pool:
-            for j in groups:
-                x[(i, j)] = model.add_variable(lb=0, ub=1, is_integer=True, name=f"x_{i}_{j}")
-
-
-        # Define constraints
-
-        # Each unit from the pool needs to be assigned into one group
-        for i in pool:
-            model.add_linear_constraint(
-                sum(x[(i, j)] for j in groups) == 1
-            )
-
-        # Define the target group size constraint
-        model.add_linear_constraint(
-            sum(x[(i, groups[0])] for i in pool) == target_group_size
-        )
-
-        # Define the control group size constraint
-        model.add_linear_constraint(
-            sum(x[(i, groups[1])] for i in pool) == control_group_size
-        )
-
-        simple_char = self.simplify_characteristics(self.characteristics)
-        #simple_char = self.characteristics[0]
-        #print(simple_char)
-        # print(":> shape:", simple_char.shape)
-
-        if integer_only is True:
-          const = 10000
-          coef = int(target_group_size/control_group_size)*const
-
-          avg_target_char = sum(
-              x[(i, "target")]*simple_char[idx] for idx, i in enumerate(pool)
-          )*const
-
-          avg_control_char = sum(
-              x[(i, "control")]*simple_char[idx] for idx, i in enumerate(pool)
-          )*coef
-
-        else:
-        
-          avg_target_char = sum(
-              x[(i, "target")]*simple_char[idx] for idx, i in enumerate(pool)
-          )/target_group_size
-
-          avg_control_char = sum(
-              x[(i, "control")]*simple_char[idx] for idx, i in enumerate(pool)
-          )/control_group_size
-
-        # Define the distance constraint
-        model.add_linear_constraint(
-            avg_target_char - avg_control_char <= b
-        )
-
-        model.add_linear_constraint(
-            avg_control_char - avg_target_char <= b
-        )
-
-        # Define the in target group constraint
-        if self.in_target_group is not None:
-            for i in self.in_target_group:
-                model.add_linear_constraint(x[(i, self.groups[0])] == 1)
-
-        # Define the in control group constraint
-        if self.in_control_group is not None:
-            for i in self.in_control_group:
-                model.add_linear_constraint(x[(i, self.groups[1])] == 1)
-
-        # Define the out target group constraint
-        if self.out_target_group is not None:
-            for i in self.out_target_group:
-                model.add_linear_constraint(x[(i, self.groups[0])] == 0)
-
-        # Define the out control group constraint
-        if self.out_control_group is not None:
-            for i in self.out_control_group:
-                model.add_linear_constraint(x[(i, self.groups[1])] == 0)
-
-        model.minimize(b)
-
-        return model, x, b
-
-    def solve(self, integer_only=False, limit=180, remote=False, api_key=None):
-        """Method to solve the optimization model.
-
-        Args:
-            limit (int): The time limit for the optimization model. (default is 60 seconds)
-            remote (bool): Whether to solve the optimization model remotely. (default is False)
-            api_key (str): The API key for the remote solver. (default is None)
-        Returns:
-            dict: A dictionary with the units in each group.
-        """
-
-        groups = {"target": [], "control": [], "unassigned": []}
-
-        model, x, b = self._get_model(integer_only=integer_only)
-        params = mathopt.SolveParameters(time_limit=timedelta(seconds=limit))
-
-        # Solve the optimization model
-        if remote is True:
-            api_key = api_key
-            result, logs = remote_http_solve.remote_http_solve(
-                model, 
-                mathopt.SolverType.CP_SAT, 
-                api_key=api_key
-                # ToDO: add SolveParameters
-            )
-
-        else:
-            result = mathopt.solve(
-                model,
-                mathopt.SolverType.CP_SAT,
-                params=params
-            )
-
-        if result.termination.reason == mathopt.TerminationReason.OPTIMAL \
-           or result.termination.reason == mathopt.TerminationReason.FEASIBLE:
-
-            vec = {
-                "target": np.array([result.variable_values()[x[(i, self.groups[0])]] for i in self.pool]),
-                "control": np.array([result.variable_values()[x[(i, self.groups[1])]] for i in self.pool]),
-                "unassigned": np.array([result.variable_values()[x[(i, self.groups[2])]] for i in self.pool])
-            }
-
-            # Get units in target and control groups
-            for i in self.pool:
-                for j in self.groups:
-                    if result.variable_values()[x[(i, j)]] == 1:
-                        groups[j].append(i)
-
-            # Get avg characteristics for each group
-            avg = {"characteristics": [], "total": None}
-
-            n_characteristics = len(self.characteristics)
-
-            for ch in range(n_characteristics):
-
-                vec_characteristics = np.array(self.characteristics[ch])
-
-                char_avg = {
-                    "target": np.dot(vec.get("target"), vec_characteristics)
-                    / self.target_group_size,
-                    "control": np.dot(vec.get("control"), vec_characteristics)
-                    / self.control_group_size,
-                }
-
-                avg["characteristics"].append(char_avg)
-
-            # Get total avg characteristics
-            avg["total"] = {
-                "cf": result.variable_values()[b],
-                "target": np.sum(
-                    [
-                        avg["characteristics"][ch]["target"]
-                        for ch in range(n_characteristics)
-                    ]
-                ),
-                "control": np.sum(
-                    [
-                        avg["characteristics"][ch]["control"]
-                        for ch in range(n_characteristics)
-                    ]
-                ),
-            }
-
-        else:
-
-            logging.error("The problem does not have an optimal solution.")
-            raise NoOptimalSolutionError()
-
-        return {"stats": avg, "assignments": groups}
-
-    @staticmethod
-    def simplify_characteristics(characteristics, do_rescale=True, scale=1):
-        """Method to simplify the characteristics of the units.
-        to a single vector with values between 0 and 1.
-
-        Args:
-            characteristics (list of list): The characteristics of the units.
-            do_rescale (bool): Whether to rescale (integers in rage 0 and 1000) the characteristics. 
-
-        Returns:
-            list: The simplified characteristics of the units.
-        """
-
-
-        matrix = np.array(characteristics)
-        
-        # Standardize the characteristics between 0 and 1
-        std_matrix = (matrix - matrix.min()) / (matrix.max() - matrix.min())
-
-        # Calculate the mean for each characteristic (column)
-        average_unit = np.mean(std_matrix, axis=0)
-
+"""
+
+"""
+
+from ortools.math_opt.python import mathopt
+from ortools.math_opt.python.ipc import remote_http_solve
+from datetime import datetime, timedelta
+from surquest.utils.split_balancer.errors import *
+import numpy as np
+import logging
+
+
+class SplitBalancer:
+    """Class to balance the split of units into two groups based on their characteristics. 
+    """
+
+    def __init__(
+        self,
+        pool: list,
+        characteristics: list,
+        target_group_size: int,
+        control_group_size: int,
+        in_target_group: list | None = None,
+        in_control_group: list | None = None,
+        out_target_group: list | None = None,
+        out_control_group: list | None = None
+        # model_type: str = "CP-SAT", # "SCIP", # "GLOP", #"CP-SAT",
+        # groups: list = ["target", "control", "unassigned"]
+    ):
+        """Initializes the SplitBalancer class.
+
+        Args:
+            pool (list): A list of the pool of units.
+            characteristics (list of list): An array of the characteristics of the units.
+            target_group_size (int): The size of the target group.
+            control_group_size (int): The size of the control group.
+            in_target_group (list): A list of the units that must be in the target group.
+            in_control_group (list): A list of the units that must be in the control group.
+            out_target_group (list): A list of the units that must be out ofthe target group.
+            out_control_group (list): A list of the units that must be out the control group.
+        """
+
+        # Validate the input
+
+        # Check if the pool has enough units
+        if len(pool) < target_group_size + control_group_size:
+
+            raise InsufficientUnitsError(
+                len(pool), target_group_size, control_group_size
+            )
+
+        # Check if the same units are in both the target and control groups
+        if in_target_group is not None and in_control_group is not None:
+
+            overlapping_units = list(set(in_target_group) & set(in_control_group))
+
+            if len(overlapping_units) > 0:
+
+                raise OverlappingUnitsError(overlapping_units)
+
+        # Check if the same units are required to be in as well as out of the target
+        if out_target_group is not None and in_target_group is not None:
+
+            overlapping_units = list(set(in_target_group) & set(out_target_group))
+
+            if len(overlapping_units) > 0:
+
+                raise DuplicateUnitsError(overlapping_units, "target")
+
+        # Check if the same units are required to be in as well as out of the control
+        if out_control_group is not None and in_control_group is not None:
+
+            overlapping_units = list(set(in_control_group) & set(out_control_group))
+
+            if len(overlapping_units) > 0:
+
+                raise DuplicateUnitsError(overlapping_units, "control")
+
+        # Check if the group size is smaller than 1 or greater than the amount of units in the pool - 1
+        if target_group_size < 1 or target_group_size > len(pool) - 1:
+
+            raise InvalidGroupSizeError(target_group_size, len(pool))
+
+        if control_group_size < 1 or control_group_size > len(pool) - 1:
+
+            raise InvalidGroupSizeError(control_group_size, len(pool))
+
+        self.pool = pool
+        self.characteristics = characteristics
+        self.target_group_size = target_group_size
+        self.control_group_size = control_group_size
+        self.in_target_group = in_target_group
+        self.in_control_group = in_control_group
+        self.out_target_group = out_target_group
+        self.out_control_group = out_control_group
+
+        # Log inputs
+        logging.info(f"Pool: {self.pool}")
+        logging.info(f"Characteristics: {self.characteristics}")
+        logging.info(f"Target group size: {self.target_group_size}")
+        logging.info(f"Control group size: {self.control_group_size}")
+        logging.info(f"In target group: {self.in_target_group}")
+        logging.info(f"In control group: {self.in_control_group}")
+        logging.info(f"Out target group: {self.out_target_group}")
+        logging.info(f"Out control group: {self.out_control_group}")
+
+        self.groups = ["target", "control", "unassigned"]
+
+
+    def _get_model(self, integer_only=False):
+        """Method to create the optimization model.
+
+        Returns:
+            pywraplp.Solver: The optimization model.
+        """
+
+        pool = self.pool
+        groups = self.groups
+        target_group_size = self.target_group_size
+        control_group_size = self.control_group_size
+        in_target_group = self.in_target_group
+        in_control_group = self.in_control_group
+        out_target_group = self.out_target_group
+        out_control_group = self.out_control_group
+
+        # Create the optimization model
+        model = mathopt.Model(name="split_balancer")
+
+        # Define variables
+
+        if integer_only is True:
+            b = model.add_variable(is_integer=True, name="b")
+        else:
+            b = model.add_variable(name="b")
+
+        x = {}
+        for i in pool:
+            for j in groups:
+                x[(i, j)] = model.add_variable(lb=0, ub=1, is_integer=True, name=f"x_{i}_{j}")
+
+
+        # Define constraints
+
+        # Each unit from the pool needs to be assigned into one group
+        for i in pool:
+            model.add_linear_constraint(
+                sum(x[(i, j)] for j in groups) == 1
+            )
+
+        # Define the target group size constraint
+        model.add_linear_constraint(
+            sum(x[(i, groups[0])] for i in pool) == target_group_size
+        )
+
+        # Define the control group size constraint
+        model.add_linear_constraint(
+            sum(x[(i, groups[1])] for i in pool) == control_group_size
+        )
+
+        simple_char = self.simplify_characteristics(self.characteristics)
+        #simple_char = self.characteristics[0]
+        #print(simple_char)
+        # print(":> shape:", simple_char.shape)
+
+        if integer_only is True:
+          const = 10000
+          coef = int(target_group_size/control_group_size)*const
+
+          avg_target_char = sum(
+              x[(i, "target")]*simple_char[idx] for idx, i in enumerate(pool)
+          )*const
+
+          avg_control_char = sum(
+              x[(i, "control")]*simple_char[idx] for idx, i in enumerate(pool)
+          )*coef
+
+        else:
+        
+          avg_target_char = sum(
+              x[(i, "target")]*simple_char[idx] for idx, i in enumerate(pool)
+          )/target_group_size
+
+          avg_control_char = sum(
+              x[(i, "control")]*simple_char[idx] for idx, i in enumerate(pool)
+          )/control_group_size
+
+        # Define the distance constraint
+        model.add_linear_constraint(
+            avg_target_char - avg_control_char <= b
+        )
+
+        model.add_linear_constraint(
+            avg_control_char - avg_target_char <= b
+        )
+
+        # Define the in target group constraint
+        if self.in_target_group is not None:
+            for i in self.in_target_group:
+                model.add_linear_constraint(x[(i, self.groups[0])] == 1)
+
+        # Define the in control group constraint
+        if self.in_control_group is not None:
+            for i in self.in_control_group:
+                model.add_linear_constraint(x[(i, self.groups[1])] == 1)
+
+        # Define the out target group constraint
+        if self.out_target_group is not None:
+            for i in self.out_target_group:
+                model.add_linear_constraint(x[(i, self.groups[0])] == 0)
+
+        # Define the out control group constraint
+        if self.out_control_group is not None:
+            for i in self.out_control_group:
+                model.add_linear_constraint(x[(i, self.groups[1])] == 0)
+
+        model.minimize(b)
+
+        return model, x, b
+
+    def solve(self, integer_only=False, limit=180, remote=False, api_key=None):
+        """Method to solve the optimization model.
+
+        Args:
+            limit (int): The time limit for the optimization model. (default is 60 seconds)
+            remote (bool): Whether to solve the optimization model remotely. (default is False)
+            api_key (str): The API key for the remote solver. (default is None)
+        Returns:
+            dict: A dictionary with the units in each group.
+        """
+
+        groups = {"target": [], "control": [], "unassigned": []}
+
+        model, x, b = self._get_model(integer_only=integer_only)
+        params = mathopt.SolveParameters(time_limit=timedelta(seconds=limit))
+
+        # Solve the optimization model
+        if remote is True:
+            api_key = api_key
+            result, logs = remote_http_solve.remote_http_solve(
+                model, 
+                mathopt.SolverType.CP_SAT, 
+                api_key=api_key
+                # ToDO: add SolveParameters
+            )
+
+        else:
+            result = mathopt.solve(
+                model,
+                mathopt.SolverType.CP_SAT,
+                params=params
+            )
+
+        if result.termination.reason == mathopt.TerminationReason.OPTIMAL \
+           or result.termination.reason == mathopt.TerminationReason.FEASIBLE:
+
+            vec = {
+                "target": np.array([result.variable_values()[x[(i, self.groups[0])]] for i in self.pool]),
+                "control": np.array([result.variable_values()[x[(i, self.groups[1])]] for i in self.pool]),
+                "unassigned": np.array([result.variable_values()[x[(i, self.groups[2])]] for i in self.pool])
+            }
+
+            # Get units in target and control groups
+            for i in self.pool:
+                for j in self.groups:
+                    if result.variable_values()[x[(i, j)]] == 1:
+                        groups[j].append(i)
+
+            # Get avg characteristics for each group
+            avg = {"characteristics": [], "total": None}
+
+            n_characteristics = len(self.characteristics)
+
+            for ch in range(n_characteristics):
+
+                vec_characteristics = np.array(self.characteristics[ch])
+
+                char_avg = {
+                    "target": np.dot(vec.get("target"), vec_characteristics)
+                    / self.target_group_size,
+                    "control": np.dot(vec.get("control"), vec_characteristics)
+                    / self.control_group_size,
+                }
+
+                avg["characteristics"].append(char_avg)
+
+            # Get total avg characteristics
+            avg["total"] = {
+                "objectiveFunction": result.variable_values()[b],
+                "target": np.sum(
+                    [
+                        avg["characteristics"][ch]["target"]
+                        for ch in range(n_characteristics)
+                    ]
+                ),
+                "control": np.sum(
+                    [
+                        avg["characteristics"][ch]["control"]
+                        for ch in range(n_characteristics)
+                    ]
+                ),
+            }
+
+        else:
+
+            logging.error("The problem does not have an optimal solution.")
+            raise NoOptimalSolutionError()
+
+        return {"stats": avg, "assignments": groups}
+
+    @staticmethod
+    def simplify_characteristics(characteristics, do_rescale=True, scale=1):
+        """Method to simplify the characteristics of the units.
+        to a single vector with values between 0 and 1.
+
+        Args:
+            characteristics (list of list): The characteristics of the units.
+            do_rescale (bool): Whether to rescale (integers in rage 0 and 1000) the characteristics. 
+
+        Returns:
+            list: The simplified characteristics of the units.
+        """
+
+
+        matrix = np.array(characteristics)
+        
+        # Standardize the characteristics between 0 and 1
+        std_matrix = (matrix - matrix.min()) / (matrix.max() - matrix.min())
+
+        # Calculate the mean for each characteristic (column)
+        average_unit = np.mean(std_matrix, axis=0)
+
         return average_unit
```

### Comparing `surquest_split_balancer-0.0.4/test/surquest/utils/split_balancer/test_split_balancer.py` & `surquest_split_balancer-0.0.5/test/surquest/utils/split_balancer/test_split_balancer.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,157 +1,157 @@
-import pytest
-import random
-import time
-from surquest.utils.split_balancer import SplitBalancer
-from surquest.utils.split_balancer.errors import *
-
-
-target_group_size = 5
-control_group_size = 3
-in_target_group = [1, 2, 3]
-in_control_group = [10]
-out_target_group = [9, 10]
-out_control_group = [4, 5]
-pool = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
-characteristics = {
-    1: [
-        [4, 5, 6, 4, 6, 9, 1, 4, 6, 5]
-    ],
-    2: [
-        [4, 5, 6, 4, 6, 9, 1, 4, 6, 5],
-        [2, 3, 4, 2, 4, 7, 1, 2, 4, 3]
-    ]
-}
-
-big_N = 1000
-big_pool = range(big_N)
-characteristics["big"] = [
-    [random.randrange(1, 100) for _ in range(big_N)],
-    [random.randrange(1, 100) for _ in range(big_N)],
-    [random.randrange(1, 100) for _ in range(big_N)]
-]
-big_target_group_size = int(0.8*big_N)
-big_control_group_size = int(0.1*big_N)
-
-class TestSplitBalancer:
-
-
-    @pytest.mark.parametrize(
-        "target_group_size, control_group_size, in_target_group, in_control_group, out_target_group, out_control_group, pool, characteristics, expected",
-        [
-            (8, control_group_size, in_target_group, in_control_group, out_target_group, out_control_group, pool, characteristics.get(1), InsufficientUnitsError),
-            (0, control_group_size, in_target_group, in_control_group, out_target_group, out_control_group, pool, characteristics.get(1), InvalidGroupSizeError),
-            (target_group_size, 0, in_target_group, in_control_group, out_target_group, out_control_group, pool, characteristics.get(1), InvalidGroupSizeError),
-            (target_group_size, control_group_size, [1], [1], out_target_group, out_control_group, pool, characteristics.get(1), OverlappingUnitsError),
-            (target_group_size, control_group_size, [1,2,3,4], [1,2,3,4], out_target_group, out_control_group, pool, characteristics.get(1), OverlappingUnitsError),
-            (target_group_size, control_group_size, [1,2,3,4,5,6], [1,2,3,4,5,6], out_target_group, out_control_group, pool, characteristics.get(1), OverlappingUnitsError),
-            (target_group_size, control_group_size, [1], in_control_group, [1], out_control_group, pool, characteristics.get(1), DuplicateUnitsError),
-            (target_group_size, control_group_size, [1,2,3,4], in_control_group, [1,2,3,4], out_control_group, pool, characteristics.get(1), DuplicateUnitsError),
-            (target_group_size, control_group_size, [1,2,3,4,5,6], in_control_group, [1,2,3,4,5,6], out_control_group, pool, characteristics.get(1), DuplicateUnitsError),
-            (target_group_size, control_group_size, in_target_group, in_control_group, out_target_group, in_control_group, pool, characteristics.get(1), DuplicateUnitsError),
-            (8, 2, in_target_group, [7, 8, 9, 10], out_target_group, out_control_group, pool, characteristics.get(1), NoOptimalSolutionError),
-        ],
-    )
-    def test_failure(self, target_group_size, control_group_size, in_target_group, in_control_group, out_target_group, out_control_group, pool, characteristics, expected):
-
-        try:
-            split_balancer = SplitBalancer(
-                pool=pool,
-                characteristics=characteristics,
-                target_group_size=target_group_size,
-                control_group_size=control_group_size,
-                in_target_group=in_target_group,
-                in_control_group=in_control_group,
-                out_target_group=out_target_group,
-                out_control_group=out_control_group
-            )
-        except Exception as e:
-            assert isinstance(e, expected), f"Expected {expected}, but got {type(e)}"
-
-    @pytest.mark.parametrize(
-        "target_group_size, control_group_size, in_target_group, in_control_group, out_target_group, out_control_group, pool, characteristics, expected",
-        [
-            (target_group_size, control_group_size, in_target_group, in_control_group, out_target_group, out_control_group, pool, characteristics.get(1), dict),
-            (target_group_size, control_group_size, in_target_group, in_control_group, out_target_group, out_control_group, pool, characteristics.get(2), dict),
-            (target_group_size, control_group_size, in_target_group, [7, 8, 9, 10], out_target_group, out_control_group, pool, characteristics.get(1), type(None)),
-        ],
-    )
-    def test_success(self, target_group_size, control_group_size, in_target_group, in_control_group, out_target_group, out_control_group, pool, characteristics, expected):
-        
-        split_balancer = SplitBalancer(
-            pool=pool,
-            characteristics=characteristics,
-            target_group_size=target_group_size,
-            control_group_size=control_group_size,
-            in_target_group=in_target_group,
-            in_control_group=in_control_group,
-            out_target_group=out_target_group,
-            out_control_group=out_control_group
-        )
-
-        results = None
-
-        try:
-            results = split_balancer.solve()
-        except NoOptimalSolutionError as e:
-            pass
-
-        assert isinstance(results, expected)
-
-        if expected is dict:
-
-            groups = results.get("assignments")
-
-            # Check if the groups are of the correct size
-            assert target_group_size == len(groups["target"])
-            assert control_group_size == len(groups["control"])
-
-            # Check if the units are in the correct groups
-            for unit in in_target_group:
-                assert unit in groups["target"], f"Unit {unit} is not in the target group: {groups['target']}"
-
-            for unit in in_control_group:
-                assert unit in groups["control"], f"Unit {unit} is not in the control group: {groups['control']}"
-
-            for unit in out_target_group:
-                assert unit not in groups["target"], f"Unit {unit} is in the target group: {groups['target']}"
-
-            for unit in out_control_group:
-                assert unit not in groups["control"], f"Unit {unit} is in the control group: {groups['control']}"
-
-    def test_benchmark(self):
-
-        for i in [10, 100]: # 500, 1000, 1500, 2500, 5000
-            for j in [1, 2, 5, 10, 100]: # [1, 5, 10, 50]:
-
-                n = i
-                pool = range(n)
-                characteristics = []
-                for x in range(j):
-                    characteristics.append(
-                        [random.randrange(0, 100) for _ in range(n)]
-                        )
-                        
-                target_group_size = int(0.6*n)
-                control_group_size = int(0.2*n)
-                in_target_group = None
-                in_control_group = None
-                out_target_group = None
-                out_control_group = None
-
-                split_balancer = SplitBalancer(
-                    pool=pool,
-                    characteristics=characteristics,
-                    target_group_size=target_group_size,
-                    control_group_size=control_group_size,
-                    in_target_group=in_target_group,
-                    in_control_group=in_control_group,
-                    out_target_group=out_target_group,
-                    out_control_group=out_control_group
-                )
-
-                start = time.time()
-                out = split_balancer.solve()
-                end = time.time()
-
-                print(f":> {i} - {j} - time {end-start}")
+import pytest
+import random
+import time
+from surquest.utils.split_balancer import SplitBalancer
+from surquest.utils.split_balancer.errors import *
+
+
+target_group_size = 5
+control_group_size = 3
+in_target_group = [1, 2, 3]
+in_control_group = [10]
+out_target_group = [9, 10]
+out_control_group = [4, 5]
+pool = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
+characteristics = {
+    1: [
+        [4, 5, 6, 4, 6, 9, 1, 4, 6, 5]
+    ],
+    2: [
+        [4, 5, 6, 4, 6, 9, 1, 4, 6, 5],
+        [2, 3, 4, 2, 4, 7, 1, 2, 4, 3]
+    ]
+}
+
+big_N = 1000
+big_pool = range(big_N)
+characteristics["big"] = [
+    [random.randrange(1, 100) for _ in range(big_N)],
+    [random.randrange(1, 100) for _ in range(big_N)],
+    [random.randrange(1, 100) for _ in range(big_N)]
+]
+big_target_group_size = int(0.8*big_N)
+big_control_group_size = int(0.1*big_N)
+
+class TestSplitBalancer:
+
+
+    @pytest.mark.parametrize(
+        "target_group_size, control_group_size, in_target_group, in_control_group, out_target_group, out_control_group, pool, characteristics, expected",
+        [
+            (8, control_group_size, in_target_group, in_control_group, out_target_group, out_control_group, pool, characteristics.get(1), InsufficientUnitsError),
+            (0, control_group_size, in_target_group, in_control_group, out_target_group, out_control_group, pool, characteristics.get(1), InvalidGroupSizeError),
+            (target_group_size, 0, in_target_group, in_control_group, out_target_group, out_control_group, pool, characteristics.get(1), InvalidGroupSizeError),
+            (target_group_size, control_group_size, [1], [1], out_target_group, out_control_group, pool, characteristics.get(1), OverlappingUnitsError),
+            (target_group_size, control_group_size, [1,2,3,4], [1,2,3,4], out_target_group, out_control_group, pool, characteristics.get(1), OverlappingUnitsError),
+            (target_group_size, control_group_size, [1,2,3,4,5,6], [1,2,3,4,5,6], out_target_group, out_control_group, pool, characteristics.get(1), OverlappingUnitsError),
+            (target_group_size, control_group_size, [1], in_control_group, [1], out_control_group, pool, characteristics.get(1), DuplicateUnitsError),
+            (target_group_size, control_group_size, [1,2,3,4], in_control_group, [1,2,3,4], out_control_group, pool, characteristics.get(1), DuplicateUnitsError),
+            (target_group_size, control_group_size, [1,2,3,4,5,6], in_control_group, [1,2,3,4,5,6], out_control_group, pool, characteristics.get(1), DuplicateUnitsError),
+            (target_group_size, control_group_size, in_target_group, in_control_group, out_target_group, in_control_group, pool, characteristics.get(1), DuplicateUnitsError),
+            (8, 2, in_target_group, [7, 8, 9, 10], out_target_group, out_control_group, pool, characteristics.get(1), NoOptimalSolutionError),
+        ],
+    )
+    def test_failure(self, target_group_size, control_group_size, in_target_group, in_control_group, out_target_group, out_control_group, pool, characteristics, expected):
+
+        try:
+            split_balancer = SplitBalancer(
+                pool=pool,
+                characteristics=characteristics,
+                target_group_size=target_group_size,
+                control_group_size=control_group_size,
+                in_target_group=in_target_group,
+                in_control_group=in_control_group,
+                out_target_group=out_target_group,
+                out_control_group=out_control_group
+            )
+        except Exception as e:
+            assert isinstance(e, expected), f"Expected {expected}, but got {type(e)}"
+
+    @pytest.mark.parametrize(
+        "target_group_size, control_group_size, in_target_group, in_control_group, out_target_group, out_control_group, pool, characteristics, expected",
+        [
+            (target_group_size, control_group_size, in_target_group, in_control_group, out_target_group, out_control_group, pool, characteristics.get(1), dict),
+            (target_group_size, control_group_size, in_target_group, in_control_group, out_target_group, out_control_group, pool, characteristics.get(2), dict),
+            (target_group_size, control_group_size, in_target_group, [7, 8, 9, 10], out_target_group, out_control_group, pool, characteristics.get(1), type(None)),
+        ],
+    )
+    def test_success(self, target_group_size, control_group_size, in_target_group, in_control_group, out_target_group, out_control_group, pool, characteristics, expected):
+        
+        split_balancer = SplitBalancer(
+            pool=pool,
+            characteristics=characteristics,
+            target_group_size=target_group_size,
+            control_group_size=control_group_size,
+            in_target_group=in_target_group,
+            in_control_group=in_control_group,
+            out_target_group=out_target_group,
+            out_control_group=out_control_group
+        )
+
+        results = None
+
+        try:
+            results = split_balancer.solve()
+        except NoOptimalSolutionError as e:
+            pass
+
+        assert isinstance(results, expected)
+
+        if expected is dict:
+
+            groups = results.get("assignments")
+
+            # Check if the groups are of the correct size
+            assert target_group_size == len(groups["target"])
+            assert control_group_size == len(groups["control"])
+
+            # Check if the units are in the correct groups
+            for unit in in_target_group:
+                assert unit in groups["target"], f"Unit {unit} is not in the target group: {groups['target']}"
+
+            for unit in in_control_group:
+                assert unit in groups["control"], f"Unit {unit} is not in the control group: {groups['control']}"
+
+            for unit in out_target_group:
+                assert unit not in groups["target"], f"Unit {unit} is in the target group: {groups['target']}"
+
+            for unit in out_control_group:
+                assert unit not in groups["control"], f"Unit {unit} is in the control group: {groups['control']}"
+
+    def test_benchmark(self):
+
+        for i in [10, 100]: # 500, 1000, 1500, 2500, 5000
+            for j in [1, 2, 5]: # [1, 5, 10, 50]:
+
+                n = i
+                pool = range(n)
+                characteristics = []
+                for x in range(j):
+                    characteristics.append(
+                        [random.randrange(0, 10000) for _ in range(n)]
+                        )
+                        
+                target_group_size = int(0.6*n)
+                control_group_size = int(0.2*n)
+                in_target_group = None
+                in_control_group = None
+                out_target_group = None
+                out_control_group = None
+
+                split_balancer = SplitBalancer(
+                    pool=pool,
+                    characteristics=characteristics,
+                    target_group_size=target_group_size,
+                    control_group_size=control_group_size,
+                    in_target_group=in_target_group,
+                    in_control_group=in_control_group,
+                    out_target_group=out_target_group,
+                    out_control_group=out_control_group
+                )
+
+                start = time.time()
+                out = split_balancer.solve()
+                end = time.time()
+
+                print(f":> {i} - {j} - time {end-start}")
                 print("-"*150)
```

### Comparing `surquest_split_balancer-0.0.4/.gitignore` & `surquest_split_balancer-0.0.5/.gitignore`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,161 +1,161 @@
-# Byte-compiled / optimized / DLL files
-__pycache__/
-*.py[cod]
-*$py.class
-
-# C extensions
-*.so
-
-# Distribution / packaging
-.Python
-build/
-develop-eggs/
-dist/
-downloads/
-eggs/
-.eggs/
-lib/
-lib64/
-parts/
-sdist/
-var/
-wheels/
-share/python-wheels/
-*.egg-info/
-.installed.cfg
-*.egg
-MANIFEST
-
-# PyInstaller
-#  Usually these files are written by a python script from a template
-#  before PyInstaller builds the exe, so as to inject date/other infos into it.
-*.manifest
-*.spec
-
-# Installer logs
-pip-log.txt
-pip-delete-this-directory.txt
-
-# Unit test / coverage reports
-htmlcov/
-.tox/
-.nox/
-.coverage
-.coverage.*
-.cache
-nosetests.xml
-coverage.xml
-*.cover
-*.py,cover
-.hypothesis/
-.pytest_cache/
-cover/
-report.xml
-
-# Translations
-*.mo
-*.pot
-
-# Django stuff:
-*.log
-local_settings.py
-db.sqlite3
-db.sqlite3-journal
-
-# Flask stuff:
-instance/
-.webassets-cache
-
-# Scrapy stuff:
-.scrapy
-
-# Sphinx documentation
-docs/_build/
-
-# PyBuilder
-.pybuilder/
-target/
-
-# Jupyter Notebook
-.ipynb_checkpoints
-
-# IPython
-profile_default/
-ipython_config.py
-
-# pyenv
-#   For a library or package, you might want to ignore these files since the code is
-#   intended to run in multiple environments; otherwise, check them in:
-# .python-version
-
-# pipenv
-#   According to pypa/pipenv#598, it is recommended to include Pipfile.lock in version control.
-#   However, in case of collaboration, if having platform-specific dependencies or dependencies
-#   having no cross-platform support, pipenv may install dependencies that don't work, or not
-#   install all needed dependencies.
-#Pipfile.lock
-
-# poetry
-#   Similar to Pipfile.lock, it is generally recommended to include poetry.lock in version control.
-#   This is especially recommended for binary packages to ensure reproducibility, and is more
-#   commonly ignored for libraries.
-#   https://python-poetry.org/docs/basic-usage/#commit-your-poetrylock-file-to-version-control
-#poetry.lock
-
-# pdm
-#   Similar to Pipfile.lock, it is generally recommended to include pdm.lock in version control.
-#pdm.lock
-#   pdm stores project-wide configurations in .pdm.toml, but it is recommended to not include it
-#   in version control.
-#   https://pdm.fming.dev/#use-with-ide
-.pdm.toml
-
-# PEP 582; used by e.g. github.com/David-OConnor/pyflow and github.com/pdm-project/pdm
-__pypackages__/
-
-# Celery stuff
-celerybeat-schedule
-celerybeat.pid
-
-# SageMath parsed files
-*.sage.py
-
-# Environments
-.env
-.venv
-env/
-venv/
-ENV/
-env.bak/
-venv.bak/
-
-# Spyder project settings
-.spyderproject
-.spyproject
-
-# Rope project settings
-.ropeproject
-
-# mkdocs documentation
-/site
-
-# mypy
-.mypy_cache/
-.dmypy.json
-dmypy.json
-
-# Pyre type checker
-.pyre/
-
-# pytype static type analyzer
-.pytype/
-
-# Cython debug symbols
-cython_debug/
-
-# PyCharm
-#  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
-#  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
-#  and can be added to the global gitignore or merged into this file.  For a more nuclear
-#  option (not recommended) you can uncomment the following to ignore the entire idea folder.
-#.idea/
+# Byte-compiled / optimized / DLL files
+__pycache__/
+*.py[cod]
+*$py.class
+
+# C extensions
+*.so
+
+# Distribution / packaging
+.Python
+build/
+develop-eggs/
+dist/
+downloads/
+eggs/
+.eggs/
+lib/
+lib64/
+parts/
+sdist/
+var/
+wheels/
+share/python-wheels/
+*.egg-info/
+.installed.cfg
+*.egg
+MANIFEST
+
+# PyInstaller
+#  Usually these files are written by a python script from a template
+#  before PyInstaller builds the exe, so as to inject date/other infos into it.
+*.manifest
+*.spec
+
+# Installer logs
+pip-log.txt
+pip-delete-this-directory.txt
+
+# Unit test / coverage reports
+htmlcov/
+.tox/
+.nox/
+.coverage
+.coverage.*
+.cache
+nosetests.xml
+coverage.xml
+*.cover
+*.py,cover
+.hypothesis/
+.pytest_cache/
+cover/
+report.xml
+
+# Translations
+*.mo
+*.pot
+
+# Django stuff:
+*.log
+local_settings.py
+db.sqlite3
+db.sqlite3-journal
+
+# Flask stuff:
+instance/
+.webassets-cache
+
+# Scrapy stuff:
+.scrapy
+
+# Sphinx documentation
+docs/_build/
+
+# PyBuilder
+.pybuilder/
+target/
+
+# Jupyter Notebook
+.ipynb_checkpoints
+
+# IPython
+profile_default/
+ipython_config.py
+
+# pyenv
+#   For a library or package, you might want to ignore these files since the code is
+#   intended to run in multiple environments; otherwise, check them in:
+# .python-version
+
+# pipenv
+#   According to pypa/pipenv#598, it is recommended to include Pipfile.lock in version control.
+#   However, in case of collaboration, if having platform-specific dependencies or dependencies
+#   having no cross-platform support, pipenv may install dependencies that don't work, or not
+#   install all needed dependencies.
+#Pipfile.lock
+
+# poetry
+#   Similar to Pipfile.lock, it is generally recommended to include poetry.lock in version control.
+#   This is especially recommended for binary packages to ensure reproducibility, and is more
+#   commonly ignored for libraries.
+#   https://python-poetry.org/docs/basic-usage/#commit-your-poetrylock-file-to-version-control
+#poetry.lock
+
+# pdm
+#   Similar to Pipfile.lock, it is generally recommended to include pdm.lock in version control.
+#pdm.lock
+#   pdm stores project-wide configurations in .pdm.toml, but it is recommended to not include it
+#   in version control.
+#   https://pdm.fming.dev/#use-with-ide
+.pdm.toml
+
+# PEP 582; used by e.g. github.com/David-OConnor/pyflow and github.com/pdm-project/pdm
+__pypackages__/
+
+# Celery stuff
+celerybeat-schedule
+celerybeat.pid
+
+# SageMath parsed files
+*.sage.py
+
+# Environments
+.env
+.venv
+env/
+venv/
+ENV/
+env.bak/
+venv.bak/
+
+# Spyder project settings
+.spyderproject
+.spyproject
+
+# Rope project settings
+.ropeproject
+
+# mkdocs documentation
+/site
+
+# mypy
+.mypy_cache/
+.dmypy.json
+dmypy.json
+
+# Pyre type checker
+.pyre/
+
+# pytype static type analyzer
+.pytype/
+
+# Cython debug symbols
+cython_debug/
+
+# PyCharm
+#  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
+#  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
+#  and can be added to the global gitignore or merged into this file.  For a more nuclear
+#  option (not recommended) you can uncomment the following to ignore the entire idea folder.
+#.idea/
```

### Comparing `surquest_split_balancer-0.0.4/LICENSE` & `surquest_split_balancer-0.0.5/LICENSE`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2024 surquest
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2024 surquest
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `surquest_split_balancer-0.0.4/README.md` & `surquest_split_balancer-0.0.5/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,89 +1,89 @@
-![GitHub](https://img.shields.io/github/license/surquest/python-split-balancer?style=flat-square)
-![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/surquest/python-split-balancer/test.yml?branch=main&style=flat-square)
-![Coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/surquest/6e25c317000917840152a5e702e71963/raw/python-split-balancer.json&style=flat-square)
-![PyPI - Downloads](https://img.shields.io/pypi/dm/surquest-GCP-secret-assessor?style=flat-square)
-
-# Introduction
-
-This project provides a Python package and REST API applications for dividing a set of units into two most comparable groups based on their characteristics.
-
-## Problem Statement
-
-Balancing Numeric Characteristics Across Two Groups
-
-### Input:
-
-* A set of units, where each unit possesses one or more numeric characteristics.
-* Desired size for each of the two groups.
-* (Optional) Pre-assignment constraints:
-    
-   - Specify units that must belong to a particular group (Group A or Group B).
-   - Specify units that cannot belong to a particular group (Group A or Group B).
-
-### Objective:
-
-Partition the units into two groups (Group A and Group B) of the specified size, ensuring maximum similarity between the groups. Similarity is measured by minimizing the sum of absolute differences in mean values for each characteristic across the two groups.
-
-### Constraints:
-
-* Each unit is assigned to either Group A, Group B, or remains unassigned.
-* The final size of Group A and Group B must match the specified desired size.
-
-### Output:
-
-* A list of units assigned to Group A and Group B.
-* The mean values for each characteristic in Group A and Group B.
-* The sum of absolute differences in mean values for each characteristic across the two groups.
-
-
-# Local development
-
-You are more than welcome to contribute to this project. To make your start easier we have prepared a docker image with all the necessary tools to run it as interpreter for Pycharm or to run tests.
-
-
-## Build docker image
-```
-docker build `
-     --tag surquest/surquest/split-balancer:latest `
-     --file package.base.dockerfile `
-     --target test .
-```
-
-
-## Run docker container
-```
-docker run --rm -it `
- -v "${pwd}:/opt/project" `
- -w "/opt/project/test" `
- surquest/surquest/split-balancer:latest pytest
-```
-
-
-# REST API Quick Start
-
-```powershell
-
-# Build the docker image
-
-docker build `
-     --no-cache `
-     --tag surquest/app-split-balancer:latest `
-     --file app.base.dockerfile `
-     --target base .
-
-docker build `
-     --no-cache `
-     --tag python/instore/pmp-integration-proxy `
-     --file app.base.dockerfile `
-     --target app .
-
-# Run the docker container
-docker run --rm -it `
-    --name pmp-integration-proxy `
-    -v "$(pwd):/opt/project" `
-    -p 1010:8080 surquest/app-split-balancer:latest
-
-docker run --rm -it `
-    --name pmp-integration-proxy `
-    -p 1010:8080 python/instore/pmp-integration-proxy
+![GitHub](https://img.shields.io/github/license/surquest/python-split-balancer?style=flat-square)
+![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/surquest/python-split-balancer/test.yml?branch=main&style=flat-square)
+![Coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/surquest/373e1859cb547514516a8f22cd8f18a7/raw/python-split-balancer.json&style=flat-square)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/surquest-GCP-secret-assessor?style=flat-square)
+
+# Introduction
+
+This project provides a Python package and REST API applications for dividing a set of units into two most comparable groups based on their characteristics.
+
+## Problem Statement
+
+Balancing Numeric Characteristics Across Two Groups
+
+### Input:
+
+* A set of units, where each unit possesses one or more numeric characteristics.
+* Desired size for each of the two groups.
+* (Optional) Pre-assignment constraints:
+    
+   - Specify units that must belong to a particular group (Group A or Group B).
+   - Specify units that cannot belong to a particular group (Group A or Group B).
+
+### Objective:
+
+Partition the units into two groups (Group A and Group B) of the specified size, ensuring maximum similarity between the groups. Similarity is measured by minimizing the sum of absolute differences in mean values for each characteristic across the two groups.
+
+### Constraints:
+
+* Each unit is assigned to either Group A, Group B, or remains unassigned.
+* The final size of Group A and Group B must match the specified desired size.
+
+### Output:
+
+* A list of units assigned to Group A and Group B.
+* The mean values for each characteristic in Group A and Group B.
+* The sum of absolute differences in mean values for each characteristic across the two groups.
+
+
+# Local development
+
+You are more than welcome to contribute to this project. To make your start easier we have prepared a docker image with all the necessary tools to run it as interpreter for Pycharm or to run tests.
+
+
+## Build docker image
+```
+docker build `
+     --tag surquest/surquest/split-balancer:latest `
+     --file package.base.dockerfile `
+     --target test .
+```
+
+
+## Run docker container
+```
+docker run --rm -it `
+ -v "${pwd}:/opt/project" `
+ -w "/opt/project/test" `
+ surquest/surquest/split-balancer:latest pytest
+```
+
+
+# REST API Quick Start
+
+```powershell
+
+# Build the docker image
+
+docker build `
+     --no-cache `
+     --tag surquest/app-split-balancer:latest `
+     --file app.base.dockerfile `
+     --target base .
+
+docker build `
+     --no-cache `
+     --tag python/instore/pmp-integration-proxy `
+     --file app.base.dockerfile `
+     --target app .
+
+# Run the docker container
+docker run --rm -it `
+    --name pmp-integration-proxy `
+    -v "$(pwd):/opt/project" `
+    -p 1010:8080 surquest/app-split-balancer:latest
+
+docker run --rm -it `
+    --name pmp-integration-proxy `
+    -p 1010:8080 python/instore/pmp-integration-proxy
 ```
```

### Comparing `surquest_split_balancer-0.0.4/pyproject.toml` & `surquest_split_balancer-0.0.5/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-[build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
-
-[project]
-name = "surquest-split-balancer"
-version = "0.0.4"
-description = "A Python package for dividing a set of units into two most comparable groups based on their characteristics."
-authors = [
-    {name= "Michal Švarc", email= "michal.svarc@surquest.com"}
-]
-readme = "README.md"
-dependencies = [
-    "ortools >= 9.9.3963",
-    "requests"
-]
-
-[project.optional-dependencies]
-test = [
-    "pytest>=8.1.1",
-    "pytest-cov>=5.0.0"
-]
-
-
-[project.urls]
-"Homepage" = "https://github.com/surquest/python-split-balancer"
-"Bug Tracker" = "https://github.com/surquest/python-split-balancer/issues"
-
-
-[tool.hatch.build.targets.wheel]
-packages = ["surquest"]
-
-[tool.hatch.build.targets.sdist.sources]
-"src" = ""
+[build-system]
+requires = ["hatchling"]
+build-backend = "hatchling.build"
+
+[project]
+name = "surquest-split-balancer"
+version = "0.0.5"
+description = "A Python package for dividing a set of units into two most comparable groups based on their characteristics."
+authors = [
+    {name= "Michal Švarc", email= "michal.svarc@surquest.com"}
+]
+readme = "README.md"
+dependencies = [
+    "ortools >= 9.9.3963",
+    "requests"
+]
+
+[project.optional-dependencies]
+test = [
+    "pytest>=8.1.1",
+    "pytest-cov>=5.0.0"
+]
+
+
+[project.urls]
+"Homepage" = "https://github.com/surquest/python-split-balancer"
+"Bug Tracker" = "https://github.com/surquest/python-split-balancer/issues"
+
+
+[tool.hatch.build.targets.wheel]
+packages = ["surquest"]
+
+[tool.hatch.build.targets.sdist.sources]
+"src" = ""
```

### Comparing `surquest_split_balancer-0.0.4/PKG-INFO` & `surquest_split_balancer-0.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.3
 Name: surquest-split-balancer
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Python package for dividing a set of units into two most comparable groups based on their characteristics.
 Project-URL: Homepage, https://github.com/surquest/python-split-balancer
 Project-URL: Bug Tracker, https://github.com/surquest/python-split-balancer/issues
 Author-email: Michal Švarc <michal.svarc@surquest.com>
 License-File: LICENSE
 Requires-Dist: ortools>=9.9.3963
 Requires-Dist: requests
 Provides-Extra: test
 Requires-Dist: pytest-cov>=5.0.0; extra == 'test'
 Requires-Dist: pytest>=8.1.1; extra == 'test'
 Description-Content-Type: text/markdown
 
 ![GitHub](https://img.shields.io/github/license/surquest/python-split-balancer?style=flat-square)
 ![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/surquest/python-split-balancer/test.yml?branch=main&style=flat-square)
-![Coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/surquest/6e25c317000917840152a5e702e71963/raw/python-split-balancer.json&style=flat-square)
+![Coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/surquest/373e1859cb547514516a8f22cd8f18a7/raw/python-split-balancer.json&style=flat-square)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/surquest-GCP-secret-assessor?style=flat-square)
 
 # Introduction
 
 This project provides a Python package and REST API applications for dividing a set of units into two most comparable groups based on their characteristics.
 
 ## Problem Statement
```

