# Comparing `tmp/webscout-1.2.9.tar.gz` & `tmp/webscout-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webscout-1.2.9.tar", last modified: Fri Apr 12 12:05:49 2024, max compression
+gzip compressed data, was "webscout-1.3.0.tar", last modified: Tue Apr 16 06:20:30 2024, max compression
```

## Comparing `webscout-1.2.9.tar` & `webscout-1.3.0.tar`

### file list

```diff
@@ -1,46 +1,47 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 12:05:49.785675 webscout-1.2.9/
-drwxrwxrwx   0        0        0        0 2024-04-12 12:05:48.784895 webscout-1.2.9/DeepWEBS/
--rw-rw-rw-   0        0        0        0 2024-04-11 08:32:30.000000 webscout-1.2.9/DeepWEBS/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 12:05:48.833863 webscout-1.2.9/DeepWEBS/documents/
--rw-rw-rw-   0        0        0        0 2024-04-11 08:32:30.000000 webscout-1.2.9/DeepWEBS/documents/__init__.py
--rw-rw-rw-   0        0        0     4049 2024-04-11 08:32:30.000000 webscout-1.2.9/DeepWEBS/documents/query_results_extractor.py
--rw-rw-rw-   0        0        0     5272 2024-04-11 08:32:30.000000 webscout-1.2.9/DeepWEBS/documents/webpage_content_extractor.py
-drwxrwxrwx   0        0        0        0 2024-04-12 12:05:48.903418 webscout-1.2.9/DeepWEBS/networks/
--rw-rw-rw-   0        0        0        0 2024-04-11 08:32:30.000000 webscout-1.2.9/DeepWEBS/networks/__init__.py
--rw-rw-rw-   0        0        0     3183 2024-04-11 08:32:30.000000 webscout-1.2.9/DeepWEBS/networks/filepath_converter.py
--rw-rw-rw-   0        0        0     1966 2024-04-11 08:32:30.000000 webscout-1.2.9/DeepWEBS/networks/google_searcher.py
--rw-rw-rw-   0        0        0      726 2024-04-11 08:32:30.000000 webscout-1.2.9/DeepWEBS/networks/network_configs.py
--rw-rw-rw-   0        0        0     3846 2024-04-11 08:32:30.000000 webscout-1.2.9/DeepWEBS/networks/webpage_fetcher.py
-drwxrwxrwx   0        0        0        0 2024-04-12 12:05:48.964442 webscout-1.2.9/DeepWEBS/utilsdw/
--rw-rw-rw-   0        0        0        0 2024-04-11 08:32:30.000000 webscout-1.2.9/DeepWEBS/utilsdw/__init__.py
--rw-rw-rw-   0        0        0     1754 2024-04-11 08:32:30.000000 webscout-1.2.9/DeepWEBS/utilsdw/enver.py
--rw-rw-rw-   0        0        0     8174 2024-04-11 08:32:30.000000 webscout-1.2.9/DeepWEBS/utilsdw/logger.py
--rw-rw-rw-   0        0        0     3150 2024-04-11 08:32:30.000000 webscout-1.2.9/LICENSE.md
--rw-rw-rw-   0        0        0    24513 2024-04-12 12:05:49.768680 webscout-1.2.9/PKG-INFO
--rw-rw-rw-   0        0        0    22338 2024-04-11 08:32:30.000000 webscout-1.2.9/README.md
--rw-rw-rw-   0        0        0       42 2024-04-12 12:05:49.786678 webscout-1.2.9/setup.cfg
--rw-rw-rw-   0        0        0     2817 2024-04-12 12:04:17.000000 webscout-1.2.9/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-12 12:05:49.350092 webscout-1.2.9/webscout/
--rw-rw-rw-   0        0        0    57985 2024-04-11 08:32:30.000000 webscout-1.2.9/webscout/AI.py
--rw-rw-rw-   0        0        0     2343 2024-04-11 08:32:30.000000 webscout-1.2.9/webscout/AIbase.py
--rw-rw-rw-   0        0        0    24123 2024-04-11 08:32:30.000000 webscout-1.2.9/webscout/AIutel.py
--rw-rw-rw-   0        0        0     7332 2024-04-11 08:32:30.000000 webscout-1.2.9/webscout/DWEBS.py
--rw-rw-rw-   0        0        0     8103 2024-04-11 08:32:30.000000 webscout-1.2.9/webscout/HelpingAI.py
--rw-rw-rw-   0        0        0     3309 2024-04-11 08:32:30.000000 webscout-1.2.9/webscout/LLM.py
--rw-rw-rw-   0        0        0      519 2024-04-11 08:32:30.000000 webscout-1.2.9/webscout/__init__.py
--rw-rw-rw-   0        0        0      126 2024-04-11 08:32:30.000000 webscout-1.2.9/webscout/__main__.py
--rw-rw-rw-   0        0        0    17059 2024-04-11 08:32:30.000000 webscout-1.2.9/webscout/cli.py
--rw-rw-rw-   0        0        0      276 2024-04-11 08:32:30.000000 webscout-1.2.9/webscout/exceptions.py
--rw-rw-rw-   0        0        0      692 2024-04-11 08:32:30.000000 webscout-1.2.9/webscout/models.py
--rw-rw-rw-   0        0        0    20622 2024-04-11 08:35:51.000000 webscout-1.2.9/webscout/transcriber.py
--rw-rw-rw-   0        0        0     2605 2024-04-11 08:32:30.000000 webscout-1.2.9/webscout/utils.py
--rw-rw-rw-   0        0        0       25 2024-04-12 12:04:27.000000 webscout-1.2.9/webscout/version.py
--rw-rw-rw-   0        0        0     3085 2024-04-11 08:32:30.000000 webscout-1.2.9/webscout/webscout_search.py
--rw-rw-rw-   0        0        0    40670 2024-04-11 08:32:30.000000 webscout-1.2.9/webscout/webscout_search_async.py
-drwxrwxrwx   0        0        0        0 2024-04-12 12:05:49.753666 webscout-1.2.9/webscout.egg-info/
--rw-rw-rw-   0        0        0    24513 2024-04-12 12:05:47.000000 webscout-1.2.9/webscout.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      965 2024-04-12 12:05:48.000000 webscout-1.2.9/webscout.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 12:05:47.000000 webscout-1.2.9/webscout.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      197 2024-04-12 12:05:47.000000 webscout-1.2.9/webscout.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      334 2024-04-12 12:05:47.000000 webscout-1.2.9/webscout.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-12 12:05:47.000000 webscout-1.2.9/webscout.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-16 06:20:30.401520 webscout-1.3.0/
+drwxrwxrwx   0        0        0        0 2024-04-16 06:20:28.274165 webscout-1.3.0/DeepWEBS/
+-rw-rw-rw-   0        0        0        0 2024-04-11 08:32:30.000000 webscout-1.3.0/DeepWEBS/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 06:20:28.316481 webscout-1.3.0/DeepWEBS/documents/
+-rw-rw-rw-   0        0        0        0 2024-04-11 08:32:30.000000 webscout-1.3.0/DeepWEBS/documents/__init__.py
+-rw-rw-rw-   0        0        0     4049 2024-04-11 08:32:30.000000 webscout-1.3.0/DeepWEBS/documents/query_results_extractor.py
+-rw-rw-rw-   0        0        0     5272 2024-04-11 08:32:30.000000 webscout-1.3.0/DeepWEBS/documents/webpage_content_extractor.py
+drwxrwxrwx   0        0        0        0 2024-04-16 06:20:28.398477 webscout-1.3.0/DeepWEBS/networks/
+-rw-rw-rw-   0        0        0        0 2024-04-11 08:32:30.000000 webscout-1.3.0/DeepWEBS/networks/__init__.py
+-rw-rw-rw-   0        0        0     3183 2024-04-11 08:32:30.000000 webscout-1.3.0/DeepWEBS/networks/filepath_converter.py
+-rw-rw-rw-   0        0        0     1966 2024-04-11 08:32:30.000000 webscout-1.3.0/DeepWEBS/networks/google_searcher.py
+-rw-rw-rw-   0        0        0      726 2024-04-11 08:32:30.000000 webscout-1.3.0/DeepWEBS/networks/network_configs.py
+-rw-rw-rw-   0        0        0     3846 2024-04-11 08:32:30.000000 webscout-1.3.0/DeepWEBS/networks/webpage_fetcher.py
+drwxrwxrwx   0        0        0        0 2024-04-16 06:20:28.487584 webscout-1.3.0/DeepWEBS/utilsdw/
+-rw-rw-rw-   0        0        0        0 2024-04-11 08:32:30.000000 webscout-1.3.0/DeepWEBS/utilsdw/__init__.py
+-rw-rw-rw-   0        0        0     1754 2024-04-11 08:32:30.000000 webscout-1.3.0/DeepWEBS/utilsdw/enver.py
+-rw-rw-rw-   0        0        0     8174 2024-04-11 08:32:30.000000 webscout-1.3.0/DeepWEBS/utilsdw/logger.py
+-rw-rw-rw-   0        0        0     3150 2024-04-11 08:32:30.000000 webscout-1.3.0/LICENSE.md
+-rw-rw-rw-   0        0        0    28244 2024-04-16 06:20:30.394520 webscout-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0    26069 2024-04-16 06:09:35.000000 webscout-1.3.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-16 06:20:30.402520 webscout-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     2817 2024-04-16 06:11:02.000000 webscout-1.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 06:20:29.891443 webscout-1.3.0/webscout/
+-rw-rw-rw-   0        0        0    57985 2024-04-11 08:32:30.000000 webscout-1.3.0/webscout/AI.py
+-rw-rw-rw-   0        0        0     2343 2024-04-11 08:32:30.000000 webscout-1.3.0/webscout/AIbase.py
+-rw-rw-rw-   0        0        0    24123 2024-04-11 08:32:30.000000 webscout-1.3.0/webscout/AIutel.py
+-rw-rw-rw-   0        0        0     7332 2024-04-11 08:32:30.000000 webscout-1.3.0/webscout/DWEBS.py
+-rw-rw-rw-   0        0        0     8103 2024-04-11 08:32:30.000000 webscout-1.3.0/webscout/HelpingAI.py
+-rw-rw-rw-   0        0        0     3309 2024-04-11 08:32:30.000000 webscout-1.3.0/webscout/LLM.py
+-rw-rw-rw-   0        0        0      550 2024-04-16 06:01:50.000000 webscout-1.3.0/webscout/__init__.py
+-rw-rw-rw-   0        0        0      126 2024-04-11 08:32:30.000000 webscout-1.3.0/webscout/__main__.py
+-rw-rw-rw-   0        0        0    17059 2024-04-11 08:32:30.000000 webscout-1.3.0/webscout/cli.py
+-rw-rw-rw-   0        0        0      276 2024-04-11 08:32:30.000000 webscout-1.3.0/webscout/exceptions.py
+-rw-rw-rw-   0        0        0      692 2024-04-11 08:32:30.000000 webscout-1.3.0/webscout/models.py
+-rw-rw-rw-   0        0        0    20622 2024-04-11 08:35:51.000000 webscout-1.3.0/webscout/transcriber.py
+-rw-rw-rw-   0        0        0     2605 2024-04-11 08:32:30.000000 webscout-1.3.0/webscout/utils.py
+-rw-rw-rw-   0        0        0       25 2024-04-16 06:11:14.000000 webscout-1.3.0/webscout/version.py
+-rw-rw-rw-   0        0        0      941 2024-04-16 06:00:31.000000 webscout-1.3.0/webscout/voice.py
+-rw-rw-rw-   0        0        0     3085 2024-04-11 08:32:30.000000 webscout-1.3.0/webscout/webscout_search.py
+-rw-rw-rw-   0        0        0    40670 2024-04-11 08:32:30.000000 webscout-1.3.0/webscout/webscout_search_async.py
+drwxrwxrwx   0        0        0        0 2024-04-16 06:20:30.369522 webscout-1.3.0/webscout.egg-info/
+-rw-rw-rw-   0        0        0    28244 2024-04-16 06:20:26.000000 webscout-1.3.0/webscout.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      983 2024-04-16 06:20:27.000000 webscout-1.3.0/webscout.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 06:20:26.000000 webscout-1.3.0/webscout.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      197 2024-04-16 06:20:26.000000 webscout-1.3.0/webscout.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      334 2024-04-16 06:20:26.000000 webscout-1.3.0/webscout.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-16 06:20:26.000000 webscout-1.3.0/webscout.egg-info/top_level.txt
```

### Comparing `webscout-1.2.9/DeepWEBS/documents/query_results_extractor.py` & `webscout-1.3.0/DeepWEBS/documents/query_results_extractor.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.9/DeepWEBS/documents/webpage_content_extractor.py` & `webscout-1.3.0/DeepWEBS/documents/webpage_content_extractor.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.9/DeepWEBS/networks/filepath_converter.py` & `webscout-1.3.0/DeepWEBS/networks/filepath_converter.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.9/DeepWEBS/networks/google_searcher.py` & `webscout-1.3.0/DeepWEBS/networks/google_searcher.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.9/DeepWEBS/networks/network_configs.py` & `webscout-1.3.0/DeepWEBS/networks/network_configs.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.9/DeepWEBS/networks/webpage_fetcher.py` & `webscout-1.3.0/DeepWEBS/networks/webpage_fetcher.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.9/DeepWEBS/utilsdw/enver.py` & `webscout-1.3.0/DeepWEBS/utilsdw/enver.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.9/DeepWEBS/utilsdw/logger.py` & `webscout-1.3.0/DeepWEBS/utilsdw/logger.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.9/LICENSE.md` & `webscout-1.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `webscout-1.2.9/PKG-INFO` & `webscout-1.3.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,59 +1,7 @@
-Metadata-Version: 2.1
-Name: webscout
-Version: 1.2.9
-Summary: Search for words, documents, images, videos, news, maps and text translation using the Google, DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models and now can transcribe yt videos
-Author: OEvortex
-Author-email: helpingai5@gmail.com
-License: HelpingAI Simplified Universal License
-Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
-Project-URL: Source, https://github.com/OE-LUCIFER/Webscout
-Project-URL: Tracker, https://github.com/OE-LUCIFER/Webscout/issues
-Project-URL: YouTube, https://youtube.com/@OEvortex
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: Other/Proprietary License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-Requires-Dist: docstring_inheritance>=2.1.2
-Requires-Dist: click>=8.1.7
-Requires-Dist: curl_cffi>=0.6.0b7
-Requires-Dist: lxml>=5.1.0
-Requires-Dist: nest-asyncio>=1.6.0
-Requires-Dist: selenium>=4.1.3
-Requires-Dist: tqdm>=4.64.0
-Requires-Dist: webdriver-manager>=3.5.4
-Requires-Dist: halo>=0.0.31
-Requires-Dist: g4f>=0.2.2.3
-Requires-Dist: rich
-Requires-Dist: python-dotenv
-Requires-Dist: Helpingai-T2
-Requires-Dist: beautifulsoup4
-Requires-Dist: markdownify
-Requires-Dist: pydantic
-Requires-Dist: requests
-Requires-Dist: sse_starlette
-Requires-Dist: termcolor
-Requires-Dist: tiktoken
-Requires-Dist: tldextract
-Requires-Dist: orjson
-Provides-Extra: dev
-Requires-Dist: ruff>=0.1.6; extra == "dev"
-Requires-Dist: pytest>=7.4.2; extra == "dev"
-
 #  webscout
 <p align="center">
 
 <a href="#"><img alt="Python version" src="https://img.shields.io/pypi/pyversions/webscout"/></a>
 <a href="https://pepy.tech/project/webscout"><img alt="Downloads" src="https://static.pepy.tech/badge/webscout"></a>
 
 Search for words, documents, images, videos, news, maps and text translation using the Google, DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models and now can transcribe yt videos
@@ -68,14 +16,17 @@
   - [CLI to use LLM](#cli-to-use-llm)
   - [Regions](#regions)
   - [Transcriber](#transcriber)
   - [DeepWEBS: Advanced Web Searches](#deepwebs-advanced-web-searches)
     - [Activating DeepWEBS](#activating-deepwebs)
     - [Point to remember before using `DeepWEBS`](#point-to-remember-before-using-deepwebs)
     - [Usage Example](#usage-example)
+  - [Text-to-Speech:](#text-to-speech)
+    - [Available TTS Voices:](#available-tts-voices)
+    - [ALL voices:](#all-voices)
   - [WEBS and AsyncWEBS classes](#webs-and-asyncwebs-classes)
   - [Exceptions](#exceptions)
   - [usage of webscout](#usage-of-webscout)
     - [1. `text()` - text search by DuckDuckGo.com and Yep.com](#1-text---text-search-by-duckduckgocom-and-yepcom)
     - [2. `answers()` - instant answers by DuckDuckGo.com and Yep.com](#2-answers---instant-answers-by-duckduckgocom-and-yepcom)
     - [3. `images()` - image search by DuckDuckGo.com and Yep.com](#3-images---image-search-by-duckduckgocom-and-yepcom)
     - [4. `videos()` - video search by DuckDuckGo.com](#4-videos---video-search-by-duckduckgocom)
@@ -333,14 +284,31 @@
     # Print the search results
     print_search_results(results)
 
 if __name__ == "__main__":
     main()
 
 ```
