# Comparing `tmp/nonebot_plugin_nai3-0.1.2.tar.gz` & `tmp/nonebot_plugin_nai3-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_nai3-0.1.2.tar", max compression
+gzip compressed data, was "nonebot_plugin_nai3-0.1.3.tar", max compression
```

## Comparing `nonebot_plugin_nai3-0.1.2.tar` & `nonebot_plugin_nai3-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1098 2024-04-13 00:11:40.913503 nonebot_plugin_nai3-0.1.2/LICENSE
--rw-r--r--   0        0        0    12762 2024-04-15 06:06:34.338313 nonebot_plugin_nai3-0.1.2/nonebot_plugin_nai3/__init__.py
--rw-r--r--   0        0        0      691 2024-04-15 03:42:07.432330 nonebot_plugin_nai3-0.1.2/nonebot_plugin_nai3/config.py
--rw-r--r--   0        0        0     2440 2024-04-14 23:34:30.728833 nonebot_plugin_nai3-0.1.2/nonebot_plugin_nai3/utils.py
--rw-r--r--   0        0        0     1071 2024-04-15 06:07:30.637070 nonebot_plugin_nai3-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     5132 2024-04-15 05:01:56.830191 nonebot_plugin_nai3-0.1.2/README.md
--rw-r--r--   0        0        0     5731 1970-01-01 00:00:00.000000 nonebot_plugin_nai3-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1098 2024-04-13 00:11:40.913503 nonebot_plugin_nai3-0.1.3/LICENSE
+-rw-r--r--   0        0        0    12717 2024-04-15 06:36:42.263990 nonebot_plugin_nai3-0.1.3/nonebot_plugin_nai3/__init__.py
+-rw-r--r--   0        0        0      691 2024-04-15 03:42:07.432330 nonebot_plugin_nai3-0.1.3/nonebot_plugin_nai3/config.py
+-rw-r--r--   0        0        0     2440 2024-04-14 23:34:30.728833 nonebot_plugin_nai3-0.1.3/nonebot_plugin_nai3/utils.py
+-rw-r--r--   0        0        0     1071 2024-04-15 06:37:14.171975 nonebot_plugin_nai3-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     5132 2024-04-15 05:01:56.830191 nonebot_plugin_nai3-0.1.3/README.md
+-rw-r--r--   0        0        0     5731 1970-01-01 00:00:00.000000 nonebot_plugin_nai3-0.1.3/PKG-INFO
```

### Comparing `nonebot_plugin_nai3-0.1.2/LICENSE` & `nonebot_plugin_nai3-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nai3-0.1.2/nonebot_plugin_nai3/__init__.py` & `nonebot_plugin_nai3-0.1.3/nonebot_plugin_nai3/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -215,30 +215,28 @@
                         "FEMALE_BREAST_EXPOSED",
                         "FEMALE_GENITALIA_EXPOSED",
                         "ANUS_EXPOSED",
                         "MALE_GENITALIA_EXPOSED",
                     ]:
                         safe = "R18"
                 if safe == "R18":
-                    await nai3.send(
-                        "图片已生成, 但检测到 R18 内容! 不可以涩涩!! 人家要火速告诉主人去!!!", at_sender=True
-                    )
+                    await nai3.send("图片已生成, 但检测到 R18 内容! 不可以涩涩!! 脑积水要告诉主人去!!!", at_sender=True)
                     if nai3_config.smms_token:
                         file = await smms.upload(Path("./data/nai3/temp.png"))
                         for superuser in bot.config.superusers:
                             await bot.call_api(
                                 "send_msg",
                                 **{
                                     "message": f"群: {gid}, 用户: {uid}, 画了一张涩图!\n{file.url}",
                                     "user_id": superuser,
                                 },
                             )
                             asyncio.sleep(3)
                     return
-            await nai3.send(f"种子: {seed}\n" + MessageSegment.image("./data/nai3/temp.png"), at_sender=True)
+            await nai3.send(f"种子: {seed}\n" + MessageSegment.image(Path("./data/nai3/temp.png")), at_sender=True)
             return
     except Exception as e:
         await nai3.finish(f"出现错误: {e}", at_sender=True)
 
 
 @nai3_black.handle()
 async def _(event: MessageEvent, msg: Message = CommandArg()):
```

### Comparing `nonebot_plugin_nai3-0.1.2/nonebot_plugin_nai3/config.py` & `nonebot_plugin_nai3-0.1.3/nonebot_plugin_nai3/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nai3-0.1.2/nonebot_plugin_nai3/utils.py` & `nonebot_plugin_nai3-0.1.3/nonebot_plugin_nai3/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nai3-0.1.2/pyproject.toml` & `nonebot_plugin_nai3-0.1.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-nai3"
-version = "0.1.2"
+version = "0.1.3"
 description = "通过 NovelAI 生成图片"
 authors = ["zhulinyv <zhulinyv2005@outlook.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_nai3"}]
 
 [tool.poetry.dependencies]
```

### Comparing `nonebot_plugin_nai3-0.1.2/README.md` & `nonebot_plugin_nai3-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nai3-0.1.2/PKG-INFO` & `nonebot_plugin_nai3-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-nai3
-Version: 0.1.2
+Version: 0.1.3
 Summary: 通过 NovelAI 生成图片
 License: MIT
 Author: zhulinyv
 Author-email: zhulinyv2005@outlook.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-nai3 Version: 0.1.2 Summary: éè¿
+Metadata-Version: 2.1 Name: nonebot-plugin-nai3 Version: 0.1.3 Summary: éè¿
 NovelAI çæå¾ç License: MIT Author: zhulinyv Author-email:
 zhulinyv2005@outlook.com Requires-Python: >=3.9,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: httpx (>=0.24.1,<0.25.0) Requires-Dist: nonebot-adapter-onebot
 (>=2.2.3,<3.0.0) Requires-Dist: nonebot-plugin-smms (>=0.1.0,<0.2.0) Requires-
```

