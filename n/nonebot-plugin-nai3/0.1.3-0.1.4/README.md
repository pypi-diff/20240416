# Comparing `tmp/nonebot_plugin_nai3-0.1.3.tar.gz` & `tmp/nonebot_plugin_nai3-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_nai3-0.1.3.tar", max compression
+gzip compressed data, was "nonebot_plugin_nai3-0.1.4.tar", max compression
```

## Comparing `nonebot_plugin_nai3-0.1.3.tar` & `nonebot_plugin_nai3-0.1.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1098 2024-04-13 00:11:40.913503 nonebot_plugin_nai3-0.1.3/LICENSE
--rw-r--r--   0        0        0    12717 2024-04-15 06:36:42.263990 nonebot_plugin_nai3-0.1.3/nonebot_plugin_nai3/__init__.py
--rw-r--r--   0        0        0      691 2024-04-15 03:42:07.432330 nonebot_plugin_nai3-0.1.3/nonebot_plugin_nai3/config.py
--rw-r--r--   0        0        0     2440 2024-04-14 23:34:30.728833 nonebot_plugin_nai3-0.1.3/nonebot_plugin_nai3/utils.py
--rw-r--r--   0        0        0     1071 2024-04-15 06:37:14.171975 nonebot_plugin_nai3-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     5132 2024-04-15 05:01:56.830191 nonebot_plugin_nai3-0.1.3/README.md
--rw-r--r--   0        0        0     5731 1970-01-01 00:00:00.000000 nonebot_plugin_nai3-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1098 2024-04-13 00:11:40.913503 nonebot_plugin_nai3-0.1.4/LICENSE
+-rw-r--r--   0        0        0    13288 2024-04-16 03:52:10.702983 nonebot_plugin_nai3-0.1.4/nonebot_plugin_nai3/__init__.py
+-rw-r--r--   0        0        0      802 2024-04-16 00:56:07.898683 nonebot_plugin_nai3-0.1.4/nonebot_plugin_nai3/config.py
+-rw-r--r--   0        0        0     2440 2024-04-14 23:34:30.728833 nonebot_plugin_nai3-0.1.4/nonebot_plugin_nai3/utils.py
+-rw-r--r--   0        0        0     1071 2024-04-16 03:52:59.576733 nonebot_plugin_nai3-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     5378 2024-04-16 01:05:53.720148 nonebot_plugin_nai3-0.1.4/README.md
+-rw-r--r--   0        0        0     5974 1970-01-01 00:00:00.000000 nonebot_plugin_nai3-0.1.4/PKG-INFO
```

### Comparing `nonebot_plugin_nai3-0.1.3/LICENSE` & `nonebot_plugin_nai3-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nai3-0.1.3/nonebot_plugin_nai3/__init__.py` & `nonebot_plugin_nai3-0.1.4/nonebot_plugin_nai3/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,48 +1,46 @@
 import asyncio
 import io
 import os
 import random
+import shutil
 import time
 import zipfile
 from argparse import Namespace
 from importlib.metadata import version
 from pathlib import Path
 
 import ujson as json
 from httpx import AsyncClient
-from nonebot import require
 from nonebot.adapters.onebot.v11 import (
     GROUP_ADMIN,
     GROUP_OWNER,
     Bot,
     Event,
     GroupMessageEvent,
     Message,
     MessageEvent,
     MessageSegment,
     PrivateMessageEvent,
 )
 from nonebot.log import logger
 from nonebot.params import CommandArg, ShellCommandArgs
 from nonebot.permission import SUPERUSER
-from nonebot.plugin import PluginMetadata
+from nonebot.plugin import PluginMetadata, require
 from nonebot.plugin.on import on_command, on_shell_command
 from nonebot.rule import ArgumentParser
 from nudenet import NudeDetector
 
 from .config import Config, nai3_config
 from .utils import format_str, get_at, headers, json_for_t2i, list_to_str, proxies
 
 require("nonebot_plugin_smms")
 from nonebot_plugin_smms import SMMS  # noqa: E402, F401
 
 ADMIN = SUPERUSER | GROUP_ADMIN | GROUP_OWNER
