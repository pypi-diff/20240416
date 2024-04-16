# Comparing `tmp/clovers_leafgame-0.1.1.tar.gz` & `tmp/clovers_leafgame-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clovers_leafgame-0.1.1.tar", max compression
+gzip compressed data, was "clovers_leafgame-0.1.2.tar", max compression
```

## Comparing `clovers_leafgame-0.1.1.tar` & `clovers_leafgame-0.1.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0      300 2024-04-15 02:23:00.888180 clovers_leafgame-0.1.1/clovers_leafgame/__init__.py
--rw-r--r--   0        0        0      666 2024-04-15 08:08:50.767249 clovers_leafgame-0.1.1/clovers_leafgame/config.py
--rw-r--r--   0        0        0     4100 2024-04-15 11:16:35.533032 clovers_leafgame-0.1.1/clovers_leafgame/core/clovers.py
--rw-r--r--   0        0        0     5589 2024-03-26 03:51:17.003276 clovers_leafgame-0.1.1/clovers_leafgame/core/data.py
--rw-r--r--   0        0        0     1617 2024-04-15 02:23:00.889680 clovers_leafgame-0.1.1/clovers_leafgame/item.py
--rw-r--r--   0        0        0     1140 2024-04-15 04:29:38.753994 clovers_leafgame-0.1.1/clovers_leafgame/main.py
--rw-r--r--   0        0        0     6452 2024-04-15 02:23:00.890680 clovers_leafgame-0.1.1/clovers_leafgame/manager.py
--rw-r--r--   0        0        0    14529 2024-04-15 02:23:00.891179 clovers_leafgame-0.1.1/clovers_leafgame/modules/account/__init__.py
--rw-r--r--   0        0        0      332 2024-04-15 02:23:00.891680 clovers_leafgame-0.1.1/clovers_leafgame/modules/account/config.py
--rw-r--r--   0        0        0    43276 2024-04-15 11:08:23.324684 clovers_leafgame-0.1.1/clovers_leafgame/modules/game/__init__.py
--rw-r--r--   0        0        0      153 2024-04-15 07:55:35.192417 clovers_leafgame-0.1.1/clovers_leafgame/modules/game/config.py
--rw-r--r--   0        0        0     8783 2024-04-15 02:23:00.893679 clovers_leafgame-0.1.1/clovers_leafgame/modules/game/core.py
--rw-r--r--   0        0        0    10104 2024-04-15 02:23:00.894179 clovers_leafgame-0.1.1/clovers_leafgame/modules/game/fortress/core.py
--rw-r--r--   0        0        0    12791 2024-04-15 02:23:00.894679 clovers_leafgame-0.1.1/clovers_leafgame/modules/game/horse_race/__init__.py
--rw-r--r--   0        0        0      420 2024-04-15 02:23:00.895180 clovers_leafgame-0.1.1/clovers_leafgame/modules/game/horse_race/config.py
--rw-r--r--   0        0        0     5817 2024-02-25 09:48:38.952874 clovers_leafgame-0.1.1/clovers_leafgame/modules/game/horse_race/event_library/Stand.json
--rw-r--r--   0        0        0     5728 2024-02-25 09:48:38.952874 clovers_leafgame-0.1.1/clovers_leafgame/modules/game/horse_race/event_library/“日常，真的很日常”.json
--rw-r--r--   0        0        0     2174 2024-02-25 09:48:38.953876 clovers_leafgame-0.1.1/clovers_leafgame/modules/game/horse_race/event_library/克苏鲁.json
--rw-r--r--   0        0        0     1231 2024-02-25 09:48:38.953876 clovers_leafgame-0.1.1/clovers_leafgame/modules/game/horse_race/event_library/基础事件.json
--rw-r--r--   0        0        0     2742 2024-02-25 09:48:38.954376 clovers_leafgame-0.1.1/clovers_leafgame/modules/game/horse_race/event_library/复刻经典事件集合v1.json
--rw-r--r--   0        0        0     1606 2024-02-25 09:48:38.954376 clovers_leafgame-0.1.1/clovers_leafgame/modules/game/horse_race/event_library/崩坏集合v1.json
--rw-r--r--   0        0        0    25830 2024-02-25 09:48:38.954877 clovers_leafgame-0.1.1/clovers_leafgame/modules/game/horse_race/event_library/群友日常.json
--rw-r--r--   0        0        0     5180 2024-02-25 09:48:38.955377 clovers_leafgame-0.1.1/clovers_leafgame/modules/game/horse_race/event_library/芜湖事件合集.json
--rw-r--r--   0        0        0     1072 2024-02-25 09:48:38.955878 clovers_leafgame-0.1.1/clovers_leafgame/modules/game/horse_race/event_library/赫尔事件集v1.json
--rw-r--r--   0        0        0     2294 2024-02-25 09:48:38.955878 clovers_leafgame-0.1.1/clovers_leafgame/modules/game/horse_race/event_library/赫尔的赛马场事件簿.json
--rw-r--r--   0        0        0     7488 2024-04-13 05:59:32.008464 clovers_leafgame-0.1.1/clovers_leafgame/modules/game/horse_race/horse.py
--rw-r--r--   0        0        0     9296 2024-04-15 02:23:00.895680 clovers_leafgame-0.1.1/clovers_leafgame/modules/game/horse_race/start.py
--rw-r--r--   0        0        0      754 2024-03-28 05:01:34.333218 clovers_leafgame-0.1.1/clovers_leafgame/modules/game/tools.py
--rw-r--r--   0        0        0    15886 2024-04-15 11:18:31.339286 clovers_leafgame-0.1.1/clovers_leafgame/modules/market/__init__.py
--rw-r--r--   0        0        0      352 2024-04-15 07:59:02.703065 clovers_leafgame-0.1.1/clovers_leafgame/modules/market/config.py
--rw-r--r--   0        0        0    12209 2024-04-15 09:59:29.627236 clovers_leafgame-0.1.1/clovers_leafgame/modules/prop/__init__.py
--rw-r--r--   0        0        0      271 2024-03-19 17:24:33.296953 clovers_leafgame-0.1.1/clovers_leafgame/modules/prop/config.py
--rw-r--r--   0        0        0     2085 2024-04-15 02:23:00.897679 clovers_leafgame-0.1.1/clovers_leafgame/modules/prop/core.py
--rw-r--r--   0        0        0     2681 2024-03-20 09:21:29.211881 clovers_leafgame-0.1.1/clovers_leafgame/modules/prop/output.py
--rw-r--r--   0        0        0     4516 2024-04-15 09:58:44.129537 clovers_leafgame-0.1.1/clovers_leafgame/modules/prop/props_library.json
--rw-r--r--   0        0        0     3850 2024-04-15 11:19:15.895133 clovers_leafgame-0.1.1/clovers_leafgame/modules/ranklist/__init__.py
--rw-r--r--   0        0        0     1003 2024-04-15 02:23:00.898679 clovers_leafgame-0.1.1/clovers_leafgame/modules/ranklist/output.py
--rw-r--r--   0        0        0     3587 2024-04-15 09:04:34.774669 clovers_leafgame-0.1.1/clovers_leafgame/modules/task/__init__.py
--rw-r--r--   0        0        0     6592 2024-04-15 11:17:50.623418 clovers_leafgame-0.1.1/clovers_leafgame/output.py
--rw-r--r--   0        0        0     1806 2024-03-15 10:15:49.531286 clovers_leafgame-0.1.1/clovers_leafgame/props_library.json
--rw-r--r--   0        0        0     1086 2024-04-15 07:17:11.700550 clovers_leafgame-0.1.1/LICENSE
--rw-r--r--   0        0        0      428 2024-04-15 13:15:05.742112 clovers_leafgame-0.1.1/pyproject.toml
--rw-r--r--   0        0        0    18355 2024-04-15 11:14:25.199623 clovers_leafgame-0.1.1/README.md
--rw-r--r--   0        0        0    18184 1970-01-01 00:00:00.000000 clovers_leafgame-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      300 2024-04-15 02:23:00.888180 clovers_leafgame-0.1.2/clovers_leafgame/__init__.py
+-rw-r--r--   0        0        0      682 2024-04-16 00:16:47.844659 clovers_leafgame-0.1.2/clovers_leafgame/config.py
+-rw-r--r--   0        0        0     4100 2024-04-15 11:16:35.533032 clovers_leafgame-0.1.2/clovers_leafgame/core/clovers.py
+-rw-r--r--   0        0        0     5594 2024-04-16 00:21:23.484156 clovers_leafgame-0.1.2/clovers_leafgame/core/data.py
+-rw-r--r--   0        0        0     1617 2024-04-15 02:23:00.889680 clovers_leafgame-0.1.2/clovers_leafgame/item.py
+-rw-r--r--   0        0        0     1151 2024-04-16 00:26:16.638079 clovers_leafgame-0.1.2/clovers_leafgame/main.py
+-rw-r--r--   0        0        0     6480 2024-04-16 11:26:52.037879 clovers_leafgame-0.1.2/clovers_leafgame/manager.py
+-rw-r--r--   0        0        0    14540 2024-04-16 00:25:10.170581 clovers_leafgame-0.1.2/clovers_leafgame/modules/account/__init__.py
+-rw-r--r--   0        0        0      347 2024-04-16 00:17:06.391821 clovers_leafgame-0.1.2/clovers_leafgame/modules/account/config.py
+-rw-r--r--   0        0        0    44479 2024-04-16 11:38:35.616998 clovers_leafgame-0.1.2/clovers_leafgame/modules/game/__init__.py
+-rw-r--r--   0        0        0      153 2024-04-15 07:55:35.192417 clovers_leafgame-0.1.2/clovers_leafgame/modules/game/config.py
+-rw-r--r--   0        0        0     8794 2024-04-16 00:25:10.463080 clovers_leafgame-0.1.2/clovers_leafgame/modules/game/core.py
+-rw-r--r--   0        0        0    10104 2024-04-15 02:23:00.894179 clovers_leafgame-0.1.2/clovers_leafgame/modules/game/fortress/core.py
+-rw-r--r--   0        0        0    12802 2024-04-16 00:25:10.251581 clovers_leafgame-0.1.2/clovers_leafgame/modules/game/horse_race/__init__.py
+-rw-r--r--   0        0        0      447 2024-04-16 00:17:40.700801 clovers_leafgame-0.1.2/clovers_leafgame/modules/game/horse_race/config.py
+-rw-r--r--   0        0        0     5817 2024-02-25 09:48:38.952874 clovers_leafgame-0.1.2/clovers_leafgame/modules/game/horse_race/event_library/Stand.json
+-rw-r--r--   0        0        0     5728 2024-02-25 09:48:38.952874 clovers_leafgame-0.1.2/clovers_leafgame/modules/game/horse_race/event_library/“日常，真的很日常”.json
+-rw-r--r--   0        0        0     2174 2024-02-25 09:48:38.953876 clovers_leafgame-0.1.2/clovers_leafgame/modules/game/horse_race/event_library/克苏鲁.json
+-rw-r--r--   0        0        0     1231 2024-02-25 09:48:38.953876 clovers_leafgame-0.1.2/clovers_leafgame/modules/game/horse_race/event_library/基础事件.json
+-rw-r--r--   0        0        0     2742 2024-02-25 09:48:38.954376 clovers_leafgame-0.1.2/clovers_leafgame/modules/game/horse_race/event_library/复刻经典事件集合v1.json
+-rw-r--r--   0        0        0     1606 2024-02-25 09:48:38.954376 clovers_leafgame-0.1.2/clovers_leafgame/modules/game/horse_race/event_library/崩坏集合v1.json
+-rw-r--r--   0        0        0    25830 2024-02-25 09:48:38.954877 clovers_leafgame-0.1.2/clovers_leafgame/modules/game/horse_race/event_library/群友日常.json
+-rw-r--r--   0        0        0     5180 2024-02-25 09:48:38.955377 clovers_leafgame-0.1.2/clovers_leafgame/modules/game/horse_race/event_library/芜湖事件合集.json
+-rw-r--r--   0        0        0     1072 2024-02-25 09:48:38.955878 clovers_leafgame-0.1.2/clovers_leafgame/modules/game/horse_race/event_library/赫尔事件集v1.json
+-rw-r--r--   0        0        0     2294 2024-02-25 09:48:38.955878 clovers_leafgame-0.1.2/clovers_leafgame/modules/game/horse_race/event_library/赫尔的赛马场事件簿.json
+-rw-r--r--   0        0        0     7488 2024-04-13 05:59:32.008464 clovers_leafgame-0.1.2/clovers_leafgame/modules/game/horse_race/horse.py
+-rw-r--r--   0        0        0     9306 2024-04-16 00:22:36.510976 clovers_leafgame-0.1.2/clovers_leafgame/modules/game/horse_race/start.py
+-rw-r--r--   0        0        0      754 2024-03-28 05:01:34.333218 clovers_leafgame-0.1.2/clovers_leafgame/modules/game/tools.py
+-rw-r--r--   0        0        0    18112 2024-04-16 09:40:00.649790 clovers_leafgame-0.1.2/clovers_leafgame/modules/market/__init__.py
+-rw-r--r--   0        0        0      457 2024-04-16 09:18:01.778879 clovers_leafgame-0.1.2/clovers_leafgame/modules/market/config.py
+-rw-r--r--   0        0        0    12220 2024-04-16 00:24:21.794820 clovers_leafgame-0.1.2/clovers_leafgame/modules/prop/__init__.py
+-rw-r--r--   0        0        0      271 2024-04-16 00:19:07.783118 clovers_leafgame-0.1.2/clovers_leafgame/modules/prop/config.py
+-rw-r--r--   0        0        0     2085 2024-04-15 02:23:00.897679 clovers_leafgame-0.1.2/clovers_leafgame/modules/prop/core.py
+-rw-r--r--   0        0        0     2681 2024-03-20 09:21:29.211881 clovers_leafgame-0.1.2/clovers_leafgame/modules/prop/output.py
+-rw-r--r--   0        0        0     4516 2024-04-15 09:58:44.129537 clovers_leafgame-0.1.2/clovers_leafgame/modules/prop/props_library.json
+-rw-r--r--   0        0        0     3850 2024-04-15 11:19:15.895133 clovers_leafgame-0.1.2/clovers_leafgame/modules/ranklist/__init__.py
+-rw-r--r--   0        0        0     1003 2024-04-15 02:23:00.898679 clovers_leafgame-0.1.2/clovers_leafgame/modules/ranklist/output.py
+-rw-r--r--   0        0        0     3587 2024-04-15 09:04:34.774669 clovers_leafgame-0.1.2/clovers_leafgame/modules/task/__init__.py
+-rw-r--r--   0        0        0     6592 2024-04-15 11:17:50.623418 clovers_leafgame-0.1.2/clovers_leafgame/output.py
+-rw-r--r--   0        0        0     1806 2024-03-15 10:15:49.531286 clovers_leafgame-0.1.2/clovers_leafgame/props_library.json
+-rw-r--r--   0        0        0     1086 2024-04-15 07:17:11.700550 clovers_leafgame-0.1.2/LICENSE
+-rw-r--r--   0        0        0      428 2024-04-16 09:38:35.274713 clovers_leafgame-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0    18355 2024-04-15 11:14:25.199623 clovers_leafgame-0.1.2/README.md
+-rw-r--r--   0        0        0    18184 1970-01-01 00:00:00.000000 clovers_leafgame-0.1.2/PKG-INFO
```

### Comparing `clovers_leafgame-0.1.1/clovers_leafgame/config.py` & `clovers_leafgame-0.1.2/clovers_leafgame/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 from pathlib import Path
 
 
 class Config(BaseModel):
     # 主路径
     main_path: str = str(Path("LeafGames").absolute())
     # 默认显示字体
