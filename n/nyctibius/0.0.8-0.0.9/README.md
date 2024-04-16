# Comparing `tmp/nyctibius-0.0.8.tar.gz` & `tmp/nyctibius-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nyctibius-0.0.8.tar", last modified: Tue Apr  9 01:54:39 2024, max compression
+gzip compressed data, was "nyctibius-0.0.9.tar", last modified: Tue Apr  9 02:12:44 2024, max compression
```

## Comparing `nyctibius-0.0.8.tar` & `nyctibius-0.0.9.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 01:54:39.921010 nyctibius-0.0.8/
--rw-rw-rw-   0        0        0     7950 2024-04-09 01:54:39.920015 nyctibius-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     6692 2024-04-01 17:34:43.000000 nyctibius-0.0.8/README.md
--rw-rw-rw-   0        0        0       42 2024-04-09 01:54:39.921010 nyctibius-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     8551 2024-04-09 01:54:26.000000 nyctibius-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-09 01:54:39.712000 nyctibius-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2024-04-09 01:54:39.768001 nyctibius-0.0.8/src/nyctibius/
--rw-rw-rw-   0        0        0       69 2024-04-09 01:07:48.000000 nyctibius-0.0.8/src/nyctibius/__init__.py
--rw-rw-rw-   0        0        0     3290 2024-04-09 01:07:48.000000 nyctibius-0.0.8/src/nyctibius/__main__.py
--rw-rw-rw-   0        0        0    10370 2024-04-09 01:07:48.000000 nyctibius-0.0.8/src/nyctibius/bird_agent.py
--rw-rw-rw-   0        0        0        0 2023-11-22 03:20:49.000000 nyctibius-0.0.8/src/nyctibius/config.py
-drwxrwxrwx   0        0        0        0 2024-04-09 01:54:39.783005 nyctibius-0.0.8/src/nyctibius/db/
--rw-rw-rw-   0        0        0        0 2023-11-22 03:20:49.000000 nyctibius-0.0.8/src/nyctibius/db/__init__.py
--rw-rw-rw-   0        0        0     5540 2024-01-16 21:39:25.000000 nyctibius-0.0.8/src/nyctibius/db/db_setup.py
--rw-rw-rw-   0        0        0    21140 2024-03-04 18:56:08.000000 nyctibius-0.0.8/src/nyctibius/db/modifier.py
--rw-rw-rw-   0        0        0     6353 2024-04-02 15:24:52.000000 nyctibius-0.0.8/src/nyctibius/db/querier.py
-drwxrwxrwx   0        0        0        0 2024-04-09 01:54:39.904011 nyctibius-0.0.8/src/nyctibius/dto/
--rw-rw-rw-   0        0        0        0 2023-11-22 03:20:49.000000 nyctibius-0.0.8/src/nyctibius/dto/__init__.py
--rw-rw-rw-   0        0        0     1755 2024-03-20 14:21:14.000000 nyctibius-0.0.8/src/nyctibius/dto/data_info.py
-drwxrwxrwx   0        0        0        0 2024-04-09 01:54:39.907010 nyctibius-0.0.8/src/nyctibius/enums/
--rw-rw-rw-   0        0        0        0 2023-11-22 03:20:49.000000 nyctibius-0.0.8/src/nyctibius/enums/__init__.py
--rw-rw-rw-   0        0        0       94 2024-02-06 00:16:29.000000 nyctibius-0.0.8/src/nyctibius/enums/config_enum.py
--rw-rw-rw-   0        0        0     4382 2023-11-22 03:20:49.000000 nyctibius-0.0.8/src/nyctibius/enums/headers_enum.py
-drwxrwxrwx   0        0        0        0 2024-04-09 01:54:39.911010 nyctibius-0.0.8/src/nyctibius/etl/
--rw-rw-rw-   0        0        0        0 2024-01-24 04:45:52.000000 nyctibius-0.0.8/src/nyctibius/etl/__init__.py
--rw-rw-rw-   0        0        0     6703 2024-03-20 14:21:14.000000 nyctibius-0.0.8/src/nyctibius/etl/extractor.py
--rw-rw-rw-   0        0        0     2051 2024-03-16 00:35:08.000000 nyctibius-0.0.8/src/nyctibius/etl/loader.py
--rw-rw-rw-   0        0        0     2354 2024-03-20 15:05:36.000000 nyctibius-0.0.8/src/nyctibius/etl/transformer.py
--rw-rw-rw-   0        0        0     3217 2024-03-20 14:21:14.000000 nyctibius-0.0.8/src/nyctibius/harmonizer.py
--rw-rw-rw-   0        0        0     3622 2024-02-22 17:24:14.000000 nyctibius-0.0.8/src/nyctibius/test_queries.py
-drwxrwxrwx   0        0        0        0 2024-04-09 01:54:39.916017 nyctibius-0.0.8/src/nyctibius/utils/
--rw-rw-rw-   0        0        0        0 2023-11-22 03:20:49.000000 nyctibius-0.0.8/src/nyctibius/utils/__init__.py
--rw-rw-rw-   0        0        0     1545 2024-03-04 18:55:35.000000 nyctibius-0.0.8/src/nyctibius/utils/censo_spider.py
--rw-rw-rw-   0        0        0     3582 2024-03-20 14:21:14.000000 nyctibius-0.0.8/src/nyctibius/utils/extractor_utils.py
--rw-rw-rw-   0        0        0     2462 2024-03-20 14:21:14.000000 nyctibius-0.0.8/src/nyctibius/utils/standard_spider.py
-drwxrwxrwx   0        0        0        0 2024-04-09 01:54:39.778001 nyctibius-0.0.8/src/nyctibius.egg-info/
--rw-rw-rw-   0        0        0     7950 2024-04-09 01:54:39.000000 nyctibius-0.0.8/src/nyctibius.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1022 2024-04-09 01:54:39.000000 nyctibius-0.0.8/src/nyctibius.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 01:54:39.000000 nyctibius-0.0.8/src/nyctibius.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2024-04-09 01:54:39.000000 nyctibius-0.0.8/src/nyctibius.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       84 2024-04-09 01:54:39.000000 nyctibius-0.0.8/src/nyctibius.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-09 01:54:39.000000 nyctibius-0.0.8/src/nyctibius.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-09 01:54:39.919007 nyctibius-0.0.8/tests/
--rw-rw-rw-   0        0        0        0 2024-01-17 00:26:41.000000 nyctibius-0.0.8/tests/test_extractor.py
--rw-rw-rw-   0        0        0        0 2024-01-17 00:26:41.000000 nyctibius-0.0.8/tests/test_loader.py
--rw-rw-rw-   0        0        0     1665 2024-01-17 00:26:41.000000 nyctibius-0.0.8/tests/test_transformer.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:12:44.084664 nyctibius-0.0.9/
+-rw-rw-rw-   0        0        0     7950 2024-04-09 02:12:44.083659 nyctibius-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     6692 2024-04-01 17:34:43.000000 nyctibius-0.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-09 02:12:44.084664 nyctibius-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     8586 2024-04-09 02:11:25.000000 nyctibius-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:12:44.040633 nyctibius-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2024-04-09 02:12:44.051632 nyctibius-0.0.9/src/nyctibius/
+-rw-rw-rw-   0        0        0       69 2024-04-09 01:07:48.000000 nyctibius-0.0.9/src/nyctibius/__init__.py
+-rw-rw-rw-   0        0        0     3290 2024-04-09 01:07:48.000000 nyctibius-0.0.9/src/nyctibius/__main__.py
+-rw-rw-rw-   0        0        0    10286 2024-04-09 02:03:42.000000 nyctibius-0.0.9/src/nyctibius/bird_agent.py
+-rw-rw-rw-   0        0        0        0 2023-11-22 03:20:49.000000 nyctibius-0.0.9/src/nyctibius/config.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:12:44.063655 nyctibius-0.0.9/src/nyctibius/db/
+-rw-rw-rw-   0        0        0        0 2023-11-22 03:20:49.000000 nyctibius-0.0.9/src/nyctibius/db/__init__.py
+-rw-rw-rw-   0        0        0     5540 2024-01-16 21:39:25.000000 nyctibius-0.0.9/src/nyctibius/db/db_setup.py
+-rw-rw-rw-   0        0        0    21140 2024-03-04 18:56:08.000000 nyctibius-0.0.9/src/nyctibius/db/modifier.py
+-rw-rw-rw-   0        0        0     6353 2024-04-02 15:24:52.000000 nyctibius-0.0.9/src/nyctibius/db/querier.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:12:44.065654 nyctibius-0.0.9/src/nyctibius/dto/
+-rw-rw-rw-   0        0        0        0 2023-11-22 03:20:49.000000 nyctibius-0.0.9/src/nyctibius/dto/__init__.py
+-rw-rw-rw-   0        0        0     1755 2024-03-20 14:21:14.000000 nyctibius-0.0.9/src/nyctibius/dto/data_info.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:12:44.068656 nyctibius-0.0.9/src/nyctibius/enums/
+-rw-rw-rw-   0        0        0        0 2023-11-22 03:20:49.000000 nyctibius-0.0.9/src/nyctibius/enums/__init__.py
+-rw-rw-rw-   0        0        0       94 2024-02-06 00:16:29.000000 nyctibius-0.0.9/src/nyctibius/enums/config_enum.py
+-rw-rw-rw-   0        0        0     4382 2023-11-22 03:20:49.000000 nyctibius-0.0.9/src/nyctibius/enums/headers_enum.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:12:44.072655 nyctibius-0.0.9/src/nyctibius/etl/
+-rw-rw-rw-   0        0        0        0 2024-01-24 04:45:52.000000 nyctibius-0.0.9/src/nyctibius/etl/__init__.py
+-rw-rw-rw-   0        0        0     6703 2024-03-20 14:21:14.000000 nyctibius-0.0.9/src/nyctibius/etl/extractor.py
+-rw-rw-rw-   0        0        0     2051 2024-03-16 00:35:08.000000 nyctibius-0.0.9/src/nyctibius/etl/loader.py
+-rw-rw-rw-   0        0        0     2354 2024-03-20 15:05:36.000000 nyctibius-0.0.9/src/nyctibius/etl/transformer.py
+-rw-rw-rw-   0        0        0     3217 2024-03-20 14:21:14.000000 nyctibius-0.0.9/src/nyctibius/harmonizer.py
+-rw-rw-rw-   0        0        0     3622 2024-02-22 17:24:14.000000 nyctibius-0.0.9/src/nyctibius/test_queries.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:12:44.078656 nyctibius-0.0.9/src/nyctibius/utils/
+-rw-rw-rw-   0        0        0        0 2023-11-22 03:20:49.000000 nyctibius-0.0.9/src/nyctibius/utils/__init__.py
+-rw-rw-rw-   0        0        0     1545 2024-03-04 18:55:35.000000 nyctibius-0.0.9/src/nyctibius/utils/censo_spider.py
+-rw-rw-rw-   0        0        0     3582 2024-03-20 14:21:14.000000 nyctibius-0.0.9/src/nyctibius/utils/extractor_utils.py
+-rw-rw-rw-   0        0        0     2462 2024-03-20 14:21:14.000000 nyctibius-0.0.9/src/nyctibius/utils/standard_spider.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:12:44.059671 nyctibius-0.0.9/src/nyctibius.egg-info/
+-rw-rw-rw-   0        0        0     7950 2024-04-09 02:12:43.000000 nyctibius-0.0.9/src/nyctibius.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1022 2024-04-09 02:12:43.000000 nyctibius-0.0.9/src/nyctibius.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 02:12:43.000000 nyctibius-0.0.9/src/nyctibius.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2024-04-09 02:12:43.000000 nyctibius-0.0.9/src/nyctibius.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      110 2024-04-09 02:12:43.000000 nyctibius-0.0.9/src/nyctibius.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-09 02:12:43.000000 nyctibius-0.0.9/src/nyctibius.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-09 02:12:44.081655 nyctibius-0.0.9/tests/
+-rw-rw-rw-   0        0        0        0 2024-01-17 00:26:41.000000 nyctibius-0.0.9/tests/test_extractor.py
+-rw-rw-rw-   0        0        0        0 2024-01-17 00:26:41.000000 nyctibius-0.0.9/tests/test_loader.py
+-rw-rw-rw-   0        0        0     1665 2024-01-17 00:26:41.000000 nyctibius-0.0.9/tests/test_transformer.py
```

### Comparing `nyctibius-0.0.8/PKG-INFO` & `nyctibius-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nyctibius
-Version: 0.0.8
+Version: 0.0.9
 Summary: Nyctibius is a Python package for gathering and consolidating socio-demographic data.
 Home-page: https://github.com/Ersebreck/Nyctibius
 Author: Erick Lozano, Diego Irreño y Cristian Amaya
 Author-email: 
 Project-URL: Bug Reports, https://github.com/Ersebreck/Nyctibius/issues
 Project-URL: Source, https://github.com/Ersebreck/Nyctibius/
 Keywords: extract transform load etl scraping relational census