-nude_detector = NudeDetector()
-smms = SMMS()
 
 try:
     __version__ = version("nonebot_plugin_nai3")
 except Exception:
     __version__ = "0.0.0"
 
 __plugin_meta__ = PluginMetadata(
@@ -84,14 +82,18 @@
 nai3_help = on_command("nai3帮助", aliases={"nai3 帮助", "nai帮助", "nai 帮助"}, priority=25, block=True)
 
 cd = {}
 
 
 @nai3.handle()
 async def _(bot: Bot, event: MessageEvent, args: Namespace = ShellCommandArgs()):
+    # noneflow 加载报错, 移至这里实例化
+    nude_detector = NudeDetector()
+    smms = SMMS()
+
     # 获取群号和 QQ 号
     if isinstance(event, PrivateMessageEvent):
         gid = uid = str(event.user_id)
     elif isinstance(event, GroupMessageEvent):
         gid = str(event.group_id)
         uid = str(event.user_id)
     else:
@@ -141,19 +143,19 @@
                     round(nai3_config.nai3_cooltime_user - now_time + cd[gid]["cool_time"], 3)
                 ),
                 at_sender=True,
             )
         if cd[gid]["user"][uid]["limit"] <= 0:
             await nai3.finish("今天已经没次数了哦~", at_send=True)
 
-    # 组装 json 数据
     await nai3.send(
         "脑积水已收到绘画指令, 正在生成图片(剩余次数: {})...".format(cd[gid]["user"][uid]["limit"]), at_sender=True
     )
 
+    # 组装 json 数据
     json_for_t2i["input"] = format_str(list_to_str(args.prompt))
     resolution = args.resolution if args.resolution else "mb"
     if resolution == "mb":
         width = 832
         height = 1216
     elif resolution == "pc":
         width = 1216
@@ -175,14 +177,15 @@
     json_for_t2i["parameters"]["negative_prompt"] = (
         format_str(list_to_str(args.negative)) if args.negative else nai3_config.nai3_negative
     )
 
     logger.debug(">>>>>")
     logger.debug(json_for_t2i)
 
+    # 更新用户 CD
     now_time = time.time()
     cd[gid]["cool_time"] = now_time
     cd[gid]["user"][uid]["cool_time"] = now_time
 
     try:
         # 生成图片
         async with AsyncClient(proxies=proxies if nai3_config.nai3_proxy else None) as client:
@@ -197,14 +200,20 @@
                 logger.debug(response.status_code)
             logger.debug("<<<<<")
             with zipfile.ZipFile(io.BytesIO(response.content), mode="r") as zip:
                 with zip.open("image_0.png") as image:
                     with open("./data/nai3/temp.png", "wb") as f:
                         f.write(image.read())
 
+            # 保存到指定位置
+            if nai3_config.nai3_save:
+                if not os.path.exists(nai3_config.nai3_save_path):
+                    os.makedirs(nai3_config.nai3_save_path)
+                shutil.copyfile("./data/nai3/temp.png", Path(nai3_config.nai3_save_path) / f"{seed}.png")
+
             cd[gid]["user"][uid]["limit"] = (
                 999 if event.get_user_id() in bot.config.superusers else cd[gid]["user"][uid]["limit"] - 1
             )
 
             # 检测 R18
             if not nai3_config.nai3_r18:
                 body = nude_detector.detect("./data/nai3/temp.png")
@@ -218,23 +227,25 @@
                         "MALE_GENITALIA_EXPOSED",
                     ]:
                         safe = "R18"
                 if safe == "R18":
                     await nai3.send("图片已生成, 但检测到 R18 内容! 不可以涩涩!! 脑积水要告诉主人去!!!", at_sender=True)
                     if nai3_config.smms_token:
                         file = await smms.upload(Path("./data/nai3/temp.png"))
+                        if nai3_config.nai3_send_to_group:
+                            await nai3.send(f"只..只许这一次给你看看好啦!\n{file.url}", at_sender=True)
                         for superuser in bot.config.superusers:
                             await bot.call_api(
                                 "send_msg",
                                 **{
                                     "message": f"群: {gid}, 用户: {uid}, 画了一张涩图!\n{file.url}",
                                     "user_id": superuser,
                                 },
                             )
-                            asyncio.sleep(3)
+                            asyncio.sleep(1)
                     return
             await nai3.send(f"种子: {seed}\n" + MessageSegment.image(Path("./data/nai3/temp.png")), at_sender=True)
             return
     except Exception as e:
         await nai3.finish(f"出现错误: {e}", at_sender=True)
