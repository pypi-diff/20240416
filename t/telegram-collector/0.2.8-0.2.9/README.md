# Comparing `tmp/telegram_collector-0.2.8.tar.gz` & `tmp/telegram_collector-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telegram_collector-0.2.8.tar", last modified: Mon Apr 15 02:16:09 2024, max compression
+gzip compressed data, was "telegram_collector-0.2.9.tar", last modified: Mon Apr 15 03:22:15 2024, max compression
```

## Comparing `telegram_collector-0.2.8.tar` & `telegram_collector-0.2.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 02:16:09.186114 telegram_collector-0.2.8/
--rw-rw-rw-   0        0        0      317 2024-04-15 02:16:09.186114 telegram_collector-0.2.8/PKG-INFO
--rw-rw-rw-   0        0        0      343 2024-04-11 14:11:58.000000 telegram_collector-0.2.8/README.md
--rw-rw-rw-   0        0        0       42 2024-04-15 02:16:09.186114 telegram_collector-0.2.8/setup.cfg
--rw-rw-rw-   0        0        0      557 2024-04-15 02:16:07.000000 telegram_collector-0.2.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-15 02:16:09.177830 telegram_collector-0.2.8/telegram_collector/
--rw-rw-rw-   0        0        0     5340 2024-04-15 02:16:07.000000 telegram_collector-0.2.8/telegram_collector/__init__.py
--rw-rw-rw-   0        0        0     1961 2024-04-11 14:22:26.000000 telegram_collector-0.2.8/telegram_collector/__main__.py
--rw-rw-rw-   0        0        0     2821 2024-04-15 02:16:07.000000 telegram_collector-0.2.8/telegram_collector/util.py
-drwxrwxrwx   0        0        0        0 2024-04-15 02:16:09.185130 telegram_collector-0.2.8/telegram_collector.egg-info/
--rw-rw-rw-   0        0        0      317 2024-04-15 02:16:09.000000 telegram_collector-0.2.8/telegram_collector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      361 2024-04-15 02:16:09.000000 telegram_collector-0.2.8/telegram_collector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 02:16:09.000000 telegram_collector-0.2.8/telegram_collector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2024-04-15 02:16:09.000000 telegram_collector-0.2.8/telegram_collector.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       36 2024-04-15 02:16:09.000000 telegram_collector-0.2.8/telegram_collector.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-04-15 02:16:09.000000 telegram_collector-0.2.8/telegram_collector.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-15 03:22:15.384874 telegram_collector-0.2.9/
+-rw-rw-rw-   0        0        0      317 2024-04-15 03:22:15.383371 telegram_collector-0.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0      343 2024-04-11 14:11:58.000000 telegram_collector-0.2.9/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-15 03:22:15.384874 telegram_collector-0.2.9/setup.cfg
+-rw-rw-rw-   0        0        0      557 2024-04-15 03:22:11.000000 telegram_collector-0.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 03:22:15.373352 telegram_collector-0.2.9/telegram_collector/
+-rw-rw-rw-   0        0        0     5338 2024-04-15 03:22:11.000000 telegram_collector-0.2.9/telegram_collector/__init__.py
+-rw-rw-rw-   0        0        0     1961 2024-04-11 14:22:26.000000 telegram_collector-0.2.9/telegram_collector/__main__.py
+-rw-rw-rw-   0        0        0     2821 2024-04-15 02:16:07.000000 telegram_collector-0.2.9/telegram_collector/util.py
+drwxrwxrwx   0        0        0        0 2024-04-15 03:22:15.382371 telegram_collector-0.2.9/telegram_collector.egg-info/
+-rw-rw-rw-   0        0        0      317 2024-04-15 03:22:15.000000 telegram_collector-0.2.9/telegram_collector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      361 2024-04-15 03:22:15.000000 telegram_collector-0.2.9/telegram_collector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 03:22:15.000000 telegram_collector-0.2.9/telegram_collector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2024-04-15 03:22:15.000000 telegram_collector-0.2.9/telegram_collector.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       36 2024-04-15 03:22:15.000000 telegram_collector-0.2.9/telegram_collector.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-04-15 03:22:15.000000 telegram_collector-0.2.9/telegram_collector.egg-info/top_level.txt
```

### Comparing `telegram_collector-0.2.8/setup.py` & `telegram_collector-0.2.9/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # coding: utf-8
 
 from setuptools import setup
 
 setup(
     name='telegram_collector',
-    version='0.2.8',
+    version='0.2.9',
     author='fengleicn',
     author_email='fengleisemail@gmail.com',
     url='https://github.com/fengleicn/telegram_collector',
     description=u'收集电报群组的视频图片消息',
     packages=['telegram_collector'],
     install_requires=['telethon', 'python_socks', 'async_timeout'],
     entry_points={
```

### Comparing `telegram_collector-0.2.8/telegram_collector/__init__.py` & `telegram_collector-0.2.9/telegram_collector/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,15 +123,15 @@
             await self.__trigger_get_message()
         finally:
             await self.__terminate_client()
 
     async def __trigger_get_message(self):
         while True:
             # trigger
-            for i in self.src_dialogs():
+            for i in self.src_dialogs:
                 messages = self.client.get_messages(i)
                 for message in messages:
                     print_message(message)
             await asyncio.sleep(2)
 
     async def __do_after_init(self, func):
         await self.__do_init()
```

### Comparing `telegram_collector-0.2.8/telegram_collector/__main__.py` & `telegram_collector-0.2.9/telegram_collector/__main__.py`

 * *Files identical despite different names*

### Comparing `telegram_collector-0.2.8/telegram_collector/util.py` & `telegram_collector-0.2.9/telegram_collector/util.py`

 * *Files identical despite different names*