```

### Comparing `nyctibius-0.0.8/README.md` & `nyctibius-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `nyctibius-0.0.8/setup.py` & `nyctibius-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='0.0.8',  # Required
+    version='0.0.9',  # Required
 
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description='Nyctibius is a Python package for gathering and consolidating socio-demographic data.',  # Optional
 
     # This is an optional longer description of your project that represents
@@ -132,15 +132,15 @@
 
     # This field lists other packages that your project depends on to run.
     # Any package you put here will be installed by pip when your project is
     # installed, so they must be valid existing projects.
     #
     # For an analysis of "install_requires" vs pip's requirements files see:
     # https://packaging.python.org/en/latest/requirements.html
-    install_requires=['pandas','requests','Scrapy','tqdm', 'pyreadstat', 'py7zr'],  # Optional
+    install_requires=['pandas','requests','Scrapy','tqdm', 'pyreadstat', 'py7zr', 'pandasai', 'matplotlib', 'numpy'],  # Optional
 
     # List additional groups of dependencies here (e.g. development
     # dependencies). Users will be able to install these using the "extras"
     # syntax, for example:
     #
     #   $ pip install sampleproject[dev]
     #
```

### Comparing `nyctibius-0.0.8/src/nyctibius/__main__.py` & `nyctibius-0.0.9/src/nyctibius/__main__.py`

 * *Files identical despite different names*

