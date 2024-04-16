# Comparing `tmp/ai-models-0.5.1.tar.gz` & `tmp/ai-models-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai-models-0.5.1.tar", last modified: Mon Apr 15 13:14:47 2024, max compression
+gzip compressed data, was "ai-models-0.5.2.tar", last modified: Tue Apr 16 13:10:20 2024, max compression
```

## Comparing `ai-models-0.5.1.tar` & `ai-models-0.5.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:14:47.752941 ai-models-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-15 13:14:36.000000 ai-models-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8930 2024-04-15 13:14:47.752941 ai-models-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7995 2024-04-15 13:14:36.000000 ai-models-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:14:47.748941 ai-models-0.5.1/ai_models/
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-15 13:14:36.000000 ai-models-0.5.1/ai_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8788 2024-04-15 13:14:36.000000 ai-models-0.5.1/ai_models/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-15 13:14:36.000000 ai-models-0.5.1/ai_models/checkpoint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:14:47.748941 ai-models-0.5.1/ai_models/inputs/
--rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-04-15 13:14:36.000000 ai-models-0.5.1/ai_models/inputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13834 2024-04-15 13:14:36.000000 ai-models-0.5.1/ai_models/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:14:47.752941 ai-models-0.5.1/ai_models/outputs/
--rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-04-15 13:14:36.000000 ai-models-0.5.1/ai_models/outputs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:14:47.752941 ai-models-0.5.1/ai_models/remote/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-15 13:14:36.000000 ai-models-0.5.1/ai_models/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5394 2024-04-15 13:14:36.000000 ai-models-0.5.1/ai_models/remote/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-15 13:14:36.000000 ai-models-0.5.1/ai_models/remote/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-04-15 13:14:36.000000 ai-models-0.5.1/ai_models/remote/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-15 13:14:36.000000 ai-models-0.5.1/ai_models/stepper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:14:47.748941 ai-models-0.5.1/ai_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8930 2024-04-15 13:14:47.000000 ai-models-0.5.1/ai_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-15 13:14:47.000000 ai-models-0.5.1/ai_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 13:14:47.000000 ai-models-0.5.1/ai_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-15 13:14:47.000000 ai-models-0.5.1/ai_models.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-15 13:14:47.000000 ai-models-0.5.1/ai_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-15 13:14:47.000000 ai-models-0.5.1/ai_models.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 13:14:47.000000 ai-models-0.5.1/ai_models.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 13:14:47.752941 ai-models-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-04-15 13:14:36.000000 ai-models-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:10:20.093562 ai-models-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-16 13:10:08.000000 ai-models-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8930 2024-04-16 13:10:20.093562 ai-models-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7995 2024-04-16 13:10:08.000000 ai-models-0.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:10:20.089562 ai-models-0.5.2/ai_models/
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-16 13:10:08.000000 ai-models-0.5.2/ai_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8788 2024-04-16 13:10:08.000000 ai-models-0.5.2/ai_models/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-16 13:10:08.000000 ai-models-0.5.2/ai_models/checkpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:10:20.089562 ai-models-0.5.2/ai_models/inputs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-04-16 13:10:08.000000 ai-models-0.5.2/ai_models/inputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13834 2024-04-16 13:10:08.000000 ai-models-0.5.2/ai_models/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:10:20.089562 ai-models-0.5.2/ai_models/outputs/
+-rw-r--r--   0 runner    (1001) docker     (127)     4556 2024-04-16 13:10:08.000000 ai-models-0.5.2/ai_models/outputs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:10:20.093562 ai-models-0.5.2/ai_models/remote/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-16 13:10:08.000000 ai-models-0.5.2/ai_models/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5394 2024-04-16 13:10:08.000000 ai-models-0.5.2/ai_models/remote/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-16 13:10:08.000000 ai-models-0.5.2/ai_models/remote/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-04-16 13:10:08.000000 ai-models-0.5.2/ai_models/remote/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-16 13:10:08.000000 ai-models-0.5.2/ai_models/stepper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:10:20.089562 ai-models-0.5.2/ai_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8930 2024-04-16 13:10:20.000000 ai-models-0.5.2/ai_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-16 13:10:20.000000 ai-models-0.5.2/ai_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 13:10:20.000000 ai-models-0.5.2/ai_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-16 13:10:20.000000 ai-models-0.5.2/ai_models.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-16 13:10:20.000000 ai-models-0.5.2/ai_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-16 13:10:20.000000 ai-models-0.5.2/ai_models.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 13:10:20.000000 ai-models-0.5.2/ai_models.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 13:10:20.093562 ai-models-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-04-16 13:10:08.000000 ai-models-0.5.2/setup.py
```

### Comparing `ai-models-0.5.1/LICENSE` & `ai-models-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ai-models-0.5.1/PKG-INFO` & `ai-models-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-models
-Version: 0.5.1
+Version: 0.5.2
 Summary: A package to run AI weather models
 Home-page: https://github.com/ecmwf-lab/ai-models
 Author: European Centre for Medium-Range Weather Forecasts (ECMWF)
 Author-email: software.support@ecmwf.int
 License: Apache License Version 2.0
 Keywords: tool
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ai-models-0.5.1/README.md` & `ai-models-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `ai-models-0.5.1/ai_models/__main__.py` & `ai-models-0.5.2/ai_models/__main__.py`

 * *Files identical despite different names*

