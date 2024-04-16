# Comparing `tmp/sciveo-0.0.48.tar.gz` & `tmp/sciveo-0.0.49.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sciveo-0.0.48.tar", last modified: Sun Apr 14 11:47:40 2024, max compression
+gzip compressed data, was "sciveo-0.0.49.tar", last modified: Tue Apr 16 17:56:09 2024, max compression
```

## Comparing `sciveo-0.0.48.tar` & `sciveo-0.0.49.tar`

### file list

```diff
@@ -1,46 +1,48 @@
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-14 11:47:40.402833 sciveo-0.0.48/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     6168 2024-04-14 11:47:40.402677 sciveo-0.0.48/PKG-INFO
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     6055 2024-04-10 20:04:28.000000 sciveo-0.0.48/README.md
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-14 11:47:40.377834 sciveo-0.0.48/sciveo/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1297 2024-04-13 06:50:59.000000 sciveo-0.0.48/sciveo/__init__.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-14 11:47:40.388895 sciveo-0.0.48/sciveo/api/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:04:12.000000 sciveo-0.0.48/sciveo/api/__init__.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1788 2024-04-07 18:52:23.000000 sciveo-0.0.48/sciveo/api/base.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1815 2024-04-05 16:37:24.000000 sciveo-0.0.48/sciveo/api/upload.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-14 11:47:40.391373 sciveo-0.0.48/sciveo/common/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:03:59.000000 sciveo-0.0.48/sciveo/common/__init__.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     2043 2024-03-14 17:02:24.000000 sciveo-0.0.48/sciveo/common/configuration.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1583 2024-03-14 17:02:24.000000 sciveo-0.0.48/sciveo/common/model.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     3842 2024-04-07 18:52:23.000000 sciveo-0.0.48/sciveo/common/optimizers.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)    10567 2024-03-19 14:47:24.000000 sciveo-0.0.48/sciveo/common/sampling.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-14 11:47:40.395887 sciveo-0.0.48/sciveo/common/tools/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:07:07.000000 sciveo-0.0.48/sciveo/common/tools/__init__.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1416 2024-04-13 06:51:43.000000 sciveo-0.0.48/sciveo/common/tools/daemon.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1053 2023-11-17 12:42:35.000000 sciveo-0.0.48/sciveo/common/tools/formating.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1654 2024-04-14 08:49:26.000000 sciveo-0.0.48/sciveo/common/tools/hardware.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1071 2023-11-15 15:21:05.000000 sciveo-0.0.48/sciveo/common/tools/logger.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1102 2023-12-10 07:08:19.000000 sciveo-0.0.48/sciveo/common/tools/synchronized.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-14 11:47:40.399212 sciveo-0.0.48/sciveo/content/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:14:23.000000 sciveo-0.0.48/sciveo/content/__init__.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)      827 2024-03-14 17:02:24.000000 sciveo-0.0.48/sciveo/content/dataset.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     5859 2024-04-07 18:52:23.000000 sciveo-0.0.48/sciveo/content/experiment.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     3129 2024-04-07 18:52:23.000000 sciveo-0.0.48/sciveo/content/project.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     2015 2024-03-19 14:47:07.000000 sciveo-0.0.48/sciveo/content/runner.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-14 11:47:40.400143 sciveo-0.0.48/sciveo/monitoring/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2024-04-07 18:52:23.000000 sciveo-0.0.48/sciveo/monitoring/__init__.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     5380 2024-04-14 11:46:31.000000 sciveo-0.0.48/sciveo/monitoring/monitor.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1440 2024-04-13 06:48:20.000000 sciveo-0.0.48/sciveo/monitoring/start.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)       24 2024-04-14 11:36:47.000000 sciveo-0.0.48/sciveo/version.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-14 11:47:40.387996 sciveo-0.0.48/sciveo.egg-info/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     6168 2024-04-14 11:47:40.000000 sciveo-0.0.48/sciveo.egg-info/PKG-INFO
--rw-r--r--   0 sgeorgiev   (501) staff       (20)      906 2024-04-14 11:47:40.000000 sciveo-0.0.48/sciveo.egg-info/SOURCES.txt
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        1 2024-04-14 11:47:40.000000 sciveo-0.0.48/sciveo.egg-info/dependency_links.txt
--rw-r--r--   0 sgeorgiev   (501) staff       (20)       50 2024-04-14 11:47:40.000000 sciveo-0.0.48/sciveo.egg-info/requires.txt
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        7 2024-04-14 11:47:40.000000 sciveo-0.0.48/sciveo.egg-info/top_level.txt
--rw-r--r--   0 sgeorgiev   (501) staff       (20)       38 2024-04-14 11:47:40.402884 sciveo-0.0.48/setup.cfg
--rw-r--r--   0 sgeorgiev   (501) staff       (20)      418 2024-04-07 18:52:23.000000 sciveo-0.0.48/setup.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-14 11:47:40.402321 sciveo-0.0.48/test/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)      521 2024-03-14 17:02:24.000000 sciveo-0.0.48/test/test_configuration.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     3256 2024-04-10 18:44:45.000000 sciveo-0.0.48/test/test_monitoring.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1554 2024-03-19 14:47:07.000000 sciveo-0.0.48/test/test_runner.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     9045 2024-03-19 14:47:24.000000 sciveo-0.0.48/test/test_sampling.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-16 17:56:09.946414 sciveo-0.0.49/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     6208 2024-04-16 17:56:09.946226 sciveo-0.0.49/PKG-INFO
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     6055 2024-04-10 20:04:28.000000 sciveo-0.0.49/README.md
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-16 17:56:09.930226 sciveo-0.0.49/sciveo/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1428 2024-04-16 17:53:18.000000 sciveo-0.0.49/sciveo/__init__.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-16 17:56:09.934712 sciveo-0.0.49/sciveo/api/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:04:12.000000 sciveo-0.0.49/sciveo/api/__init__.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1788 2024-04-16 17:39:04.000000 sciveo-0.0.49/sciveo/api/base.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1815 2024-04-05 16:37:24.000000 sciveo-0.0.49/sciveo/api/upload.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-16 17:56:09.936430 sciveo-0.0.49/sciveo/common/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:03:59.000000 sciveo-0.0.49/sciveo/common/__init__.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     2043 2024-03-14 17:02:24.000000 sciveo-0.0.49/sciveo/common/configuration.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1583 2024-03-14 17:02:24.000000 sciveo-0.0.49/sciveo/common/model.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     3842 2024-04-07 18:52:23.000000 sciveo-0.0.49/sciveo/common/optimizers.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)    10567 2024-03-19 14:47:24.000000 sciveo-0.0.49/sciveo/common/sampling.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-16 17:56:09.939264 sciveo-0.0.49/sciveo/common/tools/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:07:07.000000 sciveo-0.0.49/sciveo/common/tools/__init__.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1647 2024-04-16 17:39:58.000000 sciveo-0.0.49/sciveo/common/tools/daemon.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1053 2023-11-17 12:42:35.000000 sciveo-0.0.49/sciveo/common/tools/formating.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1654 2024-04-14 08:49:26.000000 sciveo-0.0.49/sciveo/common/tools/hardware.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1071 2023-11-15 15:21:05.000000 sciveo-0.0.49/sciveo/common/tools/logger.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1333 2024-04-16 17:40:12.000000 sciveo-0.0.49/sciveo/common/tools/synchronized.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1087 2024-04-16 17:42:03.000000 sciveo-0.0.49/sciveo/common/tools/timers.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-16 17:56:09.940768 sciveo-0.0.49/sciveo/content/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:14:23.000000 sciveo-0.0.49/sciveo/content/__init__.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)      827 2024-03-14 17:02:24.000000 sciveo-0.0.49/sciveo/content/dataset.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     5859 2024-04-07 18:52:23.000000 sciveo-0.0.49/sciveo/content/experiment.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     3129 2024-04-07 18:52:23.000000 sciveo-0.0.49/sciveo/content/project.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     2015 2024-03-19 14:47:07.000000 sciveo-0.0.49/sciveo/content/runner.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-16 17:56:09.941964 sciveo-0.0.49/sciveo/monitoring/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2024-04-07 18:52:23.000000 sciveo-0.0.49/sciveo/monitoring/__init__.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     5380 2024-04-14 11:46:31.000000 sciveo-0.0.49/sciveo/monitoring/monitor.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     2564 2024-04-16 17:50:56.000000 sciveo-0.0.49/sciveo/monitoring/network.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1671 2024-04-16 17:41:11.000000 sciveo-0.0.49/sciveo/monitoring/start.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)       24 2024-04-16 17:56:04.000000 sciveo-0.0.49/sciveo/version.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-16 17:56:09.933777 sciveo-0.0.49/sciveo.egg-info/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     6208 2024-04-16 17:56:09.000000 sciveo-0.0.49/sciveo.egg-info/PKG-INFO
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)      965 2024-04-16 17:56:09.000000 sciveo-0.0.49/sciveo.egg-info/SOURCES.txt
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        1 2024-04-16 17:56:09.000000 sciveo-0.0.49/sciveo.egg-info/dependency_links.txt
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)      112 2024-04-16 17:56:09.000000 sciveo-0.0.49/sciveo.egg-info/requires.txt
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        7 2024-04-16 17:56:09.000000 sciveo-0.0.49/sciveo.egg-info/top_level.txt
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)       38 2024-04-16 17:56:09.946472 sciveo-0.0.49/setup.cfg
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)      778 2024-04-16 17:42:22.000000 sciveo-0.0.49/setup.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-16 17:56:09.945889 sciveo-0.0.49/test/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)      521 2024-03-14 17:02:24.000000 sciveo-0.0.49/test/test_configuration.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     3256 2024-04-10 18:44:45.000000 sciveo-0.0.49/test/test_monitoring.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1554 2024-03-19 14:47:07.000000 sciveo-0.0.49/test/test_runner.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     9045 2024-03-19 14:47:24.000000 sciveo-0.0.49/test/test_sampling.py
```

### Comparing `sciveo-0.0.48/PKG-INFO` & `sciveo-0.0.49/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 Metadata-Version: 2.1
 Name: sciveo
