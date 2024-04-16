# Comparing `tmp/KesslerGame-2.1.2.tar.gz` & `tmp/KesslerGame-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KesslerGame-2.1.2.tar", last modified: Fri Apr 12 22:42:52 2024, max compression
+gzip compressed data, was "KesslerGame-2.1.3.tar", last modified: Tue Apr 16 18:17:30 2024, max compression
```

## Comparing `KesslerGame-2.1.2.tar` & `KesslerGame-2.1.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 22:42:52.518264 KesslerGame-2.1.2/
--rw-rw-rw-   0        0        0    11565 2024-04-12 22:42:24.000000 KesslerGame-2.1.2/LICENSE
--rw-rw-rw-   0        0        0       73 2024-04-12 22:42:24.000000 KesslerGame-2.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     3345 2024-04-12 22:42:52.518264 KesslerGame-2.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2677 2024-04-12 22:42:24.000000 KesslerGame-2.1.2/README.md
--rw-rw-rw-   0        0        0      477 2024-04-12 22:42:24.000000 KesslerGame-2.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       29 2024-04-12 22:42:24.000000 KesslerGame-2.1.2/requirements.txt
--rw-rw-rw-   0        0        0      896 2024-04-12 22:42:52.518264 KesslerGame-2.1.2/setup.cfg
--rw-rw-rw-   0        0        0      747 2024-04-12 22:42:24.000000 KesslerGame-2.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-12 22:42:52.502638 KesslerGame-2.1.2/src/
-drwxrwxrwx   0        0        0        0 2024-04-12 22:42:52.518264 KesslerGame-2.1.2/src/KesslerGame.egg-info/
--rw-rw-rw-   0        0        0     3345 2024-04-12 22:42:52.000000 KesslerGame-2.1.2/src/KesslerGame.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1182 2024-04-12 22:42:52.000000 KesslerGame-2.1.2/src/KesslerGame.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 22:42:52.000000 KesslerGame-2.1.2/src/KesslerGame.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-04-12 22:42:52.000000 KesslerGame-2.1.2/src/KesslerGame.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-12 22:42:52.000000 KesslerGame-2.1.2/src/KesslerGame.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2024-04-12 22:42:52.000000 KesslerGame-2.1.2/src/KesslerGame.egg-info/zip-safe
-drwxrwxrwx   0        0        0        0 2024-04-12 22:42:52.518264 KesslerGame-2.1.2/src/kesslergame/
--rw-rw-rw-   0        0        0      701 2024-04-12 22:42:24.000000 KesslerGame-2.1.2/src/kesslergame/__init__.py
--rw-rw-rw-   0        0        0       21 2024-04-12 22:42:24.000000 KesslerGame-2.1.2/src/kesslergame/_version.py
--rw-rw-rw-   0        0        0     7086 2024-04-12 22:42:24.000000 KesslerGame-2.1.2/src/kesslergame/asteroid.py
--rw-rw-rw-   0        0        0     1886 2024-04-12 22:42:24.000000 KesslerGame-2.1.2/src/kesslergame/bullet.py
--rw-rw-rw-   0        0        0     1423 2024-04-12 22:42:24.000000 KesslerGame-2.1.2/src/kesslergame/collisions.py
--rw-rw-rw-   0        0        0     1432 2024-04-12 22:42:24.000000 KesslerGame-2.1.2/src/kesslergame/controller.py
--rw-rw-rw-   0        0        0     6110 2024-04-12 22:42:24.000000 KesslerGame-2.1.2/src/kesslergame/controller_gamepad.py
-drwxrwxrwx   0        0        0        0 2024-04-12 22:42:52.518264 KesslerGame-2.1.2/src/kesslergame/graphics/
--rw-rw-rw-   0        0        0      380 2024-04-12 22:42:24.000000 KesslerGame-2.1.2/src/kesslergame/graphics/__init__.py
--rw-rw-rw-   0        0        0     1054 2024-04-12 22:42:24.000000 KesslerGame-2.1.2/src/kesslergame/graphics/graphics_base.py
--rw-rw-rw-   0        0        0     3034 2024-04-12 22:42:24.000000 KesslerGame-2.1.2/src/kesslergame/graphics/graphics_handler.py
--rw-rw-rw-   0        0        0     5761 2024-04-12 22:42:24.000000 KesslerGame-2.1.2/src/kesslergame/graphics/graphics_plt.py
--rw-rw-rw-   0        0        0    12623 2024-04-12 22:42:24.000000 KesslerGame-2.1.2/src/kesslergame/graphics/graphics_tk.py
--rw-rw-rw-   0        0        0     3912 2024-04-12 22:42:24.000000 KesslerGame-2.1.2/src/kesslergame/graphics/graphics_ue.py
-drwxrwxrwx   0        0        0        0 2024-04-12 22:42:52.518264 KesslerGame-2.1.2/src/kesslergame/graphics/images/
--rw-rw-rw-   0        0        0        0 2024-04-12 22:42:24.000000 KesslerGame-2.1.2/src/kesslergame/graphics/images/__init__.py
--rw-rw-rw-   0        0        0     2708 2024-04-12 22:42:24.000000 KesslerGame-2.1.2/src/kesslergame/graphics/images/playerShip1_green.png
--rw-rw-rw-   0        0        0     2578 2024-04-12 22:42:24.000000 KesslerGame-2.1.2/src/kesslergame/graphics/images/playerShip1_orange.png
--rw-rw-rw-   0        0        0     3597 2024-04-12 22:42:24.000000 KesslerGame-2.1.2/src/kesslergame/graphics/images/playerShip2_orange.png
--rw-rw-rw-   0        0        0     2725 2024-04-12 22:42:24.000000 KesslerGame-2.1.2/src/kesslergame/graphics/images/playerShip3_orange.png
--rw-rw-rw-   0        0        0    17860 2024-04-12 22:42:24.000000 KesslerGame-2.1.2/src/kesslergame/kessler_game.py
--rw-rw-rw-   0        0        0     2035 2024-04-12 22:42:24.000000 KesslerGame-2.1.2/src/kesslergame/mines.py
--rw-rw-rw-   0        0        0     6571 2024-04-12 22:42:24.000000 KesslerGame-2.1.2/src/kesslergame/scenario.py
--rw-rw-rw-   0        0        0     2488 2024-04-12 22:42:24.000000 KesslerGame-2.1.2/src/kesslergame/score.py
--rw-rw-rw-   0        0        0    11089 2024-04-12 22:42:24.000000 KesslerGame-2.1.2/src/kesslergame/ship.py
--rw-rw-rw-   0        0        0     1881 2024-04-12 22:42:24.000000 KesslerGame-2.1.2/src/kesslergame/team.py
+drwxrwxrwx   0        0        0        0 2024-04-16 18:17:30.232580 KesslerGame-2.1.3/
+-rw-rw-rw-   0        0        0    11565 2024-04-16 18:16:55.000000 KesslerGame-2.1.3/LICENSE
+-rw-rw-rw-   0        0        0       73 2024-04-16 18:16:55.000000 KesslerGame-2.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     3345 2024-04-16 18:17:30.232580 KesslerGame-2.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2677 2024-04-16 18:16:55.000000 KesslerGame-2.1.3/README.md
+-rw-rw-rw-   0        0        0      477 2024-04-16 18:16:55.000000 KesslerGame-2.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       29 2024-04-16 18:16:55.000000 KesslerGame-2.1.3/requirements.txt
+-rw-rw-rw-   0        0        0      896 2024-04-16 18:17:30.232580 KesslerGame-2.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      747 2024-04-16 18:16:55.000000 KesslerGame-2.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 18:17:30.216983 KesslerGame-2.1.3/src/
+drwxrwxrwx   0        0        0        0 2024-04-16 18:17:30.232580 KesslerGame-2.1.3/src/KesslerGame.egg-info/
+-rw-rw-rw-   0        0        0     3345 2024-04-16 18:17:30.000000 KesslerGame-2.1.3/src/KesslerGame.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1182 2024-04-16 18:17:30.000000 KesslerGame-2.1.3/src/KesslerGame.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 18:17:30.000000 KesslerGame-2.1.3/src/KesslerGame.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-04-16 18:17:30.000000 KesslerGame-2.1.3/src/KesslerGame.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-16 18:17:30.000000 KesslerGame-2.1.3/src/KesslerGame.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2024-04-16 18:17:30.000000 KesslerGame-2.1.3/src/KesslerGame.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2024-04-16 18:17:30.232580 KesslerGame-2.1.3/src/kesslergame/
+-rw-rw-rw-   0        0        0      701 2024-04-16 18:16:55.000000 KesslerGame-2.1.3/src/kesslergame/__init__.py
+-rw-rw-rw-   0        0        0       21 2024-04-16 18:16:55.000000 KesslerGame-2.1.3/src/kesslergame/_version.py
+-rw-rw-rw-   0        0        0     7086 2024-04-16 18:16:55.000000 KesslerGame-2.1.3/src/kesslergame/asteroid.py
+-rw-rw-rw-   0        0        0     1886 2024-04-16 18:16:55.000000 KesslerGame-2.1.3/src/kesslergame/bullet.py
+-rw-rw-rw-   0        0        0     1423 2024-04-16 18:16:55.000000 KesslerGame-2.1.3/src/kesslergame/collisions.py
+-rw-rw-rw-   0        0        0     1432 2024-04-16 18:16:55.000000 KesslerGame-2.1.3/src/kesslergame/controller.py
+-rw-rw-rw-   0        0        0     6110 2024-04-16 18:16:55.000000 KesslerGame-2.1.3/src/kesslergame/controller_gamepad.py
+drwxrwxrwx   0        0        0        0 2024-04-16 18:17:30.232580 KesslerGame-2.1.3/src/kesslergame/graphics/
+-rw-rw-rw-   0        0        0      380 2024-04-16 18:16:55.000000 KesslerGame-2.1.3/src/kesslergame/graphics/__init__.py
+-rw-rw-rw-   0        0        0     1054 2024-04-16 18:16:55.000000 KesslerGame-2.1.3/src/kesslergame/graphics/graphics_base.py
+-rw-rw-rw-   0        0        0     3034 2024-04-16 18:16:55.000000 KesslerGame-2.1.3/src/kesslergame/graphics/graphics_handler.py
+-rw-rw-rw-   0        0        0     5761 2024-04-16 18:16:55.000000 KesslerGame-2.1.3/src/kesslergame/graphics/graphics_plt.py
+-rw-rw-rw-   0        0        0    13962 2024-04-16 18:16:55.000000 KesslerGame-2.1.3/src/kesslergame/graphics/graphics_tk.py
+-rw-rw-rw-   0        0        0     3912 2024-04-16 18:16:55.000000 KesslerGame-2.1.3/src/kesslergame/graphics/graphics_ue.py
+drwxrwxrwx   0        0        0        0 2024-04-16 18:17:30.232580 KesslerGame-2.1.3/src/kesslergame/graphics/images/
+-rw-rw-rw-   0        0        0        0 2024-04-16 18:16:55.000000 KesslerGame-2.1.3/src/kesslergame/graphics/images/__init__.py
+-rw-rw-rw-   0        0        0     2708 2024-04-16 18:16:55.000000 KesslerGame-2.1.3/src/kesslergame/graphics/images/playerShip1_green.png
+-rw-rw-rw-   0        0        0     2578 2024-04-16 18:16:55.000000 KesslerGame-2.1.3/src/kesslergame/graphics/images/playerShip1_orange.png
+-rw-rw-rw-   0        0        0     3597 2024-04-16 18:16:55.000000 KesslerGame-2.1.3/src/kesslergame/graphics/images/playerShip2_orange.png
+-rw-rw-rw-   0        0        0     2725 2024-04-16 18:16:55.000000 KesslerGame-2.1.3/src/kesslergame/graphics/images/playerShip3_orange.png
+-rw-rw-rw-   0        0        0    17992 2024-04-16 18:16:55.000000 KesslerGame-2.1.3/src/kesslergame/kessler_game.py
+-rw-rw-rw-   0        0        0     2035 2024-04-16 18:16:55.000000 KesslerGame-2.1.3/src/kesslergame/mines.py
+-rw-rw-rw-   0        0        0     6571 2024-04-16 18:16:55.000000 KesslerGame-2.1.3/src/kesslergame/scenario.py
+-rw-rw-rw-   0        0        0     2488 2024-04-16 18:16:55.000000 KesslerGame-2.1.3/src/kesslergame/score.py
+-rw-rw-rw-   0        0        0    11185 2024-04-16 18:16:55.000000 KesslerGame-2.1.3/src/kesslergame/ship.py
+-rw-rw-rw-   0        0        0     1881 2024-04-16 18:16:55.000000 KesslerGame-2.1.3/src/kesslergame/team.py
```

### Comparing `KesslerGame-2.1.2/LICENSE` & `KesslerGame-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `KesslerGame-2.1.2/PKG-INFO` & `KesslerGame-2.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KesslerGame
-Version: 2.1.2
+Version: 2.1.3
 Summary: Asteroids game simulation environment for ML and AI applications
 Home-page: https://github.com/ThalesGroup/kessler-game
 Author: Zachariah Phillips
 Author-email: zach.phillips@defense.us.thalesgroup.com
 Maintainer: Timothy Arnett
 Maintainer-email: tim.arnett@defense.us.thalesgroup.com
 License: Apache 2.0 License
```

