# Comparing `tmp/nonebot_plugin_disconnect_notice-0.2.0.tar.gz` & `tmp/nonebot_plugin_disconnect_notice-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_disconnect_notice-0.2.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_disconnect_notice-0.2.1.tar", max compression
```

## Comparing `nonebot_plugin_disconnect_notice-0.2.0.tar` & `nonebot_plugin_disconnect_notice-0.2.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1066 2024-04-08 08:32:31.468409 nonebot_plugin_disconnect_notice-0.2.0/LICENSE
--rw-r--r--   0        0        0     5782 2024-04-08 08:32:31.468409 nonebot_plugin_disconnect_notice-0.2.0/README.md
--rw-r--r--   0        0        0     3606 2024-04-08 08:32:31.472409 nonebot_plugin_disconnect_notice-0.2.0/nonebot_plugin_disconnect_notice/__init__.py
--rw-r--r--   0        0        0      797 2024-04-08 08:32:31.472409 nonebot_plugin_disconnect_notice-0.2.0/nonebot_plugin_disconnect_notice/config.py
--rw-r--r--   0        0        0      784 2024-04-08 08:32:31.472409 nonebot_plugin_disconnect_notice-0.2.0/nonebot_plugin_disconnect_notice/dataClass.py
--rw-r--r--   0        0        0     2102 2024-04-08 08:32:31.472409 nonebot_plugin_disconnect_notice-0.2.0/nonebot_plugin_disconnect_notice/utils.py
--rw-r--r--   0        0        0      483 2024-04-08 08:32:31.472409 nonebot_plugin_disconnect_notice-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     6512 1970-01-01 00:00:00.000000 nonebot_plugin_disconnect_notice-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-16 11:45:30.012988 nonebot_plugin_disconnect_notice-0.2.1/LICENSE
+-rw-r--r--   0        0        0     5782 2024-04-16 11:45:30.012988 nonebot_plugin_disconnect_notice-0.2.1/README.md
+-rw-r--r--   0        0        0     3630 2024-04-16 11:45:30.020988 nonebot_plugin_disconnect_notice-0.2.1/nonebot_plugin_disconnect_notice/__init__.py
+-rw-r--r--   0        0        0      803 2024-04-16 11:45:30.020988 nonebot_plugin_disconnect_notice-0.2.1/nonebot_plugin_disconnect_notice/config.py
+-rw-r--r--   0        0        0      784 2024-04-16 11:45:30.020988 nonebot_plugin_disconnect_notice-0.2.1/nonebot_plugin_disconnect_notice/dataClass.py
+-rw-r--r--   0        0        0     2102 2024-04-16 11:45:30.020988 nonebot_plugin_disconnect_notice-0.2.1/nonebot_plugin_disconnect_notice/utils.py
+-rw-r--r--   0        0        0      483 2024-04-16 11:45:30.020988 nonebot_plugin_disconnect_notice-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     6512 1970-01-01 00:00:00.000000 nonebot_plugin_disconnect_notice-0.2.1/PKG-INFO
```

### Comparing `nonebot_plugin_disconnect_notice-0.2.0/LICENSE` & `nonebot_plugin_disconnect_notice-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_disconnect_notice-0.2.0/README.md` & `nonebot_plugin_disconnect_notice-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_disconnect_notice-0.2.0/nonebot_plugin_disconnect_notice/__init__.py` & `nonebot_plugin_disconnect_notice-0.2.1/nonebot_plugin_disconnect_notice/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     # 发布必填，当前有效类型有：`library`（为其他插件编写提供功能），`application`（向机器人用户提供功能）。
     homepage="https://github.com/Cypas/nonebot_plugin_disconnect_notice",
     # 发布必填。
     config=Config,
     supported_adapters=None,
 )
 
-notice_test = on_command("断连通知测试", permission=SUPERUSER)
+notice_test = on_command("断连通知测试", priority=8, block=True, permission=SUPERUSER)
 
 
 @notice_test.handle()
 async def _(matcher: Matcher):
     """主动触发掉线通知测试"""
     msg = "已发送测试邮件，如未收到请检查邮件垃圾箱"
     bot_params = BotParams(
```

### Comparing `nonebot_plugin_disconnect_notice-0.2.0/nonebot_plugin_disconnect_notice/config.py` & `nonebot_plugin_disconnect_notice-0.2.1/nonebot_plugin_disconnect_notice/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from nonebot import get_driver, get_plugin_config
 from pydantic import BaseModel
 
 
 # 其他地方出现的类似 from .. import config，均是从 __init__.py 导入的 Config 实例
 class Config(BaseModel):
     disconnect_notice_smtp_user: str | int = ""
-    disconnect_notice_smtp_password: str = ""
+    disconnect_notice_smtp_password: str | int = ""
     disconnect_notice_smtp_server: str | int = ""
     disconnect_notice_smtp_port: int = 465
     disconnect_notice_notice_email: str | int = ""
     disconnect_notice_dev_mode: bool = False
     disconnect_notice_max_grace_time: int = 10
```

### Comparing `nonebot_plugin_disconnect_notice-0.2.0/nonebot_plugin_disconnect_notice/dataClass.py` & `nonebot_plugin_disconnect_notice-0.2.1/nonebot_plugin_disconnect_notice/dataClass.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_disconnect_notice-0.2.0/nonebot_plugin_disconnect_notice/utils.py` & `nonebot_plugin_disconnect_notice-0.2.1/nonebot_plugin_disconnect_notice/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_disconnect_notice-0.2.0/PKG-INFO` & `nonebot_plugin_disconnect_notice-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-disconnect-notice
-Version: 0.2.0
+Version: 0.2.1
 Summary: bot断连时的通知插件
 Author: cypas
 Author-email: ayano05@outlook.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-disconnect-notice Version: 0.2.0
+Metadata-Version: 2.1 Name: nonebot-plugin-disconnect-notice Version: 0.2.1
 Summary: botæ­è¿æ¶çéç¥æä»¶ Author: cypas Author-email:
 ayano05@outlook.com Requires-Python: >=3.8,<4.0 Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Requires-Dist: aiosmtplib
 (>=2.0.2,<3.0.0) Requires-Dist: nonebot-adapter-onebot (>=2.4.1,<3.0.0)
```

