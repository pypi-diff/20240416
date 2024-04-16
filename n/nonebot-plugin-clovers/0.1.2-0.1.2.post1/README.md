# Comparing `tmp/nonebot_plugin_clovers-0.1.2.tar.gz` & `tmp/nonebot_plugin_clovers-0.1.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_clovers-0.1.2.tar", max compression
+gzip compressed data, was "nonebot_plugin_clovers-0.1.2.post1.tar", max compression
```

## Comparing `nonebot_plugin_clovers-0.1.2.tar` & `nonebot_plugin_clovers-0.1.2.post1.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1086 2024-04-15 11:49:16.312798 nonebot_plugin_clovers-0.1.2/LICENSE
--rw-r--r--   0        0        0     2213 2024-04-15 14:42:38.315950 nonebot_plugin_clovers-0.1.2/nonebot_plugin_clovers/__init__.py
--rw-r--r--   0        0        0      842 2024-04-15 02:23:00.900179 nonebot_plugin_clovers-0.1.2/nonebot_plugin_clovers/adapters/main.py
--rw-r--r--   0        0        0     1730 2024-04-15 11:51:19.416688 nonebot_plugin_clovers-0.1.2/nonebot_plugin_clovers/adapters/qq.py
--rw-r--r--   0        0        0     3609 2024-04-15 11:51:16.127157 nonebot_plugin_clovers-0.1.2/nonebot_plugin_clovers/adapters/v11.py
--rw-r--r--   0        0        0      397 2024-04-15 14:43:28.422454 nonebot_plugin_clovers-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2514 2024-04-15 11:57:25.353441 nonebot_plugin_clovers-0.1.2/README.md
--rw-r--r--   0        0        0     2946 1970-01-01 00:00:00.000000 nonebot_plugin_clovers-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1086 2024-04-15 11:49:16.312798 nonebot_plugin_clovers-0.1.2.post1/LICENSE
+-rw-r--r--   0        0        0     2332 2024-04-16 09:24:45.888724 nonebot_plugin_clovers-0.1.2.post1/nonebot_plugin_clovers/__init__.py
+-rw-r--r--   0        0        0      842 2024-04-15 02:23:00.900179 nonebot_plugin_clovers-0.1.2.post1/nonebot_plugin_clovers/adapters/main.py
+-rw-r--r--   0        0        0     1730 2024-04-15 11:51:19.416688 nonebot_plugin_clovers-0.1.2.post1/nonebot_plugin_clovers/adapters/qq.py
+-rw-r--r--   0        0        0     3609 2024-04-15 11:51:16.127157 nonebot_plugin_clovers-0.1.2.post1/nonebot_plugin_clovers/adapters/v11.py
+-rw-r--r--   0        0        0      252 2024-04-16 04:31:38.942676 nonebot_plugin_clovers-0.1.2.post1/nonebot_plugin_clovers/config.py
+-rw-r--r--   0        0        0      399 2024-04-16 09:30:20.743003 nonebot_plugin_clovers-0.1.2.post1/pyproject.toml
+-rw-r--r--   0        0        0     2514 2024-04-15 11:57:25.353441 nonebot_plugin_clovers-0.1.2.post1/README.md
+-rw-r--r--   0        0        0     2952 1970-01-01 00:00:00.000000 nonebot_plugin_clovers-0.1.2.post1/PKG-INFO
```

### Comparing `nonebot_plugin_clovers-0.1.2/LICENSE` & `nonebot_plugin_clovers-0.1.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_clovers-0.1.2/nonebot_plugin_clovers/__init__.py` & `nonebot_plugin_clovers-0.1.2.post1/nonebot_plugin_clovers/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,58 +1,57 @@
 import os
 from pathlib import Path
-from pydantic import BaseModel
-from nonebot import get_driver
+from nonebot import get_driver, get_plugin_config, on_message
+from nonebot.matcher import Matcher
+from nonebot.plugin import PluginMetadata
 from clovers.core.adapter import AdapterMethod
 from clovers.core.plugin import PluginLoader
 from .adapters.main import extract_command, new_adapter
-from nonebot.plugin import PluginMetadata
+from .config import Config, ConfigClovers
 
 __plugin_meta__ = PluginMetadata(
     name="clovers插件框架",
     description="NoneBot clovers框架",
-    usage="None",
-    type="library",
+    usage="加载即用",
+    type="application",
     homepage="https://github.com/KarisAya/nonebot_plugin_clovers",
+    config=Config,
+    supported_adapters={
+        "nonebot.adapters.qq",
+        "nonebot.adapters.onebot.v11",
+    },
 )
 
 # 加载配置