### Comparing `KesslerGame-2.1.2/README.md` & `KesslerGame-2.1.3/README.md`

 * *Files identical despite different names*

### Comparing `KesslerGame-2.1.2/setup.cfg` & `KesslerGame-2.1.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `KesslerGame-2.1.2/setup.py` & `KesslerGame-2.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `KesslerGame-2.1.2/src/KesslerGame.egg-info/PKG-INFO` & `KesslerGame-2.1.3/src/KesslerGame.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KesslerGame
-Version: 2.1.2
+Version: 2.1.3
 Summary: Asteroids game simulation environment for ML and AI applications
 Home-page: https://github.com/ThalesGroup/kessler-game
 Author: Zachariah Phillips
 Author-email: zach.phillips@defense.us.thalesgroup.com
 Maintainer: Timothy Arnett
 Maintainer-email: tim.arnett@defense.us.thalesgroup.com
 License: Apache 2.0 License
```

### Comparing `KesslerGame-2.1.2/src/KesslerGame.egg-info/SOURCES.txt` & `KesslerGame-2.1.3/src/KesslerGame.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `KesslerGame-2.1.2/src/kesslergame/__init__.py` & `KesslerGame-2.1.3/src/kesslergame/__init__.py`

 * *Files identical despite different names*

### Comparing `KesslerGame-2.1.2/src/kesslergame/asteroid.py` & `KesslerGame-2.1.3/src/kesslergame/asteroid.py`

 * *Files identical despite different names*

