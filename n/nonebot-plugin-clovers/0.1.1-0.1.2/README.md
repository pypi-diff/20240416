# Comparing `tmp/nonebot_plugin_clovers-0.1.1.tar.gz` & `tmp/nonebot_plugin_clovers-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_clovers-0.1.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_clovers-0.1.2.tar", max compression
```

## Comparing `nonebot_plugin_clovers-0.1.1.tar` & `nonebot_plugin_clovers-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1086 2024-04-15 11:49:16.312798 nonebot_plugin_clovers-0.1.1/LICENSE
--rw-r--r--   0        0        0     2212 2024-04-15 13:06:26.886936 nonebot_plugin_clovers-0.1.1/nonebot_plugin_clovers/__init__.py
--rw-r--r--   0        0        0      842 2024-04-15 02:23:00.900179 nonebot_plugin_clovers-0.1.1/nonebot_plugin_clovers/adapters/main.py
--rw-r--r--   0        0        0     1730 2024-04-15 11:51:19.416688 nonebot_plugin_clovers-0.1.1/nonebot_plugin_clovers/adapters/qq.py
--rw-r--r--   0        0        0     3609 2024-04-15 11:51:16.127157 nonebot_plugin_clovers-0.1.1/nonebot_plugin_clovers/adapters/v11.py
--rw-r--r--   0        0        0      397 2024-04-15 13:07:06.137229 nonebot_plugin_clovers-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2514 2024-04-15 11:57:25.353441 nonebot_plugin_clovers-0.1.1/README.md
--rw-r--r--   0        0        0     2946 1970-01-01 00:00:00.000000 nonebot_plugin_clovers-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1086 2024-04-15 11:49:16.312798 nonebot_plugin_clovers-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2213 2024-04-15 14:42:38.315950 nonebot_plugin_clovers-0.1.2/nonebot_plugin_clovers/__init__.py
+-rw-r--r--   0        0        0      842 2024-04-15 02:23:00.900179 nonebot_plugin_clovers-0.1.2/nonebot_plugin_clovers/adapters/main.py
+-rw-r--r--   0        0        0     1730 2024-04-15 11:51:19.416688 nonebot_plugin_clovers-0.1.2/nonebot_plugin_clovers/adapters/qq.py
+-rw-r--r--   0        0        0     3609 2024-04-15 11:51:16.127157 nonebot_plugin_clovers-0.1.2/nonebot_plugin_clovers/adapters/v11.py
+-rw-r--r--   0        0        0      397 2024-04-15 14:43:28.422454 nonebot_plugin_clovers-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2514 2024-04-15 11:57:25.353441 nonebot_plugin_clovers-0.1.2/README.md
+-rw-r--r--   0        0        0     2946 1970-01-01 00:00:00.000000 nonebot_plugin_clovers-0.1.2/PKG-INFO
```

### Comparing `nonebot_plugin_clovers-0.1.1/LICENSE` & `nonebot_plugin_clovers-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_clovers-0.1.1/nonebot_plugin_clovers/__init__.py` & `nonebot_plugin_clovers-0.1.2/nonebot_plugin_clovers/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 adapter = new_adapter(loader.plugins)
 
 driver.on_startup(adapter.startup)
 
 from nonebot import on_message
 from nonebot.matcher import Matcher
 
-main = on_message(priority=50, block=True)
+main = on_message(priority=50, block=False)
 
 
 def add_response(Bot, Event, adapter_method: AdapterMethod, adapter_key: str):
     adapter.methods[adapter_key] = adapter_method
 
     @main.handle()
     async def _(matcher: Matcher, bot: Bot, event: Event):
```

### Comparing `nonebot_plugin_clovers-0.1.1/nonebot_plugin_clovers/adapters/main.py` & `nonebot_plugin_clovers-0.1.2/nonebot_plugin_clovers/adapters/main.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_clovers-0.1.1/nonebot_plugin_clovers/adapters/qq.py` & `nonebot_plugin_clovers-0.1.2/nonebot_plugin_clovers/adapters/qq.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_clovers-0.1.1/nonebot_plugin_clovers/adapters/v11.py` & `nonebot_plugin_clovers-0.1.2/nonebot_plugin_clovers/adapters/v11.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_clovers-0.1.1/README.md` & `nonebot_plugin_clovers-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_clovers-0.1.1/PKG-INFO` & `nonebot_plugin_clovers-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-clovers
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: KarisAya
 Author-email: 1048827424@qq.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-clovers Version: 0.1.1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-clovers Version: 0.1.2 Summary:
 Author: KarisAya Author-email: 1048827424@qq.com Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: clovers (>=0.1.2,<0.2.0) Requires-Dist: nonebot-adapter-onebot
 (>=2.4.3,<3.0.0) Requires-Dist: nonebot-adapter-qq (>=1.4.3,<2.0.0) Requires-
 Dist: nonebot2 (>=2.2.1,<3.0.0) Description-Content-Type: text/markdown
                                    _[_n_o_n_e_b_o_t_]
```

