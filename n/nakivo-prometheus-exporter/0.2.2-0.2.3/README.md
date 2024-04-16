# Comparing `tmp/nakivo_prometheus_exporter-0.2.2.tar.gz` & `tmp/nakivo_prometheus_exporter-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nakivo_prometheus_exporter-0.2.2.tar", last modified: Fri Apr  5 14:14:44 2024, max compression
+gzip compressed data, was "nakivo_prometheus_exporter-0.2.3.tar", last modified: Tue Apr 16 13:22:56 2024, max compression
```

## Comparing `nakivo_prometheus_exporter-0.2.2.tar` & `nakivo_prometheus_exporter-0.2.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 14:14:44.941533 nakivo_prometheus_exporter-0.2.2/
--rw-rw-rw-   0        0        0     5683 2024-04-05 14:14:44.941533 nakivo_prometheus_exporter-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     3816 2024-04-05 13:49:48.000000 nakivo_prometheus_exporter-0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-05 14:14:44.891649 nakivo_prometheus_exporter-0.2.2/nakivo_prometheus_exporter/
--rw-rw-rw-   0        0        0     1651 2024-04-05 13:26:41.000000 nakivo_prometheus_exporter-0.2.2/nakivo_prometheus_exporter/__debug__.py
--rw-rw-rw-   0        0        0      104 2024-03-26 13:49:20.000000 nakivo_prometheus_exporter-0.2.2/nakivo_prometheus_exporter/__init__.py
--rw-rw-rw-   0        0        0      440 2024-04-05 14:13:45.000000 nakivo_prometheus_exporter-0.2.2/nakivo_prometheus_exporter/__version__.py
--rw-rw-rw-   0        0        0     3382 2024-04-05 13:24:38.000000 nakivo_prometheus_exporter-0.2.2/nakivo_prometheus_exporter/metrics.py
--rw-rw-rw-   0        0        0     4088 2024-04-05 13:24:38.000000 nakivo_prometheus_exporter-0.2.2/nakivo_prometheus_exporter/nakivo_api.py
--rw-rw-rw-   0        0        0    11030 2024-04-05 13:58:47.000000 nakivo_prometheus_exporter-0.2.2/nakivo_prometheus_exporter/prom_parser.py
--rw-rw-rw-   0        0        0     4715 2024-04-05 13:54:13.000000 nakivo_prometheus_exporter-0.2.2/nakivo_prometheus_exporter/server.py
-drwxrwxrwx   0        0        0        0 2024-04-05 14:14:44.932890 nakivo_prometheus_exporter-0.2.2/nakivo_prometheus_exporter.egg-info/
--rw-rw-rw-   0        0        0     5683 2024-04-05 14:14:44.000000 nakivo_prometheus_exporter-0.2.2/nakivo_prometheus_exporter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      599 2024-04-05 14:14:44.000000 nakivo_prometheus_exporter-0.2.2/nakivo_prometheus_exporter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 14:14:44.000000 nakivo_prometheus_exporter-0.2.2/nakivo_prometheus_exporter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       86 2024-04-05 14:14:44.000000 nakivo_prometheus_exporter-0.2.2/nakivo_prometheus_exporter.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      169 2024-04-05 14:14:44.000000 nakivo_prometheus_exporter-0.2.2/nakivo_prometheus_exporter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2024-04-05 14:14:44.000000 nakivo_prometheus_exporter-0.2.2/nakivo_prometheus_exporter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-05 14:14:44.944702 nakivo_prometheus_exporter-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0     5248 2024-03-26 16:09:56.000000 nakivo_prometheus_exporter-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 13:22:56.646417 nakivo_prometheus_exporter-0.2.3/
+-rw-rw-rw-   0        0        0     5878 2024-04-16 13:22:56.644405 nakivo_prometheus_exporter-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4011 2024-04-05 14:17:03.000000 nakivo_prometheus_exporter-0.2.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-16 13:22:56.594307 nakivo_prometheus_exporter-0.2.3/nakivo_prometheus_exporter/
+-rw-rw-rw-   0        0        0     1651 2024-04-05 13:26:41.000000 nakivo_prometheus_exporter-0.2.3/nakivo_prometheus_exporter/__debug__.py
+-rw-rw-rw-   0        0        0      104 2024-03-26 13:49:20.000000 nakivo_prometheus_exporter-0.2.3/nakivo_prometheus_exporter/__init__.py
+-rw-rw-rw-   0        0        0      440 2024-04-16 13:21:46.000000 nakivo_prometheus_exporter-0.2.3/nakivo_prometheus_exporter/__version__.py
+-rw-rw-rw-   0        0        0     3382 2024-04-05 13:24:38.000000 nakivo_prometheus_exporter-0.2.3/nakivo_prometheus_exporter/metrics.py
+-rw-rw-rw-   0        0        0     4088 2024-04-05 13:24:38.000000 nakivo_prometheus_exporter-0.2.3/nakivo_prometheus_exporter/nakivo_api.py
+-rw-rw-rw-   0        0        0    11041 2024-04-16 13:21:36.000000 nakivo_prometheus_exporter-0.2.3/nakivo_prometheus_exporter/prom_parser.py
+-rw-rw-rw-   0        0        0     4715 2024-04-05 13:54:13.000000 nakivo_prometheus_exporter-0.2.3/nakivo_prometheus_exporter/server.py
+drwxrwxrwx   0        0        0        0 2024-04-16 13:22:56.635268 nakivo_prometheus_exporter-0.2.3/nakivo_prometheus_exporter.egg-info/
+-rw-rw-rw-   0        0        0     5878 2024-04-16 13:22:56.000000 nakivo_prometheus_exporter-0.2.3/nakivo_prometheus_exporter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      599 2024-04-16 13:22:56.000000 nakivo_prometheus_exporter-0.2.3/nakivo_prometheus_exporter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 13:22:56.000000 nakivo_prometheus_exporter-0.2.3/nakivo_prometheus_exporter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       86 2024-04-16 13:22:56.000000 nakivo_prometheus_exporter-0.2.3/nakivo_prometheus_exporter.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      169 2024-04-16 13:22:56.000000 nakivo_prometheus_exporter-0.2.3/nakivo_prometheus_exporter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2024-04-16 13:22:56.000000 nakivo_prometheus_exporter-0.2.3/nakivo_prometheus_exporter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-16 13:22:56.646417 nakivo_prometheus_exporter-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     5248 2024-03-26 16:09:56.000000 nakivo_prometheus_exporter-0.2.3/setup.py
```

### Comparing `nakivo_prometheus_exporter-0.2.2/PKG-INFO` & `nakivo_prometheus_exporter-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nakivo_prometheus_exporter
-Version: 0.2.2
+Version: 0.2.3
 Summary: Connecto to Nakivo API and export metrics to Prometheus
 Home-page: https://github.com/netinvent/nakivo_prometheus_exporter
 Author: NetInvent - Orsiris de Jong
 Author-email: contact@netinvent.fr
 License: GPLv3
 Keywords: shell,backup,prometheus,linux,cli
 Classifier: Development Status :: 5 - Production/Stable
