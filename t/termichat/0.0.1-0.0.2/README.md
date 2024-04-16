# Comparing `tmp/termichat-0.0.1.tar.gz` & `tmp/termichat-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "termichat-0.0.1.tar", last modified: Tue Apr 16 01:55:40 2024, max compression
+gzip compressed data, was "termichat-0.0.2.tar", last modified: Tue Apr 16 01:59:50 2024, max compression
```

## Comparing `termichat-0.0.1.tar` & `termichat-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
-drwxrwxr-x   0 guodcz    (1000) guodcz    (1000)        0 2024-04-16 01:55:40.783468 termichat-0.0.1/
--rw-rw-r--   0 guodcz    (1000) guodcz    (1000)      779 2024-04-16 01:55:40.783468 termichat-0.0.1/PKG-INFO
--rw-rw-r--   0 guodcz    (1000) guodcz    (1000)       97 2024-04-16 01:05:24.279940 termichat-0.0.1/setup.cfg
--rw-rw-r--   0 guodcz    (1000) guodcz    (1000)     1078 2024-04-16 01:55:38.911445 termichat-0.0.1/setup.py
-drwxrwxr-x   0 guodcz    (1000) guodcz    (1000)        0 2024-04-16 01:55:40.783468 termichat-0.0.1/termichat/
--rw-rw-r--   0 guodcz    (1000) guodcz    (1000)       20 2024-04-16 01:34:31.859426 termichat-0.0.1/termichat/__init__.py
--rw-rw-r--   0 guodcz    (1000) guodcz    (1000)     4348 2024-04-16 01:47:12.415201 termichat-0.0.1/termichat/main.py
+drwxrwxr-x   0 guodcz    (1000) guodcz    (1000)        0 2024-04-16 01:59:50.941723 termichat-0.0.2/
+-rw-rw-r--   0 guodcz    (1000) guodcz    (1000)      779 2024-04-16 01:59:50.941723 termichat-0.0.2/PKG-INFO
+-rw-rw-r--   0 guodcz    (1000) guodcz    (1000)       97 2024-04-16 01:05:24.279940 termichat-0.0.2/setup.cfg
+-rw-rw-r--   0 guodcz    (1000) guodcz    (1000)     1078 2024-04-16 01:59:44.501681 termichat-0.0.2/setup.py
+drwxrwxr-x   0 guodcz    (1000) guodcz    (1000)        0 2024-04-16 01:59:50.941723 termichat-0.0.2/termichat/
+-rw-rw-r--   0 guodcz    (1000) guodcz    (1000)        0 2024-04-16 01:58:40.545222 termichat-0.0.2/termichat/__init__.py
+-rw-rw-r--   0 guodcz    (1000) guodcz    (1000)     4321 2024-04-16 01:58:55.949339 termichat-0.0.2/termichat/main.py
```

### Comparing `termichat-0.0.1/PKG-INFO` & `termichat-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: termichat
-Version: 0.0.1
+Version: 0.0.2
 Summary: Use ChatGPT in terminal
 Home-page: https://github.com/GuoDCZ/termichat
 Author: GuoDCZ
 Author-email: guodcz@gmail.com
 License: MIT
 Description: UNKNOWN
 Keywords: chat,chatbot,gpt,gpt-3,openai,terminal,cli
```

### Comparing `termichat-0.0.1/setup.py` & `termichat-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from distutils.core import setup
 
 setup(
     name="termichat",
     packages=["termichat"],
-    version="0.0.1",
+    version="0.0.2",
     license="MIT",
     description="Use ChatGPT in terminal",
     author="GuoDCZ",
     author_email="guodcz@gmail.com",
     url="https://github.com/GuoDCZ/termichat",
     download_url="", # FIXME
     keywords=[
```

### Comparing `termichat-0.0.1/termichat/main.py` & `termichat-0.0.2/termichat/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import openai
 import curses
 
-from termichat.lib.ChatConfig import *
-from termichat.lib.TextUI import *
-from termichat.lib.LogUI import *
+from .lib.ChatConfig import *
+from .lib.TextUI import *
+from .lib.LogUI import *
 
 def initUI():
     curses.initscr()
     curses.start_color()
     curses.init_color(0xf0, 0xf3*1000//0x100//2+500, 0x94*1000//0x100//2+500, 0x25*1000//0x100//2+500)
     curses.init_pair(0xf0, 0xf0, 0)
     # self.COLOR_USR = curses.color_pair(0xf0)
```

