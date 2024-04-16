# Comparing `tmp/thepipe_api-0.1.8.tar.gz` & `tmp/thepipe_api-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thepipe_api-0.1.8.tar", last modified: Mon Apr 15 23:07:30 2024, max compression
+gzip compressed data, was "thepipe_api-0.1.9.tar", last modified: Mon Apr 15 23:17:18 2024, max compression
```

## Comparing `thepipe_api-0.1.8.tar` & `thepipe_api-0.1.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 23:07:30.469329 thepipe_api-0.1.8/
--rw-rw-rw-   0        0        0     1094 2024-03-27 18:15:40.000000 thepipe_api-0.1.8/LICENSE
--rw-rw-rw-   0        0        0     9671 2024-04-15 23:07:30.468328 thepipe_api-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     8943 2024-04-15 22:58:42.000000 thepipe_api-0.1.8/README.md
--rw-rw-rw-   0        0        0       42 2024-04-15 23:07:30.469329 thepipe_api-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      859 2024-04-15 23:07:13.000000 thepipe_api-0.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-15 23:07:30.447328 thepipe_api-0.1.8/tests/
--rw-rw-rw-   0        0        0        0 2024-03-23 01:45:32.000000 thepipe_api-0.1.8/tests/__init__.py
--rw-rw-rw-   0        0        0     9523 2024-04-13 23:06:00.000000 thepipe_api-0.1.8/tests/test_thepipe.py
-drwxrwxrwx   0        0        0        0 2024-04-15 23:07:30.452327 thepipe_api-0.1.8/thepipe_api/
--rw-rw-rw-   0        0        0       86 2024-04-15 22:46:19.000000 thepipe_api-0.1.8/thepipe_api/__init__.py
--rw-rw-rw-   0        0        0     4821 2024-04-13 20:40:22.000000 thepipe_api-0.1.8/thepipe_api/compressor.py
--rw-rw-rw-   0        0        0     2789 2024-04-15 23:00:33.000000 thepipe_api-0.1.8/thepipe_api/core.py
--rw-rw-rw-   0        0        0    19810 2024-04-15 22:43:34.000000 thepipe_api-0.1.8/thepipe_api/extractor.py
--rw-rw-rw-   0        0        0     3606 2024-04-15 23:06:13.000000 thepipe_api-0.1.8/thepipe_api/thepipe.py
-drwxrwxrwx   0        0        0        0 2024-04-15 23:07:30.467328 thepipe_api-0.1.8/thepipe_api.egg-info/
--rw-rw-rw-   0        0        0     9671 2024-04-15 23:07:30.000000 thepipe_api-0.1.8/thepipe_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      396 2024-04-15 23:07:30.000000 thepipe_api-0.1.8/thepipe_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 23:07:30.000000 thepipe_api-0.1.8/thepipe_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2024-04-15 23:07:30.000000 thepipe_api-0.1.8/thepipe_api.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      105 2024-04-15 23:07:30.000000 thepipe_api-0.1.8/thepipe_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-15 23:07:30.000000 thepipe_api-0.1.8/thepipe_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-15 23:17:18.091697 thepipe_api-0.1.9/
+-rw-rw-rw-   0        0        0     1094 2024-03-27 18:15:40.000000 thepipe_api-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0     9671 2024-04-15 23:17:18.090696 thepipe_api-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     8943 2024-04-15 22:58:42.000000 thepipe_api-0.1.9/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-15 23:17:18.091697 thepipe_api-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      859 2024-04-15 23:16:36.000000 thepipe_api-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 23:17:18.068698 thepipe_api-0.1.9/tests/
+-rw-rw-rw-   0        0        0        0 2024-03-23 01:45:32.000000 thepipe_api-0.1.9/tests/__init__.py
+-rw-rw-rw-   0        0        0     9523 2024-04-13 23:06:00.000000 thepipe_api-0.1.9/tests/test_thepipe.py
+drwxrwxrwx   0        0        0        0 2024-04-15 23:17:18.073696 thepipe_api-0.1.9/thepipe_api/
+-rw-rw-rw-   0        0        0       86 2024-04-15 22:46:19.000000 thepipe_api-0.1.9/thepipe_api/__init__.py
+-rw-rw-rw-   0        0        0     4821 2024-04-13 20:40:22.000000 thepipe_api-0.1.9/thepipe_api/compressor.py
+-rw-rw-rw-   0        0        0     2789 2024-04-15 23:00:33.000000 thepipe_api-0.1.9/thepipe_api/core.py
+-rw-rw-rw-   0        0        0    19810 2024-04-15 22:43:34.000000 thepipe_api-0.1.9/thepipe_api/extractor.py
+-rw-rw-rw-   0        0        0     3689 2024-04-15 23:15:24.000000 thepipe_api-0.1.9/thepipe_api/thepipe.py
+drwxrwxrwx   0        0        0        0 2024-04-15 23:17:18.089697 thepipe_api-0.1.9/thepipe_api.egg-info/
+-rw-rw-rw-   0        0        0     9671 2024-04-15 23:17:17.000000 thepipe_api-0.1.9/thepipe_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      396 2024-04-15 23:17:17.000000 thepipe_api-0.1.9/thepipe_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 23:17:17.000000 thepipe_api-0.1.9/thepipe_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2024-04-15 23:17:17.000000 thepipe_api-0.1.9/thepipe_api.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      105 2024-04-15 23:17:17.000000 thepipe_api-0.1.9/thepipe_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-15 23:17:17.000000 thepipe_api-0.1.9/thepipe_api.egg-info/top_level.txt
```

### Comparing `thepipe_api-0.1.8/LICENSE` & `thepipe_api-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `thepipe_api-0.1.8/PKG-INFO` & `thepipe_api-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thepipe_api
-Version: 0.1.8
+Version: 0.1.9
 Summary: Automate information extraction for multimodal LLMs.
 Home-page: https://github.com/emcf/thepipe
 Author: Emmett McFarlane
 Author-email: emmett@thepi.pe
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: thepipe_api Version: 0.1.8 Summary: Automate
+Metadata-Version: 2.1 Name: thepipe_api Version: 0.1.9 Summary: Automate
 information extraction for multimodal LLMs. Home-page: https://github.com/emcf/
 thepipe Author: Emmett McFarlane Author-email: emmett@thepi.pe Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 aiohttp Requires-Dist: charset-normalizer Requires-Dist: Pyarrow Requires-Dist:
 python-magic Requires-Dist: colorama Requires-Dist: requests Requires-Dist:
```