@@ -130,10 +130,18 @@
 If some traction is obersved for the project, we might add missing or interesting metrics.
 
 ## Running on Windows
 
 While this typically targets Linux, one can run this exporter on Windows, as single threaded instance without concurrency.
 Running as service can be achieved via nssm.
 
+## Troubleshooting
+
+You can enable debugging in order to have more info with
+```
+export _DEBUG=true
+/usr/local/bin/nakivo_prometheus_exporter -c /etc/nakivo_prometheus.exporter.yaml
+```
+
 ## Like it ?
 
 Write us ;)
```

### Comparing `nakivo_prometheus_exporter-0.2.2/README.md` & `nakivo_prometheus_exporter-0.2.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -87,10 +87,18 @@
 If some traction is obersved for the project, we might add missing or interesting metrics.
 
 ## Running on Windows
 
 While this typically targets Linux, one can run this exporter on Windows, as single threaded instance without concurrency.
 Running as service can be achieved via nssm.
 
+## Troubleshooting
+
+You can enable debugging in order to have more info with
+```
+export _DEBUG=true
+/usr/local/bin/nakivo_prometheus_exporter -c /etc/nakivo_prometheus.exporter.yaml
+```
+
 ## Like it ?
 
 Write us ;)
```

### Comparing `nakivo_prometheus_exporter-0.2.2/nakivo_prometheus_exporter/__debug__.py` & `nakivo_prometheus_exporter-0.2.3/nakivo_prometheus_exporter/__debug__.py`

 * *Files identical despite different names*

### Comparing `nakivo_prometheus_exporter-0.2.2/nakivo_prometheus_exporter/metrics.py` & `nakivo_prometheus_exporter-0.2.3/nakivo_prometheus_exporter/metrics.py`

 * *Files identical despite different names*

### Comparing `nakivo_prometheus_exporter-0.2.2/nakivo_prometheus_exporter/nakivo_api.py` & `nakivo_prometheus_exporter-0.2.3/nakivo_prometheus_exporter/nakivo_api.py`

 * *Files identical despite different names*

### Comparing `nakivo_prometheus_exporter-0.2.2/nakivo_prometheus_exporter/prom_parser.py` & `nakivo_prometheus_exporter-0.2.3/nakivo_prometheus_exporter/prom_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 __appname__ = "nakivo_prometheus_exporter"
 __author__ = "Orsiris de Jong"
 __site__ = "https://www.github.com/netinvent/nakivo_prometheus_exporter"
 __description__ = "Naviko API Prometheus data exporter"
 __copyright__ = "Copyright (C) 2024 NetInvent"
 __license__ = "GPL-3.0-only"
