# Comparing `tmp/tiktok-dlpy-2.0.1.tar.gz` & `tmp/tiktok-dlpy-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiktok-dlpy-2.0.1.tar", last modified: Wed Mar 27 19:19:08 2024, max compression
+gzip compressed data, was "tiktok-dlpy-2.1.0.tar", last modified: Tue Apr 16 11:14:36 2024, max compression
```

## Comparing `tiktok-dlpy-2.0.1.tar` & `tiktok-dlpy-2.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 becky      (501) staff       (20)        0 2024-03-27 19:19:08.790880 tiktok-dlpy-2.0.1/
--rw-r--r--   0 becky      (501) staff       (20)    34888 2024-03-27 19:03:28.000000 tiktok-dlpy-2.0.1/LICENSE
--rw-r--r--   0 becky      (501) staff       (20)     1407 2024-03-27 19:19:08.790800 tiktok-dlpy-2.0.1/PKG-INFO
--rw-r--r--   0 becky      (501) staff       (20)      645 2024-03-27 19:03:28.000000 tiktok-dlpy-2.0.1/README.md
--rw-r--r--   0 becky      (501) staff       (20)       79 2024-03-27 19:19:08.791120 tiktok-dlpy-2.0.1/setup.cfg
--rw-r--r--   0 becky      (501) staff       (20)     1064 2024-03-27 19:17:07.000000 tiktok-dlpy-2.0.1/setup.py
-drwxr-xr-x   0 becky      (501) staff       (20)        0 2024-03-27 19:19:08.788933 tiktok-dlpy-2.0.1/tests/
--rw-r--r--   0 becky      (501) staff       (20)     4734 2024-03-27 19:03:28.000000 tiktok-dlpy-2.0.1/tests/test_dataclasses.py
--rw-r--r--   0 becky      (501) staff       (20)     3642 2024-03-27 19:15:10.000000 tiktok-dlpy-2.0.1/tests/test_urls.py
-drwxr-xr-x   0 becky      (501) staff       (20)        0 2024-03-27 19:19:08.790613 tiktok-dlpy-2.0.1/tiktok_dlpy.egg-info/
--rw-r--r--   0 becky      (501) staff       (20)     1407 2024-03-27 19:19:08.000000 tiktok-dlpy-2.0.1/tiktok_dlpy.egg-info/PKG-INFO
--rw-r--r--   0 becky      (501) staff       (20)      447 2024-03-27 19:19:08.000000 tiktok-dlpy-2.0.1/tiktok_dlpy.egg-info/SOURCES.txt
--rw-r--r--   0 becky      (501) staff       (20)        1 2024-03-27 19:19:08.000000 tiktok-dlpy-2.0.1/tiktok_dlpy.egg-info/dependency_links.txt
--rw-r--r--   0 becky      (501) staff       (20)       31 2024-03-27 19:19:08.000000 tiktok-dlpy-2.0.1/tiktok_dlpy.egg-info/requires.txt
--rw-r--r--   0 becky      (501) staff       (20)        9 2024-03-27 19:19:08.000000 tiktok-dlpy-2.0.1/tiktok_dlpy.egg-info/top_level.txt
-drwxr-xr-x   0 becky      (501) staff       (20)        0 2024-03-27 19:19:08.790459 tiktok-dlpy-2.0.1/tiktokdl/
--rw-r--r--   0 becky      (501) staff       (20)      316 2024-01-23 11:05:03.000000 tiktok-dlpy-2.0.1/tiktokdl/__init__.py
--rw-r--r--   0 becky      (501) staff       (20)     7480 2024-03-27 19:03:28.000000 tiktok-dlpy-2.0.1/tiktokdl/captcha.py
--rw-r--r--   0 becky      (501) staff       (20)    10854 2024-03-27 19:15:56.000000 tiktok-dlpy-2.0.1/tiktokdl/download_post.py
--rw-r--r--   0 becky      (501) staff       (20)     1111 2024-03-24 14:23:50.000000 tiktok-dlpy-2.0.1/tiktokdl/exceptions.py
--rw-r--r--   0 becky      (501) staff       (20)     2316 2024-03-27 19:03:28.000000 tiktok-dlpy-2.0.1/tiktokdl/image_processing.py
--rw-r--r--   0 becky      (501) staff       (20)      586 2024-03-24 14:23:53.000000 tiktok-dlpy-2.0.1/tiktokdl/post_data.py
--rw-r--r--   0 becky      (501) staff       (20)     3791 2024-03-27 19:03:28.000000 tiktok-dlpy-2.0.1/tiktokdl/session_store.py
--rw-r--r--   0 becky      (501) staff       (20)     1042 2024-03-27 19:03:28.000000 tiktok-dlpy-2.0.1/tiktokdl/tiktok_magic.py
+drwxr-xr-x   0 becky      (501) staff       (20)        0 2024-04-16 11:14:36.661659 tiktok-dlpy-2.1.0/
+-rw-r--r--   0 becky      (501) staff       (20)    34888 2024-03-27 19:03:28.000000 tiktok-dlpy-2.1.0/LICENSE
+-rw-r--r--   0 becky      (501) staff       (20)     1551 2024-04-16 11:14:36.661586 tiktok-dlpy-2.1.0/PKG-INFO
+-rw-r--r--   0 becky      (501) staff       (20)      739 2024-04-16 11:04:03.000000 tiktok-dlpy-2.1.0/README.md
+-rw-r--r--   0 becky      (501) staff       (20)       79 2024-04-16 11:14:36.661832 tiktok-dlpy-2.1.0/setup.cfg
+-rw-r--r--   0 becky      (501) staff       (20)     1071 2024-04-16 11:07:18.000000 tiktok-dlpy-2.1.0/setup.py
+drwxr-xr-x   0 becky      (501) staff       (20)        0 2024-04-16 11:14:36.658952 tiktok-dlpy-2.1.0/tests/
+-rw-r--r--   0 becky      (501) staff       (20)     4734 2024-03-27 19:03:28.000000 tiktok-dlpy-2.1.0/tests/test_dataclasses.py
+-rw-r--r--   0 becky      (501) staff       (20)     3642 2024-03-27 19:15:10.000000 tiktok-dlpy-2.1.0/tests/test_urls.py
+drwxr-xr-x   0 becky      (501) staff       (20)        0 2024-04-16 11:14:36.661402 tiktok-dlpy-2.1.0/tiktok_dlpy.egg-info/
+-rw-r--r--   0 becky      (501) staff       (20)     1551 2024-04-16 11:14:36.000000 tiktok-dlpy-2.1.0/tiktok_dlpy.egg-info/PKG-INFO
+-rw-r--r--   0 becky      (501) staff       (20)      447 2024-04-16 11:14:36.000000 tiktok-dlpy-2.1.0/tiktok_dlpy.egg-info/SOURCES.txt
+-rw-r--r--   0 becky      (501) staff       (20)        1 2024-04-16 11:14:36.000000 tiktok-dlpy-2.1.0/tiktok_dlpy.egg-info/dependency_links.txt
+-rw-r--r--   0 becky      (501) staff       (20)       40 2024-04-16 11:14:36.000000 tiktok-dlpy-2.1.0/tiktok_dlpy.egg-info/requires.txt
+-rw-r--r--   0 becky      (501) staff       (20)        9 2024-04-16 11:14:36.000000 tiktok-dlpy-2.1.0/tiktok_dlpy.egg-info/top_level.txt
+drwxr-xr-x   0 becky      (501) staff       (20)        0 2024-04-16 11:14:36.661259 tiktok-dlpy-2.1.0/tiktokdl/
+-rw-r--r--   0 becky      (501) staff       (20)      316 2024-01-23 11:05:03.000000 tiktok-dlpy-2.1.0/tiktokdl/__init__.py
+-rw-r--r--   0 becky      (501) staff       (20)     7480 2024-03-27 19:03:28.000000 tiktok-dlpy-2.1.0/tiktokdl/captcha.py
+-rw-r--r--   0 becky      (501) staff       (20)    11384 2024-04-16 11:02:33.000000 tiktok-dlpy-2.1.0/tiktokdl/download_post.py
+-rw-r--r--   0 becky      (501) staff       (20)     1111 2024-03-24 14:23:50.000000 tiktok-dlpy-2.1.0/tiktokdl/exceptions.py
+-rw-r--r--   0 becky      (501) staff       (20)     2316 2024-03-27 19:03:28.000000 tiktok-dlpy-2.1.0/tiktokdl/image_processing.py
+-rw-r--r--   0 becky      (501) staff       (20)      586 2024-03-24 14:23:53.000000 tiktok-dlpy-2.1.0/tiktokdl/post_data.py
+-rw-r--r--   0 becky      (501) staff       (20)     3791 2024-03-27 19:03:28.000000 tiktok-dlpy-2.1.0/tiktokdl/session_store.py
+-rw-r--r--   0 becky      (501) staff       (20)     1163 2024-04-16 11:03:31.000000 tiktok-dlpy-2.1.0/tiktokdl/tiktok_magic.py
```

### Comparing `tiktok-dlpy-2.0.1/LICENSE` & `tiktok-dlpy-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tiktok-dlpy-2.0.1/PKG-INFO` & `tiktok-dlpy-2.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,38 @@
 Metadata-Version: 2.1
 Name: tiktok-dlpy