-    fontname = "simsun"
+    fontname: str = "simsun"
     # 默认备用字体
-    fallback_fonts = [
+    fallback_fonts: list[str] = [
         "Arial",
         "Tahoma",
         "Microsoft YaHei",
         "Segoe UI",
         "Segoe UI Emoji",
         "Segoe UI Symbol",
         "Helvetica Neue",
```

### Comparing `clovers_leafgame-0.1.1/clovers_leafgame/core/clovers.py` & `clovers_leafgame-0.1.2/clovers_leafgame/core/clovers.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.1/clovers_leafgame/core/data.py` & `clovers_leafgame-0.1.2/clovers_leafgame/core/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,15 +123,15 @@
     account_dict: dict[str, Account] = {}
     extra: dict = {}
 
     @classmethod
     def load(cls, file: Path) -> "DataBase":
         if file.exists():
             with open(file, "r", encoding="utf8") as f:
-                data = cls.parse_obj(json.load(f))
+                data = cls.model_validate(json.load(f))
         else:
             data = cls()
         return data
 
     def register(self, account: Account):
         """注册个人账户"""
         user_id = account.user_id
```

### Comparing `clovers_leafgame-0.1.1/clovers_leafgame/item.py` & `clovers_leafgame-0.1.2/clovers_leafgame/item.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.1/clovers_leafgame/main.py` & `clovers_leafgame-0.1.2/clovers_leafgame/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 from clovers.core.plugin import Plugin, Result
 from clovers.core.config import config as clovers_config
 from clovers_leafgame.core.clovers import Event
 from .manager import Manager
 from .config import Config
 
 config_key = __package__
-config_data = Config.parse_obj(clovers_config.get(config_key, {}))
+config_data = Config.model_validate(clovers_config.get(config_key, {}))
 """主配置类"""
-clovers_config[config_key] = config_data.dict()
+clovers_config[config_key] = config_data.model_dump()
 
 
 def build_result(result):
     if isinstance(result, str):
         return Result("text", result)
     if isinstance(result, BytesIO):
         return Result("image", result)
```

### Comparing `clovers_leafgame-0.1.1/clovers_leafgame/manager.py` & `clovers_leafgame-0.1.2/clovers_leafgame/manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,16 +28,16 @@
         self.backup_path.mkdir(exist_ok=True, parents=True)
         self.props_library = props_library
         self.marking_library = marking_library
         self.group_library: Library[str, Group] = Library()
         self.load()
 
     def save(self):
-        with open(self.DATA_PATH, "w") as f:
-            f.write(self.data.json(indent=4))
+        with open(self.DATA_PATH, "w", encoding="utf8") as f:
+            f.write(self.data.model_dump_json(indent=4))
 
     def load(self):
         self.data = DataBase.load(self.DATA_PATH)
         for group in self.data.group_dict.values():
             if (stock := group.stock) and (stock_name := stock.name):
                 self.group_library.set_item(group.id, {stock_name}, group)
             else:
```

### Comparing `clovers_leafgame-0.1.1/clovers_leafgame/modules/account/__init__.py` & `clovers_leafgame-0.1.2/clovers_leafgame/modules/account/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,16 +25,16 @@
     dist_card,
 )
 from clovers.core.config import config as clovers_config
 from .config import Config
 
 
 config_key = __package__
-config_data = Config.parse_obj(clovers_config.get(config_key, {}))
-clovers_config[config_key] = config_data.dict()
+config_data = Config.model_validate(clovers_config.get(config_key, {}))
+clovers_config[config_key] = config_data.model_dump()
 
 sign_gold = config_data.sign_gold
 clovers_marking = config_data.clovers_marking
 revolution_marking = config_data.revolution_marking
 debug_marking = config_data.debug_marking
```

### Comparing `clovers_leafgame-0.1.1/clovers_leafgame/modules/game/__init__.py` & `clovers_leafgame-0.1.2/clovers_leafgame/modules/game/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -860,53 +860,77 @@
     return tip + "\n本轮平局。"
 
 
 buckshot_roulette = Game("恶魔轮盘", "向自己开枪|向对方开枪|使用道具")
 
 
 def buckshot_roulette_random_bullet(bullet_num: int):
-    real_bullet_num = random.randint(1, bullet_num // 2 + 1)
-    empty_bullet_num = bullet_num - real_bullet_num
+    empty_bullet_num = random.randint(1, bullet_num // 2)
+    real_bullet_num = bullet_num - empty_bullet_num
     bullet = [1] * real_bullet_num + [0] * empty_bullet_num
     random.shuffle(bullet)
     return bullet, real_bullet_num, empty_bullet_num
 
 
 def buckshot_roulette_random_props(props_num: int):
-    prop_list = ["手铐", "短锯", "放大镜", "香烟", "啤酒", "逆转器", "过期药品", "箱子"]
+    prop_list = ["手铐", "短锯", "放大镜", "香烟", "啤酒", "逆转器", "过期药品", "肾上腺素", "手机", "箱子"]
     return random.choices(prop_list, k=props_num)
 
 
+def buckshot_roulette_status(session: Session):
+
+    result = []
+    result.append(f"玩家 {session.p1_nickname}[nowrap]\n[pixel][340]玩家 {session.p2_nickname}")
+    heart = lambda n: f"血量 [nowrap]\n[color][red]{n * '♥'}"
+    result.append(f"{heart(session.data['HP1'])}[nowrap]\n[pixel][340]{heart(session.data['HP2'])}")
+    result.append("----")
+    props1 = [f"{k} {v}" for k, v in Counter(session.data["props1"]).items()]
+    props2 = [f"[pixel][340]{k} {v}" for k, v in Counter(session.data["props2"]).items()]
+    props = [["", ""] for _ in range(max(len(props1), len(props2)))]
+    for i, x in enumerate(props1):
+        props[i][0] = x
+    for i, x in enumerate(props2):
+        props[i][1] = x
+    result.append("\n".join(f"{x}[nowrap]\n{y}" for x, y in props))
+    output = BytesIO()
+    text_to_image("\n".join(result), bg_color="white", width=660).save(output, format="png")
+    return output
+
+
+def buckshot_roulette_loading(session: Session):
+    props_num = random.randint(1, 4)
+    session.data["props1"] += buckshot_roulette_random_props(props_num)
+    session.data["props1"] = session.data["props1"][:8]
+    session.data["buff1"].clear()
+    session.data["props2"] += buckshot_roulette_random_props(props_num)
+    session.data["props2"] = session.data["props2"][:8]
+    session.data["buff2"].clear()
+    bullet, real_bullet_num, empty_bullet_num = buckshot_roulette_random_bullet(random.randint(2, 8))
+    session.data["bullet"] = bullet
+    return f"本轮装弹：\n实弹:{real_bullet_num} 空弹:{empty_bullet_num}"
+
+
 @plugin.handle({"恶魔轮盘"}, {"user_id", "group_id", "at"})
 @buckshot_roulette.create(place)
 async def _(session: Session, arg: str):
-    bullet, real_bullet_num, empty_bullet_num = buckshot_roulette_random_bullet(random.randint(3, 8))
-    session.data["bullet"] = bullet
     hp = random.randint(3, 6)
     session.data["HP_MAX"] = hp
     session.data["HP1"] = hp
     session.data["HP2"] = hp
-    props_num = random.randint(1, 4)
-    props1 = buckshot_roulette_random_props(props_num)
-    session.data["props1"] = props1
-    session.data["buff1"] = []
-    session.data["props2"] = buckshot_roulette_random_props(props_num)
-    session.data["buff2"] = []
+    session.data["buff1"] = set()
+    session.data["buff2"] = set()
+    session.data["props1"] = []
+    session.data["props2"] = []
     if session.bet:
         prop, n = session.bet
         tip = f"\n本场下注：{n}{prop.name}/轮"
     else:
         tip = ""
-    start_tips = []
-    start_tips.append(f"双方血量：{hp}")
-    start_tips.append(f"本轮装弹：\n实弹:{real_bullet_num} 空弹:{empty_bullet_num}")
-    start_tips.append("你的道具：")
-    start_tips.append(" ".join(props1))
-    session.start_tips = "\n".join(start_tips)
-    return f"恶魔轮盘场地已创建。{tip}\n{session.create_info()}"
+    session.start_tips = [buckshot_roulette_loading(session), buckshot_roulette_status(session)]
+    return f"【恶魔轮盘】场地已创建。{tip}\n{session.create_info()}"
 
 
 @plugin.handle(r"向(自己|对方)开枪$", {"user_id", "group_id"})
 @buckshot_roulette.action(place)
 async def _(event: Event, session: Session):
     user_id = event.user_id
     bullet = session.data["bullet"]
@@ -918,148 +942,137 @@
         buff = "buff1"
     else:
         hp_self = "HP2"
         hp_others = "HP1"
         buff = "buff2"
     target = event.single_arg()
     hp = hp_self if target == "自己" else hp_others
+
+    def remove_tag(buffs: set[str], tag: str):
+        if tag in buffs:
+            buffs.remove(tag)
+            return True
+        else:
+            return False
+
+    if remove_tag(session.data[buff], "短锯"):
+        current_bullet *= 2
     session.data[hp] -= current_bullet
     result = []
     if current_bullet:
         result.append(f"砰的一声炸响，子弹的击中了{target}")
     else:
         result.append("扣动板机，发出清脆的敲击声...")
 
     if session.data[hp] <= 0:
         session.win = session.p1_uid if hp == "HP2" else session.p2_uid
         return session.end(result[0])
 
     if not bullet:
         result.append("最后一发子弹已打出。")
-        props_num = random.randint(1, 4)
-        session.data["props1"] += buckshot_roulette_random_props(props_num)
-        session.data["props1"] = session.data["props1"][:8]
-        session.data["buff1"] = []
-        session.data["props2"] += buckshot_roulette_random_props(props_num)
-        session.data["props2"] = session.data["props2"][:8]
-        session.data["buff2"] = []
-        bullet, real_bullet_num, empty_bullet_num = buckshot_roulette_random_bullet(random.randint(2, 8))
-        result.append(f"本轮装弹：\n实弹:{real_bullet_num} 空弹:{empty_bullet_num}")
-    if target == "自己" and current_bullet == 0:
-        session.delay()
-    elif "手铐" in session.data[buff]:
-        session.data[buff].remove("手铐")
+        result.append(buckshot_roulette_loading(session))
+    else:
+        session.data["bullet"] = bullet
+
+    if (target == "自己" and current_bullet == 0) or remove_tag(session.data[buff], "手铐"):
         session.delay()
     else:
         session.nextround()
-    session.data["bullet"] = bullet
-    result.append(f"玩家{session.p1_nickname}血量:{session.data['HP1']}")
-    result.append("道具：")
-    result.append(" ".join(f"{k} {v}" for k, v in Counter(session.data["props1"]).items()))
-    result.append(f"玩家{session.p2_nickname}血量:{session.data['HP2']}")
-    result.append("道具：")
-    result.append(" ".join(f"{k} {v}" for k, v in Counter(session.data["props2"]).items()))
     next_name = session.p1_nickname if session.next == session.p1_uid else session.p2_nickname
     result.append(f"请下一位玩家：{next_name}\n{buckshot_roulette.action_tip}")
-    return "\n".join(result)
+    return ["\n".join(result), buckshot_roulette_status(session)]
 
 
 @plugin.handle({"使用道具"}, {"user_id", "group_id"})
 @buckshot_roulette.action(place)
 async def _(event: Event, session: Session):
-    # """
-    # 手铐：让对方下一回合无法行动。
-    # 短锯：
-    # 放大镜：
-    # 香烟：
-    # 啤酒：
-    # 逆转器：转换当前枪膛里面的子弹真假
-    # 肾上脉素：偷取对方的道具并立即使用
-    # 过期药品：40%的概率回两滴血，剩下的概率扣一滴血
-    # 手机：可以知道第n发的子弹真假
-    # 眼罩：对家或自己下次射击有50%概率无效，50%概率伤害+1
-    # 治疗针：下颗子弹回复1点生命
-    # 吗啡：受到致死伤害时自动使用，免疫一次死亡
-    # 箱子：每人抽取一件道具
-    # """
-
-    prop_tips = {
-        "手铐": "对方一回合无法行动",
-        "短锯": "本发子弹伤害翻倍",
-        "放大镜": "查看本发子弹",
-        "香烟": "增加1点血量",
-        "啤酒": "退一发子弹",
-        "逆转器": "转换当前枪膛里面的子弹真假",
-        "过期药品": "40%的概率回两滴血，剩下的概率扣一滴血",
-        "箱子": "每人抽取一件道具",
-    }
-    if event.user_id == session.p1_uid:
-        hp_self = "HP1"
-        hp_others = "HP2"
-        buff = "buff1"
-        props_self = "props1"
-        props_others = "props2"
-    else:
-        hp_self = "HP2"
-        hp_others = "HP1"
-        buff = "buff2"
-        props_self = "props2"
-        props_others = "props1"
     prop_key = event.single_arg()
     if not prop_key:
         return
-    if prop_key not in session.data[props_self]:
-        return f"你未持有道具{prop_key}"
-    session.data[props_self].remove(prop_key)
-    tips = prop_tips.get(prop_key, "")
-    match event.single_arg():
-        case "手铐":
-            session.data[buff].append("手铐")
-        case "短锯":
-            if session.data["bullet"][0] != 0:
-                session.data["bullet"][0] = 2
-        case "放大镜":
-            tips += f"\n本发是{'空弹' if session.data['bullet'][0] == 0 else '实弹'}"
-        case "香烟":
-            session.data[hp_self] += 1
-            session.data[hp_self] = min(session.data[hp_self], session.data["HP_MAX"])
-            tips += f"\n你的血量：{session.data[hp_self]}"
-        case "啤酒":
-            bullet = session.data["bullet"]
-            if len(bullet) < 2:
-                return "不可退掉最后一发子弹。"
-            bullet_name = "空弹" if bullet[0] == 0 else "实弹"
-            tips += f"\n你退掉了一发{bullet_name}"
-            session.data["bullet"] = bullet[1:]
-        case "逆转器":
-            bullet = session.data["bullet"]
-            bullet[0] == 1 if bullet[0] == 0 else 0
-            session.data["bullet"] = bullet
-        case "过期药品":
-            if random.randint(1, 10) <= 4:
-                tips += "\n你增加了2滴血"
-                session.data[hp_self] += 2
+    session.delay()
+
+    def use(session: Session, prop_key: str):
+        prop_tips = {
+            "手铐": "对方一回合无法行动",
+            "短锯": "本发子弹伤害翻倍",
+            "放大镜": "查看本发子弹",
+            "香烟": "增加1点血量",
+            "啤酒": "退一发子弹",
+            "逆转器": "转换当前枪膛里面的子弹真假",
+            "过期药品": "50%的概率回两滴血，剩下的概率扣一滴血",
+            "肾上腺素": "偷取对方的道具并立即使用",
+            "手机": "查看接下来第n发子弹真假",
+            "箱子": "每人抽取一件道具",
+        }
+        if session.next == session.p1_uid:
+            hp_self, hp_others, buff, props_self, props_others = "HP1", "HP2", "buff1", "props1", "props2"
+        else:
+            hp_self, hp_others, buff, props_self, props_others = "HP2", "HP1", "buff2", "props2", "props1"
+        if prop_key not in session.data[props_self]:
+            return f"你未持有道具【{prop_key}】"
+        session.data[props_self].remove(prop_key)
+        tips = "效果：" + prop_tips[prop_key]
+
+        match prop_key:
+            case "手铐" | "短锯":
+                session.data[buff].add(prop_key)
+            case "放大镜":
+                tips += f"\n本发是：{'空弹' if session.data['bullet'][0] == 0 else '实弹'}"
+            case "香烟":
+                session.data[hp_self] += 1
                 session.data[hp_self] = min(session.data[hp_self], session.data["HP_MAX"])
-            else:
-                tips += "\n你减少了1滴血"
-                session.data[hp_self] -= 1
-                if session.data[hp_self] <= 0:
-                    session.win = session.p1_uid if hp_self == "HP2" else session.p2_uid
-                    return session.end(tips)
-        case "箱子":
-            prop1, prop2 = buckshot_roulette_random_props(2)
-            tips += f"\n你获得了{prop1}\n对方获得了{prop2}"
-            session.data[props_self].append(prop1)
-            session.data[props_self] = session.data[props_self][:8]
-            session.data[props_others].append(prop2)
-            session.data[props_others] = session.data[props_others][:8]
-        case _:
-            return
-    session.delay(60)
-    return tips
+                tips += f"\n你的血量：{session.data[hp_self]}"
+            case "啤酒":
+                tips += f"\n你退掉了一发：{'空弹' if session.data['bullet'][0] == 0 else '实弹'}"
+                session.data["bullet"] = session.data["bullet"][1:]
+                if not session.data["bullet"]:
+                    return [f"最后一发子弹已被退出{tips}", buckshot_roulette_loading(session)]
+            case "逆转器":
+                session.data["bullet"][0] = 1 - session.data["bullet"][0]
+            case "过期药品":
+                if random.randint(0, 1) == 0:
+                    tips += "\n你减少了1滴血"
+                    session.data[hp_self] -= 1
+                    if session.data[hp_self] <= 0:
+                        session.win = session.p1_uid if hp_self == "HP2" else session.p2_uid
+                        return session.end(tips)
+                else:
+                    tips += "\n你增加了2滴血"
+                    session.data[hp_self] += 2
+                    session.data[hp_self] = min(session.data[hp_self], session.data["HP_MAX"])
+            case "肾上腺素":
+                if len(event.args) < 2:
+                    return tips + "使用失败，你未指定对方的道具"
+                inner_prop_key = event.args[1]
+                if inner_prop_key == prop_key:
+                    return tips + "使用失败，目标不能是肾上腺素"
+                if inner_prop_key not in session.data[props_others]:
+                    return tips + f"使用失败，对方未持有道具{inner_prop_key}"
+                session.data[props_others].remove(inner_prop_key)
+                session.data[props_self].append(inner_prop_key)
+                return use(session, inner_prop_key)
+            case "手机":
+                bullet = session.data["bullet"]
+                sum_bullet = len(bullet)
+                sum_real_bullet = sum(bullet)
+                sum_empty_bullet = sum_bullet - sum_real_bullet
+                random_index = random.randint(1, sum_bullet)
+                tips += f"\n弹仓内还有{sum_real_bullet}发实弹,{sum_empty_bullet}发空弹\n接下来第{random_index}发是：{'空弹' if bullet[random_index-1] == 0 else '实弹'}"
+            case "箱子":
+                prop1, prop2 = buckshot_roulette_random_props(2)
+                tips += f"\n你获得了{prop1}\n对方获得了{prop2}"
+                session.data[props_self].append(prop1)
+                session.data[props_self] = session.data[props_self][:8]
+                session.data[props_others].append(prop2)
+                session.data[props_others] = session.data[props_others][:8]
+            case _:
+                assert False, "玩家持有无法使用的道具"
+        return tips
+
+    return use(session, prop_key)
 
 
 from .horse_race import RaceWorld
 
 horse_race_game = Game("赛马小游戏", "赛马加入 名字")
```

### Comparing `clovers_leafgame-0.1.1/clovers_leafgame/modules/game/core.py` & `clovers_leafgame-0.1.2/clovers_leafgame/modules/game/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 from clovers_leafgame.item import Prop, GOLD
 from clovers_leafgame.output import text_to_image, endline
 from clovers_leafgame.core.clovers import Event
 from clovers.core.config import config as clovers_config
 from .config import Config
 
 config_key = __package__
-config_data = Config.parse_obj(clovers_config.get(config_key, {}))
-clovers_config[config_key] = config_data.dict()
+config_data = Config.model_validate(clovers_config.get(config_key, {}))
+clovers_config[config_key] = config_data.model_dump()
 
 default_bet = config_data.default_bet
 timeout = config_data.timeout
 
 
 class Session:
     """
```

### Comparing `clovers_leafgame-0.1.1/clovers_leafgame/modules/game/fortress/core.py` & `clovers_leafgame-0.1.2/clovers_leafgame/modules/game/fortress/core.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.1/clovers_leafgame/modules/game/horse_race/__init__.py` & `clovers_leafgame-0.1.2/clovers_leafgame/modules/game/horse_race/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from collections.abc import Callable
 from .horse import Horse, Event, Event_list
 from .start import load_dlcs
 from clovers.core.config import config as clovers_config
 from .config import Config
 
 config_key = __package__
-config_data = Config.parse_obj(clovers_config.get(config_key, {}))
-clovers_config[config_key] = config_data.dict()
+config_data = Config.model_validate(clovers_config.get(config_key, {}))
+clovers_config[config_key] = config_data.model_dump()
 
 track_length = config_data.setting_track_length
 base_move_range = config_data.base_move_range
 random_move_min, random_move_max = config_data.random_move_range
 random_move_range = int(random_move_min * track_length), int(random_move_max * track_length)
 range_of_player_numbers = config_data.range_of_player_numbers
```

### Comparing `clovers_leafgame-0.1.1/clovers_leafgame/modules/game/horse_race/event_library/Stand.json` & `clovers_leafgame-0.1.2/clovers_leafgame/modules/game/horse_race/event_library/Stand.json`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.1/clovers_leafgame/modules/game/horse_race/event_library/“日常，真的很日常”.json` & `clovers_leafgame-0.1.2/clovers_leafgame/modules/game/horse_race/event_library/“日常，真的很日常”.json`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.1/clovers_leafgame/modules/game/horse_race/event_library/克苏鲁.json` & `clovers_leafgame-0.1.2/clovers_leafgame/modules/game/horse_race/event_library/克苏鲁.json`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.1/clovers_leafgame/modules/game/horse_race/event_library/基础事件.json` & `clovers_leafgame-0.1.2/clovers_leafgame/modules/game/horse_race/event_library/基础事件.json`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.1/clovers_leafgame/modules/game/horse_race/event_library/复刻经典事件集合v1.json` & `clovers_leafgame-0.1.2/clovers_leafgame/modules/game/horse_race/event_library/复刻经典事件集合v1.json`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.1/clovers_leafgame/modules/game/horse_race/event_library/崩坏集合v1.json` & `clovers_leafgame-0.1.2/clovers_leafgame/modules/game/horse_race/event_library/崩坏集合v1.json`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.1/clovers_leafgame/modules/game/horse_race/event_library/群友日常.json` & `clovers_leafgame-0.1.2/clovers_leafgame/modules/game/horse_race/event_library/群友日常.json`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.1/clovers_leafgame/modules/game/horse_race/event_library/芜湖事件合集.json` & `clovers_leafgame-0.1.2/clovers_leafgame/modules/game/horse_race/event_library/芜湖事件合集.json`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.1/clovers_leafgame/modules/game/horse_race/event_library/赫尔事件集v1.json` & `clovers_leafgame-0.1.2/clovers_leafgame/modules/game/horse_race/event_library/赫尔事件集v1.json`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.1/clovers_leafgame/modules/game/horse_race/event_library/赫尔的赛马场事件簿.json` & `clovers_leafgame-0.1.2/clovers_leafgame/modules/game/horse_race/event_library/赫尔的赛马场事件簿.json`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.1/clovers_leafgame/modules/game/horse_race/horse.py` & `clovers_leafgame-0.1.2/clovers_leafgame/modules/game/horse_race/horse.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.1/clovers_leafgame/modules/game/horse_race/start.py` & `clovers_leafgame-0.1.2/clovers_leafgame/modules/game/horse_race/start.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     buff_tags = ["locate_lock", "vertigo", "hiding"]
     for buff_tag in buff_tags:
         if raw_event.get(buff_tag) == 1:
             buffs.add(buff_tag)
     for buff_tag in raw_event.get("other_buff", []):
         buffs.add(buff_tag)
     raw_event["buffs"] = buffs
-    return Event.parse_obj(raw_event)
+    return Event.model_validate(raw_event)
 
 
 def _deal(event: dict):
     event_out = {}
     # 读取事件限定值
     try:
         event_out["race_only"] = event["race_only"]
@@ -219,8 +219,8 @@
     # 替换一匹马事件
     try:
         event_out["replace_horse"] = event["replace_horse"]
     except KeyError:
         event_out["replace_horse"] = {}
 
     # 上方危险勿动
-    return Event.parse_obj(event_out)
+    return Event.model_validate(event_out)
```

### Comparing `clovers_leafgame-0.1.1/clovers_leafgame/modules/game/tools.py` & `clovers_leafgame-0.1.2/clovers_leafgame/modules/game/tools.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.1/clovers_leafgame/modules/market/__init__.py` & `clovers_leafgame-0.1.2/clovers_leafgame/modules/market/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,73 @@
 import time
+import heapq
 import math
 import random
 from io import BytesIO
 from collections import Counter
 from clovers_apscheduler import scheduler
 from clovers.utils.tools import gini_coef, format_number
 from clovers_leafgame.core.clovers import Event, Check
-from clovers_leafgame.core.data import Group, Stock
+from clovers_leafgame.core.data import Account, Group, Stock
 from clovers_leafgame.main import plugin, manager
-from clovers_leafgame.item import GOLD, LICENSE, STD_GOLD, item_name_rule
+from clovers_leafgame.item import GOLD, LICENSE, STD_GOLD, REVOLUTION_MARKING, item_name_rule
 from clovers_leafgame.output import text_to_image, endline, invest_card, prop_card
 from clovers.core.config import config as clovers_config
 from .config import Config
 
 config_key = __package__
-config_data = Config.parse_obj(clovers_config.get(config_key, {}))
-clovers_config[config_key] = config_data.dict()
+config_data = Config.model_validate(clovers_config.get(config_key, {}))
+clovers_config[config_key] = config_data.model_dump()
 
 
 revolt_gold = config_data.revolt_gold
 revolt_gini = config_data.revolt_gini
+gini_filter_gold = config_data.gini_filter_gold
 revolt_cd = config_data.revolt_cd
 company_public_gold = config_data.company_public_gold
 
 
+@plugin.handle({"发起重置"}, {"group_id"})
+async def _(event: Event):
+    group_id = event.group_id
+    group = manager.data.group(group_id)
+    revolution_time = group.extra.get("revolution_time", 0)
+    if time.time() - revolution_time < revolt_cd:
+        return f"重置正在冷却中，结束时间：{time.strftime('%H:%M:%S', time.localtime(revolution_time + revolt_cd))}"
+    ranklist: list[tuple[Account, int]] = []
+    sum_wealths = 0
+    for account_id in group.accounts_map.values():
+        account = manager.data.account_dict[account_id]
+        n = account.bank[GOLD.id]
+        if account.bank[GOLD.id] >= gini_filter_gold:
+            ranklist.append(account, n)
+        sum_wealths += n
+    if sum_wealths < company_public_gold:
+        return f"本群金币（{sum_wealths}）小于{company_public_gold}，未满足重置条件。"
+    gini = gini_coef([x[1] for x in ranklist])
+    if gini < revolt_gini:
+        return f"当前基尼系数为{round(gini,3)}，未满足重置条件。"
+    ranklist = heapq.nlargest(10, ranklist, key=lambda x: x[1])
+    top = ranklist[0][0]
+    REVOLUTION_MARKING.locate_bank(*manager.locate_account(top.user_id, group_id))[REVOLUTION_MARKING.id] += 1
+    group.extra["revolution_time"] = time.time()
+    revolution_achieve: dict = group.extra.setdefault("revolution_achieve", {})
+    revolution_achieve[top.user_id] = revolution_achieve.get(top.user_id, 0) + 1
+    for i, (account, n) in enumerate(ranklist):
+        account.bank[GOLD.id] = int(n * i / 10)
+    for account_id in group.accounts_map.values():
+        manager.data.account_dict[account_id].extra["revolution"] = False
+    rate = group.level / group.level + 1
+    for k in group.bank:
+        if k[1] == "1":
+            group.bank[k] = int(group.bank[k] * rate)
+    group.level += 1
+    return f"当前系数为：{round(gini,3)}，重置成功！恭喜{top.name}进入挂件榜☆！重置签到已刷新。"
+
+
 @plugin.handle({"重置签到", "领取金币"}, {"user_id", "group_id", "nickname", "avatar"})
 async def _(event: Event):
     user, account = manager.account(event)
     user.avatar_url = event.avatar
     extra = account.extra
     if not extra.setdefault("revolution", True):
         return "你没有待领取的金币"
@@ -114,15 +154,15 @@
         return check
     if manager.group_library.get(stock_name):
         return f"{stock_name} 已被注册"
     wealths = manager.group_wealths(group_id, GOLD.id)
     stock_value = sum(wealths)
     if stock_value < company_public_gold:
         return f"本群金币（{stock_value}）小于{company_public_gold}，注册失败。"
-    gini = gini_coef(wealths[:-1])
+    gini = gini_coef([x for x in wealths[:-1] if x >= gini_filter_gold])
     if gini > revolt_gini:
         return f"本群基尼系数（{round(gini,3)}）过高，注册失败。"
     level = group.level = (sum(ra.values()) if (ra := group.extra.get("revolution_achieve")) else 0) + 1
     stock_value *= level
     stock = Stock(
         id=group_id,
         name=stock_name,
@@ -353,21 +393,24 @@
                 for _ in range(n):
                     unit = max(floating / issuance, 0.0)
                     value += unit
                     floating -= unit
                 settle = n
             if settle == 0:
                 continue
-            if settle < n:
+            elif settle < n:
                 stock.exchange[user_id] = (n - settle, quote)
+            else:
+                stock.exchange[user_id] = (0, 0)
             user.invest[stock.id] -= settle
             group.invest[stock.id] += settle
-            user.bank[STD_GOLD.id] += int(value)
+            int_value = int(value)
+            user.bank[STD_GOLD.id] += int_value
             user.message.append(
-                f"【交易市场 {clock}】收入{value}标准金币。\n{stock.name}已出售{settle}/{n}，报价{quote or format_number(value/settle)}。"
+                f"【交易市场 {clock}】收入{int_value}标准金币。\n{stock.name}已出售{settle}/{n}，报价{quote or format_number(value/settle)}。"
             )
             std_value += value
         group.bank[GOLD.id] -= int(std_value / level)
         stock.exchange = {user_id: exchange for user_id, exchange in stock.exchange.items() if exchange[0] > 0}
         # 更新浮动价格
         stock.floating = floating
         # 记录价格历史
```

### Comparing `clovers_leafgame-0.1.1/clovers_leafgame/modules/prop/__init__.py` & `clovers_leafgame-0.1.2/clovers_leafgame/modules/prop/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 from clovers_leafgame.output import prop_card, bank_card
 from .output import report_card
 
 from clovers.core.config import config as clovers_config
 from .config import Config
 
 config_key = __package__
-config_data = Config.parse_obj(clovers_config.get(config_key, {}))
-clovers_config[config_key] = config_data.dict()
+config_data = Config.model_validate(clovers_config.get(config_key, {}))
+clovers_config[config_key] = config_data.model_dump()
 
 gacha_gold = config_data.gacha_gold
 packet_gold = config_data.packet_gold
 luckey_min, luckey_max = config_data.luckey_coin
 ticket_price = gacha_gold * 50
```

### Comparing `clovers_leafgame-0.1.1/clovers_leafgame/modules/prop/core.py` & `clovers_leafgame-0.1.2/clovers_leafgame/modules/prop/core.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.1/clovers_leafgame/modules/prop/output.py` & `clovers_leafgame-0.1.2/clovers_leafgame/modules/prop/output.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.1/clovers_leafgame/modules/prop/props_library.json` & `clovers_leafgame-0.1.2/clovers_leafgame/modules/prop/props_library.json`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.1/clovers_leafgame/modules/ranklist/__init__.py` & `clovers_leafgame-0.1.2/clovers_leafgame/modules/ranklist/__init__.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.1/clovers_leafgame/modules/ranklist/output.py` & `clovers_leafgame-0.1.2/clovers_leafgame/modules/ranklist/output.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.1/clovers_leafgame/modules/task/__init__.py` & `clovers_leafgame-0.1.2/clovers_leafgame/modules/task/__init__.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.1/clovers_leafgame/output.py` & `clovers_leafgame-0.1.2/clovers_leafgame/output.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.1/clovers_leafgame/props_library.json` & `clovers_leafgame-0.1.2/clovers_leafgame/props_library.json`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.1/LICENSE` & `clovers_leafgame-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.1/README.md` & `clovers_leafgame-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.1/PKG-INFO` & `clovers_leafgame-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: clovers-leafgame
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: KarisAya
 Author-email: 1048827424@qq.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: clovers-apscheduler (>=0.1.2,<0.2.0)
+Requires-Dist: clovers-apscheduler (>=0.1.3,<0.2.0)
 Requires-Dist: clovers[linecard,tools] (>=0.1.2,<0.2.0)
 Requires-Dist: mplfinance (>=0.12.10b0,<0.13.0)
 Requires-Dist: pydantic (>=2.7.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 <!-- markdownlint-disable MD031 MD033 MD036 MD041 -->
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: clovers-leafgame Version: 0.1.1 Summary: Author:
+Metadata-Version: 2.1 Name: clovers-leafgame Version: 0.1.2 Summary: Author:
 KarisAya Author-email: 1048827424@qq.com Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: clovers-apscheduler (>=0.1.2,<0.2.0) Requires-Dist: clovers
+Requires-Dist: clovers-apscheduler (>=0.1.3,<0.2.0) Requires-Dist: clovers
 [linecard,tools] (>=0.1.2,<0.2.0) Requires-Dist: mplfinance
 (>=0.12.10b0,<0.13.0) Requires-Dist: pydantic (>=2.7.0,<3.0.0) Description-
 Content-Type: text/markdown # clovers_leafgame _â¨ æ¹èª
 [nonebot_plugin_russian](https://github.com/HibiKier/nonebot_plugin_russian)
 å [nonebot_plugin_horserace](https://github.com/shinianj/
 nonebot_plugin_horserace) çå°æ¸¸æåé â¨_
                     [python]_[_l_i_c_e_n_s_e_]_[_p_y_p_i_]_[_p_y_p_i_ _d_o_w_n_l_o_a_d_]
```