-Version: 0.0.48
+Version: 0.0.49
 Description-Content-Type: text/markdown
 Provides-Extra: mon
+Provides-Extra: net
+Provides-Extra: all
 
 # SCIVEO - ML/Scientific Experiments Management Client
 
 `sciveo` is a Python library that serves as a client for managing machine learning and scientific experiments on the sciveo.com platform. This library provides a convenient interface to interact with the sciveo.com API, enabling users to organize, track, and analyze their experiments efficiently.
 There are few configuration params samplers, which allows easy parameter tuning. The "auto" sampler perhaps is the easiest to use, but also
 "random" and "grid" ones are available.
```

### Comparing `sciveo-0.0.48/README.md` & `sciveo-0.0.49/README.md`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.48/sciveo/__init__.py` & `sciveo-0.0.49/sciveo/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -17,14 +17,15 @@
   import time
 
   from sciveo.common.tools.logger import *
   from sciveo.common.tools.daemon import TasksDaemon, __upload_content__
   from sciveo.content.runner import ProjectRunner
   from sciveo.content.dataset import Dataset
   from sciveo.monitoring.start import MonitorStart
+  from sciveo.monitoring.network import NetworkTools
   from sciveo.version import __version__
 
 
   TasksDaemon.current = TasksDaemon(num_threads=int(os.environ.get("SCIVEO_TASKS_NUM_THREADS", 1)))
 
 
   # New Experiment
@@ -43,9 +44,13 @@
   def dataset(info={}):
     return Dataset.get(info)
 
   # Monitoring start
   def monitor(**kwargs):
     MonitorStart(**kwargs)()
 
+  # Network tools
+  def network(**kwargs):
+    return NetworkTools(**kwargs)
+
 except ImportError as e:
   pass
```

