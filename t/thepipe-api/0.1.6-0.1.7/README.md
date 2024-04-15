# Comparing `tmp/thepipe_api-0.1.6.tar.gz` & `tmp/thepipe_api-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thepipe_api-0.1.6.tar", last modified: Sun Apr 14 21:15:59 2024, max compression
+gzip compressed data, was "thepipe_api-0.1.7.tar", last modified: Mon Apr 15 22:52:06 2024, max compression
```

## Comparing `thepipe_api-0.1.6.tar` & `thepipe_api-0.1.7.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-14 21:15:59.058338 thepipe_api-0.1.6/
--rw-rw-rw-   0        0        0     1094 2024-03-27 18:15:40.000000 thepipe_api-0.1.6/LICENSE
--rw-rw-rw-   0        0        0     9416 2024-04-14 21:15:59.057339 thepipe_api-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     8688 2024-04-14 00:39:19.000000 thepipe_api-0.1.6/README.md
--rw-rw-rw-   0        0        0       42 2024-04-14 21:15:59.058338 thepipe_api-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      740 2024-04-14 21:15:32.000000 thepipe_api-0.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-14 21:15:59.029341 thepipe_api-0.1.6/tests/
--rw-rw-rw-   0        0        0        0 2024-03-23 01:45:32.000000 thepipe_api-0.1.6/tests/__init__.py
--rw-rw-rw-   0        0        0     9523 2024-04-13 23:06:00.000000 thepipe_api-0.1.6/tests/test_thepipe.py
-drwxrwxrwx   0        0        0        0 2024-04-14 21:15:59.033340 thepipe_api-0.1.6/thepipe_api/
--rw-rw-rw-   0        0        0       48 2024-04-13 19:44:21.000000 thepipe_api-0.1.6/thepipe_api/__init__.py
--rw-rw-rw-   0        0        0     4821 2024-04-13 20:40:22.000000 thepipe_api-0.1.6/thepipe_api/compressor.py
--rw-rw-rw-   0        0        0     2849 2024-04-14 20:41:11.000000 thepipe_api-0.1.6/thepipe_api/core.py
--rw-rw-rw-   0        0        0    19797 2024-04-14 00:54:40.000000 thepipe_api-0.1.6/thepipe_api/extractor.py
--rw-rw-rw-   0        0        0     3504 2024-04-13 20:43:49.000000 thepipe_api-0.1.6/thepipe_api/thepipe.py
-drwxrwxrwx   0        0        0        0 2024-04-14 21:15:59.056340 thepipe_api-0.1.6/thepipe_api.egg-info/
--rw-rw-rw-   0        0        0     9416 2024-04-14 21:15:58.000000 thepipe_api-0.1.6/thepipe_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      358 2024-04-14 21:15:58.000000 thepipe_api-0.1.6/thepipe_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-14 21:15:58.000000 thepipe_api-0.1.6/thepipe_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      105 2024-04-14 21:15:58.000000 thepipe_api-0.1.6/thepipe_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-14 21:15:58.000000 thepipe_api-0.1.6/thepipe_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-15 22:52:06.262720 thepipe_api-0.1.7/
+-rw-rw-rw-   0        0        0     1094 2024-03-27 18:15:40.000000 thepipe_api-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0     9416 2024-04-15 22:52:06.261721 thepipe_api-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     8688 2024-04-14 00:39:19.000000 thepipe_api-0.1.7/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-15 22:52:06.262720 thepipe_api-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      859 2024-04-15 22:51:37.000000 thepipe_api-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 22:52:06.239718 thepipe_api-0.1.7/tests/
+-rw-rw-rw-   0        0        0        0 2024-03-23 01:45:32.000000 thepipe_api-0.1.7/tests/__init__.py
+-rw-rw-rw-   0        0        0     9523 2024-04-13 23:06:00.000000 thepipe_api-0.1.7/tests/test_thepipe.py
+drwxrwxrwx   0        0        0        0 2024-04-15 22:52:06.243719 thepipe_api-0.1.7/thepipe_api/
+-rw-rw-rw-   0        0        0       86 2024-04-15 22:46:19.000000 thepipe_api-0.1.7/thepipe_api/__init__.py
+-rw-rw-rw-   0        0        0     4821 2024-04-13 20:40:22.000000 thepipe_api-0.1.7/thepipe_api/compressor.py
+-rw-rw-rw-   0        0        0     2767 2024-04-15 06:49:44.000000 thepipe_api-0.1.7/thepipe_api/core.py
+-rw-rw-rw-   0        0        0    19810 2024-04-15 22:43:34.000000 thepipe_api-0.1.7/thepipe_api/extractor.py
+-rw-rw-rw-   0        0        0     3504 2024-04-13 20:43:49.000000 thepipe_api-0.1.7/thepipe_api/thepipe.py
+drwxrwxrwx   0        0        0        0 2024-04-15 22:52:06.259719 thepipe_api-0.1.7/thepipe_api.egg-info/
+-rw-rw-rw-   0        0        0     9416 2024-04-15 22:52:05.000000 thepipe_api-0.1.7/thepipe_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      396 2024-04-15 22:52:06.000000 thepipe_api-0.1.7/thepipe_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 22:52:05.000000 thepipe_api-0.1.7/thepipe_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2024-04-15 22:52:06.000000 thepipe_api-0.1.7/thepipe_api.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      105 2024-04-15 22:52:06.000000 thepipe_api-0.1.7/thepipe_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-15 22:52:06.000000 thepipe_api-0.1.7/thepipe_api.egg-info/top_level.txt
```

### Comparing `thepipe_api-0.1.6/LICENSE` & `thepipe_api-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `thepipe_api-0.1.6/PKG-INFO` & `thepipe_api-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thepipe_api
-Version: 0.1.6
+Version: 0.1.7
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
-Metadata-Version: 2.1 Name: thepipe_api Version: 0.1.6 Summary: Automate
+Metadata-Version: 2.1 Name: thepipe_api Version: 0.1.7 Summary: Automate
 information extraction for multimodal LLMs. Home-page: https://github.com/emcf/
 thepipe Author: Emmett McFarlane Author-email: emmett@thepi.pe Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 aiohttp Requires-Dist: charset-normalizer Requires-Dist: Pyarrow Requires-Dist:
 python-magic Requires-Dist: colorama Requires-Dist: requests Requires-Dist:
```

