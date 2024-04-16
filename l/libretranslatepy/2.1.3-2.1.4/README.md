# Comparing `tmp/libretranslatepy-2.1.3.tar.gz` & `tmp/libretranslatepy-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libretranslatepy-2.1.3.tar", last modified: Sat Oct 15 12:21:49 2022, max compression
+gzip compressed data, was "libretranslatepy-2.1.4.tar", last modified: Tue Apr 16 21:47:47 2024, max compression
```

## Comparing `libretranslatepy-2.1.3.tar` & `libretranslatepy-2.1.4.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxr-x   0 argosopentech  (1001) argosopentech  (1003)        0 2022-10-15 12:21:49.162945 libretranslatepy-2.1.3/
--rw-rw-r--   0 argosopentech  (1001) argosopentech  (1003)      774 2022-10-15 12:21:49.154945 libretranslatepy-2.1.3/PKG-INFO
--rw-rw-r--   0 argosopentech  (1001) argosopentech  (1003)     4049 2022-10-15 12:20:36.000000 libretranslatepy-2.1.3/README.md
-drwxrwxr-x   0 argosopentech  (1001) argosopentech  (1003)        0 2022-10-15 12:21:49.154945 libretranslatepy-2.1.3/libretranslatepy/
--rw-rw-r--   0 argosopentech  (1001) argosopentech  (1003)       35 2022-04-30 11:37:17.000000 libretranslatepy-2.1.3/libretranslatepy/__init__.py
--rw-rw-r--   0 argosopentech  (1001) argosopentech  (1003)     3003 2022-10-15 12:20:36.000000 libretranslatepy-2.1.3/libretranslatepy/api.py
-drwxrwxr-x   0 argosopentech  (1001) argosopentech  (1003)        0 2022-10-15 12:21:49.154945 libretranslatepy-2.1.3/libretranslatepy.egg-info/
--rw-rw-r--   0 argosopentech  (1001) argosopentech  (1003)      774 2022-10-15 12:21:48.000000 libretranslatepy-2.1.3/libretranslatepy.egg-info/PKG-INFO
--rw-rw-r--   0 argosopentech  (1001) argosopentech  (1003)      231 2022-10-15 12:21:49.000000 libretranslatepy-2.1.3/libretranslatepy.egg-info/SOURCES.txt
--rw-rw-r--   0 argosopentech  (1001) argosopentech  (1003)        1 2022-10-15 12:21:48.000000 libretranslatepy-2.1.3/libretranslatepy.egg-info/dependency_links.txt
--rw-rw-r--   0 argosopentech  (1001) argosopentech  (1003)       17 2022-10-15 12:21:48.000000 libretranslatepy-2.1.3/libretranslatepy.egg-info/top_level.txt
--rw-rw-r--   0 argosopentech  (1001) argosopentech  (1003)       38 2022-10-15 12:21:49.162945 libretranslatepy-2.1.3/setup.cfg
--rw-rw-r--   0 argosopentech  (1001) argosopentech  (1003)      877 2022-10-15 12:21:08.000000 libretranslatepy-2.1.3/setup.py
+drwxrwxr-x   0 pj        (1000) pj        (1000)        0 2024-04-16 21:47:47.534662 libretranslatepy-2.1.4/
+-rw-rw-r--   0 pj        (1000) pj        (1000)     1072 2024-04-16 21:47:04.000000 libretranslatepy-2.1.4/LICENSE
+-rw-rw-r--   0 pj        (1000) pj        (1000)      785 2024-04-16 21:47:47.534662 libretranslatepy-2.1.4/PKG-INFO
+-rw-rw-r--   0 pj        (1000) pj        (1000)     4354 2024-04-16 21:47:04.000000 libretranslatepy-2.1.4/README.md
+drwxrwxr-x   0 pj        (1000) pj        (1000)        0 2024-04-16 21:47:47.530662 libretranslatepy-2.1.4/libretranslatepy/
+-rw-rw-r--   0 pj        (1000) pj        (1000)       35 2024-04-16 21:47:04.000000 libretranslatepy-2.1.4/libretranslatepy/__init__.py
+-rw-rw-r--   0 pj        (1000) pj        (1000)     3463 2024-04-16 21:47:04.000000 libretranslatepy-2.1.4/libretranslatepy/api.py
+drwxrwxr-x   0 pj        (1000) pj        (1000)        0 2024-04-16 21:47:47.530662 libretranslatepy-2.1.4/libretranslatepy.egg-info/
+-rw-rw-r--   0 pj        (1000) pj        (1000)      785 2024-04-16 21:47:47.000000 libretranslatepy-2.1.4/libretranslatepy.egg-info/PKG-INFO
+-rw-rw-r--   0 pj        (1000) pj        (1000)      239 2024-04-16 21:47:47.000000 libretranslatepy-2.1.4/libretranslatepy.egg-info/SOURCES.txt
+-rw-rw-r--   0 pj        (1000) pj        (1000)        1 2024-04-16 21:47:47.000000 libretranslatepy-2.1.4/libretranslatepy.egg-info/dependency_links.txt
+-rw-rw-r--   0 pj        (1000) pj        (1000)       17 2024-04-16 21:47:47.000000 libretranslatepy-2.1.4/libretranslatepy.egg-info/top_level.txt
+-rw-rw-r--   0 pj        (1000) pj        (1000)       38 2024-04-16 21:47:47.534662 libretranslatepy-2.1.4/setup.cfg
+-rw-rw-r--   0 pj        (1000) pj        (1000)      877 2024-04-16 21:47:41.000000 libretranslatepy-2.1.4/setup.py
```

### Comparing `libretranslatepy-2.1.3/PKG-INFO` & `libretranslatepy-2.1.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,21 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: libretranslatepy
-Version: 2.1.3
+Version: 2.1.4
 Summary: Python bindings for LibreTranslate API
 Home-page: https://github.com/argosopentech/LibreTranslate-py
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/argosopentech/LibreTranslate-py/issues
 Project-URL: Source, https://github.com/argosopentech/LibreTranslate-py/