-__build__ = "2024040501"
+__build__ = "2024041601"
 
 
 import sys
 from argparse import ArgumentParser
 from typing import Union
 from ruamel.yaml import YAML
 from pathlib import Path
@@ -173,15 +173,15 @@
         for vm in job["objects"]:
             name = vm["sourceName"]
             state = vm["lrState"]
             # States used in prometheus will be 0 = all okay, 1 = warnings, 2 = failures
             if isinstance(state, str):
                 if state in ("SUCCEEDED"):
                     num_state = 0
-                elif state in ("RUNNING", "DEMAND", "SCHEDULED", "WAITING"):
+                elif state in ("RUNNING", "DEMAND", "SCHEDULED", "WAITING", "SKIPPED"):
                     num_state = 1
                 else:
                     num_state = 2
             else:
                 # If lrState is null, it means that the job has not yet been executed once on the child, let's put a warning state by default
                 num_state = 1
             prom_data += f'nakivo_backup_state{{host="{host}",object="{name}",job_name="{job_name}"}} {num_state}\n'
```

### Comparing `nakivo_prometheus_exporter-0.2.2/nakivo_prometheus_exporter/server.py` & `nakivo_prometheus_exporter-0.2.3/nakivo_prometheus_exporter/server.py`

 * *Files identical despite different names*

### Comparing `nakivo_prometheus_exporter-0.2.2/nakivo_prometheus_exporter.egg-info/PKG-INFO` & `nakivo_prometheus_exporter-0.2.3/nakivo_prometheus_exporter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nakivo_prometheus_exporter
-Version: 0.2.2
+Version: 0.2.3
 Summary: Connecto to Nakivo API and export metrics to Prometheus
 Home-page: https://github.com/netinvent/nakivo_prometheus_exporter
 Author: NetInvent - Orsiris de Jong
 Author-email: contact@netinvent.fr
 License: GPLv3
 Keywords: shell,backup,prometheus,linux,cli
 Classifier: Development Status :: 5 - Production/Stable
@@ -130,10 +130,18 @@
 If some traction is obersved for the project, we might add missing or interesting metrics.
 
 ## Running on Windows
 
 While this typically targets Linux, one can run this exporter on Windows, as single threaded instance without concurrency.
 Running as service can be achieved via nssm.
 
+## Troubleshooting
+
+You can enable debugging in order to have more info with
+```
+export _DEBUG=true
+/usr/local/bin/nakivo_prometheus_exporter -c /etc/nakivo_prometheus.exporter.yaml
+```
+
 ## Like it ?
 
 Write us ;)
```

### Comparing `nakivo_prometheus_exporter-0.2.2/nakivo_prometheus_exporter.egg-info/SOURCES.txt` & `nakivo_prometheus_exporter-0.2.3/nakivo_prometheus_exporter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nakivo_prometheus_exporter-0.2.2/setup.py` & `nakivo_prometheus_exporter-0.2.3/setup.py`

 * *Files identical despite different names*

