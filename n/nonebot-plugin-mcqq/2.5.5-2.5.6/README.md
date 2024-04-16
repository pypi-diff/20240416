# Comparing `tmp/nonebot_plugin_mcqq-2.5.5.tar.gz` & `tmp/nonebot_plugin_mcqq-2.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_mcqq-2.5.5.tar", max compression
+gzip compressed data, was "nonebot_plugin_mcqq-2.5.6.tar", max compression
```

## Comparing `nonebot_plugin_mcqq-2.5.5.tar` & `nonebot_plugin_mcqq-2.5.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1065 2024-03-28 14:52:52.283836 nonebot_plugin_mcqq-2.5.5/LICENSE
--rw-r--r--   0        0        0     2403 2024-03-28 14:52:52.283836 nonebot_plugin_mcqq-2.5.5/README.md
--rw-r--r--   0        0        0      658 2024-03-28 14:52:52.283836 nonebot_plugin_mcqq-2.5.5/nonebot_plugin_mcqq/__init__.py
--rw-r--r--   0        0        0     2612 2024-03-28 14:52:52.283836 nonebot_plugin_mcqq-2.5.5/nonebot_plugin_mcqq/bot_manage.py
--rw-r--r--   0        0        0     1256 2024-03-28 14:52:52.283836 nonebot_plugin_mcqq-2.5.5/nonebot_plugin_mcqq/minecraft_msg.py
--rw-r--r--   0        0        0     3943 2024-03-28 14:52:52.283836 nonebot_plugin_mcqq-2.5.5/nonebot_plugin_mcqq/qq_msg.py
--rw-r--r--   0        0        0      567 2024-03-28 14:52:52.287836 nonebot_plugin_mcqq-2.5.5/pyproject.toml
--rw-r--r--   0        0        0     3336 1970-01-01 00:00:00.000000 nonebot_plugin_mcqq-2.5.5/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-16 04:29:01.740356 nonebot_plugin_mcqq-2.5.6/LICENSE
+-rw-r--r--   0        0        0     2403 2024-04-16 04:29:01.740356 nonebot_plugin_mcqq-2.5.6/README.md
+-rw-r--r--   0        0        0      658 2024-04-16 04:29:01.744356 nonebot_plugin_mcqq-2.5.6/nonebot_plugin_mcqq/__init__.py
+-rw-r--r--   0        0        0     2612 2024-04-16 04:29:01.744356 nonebot_plugin_mcqq-2.5.6/nonebot_plugin_mcqq/bot_manage.py
+-rw-r--r--   0        0        0      916 2024-04-16 04:29:01.744356 nonebot_plugin_mcqq-2.5.6/nonebot_plugin_mcqq/minecraft_msg.py
+-rw-r--r--   0        0        0     3943 2024-04-16 04:29:01.744356 nonebot_plugin_mcqq-2.5.6/nonebot_plugin_mcqq/qq_msg.py
+-rw-r--r--   0        0        0      567 2024-04-16 04:29:01.744356 nonebot_plugin_mcqq-2.5.6/pyproject.toml
+-rw-r--r--   0        0        0     3336 1970-01-01 00:00:00.000000 nonebot_plugin_mcqq-2.5.6/PKG-INFO
```

### Comparing `nonebot_plugin_mcqq-2.5.5/LICENSE` & `nonebot_plugin_mcqq-2.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mcqq-2.5.5/README.md` & `nonebot_plugin_mcqq-2.5.6/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mcqq-2.5.5/nonebot_plugin_mcqq/__init__.py` & `nonebot_plugin_mcqq-2.5.6/nonebot_plugin_mcqq/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mcqq-2.5.5/nonebot_plugin_mcqq/bot_manage.py` & `nonebot_plugin_mcqq-2.5.6/nonebot_plugin_mcqq/bot_manage.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mcqq-2.5.5/nonebot_plugin_mcqq/qq_msg.py` & `nonebot_plugin_mcqq-2.5.6/nonebot_plugin_mcqq/qq_msg.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mcqq-2.5.5/pyproject.toml` & `nonebot_plugin_mcqq-2.5.6/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "nonebot-plugin-mcqq"
-version = "2.5.5"
+version = "2.5.6"
 description = "基于NoneBot的QQ群聊与Minecraft Server消息互通插件"
 authors = ["17TheWord <17theword@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 nonebot2 = "^2.2.1"
+mcqq-tool = "^1.1.7"
 aio-mc-rcon = "^3.2.2"
 nonebot-adapter-qq = "^1.4.2"
 nonebot-adapter-onebot = "^2.4.1"
 nonebot-adapter-minecraft = "^1.0.8.post1"
 nonebot-plugin-guild-patch-remix = "^0.2.4"
-mcqq-tool = "^1.1.7"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot_plugin_mcqq-2.5.5/PKG-INFO` & `nonebot_plugin_mcqq-2.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-mcqq
-Version: 2.5.5
+Version: 2.5.6
 Summary: 基于NoneBot的QQ群聊与Minecraft Server消息互通插件
 License: MIT
 Author: 17TheWord
 Author-email: 17theword@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

