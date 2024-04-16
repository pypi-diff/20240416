# Comparing `tmp/termichat-0.0.2.tar.gz` & `tmp/termichat-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "termichat-0.0.2.tar", last modified: Tue Apr 16 01:59:50 2024, max compression
+gzip compressed data, was "termichat-0.0.3.tar", last modified: Tue Apr 16 02:04:10 2024, max compression
```

## Comparing `termichat-0.0.2.tar` & `termichat-0.0.3.tar`

### file list

```diff
@@ -1,7 +1,16 @@
-drwxrwxr-x   0 guodcz    (1000) guodcz    (1000)        0 2024-04-16 01:59:50.941723 termichat-0.0.2/
--rw-rw-r--   0 guodcz    (1000) guodcz    (1000)      779 2024-04-16 01:59:50.941723 termichat-0.0.2/PKG-INFO
--rw-rw-r--   0 guodcz    (1000) guodcz    (1000)       97 2024-04-16 01:05:24.279940 termichat-0.0.2/setup.cfg
--rw-rw-r--   0 guodcz    (1000) guodcz    (1000)     1078 2024-04-16 01:59:44.501681 termichat-0.0.2/setup.py
-drwxrwxr-x   0 guodcz    (1000) guodcz    (1000)        0 2024-04-16 01:59:50.941723 termichat-0.0.2/termichat/
--rw-rw-r--   0 guodcz    (1000) guodcz    (1000)        0 2024-04-16 01:58:40.545222 termichat-0.0.2/termichat/__init__.py
--rw-rw-r--   0 guodcz    (1000) guodcz    (1000)     4321 2024-04-16 01:58:55.949339 termichat-0.0.2/termichat/main.py
+drwxrwxr-x   0 guodcz    (1000) guodcz    (1000)        0 2024-04-16 02:04:10.710921 termichat-0.0.3/
+-rw-rw-r--   0 guodcz    (1000) guodcz    (1000)      779 2024-04-16 02:04:10.710921 termichat-0.0.3/PKG-INFO
+-rw-rw-r--   0 guodcz    (1000) guodcz    (1000)       97 2024-04-16 01:05:24.279940 termichat-0.0.3/setup.cfg
+-rw-rw-r--   0 guodcz    (1000) guodcz    (1000)     1095 2024-04-16 02:04:05.358905 termichat-0.0.3/setup.py
+drwxrwxr-x   0 guodcz    (1000) guodcz    (1000)        0 2024-04-16 02:04:10.710921 termichat-0.0.3/termichat/
+-rw-rw-r--   0 guodcz    (1000) guodcz    (1000)        0 2024-04-16 01:58:40.545222 termichat-0.0.3/termichat/__init__.py
+drwxrwxr-x   0 guodcz    (1000) guodcz    (1000)        0 2024-04-16 02:04:10.710921 termichat-0.0.3/termichat/lib/
+-rw-rw-r--   0 guodcz    (1000) guodcz    (1000)     2140 2024-04-16 01:14:42.437719 termichat-0.0.3/termichat/lib/ChatConfig.py
+-rw-rw-r--   0 guodcz    (1000) guodcz    (1000)     1426 2023-07-30 15:16:07.079799 termichat-0.0.3/termichat/lib/ChatLog.py
+-rw-rw-r--   0 guodcz    (1000) guodcz    (1000)     4830 2024-04-16 01:15:30.893872 termichat-0.0.3/termichat/lib/LogPad.py
+-rw-rw-r--   0 guodcz    (1000) guodcz    (1000)     2415 2024-04-16 01:11:33.249118 termichat-0.0.3/termichat/lib/LogUI.py
+-rw-rw-r--   0 guodcz    (1000) guodcz    (1000)     2463 2023-07-28 16:53:15.808792 termichat-0.0.3/termichat/lib/TextEditor.py
+-rw-rw-r--   0 guodcz    (1000) guodcz    (1000)     2383 2024-04-16 01:11:35.645126 termichat-0.0.3/termichat/lib/TextPad.py
+-rw-rw-r--   0 guodcz    (1000) guodcz    (1000)     1831 2024-04-16 01:11:19.993076 termichat-0.0.3/termichat/lib/TextUI.py
+-rw-rw-r--   0 guodcz    (1000) guodcz    (1000)        0 2024-04-16 01:27:05.299234 termichat-0.0.3/termichat/lib/__init__.py
+-rw-rw-r--   0 guodcz    (1000) guodcz    (1000)     4321 2024-04-16 01:58:55.949339 termichat-0.0.3/termichat/main.py
```

### Comparing `termichat-0.0.2/PKG-INFO` & `termichat-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: termichat
-Version: 0.0.2
+Version: 0.0.3
 Summary: Use ChatGPT in terminal
 Home-page: https://github.com/GuoDCZ/termichat
 Author: GuoDCZ
 Author-email: guodcz@gmail.com
 License: MIT
 Description: UNKNOWN
 Keywords: chat,chatbot,gpt,gpt-3,openai,terminal,cli
```

### Comparing `termichat-0.0.2/setup.py` & `termichat-0.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from distutils.core import setup
 
 setup(
     name="termichat",
-    packages=["termichat"],
-    version="0.0.2",
+    packages=["termichat", "termichat.lib"],
+    version="0.0.3",
     license="MIT",
     description="Use ChatGPT in terminal",
     author="GuoDCZ",
     author_email="guodcz@gmail.com",
     url="https://github.com/GuoDCZ/termichat",
     download_url="", # FIXME
     keywords=[
```

### Comparing `termichat-0.0.2/termichat/main.py` & `termichat-0.0.3/termichat/main.py`

 * *Files identical despite different names*

