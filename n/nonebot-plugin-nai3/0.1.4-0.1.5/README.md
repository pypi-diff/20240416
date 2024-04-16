# Comparing `tmp/nonebot_plugin_nai3-0.1.4.tar.gz` & `tmp/nonebot_plugin_nai3-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_nai3-0.1.4.tar", max compression
+gzip compressed data, was "nonebot_plugin_nai3-0.1.5.tar", max compression
```

## Comparing `nonebot_plugin_nai3-0.1.4.tar` & `nonebot_plugin_nai3-0.1.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1098 2024-04-13 00:11:40.913503 nonebot_plugin_nai3-0.1.4/LICENSE
--rw-r--r--   0        0        0    13288 2024-04-16 03:52:10.702983 nonebot_plugin_nai3-0.1.4/nonebot_plugin_nai3/__init__.py
--rw-r--r--   0        0        0      802 2024-04-16 00:56:07.898683 nonebot_plugin_nai3-0.1.4/nonebot_plugin_nai3/config.py
--rw-r--r--   0        0        0     2440 2024-04-14 23:34:30.728833 nonebot_plugin_nai3-0.1.4/nonebot_plugin_nai3/utils.py
--rw-r--r--   0        0        0     1071 2024-04-16 03:52:59.576733 nonebot_plugin_nai3-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     5378 2024-04-16 01:05:53.720148 nonebot_plugin_nai3-0.1.4/README.md
--rw-r--r--   0        0        0     5974 1970-01-01 00:00:00.000000 nonebot_plugin_nai3-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1098 2024-04-13 00:11:40.913503 nonebot_plugin_nai3-0.1.5/LICENSE
+-rw-r--r--   0        0        0    13228 2024-04-16 04:20:39.881369 nonebot_plugin_nai3-0.1.5/nonebot_plugin_nai3/__init__.py
+-rw-r--r--   0        0        0      802 2024-04-16 00:56:07.898683 nonebot_plugin_nai3-0.1.5/nonebot_plugin_nai3/config.py
+-rw-r--r--   0        0        0     2440 2024-04-14 23:34:30.728833 nonebot_plugin_nai3-0.1.5/nonebot_plugin_nai3/utils.py
+-rw-r--r--   0        0        0     1071 2024-04-16 04:21:05.714080 nonebot_plugin_nai3-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     5370 2024-04-16 04:03:22.401850 nonebot_plugin_nai3-0.1.5/README.md
+-rw-r--r--   0        0        0     5966 1970-01-01 00:00:00.000000 nonebot_plugin_nai3-0.1.5/PKG-INFO
```

### Comparing `nonebot_plugin_nai3-0.1.4/LICENSE` & `nonebot_plugin_nai3-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nai3-0.1.4/nonebot_plugin_nai3/__init__.py` & `nonebot_plugin_nai3-0.1.5/nonebot_plugin_nai3/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,16 @@
 from .config import Config, nai3_config
 from .utils import format_str, get_at, headers, json_for_t2i, list_to_str, proxies
 
 require("nonebot_plugin_smms")
 from nonebot_plugin_smms import SMMS  # noqa: E402, F401
 
 ADMIN = SUPERUSER | GROUP_ADMIN | GROUP_OWNER
+nude_detector = NudeDetector()
+smms = SMMS()
 
 try:
     __version__ = version("nonebot_plugin_nai3")
 except Exception:
     __version__ = "0.0.0"
 
 __plugin_meta__ = PluginMetadata(
@@ -82,17 +84,14 @@
 nai3_help = on_command("nai3帮助", aliases={"nai3 帮助", "nai帮助", "nai 帮助"}, priority=25, block=True)
 
 cd = {}
 
 
 @nai3.handle()
 async def _(bot: Bot, event: MessageEvent, args: Namespace = ShellCommandArgs()):
-    # noneflow 加载报错, 移至这里实例化
-    nude_detector = NudeDetector()
-    smms = SMMS()
 
     # 获取群号和 QQ 号
     if isinstance(event, PrivateMessageEvent):
         gid = uid = str(event.user_id)
     elif isinstance(event, GroupMessageEvent):
         gid = str(event.group_id)
         uid = str(event.user_id)
```

### Comparing `nonebot_plugin_nai3-0.1.4/nonebot_plugin_nai3/config.py` & `nonebot_plugin_nai3-0.1.5/nonebot_plugin_nai3/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nai3-0.1.4/nonebot_plugin_nai3/utils.py` & `nonebot_plugin_nai3-0.1.5/nonebot_plugin_nai3/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nai3-0.1.4/pyproject.toml` & `nonebot_plugin_nai3-0.1.5/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-nai3"
-version = "0.1.4"
+version = "0.1.5"
 description = "通过 NovelAI 生成图片"
 authors = ["zhulinyv <zhulinyv2005@outlook.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_nai3"}]
 
 [tool.poetry.dependencies]