### Comparing `thepipe_api-0.1.6/README.md` & `thepipe_api-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `thepipe_api-0.1.6/setup.py` & `thepipe_api-0.1.7/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 from setuptools import setup, find_packages
 
 setup(
     name='thepipe_api',
-    version='0.1.6',
+    version='0.1.7',
     author='Emmett McFarlane',
     author_email='emmett@thepi.pe',
     description='Automate information extraction for multimodal LLMs.',
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/emcf/thepipe',
     packages=find_packages(),
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     python_requires='>=3.6',
     install_requires=open('requirements.txt').read().splitlines(),
-    include_package_data=True
+    include_package_data=True,
+    entry_points={
+        'console_scripts': [
+            'thepipe=thepipe_api.thepipe:main',
+        ],
+    }
 )
```

### Comparing `thepipe_api-0.1.6/tests/test_thepipe.py` & `thepipe_api-0.1.7/tests/test_thepipe.py`

 * *Files identical despite different names*

### Comparing `thepipe_api-0.1.6/thepipe_api/compressor.py` & `thepipe_api-0.1.7/thepipe_api/compressor.py`

 * *Files identical despite different names*

### Comparing `thepipe_api-0.1.6/thepipe_api/core.py` & `thepipe_api-0.1.7/thepipe_api/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,11 +68,10 @@
     messages = []
     for chunk in chunks:
         content = []
         if chunk.text:
             content.append({"type": "text", "text": f"""{chunk.path}:\n```\n{chunk.text}\n```\n"""})
         if chunk.image:
             base64_image = image_to_base64(chunk.image)
-            content.append({"type": "text", "text": f"""{chunk.path} image:"""})
             content.append({"type": "image_url", "image_url": {"url": f"data:image/jpeg;base64,{base64_image}"}})
         messages.append({"role": "user", "content": content})
     return messages
```

### Comparing `thepipe_api-0.1.6/thepipe_api/extractor.py` & `thepipe_api-0.1.7/thepipe_api/extractor.py`

 * *Files 1% similar despite different names*

```diff
@@ -247,15 +247,15 @@
     if extension is not None and extension in KNOWN_EXTENSIONS:
         # if url has a file extension, download and extract into tempfile
         with tempfile.TemporaryDirectory() as temp_dir:
             file_path = os.path.join(temp_dir, os.path.basename(url))
             response = requests.get(url)
             with open(file_path, 'wb') as file:
                 file.write(response.content)
-            chunks = extract_from_source(source=file_path, text_only=text_only)
+            chunks = extract_from_source(source=file_path, text_only=text_only, local=local)
     else:
         # use playwright to extract text and images from the URL
         from playwright.sync_api import sync_playwright # import only if needed
         with sync_playwright() as p:
             browser = p.chromium.launch()
             page = browser.new_page()
             page.goto(url)
```

### Comparing `thepipe_api-0.1.6/thepipe_api/thepipe.py` & `thepipe_api-0.1.7/thepipe_api/thepipe.py`

 * *Files identical despite different names*

### Comparing `thepipe_api-0.1.6/thepipe_api.egg-info/PKG-INFO` & `thepipe_api-0.1.7/thepipe_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thepipe_api
-Version: 0.1.6
+Version: 0.1.7
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
-Metadata-Version: 2.1 Name: thepipe_api Version: 0.1.6 Summary: Automate
+Metadata-Version: 2.1 Name: thepipe_api Version: 0.1.7 Summary: Automate
 information extraction for multimodal LLMs. Home-page: https://github.com/emcf/
 thepipe Author: Emmett McFarlane Author-email: emmett@thepi.pe Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 aiohttp Requires-Dist: charset-normalizer Requires-Dist: Pyarrow Requires-Dist:
 python-magic Requires-Dist: colorama Requires-Dist: requests Requires-Dist:
```