### Comparing `KesslerGame-2.1.2/src/kesslergame/bullet.py` & `KesslerGame-2.1.3/src/kesslergame/bullet.py`

 * *Files identical despite different names*

### Comparing `KesslerGame-2.1.2/src/kesslergame/collisions.py` & `KesslerGame-2.1.3/src/kesslergame/collisions.py`

 * *Files identical despite different names*

### Comparing `KesslerGame-2.1.2/src/kesslergame/controller.py` & `KesslerGame-2.1.3/src/kesslergame/controller.py`

 * *Files identical despite different names*

### Comparing `KesslerGame-2.1.2/src/kesslergame/controller_gamepad.py` & `KesslerGame-2.1.3/src/kesslergame/controller_gamepad.py`

 * *Files identical despite different names*

### Comparing `KesslerGame-2.1.2/src/kesslergame/graphics/graphics_base.py` & `KesslerGame-2.1.3/src/kesslergame/graphics/graphics_base.py`

 * *Files identical despite different names*

### Comparing `KesslerGame-2.1.2/src/kesslergame/graphics/graphics_handler.py` & `KesslerGame-2.1.3/src/kesslergame/graphics/graphics_handler.py`

 * *Files identical despite different names*

### Comparing `KesslerGame-2.1.2/src/kesslergame/graphics/graphics_plt.py` & `KesslerGame-2.1.3/src/kesslergame/graphics/graphics_plt.py`

 * *Files identical despite different names*