```

### Comparing `nonebot_plugin_nai3-0.1.4/README.md` & `nonebot_plugin_nai3-0.1.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -62,23 +62,23 @@
 
 ## ⚙️ 配置
 
 在 nonebot2 项目的`.env`文件中添加下表中的必填配置
 
 | 配置项 | 必填 | 类型 | 默认值 | 说明 |
 |:-----:|:----:|:----:|:----:|:----:|
-| nai3_token | 是 | str | xxx | 请求头中必需的 token |
-| nai3_negative | 否 | str | nsfw,... | 负面提示词 |
+| nai3_token | 是 | str | "xxx" | 请求头中必需的 token |
+| nai3_negative | 否 | str | "nsfw,..." | 负面提示词 |
 | nai3_limit | 否 | int | 10 | 每人最多生成次数 |
 | nai3_cooltime_group | 否 | int | 30 | 群聊画图冷却时间(单位: 秒) |
 | nai3_cooltime_user | 否 | int | 300 | 个人画图冷却时间(单位: 秒) |
 | nai3_proxy | 否 | str | None | post 请求生成图片使用的代理 |
 | nai3_r18 | 否 | bool | False | 是否允许 R18 图片(False 将会把图片链接发给超级用户) |
 | nai3_send_to_group | 否 | bool | True | 是否允许将图片链接发送到群 |
-| nai3_save | 否 | bool | "./data/nai3/img" | 是否将用户生成的图片保存 |
+| nai3_save | 否 | bool | False | 是否将用户生成的图片保存 |
 | nai3_save_path | 否 | str | "./data/nai3/img" | 图片保存位置 |
 | SMMS_API_URL | 否 | str | "https://sm.ms/api/v2" | SMMS 图床 API 地址 |
 | SMMS_TOKEN | 否 | str | None | 不配置将损失一张 R18 图片(bushi) |
 
 ⚠️ token 的获取:
 
 - 1.登录 https://novelai.net/login
```

#### html2text {}

```diff
@@ -14,26 +14,26 @@
 æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
 pip pip install nonebot-plugin-nai3 pdm pdm add nonebot-plugin-nai3 poetry
 poetry add nonebot-plugin-nai3 conda conda install nonebot-plugin-nai3 æå¼
 nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `[tool.nonebot]`
 é¨åè¿½å åå¥ plugins = ["nonebot_plugin_hoshino_sign"] ## âï¸ éç½®
 å¨ nonebot2 é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½® | éç½®é¡¹
 | å¿å¡« | ç±»å | é»è®¤å¼ | è¯´æ | |:-----:|:----:|:----:|:----:|:----:
-| | nai3_token | æ¯ | str | xxx | è¯·æ±å¤´ä¸­å¿éç token | |
-nai3_negative | å¦ | str | nsfw,... | è´é¢æç¤ºè¯ | | nai3_limit | å¦ |
+| | nai3_token | æ¯ | str | "xxx" | è¯·æ±å¤´ä¸­å¿éç token | |
+nai3_negative | å¦ | str | "nsfw,..." | è´é¢æç¤ºè¯ | | nai3_limit | å¦ |
 int | 10 | æ¯äººæå¤çææ¬¡æ° | | nai3_cooltime_group | å¦ | int | 30 |
 ç¾¤èç»å¾å·å´æ¶é´(åä½: ç§) | | nai3_cooltime_user | å¦ | int | 300
 | ä¸ªäººç»å¾å·å´æ¶é´(åä½: ç§) | | nai3_proxy | å¦ | str | None |
 post è¯·æ±çæå¾çä½¿ç¨çä»£ç | | nai3_r18 | å¦ | bool | False |
 æ¯å¦åè®¸ R18 å¾ç(False å°ä¼æå¾çé¾æ¥åç»è¶çº§ç¨æ·) | |
 nai3_send_to_group | å¦ | bool | True |