-driver = get_driver()
-global_config = driver.config
-clovers_config_file = getattr(global_config, "clovers_config_file", "clovers.toml")
-os.environ["clovers_config_file"] = clovers_config_file
+config_data = get_plugin_config(Config)
 
-# 添加环境变量之后加载config
-from clovers.core.config import config as clovers_config
+clovers_config_file = config_data.clovers_config_file
+clovers_priority = config_data.clovers_priority
 
+os.environ["clovers_config_file"] = clovers_config_file
 
-# 加载clovers配置
-class Config(BaseModel):
-    plugins_path: str = "./clovers_library"
-    plugins_list: list = []
+# 添加环境变量之后加载config
 
+from clovers.core.config import config as clovers_config
 
 config_key = __package__
-config = Config.parse_obj(clovers_config.get(config_key, {}))
-clovers_config[config_key] = config.dict()
+clovers_config_data = ConfigClovers.model_validate(clovers_config.get(config_key, {}))
+clovers_config[config_key] = clovers_config_data.model_dump()
 clovers_config.save()
 
 
-plugins_path = Path(config.plugins_path)
+plugins_path = Path(clovers_config_data.plugins_path)
 plugins_path.mkdir(exist_ok=True, parents=True)
 
-loader = PluginLoader(plugins_path, config.plugins_list)
+loader = PluginLoader(plugins_path, clovers_config_data.plugins_list)
 adapter = new_adapter(loader.plugins)
 
-driver.on_startup(adapter.startup)
-
-from nonebot import on_message
-from nonebot.matcher import Matcher
+get_driver().on_startup(adapter.startup)
 
-main = on_message(priority=50, block=False)
+main = on_message(priority=clovers_priority, block=False)
 
 
 def add_response(Bot, Event, adapter_method: AdapterMethod, adapter_key: str):
     adapter.methods[adapter_key] = adapter_method
 
     @main.handle()
     async def _(matcher: Matcher, bot: Bot, event: Event):
```

### Comparing `nonebot_plugin_clovers-0.1.2/nonebot_plugin_clovers/adapters/main.py` & `nonebot_plugin_clovers-0.1.2.post1/nonebot_plugin_clovers/adapters/main.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_clovers-0.1.2/nonebot_plugin_clovers/adapters/qq.py` & `nonebot_plugin_clovers-0.1.2.post1/nonebot_plugin_clovers/adapters/qq.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_clovers-0.1.2/nonebot_plugin_clovers/adapters/v11.py` & `nonebot_plugin_clovers-0.1.2.post1/nonebot_plugin_clovers/adapters/v11.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_clovers-0.1.2/README.md` & `nonebot_plugin_clovers-0.1.2.post1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_clovers-0.1.2/PKG-INFO` & `nonebot_plugin_clovers-0.1.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-clovers
-Version: 0.1.2
+Version: 0.1.2.post1
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
@@ -1,14 +1,15 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-clovers Version: 0.1.2 Summary:
-Author: KarisAya Author-email: 1048827424@qq.com Requires-Python: >=3.10,<4.0
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: clovers (>=0.1.2,<0.2.0) Requires-Dist: nonebot-adapter-onebot
-(>=2.4.3,<3.0.0) Requires-Dist: nonebot-adapter-qq (>=1.4.3,<2.0.0) Requires-
-Dist: nonebot2 (>=2.2.1,<3.0.0) Description-Content-Type: text/markdown
+Metadata-Version: 2.1 Name: nonebot-plugin-clovers Version: 0.1.2.post1
+Summary: Author: KarisAya Author-email: 1048827424@qq.com Requires-Python:
+>=3.10,<4.0 Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Requires-Dist: clovers (>=0.1.2,<0.2.0) Requires-Dist: nonebot-
+adapter-onebot (>=2.4.3,<3.0.0) Requires-Dist: nonebot-adapter-qq
+(>=1.4.3,<2.0.0) Requires-Dist: nonebot2 (>=2.2.1,<3.0.0) Description-Content-
+Type: text/markdown
                                    _[_n_o_n_e_b_o_t_]
         # nonebot_plugin_clovers[python]_[_l_i_c_e_n_s_e_]_[_p_y_p_i_]_[_p_y_p_i_ _d_o_w_n_l_o_a_d_]
 ## ð¿ å®è£ æ¨èä½¿ç¨ nb-cli å®è£ å¨ nonebot2
 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ ```bash nb
 plugin install nonebot_plugin_clovers ``` ä½¿ç¨åç®¡çå¨å®è£ pip ```bash
 pip install nonebot_plugin_clovers ``` poetry ```bash poetry add
 nonebot_plugin_clovers ``` æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç
```

