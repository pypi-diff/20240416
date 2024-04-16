# Comparing `tmp/termichat-0.0.3.tar.gz` & `tmp/termichat-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "termichat-0.0.3.tar", last modified: Tue Apr 16 02:04:10 2024, max compression
+gzip compressed data, was "termichat-0.0.4.tar", last modified: Tue Apr 16 02:08:02 2024, max compression
```

## Comparing `termichat-0.0.3.tar` & `termichat-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 guodcz    (1000) guodcz    (1000)        0 2024-04-16 02:04:10.710921 termichat-0.0.3/
--rw-rw-r--   0 guodcz    (1000) guodcz    (1000)      779 2024-04-16 02:04:10.710921 termichat-0.0.3/PKG-INFO
--rw-rw-r--   0 guodcz    (1000) guodcz    (1000)       97 2024-04-16 01:05:24.279940 termichat-0.0.3/setup.cfg
--rw-rw-r--   0 guodcz    (1000) guodcz    (1000)     1095 2024-04-16 02:04:05.358905 termichat-0.0.3/setup.py
-drwxrwxr-x   0 guodcz    (1000) guodcz    (1000)        0 2024-04-16 02:04:10.710921 termichat-0.0.3/termichat/
--rw-rw-r--   0 guodcz    (1000) guodcz    (1000)        0 2024-04-16 01:58:40.545222 termichat-0.0.3/termichat/__init__.py
-drwxrwxr-x   0 guodcz    (1000) guodcz    (1000)        0 2024-04-16 02:04:10.710921 termichat-0.0.3/termichat/lib/
--rw-rw-r--   0 guodcz    (1000) guodcz    (1000)     2140 2024-04-16 01:14:42.437719 termichat-0.0.3/termichat/lib/ChatConfig.py
--rw-rw-r--   0 guodcz    (1000) guodcz    (1000)     1426 2023-07-30 15:16:07.079799 termichat-0.0.3/termichat/lib/ChatLog.py
--rw-rw-r--   0 guodcz    (1000) guodcz    (1000)     4830 2024-04-16 01:15:30.893872 termichat-0.0.3/termichat/lib/LogPad.py
--rw-rw-r--   0 guodcz    (1000) guodcz    (1000)     2415 2024-04-16 01:11:33.249118 termichat-0.0.3/termichat/lib/LogUI.py
--rw-rw-r--   0 guodcz    (1000) guodcz    (1000)     2463 2023-07-28 16:53:15.808792 termichat-0.0.3/termichat/lib/TextEditor.py
--rw-rw-r--   0 guodcz    (1000) guodcz    (1000)     2383 2024-04-16 01:11:35.645126 termichat-0.0.3/termichat/lib/TextPad.py
--rw-rw-r--   0 guodcz    (1000) guodcz    (1000)     1831 2024-04-16 01:11:19.993076 termichat-0.0.3/termichat/lib/TextUI.py
--rw-rw-r--   0 guodcz    (1000) guodcz    (1000)        0 2024-04-16 01:27:05.299234 termichat-0.0.3/termichat/lib/__init__.py
--rw-rw-r--   0 guodcz    (1000) guodcz    (1000)     4321 2024-04-16 01:58:55.949339 termichat-0.0.3/termichat/main.py
+drwxrwxr-x   0 guodcz    (1000) guodcz    (1000)        0 2024-04-16 02:08:02.855385 termichat-0.0.4/
+-rw-rw-r--   0 guodcz    (1000) guodcz    (1000)      779 2024-04-16 02:08:02.855385 termichat-0.0.4/PKG-INFO
+-rw-rw-r--   0 guodcz    (1000) guodcz    (1000)       97 2024-04-16 01:05:24.279940 termichat-0.0.4/setup.cfg
+-rw-rw-r--   0 guodcz    (1000) guodcz    (1000)     1095 2024-04-16 02:08:00.987383 termichat-0.0.4/setup.py
+drwxrwxr-x   0 guodcz    (1000) guodcz    (1000)        0 2024-04-16 02:08:02.855385 termichat-0.0.4/termichat/
+-rw-rw-r--   0 guodcz    (1000) guodcz    (1000)        0 2024-04-16 01:58:40.545222 termichat-0.0.4/termichat/__init__.py
+drwxrwxr-x   0 guodcz    (1000) guodcz    (1000)        0 2024-04-16 02:08:02.855385 termichat-0.0.4/termichat/lib/
+-rw-rw-r--   0 guodcz    (1000) guodcz    (1000)     2140 2024-04-16 02:06:07.807210 termichat-0.0.4/termichat/lib/ChatConfig.py
+-rw-rw-r--   0 guodcz    (1000) guodcz    (1000)     1426 2023-07-30 15:16:07.079799 termichat-0.0.4/termichat/lib/ChatLog.py
+-rw-rw-r--   0 guodcz    (1000) guodcz    (1000)     4830 2024-04-16 01:15:30.893872 termichat-0.0.4/termichat/lib/LogPad.py
+-rw-rw-r--   0 guodcz    (1000) guodcz    (1000)     2415 2024-04-16 01:11:33.249118 termichat-0.0.4/termichat/lib/LogUI.py
+-rw-rw-r--   0 guodcz    (1000) guodcz    (1000)     2463 2023-07-28 16:53:15.808792 termichat-0.0.4/termichat/lib/TextEditor.py
+-rw-rw-r--   0 guodcz    (1000) guodcz    (1000)     2383 2024-04-16 01:11:35.645126 termichat-0.0.4/termichat/lib/TextPad.py
+-rw-rw-r--   0 guodcz    (1000) guodcz    (1000)     1831 2024-04-16 01:11:19.993076 termichat-0.0.4/termichat/lib/TextUI.py
+-rw-rw-r--   0 guodcz    (1000) guodcz    (1000)        0 2024-04-16 01:27:05.299234 termichat-0.0.4/termichat/lib/__init__.py
+-rw-rw-r--   0 guodcz    (1000) guodcz    (1000)     4775 2024-04-16 02:07:25.455339 termichat-0.0.4/termichat/main.py
```

### Comparing `termichat-0.0.3/PKG-INFO` & `termichat-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: termichat
-Version: 0.0.3
+Version: 0.0.4
 Summary: Use ChatGPT in terminal
 Home-page: https://github.com/GuoDCZ/termichat
 Author: GuoDCZ
 Author-email: guodcz@gmail.com
 License: MIT
 Description: UNKNOWN
 Keywords: chat,chatbot,gpt,gpt-3,openai,terminal,cli