### Comparing `thepipe_api-0.1.8/README.md` & `thepipe_api-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `thepipe_api-0.1.8/setup.py` & `thepipe_api-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='thepipe_api',
-    version='0.1.8',
+    version='0.1.9',
     author='Emmett McFarlane',
     author_email='emmett@thepi.pe',
     description='Automate information extraction for multimodal LLMs.',
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/emcf/thepipe',
     packages=find_packages(),
```

### Comparing `thepipe_api-0.1.8/tests/test_thepipe.py` & `thepipe_api-0.1.9/tests/test_thepipe.py`

 * *Files identical despite different names*

### Comparing `thepipe_api-0.1.8/thepipe_api/compressor.py` & `thepipe_api-0.1.9/thepipe_api/compressor.py`

 * *Files identical despite different names*

### Comparing `thepipe_api-0.1.8/thepipe_api/core.py` & `thepipe_api-0.1.9/thepipe_api/core.py`

 * *Files identical despite different names*

### Comparing `thepipe_api-0.1.8/thepipe_api/extractor.py` & `thepipe_api-0.1.9/thepipe_api/extractor.py`

 * *Files identical despite different names*

### Comparing `thepipe_api-0.1.8/thepipe_api/thepipe.py` & `thepipe_api-0.1.9/thepipe_api/thepipe.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,11 +52,13 @@
     verbose = not args.quiet
     args.verbose = verbose
     return args
 
 def main() -> None:
     args = parse_arguments()
     chunks = extract(source=args.source, match=args.match, ignore=args.ignore, limit=args.limit, verbose=args.verbose, ai_extraction=args.ai_extraction, text_only=args.text_only, local=args.local)
+    if not args.local:
+        chunks = core.create_chunks_from_messages(chunks)
     save_outputs(chunks=chunks, verbose=args.verbose, text_only=args.text_only)
 
 if __name__ == '__main__':
     main()
```

### Comparing `thepipe_api-0.1.8/thepipe_api.egg-info/PKG-INFO` & `thepipe_api-0.1.9/thepipe_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thepipe_api
-Version: 0.1.8
+Version: 0.1.9
 Summary: Automate information extraction for multimodal LLMs.
 Home-page: https://github.com/emcf/thepipe
 Author: Emmett McFarlane
 Author-email: emmett@thepi.pe
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: thepipe_api Version: 0.1.8 Summary: Automate
+Metadata-Version: 2.1 Name: thepipe_api Version: 0.1.9 Summary: Automate
 information extraction for multimodal LLMs. Home-page: https://github.com/emcf/
 thepipe Author: Emmett McFarlane Author-email: emmett@thepi.pe Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 aiohttp Requires-Dist: charset-normalizer Requires-Dist: Pyarrow Requires-Dist:
 python-magic Requires-Dist: colorama Requires-Dist: requests Requires-Dist:
```