```

### Comparing `nonebot_plugin_nai3-0.1.3/nonebot_plugin_nai3/config.py` & `nonebot_plugin_nai3-0.1.4/nonebot_plugin_nai3/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,12 +8,15 @@
         "nsfw, lowres, {bad}, error, fewer, extra, missing, worst quality, jpeg artifacts, bad quality, watermark, unfinished, displeasing, chromatic aberration, signature, extra digits, artistic error, username, scan, [abstract]"  # noqa: E501
     )
     nai3_limit: int = 10
     nai3_cooltime_group: int = 30
     nai3_cooltime_user: int = 300
     nai3_proxy: str = None
     nai3_r18: bool = False
+    nai3_send_to_group: bool = True
+    nai3_save: bool = False
+    nai3_save_path: str = "./data/nai3/img"
     smms_api_url: str = "https://sm.ms/api/v2"
     smms_token: str = None
 
 
 nai3_config = get_plugin_config(Config)
```

### Comparing `nonebot_plugin_nai3-0.1.3/nonebot_plugin_nai3/utils.py` & `nonebot_plugin_nai3-0.1.4/nonebot_plugin_nai3/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nai3-0.1.3/pyproject.toml` & `nonebot_plugin_nai3-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-nai3"
-version = "0.1.3"
+version = "0.1.4"
 description = "通过 NovelAI 生成图片"
 authors = ["zhulinyv <zhulinyv2005@outlook.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_nai3"}]
 
 [tool.poetry.dependencies]
```

### Comparing `nonebot_plugin_nai3-0.1.3/README.md` & `nonebot_plugin_nai3-0.1.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -69,14 +69,17 @@
 | nai3_token | 是 | str | xxx | 请求头中必需的 token |
 | nai3_negative | 否 | str | nsfw,... | 负面提示词 |
 | nai3_limit | 否 | int | 10 | 每人最多生成次数 |
 | nai3_cooltime_group | 否 | int | 30 | 群聊画图冷却时间(单位: 秒) |
 | nai3_cooltime_user | 否 | int | 300 | 个人画图冷却时间(单位: 秒) |
 | nai3_proxy | 否 | str | None | post 请求生成图片使用的代理 |
 | nai3_r18 | 否 | bool | False | 是否允许 R18 图片(False 将会把图片链接发给超级用户) |
+| nai3_send_to_group | 否 | bool | True | 是否允许将图片链接发送到群 |
+| nai3_save | 否 | bool | "./data/nai3/img" | 是否将用户生成的图片保存 |
+| nai3_save_path | 否 | str | "./data/nai3/img" | 图片保存位置 |
 | SMMS_API_URL | 否 | str | "https://sm.ms/api/v2" | SMMS 图床 API 地址 |
 | SMMS_TOKEN | 否 | str | None | 不配置将损失一张 R18 图片(bushi) |
 
 ⚠️ token 的获取:
 
 - 1.登录 https://novelai.net/login
 - 2.F12 打开控制台并切换到控制台
@@ -139,15 +142,15 @@
 + [x] 上限功能
 + [x] 黑名单功能
 + [x] 代理
 + [x] R18 检测
 + [ ] 翻译
 + [x] 帮助指令
 + [x] 检测到 R18 图片生成链接并上报超级用户