### Comparing `KesslerGame-2.1.2/src/kesslergame/graphics/graphics_tk.py` & `KesslerGame-2.1.3/src/kesslergame/graphics/graphics_tk.py`

 * *Files 11% similar despite different names*

```diff
@@ -27,14 +27,28 @@
         self.show_ships = UI_settings.get('ships', True)
         self.show_lives = UI_settings.get('lives_remaining', True)
         self.show_accuracy = UI_settings.get('accuracy', True)
         self.show_asteroids_hit = UI_settings.get('asteroids_hit', True)
         self.show_shots_fired = UI_settings.get('shots_fired', False)
         self.show_bullets_remaining = UI_settings.get('bullets_remaining', False)
         self.show_controller_name = UI_settings.get('controller_name', True)
+        self.script_dir = os.path.dirname(__file__)
+        self.img_dir = os.path.join(self.script_dir, "images")
+
+    def sort_list(self, order, list_to_order):
+        i = len(order)
+        sorted_list = [None] * (len(list_to_order) + (len(order)))
+        for value in list_to_order:
+            try:
+                idx = order.index(value)
+                sorted_list[idx] = value
+            except ValueError:  # value not found in the list
+                sorted_list[i] = value
+                i = i + 1
+        return [x for x in sorted_list if x != None]
 
     def start(self, scenario: Scenario) -> None:
         self.game_width = scenario.map_size[0]
         self.game_height = scenario.map_size[1]
         self.max_time = scenario.time_limit
         self.score_width = 385
         self.window_width = self.game_width + self.score_width
@@ -51,23 +65,30 @@
 
         # create canvas for object and image display
         self.game_canvas = Canvas(self.window, width=self.window_width, height=self.game_height, bg="black")
         self.game_canvas.pack()
         self.window.update()
 
         # Grab and open sprite images in python
-        script_dir = os.path.dirname(__file__)
-        self.image_paths = ["images/playerShip1_green.png",
-                            "images/playerShip1_orange.png",
-                            "images/playerShip2_orange.png",
-                            "images/playerShip3_orange.png"]
+        default_images = ["playerShip1_green.png",
+                            "playerShip1_orange.png",
+                            "playerShip2_orange.png",
+                            "playerShip3_orange.png"]
+
+        img_list = []
+        for file in os.listdir(self.img_dir):
+            if file.endswith(".png") or file.endswith(".jpg"):
+                img_list.append(file)
+        img_list2 = self.sort_list(default_images, img_list)
+        self.image_paths = [os.path.join(self.img_dir, img) for img in img_list2]
+
         self.num_images = len(self.image_paths)
-        self.ship_images = [(Image.open(os.path.join(script_dir, image))).resize((ship_radius, ship_radius)) for image in self.image_paths]
+        self.ship_images = [(Image.open(image)).resize((ship_radius, ship_radius)) for image in self.image_paths]
         self.ship_sprites = [ImageTk.PhotoImage(img) for img in self.ship_images]
-        self.ship_icons = [ImageTk.PhotoImage((Image.open(os.path.join(script_dir, image))).resize((ship_radius, ship_radius))) for image in self.image_paths]
+        self.ship_icons = [ImageTk.PhotoImage((Image.open(image)).resize((ship_radius, ship_radius))) for image in self.image_paths]
 
         self.detoantion_time = 0.3
         #self.detonation_timers = []
 
     def update(self, score: Score, ships: List[Ship], asteroids: List[Asteroid], bullets: List[Bullet], mines: List[Mine]) -> None:
 
         # Delete everything from canvas so we can re-plot
@@ -144,17 +165,20 @@
                 # change max lines in the row if odd team has more lines then even
                 if score_board.count("\n") > max_lines:
                     max_lines = score_board.count("\n")
 
             # display of team information
             self.game_canvas.create_text(output_location_x, output_location_y,
                                     text=score_board, fill="white", font=("Courier New", 10), anchor=NW, )
-
+            icon_idx = team.team_id-1
+            for ship in ships:
+                if ship.custom_sprite_path and ship.team == team.team_id:
+                    icon_idx = self.image_paths.index(os.path.join(self.img_dir, ship.custom_sprite_path))
             self.game_canvas.create_image(output_location_x + 120, output_location_y + 15,
-                                     image=self.ship_icons[(team.team_id-1) % self.num_images])
+                                     image=self.ship_icons[icon_idx % self.num_images])
             team_num += 1
 
     def format_ui(self, team: Team) -> str:
         # lives, accuracy, asteroids hit, shots taken, bullets left
         team_info = "_________\n"
         if self.show_lives:
             team_info += "Lives: " + str(team.lives_remaining) + "\n"
@@ -169,20 +193,27 @@
 
         return team_info
 
     def plot_ships(self, ships: List[Ship]) -> None:
         """
         Plots each ship on the game screen using cached sprites and rotating them
         """
+        no_sprite_count = 0
         for idx, ship in enumerate(ships):
             if ship.alive:
                 # plot ship image and id text next to it
-                self.ship_sprites[idx] = ImageTk.PhotoImage(self.ship_images[idx].rotate(180 - (-ship.heading - 90)))
+                if ship.custom_sprite_path:
+                    sprite_idx = self.image_paths.index(os.path.join(self.img_dir,ship.custom_sprite_path))
+                else:
+                    sprite_idx = no_sprite_count
+                    no_sprite_count += 1
+
+                self.ship_sprites[sprite_idx] = ImageTk.PhotoImage(self.ship_images[sprite_idx].rotate(180 - (-ship.heading - 90)))
                 self.game_canvas.create_image(ship.position[0], self.game_height - ship.position[1],
-                                              image=self.ship_sprites[idx])
+                                              image=self.ship_sprites[sprite_idx])
                 self.game_canvas.create_text(ship.position[0] + ship.radius,
                                              self.game_height - (ship.position[1] + ship.radius), text=str(ship.id),
                                              fill="white")
 
     def plot_shields(self, ships: List[Ship]) -> None:
         """
         Plots each ship's shield ring
```