+## Text-to-Speech:
+```python
+from webscout import play_audio
+
+message = "This is an example of text-to-speech."
+audio_content = play_audio(message, voice="Brian")
+
+# Save the audio to a file
+with open("output.mp3", "wb") as f:
+    f.write(audio_content)
+```
+### Available TTS Voices:
+You can choose from a wide range of voices, including:
+- Filiz, Astrid, Tatyana, Maxim, Carmen, Ines, Cristiano, Vitoria, Ricardo, Maja, Jan, Jacek, Ewa, Ruben, Lotte, Liv, Seoyeon, Takumi, Mizuki, Giorgio, Carla, Bianca, Karl, Dora, Mathieu, Celine, Chantal, Penelope, Miguel, Mia, Enrique, Conchita, Geraint, Salli, Matthew, Kimberly, Kendra, Justin, Joey, Joanna, Ivy, Raveena, Aditi, Emma, Brian, Amy, Russell, Nicole, Vicki, Marlene, Hans, Naja, Mads, Gwyneth, Zhiyu
+- Standard and WaveNet voices for various languages (e.g., en-US, es-ES, ja-JP, etc.)
+### ALL voices:
+[Filiz, Astrid, Tatyana, Maxim, Carmen, Ines, Cristiano, Vitoria, Ricardo, Maja, Jan, Jacek, Ewa, Ruben, Lotte, Liv, Seoyeon, Takumi, Mizuki, Giorgio, Carla, Bianca, Karl, Dora, Mathieu, Celine, Chantal, Penelope, Miguel, Mia, Enrique, Conchita, Geraint, Salli, Matthew, Kimberly, Kendra, Justin, Joey, Joanna, Ivy, Raveena, Aditi, Emma, Brian, Amy, Russell, Nicole, Vicki, Marlene, Hans, Naja, Mads, Gwyneth, Zhiyu, es-ES-Standard-A, it-IT-Standard-A, it-IT-Wavenet-A, ja-JP-Standard-A, ja-JP-Wavenet-A, ko-KR-Standard-A, ko-KR-Wavenet-A, pt-BR-Standard-A, tr-TR-Standard-A, sv-SE-Standard-A, nl-NL-Standard-A, nl-NL-Wavenet-A, en-US-Wavenet-A, en-US-Wavenet-B, en-US-Wavenet-C, en-US-Wavenet-D, en-US-Wavenet-E, en-US-Wavenet-F, en-GB-Standard-A, en-GB-Standard-B, en-GB-Standard-C, en-GB-Standard-D, en-GB-Wavenet-A, en-GB-Wavenet-B, en-GB-Wavenet-C, en-GB-Wavenet-D, en-US-Standard-B, en-US-Standard-C, en-US-Standard-D, en-US-Standard-E, de-DE-Standard-A, de-DE-Standard-B, de-DE-Wavenet-A, de-DE-Wavenet-B, de-DE-Wavenet-C, de-DE-Wavenet-D, en-AU-Standard-A, en-AU-Standard-B, en-AU-Wavenet-A, en-AU-Wavenet-B, en-AU-Wavenet-C, en-AU-Wavenet-D, en-AU-Standard-C, en-AU-Standard-D, fr-CA-Standard-A, fr-CA-Standard-B, fr-CA-Standard-C, fr-CA-Standard-D, fr-FR-Standard-C, fr-FR-Standard-D, fr-FR-Wavenet-A, fr-FR-Wavenet-B, fr-FR-Wavenet-C, fr-FR-Wavenet-D, da-DK-Wavenet-A, pl-PL-Wavenet-A, pl-PL-Wavenet-B, pl-PL-Wavenet-C, pl-PL-Wavenet-D, pt-PT-Wavenet-A, pt-PT-Wavenet-B, pt-PT-Wavenet-C, pt-PT-Wavenet-D, ru-RU-Wavenet-A, ru-RU-Wavenet-B, ru-RU-Wavenet-C, ru-RU-Wavenet-D, sk-SK-Wavenet-A, tr-TR-Wavenet-A, tr-TR-Wavenet-B, tr-TR-Wavenet-C, tr-TR-Wavenet-D, tr-TR-Wavenet-E, uk-UA-Wavenet-A, ar-XA-Wavenet-A, ar-XA-Wavenet-B, ar-XA-Wavenet-C, cs-CZ-Wavenet-A, nl-NL-Wavenet-B, nl-NL-Wavenet-C, nl-NL-Wavenet-D, nl-NL-Wavenet-E, en-IN-Wavenet-A, en-IN-Wavenet-B, en-IN-Wavenet-C, fil-PH-Wavenet-A, fi-FI-Wavenet-A, el-GR-Wavenet-A, hi-IN-Wavenet-A, hi-IN-Wavenet-B, hi-IN-Wavenet-C, hu-HU-Wavenet-A, id-ID-Wavenet-A, id-ID-Wavenet-B, id-ID-Wavenet-C, it-IT-Wavenet-B, it-IT-Wavenet-C, it-IT-Wavenet-D, ja-JP-Wavenet-B, ja-JP-Wavenet-C, ja-JP-Wavenet-D, cmn-CN-Wavenet-A, cmn-CN-Wavenet-B, cmn-CN-Wavenet-C, cmn-CN-Wavenet-D, nb-no-Wavenet-E, nb-no-Wavenet-A, nb-no-Wavenet-B, nb-no-Wavenet-C, nb-no-Wavenet-D, vi-VN-Wavenet-A, vi-VN-Wavenet-B, vi-VN-Wavenet-C, vi-VN-Wavenet-D, sr-rs-Standard-A, lv-lv-Standard-A, is-is-Standard-A, bg-bg-Standard-A, af-ZA-Standard-A, Tracy, Danny, Huihui, Yaoyao, Kangkang, HanHan, Zhiwei, Asaf, An, Stefanos, Filip, Ivan, Heidi, Herena, Kalpana, Hemant, Matej, Andika, Rizwan, Lado, Valluvar, Linda, Heather, Sean, Michael, Karsten, Guillaume, Pattara, Jakub, Szabolcs, Hoda, Naayf]
 ## WEBS and AsyncWEBS classes
 
 The WEBS and AsyncWEBS classes are used to retrieve search results from DuckDuckGo.com and yep.com periodically.
 To use the AsyncWEBS class, you can perform asynchronous operations using Python's asyncio library.
 To initialize an instance of the WEBS or AsyncWEBS classes, you can provide the following optional arguments:
 
 Here is an example of initializing the WEBS class:
