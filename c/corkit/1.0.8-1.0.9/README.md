# Comparing `tmp/corkit-1.0.8.tar.gz` & `tmp/corkit-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corkit-1.0.8.tar", last modified: Mon Apr 15 01:21:49 2024, max compression
+gzip compressed data, was "corkit-1.0.9.tar", last modified: Mon Apr 15 01:57:38 2024, max compression
```

## Comparing `corkit-1.0.8.tar` & `corkit-1.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 jenci     (1000) jenci     (1000)        0 2024-04-15 01:21:49.569021 corkit-1.0.8/
--rw-rw-r--   0 jenci     (1000) jenci     (1000)     1078 2024-04-14 19:27:35.000000 corkit-1.0.8/LICENSE
--rw-rw-r--   0 jenci     (1000) jenci     (1000)     2876 2024-04-15 01:21:49.569021 corkit-1.0.8/PKG-INFO
--rw-rw-r--   0 jenci     (1000) jenci     (1000)     2583 2024-04-15 01:18:04.000000 corkit-1.0.8/README.md
-drwxrwxr-x   0 jenci     (1000) jenci     (1000)        0 2024-04-15 01:21:49.569021 corkit-1.0.8/corkit/
--rw-rw-r--   0 jenci     (1000) jenci     (1000)      146 2024-04-15 00:50:20.000000 corkit-1.0.8/corkit/__init__.py
--rw-rw-r--   0 jenci     (1000) jenci     (1000)     6854 2024-04-15 00:50:19.000000 corkit-1.0.8/corkit/dataset.py
--rw-rw-r--   0 jenci     (1000) jenci     (1000)    18207 2024-04-15 01:00:44.000000 corkit-1.0.8/corkit/lasco.py
--rw-rw-r--   0 jenci     (1000) jenci     (1000)     8006 2024-04-15 00:50:17.000000 corkit-1.0.8/corkit/reconstruction.py
--rw-rw-r--   0 jenci     (1000) jenci     (1000)       98 2024-04-15 00:50:16.000000 corkit-1.0.8/corkit/secchi.py
--rw-rw-r--   0 jenci     (1000) jenci     (1000)    42201 2024-04-15 01:17:23.000000 corkit-1.0.8/corkit/utils.py
-drwxrwxr-x   0 jenci     (1000) jenci     (1000)        0 2024-04-15 01:21:49.569021 corkit-1.0.8/corkit.egg-info/
--rw-rw-r--   0 jenci     (1000) jenci     (1000)     2876 2024-04-15 01:21:49.000000 corkit-1.0.8/corkit.egg-info/PKG-INFO
--rw-rw-r--   0 jenci     (1000) jenci     (1000)      286 2024-04-15 01:21:49.000000 corkit-1.0.8/corkit.egg-info/SOURCES.txt
--rw-rw-r--   0 jenci     (1000) jenci     (1000)        1 2024-04-15 01:21:49.000000 corkit-1.0.8/corkit.egg-info/dependency_links.txt
--rw-rw-r--   0 jenci     (1000) jenci     (1000)       82 2024-04-15 01:21:49.000000 corkit-1.0.8/corkit.egg-info/requires.txt
--rw-rw-r--   0 jenci     (1000) jenci     (1000)        7 2024-04-15 01:21:49.000000 corkit-1.0.8/corkit.egg-info/top_level.txt
--rw-rw-r--   0 jenci     (1000) jenci     (1000)       38 2024-04-15 01:21:49.569021 corkit-1.0.8/setup.cfg
--rw-rw-r--   0 jenci     (1000) jenci     (1000)     1485 2024-04-15 01:17:57.000000 corkit-1.0.8/setup.py
+drwxrwxr-x   0 jenci     (1000) jenci     (1000)        0 2024-04-15 01:57:38.796327 corkit-1.0.9/
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)     1078 2024-04-15 01:44:25.000000 corkit-1.0.9/LICENSE
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)     4552 2024-04-15 01:57:38.796327 corkit-1.0.9/PKG-INFO
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)     2583 2024-04-15 01:44:24.000000 corkit-1.0.9/README.md
+drwxrwxr-x   0 jenci     (1000) jenci     (1000)        0 2024-04-15 01:57:38.792327 corkit-1.0.9/corkit/
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)      146 2024-04-15 00:50:20.000000 corkit-1.0.9/corkit/__init__.py
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)     6854 2024-04-15 01:43:38.000000 corkit-1.0.9/corkit/dataset.py
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)    18207 2024-04-15 01:44:32.000000 corkit-1.0.9/corkit/lasco.py
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)     8006 2024-04-15 01:43:37.000000 corkit-1.0.9/corkit/reconstruction.py
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)       98 2024-04-15 01:43:37.000000 corkit-1.0.9/corkit/secchi.py
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)    42201 2024-04-15 01:44:31.000000 corkit-1.0.9/corkit/utils.py
+drwxrwxr-x   0 jenci     (1000) jenci     (1000)        0 2024-04-15 01:57:38.796327 corkit-1.0.9/corkit.egg-info/
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)     4552 2024-04-15 01:57:38.000000 corkit-1.0.9/corkit.egg-info/PKG-INFO
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)      286 2024-04-15 01:57:38.000000 corkit-1.0.9/corkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)        1 2024-04-15 01:57:38.000000 corkit-1.0.9/corkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)       82 2024-04-15 01:57:38.000000 corkit-1.0.9/corkit.egg-info/requires.txt
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)        7 2024-04-15 01:57:38.000000 corkit-1.0.9/corkit.egg-info/top_level.txt
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)       38 2024-04-15 01:57:38.796327 corkit-1.0.9/setup.cfg
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)     3368 2024-04-15 01:57:37.000000 corkit-1.0.9/setup.py
```

### Comparing `corkit-1.0.8/LICENSE` & `corkit-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `corkit-1.0.8/PKG-INFO` & `corkit-1.0.9/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: corkit
-Version: 1.0.8
-Summary: Open source coronagraph data downloader and calibrator
-Home-page: https://github.com/Jorgedavyd/corkit
-Author: Jorge David Enciso Martínez
-Author-email: jorged.encyso@gmail.com
-License: MIT
-Platform: UNKNOWN
-License-File: LICENSE
-
 [![pypi](https://img.shields.io/pypi/v/corkit)](https://pypi.org/project/corkit)
 ![status](https://img.shields.io/badge/status-beta-red.svg)
 [![license](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 # CorKit: Coronagraph Science Kit
 
 [![logo](https://github.com/Jorgedavyd/corkit/blob/main/docs/source/logo.png)](https://pypi.org/project/corkit)
@@ -51,9 +40,8 @@
 <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/d/db/Stereo_logo.gif/1200px-Stereo_logo.gif" width="200" height="200" />
 <img src="https://lh6.googleusercontent.com/proxy/1sXRF-9df_jeWpUWlyDqUn4ddQ34PIis-2zBpOf46TeKkQPJdNVbLL_ciXXUaS-AZR0Z4tBFqaYSdIZJwuKnhNtIy2pFekckiA" width="200" height="200" />
 
 ## Contact  
 
 - [Linkedin](https://www.linkedin.com/in/jorge-david-enciso-mart%C3%ADnez-149977265/)
 - [Email](jorged.encyso@gmail.com)
-- [GitHub](https://github.com/Jorgedavyd)
-
+- [GitHub](https://github.com/Jorgedavyd)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `corkit-1.0.8/corkit/dataset.py` & `corkit-1.0.9/corkit/dataset.py`

 * *Files identical despite different names*

### Comparing `corkit-1.0.8/corkit/lasco.py` & `corkit-1.0.9/corkit/lasco.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import numpy as np
 import aiofiles
 import aiohttp
 import asyncio
 import os
 import glob
 
-version = '1.0.7'
+version = '1.0.9'
 
 #done
 def level_1(
         fits_file: Union[str, BytesIO],
         target_path: str,
         **kwargs
 ) -> None:
```

### Comparing `corkit-1.0.8/corkit/reconstruction.py` & `corkit-1.0.9/corkit/reconstruction.py`

 * *Files identical despite different names*

### Comparing `corkit-1.0.8/corkit/utils.py` & `corkit-1.0.9/corkit/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from matplotlib import tri
 from PIL import Image
 import pandas as pd
 import numpy as np 
 import glob
 import os
 
-version = '1.0.8'
+version = '1.0.9'
 
 radeg = 180/np.pi
 
 DEFAULT_SAVE_DIR = os.path.join(os.path.dirname(__file__),'data')
 
 #done
 def datetime_interval(init: datetime, last: datetime, step_size: timedelta, output_format: str = '%Y%m%d'):
```