### Comparing `KesslerGame-2.1.2/src/kesslergame/graphics/graphics_ue.py` & `KesslerGame-2.1.3/src/kesslergame/graphics/graphics_ue.py`

 * *Files identical despite different names*

### Comparing `KesslerGame-2.1.2/src/kesslergame/graphics/images/playerShip1_green.png` & `KesslerGame-2.1.3/src/kesslergame/graphics/images/playerShip1_green.png`

 * *Files identical despite different names*

### Comparing `KesslerGame-2.1.2/src/kesslergame/graphics/images/playerShip1_orange.png` & `KesslerGame-2.1.3/src/kesslergame/graphics/images/playerShip1_orange.png`

 * *Files identical despite different names*

### Comparing `KesslerGame-2.1.2/src/kesslergame/graphics/images/playerShip2_orange.png` & `KesslerGame-2.1.3/src/kesslergame/graphics/images/playerShip2_orange.png`

 * *Files identical despite different names*

### Comparing `KesslerGame-2.1.2/src/kesslergame/graphics/images/playerShip3_orange.png` & `KesslerGame-2.1.3/src/kesslergame/graphics/images/playerShip3_orange.png`

 * *Files identical despite different names*

### Comparing `KesslerGame-2.1.2/src/kesslergame/kessler_game.py` & `KesslerGame-2.1.3/src/kesslergame/kessler_game.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,14 +87,16 @@
         step: int = 0
         time_limit = scenario.time_limit if scenario.time_limit else self.time_limit
 
         # Assign controllers to each ship
         for controller, ship in zip(controllers, ships):
             controller.ship_id = ship.id
             ship.controller = controller