-æ¯å¦åè®¸å°å¾çé¾æ¥åéå°ç¾¤ | | nai3_save | å¦ | bool | "./data/
-nai3/img" | æ¯å¦å°ç¨æ·çæçå¾çä¿å­ | | nai3_save_path | å¦ | str
-| "./data/nai3/img" | å¾çä¿å­ä½ç½® | | SMMS_API_URL | å¦ | str | "https:
-//sm.ms/api/v2" | SMMS å¾åº API å°å | | SMMS_TOKEN | å¦ | str | None |
+æ¯å¦åè®¸å°å¾çé¾æ¥åéå°ç¾¤ | | nai3_save | å¦ | bool | False |
+æ¯å¦å°ç¨æ·çæçå¾çä¿å­ | | nai3_save_path | å¦ | str | "./data/
+nai3/img" | å¾çä¿å­ä½ç½® | | SMMS_API_URL | å¦ | str | "https://sm.ms/
+api/v2" | SMMS å¾åº API å°å | | SMMS_TOKEN | å¦ | str | None |
 ä¸éç½®å°æå¤±ä¸å¼  R18 å¾ç(bushi) | â ï¸ token çè·å: - 1.ç»å½
 https://novelai.net/login - 2.F12 æå¼æ§å¶å°å¹¶åæ¢å°æ§å¶å° -
 3.è¾å¥ `console.log(JSON.parse(localStorage.session).auth_token)` åè½¦,
 è¿åçå­ç¬¦ä¸²å³ä¸º token - ![e3756ce75c6f6850efa633dbaa3a5ae6](https://
 github.com/zhulinyv/Semi-Auto-NovelAI-to-Pixiv/assets/66541860/502c9a49-6a73-
 446d-9401-e559628ad079) â ï¸ SMMS token çè·å: - ç»å½SM.MS" -
 ç¹å»"Sign Up"æ³¨åä¸ä¸ªè´¦å·" - è¾å¥è´¦å·é®ç®±åå¯ç " -
```

### Comparing `nonebot_plugin_nai3-0.1.4/PKG-INFO` & `nonebot_plugin_nai3-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-nai3
-Version: 0.1.4
+Version: 0.1.5
 Summary: 通过 NovelAI 生成图片
 License: MIT
 Author: zhulinyv
 Author-email: zhulinyv2005@outlook.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -83,23 +83,23 @@
 
 ## ⚙️ 配置
 
 在 nonebot2 项目的`.env`文件中添加下表中的必填配置
 
 | 配置项 | 必填 | 类型 | 默认值 | 说明 |
 |:-----:|:----:|:----:|:----:|:----:|
-| nai3_token | 是 | str | xxx | 请求头中必需的 token |
-| nai3_negative | 否 | str | nsfw,... | 负面提示词 |
+| nai3_token | 是 | str | "xxx" | 请求头中必需的 token |
+| nai3_negative | 否 | str | "nsfw,..." | 负面提示词 |
 | nai3_limit | 否 | int | 10 | 每人最多生成次数 |
 | nai3_cooltime_group | 否 | int | 30 | 群聊画图冷却时间(单位: 秒) |
 | nai3_cooltime_user | 否 | int | 300 | 个人画图冷却时间(单位: 秒) |
 | nai3_proxy | 否 | str | None | post 请求生成图片使用的代理 |
 | nai3_r18 | 否 | bool | False | 是否允许 R18 图片(False 将会把图片链接发给超级用户) |
 | nai3_send_to_group | 否 | bool | True | 是否允许将图片链接发送到群 |
-| nai3_save | 否 | bool | "./data/nai3/img" | 是否将用户生成的图片保存 |
+| nai3_save | 否 | bool | False | 是否将用户生成的图片保存 |
 | nai3_save_path | 否 | str | "./data/nai3/img" | 图片保存位置 |
 | SMMS_API_URL | 否 | str | "https://sm.ms/api/v2" | SMMS 图床 API 地址 |
 | SMMS_TOKEN | 否 | str | None | 不配置将损失一张 R18 图片(bushi) |
 
 ⚠️ token 的获取:
 
 - 1.登录 https://novelai.net/login
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-nai3 Version: 0.1.4 Summary: éè¿
+Metadata-Version: 2.1 Name: nonebot-plugin-nai3 Version: 0.1.5 Summary: éè¿
 NovelAI çæå¾ç License: MIT Author: zhulinyv Author-email:
 zhulinyv2005@outlook.com Requires-Python: >=3.9,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: httpx (>=0.24.1,<0.25.0) Requires-Dist: nonebot-adapter-onebot
 (>=2.2.3,<3.0.0) Requires-Dist: nonebot-plugin-smms (>=0.1.0,<0.2.0) Requires-