```

#### html2text {}

```diff
@@ -1,97 +1,71 @@
-Metadata-Version: 2.1 Name: webscout Version: 1.2.9 Summary: Search for words,
-documents, images, videos, news, maps and text translation using the Google,
-DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models and
-now can transcribe yt videos Author: OEvortex Author-email:
-helpingai5@gmail.com License: HelpingAI Simplified Universal License Project-
-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki Project-URL:
-Source, https://github.com/OE-LUCIFER/Webscout Project-URL: Tracker, https://
-github.com/OE-LUCIFER/Webscout/issues Project-URL: YouTube, https://
-youtube.com/@OEvortex Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers Classifier: License :: Other/
-Proprietary License Classifier: Operating System :: OS Independent Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
-Programming Language :: Python :: Implementation :: CPython Classifier: Topic
-:: Internet :: WWW/HTTP :: Indexing/Search Classifier: Topic :: Software
-Development :: Libraries :: Python Modules Description-Content-Type: text/
-markdown License-File: LICENSE.md Requires-Dist: docstring_inheritance>=2.1.2
-Requires-Dist: click>=8.1.7 Requires-Dist: curl_cffi>=0.6.0b7 Requires-Dist:
-lxml>=5.1.0 Requires-Dist: nest-asyncio>=1.6.0 Requires-Dist: selenium>=4.1.3
-Requires-Dist: tqdm>=4.64.0 Requires-Dist: webdriver-manager>=3.5.4 Requires-
-Dist: halo>=0.0.31 Requires-Dist: g4f>=0.2.2.3 Requires-Dist: rich Requires-
-Dist: python-dotenv Requires-Dist: Helpingai-T2 Requires-Dist: beautifulsoup4
-Requires-Dist: markdownify Requires-Dist: pydantic Requires-Dist: requests
-Requires-Dist: sse_starlette Requires-Dist: termcolor Requires-Dist: tiktoken
-Requires-Dist: tldextract Requires-Dist: orjson Provides-Extra: dev Requires-
-Dist: ruff>=0.1.6; extra == "dev" Requires-Dist: pytest>=7.4.2; extra == "dev"
 # webscout
  _[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_D_o_w_n_l_o_a_d_s_]Search for words, documents, images, videos, news,
 maps and text translation using the Google, DuckDuckGo.com, yep.com, phind.com,
 you.com, etc Also containes AI models and now can transcribe yt videos ## Table
 of Contents - [webscout](#webscout) - [Table of Contents](#table-of-contents) -
       [Install](#install) - [CLI version](#cli-version) - [CLI version of
 webscout.AI](#cli-version-of-webscoutai) - [CLI to use LLM](#cli-to-use-llm) -
   [Regions](#regions) - [Transcriber](#transcriber) - [DeepWEBS: Advanced Web
 Searches](#deepwebs-advanced-web-searches) - [Activating DeepWEBS](#activating-
   deepwebs) - [Point to remember before using `DeepWEBS`](#point-to-remember-
-before-using-deepwebs) - [Usage Example](#usage-example) - [WEBS and AsyncWEBS
- classes](#webs-and-asyncwebs-classes) - [Exceptions](#exceptions) - [usage of
- webscout](#usage-of-webscout) - [1. `text()` - text search by DuckDuckGo.com
-and Yep.com](#1-text---text-search-by-duckduckgocom-and-yepcom) - [2. `answers
-  ()` - instant answers by DuckDuckGo.com and Yep.com](#2-answers---instant-
-    answers-by-duckduckgocom-and-yepcom) - [3. `images()` - image search by
-  DuckDuckGo.com and Yep.com](#3-images---image-search-by-duckduckgocom-and-
- yepcom) - [4. `videos()` - video search by DuckDuckGo.com](#4-videos---video-
-  search-by-duckduckgocom) - [5. `news()` - news search by DuckDuckGo.com and
- yep.com](#5-news---news-search-by-duckduckgocom-and-yepcom) - [6. `maps()` -
-map search by DuckDuckGo.com and](#6-maps---map-search-by-duckduckgocom-and) -
-[7. `translate()` - translation by DuckDuckGo.com and Yep.com](#7-translate---
-translation-by-duckduckgocom-and-yepcom) - [8. `suggestions()` - suggestions by
-DuckDuckGo.com and Yep.com](#8-suggestions---suggestions-by-duckduckgocom-and-
- yepcom) - [usage of webscout.AI](#usage-of-webscoutai) - [1. `PhindSearch` -
-Search using Phind.com](#1-phindsearch---search-using-phindcom) - [2. `YepChat`
- - Chat with mistral 8x7b powered by yepchat](#2-yepchat---chat-with-mistral-
- 8x7b-powered-by-yepchat) - [3. `You.com` - search with you.com](#3-youcom---
- search-with-youcom) - [4. `Gemini` - search with google gemini](#4-gemini---
-   search-with-google-gemini) - [usage of image generator from Webscout.AI]
- (#usage-of-image-generator-from-webscoutai) - [5. `Prodia` - make image using
-  prodia](#5-prodia---make-image-using-prodia) - [6. `BlackBox` - Search/chat
-  With BlackBox](#6-blackbox---searchchat-with-blackbox) - [7. `PERPLEXITY` -
-Search With PERPLEXITY](#7-perplexity---search-with-perplexity) - [8. `OpenGPT`
- - chat With OPENGPT](#8-opengpt---chat-with-opengpt) - [9. `KOBOLDIA` -](#9-
-koboldia--) - [usage of special .LLM file from webscout (webscout.LLM)](#usage-
-   of-special-llm-file-from-webscout-webscoutllm) - [`LLM`](#llm) ## Install
-   ```python pip install -U webscout ``` ## CLI version ```python3 python -
-m webscout --help ``` | Command | Description | |------------------------------
--------------|-----------------------------------------------------------------
---------------------------------------| | python -m webscout answers -k Text |
-    CLI function to perform an answers search using Webscout. | | python -
-  m webscout images -k Text | CLI function to perform an images search using
-Webscout. | | python -m webscout maps -k Text | CLI function to perform a maps
- search using Webscout. | | python -m webscout news -k Text | CLI function to
-  perform a news search using Webscout. | | python -m webscout suggestions -
-   k Text | CLI function to perform a suggestions search using Webscout. | |
- python -m webscout text -k Text | CLI function to perform a text search using
- Webscout. | | python -m webscout translate -k Text | CLI function to perform
-   translate using Webscout. | | python -m webscout version | A command-line
-   interface command that prints and returns the version of the program. | |
-  python -m webscout videos -k Text | CLI function to perform a videos search
-using DuckDuckGo API. | ## CLI version of webscout.AI | Command | Description |
-|-----------------------------------------------|------------------------------
- --------------------------------------------------------------------------| |
-`python -m webscout.AI phindsearch --prompt "your search query"` | CLI function
-to perform a search query using Webscout.AI's Phindsearch feature. | | `python
--m webscout.AI yepchat --message "your_message_here"` | CLI function to send a
-message using Webscout.AI's Yepchat feature. | | `python -m webscout.AI youchat
- --prompt "your_prompt_here"` | CLI function to generate a response based on a
-prompt using Webscout.AI's Youchat feature. | | `python -m webscout.AI gemini -
- -message "tell me about gemma 7b"` | CLI function to get information about a
+ before-using-deepwebs) - [Usage Example](#usage-example) - [Text-to-Speech:]
+   (#text-to-speech) - [Available TTS Voices:](#available-tts-voices) - [ALL
+   voices:](#all-voices) - [WEBS and AsyncWEBS classes](#webs-and-asyncwebs-
+classes) - [Exceptions](#exceptions) - [usage of webscout](#usage-of-webscout)
+  - [1. `text()` - text search by DuckDuckGo.com and Yep.com](#1-text---text-
+  search-by-duckduckgocom-and-yepcom) - [2. `answers()` - instant answers by
+DuckDuckGo.com and Yep.com](#2-answers---instant-answers-by-duckduckgocom-and-
+  yepcom) - [3. `images()` - image search by DuckDuckGo.com and Yep.com](#3-
+  images---image-search-by-duckduckgocom-and-yepcom) - [4. `videos()` - video
+  search by DuckDuckGo.com](#4-videos---video-search-by-duckduckgocom) - [5.
+`news()` - news search by DuckDuckGo.com and yep.com](#5-news---news-search-by-
+ duckduckgocom-and-yepcom) - [6. `maps()` - map search by DuckDuckGo.com and]
+ (#6-maps---map-search-by-duckduckgocom-and) - [7. `translate()` - translation
+by DuckDuckGo.com and Yep.com](#7-translate---translation-by-duckduckgocom-and-
+yepcom) - [8. `suggestions()` - suggestions by DuckDuckGo.com and Yep.com](#8-
+suggestions---suggestions-by-duckduckgocom-and-yepcom) - [usage of webscout.AI]
+   (#usage-of-webscoutai) - [1. `PhindSearch` - Search using Phind.com](#1-
+ phindsearch---search-using-phindcom) - [2. `YepChat` - Chat with mistral 8x7b
+powered by yepchat](#2-yepchat---chat-with-mistral-8x7b-powered-by-yepchat) -
+  [3. `You.com` - search with you.com](#3-youcom---search-with-youcom) - [4.
+`Gemini` - search with google gemini](#4-gemini---search-with-google-gemini) -
+  [usage of image generator from Webscout.AI](#usage-of-image-generator-from-
+ webscoutai) - [5. `Prodia` - make image using prodia](#5-prodia---make-image-
+  using-prodia) - [6. `BlackBox` - Search/chat With BlackBox](#6-blackbox---
+  searchchat-with-blackbox) - [7. `PERPLEXITY` - Search With PERPLEXITY](#7-
+ perplexity---search-with-perplexity) - [8. `OpenGPT` - chat With OPENGPT](#8-
+  opengpt---chat-with-opengpt) - [9. `KOBOLDIA` -](#9-koboldia--) - [usage of
+  special .LLM file from webscout (webscout.LLM)](#usage-of-special-llm-file-
+ from-webscout-webscoutllm) - [`LLM`](#llm) ## Install ```python pip install -
+   U webscout ``` ## CLI version ```python3 python -m webscout --help ``` |
+Command | Description | |-------------------------------------------|----------
+-------------------------------------------------------------------------------
+--------------| | python -m webscout answers -k Text | CLI function to perform
+ an answers search using Webscout. | | python -m webscout images -k Text | CLI
+  function to perform an images search using Webscout. | | python -m webscout
+maps -k Text | CLI function to perform a maps search using Webscout. | | python
+    -m webscout news -k Text | CLI function to perform a news search using
+Webscout. | | python -m webscout suggestions -k Text | CLI function to perform
+a suggestions search using Webscout. | | python -m webscout text -k Text | CLI
+   function to perform a text search using Webscout. | | python -m webscout
+   translate -k Text | CLI function to perform translate using Webscout. | |
+ python -m webscout version | A command-line interface command that prints and
+returns the version of the program. | | python -m webscout videos -k Text | CLI
+ function to perform a videos search using DuckDuckGo API. | ## CLI version of
+webscout.AI | Command | Description | |----------------------------------------
+-------|-----------------------------------------------------------------------
+  ---------------------------------| | `python -m webscout.AI phindsearch --
+  prompt "your search query"` | CLI function to perform a search query using
+Webscout.AI's Phindsearch feature. | | `python -m webscout.AI yepchat --message
+   "your_message_here"` | CLI function to send a message using Webscout.AI's
+         Yepchat feature. | | `python -m webscout.AI youchat --prompt
+  "your_prompt_here"` | CLI function to generate a response based on a prompt
+   using Webscout.AI's Youchat feature. | | `python -m webscout.AI gemini --
+  message "tell me about gemma 7b"` | CLI function to get information about a
  specific topic using Webscout.AI's Gemini feature. | | `python -m webscout.AI
  prodia --prompt "car"` | CLI function to generate content related to a prompt
  using Webscout.AI's Prodia feature. | | `python -m webscout.AI blackboxai --
       prompt "Your prompt here"` | CLI function to perform a search using
 Webscout.AI's Blackbox search feature. | | `python -m webscout.AI perplexity --
       prompt "Your prompt here"` | CLI function to perform a search using
  Webscout.AI's PERPLEXITY feature. | | `python -m webscout.AI opengpt --prompt
@@ -163,57 +137,104 @@
 (search_params) return results def print_search_results(results): """ Print the
 search results. Args: - search_results (list): List of search results to print.
     """ if results: for index, result in enumerate(results, start=1): print
 (f"Result {index}: {result}") else: print("No search results found.") def main
    (): # Prompt the user for a search query query = input("Enter your search
 query: ") # Perform the web search results = perform_web_search(query) # Print
   the search results print_search_results(results) if __name__ == "__main__":
-  main() ``` ## WEBS and AsyncWEBS classes The WEBS and AsyncWEBS classes are
- used to retrieve search results from DuckDuckGo.com and yep.com periodically.
-   To use the AsyncWEBS class, you can perform asynchronous operations using
- Python's asyncio library. To initialize an instance of the WEBS or AsyncWEBS
- classes, you can provide the following optional arguments: Here is an example
- of initializing the WEBS class: ```python3 from webscout import WEBS R = WEBS
-().text("python programming", max_results=5) print(R) ``` Here is an example of
-  initializing the AsyncWEBS class: ```python3 import asyncio import logging
-   import sys from itertools import chain from random import shuffle import
-requests from webscout import AsyncWEBS # If you have proxies, define them here
-           proxies = None if sys.platform.lower().startswith("win"):
-  asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy()) def
- get_words(): word_site = "https://www.mit.edu/~ecprice/wordlist.10000" resp =
- requests.get(word_site) words = resp.text.splitlines() return words async def
- aget_results(word): async with AsyncWEBS(proxies=proxies) as WEBS: results =
-await WEBS.text(word, max_results=None) return results async def main(): words
- = get_words() shuffle(words) tasks = [aget_results(word) for word in words[:
-      10]] results = await asyncio.gather(*tasks) print(f"Done") for r in
-chain.from_iterable(results): print(r) logging.basicConfig(level=logging.DEBUG)
- await main() ``` It is important to note that the WEBS and AsyncWEBS classes
-   should always be used as a context manager (with statement). This ensures
-      proper resource management and cleanup, as the context manager will
-    automatically handle opening and closing the HTTP client connection. ##
-Exceptions Exceptions: - `WebscoutE`: Raised when there is a generic exception
- during the API request. ## usage of webscout ### 1. `text()` - text search by
- DuckDuckGo.com and Yep.com ```python from webscout import WEBS # Text search
- for 'live free or die' using DuckDuckGo.com and Yep.com with WEBS() as WEBS:
-   for r in WEBS.text('live free or die', region='wt-wt', safesearch='off',
-timelimit='y', max_results=10): print(r) for r in WEBS.text('live free or die',
-region='wt-wt', safesearch='off', timelimit='y', max_results=10): print(r) ```
- ### 2. `answers()` - instant answers by DuckDuckGo.com and Yep.com ```python
-     from webscout import WEBS # Instant answers for the query "sun" using
- DuckDuckGo.com and Yep.com with WEBS() as WEBS: for r in WEBS.answers("sun"):
-  print(r) ``` ### 3. `images()` - image search by DuckDuckGo.com and Yep.com
-```python from webscout import WEBS # Image search for the keyword 'butterfly'
- using DuckDuckGo.com and Yep.com with WEBS() as WEBS: keywords = 'butterfly'
-  WEBS_images_gen = WEBS.images( keywords, region="wt-wt", safesearch="off",
-size=None, type_image=None, layout=None, license_image=None, max_results=10, )
-  for r in WEBS_images_gen: print(r) ``` ### 4. `videos()` - video search by
-   DuckDuckGo.com ```python from webscout import WEBS # Video search for the
- keyword 'tesla' using DuckDuckGo.com with WEBS() as WEBS: keywords = 'tesla'
-  WEBS_videos_gen = WEBS.videos( keywords, region="wt-wt", safesearch="off",
-timelimit="w", resolution="high", duration="medium", max_results=10, ) for r in
+main() ``` ## Text-to-Speech: ```python from webscout import play_audio message
+ = "This is an example of text-to-speech." audio_content = play_audio(message,
+ voice="Brian") # Save the audio to a file with open("output.mp3", "wb") as f:
+f.write(audio_content) ``` ### Available TTS Voices: You can choose from a wide
+  range of voices, including: - Filiz, Astrid, Tatyana, Maxim, Carmen, Ines,
+Cristiano, Vitoria, Ricardo, Maja, Jan, Jacek, Ewa, Ruben, Lotte, Liv, Seoyeon,
+ Takumi, Mizuki, Giorgio, Carla, Bianca, Karl, Dora, Mathieu, Celine, Chantal,
+ Penelope, Miguel, Mia, Enrique, Conchita, Geraint, Salli, Matthew, Kimberly,
+ Kendra, Justin, Joey, Joanna, Ivy, Raveena, Aditi, Emma, Brian, Amy, Russell,
+Nicole, Vicki, Marlene, Hans, Naja, Mads, Gwyneth, Zhiyu - Standard and WaveNet
+voices for various languages (e.g., en-US, es-ES, ja-JP, etc.) ### ALL voices:
+  [Filiz, Astrid, Tatyana, Maxim, Carmen, Ines, Cristiano, Vitoria, Ricardo,
+  Maja, Jan, Jacek, Ewa, Ruben, Lotte, Liv, Seoyeon, Takumi, Mizuki, Giorgio,
+  Carla, Bianca, Karl, Dora, Mathieu, Celine, Chantal, Penelope, Miguel, Mia,
+  Enrique, Conchita, Geraint, Salli, Matthew, Kimberly, Kendra, Justin, Joey,
+Joanna, Ivy, Raveena, Aditi, Emma, Brian, Amy, Russell, Nicole, Vicki, Marlene,
+ Hans, Naja, Mads, Gwyneth, Zhiyu, es-ES-Standard-A, it-IT-Standard-A, it-IT-
+Wavenet-A, ja-JP-Standard-A, ja-JP-Wavenet-A, ko-KR-Standard-A, ko-KR-Wavenet-
+A, pt-BR-Standard-A, tr-TR-Standard-A, sv-SE-Standard-A, nl-NL-Standard-A, nl-
+NL-Wavenet-A, en-US-Wavenet-A, en-US-Wavenet-B, en-US-Wavenet-C, en-US-Wavenet-
+D, en-US-Wavenet-E, en-US-Wavenet-F, en-GB-Standard-A, en-GB-Standard-B, en-GB-
+Standard-C, en-GB-Standard-D, en-GB-Wavenet-A, en-GB-Wavenet-B, en-GB-Wavenet-
+ C, en-GB-Wavenet-D, en-US-Standard-B, en-US-Standard-C, en-US-Standard-D, en-
+  US-Standard-E, de-DE-Standard-A, de-DE-Standard-B, de-DE-Wavenet-A, de-DE-
+Wavenet-B, de-DE-Wavenet-C, de-DE-Wavenet-D, en-AU-Standard-A, en-AU-Standard-
+ B, en-AU-Wavenet-A, en-AU-Wavenet-B, en-AU-Wavenet-C, en-AU-Wavenet-D, en-AU-
+   Standard-C, en-AU-Standard-D, fr-CA-Standard-A, fr-CA-Standard-B, fr-CA-
+   Standard-C, fr-CA-Standard-D, fr-FR-Standard-C, fr-FR-Standard-D, fr-FR-
+Wavenet-A, fr-FR-Wavenet-B, fr-FR-Wavenet-C, fr-FR-Wavenet-D, da-DK-Wavenet-A,
+  pl-PL-Wavenet-A, pl-PL-Wavenet-B, pl-PL-Wavenet-C, pl-PL-Wavenet-D, pt-PT-
+Wavenet-A, pt-PT-Wavenet-B, pt-PT-Wavenet-C, pt-PT-Wavenet-D, ru-RU-Wavenet-A,
+  ru-RU-Wavenet-B, ru-RU-Wavenet-C, ru-RU-Wavenet-D, sk-SK-Wavenet-A, tr-TR-
+Wavenet-A, tr-TR-Wavenet-B, tr-TR-Wavenet-C, tr-TR-Wavenet-D, tr-TR-Wavenet-E,
+  uk-UA-Wavenet-A, ar-XA-Wavenet-A, ar-XA-Wavenet-B, ar-XA-Wavenet-C, cs-CZ-
+Wavenet-A, nl-NL-Wavenet-B, nl-NL-Wavenet-C, nl-NL-Wavenet-D, nl-NL-Wavenet-E,
+  en-IN-Wavenet-A, en-IN-Wavenet-B, en-IN-Wavenet-C, fil-PH-Wavenet-A, fi-FI-
+Wavenet-A, el-GR-Wavenet-A, hi-IN-Wavenet-A, hi-IN-Wavenet-B, hi-IN-Wavenet-C,
+  hu-HU-Wavenet-A, id-ID-Wavenet-A, id-ID-Wavenet-B, id-ID-Wavenet-C, it-IT-
+Wavenet-B, it-IT-Wavenet-C, it-IT-Wavenet-D, ja-JP-Wavenet-B, ja-JP-Wavenet-C,
+ja-JP-Wavenet-D, cmn-CN-Wavenet-A, cmn-CN-Wavenet-B, cmn-CN-Wavenet-C, cmn-CN-
+Wavenet-D, nb-no-Wavenet-E, nb-no-Wavenet-A, nb-no-Wavenet-B, nb-no-Wavenet-C,
+  nb-no-Wavenet-D, vi-VN-Wavenet-A, vi-VN-Wavenet-B, vi-VN-Wavenet-C, vi-VN-
+    Wavenet-D, sr-rs-Standard-A, lv-lv-Standard-A, is-is-Standard-A, bg-bg-
+ Standard-A, af-ZA-Standard-A, Tracy, Danny, Huihui, Yaoyao, Kangkang, HanHan,
+Zhiwei, Asaf, An, Stefanos, Filip, Ivan, Heidi, Herena, Kalpana, Hemant, Matej,
+    Andika, Rizwan, Lado, Valluvar, Linda, Heather, Sean, Michael, Karsten,
+Guillaume, Pattara, Jakub, Szabolcs, Hoda, Naayf] ## WEBS and AsyncWEBS classes
+    The WEBS and AsyncWEBS classes are used to retrieve search results from
+ DuckDuckGo.com and yep.com periodically. To use the AsyncWEBS class, you can
+ perform asynchronous operations using Python's asyncio library. To initialize
+  an instance of the WEBS or AsyncWEBS classes, you can provide the following
+    optional arguments: Here is an example of initializing the WEBS class:
+  ```python3 from webscout import WEBS R = WEBS().text("python programming",
+ max_results=5) print(R) ``` Here is an example of initializing the AsyncWEBS
+   class: ```python3 import asyncio import logging import sys from itertools
+ import chain from random import shuffle import requests from webscout import
+      AsyncWEBS # If you have proxies, define them here proxies = None if
+     sys.platform.lower().startswith("win"): asyncio.set_event_loop_policy
+(asyncio.WindowsSelectorEventLoopPolicy()) def get_words(): word_site = "https:
+ //www.mit.edu/~ecprice/wordlist.10000" resp = requests.get(word_site) words =
+ resp.text.splitlines() return words async def aget_results(word): async with
+      AsyncWEBS(proxies=proxies) as WEBS: results = await WEBS.text(word,
+max_results=None) return results async def main(): words = get_words() shuffle
+  (words) tasks = [aget_results(word) for word in words[:10]] results = await
+ asyncio.gather(*tasks) print(f"Done") for r in chain.from_iterable(results):
+   print(r) logging.basicConfig(level=logging.DEBUG) await main() ``` It is
+important to note that the WEBS and AsyncWEBS classes should always be used as
+a context manager (with statement). This ensures proper resource management and
+ cleanup, as the context manager will automatically handle opening and closing
+  the HTTP client connection. ## Exceptions Exceptions: - `WebscoutE`: Raised
+when there is a generic exception during the API request. ## usage of webscout
+  ### 1. `text()` - text search by DuckDuckGo.com and Yep.com ```python from
+webscout import WEBS # Text search for 'live free or die' using DuckDuckGo.com
+    and Yep.com with WEBS() as WEBS: for r in WEBS.text('live free or die',
+region='wt-wt', safesearch='off', timelimit='y', max_results=10): print(r) for
+     r in WEBS.text('live free or die', region='wt-wt', safesearch='off',
+   timelimit='y', max_results=10): print(r) ``` ### 2. `answers()` - instant
+  answers by DuckDuckGo.com and Yep.com ```python from webscout import WEBS #
+Instant answers for the query "sun" using DuckDuckGo.com and Yep.com with WEBS
+  () as WEBS: for r in WEBS.answers("sun"): print(r) ``` ### 3. `images()` -
+image search by DuckDuckGo.com and Yep.com ```python from webscout import WEBS
+  # Image search for the keyword 'butterfly' using DuckDuckGo.com and Yep.com
+   with WEBS() as WEBS: keywords = 'butterfly' WEBS_images_gen = WEBS.images
+   ( keywords, region="wt-wt", safesearch="off", size=None, type_image=None,
+ layout=None, license_image=None, max_results=10, ) for r in WEBS_images_gen:
+print(r) ``` ### 4. `videos()` - video search by DuckDuckGo.com ```python from
+       webscout import WEBS # Video search for the keyword 'tesla' using
+   DuckDuckGo.com with WEBS() as WEBS: keywords = 'tesla' WEBS_videos_gen =
+    WEBS.videos( keywords, region="wt-wt", safesearch="off", timelimit="w",
+       resolution="high", duration="medium", max_results=10, ) for r in
  WEBS_videos_gen: print(r) ``` ### 5. `news()` - news search by DuckDuckGo.com
  and yep.com ```python from webscout import WEBS # News search for the keyword
   'holiday' using DuckDuckGo.com and yep.com with WEBS() as WEBS: keywords =
         'holiday' WEBS_news_gen = WEBS.news( keywords, region="wt-wt",
 safesearch="off", timelimit="m", max_results=20 ) for r in WEBS_news_gen: print
    (r) ``` ### 6. `maps()` - map search by DuckDuckGo.com and ```python from
 webscout import WEBS # Map search for the keyword 'school' in 'anantnag' using
```

### Comparing `webscout-1.2.9/setup.py` & `webscout-1.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 #     exec(version_file.read())
 
 with open("README.md", encoding="utf-8") as f:
     README = f.read()
 
 setup(
     name="webscout",
-    version="1.2.9", 
+    version="1.3.0", 
     description="Search for words, documents, images, videos, news, maps and text translation using the Google, DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models and now can transcribe yt videos",
     long_description=README,
     long_description_content_type="text/markdown",
     author="OEvortex",
     author_email="helpingai5@gmail.com",
     packages=find_packages(),
     classifiers=[
```

### Comparing `webscout-1.2.9/webscout/AI.py` & `webscout-1.3.0/webscout/AI.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.9/webscout/AIbase.py` & `webscout-1.3.0/webscout/AIbase.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.9/webscout/AIutel.py` & `webscout-1.3.0/webscout/AIutel.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.9/webscout/DWEBS.py` & `webscout-1.3.0/webscout/DWEBS.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.9/webscout/HelpingAI.py` & `webscout-1.3.0/webscout/HelpingAI.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.9/webscout/LLM.py` & `webscout-1.3.0/webscout/LLM.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.9/webscout/__init__.py` & `webscout-1.3.0/webscout/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -6,12 +6,13 @@
 
 import logging
 from .webscout_search import WEBS
 from .webscout_search_async import AsyncWEBS
 from .version import __version__
 from .DWEBS import DeepWEBS
 from .transcriber import transcriber
+from .voice import play_audio
 
 
 __all__ = ["WEBS", "AsyncWEBS", "__version__", "cli"]
 
 logging.getLogger("webscout").addHandler(logging.NullHandler())
```

### Comparing `webscout-1.2.9/webscout/cli.py` & `webscout-1.3.0/webscout/cli.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.9/webscout/models.py` & `webscout-1.3.0/webscout/models.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.9/webscout/transcriber.py` & `webscout-1.3.0/webscout/transcriber.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.9/webscout/utils.py` & `webscout-1.3.0/webscout/utils.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.9/webscout/webscout_search.py` & `webscout-1.3.0/webscout/webscout_search.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.9/webscout/webscout_search_async.py` & `webscout-1.3.0/webscout/webscout_search_async.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.9/webscout.egg-info/PKG-INFO` & `webscout-1.3.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webscout
-Version: 1.2.9
+Version: 1.3.0
 Summary: Search for words, documents, images, videos, news, maps and text translation using the Google, DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models and now can transcribe yt videos
 Author: OEvortex
 Author-email: helpingai5@gmail.com
 License: HelpingAI Simplified Universal License
 Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
 Project-URL: Source, https://github.com/OE-LUCIFER/Webscout
 Project-URL: Tracker, https://github.com/OE-LUCIFER/Webscout/issues
@@ -68,14 +68,17 @@
   - [CLI to use LLM](#cli-to-use-llm)
   - [Regions](#regions)
   - [Transcriber](#transcriber)
   - [DeepWEBS: Advanced Web Searches](#deepwebs-advanced-web-searches)
     - [Activating DeepWEBS](#activating-deepwebs)
     - [Point to remember before using `DeepWEBS`](#point-to-remember-before-using-deepwebs)
     - [Usage Example](#usage-example)
+  - [Text-to-Speech:](#text-to-speech)
+    - [Available TTS Voices:](#available-tts-voices)
+    - [ALL voices:](#all-voices)
   - [WEBS and AsyncWEBS classes](#webs-and-asyncwebs-classes)
   - [Exceptions](#exceptions)
   - [usage of webscout](#usage-of-webscout)
     - [1. `text()` - text search by DuckDuckGo.com and Yep.com](#1-text---text-search-by-duckduckgocom-and-yepcom)
     - [2. `answers()` - instant answers by DuckDuckGo.com and Yep.com](#2-answers---instant-answers-by-duckduckgocom-and-yepcom)
     - [3. `images()` - image search by DuckDuckGo.com and Yep.com](#3-images---image-search-by-duckduckgocom-and-yepcom)
     - [4. `videos()` - video search by DuckDuckGo.com](#4-videos---video-search-by-duckduckgocom)
@@ -333,14 +336,31 @@
     # Print the search results
     print_search_results(results)
 
 if __name__ == "__main__":
     main()
 
 ```
+## Text-to-Speech:
+```python
+from webscout import play_audio
+
+message = "This is an example of text-to-speech."
+audio_content = play_audio(message, voice="Brian")
+
+# Save the audio to a file
+with open("output.mp3", "wb") as f:
+    f.write(audio_content)
+```
+### Available TTS Voices:
+You can choose from a wide range of voices, including:
+- Filiz, Astrid, Tatyana, Maxim, Carmen, Ines, Cristiano, Vitoria, Ricardo, Maja, Jan, Jacek, Ewa, Ruben, Lotte, Liv, Seoyeon, Takumi, Mizuki, Giorgio, Carla, Bianca, Karl, Dora, Mathieu, Celine, Chantal, Penelope, Miguel, Mia, Enrique, Conchita, Geraint, Salli, Matthew, Kimberly, Kendra, Justin, Joey, Joanna, Ivy, Raveena, Aditi, Emma, Brian, Amy, Russell, Nicole, Vicki, Marlene, Hans, Naja, Mads, Gwyneth, Zhiyu
+- Standard and WaveNet voices for various languages (e.g., en-US, es-ES, ja-JP, etc.)
+### ALL voices:
+[Filiz, Astrid, Tatyana, Maxim, Carmen, Ines, Cristiano, Vitoria, Ricardo, Maja, Jan, Jacek, Ewa, Ruben, Lotte, Liv, Seoyeon, Takumi, Mizuki, Giorgio, Carla, Bianca, Karl, Dora, Mathieu, Celine, Chantal, Penelope, Miguel, Mia, Enrique, Conchita, Geraint, Salli, Matthew, Kimberly, Kendra, Justin, Joey, Joanna, Ivy, Raveena, Aditi, Emma, Brian, Amy, Russell, Nicole, Vicki, Marlene, Hans, Naja, Mads, Gwyneth, Zhiyu, es-ES-Standard-A, it-IT-Standard-A, it-IT-Wavenet-A, ja-JP-Standard-A, ja-JP-Wavenet-A, ko-KR-Standard-A, ko-KR-Wavenet-A, pt-BR-Standard-A, tr-TR-Standard-A, sv-SE-Standard-A, nl-NL-Standard-A, nl-NL-Wavenet-A, en-US-Wavenet-A, en-US-Wavenet-B, en-US-Wavenet-C, en-US-Wavenet-D, en-US-Wavenet-E, en-US-Wavenet-F, en-GB-Standard-A, en-GB-Standard-B, en-GB-Standard-C, en-GB-Standard-D, en-GB-Wavenet-A, en-GB-Wavenet-B, en-GB-Wavenet-C, en-GB-Wavenet-D, en-US-Standard-B, en-US-Standard-C, en-US-Standard-D, en-US-Standard-E, de-DE-Standard-A, de-DE-Standard-B, de-DE-Wavenet-A, de-DE-Wavenet-B, de-DE-Wavenet-C, de-DE-Wavenet-D, en-AU-Standard-A, en-AU-Standard-B, en-AU-Wavenet-A, en-AU-Wavenet-B, en-AU-Wavenet-C, en-AU-Wavenet-D, en-AU-Standard-C, en-AU-Standard-D, fr-CA-Standard-A, fr-CA-Standard-B, fr-CA-Standard-C, fr-CA-Standard-D, fr-FR-Standard-C, fr-FR-Standard-D, fr-FR-Wavenet-A, fr-FR-Wavenet-B, fr-FR-Wavenet-C, fr-FR-Wavenet-D, da-DK-Wavenet-A, pl-PL-Wavenet-A, pl-PL-Wavenet-B, pl-PL-Wavenet-C, pl-PL-Wavenet-D, pt-PT-Wavenet-A, pt-PT-Wavenet-B, pt-PT-Wavenet-C, pt-PT-Wavenet-D, ru-RU-Wavenet-A, ru-RU-Wavenet-B, ru-RU-Wavenet-C, ru-RU-Wavenet-D, sk-SK-Wavenet-A, tr-TR-Wavenet-A, tr-TR-Wavenet-B, tr-TR-Wavenet-C, tr-TR-Wavenet-D, tr-TR-Wavenet-E, uk-UA-Wavenet-A, ar-XA-Wavenet-A, ar-XA-Wavenet-B, ar-XA-Wavenet-C, cs-CZ-Wavenet-A, nl-NL-Wavenet-B, nl-NL-Wavenet-C, nl-NL-Wavenet-D, nl-NL-Wavenet-E, en-IN-Wavenet-A, en-IN-Wavenet-B, en-IN-Wavenet-C, fil-PH-Wavenet-A, fi-FI-Wavenet-A, el-GR-Wavenet-A, hi-IN-Wavenet-A, hi-IN-Wavenet-B, hi-IN-Wavenet-C, hu-HU-Wavenet-A, id-ID-Wavenet-A, id-ID-Wavenet-B, id-ID-Wavenet-C, it-IT-Wavenet-B, it-IT-Wavenet-C, it-IT-Wavenet-D, ja-JP-Wavenet-B, ja-JP-Wavenet-C, ja-JP-Wavenet-D, cmn-CN-Wavenet-A, cmn-CN-Wavenet-B, cmn-CN-Wavenet-C, cmn-CN-Wavenet-D, nb-no-Wavenet-E, nb-no-Wavenet-A, nb-no-Wavenet-B, nb-no-Wavenet-C, nb-no-Wavenet-D, vi-VN-Wavenet-A, vi-VN-Wavenet-B, vi-VN-Wavenet-C, vi-VN-Wavenet-D, sr-rs-Standard-A, lv-lv-Standard-A, is-is-Standard-A, bg-bg-Standard-A, af-ZA-Standard-A, Tracy, Danny, Huihui, Yaoyao, Kangkang, HanHan, Zhiwei, Asaf, An, Stefanos, Filip, Ivan, Heidi, Herena, Kalpana, Hemant, Matej, Andika, Rizwan, Lado, Valluvar, Linda, Heather, Sean, Michael, Karsten, Guillaume, Pattara, Jakub, Szabolcs, Hoda, Naayf]
 ## WEBS and AsyncWEBS classes
 
 The WEBS and AsyncWEBS classes are used to retrieve search results from DuckDuckGo.com and yep.com periodically.
 To use the AsyncWEBS class, you can perform asynchronous operations using Python's asyncio library.
 To initialize an instance of the WEBS or AsyncWEBS classes, you can provide the following optional arguments:
 
 Here is an example of initializing the WEBS class:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: webscout Version: 1.2.9 Summary: Search for words,
+Metadata-Version: 2.1 Name: webscout Version: 1.3.0 Summary: Search for words,
 documents, images, videos, news, maps and text translation using the Google,
 DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models and
 now can transcribe yt videos Author: OEvortex Author-email:
 helpingai5@gmail.com License: HelpingAI Simplified Universal License Project-
 URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki Project-URL:
 Source, https://github.com/OE-LUCIFER/Webscout Project-URL: Tracker, https://
 github.com/OE-LUCIFER/Webscout/issues Project-URL: YouTube, https://
@@ -32,66 +32,68 @@
 you.com, etc Also containes AI models and now can transcribe yt videos ## Table
 of Contents - [webscout](#webscout) - [Table of Contents](#table-of-contents) -
       [Install](#install) - [CLI version](#cli-version) - [CLI version of
 webscout.AI](#cli-version-of-webscoutai) - [CLI to use LLM](#cli-to-use-llm) -
   [Regions](#regions) - [Transcriber](#transcriber) - [DeepWEBS: Advanced Web
 Searches](#deepwebs-advanced-web-searches) - [Activating DeepWEBS](#activating-
   deepwebs) - [Point to remember before using `DeepWEBS`](#point-to-remember-
-before-using-deepwebs) - [Usage Example](#usage-example) - [WEBS and AsyncWEBS
- classes](#webs-and-asyncwebs-classes) - [Exceptions](#exceptions) - [usage of
- webscout](#usage-of-webscout) - [1. `text()` - text search by DuckDuckGo.com
-and Yep.com](#1-text---text-search-by-duckduckgocom-and-yepcom) - [2. `answers
-  ()` - instant answers by DuckDuckGo.com and Yep.com](#2-answers---instant-
-    answers-by-duckduckgocom-and-yepcom) - [3. `images()` - image search by
-  DuckDuckGo.com and Yep.com](#3-images---image-search-by-duckduckgocom-and-
- yepcom) - [4. `videos()` - video search by DuckDuckGo.com](#4-videos---video-
-  search-by-duckduckgocom) - [5. `news()` - news search by DuckDuckGo.com and
- yep.com](#5-news---news-search-by-duckduckgocom-and-yepcom) - [6. `maps()` -
-map search by DuckDuckGo.com and](#6-maps---map-search-by-duckduckgocom-and) -
-[7. `translate()` - translation by DuckDuckGo.com and Yep.com](#7-translate---
-translation-by-duckduckgocom-and-yepcom) - [8. `suggestions()` - suggestions by
-DuckDuckGo.com and Yep.com](#8-suggestions---suggestions-by-duckduckgocom-and-
- yepcom) - [usage of webscout.AI](#usage-of-webscoutai) - [1. `PhindSearch` -
-Search using Phind.com](#1-phindsearch---search-using-phindcom) - [2. `YepChat`
- - Chat with mistral 8x7b powered by yepchat](#2-yepchat---chat-with-mistral-
- 8x7b-powered-by-yepchat) - [3. `You.com` - search with you.com](#3-youcom---
- search-with-youcom) - [4. `Gemini` - search with google gemini](#4-gemini---
-   search-with-google-gemini) - [usage of image generator from Webscout.AI]
- (#usage-of-image-generator-from-webscoutai) - [5. `Prodia` - make image using
-  prodia](#5-prodia---make-image-using-prodia) - [6. `BlackBox` - Search/chat
-  With BlackBox](#6-blackbox---searchchat-with-blackbox) - [7. `PERPLEXITY` -
-Search With PERPLEXITY](#7-perplexity---search-with-perplexity) - [8. `OpenGPT`
- - chat With OPENGPT](#8-opengpt---chat-with-opengpt) - [9. `KOBOLDIA` -](#9-
-koboldia--) - [usage of special .LLM file from webscout (webscout.LLM)](#usage-
-   of-special-llm-file-from-webscout-webscoutllm) - [`LLM`](#llm) ## Install
-   ```python pip install -U webscout ``` ## CLI version ```python3 python -
-m webscout --help ``` | Command | Description | |------------------------------
--------------|-----------------------------------------------------------------
---------------------------------------| | python -m webscout answers -k Text |
-    CLI function to perform an answers search using Webscout. | | python -
-  m webscout images -k Text | CLI function to perform an images search using
-Webscout. | | python -m webscout maps -k Text | CLI function to perform a maps
- search using Webscout. | | python -m webscout news -k Text | CLI function to
-  perform a news search using Webscout. | | python -m webscout suggestions -
-   k Text | CLI function to perform a suggestions search using Webscout. | |
- python -m webscout text -k Text | CLI function to perform a text search using
- Webscout. | | python -m webscout translate -k Text | CLI function to perform
-   translate using Webscout. | | python -m webscout version | A command-line
-   interface command that prints and returns the version of the program. | |
-  python -m webscout videos -k Text | CLI function to perform a videos search
-using DuckDuckGo API. | ## CLI version of webscout.AI | Command | Description |
-|-----------------------------------------------|------------------------------
- --------------------------------------------------------------------------| |
-`python -m webscout.AI phindsearch --prompt "your search query"` | CLI function
-to perform a search query using Webscout.AI's Phindsearch feature. | | `python
--m webscout.AI yepchat --message "your_message_here"` | CLI function to send a
-message using Webscout.AI's Yepchat feature. | | `python -m webscout.AI youchat
- --prompt "your_prompt_here"` | CLI function to generate a response based on a
-prompt using Webscout.AI's Youchat feature. | | `python -m webscout.AI gemini -
- -message "tell me about gemma 7b"` | CLI function to get information about a
+ before-using-deepwebs) - [Usage Example](#usage-example) - [Text-to-Speech:]
+   (#text-to-speech) - [Available TTS Voices:](#available-tts-voices) - [ALL
+   voices:](#all-voices) - [WEBS and AsyncWEBS classes](#webs-and-asyncwebs-
+classes) - [Exceptions](#exceptions) - [usage of webscout](#usage-of-webscout)
+  - [1. `text()` - text search by DuckDuckGo.com and Yep.com](#1-text---text-
+  search-by-duckduckgocom-and-yepcom) - [2. `answers()` - instant answers by
+DuckDuckGo.com and Yep.com](#2-answers---instant-answers-by-duckduckgocom-and-
+  yepcom) - [3. `images()` - image search by DuckDuckGo.com and Yep.com](#3-
+  images---image-search-by-duckduckgocom-and-yepcom) - [4. `videos()` - video
+  search by DuckDuckGo.com](#4-videos---video-search-by-duckduckgocom) - [5.
+`news()` - news search by DuckDuckGo.com and yep.com](#5-news---news-search-by-
+ duckduckgocom-and-yepcom) - [6. `maps()` - map search by DuckDuckGo.com and]
+ (#6-maps---map-search-by-duckduckgocom-and) - [7. `translate()` - translation
+by DuckDuckGo.com and Yep.com](#7-translate---translation-by-duckduckgocom-and-
+yepcom) - [8. `suggestions()` - suggestions by DuckDuckGo.com and Yep.com](#8-
+suggestions---suggestions-by-duckduckgocom-and-yepcom) - [usage of webscout.AI]
+   (#usage-of-webscoutai) - [1. `PhindSearch` - Search using Phind.com](#1-
+ phindsearch---search-using-phindcom) - [2. `YepChat` - Chat with mistral 8x7b
+powered by yepchat](#2-yepchat---chat-with-mistral-8x7b-powered-by-yepchat) -
+  [3. `You.com` - search with you.com](#3-youcom---search-with-youcom) - [4.
+`Gemini` - search with google gemini](#4-gemini---search-with-google-gemini) -
+  [usage of image generator from Webscout.AI](#usage-of-image-generator-from-
+ webscoutai) - [5. `Prodia` - make image using prodia](#5-prodia---make-image-
+  using-prodia) - [6. `BlackBox` - Search/chat With BlackBox](#6-blackbox---
+  searchchat-with-blackbox) - [7. `PERPLEXITY` - Search With PERPLEXITY](#7-
+ perplexity---search-with-perplexity) - [8. `OpenGPT` - chat With OPENGPT](#8-
+  opengpt---chat-with-opengpt) - [9. `KOBOLDIA` -](#9-koboldia--) - [usage of
+  special .LLM file from webscout (webscout.LLM)](#usage-of-special-llm-file-
+ from-webscout-webscoutllm) - [`LLM`](#llm) ## Install ```python pip install -
+   U webscout ``` ## CLI version ```python3 python -m webscout --help ``` |
+Command | Description | |-------------------------------------------|----------
+-------------------------------------------------------------------------------
+--------------| | python -m webscout answers -k Text | CLI function to perform
+ an answers search using Webscout. | | python -m webscout images -k Text | CLI
+  function to perform an images search using Webscout. | | python -m webscout
+maps -k Text | CLI function to perform a maps search using Webscout. | | python
+    -m webscout news -k Text | CLI function to perform a news search using
+Webscout. | | python -m webscout suggestions -k Text | CLI function to perform
+a suggestions search using Webscout. | | python -m webscout text -k Text | CLI
+   function to perform a text search using Webscout. | | python -m webscout
+   translate -k Text | CLI function to perform translate using Webscout. | |
+ python -m webscout version | A command-line interface command that prints and
+returns the version of the program. | | python -m webscout videos -k Text | CLI
+ function to perform a videos search using DuckDuckGo API. | ## CLI version of
+webscout.AI | Command | Description | |----------------------------------------
+-------|-----------------------------------------------------------------------
+  ---------------------------------| | `python -m webscout.AI phindsearch --
+  prompt "your search query"` | CLI function to perform a search query using
+Webscout.AI's Phindsearch feature. | | `python -m webscout.AI yepchat --message
+   "your_message_here"` | CLI function to send a message using Webscout.AI's
+         Yepchat feature. | | `python -m webscout.AI youchat --prompt
+  "your_prompt_here"` | CLI function to generate a response based on a prompt
+   using Webscout.AI's Youchat feature. | | `python -m webscout.AI gemini --
+  message "tell me about gemma 7b"` | CLI function to get information about a
  specific topic using Webscout.AI's Gemini feature. | | `python -m webscout.AI
  prodia --prompt "car"` | CLI function to generate content related to a prompt
  using Webscout.AI's Prodia feature. | | `python -m webscout.AI blackboxai --
       prompt "Your prompt here"` | CLI function to perform a search using
 Webscout.AI's Blackbox search feature. | | `python -m webscout.AI perplexity --
       prompt "Your prompt here"` | CLI function to perform a search using
  Webscout.AI's PERPLEXITY feature. | | `python -m webscout.AI opengpt --prompt
@@ -163,57 +165,104 @@
 (search_params) return results def print_search_results(results): """ Print the
 search results. Args: - search_results (list): List of search results to print.
     """ if results: for index, result in enumerate(results, start=1): print
 (f"Result {index}: {result}") else: print("No search results found.") def main
    (): # Prompt the user for a search query query = input("Enter your search
 query: ") # Perform the web search results = perform_web_search(query) # Print
   the search results print_search_results(results) if __name__ == "__main__":
-  main() ``` ## WEBS and AsyncWEBS classes The WEBS and AsyncWEBS classes are
- used to retrieve search results from DuckDuckGo.com and yep.com periodically.
-   To use the AsyncWEBS class, you can perform asynchronous operations using
- Python's asyncio library. To initialize an instance of the WEBS or AsyncWEBS
- classes, you can provide the following optional arguments: Here is an example
- of initializing the WEBS class: ```python3 from webscout import WEBS R = WEBS
-().text("python programming", max_results=5) print(R) ``` Here is an example of
-  initializing the AsyncWEBS class: ```python3 import asyncio import logging
-   import sys from itertools import chain from random import shuffle import
-requests from webscout import AsyncWEBS # If you have proxies, define them here
-           proxies = None if sys.platform.lower().startswith("win"):
-  asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy()) def
- get_words(): word_site = "https://www.mit.edu/~ecprice/wordlist.10000" resp =
- requests.get(word_site) words = resp.text.splitlines() return words async def
- aget_results(word): async with AsyncWEBS(proxies=proxies) as WEBS: results =
-await WEBS.text(word, max_results=None) return results async def main(): words
- = get_words() shuffle(words) tasks = [aget_results(word) for word in words[:
-      10]] results = await asyncio.gather(*tasks) print(f"Done") for r in
-chain.from_iterable(results): print(r) logging.basicConfig(level=logging.DEBUG)
- await main() ``` It is important to note that the WEBS and AsyncWEBS classes
-   should always be used as a context manager (with statement). This ensures
-      proper resource management and cleanup, as the context manager will
-    automatically handle opening and closing the HTTP client connection. ##
-Exceptions Exceptions: - `WebscoutE`: Raised when there is a generic exception
- during the API request. ## usage of webscout ### 1. `text()` - text search by
- DuckDuckGo.com and Yep.com ```python from webscout import WEBS # Text search
- for 'live free or die' using DuckDuckGo.com and Yep.com with WEBS() as WEBS:
-   for r in WEBS.text('live free or die', region='wt-wt', safesearch='off',
-timelimit='y', max_results=10): print(r) for r in WEBS.text('live free or die',
-region='wt-wt', safesearch='off', timelimit='y', max_results=10): print(r) ```
- ### 2. `answers()` - instant answers by DuckDuckGo.com and Yep.com ```python
-     from webscout import WEBS # Instant answers for the query "sun" using
- DuckDuckGo.com and Yep.com with WEBS() as WEBS: for r in WEBS.answers("sun"):
-  print(r) ``` ### 3. `images()` - image search by DuckDuckGo.com and Yep.com
-```python from webscout import WEBS # Image search for the keyword 'butterfly'
- using DuckDuckGo.com and Yep.com with WEBS() as WEBS: keywords = 'butterfly'
-  WEBS_images_gen = WEBS.images( keywords, region="wt-wt", safesearch="off",
-size=None, type_image=None, layout=None, license_image=None, max_results=10, )
-  for r in WEBS_images_gen: print(r) ``` ### 4. `videos()` - video search by
-   DuckDuckGo.com ```python from webscout import WEBS # Video search for the
- keyword 'tesla' using DuckDuckGo.com with WEBS() as WEBS: keywords = 'tesla'
-  WEBS_videos_gen = WEBS.videos( keywords, region="wt-wt", safesearch="off",
-timelimit="w", resolution="high", duration="medium", max_results=10, ) for r in
+main() ``` ## Text-to-Speech: ```python from webscout import play_audio message
+ = "This is an example of text-to-speech." audio_content = play_audio(message,
+ voice="Brian") # Save the audio to a file with open("output.mp3", "wb") as f:
+f.write(audio_content) ``` ### Available TTS Voices: You can choose from a wide
+  range of voices, including: - Filiz, Astrid, Tatyana, Maxim, Carmen, Ines,
+Cristiano, Vitoria, Ricardo, Maja, Jan, Jacek, Ewa, Ruben, Lotte, Liv, Seoyeon,
+ Takumi, Mizuki, Giorgio, Carla, Bianca, Karl, Dora, Mathieu, Celine, Chantal,
+ Penelope, Miguel, Mia, Enrique, Conchita, Geraint, Salli, Matthew, Kimberly,
+ Kendra, Justin, Joey, Joanna, Ivy, Raveena, Aditi, Emma, Brian, Amy, Russell,
+Nicole, Vicki, Marlene, Hans, Naja, Mads, Gwyneth, Zhiyu - Standard and WaveNet
+voices for various languages (e.g., en-US, es-ES, ja-JP, etc.) ### ALL voices:
+  [Filiz, Astrid, Tatyana, Maxim, Carmen, Ines, Cristiano, Vitoria, Ricardo,
+  Maja, Jan, Jacek, Ewa, Ruben, Lotte, Liv, Seoyeon, Takumi, Mizuki, Giorgio,
+  Carla, Bianca, Karl, Dora, Mathieu, Celine, Chantal, Penelope, Miguel, Mia,
+  Enrique, Conchita, Geraint, Salli, Matthew, Kimberly, Kendra, Justin, Joey,
+Joanna, Ivy, Raveena, Aditi, Emma, Brian, Amy, Russell, Nicole, Vicki, Marlene,
+ Hans, Naja, Mads, Gwyneth, Zhiyu, es-ES-Standard-A, it-IT-Standard-A, it-IT-
+Wavenet-A, ja-JP-Standard-A, ja-JP-Wavenet-A, ko-KR-Standard-A, ko-KR-Wavenet-
+A, pt-BR-Standard-A, tr-TR-Standard-A, sv-SE-Standard-A, nl-NL-Standard-A, nl-
+NL-Wavenet-A, en-US-Wavenet-A, en-US-Wavenet-B, en-US-Wavenet-C, en-US-Wavenet-
+D, en-US-Wavenet-E, en-US-Wavenet-F, en-GB-Standard-A, en-GB-Standard-B, en-GB-
+Standard-C, en-GB-Standard-D, en-GB-Wavenet-A, en-GB-Wavenet-B, en-GB-Wavenet-
+ C, en-GB-Wavenet-D, en-US-Standard-B, en-US-Standard-C, en-US-Standard-D, en-
+  US-Standard-E, de-DE-Standard-A, de-DE-Standard-B, de-DE-Wavenet-A, de-DE-
+Wavenet-B, de-DE-Wavenet-C, de-DE-Wavenet-D, en-AU-Standard-A, en-AU-Standard-
+ B, en-AU-Wavenet-A, en-AU-Wavenet-B, en-AU-Wavenet-C, en-AU-Wavenet-D, en-AU-
+   Standard-C, en-AU-Standard-D, fr-CA-Standard-A, fr-CA-Standard-B, fr-CA-
+   Standard-C, fr-CA-Standard-D, fr-FR-Standard-C, fr-FR-Standard-D, fr-FR-
+Wavenet-A, fr-FR-Wavenet-B, fr-FR-Wavenet-C, fr-FR-Wavenet-D, da-DK-Wavenet-A,
+  pl-PL-Wavenet-A, pl-PL-Wavenet-B, pl-PL-Wavenet-C, pl-PL-Wavenet-D, pt-PT-
+Wavenet-A, pt-PT-Wavenet-B, pt-PT-Wavenet-C, pt-PT-Wavenet-D, ru-RU-Wavenet-A,
+  ru-RU-Wavenet-B, ru-RU-Wavenet-C, ru-RU-Wavenet-D, sk-SK-Wavenet-A, tr-TR-
+Wavenet-A, tr-TR-Wavenet-B, tr-TR-Wavenet-C, tr-TR-Wavenet-D, tr-TR-Wavenet-E,
+  uk-UA-Wavenet-A, ar-XA-Wavenet-A, ar-XA-Wavenet-B, ar-XA-Wavenet-C, cs-CZ-
+Wavenet-A, nl-NL-Wavenet-B, nl-NL-Wavenet-C, nl-NL-Wavenet-D, nl-NL-Wavenet-E,
+  en-IN-Wavenet-A, en-IN-Wavenet-B, en-IN-Wavenet-C, fil-PH-Wavenet-A, fi-FI-
+Wavenet-A, el-GR-Wavenet-A, hi-IN-Wavenet-A, hi-IN-Wavenet-B, hi-IN-Wavenet-C,
+  hu-HU-Wavenet-A, id-ID-Wavenet-A, id-ID-Wavenet-B, id-ID-Wavenet-C, it-IT-
+Wavenet-B, it-IT-Wavenet-C, it-IT-Wavenet-D, ja-JP-Wavenet-B, ja-JP-Wavenet-C,
+ja-JP-Wavenet-D, cmn-CN-Wavenet-A, cmn-CN-Wavenet-B, cmn-CN-Wavenet-C, cmn-CN-
+Wavenet-D, nb-no-Wavenet-E, nb-no-Wavenet-A, nb-no-Wavenet-B, nb-no-Wavenet-C,
+  nb-no-Wavenet-D, vi-VN-Wavenet-A, vi-VN-Wavenet-B, vi-VN-Wavenet-C, vi-VN-
+    Wavenet-D, sr-rs-Standard-A, lv-lv-Standard-A, is-is-Standard-A, bg-bg-
+ Standard-A, af-ZA-Standard-A, Tracy, Danny, Huihui, Yaoyao, Kangkang, HanHan,
+Zhiwei, Asaf, An, Stefanos, Filip, Ivan, Heidi, Herena, Kalpana, Hemant, Matej,
+    Andika, Rizwan, Lado, Valluvar, Linda, Heather, Sean, Michael, Karsten,
+Guillaume, Pattara, Jakub, Szabolcs, Hoda, Naayf] ## WEBS and AsyncWEBS classes
+    The WEBS and AsyncWEBS classes are used to retrieve search results from
+ DuckDuckGo.com and yep.com periodically. To use the AsyncWEBS class, you can
+ perform asynchronous operations using Python's asyncio library. To initialize
+  an instance of the WEBS or AsyncWEBS classes, you can provide the following
+    optional arguments: Here is an example of initializing the WEBS class:
+  ```python3 from webscout import WEBS R = WEBS().text("python programming",
+ max_results=5) print(R) ``` Here is an example of initializing the AsyncWEBS
+   class: ```python3 import asyncio import logging import sys from itertools
+ import chain from random import shuffle import requests from webscout import
+      AsyncWEBS # If you have proxies, define them here proxies = None if
+     sys.platform.lower().startswith("win"): asyncio.set_event_loop_policy
+(asyncio.WindowsSelectorEventLoopPolicy()) def get_words(): word_site = "https:
+ //www.mit.edu/~ecprice/wordlist.10000" resp = requests.get(word_site) words =
+ resp.text.splitlines() return words async def aget_results(word): async with
+      AsyncWEBS(proxies=proxies) as WEBS: results = await WEBS.text(word,
+max_results=None) return results async def main(): words = get_words() shuffle
+  (words) tasks = [aget_results(word) for word in words[:10]] results = await
+ asyncio.gather(*tasks) print(f"Done") for r in chain.from_iterable(results):
+   print(r) logging.basicConfig(level=logging.DEBUG) await main() ``` It is
+important to note that the WEBS and AsyncWEBS classes should always be used as
+a context manager (with statement). This ensures proper resource management and
+ cleanup, as the context manager will automatically handle opening and closing
+  the HTTP client connection. ## Exceptions Exceptions: - `WebscoutE`: Raised
+when there is a generic exception during the API request. ## usage of webscout
+  ### 1. `text()` - text search by DuckDuckGo.com and Yep.com ```python from
+webscout import WEBS # Text search for 'live free or die' using DuckDuckGo.com
+    and Yep.com with WEBS() as WEBS: for r in WEBS.text('live free or die',
+region='wt-wt', safesearch='off', timelimit='y', max_results=10): print(r) for
+     r in WEBS.text('live free or die', region='wt-wt', safesearch='off',
+   timelimit='y', max_results=10): print(r) ``` ### 2. `answers()` - instant
+  answers by DuckDuckGo.com and Yep.com ```python from webscout import WEBS #
+Instant answers for the query "sun" using DuckDuckGo.com and Yep.com with WEBS
+  () as WEBS: for r in WEBS.answers("sun"): print(r) ``` ### 3. `images()` -
+image search by DuckDuckGo.com and Yep.com ```python from webscout import WEBS
+  # Image search for the keyword 'butterfly' using DuckDuckGo.com and Yep.com
+   with WEBS() as WEBS: keywords = 'butterfly' WEBS_images_gen = WEBS.images
+   ( keywords, region="wt-wt", safesearch="off", size=None, type_image=None,
+ layout=None, license_image=None, max_results=10, ) for r in WEBS_images_gen:
+print(r) ``` ### 4. `videos()` - video search by DuckDuckGo.com ```python from
+       webscout import WEBS # Video search for the keyword 'tesla' using
+   DuckDuckGo.com with WEBS() as WEBS: keywords = 'tesla' WEBS_videos_gen =
+    WEBS.videos( keywords, region="wt-wt", safesearch="off", timelimit="w",
+       resolution="high", duration="medium", max_results=10, ) for r in
  WEBS_videos_gen: print(r) ``` ### 5. `news()` - news search by DuckDuckGo.com
  and yep.com ```python from webscout import WEBS # News search for the keyword
   'holiday' using DuckDuckGo.com and yep.com with WEBS() as WEBS: keywords =
         'holiday' WEBS_news_gen = WEBS.news( keywords, region="wt-wt",
 safesearch="off", timelimit="m", max_results=20 ) for r in WEBS_news_gen: print
    (r) ``` ### 6. `maps()` - map search by DuckDuckGo.com and ```python from
 webscout import WEBS # Map search for the keyword 'school' in 'anantnag' using
```

### Comparing `webscout-1.2.9/webscout.egg-info/SOURCES.txt` & `webscout-1.3.0/webscout.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 webscout/__main__.py
 webscout/cli.py
 webscout/exceptions.py
 webscout/models.py
 webscout/transcriber.py
 webscout/utils.py
 webscout/version.py
+webscout/voice.py
 webscout/webscout_search.py
 webscout/webscout_search_async.py
 webscout.egg-info/PKG-INFO
 webscout.egg-info/SOURCES.txt
 webscout.egg-info/dependency_links.txt
 webscout.egg-info/entry_points.txt
 webscout.egg-info/requires.txt
```