+            if hasattr(controller, "custom_sprite_path"):
+                ship.custom_sprite_path = controller.custom_sprite_path
 
         # Initialize graphics display
         graphics = GraphicsHandler(type=self.graphics_type, scenario=scenario, UI_settings=self.UI_settings, graphics_obj=self.graphics_obj)
 
         # Initialize list of dictionary for performance tracking (will remain empty if perf_tracker is false
         perf_list: List[PerfDict] = []
```

### Comparing `KesslerGame-2.1.2/src/kesslergame/mines.py` & `KesslerGame-2.1.3/src/kesslergame/mines.py`

 * *Files identical despite different names*

### Comparing `KesslerGame-2.1.2/src/kesslergame/scenario.py` & `KesslerGame-2.1.3/src/kesslergame/scenario.py`

 * *Files identical despite different names*

### Comparing `KesslerGame-2.1.2/src/kesslergame/score.py` & `KesslerGame-2.1.3/src/kesslergame/score.py`

 * *Files identical despite different names*

### Comparing `KesslerGame-2.1.2/src/kesslergame/ship.py` & `KesslerGame-2.1.3/src/kesslergame/ship.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     __slots__ = (
         'controller', 'thrust', 'turn_rate', 'id', 'speed', 'position',
         'velocity', 'heading', 'lives', 'deaths', 'team', 'team_name',
         'fire', 'drop_mine', 'thrust_range', 'turn_rate_range', 'max_speed',
         'drag', 'radius', 'mass', '_respawning', '_respawn_time', '_fire_limiter',
         '_fire_time', '_mine_limiter', '_mine_deploy_time', 'mines_remaining',
         'bullets_remaining', 'bullets_shot', 'mines_dropped', 'bullets_hit',
-        'mines_hit', 'asteroids_hit'
+        'mines_hit', 'asteroids_hit', 'custom_sprite_path'
     )
     def __init__(self, ship_id: int,
                  position: Tuple[float, float],
                  angle: float = 90.0,
                  lives: int = 3,
                  team: int = 1,
                  team_name: Optional[str] = None,
@@ -36,14 +36,17 @@
         """
 
         # Control information
         self.controller: Optional[KesslerController] = None
         self.thrust: float = 0.0  # speed defaults to minimum
         self.turn_rate: float = 0.0
 
+        # Ship custom graphics
+        self.custom_sprite_path = None
+
         # State info
         self.id: int = ship_id
         self.speed: float = 0.0
         self.position: tuple[float, float] = position
         self.velocity: tuple[float, float] = (0.0, 0.0)
         self.heading: float = angle
         self.lives: int = lives
```

### Comparing `KesslerGame-2.1.2/src/kesslergame/team.py` & `KesslerGame-2.1.3/src/kesslergame/team.py`

 * *Files identical despite different names*