-+ [ ] 图片保存
++ [x] 图片保存
 + [ ] ...
 
 ## 🤝 鸣谢
 
 本项目逐步迁移自 [Semi-Auto-NovelAI-to-Pixiv](https://github.com/zhulinyv/Semi-Auto-NovelAI-to-Pixiv)
 
 本项目使用 [nonebot-plugin-smms](https://github.com/mobyw/nonebot-plugin-smms) 上传图片
```

#### html2text {}

```diff
@@ -21,37 +21,41 @@
 | | nai3_token | æ¯ | str | xxx | è¯·æ±å¤´ä¸­å¿éç token | |
 nai3_negative | å¦ | str | nsfw,... | è´é¢æç¤ºè¯ | | nai3_limit | å¦ |
 int | 10 | æ¯äººæå¤çææ¬¡æ° | | nai3_cooltime_group | å¦ | int | 30 |
 ç¾¤èç»å¾å·å´æ¶é´(åä½: ç§) | | nai3_cooltime_user | å¦ | int | 300
 | ä¸ªäººç»å¾å·å´æ¶é´(åä½: ç§) | | nai3_proxy | å¦ | str | None |
 post è¯·æ±çæå¾çä½¿ç¨çä»£ç | | nai3_r18 | å¦ | bool | False |
 æ¯å¦åè®¸ R18 å¾ç(False å°ä¼æå¾çé¾æ¥åç»è¶çº§ç¨æ·) | |
-SMMS_API_URL | å¦ | str | "https://sm.ms/api/v2" | SMMS å¾åº API å°å | |
-SMMS_TOKEN | å¦ | str | None | ä¸éç½®å°æå¤±ä¸å¼  R18 å¾ç(bushi) |
-â ï¸ token çè·å: - 1.ç»å½ https://novelai.net/login - 2.F12
-æå¼æ§å¶å°å¹¶åæ¢å°æ§å¶å° - 3.è¾å¥ `console.log(JSON.parse
-(localStorage.session).auth_token)` åè½¦, è¿åçå­ç¬¦ä¸²å³ä¸º token - !
-[e3756ce75c6f6850efa633dbaa3a5ae6](https://github.com/zhulinyv/Semi-Auto-
-NovelAI-to-Pixiv/assets/66541860/502c9a49-6a73-446d-9401-e559628ad079) â ï¸
-SMMS token çè·å: - ç»å½SM.MS" - ç¹å»"Sign Up"æ³¨åä¸ä¸ªè´¦å·" -
-è¾å¥è´¦å·é®ç®±åå¯ç " - ç¹å»"User" > "Dashboard"" - ç¹å»"API Token",
-å°±å¯ä»¥çå°Token, å¤å¶å³å¯ä½¿ç¨" ## ð ä½¿ç¨ ``` æä»¤: nai3/nai
-åæ°: prompt æç¤ºè¯(æ¯æä½ åæ¬¢çç»é£ä¸²), é»è®¤: None -n/--
-negative è´é¢æç¤ºè¯, é»è®¤: nsfw,... -r/--resolution ç»å¸å½¢ç¶/
-åè¾¨ç, ["mb", "pc", "sq"] ä¸éä¸, é»è®¤: mb -s/--scale
-æç¤ºè¯ç¸å³æ§, é»è®¤: 5.0 -sm sm, é»è®¤: False -smdyn smdyn, é»è®¤:
-False --sampler éæ ·å¨, é»è®¤: k_euler --schedule åªå£°è®¡åè¡¨, é»è®¤:
-native ç¤ºä¾: nai3 1girl, loli, cute -r mb -s 5.0 è¿å: ``` ![img](./img/
-1.png) ``` æä»¤: nai3é»åå/naié»åå(éè¦è¶çº§ç¨æ·,
-ç¾¤ä¸»æç¾¤ç®¡çåæé) åæ°: æ·»å  æ·»å é»åå å é¤
-å é¤é»åå ç¨æ· æå®æ·»å ç±»å ç¾¤è æå®æ·»å ç±»å ç¾¤å·/
-QQå·/@sb. ç¤ºä¾: nai3é»ååæ·»å ç¨æ· @èç§¯æ°´ è¿å: ``` ![img](./
-img/2.png) ``` æä»¤: nai3å¸®å©/naiå¸®å© è¿å: å±ç¤ºä»¥ä¸å¸®å© ``` ##
-ð å¾å + [x] æçå¾ + [ ] å¾çå¾ + [x] èªå®ä¹åæ° + [ ]
-~~éååè½~~ + [x] å·å´åè½ + [x] ä¸éåè½ + [x] é»åååè½ +
-[x] ä»£ç + [x] R18 æ£æµ + [ ] ç¿»è¯ + [x] å¸®å©æä»¤ + [x] æ£æµå° R18
-å¾ççæé¾æ¥å¹¶ä¸æ¥è¶çº§ç¨æ· + [ ] å¾çä¿å­ + [ ] ... ## ð¤
-é¸£è°¢ æ¬é¡¹ç®éæ­¥è¿ç§»èª [Semi-Auto-NovelAI-to-Pixiv](https://
-github.com/zhulinyv/Semi-Auto-NovelAI-to-Pixiv) æ¬é¡¹ç®ä½¿ç¨ [nonebot-
-plugin-smms](https://github.com/mobyw/nonebot-plugin-smms) ä¸ä¼ å¾ç
+nai3_send_to_group | å¦ | bool | True |
+æ¯å¦åè®¸å°å¾çé¾æ¥åéå°ç¾¤ | | nai3_save | å¦ | bool | "./data/
+nai3/img" | æ¯å¦å°ç¨æ·çæçå¾çä¿å­ | | nai3_save_path | å¦ | str
+| "./data/nai3/img" | å¾çä¿å­ä½ç½® | | SMMS_API_URL | å¦ | str | "https:
+//sm.ms/api/v2" | SMMS å¾åº API å°å | | SMMS_TOKEN | å¦ | str | None |
+ä¸éç½®å°æå¤±ä¸å¼  R18 å¾ç(bushi) | â ï¸ token çè·å: - 1.ç»å½
+https://novelai.net/login - 2.F12 æå¼æ§å¶å°å¹¶åæ¢å°æ§å¶å° -
+3.è¾å¥ `console.log(JSON.parse(localStorage.session).auth_token)` åè½¦,
+è¿åçå­ç¬¦ä¸²å³ä¸º token - ![e3756ce75c6f6850efa633dbaa3a5ae6](https://
+github.com/zhulinyv/Semi-Auto-NovelAI-to-Pixiv/assets/66541860/502c9a49-6a73-
+446d-9401-e559628ad079) â ï¸ SMMS token çè·å: - ç»å½SM.MS" -
+ç¹å»"Sign Up"æ³¨åä¸ä¸ªè´¦å·" - è¾å¥è´¦å·é®ç®±åå¯ç " -
+ç¹å»"User" > "Dashboard"" - ç¹å»"API Token", å°±å¯ä»¥çå°Token,
+å¤å¶å³å¯ä½¿ç¨" ## ð ä½¿ç¨ ``` æä»¤: nai3/nai åæ°: prompt
+æç¤ºè¯(æ¯æä½ åæ¬¢çç»é£ä¸²), é»è®¤: None -n/--negative
+è´é¢æç¤ºè¯, é»è®¤: nsfw,... -r/--resolution ç»å¸å½¢ç¶/åè¾¨ç,
+["mb", "pc", "sq"] ä¸éä¸, é»è®¤: mb -s/--scale æç¤ºè¯ç¸å³æ§, é»è®¤:
+5.0 -sm sm, é»è®¤: False -smdyn smdyn, é»è®¤: False --sampler éæ ·å¨,
+é»è®¤: k_euler --schedule åªå£°è®¡åè¡¨, é»è®¤: native ç¤ºä¾: nai3 1girl,
+loli, cute -r mb -s 5.0 è¿å: ``` ![img](./img/1.png) ``` æä»¤:
+nai3é»åå/naié»åå(éè¦è¶çº§ç¨æ·, ç¾¤ä¸»æç¾¤ç®¡çåæé)
+åæ°: æ·»å  æ·»å é»åå å é¤ å é¤é»åå ç¨æ· æå®æ·»å ç±»å
+ç¾¤è æå®æ·»å ç±»å ç¾¤å·/QQå·/@sb. ç¤ºä¾: nai3é»ååæ·»å ç¨æ·
+@èç§¯æ°´ è¿å: ``` ![img](./img/2.png) ``` æä»¤: nai3å¸®å©/naiå¸®å©
+è¿å: å±ç¤ºä»¥ä¸å¸®å© ``` ## ð å¾å + [x] æçå¾ + [ ] å¾çå¾ +
+[x] èªå®ä¹åæ° + [ ] ~~éååè½~~ + [x] å·å´åè½ + [x]
+ä¸éåè½ + [x] é»åååè½ + [x] ä»£ç + [x] R18 æ£æµ + [ ] ç¿»è¯ +
+[x] å¸®å©æä»¤ + [x] æ£æµå° R18 å¾ççæé¾æ¥å¹¶ä¸æ¥è¶çº§ç¨æ· +
+[x] å¾çä¿å­ + [ ] ... ## ð¤ é¸£è°¢ æ¬é¡¹ç®éæ­¥è¿ç§»èª [Semi-Auto-
+NovelAI-to-Pixiv](https://github.com/zhulinyv/Semi-Auto-NovelAI-to-Pixiv)
+æ¬é¡¹ç®ä½¿ç¨ [nonebot-plugin-smms](https://github.com/mobyw/nonebot-plugin-
+smms) ä¸ä¼ å¾ç
 ===============================================================================
 [https://count.getloli.com/get/@zhulinyv?theme=rule34]
```

### Comparing `nonebot_plugin_nai3-0.1.3/PKG-INFO` & `nonebot_plugin_nai3-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-nai3
-Version: 0.1.3
+Version: 0.1.4
 Summary: 通过 NovelAI 生成图片
 License: MIT
 Author: zhulinyv
 Author-email: zhulinyv2005@outlook.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -90,14 +90,17 @@
 | nai3_token | 是 | str | xxx | 请求头中必需的 token |
 | nai3_negative | 否 | str | nsfw,... | 负面提示词 |
 | nai3_limit | 否 | int | 10 | 每人最多生成次数 |
 | nai3_cooltime_group | 否 | int | 30 | 群聊画图冷却时间(单位: 秒) |
 | nai3_cooltime_user | 否 | int | 300 | 个人画图冷却时间(单位: 秒) |
 | nai3_proxy | 否 | str | None | post 请求生成图片使用的代理 |
 | nai3_r18 | 否 | bool | False | 是否允许 R18 图片(False 将会把图片链接发给超级用户) |
+| nai3_send_to_group | 否 | bool | True | 是否允许将图片链接发送到群 |
+| nai3_save | 否 | bool | "./data/nai3/img" | 是否将用户生成的图片保存 |
+| nai3_save_path | 否 | str | "./data/nai3/img" | 图片保存位置 |
 | SMMS_API_URL | 否 | str | "https://sm.ms/api/v2" | SMMS 图床 API 地址 |
 | SMMS_TOKEN | 否 | str | None | 不配置将损失一张 R18 图片(bushi) |
 
 ⚠️ token 的获取:
 
 - 1.登录 https://novelai.net/login
 - 2.F12 打开控制台并切换到控制台
@@ -160,15 +163,15 @@
 + [x] 上限功能
 + [x] 黑名单功能
 + [x] 代理
 + [x] R18 检测
 + [ ] 翻译
 + [x] 帮助指令
 + [x] 检测到 R18 图片生成链接并上报超级用户
-+ [ ] 图片保存
++ [x] 图片保存
 + [ ] ...
 
 ## 🤝 鸣谢
 
 本项目逐步迁移自 [Semi-Auto-NovelAI-to-Pixiv](https://github.com/zhulinyv/Semi-Auto-NovelAI-to-Pixiv)
 
 本项目使用 [nonebot-plugin-smms](https://github.com/mobyw/nonebot-plugin-smms) 上传图片
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-nai3 Version: 0.1.3 Summary: éè¿
+Metadata-Version: 2.1 Name: nonebot-plugin-nai3 Version: 0.1.4 Summary: éè¿
 NovelAI çæå¾ç License: MIT Author: zhulinyv Author-email:
 zhulinyv2005@outlook.com Requires-Python: >=3.9,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: httpx (>=0.24.1,<0.25.0) Requires-Dist: nonebot-adapter-onebot
 (>=2.2.3,<3.0.0) Requires-Dist: nonebot-plugin-smms (>=0.1.0,<0.2.0) Requires-
@@ -31,37 +31,41 @@
 | | nai3_token | æ¯ | str | xxx | è¯·æ±å¤´ä¸­å¿éç token | |
 nai3_negative | å¦ | str | nsfw,... | è´é¢æç¤ºè¯ | | nai3_limit | å¦ |
 int | 10 | æ¯äººæå¤çææ¬¡æ° | | nai3_cooltime_group | å¦ | int | 30 |
 ç¾¤èç»å¾å·å´æ¶é´(åä½: ç§) | | nai3_cooltime_user | å¦ | int | 300
 | ä¸ªäººç»å¾å·å´æ¶é´(åä½: ç§) | | nai3_proxy | å¦ | str | None |
 post è¯·æ±çæå¾çä½¿ç¨çä»£ç | | nai3_r18 | å¦ | bool | False |
 æ¯å¦åè®¸ R18 å¾ç(False å°ä¼æå¾çé¾æ¥åç»è¶çº§ç¨æ·) | |
-SMMS_API_URL | å¦ | str | "https://sm.ms/api/v2" | SMMS å¾åº API å°å | |
-SMMS_TOKEN | å¦ | str | None | ä¸éç½®å°æå¤±ä¸å¼  R18 å¾ç(bushi) |
-â ï¸ token çè·å: - 1.ç»å½ https://novelai.net/login - 2.F12
-æå¼æ§å¶å°å¹¶åæ¢å°æ§å¶å° - 3.è¾å¥ `console.log(JSON.parse
-(localStorage.session).auth_token)` åè½¦, è¿åçå­ç¬¦ä¸²å³ä¸º token - !
-[e3756ce75c6f6850efa633dbaa3a5ae6](https://github.com/zhulinyv/Semi-Auto-
-NovelAI-to-Pixiv/assets/66541860/502c9a49-6a73-446d-9401-e559628ad079) â ï¸
-SMMS token çè·å: - ç»å½SM.MS" - ç¹å»"Sign Up"æ³¨åä¸ä¸ªè´¦å·" -
-è¾å¥è´¦å·é®ç®±åå¯ç " - ç¹å»"User" > "Dashboard"" - ç¹å»"API Token",
-å°±å¯ä»¥çå°Token, å¤å¶å³å¯ä½¿ç¨" ## ð ä½¿ç¨ ``` æä»¤: nai3/nai
-åæ°: prompt æç¤ºè¯(æ¯æä½ åæ¬¢çç»é£ä¸²), é»è®¤: None -n/--
-negative è´é¢æç¤ºè¯, é»è®¤: nsfw,... -r/--resolution ç»å¸å½¢ç¶/
-åè¾¨ç, ["mb", "pc", "sq"] ä¸éä¸, é»è®¤: mb -s/--scale
-æç¤ºè¯ç¸å³æ§, é»è®¤: 5.0 -sm sm, é»è®¤: False -smdyn smdyn, é»è®¤:
-False --sampler éæ ·å¨, é»è®¤: k_euler --schedule åªå£°è®¡åè¡¨, é»è®¤:
-native ç¤ºä¾: nai3 1girl, loli, cute -r mb -s 5.0 è¿å: ``` ![img](./img/
-1.png) ``` æä»¤: nai3é»åå/naié»åå(éè¦è¶çº§ç¨æ·,
-ç¾¤ä¸»æç¾¤ç®¡çåæé) åæ°: æ·»å  æ·»å é»åå å é¤
-å é¤é»åå ç¨æ· æå®æ·»å ç±»å ç¾¤è æå®æ·»å ç±»å ç¾¤å·/
-QQå·/@sb. ç¤ºä¾: nai3é»ååæ·»å ç¨æ· @èç§¯æ°´ è¿å: ``` ![img](./
-img/2.png) ``` æä»¤: nai3å¸®å©/naiå¸®å© è¿å: å±ç¤ºä»¥ä¸å¸®å© ``` ##
-ð å¾å + [x] æçå¾ + [ ] å¾çå¾ + [x] èªå®ä¹åæ° + [ ]
-~~éååè½~~ + [x] å·å´åè½ + [x] ä¸éåè½ + [x] é»åååè½ +
-[x] ä»£ç + [x] R18 æ£æµ + [ ] ç¿»è¯ + [x] å¸®å©æä»¤ + [x] æ£æµå° R18
-å¾ççæé¾æ¥å¹¶ä¸æ¥è¶çº§ç¨æ· + [ ] å¾çä¿å­ + [ ] ... ## ð¤
-é¸£è°¢ æ¬é¡¹ç®éæ­¥è¿ç§»èª [Semi-Auto-NovelAI-to-Pixiv](https://
-github.com/zhulinyv/Semi-Auto-NovelAI-to-Pixiv) æ¬é¡¹ç®ä½¿ç¨ [nonebot-
-plugin-smms](https://github.com/mobyw/nonebot-plugin-smms) ä¸ä¼ å¾ç
+nai3_send_to_group | å¦ | bool | True |
+æ¯å¦åè®¸å°å¾çé¾æ¥åéå°ç¾¤ | | nai3_save | å¦ | bool | "./data/
+nai3/img" | æ¯å¦å°ç¨æ·çæçå¾çä¿å­ | | nai3_save_path | å¦ | str
+| "./data/nai3/img" | å¾çä¿å­ä½ç½® | | SMMS_API_URL | å¦ | str | "https:
+//sm.ms/api/v2" | SMMS å¾åº API å°å | | SMMS_TOKEN | å¦ | str | None |
+ä¸éç½®å°æå¤±ä¸å¼  R18 å¾ç(bushi) | â ï¸ token çè·å: - 1.ç»å½
+https://novelai.net/login - 2.F12 æå¼æ§å¶å°å¹¶åæ¢å°æ§å¶å° -
+3.è¾å¥ `console.log(JSON.parse(localStorage.session).auth_token)` åè½¦,
+è¿åçå­ç¬¦ä¸²å³ä¸º token - ![e3756ce75c6f6850efa633dbaa3a5ae6](https://
+github.com/zhulinyv/Semi-Auto-NovelAI-to-Pixiv/assets/66541860/502c9a49-6a73-
+446d-9401-e559628ad079) â ï¸ SMMS token çè·å: - ç»å½SM.MS" -
+ç¹å»"Sign Up"æ³¨åä¸ä¸ªè´¦å·" - è¾å¥è´¦å·é®ç®±åå¯ç " -
+ç¹å»"User" > "Dashboard"" - ç¹å»"API Token", å°±å¯ä»¥çå°Token,
+å¤å¶å³å¯ä½¿ç¨" ## ð ä½¿ç¨ ``` æä»¤: nai3/nai åæ°: prompt
+æç¤ºè¯(æ¯æä½ åæ¬¢çç»é£ä¸²), é»è®¤: None -n/--negative
+è´é¢æç¤ºè¯, é»è®¤: nsfw,... -r/--resolution ç»å¸å½¢ç¶/åè¾¨ç,
+["mb", "pc", "sq"] ä¸éä¸, é»è®¤: mb -s/--scale æç¤ºè¯ç¸å³æ§, é»è®¤:
+5.0 -sm sm, é»è®¤: False -smdyn smdyn, é»è®¤: False --sampler éæ ·å¨,
+é»è®¤: k_euler --schedule åªå£°è®¡åè¡¨, é»è®¤: native ç¤ºä¾: nai3 1girl,
+loli, cute -r mb -s 5.0 è¿å: ``` ![img](./img/1.png) ``` æä»¤:
+nai3é»åå/naié»åå(éè¦è¶çº§ç¨æ·, ç¾¤ä¸»æç¾¤ç®¡çåæé)
+åæ°: æ·»å  æ·»å é»åå å é¤ å é¤é»åå ç¨æ· æå®æ·»å ç±»å
+ç¾¤è æå®æ·»å ç±»å ç¾¤å·/QQå·/@sb. ç¤ºä¾: nai3é»ååæ·»å ç¨æ·
+@èç§¯æ°´ è¿å: ``` ![img](./img/2.png) ``` æä»¤: nai3å¸®å©/naiå¸®å©
+è¿å: å±ç¤ºä»¥ä¸å¸®å© ``` ## ð å¾å + [x] æçå¾ + [ ] å¾çå¾ +
+[x] èªå®ä¹åæ° + [ ] ~~éååè½~~ + [x] å·å´åè½ + [x]
+ä¸éåè½ + [x] é»åååè½ + [x] ä»£ç + [x] R18 æ£æµ + [ ] ç¿»è¯ +
+[x] å¸®å©æä»¤ + [x] æ£æµå° R18 å¾ççæé¾æ¥å¹¶ä¸æ¥è¶çº§ç¨æ· +
+[x] å¾çä¿å­ + [ ] ... ## ð¤ é¸£è°¢ æ¬é¡¹ç®éæ­¥è¿ç§»èª [Semi-Auto-
+NovelAI-to-Pixiv](https://github.com/zhulinyv/Semi-Auto-NovelAI-to-Pixiv)
+æ¬é¡¹ç®ä½¿ç¨ [nonebot-plugin-smms](https://github.com/mobyw/nonebot-plugin-
+smms) ä¸ä¼ å¾ç
 ===============================================================================
 [https://count.getloli.com/get/@zhulinyv?theme=rule34]
```