### Comparing `ai-models-0.5.1/ai_models/checkpoint.py` & `ai-models-0.5.2/ai_models/checkpoint.py`

 * *Files identical despite different names*

### Comparing `ai-models-0.5.1/ai_models/inputs/__init__.py` & `ai-models-0.5.2/ai_models/inputs/__init__.py`

 * *Files identical despite different names*

### Comparing `ai-models-0.5.1/ai_models/model.py` & `ai-models-0.5.2/ai_models/model.py`

 * *Files identical despite different names*

### Comparing `ai-models-0.5.1/ai_models/outputs/__init__.py` & `ai-models-0.5.2/ai_models/outputs/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # which can be obtained at http://www.apache.org/licenses/LICENSE-2.0.
 # In applying this licence, ECMWF does not waive the privileges and immunities
 # granted to it by virtue of its status as an intergovernmental organisation
 # nor does it submit to any jurisdiction.
 
 import itertools
 import logging
+import warnings
 from functools import cached_property
 
 import climetlab as cml
 import entrypoints
 import numpy as np
 
 LOG = logging.getLogger(__name__)
@@ -42,27 +43,29 @@
         return cml.new_grib_output(
             self.path,
             split_output=True,
             **self.grib_keys,
         )
 
     def write(self, data, *args, check=False, **kwargs):
+
         try:
             handle, path = self.output.write(data, *args, **kwargs)
 
         except Exception:
-            if np.isnan(data).any():
-                raise ValueError(
-                    f"NaN values found in field. args={args} kwargs={kwargs}"
-                )
-            if np.isinf(data).any():
-                raise ValueError(
-                    f"Infinite values found in field. args={args} kwargs={kwargs}"
-                )
-            raise
+            if data is not None:
+                if np.isnan(data).any():
+                    raise ValueError(
+                        f"NaN values found in field. args={args} kwargs={kwargs}"
+                    )
+                if np.isinf(data).any():
+                    raise ValueError(
+                        f"Infinite values found in field. args={args} kwargs={kwargs}"
+                    )
+                raise
 
         if check:
             # Check that the GRIB keys are as expected
             for key, value in itertools.chain(self.grib_keys.items(), kwargs.items()):
                 if key in ("template",):
                     continue
 
@@ -81,16 +84,25 @@
 class HindcastReLabel:
     def __init__(self, owner, output, hindcast_reference_year, **kwargs):
         self.owner = owner
         self.output = output
         self.hindcast_reference_year = int(hindcast_reference_year)
 
     def write(self, *args, **kwargs):
-        assert "hdate" not in kwargs, kwargs
-        assert "date" not in kwargs, kwargs
+        if "hdate" in kwargs:
+            warnings.warn(
+                f"Ignoring hdate='{kwargs['hdate']}' in HindcastReLabel", stacklevel=3
+            )
+            kwargs.pop("hdate")
+
+        if "date" in kwargs:
+            warnings.warn(
+                f"Ignoring date='{kwargs['date']}' in HindcastReLabel", stacklevel=3
+            )
+            kwargs.pop("date")
 
         date = kwargs["template"]["date"]
         hdate = kwargs["template"]["hdate"]
 
         if hdate is not None:
             # Input was a hindcast
             referenceDate = self.hindcast_reference_year * 10000 + date % 10000
@@ -103,15 +115,17 @@
             kwargs["referenceDate"] = referenceDate
             kwargs["hdate"] = hdate
         else:
             referenceDate = self.hindcast_reference_year * 10000 + date % 10000
             kwargs["referenceDate"] = referenceDate
             kwargs["hdate"] = date
 
-        return self.output.write(*args, check=True, **kwargs)
+        kwargs.setdefault("check", True)
+
+        return self.output.write(*args, **kwargs)
 
 
 class NoneOutput:
     def __init__(self, *args, **kwargs):
         LOG.info("Results will not be written.")
 
     def write(self, *args, **kwargs):
```

### Comparing `ai-models-0.5.1/ai_models/remote/api.py` & `ai-models-0.5.2/ai_models/remote/api.py`

 * *Files identical despite different names*

### Comparing `ai-models-0.5.1/ai_models/remote/config.py` & `ai-models-0.5.2/ai_models/remote/config.py`

 * *Files identical despite different names*

### Comparing `ai-models-0.5.1/ai_models/remote/model.py` & `ai-models-0.5.2/ai_models/remote/model.py`

 * *Files identical despite different names*

### Comparing `ai-models-0.5.1/ai_models/stepper.py` & `ai-models-0.5.2/ai_models/stepper.py`

 * *Files identical despite different names*

### Comparing `ai-models-0.5.1/ai_models.egg-info/PKG-INFO` & `ai-models-0.5.2/ai_models.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-models
-Version: 0.5.1
+Version: 0.5.2
 Summary: A package to run AI weather models
 Home-page: https://github.com/ecmwf-lab/ai-models
 Author: European Centre for Medium-Range Weather Forecasts (ECMWF)
 Author-email: software.support@ecmwf.int
 License: Apache License Version 2.0
 Keywords: tool
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ai-models-0.5.1/ai_models.egg-info/SOURCES.txt` & `ai-models-0.5.2/ai_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ai-models-0.5.1/setup.py` & `ai-models-0.5.2/setup.py`

 * *Files identical despite different names*