```

### Comparing `termichat-0.0.3/setup.py` & `termichat-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from distutils.core import setup
 
 setup(
     name="termichat",
     packages=["termichat", "termichat.lib"],
-    version="0.0.3",
+    version="0.0.4",
     license="MIT",
     description="Use ChatGPT in terminal",
     author="GuoDCZ",
     author_email="guodcz@gmail.com",
     url="https://github.com/GuoDCZ/termichat",
     download_url="", # FIXME
     keywords=[
```

### Comparing `termichat-0.0.3/termichat/lib/ChatConfig.py` & `termichat-0.0.4/termichat/lib/ChatConfig.py`

 * *Files identical despite different names*

### Comparing `termichat-0.0.3/termichat/lib/ChatLog.py` & `termichat-0.0.4/termichat/lib/ChatLog.py`

 * *Files identical despite different names*

### Comparing `termichat-0.0.3/termichat/lib/LogPad.py` & `termichat-0.0.4/termichat/lib/LogPad.py`

 * *Files identical despite different names*

### Comparing `termichat-0.0.3/termichat/lib/LogUI.py` & `termichat-0.0.4/termichat/lib/LogUI.py`

 * *Files identical despite different names*

### Comparing `termichat-0.0.3/termichat/lib/TextEditor.py` & `termichat-0.0.4/termichat/lib/TextEditor.py`

 * *Files identical despite different names*

### Comparing `termichat-0.0.3/termichat/lib/TextPad.py` & `termichat-0.0.4/termichat/lib/TextPad.py`

 * *Files identical despite different names*

### Comparing `termichat-0.0.3/termichat/lib/TextUI.py` & `termichat-0.0.4/termichat/lib/TextUI.py`

 * *Files identical despite different names*

### Comparing `termichat-0.0.3/termichat/main.py` & `termichat-0.0.4/termichat/main.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,47 @@
 import openai
 import curses
 
 from .lib.ChatConfig import *
 from .lib.TextUI import *
 from .lib.LogUI import *
 
+
 def initUI():
     curses.initscr()
     curses.start_color()
-    curses.init_color(0xf0, 0xf3*1000//0x100//2+500, 0x94*1000//0x100//2+500, 0x25*1000//0x100//2+500)
-    curses.init_pair(0xf0, 0xf0, 0)
+    curses.init_color(
+        0xF0,
+        0xF3 * 1000 // 0x100 // 2 + 500,
+        0x94 * 1000 // 0x100 // 2 + 500,
+        0x25 * 1000 // 0x100 // 2 + 500,
+    )
+    curses.init_pair(0xF0, 0xF0, 0)
     # self.COLOR_USR = curses.color_pair(0xf0)
-    curses.init_color(0xf1, 0x2d*1000//0x100//2+500, 0xbc*1000//0x100//2+500, 0xec*1000//0x100//2+500) # BLUE
-    curses.init_pair(0xf1, 0xf1, 0)
+    curses.init_color(
+        0xF1,
+        0x2D * 1000 // 0x100 // 2 + 500,
+        0xBC * 1000 // 0x100 // 2 + 500,
+        0xEC * 1000 // 0x100 // 2 + 500,
+    )  # BLUE
+    curses.init_pair(0xF1, 0xF1, 0)
     # self.COLOR_BOT = curses.color_pair(0xf1)
-    curses.init_color(0xf2, 0x25*1000//0x100//2+500, 0xf3*1000//0x100//2+500, 0x94*1000//0x100//2+500)
-    curses.init_pair(0xf2, 0xf2, 0)
+    curses.init_color(
+        0xF2,
+        0x25 * 1000 // 0x100 // 2 + 500,
+        0xF3 * 1000 // 0x100 // 2 + 500,
+        0x94 * 1000 // 0x100 // 2 + 500,
+    )
+    curses.init_pair(0xF2, 0xF2, 0)
     # self.COLOR_SYS = curses.color_pair(0xf2)
-    curses.init_color(0xf3, 500, 500, 500) # GREY
-    curses.init_pair(0xf3, 0xf3, 0)
+    curses.init_color(0xF3, 500, 500, 500)  # GREY
+    curses.init_pair(0xF3, 0xF3, 0)
     # self.COLOR_INFO = curses.color_pair(0xf3)
 
+
 class ChatBot:
     def __init__(self, config):
         self.config = config
 
     def run(self, stdscr: curses.window):
         ssize = stdscr.getmaxyx()
         self.stdscr = stdscr
@@ -39,83 +56,94 @@
         while True:
             key = stdscr.get_wch()
             if not self.put_key(ord(key) if type(key) is str else key):
                 break
 
     def cmpl_request(self, messages):
         return openai.ChatCompletion.create(
-            model = "gpt-3.5-turbo", 
+            model="gpt-3.5-turbo",
             # model = "gpt-3.5-turbo-0301",
             # model = self.config['model'],
             # model = "gpt-4-1106-preview",
             # model = "gpt-4-32k",
             # model = "gpt-4-32k-0613",
             # model = "gpt-4-1106-preview",
-            messages = messages, 
-            temperature = self.config['temperature'],
-            presence_penalty = self.config['presence_penalty'], 
-            frequency_penalty = self.config['frequency_penalty'],
-            stream = True
+            messages=messages,
+            temperature=self.config["temperature"],
+            presence_penalty=self.config["presence_penalty"],
+            frequency_penalty=self.config["frequency_penalty"],
+            stream=True,
         )
-    
+
     def put_key(self, key):
-        if not self.alt and key == 27: # ALT
+        if not self.alt and key == 27:  # ALT
             self.alt = True
-        elif self.alt and key == 10: # ALT + ENTER
-            if not 'role' in self.log.curr.chat:
-                self.log._add_msg('system', self.text.s)
+        elif self.alt and key == 10:  # ALT + ENTER
+            if not "role" in self.log.curr.chat:
+                self.log._add_msg("system", self.text.s)
                 self.text.clear()
             else:
-                if self.log.curr.chat['role'] != 'user':
+                if self.log.curr.chat["role"] != "user":
                     self.log.add_usr_msg(self.text.s)
                     self.text.clear()
                     self.log.update_yshow(self.text.yshow)
                     self.log.refresh()
                     self.text.refresh()
                 messages = self.log.get_chat()
                 cmpl = self.cmpl_request(messages)
                 content = self.log.stream_show_cmpl(cmpl)
                 self.log.add_bot_msg(content)
             self.log.update_yshow(self.text.yshow)
             self.alt = False
-        elif self.alt and key == 27: # double ESC
+        elif self.alt and key == 27:  # double ESC
             pass
             # return False
-        elif key == 410: # RESIZE
+        elif key == 410:  # RESIZE
             ssize = self.stdscr.getmaxyx()
             self.text.resize(ssize)
             self.log.update_yshow(self.text.yshow)
             self.log.resize(ssize)
         elif self.log.put_key(key):
             if not self.text.saved:
                 self.text.save()
             item = self.log.curr.get_next()
             if item:
-                if item.chat['role'] != 'assistant':
-                    self.text.set(item.chat['content'])
+                if item.chat["role"] != "assistant":
+                    self.text.set(item.chat["content"])
                 else:
                     self.text.set("Press Alt + Enter to regenerate")
             else:
                 self.text.load()
         else:
             self.text.put_key(key)
             self.log.update_yshow(self.text.yshow)
         self.log.refresh()
         self.text.refresh()
         return True
 
+
 def main():
     openai.api_key = os.getenv("OPENAI_API_KEY")
     if not openai.api_key:
         print("Please set OPENAI_API_KEY environment variable")
         return
-    if not os.path.exists(CONFIG_FILE):
-        save_config(init_config())
+    # if not os.path.exists(CONFIG_FILE):
+    #     save_config(init_config())
     else:
         initUI()
-        config = load_config()
+        # config = load_config()
+        config = {
+            "roleDir": "roleplay/",
+            "role": "Bot",
+            "model": "gpt-3.5-turbo",
+            "memorable": "n",
+            "temperature": 1.0,
+            "presence_penalty": 0.0,
+            "frequency_penalty": 0.0,
+        }
         print_config(config)
         bot = ChatBot(config)
         curses.wrapper(bot.run)
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     main()
```