-Version: 2.0.1
+Version: 2.1.0
 Summary: A package to download TikTok videos or slideshows by URL without needing to login
 Home-page: https://github.com/Fluxticks/TikTokDL
-Download-URL: https://github.com/Fluxticks/TikTokDL/archive/v2.0.1.tar.gz
+Download-URL: https://github.com/Fluxticks/TikTokDL/archive/v2.1.0.tar.gz
 Author: Fluxticks
 Keywords: tiktok,playwright,async
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: playwright
 Requires-Dist: numpy
 Requires-Dist: opencv-python
+Requires-Dist: requests
 
 ![Main Workflow](https://github.com/Fluxticks/TikTokDL/actions/workflows/main.yml/badge.svg) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tiktok-dlpy)
 
 # TikTokDL
 
 A python package to download TikTok videos or slideshows by URL without needing to login.
 
+## TODO:
+
+- Find a more exact value for `tiktok_magic.MAXIMUM_REQUEST_BODY` (Currently ~8MB)
+
 ## Usage
 
 1. Install the package
 
 ```bash
 $ pip install tiktok-dlpy
 ```
```

### Comparing `tiktok-dlpy-2.0.1/README.md` & `tiktok-dlpy-2.1.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 ![Main Workflow](https://github.com/Fluxticks/TikTokDL/actions/workflows/main.yml/badge.svg) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tiktok-dlpy)
 
 # TikTokDL
 
 A python package to download TikTok videos or slideshows by URL without needing to login.
 
+## TODO:
+
+- Find a more exact value for `tiktok_magic.MAXIMUM_REQUEST_BODY` (Currently ~8MB)
+
 ## Usage
 
 1. Install the package
 
 ```bash
 $ pip install tiktok-dlpy
 ```
```

### Comparing `tiktok-dlpy-2.0.1/setup.py` & `tiktok-dlpy-2.1.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,30 +3,26 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="tiktok-dlpy",
-    version="2.0.1",
+    version="2.1.0",
     url="https://github.com/Fluxticks/TikTokDL",
-    download_url="https://github.com/Fluxticks/TikTokDL/archive/v2.0.1.tar.gz",
+    download_url="https://github.com/Fluxticks/TikTokDL/archive/v2.1.0.tar.gz",
     author="Fluxticks",
     packages=find_packages(),
-    install_requires=[
-        "playwright",
-        "numpy",
-        "opencv-python",
-    ],
+    install_requires=["playwright", "numpy", "opencv-python", "requests"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     description="A package to download TikTok videos or slideshows by URL without needing to login",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
-        "License :: OSI Approved :: MIT License",
+        "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
     ],
     keywords=["tiktok", "playwright", "async"],
 )
```

### Comparing `tiktok-dlpy-2.0.1/tests/test_dataclasses.py` & `tiktok-dlpy-2.1.0/tests/test_dataclasses.py`

 * *Files identical despite different names*

### Comparing `tiktok-dlpy-2.0.1/tests/test_urls.py` & `tiktok-dlpy-2.1.0/tests/test_urls.py`

 * *Files identical despite different names*

### Comparing `tiktok-dlpy-2.0.1/tiktok_dlpy.egg-info/PKG-INFO` & `tiktok-dlpy-2.1.0/tiktok_dlpy.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,38 @@
 Metadata-Version: 2.1
 Name: tiktok-dlpy
-Version: 2.0.1
+Version: 2.1.0
 Summary: A package to download TikTok videos or slideshows by URL without needing to login
 Home-page: https://github.com/Fluxticks/TikTokDL
-Download-URL: https://github.com/Fluxticks/TikTokDL/archive/v2.0.1.tar.gz
+Download-URL: https://github.com/Fluxticks/TikTokDL/archive/v2.1.0.tar.gz
 Author: Fluxticks
 Keywords: tiktok,playwright,async
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: playwright
 Requires-Dist: numpy
 Requires-Dist: opencv-python
+Requires-Dist: requests
 
 ![Main Workflow](https://github.com/Fluxticks/TikTokDL/actions/workflows/main.yml/badge.svg) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tiktok-dlpy)
 
 # TikTokDL
 
 A python package to download TikTok videos or slideshows by URL without needing to login.
 
+## TODO:
+
+- Find a more exact value for `tiktok_magic.MAXIMUM_REQUEST_BODY` (Currently ~8MB)
+
 ## Usage
 
 1. Install the package
 
 ```bash
 $ pip install tiktok-dlpy
 ```
```

### Comparing `tiktok-dlpy-2.0.1/tiktokdl/captcha.py` & `tiktok-dlpy-2.1.0/tiktokdl/captcha.py`

 * *Files identical despite different names*

### Comparing `tiktok-dlpy-2.0.1/tiktokdl/download_post.py` & `tiktok-dlpy-2.1.0/tiktokdl/download_post.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import inspect
 from asyncio import sleep as async_sleep
 from datetime import datetime, timezone
 from os.path import curdir
 from os.path import sep as PATH_SEP
+import requests
 from urllib.request import urlretrieve
 
 from playwright.async_api import BrowserContext, Page, async_playwright, Playwright
 
 from tiktokdl.captcha import verify_session
 from tiktokdl.exceptions import (
     CaptchaFailedException,
     DownloadFailedException,
     ResponseParseException,
     RetryLimitReached,
 )
+from tiktokdl.tiktok_magic import MAXIMUM_REQUEST_BODY
 from tiktokdl.post_data import TikTokPost, TikTokSlide, TikTokVideo
 
 from typing import Literal, Union
 
 __all__ = ["get_post"]
 
 
@@ -149,23 +151,34 @@
         download_path (str | None): The path to download the video to. If None, uses current directory.
     """
     download_path = __validate_download_path(download_path)
     page_video_tag = playwright_page.locator("video").first
     video_source = await page_video_tag.get_attribute("src")
 
     response_base_url = video_source.split("?")[0]
-    async with playwright_page.expect_request_finished(
+    async with playwright_page.expect_request(
         lambda x: response_base_url in x.url, timeout=timeout
     ) as request:
-        request_value = await request.value
-        response = await request_value.response()
-        save_path = f"{download_path}{video_info.post_id}.mp4"
+        await playwright_page.reload()
+    request_value = await request.value
+    response = await request_value.response()
+    video_size = await response.header_value("content-length")
+    save_path = f"{download_path}{video_info.post_id}.mp4"
+    if int(video_size) < MAXIMUM_REQUEST_BODY:
         with open(save_path, "wb") as f:
             f.write(await response.body())
-        video_info.file_path = save_path
+    else:
+        request_headers = await request_value.all_headers()
+        with requests.get(request_value.url, headers=request_headers, stream=True) as r:
+            r.raise_for_status()
+            with open(save_path, "wb") as f:
+                for chunk in r.iter_content(chunk_size=8192):
+                    f.write(chunk)
+
+    video_info.file_path = save_path
 
 
 async def download_slideshow(video_info: TikTokSlide, download_path: Union[str, None]):
     """For a given Slideshow post, download the images associated with it.
 
     Args:
         video_info (TikTokSlide): The Slideshow post data.
```

### Comparing `tiktok-dlpy-2.0.1/tiktokdl/exceptions.py` & `tiktok-dlpy-2.1.0/tiktokdl/exceptions.py`

 * *Files identical despite different names*

### Comparing `tiktok-dlpy-2.0.1/tiktokdl/image_processing.py` & `tiktok-dlpy-2.1.0/tiktokdl/image_processing.py`

 * *Files identical despite different names*

### Comparing `tiktok-dlpy-2.0.1/tiktokdl/post_data.py` & `tiktok-dlpy-2.1.0/tiktokdl/post_data.py`

 * *Files identical despite different names*

### Comparing `tiktok-dlpy-2.0.1/tiktokdl/session_store.py` & `tiktok-dlpy-2.1.0/tiktokdl/session_store.py`

 * *Files identical despite different names*

### Comparing `tiktok-dlpy-2.0.1/tiktokdl/tiktok_magic.py` & `tiktok-dlpy-2.1.0/tiktokdl/tiktok_magic.py`

 * *Files 16% similar despite different names*

```diff
@@ -31,7 +31,10 @@
 # Magic numbers used for CAPTCHA verification
 OS_TYPE = 2
 CHALLENGE_CODE = 99999
 CAPTCHA_VERSION = 2
 
 # The cookie that stores the device_id of the current session.
 DEVICE_ID_TARGET_COOKIE = "__tea_cache_tokens"
+
+# The maximum size of the video that can be downloaded using playwright's body
+MAXIMUM_REQUEST_BODY = 8_000_000  # 8 MB
```