@@ -24,26 +24,26 @@
 æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
 pip pip install nonebot-plugin-nai3 pdm pdm add nonebot-plugin-nai3 poetry
 poetry add nonebot-plugin-nai3 conda conda install nonebot-plugin-nai3 æå¼
 nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `[tool.nonebot]`
 é¨åè¿½å åå¥ plugins = ["nonebot_plugin_hoshino_sign"] ## âï¸ éç½®
 å¨ nonebot2 é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½® | éç½®é¡¹
 | å¿å¡« | ç±»å | é»è®¤å¼ | è¯´æ | |:-----:|:----:|:----:|:----:|:----:
-| | nai3_token | æ¯ | str | xxx | è¯·æ±å¤´ä¸­å¿éç token | |
-nai3_negative | å¦ | str | nsfw,... | è´é¢æç¤ºè¯ | | nai3_limit | å¦ |
+| | nai3_token | æ¯ | str | "xxx" | è¯·æ±å¤´ä¸­å¿éç token | |
+nai3_negative | å¦ | str | "nsfw,..." | è´é¢æç¤ºè¯ | | nai3_limit | å¦ |
 int | 10 | æ¯äººæå¤çææ¬¡æ° | | nai3_cooltime_group | å¦ | int | 30 |
 ç¾¤èç»å¾å·å´æ¶é´(åä½: ç§) | | nai3_cooltime_user | å¦ | int | 300
 | ä¸ªäººç»å¾å·å´æ¶é´(åä½: ç§) | | nai3_proxy | å¦ | str | None |
 post è¯·æ±çæå¾çä½¿ç¨çä»£ç | | nai3_r18 | å¦ | bool | False |
 æ¯å¦åè®¸ R18 å¾ç(False å°ä¼æå¾çé¾æ¥åç»è¶çº§ç¨æ·) | |
 nai3_send_to_group | å¦ | bool | True |
-æ¯å¦åè®¸å°å¾çé¾æ¥åéå°ç¾¤ | | nai3_save | å¦ | bool | "./data/
-nai3/img" | æ¯å¦å°ç¨æ·çæçå¾çä¿å­ | | nai3_save_path | å¦ | str
-| "./data/nai3/img" | å¾çä¿å­ä½ç½® | | SMMS_API_URL | å¦ | str | "https:
-//sm.ms/api/v2" | SMMS å¾åº API å°å | | SMMS_TOKEN | å¦ | str | None |
+æ¯å¦åè®¸å°å¾çé¾æ¥åéå°ç¾¤ | | nai3_save | å¦ | bool | False |
+æ¯å¦å°ç¨æ·çæçå¾çä¿å­ | | nai3_save_path | å¦ | str | "./data/
+nai3/img" | å¾çä¿å­ä½ç½® | | SMMS_API_URL | å¦ | str | "https://sm.ms/
+api/v2" | SMMS å¾åº API å°å | | SMMS_TOKEN | å¦ | str | None |
 ä¸éç½®å°æå¤±ä¸å¼  R18 å¾ç(bushi) | â ï¸ token çè·å: - 1.ç»å½
 https://novelai.net/login - 2.F12 æå¼æ§å¶å°å¹¶åæ¢å°æ§å¶å° -
 3.è¾å¥ `console.log(JSON.parse(localStorage.session).auth_token)` åè½¦,
 è¿åçå­ç¬¦ä¸²å³ä¸º token - ![e3756ce75c6f6850efa633dbaa3a5ae6](https://
 github.com/zhulinyv/Semi-Auto-NovelAI-to-Pixiv/assets/66541860/502c9a49-6a73-
 446d-9401-e559628ad079) â ï¸ SMMS token çè·å: - ç»å½SM.MS" -
 ç¹å»"Sign Up"æ³¨åä¸ä¸ªè´¦å·" - è¾å¥è´¦å·é®ç®±åå¯ç " -
```