### Comparing `sciveo-0.0.48/sciveo/api/base.py` & `sciveo-0.0.49/sciveo/api/base.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.48/sciveo/api/upload.py` & `sciveo-0.0.49/sciveo/api/upload.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.48/sciveo/common/configuration.py` & `sciveo-0.0.49/sciveo/common/configuration.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.48/sciveo/common/model.py` & `sciveo-0.0.49/sciveo/common/model.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.48/sciveo/common/optimizers.py` & `sciveo-0.0.49/sciveo/common/optimizers.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.48/sciveo/common/sampling.py` & `sciveo-0.0.49/sciveo/common/sampling.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.48/sciveo/common/tools/daemon.py` & `sciveo-0.0.49/sciveo/common/tools/daemon.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+#
+# Pavlin Georgiev, Softel Labs
+#
+# This is a proprietary file and may not be copied,
+# distributed, or modified without express permission
+# from the owner. For licensing inquiries, please
+# contact pavlin@softel.bg.
+#
+# 2023
+#
+
 import threading
 import time
 
 from sciveo.common.tools.logger import *
 from sciveo.common.tools.synchronized import ListQueue
 from sciveo.api.upload import APIFileUploader
```

### Comparing `sciveo-0.0.48/sciveo/common/tools/formating.py` & `sciveo-0.0.49/sciveo/common/tools/formating.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.48/sciveo/common/tools/hardware.py` & `sciveo-0.0.49/sciveo/common/tools/hardware.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.48/sciveo/common/tools/logger.py` & `sciveo-0.0.49/sciveo/common/tools/logger.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.48/sciveo/content/dataset.py` & `sciveo-0.0.49/sciveo/content/dataset.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.48/sciveo/content/experiment.py` & `sciveo-0.0.49/sciveo/content/experiment.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.48/sciveo/content/project.py` & `sciveo-0.0.49/sciveo/content/project.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.48/sciveo/content/runner.py` & `sciveo-0.0.49/sciveo/content/runner.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.48/sciveo/monitoring/monitor.py` & `sciveo-0.0.49/sciveo/monitoring/monitor.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.48/sciveo/monitoring/start.py` & `sciveo-0.0.49/sciveo/monitoring/start.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+#
+# Pavlin Georgiev, Softel Labs
+#
+# This is a proprietary file and may not be copied,
+# distributed, or modified without express permission
+# from the owner. For licensing inquiries, please
+# contact pavlin@softel.bg.
+#
+# 2024
+#
+
 import os
 import time
 
 from sciveo.common.tools.logger import *
 from sciveo.monitoring.monitor import BaseMonitor
```

### Comparing `sciveo-0.0.48/sciveo.egg-info/PKG-INFO` & `sciveo-0.0.49/sciveo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 Metadata-Version: 2.1
 Name: sciveo
-Version: 0.0.48
+Version: 0.0.49
 Description-Content-Type: text/markdown
 Provides-Extra: mon
+Provides-Extra: net
+Provides-Extra: all
 
 # SCIVEO - ML/Scientific Experiments Management Client
 
 `sciveo` is a Python library that serves as a client for managing machine learning and scientific experiments on the sciveo.com platform. This library provides a convenient interface to interact with the sciveo.com API, enabling users to organize, track, and analyze their experiments efficiently.
 There are few configuration params samplers, which allows easy parameter tuning. The "auto" sampler perhaps is the easiest to use, but also
 "random" and "grid" ones are available.
```

### Comparing `sciveo-0.0.48/test/test_configuration.py` & `sciveo-0.0.49/test/test_configuration.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.48/test/test_monitoring.py` & `sciveo-0.0.49/test/test_monitoring.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.48/test/test_runner.py` & `sciveo-0.0.49/test/test_runner.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.48/test/test_sampling.py` & `sciveo-0.0.49/test/test_sampling.py`

 * *Files identical despite different names*