-Description: UNKNOWN
 Keywords: translation libretranslate
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=2.6
+License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `libretranslatepy-2.1.3/README.md` & `libretranslatepy-2.1.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,53 +1,56 @@
 # LibreTranslate-py
 
 <a href="https://pypi.org/project/libretranslatepy/" target="_blank"><img src="https://flat.badgen.net/pypi/v/libretranslatepy"></a>
 <a href="/LICENSE" target="_blank"><img src="https://flat.badgen.net/github/license/argosopentech/LibreTranslate-py"></a>
 
-Python bindings for [LibreTranslate](https://github.com/LibreTranslate/LibreTranslate)
+Python bindings to connect to a [LibreTranslate API](https://github.com/LibreTranslate/LibreTranslate)
 
 
 ## Install
 ```
 pip install libretranslatepy
 ```
 
 ## Example usage
 ```python
 from libretranslatepy import LibreTranslateAPI
 
-lt = LibreTranslateAPI("https://translate.argosopentech.com/")
+lt = LibreTranslateAPI("https://translate.terraprint.co/")
 
 print(lt.translate("LibreTranslate is awesome!", "en", "es"))
 # LibreTranslate es impresionante!
 
 print(lt.detect("Hello World"))
 # [{"confidence": 0.6, "language": "en"}]
 
 print(lt.languages())
 # [{"code":"en", "name":"English"}]
 ```
 
 ## [LibreTranslate Mirrors](https://github.com/LibreTranslate/LibreTranslate#mirrors)
-- [translate.argosopentech.com](https://translate.argosopentech.com)
+- [translate.terraprint.co](https://translate.terraprint.co)
+*translate.argosopentech.com is no longer active*
+
+If you [buy a LibreTranslate API key](https://portal.libretranslate.com/) from the [LibreTranslate project](https://libretranslate.com) you get access to a fast cloud hosted service, email support, and financially support the LibreTranslate devs ❤️.
 
 ## Source
 ```python
 import json
 import sys
 from urllib import request, parse
 
 
 class LibreTranslateAPI:
     """Connect to the LibreTranslate API"""
 
     """Example usage:
     from libretranslatepy import LibreTranslateAPI
 
-    lt = LibreTranslateAPI("https://translate.argosopentech.com/")
+    lt = LibreTranslateAPI("https://translate.terraprint.co/")
 
     print(lt.translate("LibreTranslate is awesome!", "en", "es"))
     # LibreTranslate es impresionante!
 
     print(lt.detect("Hello World"))
     # [{"confidence": 0.6, "language": "en"}]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `libretranslatepy-2.1.3/libretranslatepy.egg-info/PKG-INFO` & `libretranslatepy-2.1.4/libretranslatepy.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,21 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: libretranslatepy
-Version: 2.1.3
+Version: 2.1.4
 Summary: Python bindings for LibreTranslate API
 Home-page: https://github.com/argosopentech/LibreTranslate-py
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/argosopentech/LibreTranslate-py/issues
 Project-URL: Source, https://github.com/argosopentech/LibreTranslate-py/
-Description: UNKNOWN
 Keywords: translation libretranslate
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=2.6
+License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `libretranslatepy-2.1.3/setup.py` & `libretranslatepy-2.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import find_packages, setup
 
 setup(name='libretranslatepy',
-      version='2.1.3',
+      version='2.1.4',
       description='Python bindings for LibreTranslate API',
       keywords="translation libretranslate",
       url='https://github.com/argosopentech/LibreTranslate-py',
       python_requires=">=2.6",
       classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator",
```

