# Comparing `tmp/sneakpeek-0.8.3.tar.gz` & `tmp/sneakpeek-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sneakpeek-0.8.3.tar", max compression
+gzip compressed data, was "sneakpeek-0.9.0.tar", max compression
```

## Comparing `sneakpeek-0.8.3.tar` & `sneakpeek-0.9.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1096 2024-04-16 13:11:38.798221 sneakpeek-0.8.3/LICENSE
--rw-r--r--   0        0        0     8064 2024-04-16 13:11:38.798221 sneakpeek-0.8.3/README.md
--rw-r--r--   0        0        0     1659 2024-04-16 13:38:03.500435 sneakpeek-0.8.3/pyproject.toml
--rw-r--r--   0        0        0       56 2024-04-16 13:11:38.799221 sneakpeek-0.8.3/sneakpeek/__init__.py
--rw-r--r--   0        0        0     1245 2024-04-16 13:11:38.800221 sneakpeek-0.8.3/sneakpeek/console.py
--rw-r--r--   0        0        0      458 2024-04-16 13:11:38.800221 sneakpeek-0.8.3/sneakpeek/server.py
--rw-r--r--   0        0        0     5725 2024-04-16 13:38:03.500435 sneakpeek-0.8.3/sneakpeek/sneakpeek.py
--rw-r--r--   0        0        0     9820 1970-01-01 00:00:00.000000 sneakpeek-0.8.3/PKG-INFO
+-rw-r--r--   0        0        0     1096 2024-04-16 13:11:38.798221 sneakpeek-0.9.0/LICENSE
+-rw-r--r--   0        0        0     8064 2024-04-16 13:11:38.798221 sneakpeek-0.9.0/README.md
+-rw-r--r--   0        0        0     1659 2024-04-16 13:52:34.738196 sneakpeek-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0       56 2024-04-16 13:52:40.811062 sneakpeek-0.9.0/sneakpeek/__init__.py
+-rw-r--r--   0        0        0     1245 2024-04-16 13:11:38.800221 sneakpeek-0.9.0/sneakpeek/console.py
+-rw-r--r--   0        0        0      458 2024-04-16 13:11:38.800221 sneakpeek-0.9.0/sneakpeek/server.py
+-rw-r--r--   0        0        0     5767 2024-04-16 13:48:23.962564 sneakpeek-0.9.0/sneakpeek/sneakpeek.py
+-rw-r--r--   0        0        0     9871 1970-01-01 00:00:00.000000 sneakpeek-0.9.0/PKG-INFO
```

### Comparing `sneakpeek-0.8.3/LICENSE` & `sneakpeek-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sneakpeek-0.8.3/README.md` & `sneakpeek-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `sneakpeek-0.8.3/pyproject.toml` & `sneakpeek-0.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sneakpeek"
-version = "0.8.3"
+version = "0.9.0"
 description = "A python module to generate link previews."
 license = "MIT"
 authors = ["Ameya Shenoy <shenoy.ameya@gmail.com>"]
 maintainers = ["Ameya Shenoy <shenoy.ameya@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/codingcoffee/sneakpeek"
 repository = "https://github.com/codingcoffee/sneakpeek"
```

### Comparing `sneakpeek-0.8.3/sneakpeek/console.py` & `sneakpeek-0.9.0/sneakpeek/console.py`

 * *Files identical despite different names*

### Comparing `sneakpeek-0.8.3/sneakpeek/sneakpeek.py` & `sneakpeek-0.9.0/sneakpeek/sneakpeek.py`

 * *Files 5% similar despite different names*

```diff
@@ -60,14 +60,15 @@
         with ydl.YoutubeDL(ydl_opts) as ydl_youtube:
             try:
                 info_dict = ydl_youtube.extract_info(self.url, download=False)
                 self.title = info_dict.get("title")
                 self.description = info_dict.get("description")
                 self.title = info_dict.get("title")
                 self.image = info_dict.get("thumbnail")
+                self.type = "video.other"
             except ydl.utils.DownloadError:
                 return
 
     def fetch_and_parse_twitter(self):
         if not isinstance(self.url, str):
             return
         if "status" in self.url:
```

### Comparing `sneakpeek-0.8.3/PKG-INFO` & `sneakpeek-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sneakpeek
-Version: 0.8.3
+Version: 0.9.0
 Summary: A python module to generate link previews.
 Home-page: https://github.com/codingcoffee/sneakpeek
 License: MIT
 Keywords: open-graph-protocol,ogp,twitter,twitter-cards,python,schema,link-preview
 Author: Ameya Shenoy
 Author-email: shenoy.ameya@gmail.com
 Maintainer: Ameya Shenoy
@@ -16,14 +16,15 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing :: Markup :: HTML
 Classifier: Topic :: Utilities
 Requires-Dist: beautifulsoup4 (>=4.11.1,<5.0.0)
```