### Comparing `nyctibius-0.0.8/src/nyctibius/bird_agent.py` & `nyctibius-0.0.9/src/nyctibius/bird_agent.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,11 @@
-import re
 import pandas as pd
 import matplotlib.pyplot as plt
 import numpy as np
-import json
-import os
 from pandasai import Agent
-from pandasai import Agent
-import pandas as pd
 import os
 import json
 from .db.modifier import Modifier
 from pandasai.connectors import SqliteConnector, PandasConnector
 from pandasai.llm import OpenAI
 import warnings
 import logging
```

### Comparing `nyctibius-0.0.8/src/nyctibius/db/db_setup.py` & `nyctibius-0.0.9/src/nyctibius/db/db_setup.py`

 * *Files identical despite different names*

### Comparing `nyctibius-0.0.8/src/nyctibius/db/modifier.py` & `nyctibius-0.0.9/src/nyctibius/db/modifier.py`

 * *Files identical despite different names*

### Comparing `nyctibius-0.0.8/src/nyctibius/db/querier.py` & `nyctibius-0.0.9/src/nyctibius/db/querier.py`

 * *Files identical despite different names*

### Comparing `nyctibius-0.0.8/src/nyctibius/dto/data_info.py` & `nyctibius-0.0.9/src/nyctibius/dto/data_info.py`

 * *Files identical despite different names*

### Comparing `nyctibius-0.0.8/src/nyctibius/enums/headers_enum.py` & `nyctibius-0.0.9/src/nyctibius/enums/headers_enum.py`

 * *Files identical despite different names*

### Comparing `nyctibius-0.0.8/src/nyctibius/etl/extractor.py` & `nyctibius-0.0.9/src/nyctibius/etl/extractor.py`

 * *Files identical despite different names*

### Comparing `nyctibius-0.0.8/src/nyctibius/etl/loader.py` & `nyctibius-0.0.9/src/nyctibius/etl/loader.py`

 * *Files identical despite different names*

### Comparing `nyctibius-0.0.8/src/nyctibius/etl/transformer.py` & `nyctibius-0.0.9/src/nyctibius/etl/transformer.py`

 * *Files identical despite different names*

### Comparing `nyctibius-0.0.8/src/nyctibius/harmonizer.py` & `nyctibius-0.0.9/src/nyctibius/harmonizer.py`

 * *Files identical despite different names*

### Comparing `nyctibius-0.0.8/src/nyctibius/test_queries.py` & `nyctibius-0.0.9/src/nyctibius/test_queries.py`

 * *Files identical despite different names*

### Comparing `nyctibius-0.0.8/src/nyctibius/utils/censo_spider.py` & `nyctibius-0.0.9/src/nyctibius/utils/censo_spider.py`

 * *Files identical despite different names*

### Comparing `nyctibius-0.0.8/src/nyctibius/utils/extractor_utils.py` & `nyctibius-0.0.9/src/nyctibius/utils/extractor_utils.py`

 * *Files identical despite different names*

### Comparing `nyctibius-0.0.8/src/nyctibius/utils/standard_spider.py` & `nyctibius-0.0.9/src/nyctibius/utils/standard_spider.py`

 * *Files identical despite different names*

### Comparing `nyctibius-0.0.8/src/nyctibius.egg-info/PKG-INFO` & `nyctibius-0.0.9/src/nyctibius.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nyctibius
-Version: 0.0.8
+Version: 0.0.9
 Summary: Nyctibius is a Python package for gathering and consolidating socio-demographic data.
 Home-page: https://github.com/Ersebreck/Nyctibius
 Author: Erick Lozano, Diego Irreño y Cristian Amaya
 Author-email: 
 Project-URL: Bug Reports, https://github.com/Ersebreck/Nyctibius/issues
 Project-URL: Source, https://github.com/Ersebreck/Nyctibius/
 Keywords: extract transform load etl scraping relational census
```

### Comparing `nyctibius-0.0.8/src/nyctibius.egg-info/SOURCES.txt` & `nyctibius-0.0.9/src/nyctibius.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nyctibius-0.0.8/tests/test_transformer.py` & `nyctibius-0.0.9/tests/test_transformer.py`

 * *Files identical despite different names*

