# Comparing `tmp/pgtg-0.2.0.tar.gz` & `tmp/pgtg-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgtg-0.2.0.tar", max compression
+gzip compressed data, was "pgtg-0.3.0.tar", max compression
```

## Comparing `pgtg-0.2.0.tar` & `pgtg-0.3.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      181 2024-04-04 18:03:29.163895 pgtg-0.2.0/pgtg/__init__.py
--rw-r--r--   0        0        0      706 2024-03-25 09:00:18.472318 pgtg-0.2.0/pgtg/constants.py
--rw-r--r--   0        0        0    31146 2024-04-04 17:13:49.100300 pgtg-0.2.0/pgtg/environment.py
--rw-r--r--   0        0        0    12292 2024-03-25 09:00:18.472318 pgtg-0.2.0/pgtg/evaluator.py
--rw-r--r--   0        0        0     5717 2024-03-25 09:00:18.472318 pgtg-0.2.0/pgtg/example_maps/tile_map_big_with_obstacles.json
--rw-r--r--   0        0        0     4494 2024-03-25 09:00:18.472318 pgtg-0.2.0/pgtg/example_maps/tile_map_big_without_obstacles.json
--rw-r--r--   0        0        0     1422 2024-03-25 09:00:18.472318 pgtg-0.2.0/pgtg/example_maps/tile_map_medium_with_obstacles.json
--rw-r--r--   0        0        0      716 2024-03-25 09:00:18.472318 pgtg-0.2.0/pgtg/example_maps/tile_map_medium_without_obstacles.json
--rw-r--r--   0        0        0      254 2024-03-25 09:00:18.485270 pgtg-0.2.0/pgtg/example_maps/tile_map_minimal_without_obstacles.json
--rw-r--r--   0        0        0    10624 2024-03-25 09:00:18.486753 pgtg-0.2.0/pgtg/graphic.py
--rw-r--r--   0        0        0     5857 2024-03-25 09:00:18.497055 pgtg-0.2.0/pgtg/map.py
--rw-r--r--   0        0        0    10757 2024-03-25 09:00:18.497293 pgtg-0.2.0/pgtg/map_generator.py
--rw-r--r--   0        0        0    85827 2024-03-25 09:00:18.497293 pgtg-0.2.0/pgtg/map_tiles_data.py
--rw-r--r--   0        0        0    10153 2024-03-25 09:00:18.497293 pgtg-0.2.0/pgtg/parser.py
--rw-r--r--   0        0        0    12838 2024-03-25 09:00:18.502311 pgtg-0.2.0/pgtg/pics/beginning.png
--rw-r--r--   0        0        0    13575 2024-03-25 09:00:18.502883 pgtg-0.2.0/pgtg/pics/road_break.png
--rw-r--r--   0        0        0     8739 2024-03-25 09:00:18.504371 pgtg-0.2.0/pgtg/pics/road_left.png
--rw-r--r--   0        0        0      336 2024-03-25 09:00:18.505409 pgtg-0.2.0/pgtg/pics/test.png
--rw-r--r--   0        0        0      974 2024-04-04 18:02:17.309218 pgtg-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3924 2024-04-04 17:44:46.079919 pgtg-0.2.0/README.md
--rw-r--r--   0        0        0     4729 1970-01-01 00:00:00.000000 pgtg-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      181 2024-04-16 12:03:53.875555 pgtg-0.3.0/pgtg/__init__.py
+-rw-r--r--   0        0        0      886 2024-04-16 10:56:00.313150 pgtg-0.3.0/pgtg/constants.py
+-rw-r--r--   0        0        0    36143 2024-04-16 10:56:00.317912 pgtg-0.3.0/pgtg/environment.py
+-rw-r--r--   0        0        0    12292 2024-04-16 10:56:00.317912 pgtg-0.3.0/pgtg/evaluator.py
+-rw-r--r--   0        0        0     5717 2024-04-16 10:56:00.317912 pgtg-0.3.0/pgtg/example_maps/tile_map_big_with_obstacles.json
+-rw-r--r--   0        0        0     4494 2024-04-16 10:56:00.317912 pgtg-0.3.0/pgtg/example_maps/tile_map_big_without_obstacles.json
+-rw-r--r--   0        0        0     1422 2024-04-16 10:56:00.317912 pgtg-0.3.0/pgtg/example_maps/tile_map_medium_with_obstacles.json
+-rw-r--r--   0        0        0      716 2024-04-16 10:56:00.329316 pgtg-0.3.0/pgtg/example_maps/tile_map_medium_without_obstacles.json
+-rw-r--r--   0        0        0      254 2024-04-16 10:56:00.329316 pgtg-0.3.0/pgtg/example_maps/tile_map_minimal_without_obstacles.json
+-rw-r--r--   0        0        0    11392 2024-04-16 10:56:00.329316 pgtg-0.3.0/pgtg/graphic.py
+-rw-r--r--   0        0        0     7203 2024-04-16 10:56:00.329316 pgtg-0.3.0/pgtg/map.py
+-rw-r--r--   0        0        0    10757 2024-04-16 10:56:00.337905 pgtg-0.3.0/pgtg/map_generator.py
+-rw-r--r--   0        0        0    85827 2024-04-16 10:56:00.339505 pgtg-0.3.0/pgtg/map_tiles_data.py
+-rw-r--r--   0        0        0    10474 2024-04-16 10:56:00.343927 pgtg-0.3.0/pgtg/parser.py
+-rw-r--r--   0        0        0    12838 2024-04-16 10:56:00.346550 pgtg-0.3.0/pgtg/pics/beginning.png
+-rw-r--r--   0        0        0    13575 2024-04-16 10:56:00.347808 pgtg-0.3.0/pgtg/pics/road_break.png
+-rw-r--r--   0        0        0     8739 2024-04-16 10:56:00.349111 pgtg-0.3.0/pgtg/pics/road_left.png
+-rw-r--r--   0        0        0      336 2024-04-16 10:56:00.349111 pgtg-0.3.0/pgtg/pics/test.png
+-rw-r--r--   0        0        0     1061 2024-04-16 12:02:35.829177 pgtg-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4889 2024-04-16 10:58:57.187753 pgtg-0.3.0/README.md
+-rw-r--r--   0        0        0     5685 1970-01-01 00:00:00.000000 pgtg-0.3.0/PKG-INFO
```

### Comparing `pgtg-0.2.0/pgtg/constants.py` & `pgtg-0.3.0/pgtg/constants.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,7 +22,15 @@
     "chess_field",
     "reverse_chess_field",
     "top_half",
     "bottom_half",
     "left_half",
     "right_half",
 ]
+
+# a dictionary mapping the names of cardinal directions to integers
+DIRECTIONS_TO_INTS: dict[str, int] = {
+    "north": 0,
+    "east": 1,
+    "south": 2,
+    "west": 3,
+}
```

### Comparing `pgtg-0.2.0/pgtg/environment.py` & `pgtg-0.3.0/pgtg/environment.py`

 * *Files 12% similar despite different names*

```diff
@@ -33,14 +33,17 @@
         random_map_height: int = 4,
         random_map_percentage_of_connections: float = 0.5,
         random_map_obstacle_probability: float = 0.0,
         random_map_ice_probability_weight: float = 1,
         random_map_broken_road_probability_weight: float = 1,
         random_map_sand_probability_weight: float = 1,
         render_mode: str | None = None,
+        use_sliding_observation_window: bool = False,
+        sliding_observation_window_size: int = 4,
+        use_next_subgoal_direction: bool = False,
         sum_subgoals_reward: int = 100,
         final_goal_bonus: int = 0,
         crash_penalty: int = 100,
         standing_still_penalty: int = 0,
         already_visited_position_penalty: int = 0,
         ice_probability: float = 0.1,
         street_damage_probability: float = 0.1,
@@ -56,14 +59,18 @@
             random_map_height: Default 4. Height of the random map.
             random_map_percentage_of_connections: Default 0.5. Percentage of connections between tiles that will be kept while generating the random map.
             random_map_obstacle_probability: Default 0.0. Probability that a tile receives an obstacle while generating the random map.
             random_map_ice_probability_weight: Default 1. Relative weight of the ice obstacle when generating the random map.
             random_map_broken_road_probability_weight: Default 1. Relative weight of the broken_road obstacle when generating the random map.
             random_map_sand_probability_weight: Default 1. Relative weight of the sand obstacle when generating the random map.
             render_mode: Default None. What kind of output render() generates. "human" results in no output by render() but automatic displaying during step().
+            use_sliding_observation_window: Default False. Whether or not to use a observation window that moves with the agent. If False instead the current tile is observed.
+            sliding_observation_window_size: Default 4. The distance to the border of the moving observation window. A size of 1 results in a 3x3 window, a size of 4 in a 9x9 window and a size of 0 in a 1x1 window
+            (only the currently occupied square is visible). No effect if use_sliding_observation_window is False.
+            use_next_subgoal_direction: Default False. Whether or not to use the direction to the next subgoal as an additional feature in the observation.
             sum_subgoals_reward: Default 100. The sum of all subgoal rewards. Gets split evenly among all subgoals.
             final_goal_bonus: Default 0. Bonus for the final goal that gets added to the subgoal reward.
             crash_penalty: Default 100. Penalty for driving into a wall or out of the map. The value will get negated so a positive value should be used.
             standing_still_penalty: Default 0. Penalty for not moving. Gets applied every step. The value will get negated so a positive value should be used.
             already_visited_position_penalty: Default 0. Penalty for moving to a position that was visited before. Gets applied every step for the final position of that step. Standing still does not result in penalty. The value will get negated so a positive value should be used.
             ice_probability: Default 0.1. Probability of the ice effect happening when the agent drives over it.
             street_damage_probability: Default  0.1. Probability of the broken road effect happening when the agent drives over it.
@@ -71,35 +78,52 @@
             traffic_density: Default 0.0. The density of the traffic as fraction of the number of traffic cars and the number of positions where traffic could be. For a value of 0 no traffic is generated.
             ignore_traffic_collisions: Default False. If true collisions with traffic are ignored. For testing purposes.
         """
 
         # There are 8 different directions to accelerate into and the option to stand still.
         self.action_space = spaces.Discrete(9)
 
-        # The agent sees the position in the current tile, its velocity and the map tile.
-        self.observation_space = spaces.Dict(
-            {
-                "position": spaces.MultiDiscrete(
-                    [TILE_WIDTH, TILE_HEIGHT], dtype=np.int32
-                ),
-                "velocity": spaces.Box(low=-99, high=99, shape=(2,), dtype=np.int32),
-                "map": spaces.Dict(
-                    {
-                        "walls": spaces.MultiBinary((TILE_WIDTH, TILE_HEIGHT)),
-                        "goals": spaces.MultiBinary((TILE_WIDTH, TILE_HEIGHT)),
-                        "ice": spaces.MultiBinary((TILE_WIDTH, TILE_HEIGHT)),
-                        "broken road": spaces.MultiBinary((TILE_WIDTH, TILE_HEIGHT)),
-                        "sand": spaces.MultiBinary((TILE_WIDTH, TILE_HEIGHT)),
-                        "traffic": spaces.MultiBinary((TILE_WIDTH, TILE_HEIGHT)),
-                    }
-                ),
-            }
+        observation_window_size = (
+            (TILE_WIDTH, TILE_HEIGHT)
+            if not use_sliding_observation_window
+            else (
+                1 + sliding_observation_window_size * 2,
+                1 + sliding_observation_window_size * 2,
+            )
         )
 
+        # The agent sees the position in the current tile, its velocity and the map tile.
+        observation_space_dict = {
+            "position": spaces.MultiDiscrete([TILE_WIDTH, TILE_HEIGHT], dtype=np.int32),
+            "velocity": spaces.Box(low=-99, high=99, shape=(2,), dtype=np.int32),
+            "map": spaces.Dict(
+                {
+                    "walls": spaces.MultiBinary(observation_window_size),
+                    "goals": spaces.MultiBinary(observation_window_size),
+                    "ice": spaces.MultiBinary(observation_window_size),
+                    "broken road": spaces.MultiBinary(observation_window_size),
+                    "sand": spaces.MultiBinary(observation_window_size),
+                    "traffic": spaces.MultiBinary(observation_window_size),
+                }
+            ),
+        }
+
+        if use_next_subgoal_direction:
+            observation_space_dict["next_subgoal_direction"] = spaces.Discrete(
+                5, start=-1
+            )
+
+        self.observation_space = spaces.Dict(observation_space_dict)
+
         self.render_mode = render_mode
+
+        self.use_sliding_observation_window = use_sliding_observation_window
+        self.sliding_observation_window_size = sliding_observation_window_size
+        self.use_next_subgoal_direction = use_next_subgoal_direction
+
         self.reward_range = (-np.inf, np.inf)
 
         self.map_path = map_path
         self.map_plan = None
 
         self.random_map_width = random_map_width
         self.random_map_height = random_map_height
@@ -249,25 +273,31 @@
             pre = tmp
 
         return res
 
     def generate_frame(
         self,
         hide_positions: bool = False,
+        show_observation_window: bool = True,
     ) -> Image:
         """Generates a image showing the current state of the environment.
 
         Args:
             hide_positions: Default False. Whether or not to hide the positions of the agent.
+            show_observation_window: Default True. Whether or not to show the observation window.
 
         Returns:
             The generated image.
         """
 
-        pic = graphic.create_map(self, show_path=(not hide_positions))
+        pic = graphic.create_map(
+            self,
+            show_path=(not hide_positions),
+            show_observation_window=show_observation_window,
+        )
 
         return pic
 
     def render(self) -> Image | npt.NDArray | None:
         """Potentially returns a rendered representation of the game according to the render mode.
 
         Returns:
@@ -656,91 +686,136 @@
     def get_observation(self) -> OrderedDict[str, Any]:
         """Returns the current observation visible to the agent.
 
         Returns:
             A element from within the observation space.
         """
 
-        tile_x = int(self.position[0] / TILE_WIDTH)
-        tile_y = int(self.position[1] / TILE_HEIGHT)
+        # after the last step the agent could be outside the map
+        position_inside_map_x = min(max(0, self.position[0]), self.map.width - 1)
+        position_inside_map_y = min(max(0, self.position[1]), self.map.height - 1)
+
+        tile_x = int(position_inside_map_x / TILE_WIDTH)
+        tile_y = int(position_inside_map_y / TILE_HEIGHT)
+
+        if not self.use_sliding_observation_window:
+            cutout_top_left_x = tile_x * TILE_WIDTH
+            cutout_top_left_y = tile_y * TILE_HEIGHT
+            cutout_bottom_right_x = tile_x * TILE_WIDTH + TILE_WIDTH - 1
+            cutout_bottom_right_y = tile_y * TILE_HEIGHT + TILE_HEIGHT - 1
+        else:
+            cutout_top_left_x = self.position[0] - self.sliding_observation_window_size
+            cutout_top_left_y = self.position[1] - self.sliding_observation_window_size
+            cutout_bottom_right_x = (
+                self.position[0] + self.sliding_observation_window_size
+            )
+            cutout_bottom_right_y = (
+                self.position[1] + self.sliding_observation_window_size
+            )
 
-        view = self.map.get_tile_view(tile_x, tile_y)
+        map_cutout = self.map.get_map_cutout(
+            cutout_top_left_x,
+            cutout_top_left_y,
+            cutout_bottom_right_x,
+            cutout_bottom_right_y,
+            None if not self.use_sliding_observation_window else {"wall"},
+        )
 
         map = OrderedDict(
             {
-                "walls": self.translate_view_to_one_hot_encoding(view, ["wall"]),
-                "goals": self.translate_view_to_one_hot_encoding(
-                    view, ["subgoal", "final goal"]
+                "walls": np.array(self.encode_map_with_hot_one(map_cutout, "wall")),
+                "goals": np.array(
+                    self.encode_map_with_hot_one(map_cutout, {"subgoal", "final goal"})
                 ),
-                "ice": self.translate_view_to_one_hot_encoding(view, ["ice"]),
-                "broken road": self.translate_view_to_one_hot_encoding(
-                    view, ["broken road"]
+                "ice": np.array(self.encode_map_with_hot_one(map_cutout, "ice")),
+                "broken road": np.array(
+                    self.encode_map_with_hot_one(map_cutout, "broken road")
                 ),
-                "sand": self.translate_view_to_one_hot_encoding(view, ["sand"]),
+                "sand": np.array(self.encode_map_with_hot_one(map_cutout, "sand")),
                 "traffic": [],
             }
         )
 
-        traffic = np.array(
-            [[0] * len(view[0]) for _ in range(len(view))]
-        )  # creates a (# columns in view) x (# rows in view) 2d array filled with 0
+        # creates a 2d array of the same size as map_cutout filled with 0
+        traffic = np.array([[0] * len(map_cutout[0]) for _ in range(len(map_cutout))])
 
         for car in self.cars:
             if (
-                tile_x * TILE_WIDTH
+                cutout_top_left_x
                 <= car["position"][0]  # car[0] is the car's x position
-                < (tile_x + 1) * TILE_WIDTH
-                and tile_y * TILE_HEIGHT
+                <= cutout_bottom_right_x
+                and cutout_top_left_y
                 <= car["position"][1]  # car[1] is the car's y position
-                < (tile_y + 1) * TILE_HEIGHT
+                <= cutout_bottom_right_y
             ):
-                traffic[car["position"][1] - tile_y * TILE_HEIGHT][
-                    car["position"][0] - tile_x * TILE_WIDTH
-                ] = 1  # x and y are switched on purpose to match observations from before the map representation redesign
+                traffic[car["position"][0] - cutout_top_left_x][
+                    car["position"][1] - cutout_top_left_y
+                ] = 1
 
         map["traffic"] = traffic
 
-        position_in_tile_x = max(0, min(8, self.position[0] - (TILE_WIDTH * tile_x)))
-        position_in_tile_y = max(0, min(8, self.position[1] - (TILE_HEIGHT * tile_y)))
-
-        observation = OrderedDict(
+        observation: OrderedDict[str, Any] = OrderedDict(
             {
-                "position": np.array([position_in_tile_x, position_in_tile_y]),
-                "velocity": np.array(
-                    [self.velocity[1], self.velocity[0]]
-                ),  # x and y are switched on purpose to match observations from before the map representation redesign
+                "position": np.array(
+                    [
+                        (
+                            (position_inside_map_x - cutout_top_left_x)
+                            if not self.use_sliding_observation_window
+                            else 0
+                        ),
+                        (
+                            (position_inside_map_y - cutout_top_left_y)
+                            if not self.use_sliding_observation_window
+                            else 0
+                        ),
+                    ]
+                ),
+                "velocity": self.velocity,
                 "map": map,
             }
         )
 
+        if self.use_next_subgoal_direction:
+            next_subgoal_direction = self.map.get_next_subgoal_direction(
+                position_inside_map_x, position_inside_map_y
+            )
+            observation["next_subgoal_direction"] = next_subgoal_direction
+
         return observation
 
-    def translate_view_to_one_hot_encoding(
-        self, view: list[list[set[str]]], characters_to_match: list[str]
-    ) -> npt.NDArray:
-        """Translates the 2D list of sets of the map into the hot one representation for one feature.
+    def encode_map_with_hot_one(
+        self, map_cutout: list[list[set[str]]], features_to_match: str | set[str]
+    ) -> list[list[int]]:
+        """Transforms a map or map cutout into a hot-one encoding.
+        If a square contains one or more of the features to match, the hot-one encoding will have a 1 at that position and otherwise it will have a 0.
 
         Args:
-            view: The part of the map to be translated
-            characters_to_match: List of characters that represent this feature.
+            map_cutout: The map or map cutout to transform.
+            features_to_match: The feature(s) that will result in a 1 in the hot one encoding.
 
         Returns:
-            The hot one encoding for the specified feature.
+            The hot-one encoding for the specified feature(s).
         """
 
-        res = []
-        for row in view:
-            cur = []
-            for tile in row:
-                if not tile.isdisjoint(characters_to_match):
-                    cur.append(1)
-                else:
-                    cur.append(0)
-            res.append(cur)
-        return np.array(res)
+        assert isinstance(features_to_match, str) or isinstance(
+            features_to_match, set
+        ), "features_to_match must be a string or a set of strings"
+
+        if isinstance(features_to_match, str):
+            features_to_match = {features_to_match}
+
+        # creates a 2d array of the same size as map_cutout filled with 0
+        res = [[0] * len(map_cutout[0]) for _ in range(len(map_cutout))]
+
+        for x in range(len(map_cutout)):
+            for y in range(len(map_cutout[0])):
+                if not map_cutout[x][y].isdisjoint(features_to_match):
+                    res[x][y] = 1
+
+        return res
 
     def get_info(self) -> dict[str, Any]:
         """Returns additional information about the state of the environment."""
 
         state = {
             "x": self.position[0],
             "y": self.position[1],
@@ -768,7 +843,36 @@
             A list of applicable actions.
         """
 
         if not (self.terminated or self.truncated):
             return list(range(9))
         else:
             return []
+
+    def get_observation_window_coordinates(self) -> tuple[int, int, int, int]:
+        """Returns the top left and bottom right corner of the observation window.
+
+        Returns:
+            A tuple (top_left_x, top_left_y, bottom_right_x, bottom_right_y).
+        """
+
+        if not self.use_sliding_observation_window:
+            # after the last step the agent could be outside the map
+            position_inside_map_x = min(max(0, self.position[0]), self.map.width - 1)
+            position_inside_map_y = min(max(0, self.position[1]), self.map.height - 1)
+
+            tile_x = int(position_inside_map_x / TILE_WIDTH)
+            tile_y = int(position_inside_map_y / TILE_HEIGHT)
+
+            return (
+                tile_x * TILE_WIDTH,
+                tile_y * TILE_HEIGHT,
+                tile_x * TILE_WIDTH + TILE_WIDTH - 1,
+                tile_y * TILE_HEIGHT + TILE_HEIGHT - 1,
+            )
+        else:
+            return (
+                self.position[0] - self.sliding_observation_window_size,
+                self.position[1] - self.sliding_observation_window_size,
+                self.position[0] + self.sliding_observation_window_size,
+                self.position[1] + self.sliding_observation_window_size,
+            )
```

### Comparing `pgtg-0.2.0/pgtg/evaluator.py` & `pgtg-0.3.0/pgtg/evaluator.py`

 * *Files identical despite different names*

### Comparing `pgtg-0.2.0/pgtg/example_maps/tile_map_big_with_obstacles.json` & `pgtg-0.3.0/pgtg/example_maps/tile_map_big_with_obstacles.json`

 * *Files identical despite different names*

### Comparing `pgtg-0.2.0/pgtg/example_maps/tile_map_big_without_obstacles.json` & `pgtg-0.3.0/pgtg/example_maps/tile_map_big_without_obstacles.json`

 * *Files identical despite different names*

### Comparing `pgtg-0.2.0/pgtg/example_maps/tile_map_medium_with_obstacles.json` & `pgtg-0.3.0/pgtg/example_maps/tile_map_medium_with_obstacles.json`

 * *Files identical despite different names*

### Comparing `pgtg-0.2.0/pgtg/example_maps/tile_map_medium_without_obstacles.json` & `pgtg-0.3.0/pgtg/example_maps/tile_map_medium_without_obstacles.json`

 * *Files identical despite different names*

### Comparing `pgtg-0.2.0/pgtg/graphic.py` & `pgtg-0.3.0/pgtg/graphic.py`

 * *Files 6% similar despite different names*

```diff
@@ -146,14 +146,15 @@
     return (x + offset) * size, (y + offset) * size
 
 
 def create_map(
     env,
     show_path=False,
     hide_start_line=False,
+    show_observation_window=False,
 ):
     """create the map
 
     Args:
         env (Environment): Instance of rt game.
         show_path (bool, optional): show the taken path in the current episode. Defaults to False.
         hide_start_line (bool, optional): Hide the start line. Defaults to False.
@@ -265,14 +266,30 @@
                 y - car_half_width,
                 x + car_half_width,
                 y + car_half_width,
             ),
             other_car_color,
         )
 
+    if show_observation_window:
+        observation_window_coordinates = env.get_observation_window_coordinates()
+        scaled_observation_window_coordinates = (
+            observation_window_coordinates[0] * size,
+            observation_window_coordinates[1] * size,
+            (observation_window_coordinates[2] + 1) * size,
+            (observation_window_coordinates[3] + 1) * size,
+        )
+
+        observation_window_mask = Image.new("RGBA", (size * h, size * w), (0, 0, 0, 99))
+        ImageDraw.Draw(observation_window_mask).rectangle(
+            scaled_observation_window_coordinates, fill=(0, 0, 0, 0)
+        )
+
+        result.paste(observation_window_mask, (0, 0), mask=observation_window_mask)
+
     return result
 
 
 def print_heatmap(
     values,
     bounds=None,
     colormap=None,
```

### Comparing `pgtg-0.2.0/pgtg/map.py` & `pgtg-0.3.0/pgtg/map.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 import json
 
 from pgtg import parser
-from pgtg.constants import TILE_HEIGHT, TILE_WIDTH
+from pgtg.constants import DIRECTIONS_TO_INTS, TILE_HEIGHT, TILE_WIDTH
 from pgtg.map_generator import MapPlan
 
 
 class EpisodeMap:
     """Class representing a map for the environment that can be modified and used for running a episode."""
 
     def __init__(self, map_plan: MapPlan):
         # save the original map plan to be able to later save the map to a file
         self.map_plan = map_plan
 
-        (self.width, self.height, self._map, self.num_subgoals) = (
-            parser.parse_map_object(self.map_plan)
-        )
+        (
+            self.width,
+            self.height,
+            self._map,
+            self.num_subgoals,
+            self.tile_coordinates_to_subgoal_directions,
+        ) = parser.parse_map_object(self.map_plan)
 
         self.tile_width = int(self.width / TILE_WIDTH)
         self.tile_height = int(self.height / TILE_HEIGHT)
 
         self.starters = []
         self.goals = []
         self.traffic_spawnable_positions = []
@@ -69,42 +73,73 @@
         self.get_features_at(x, y).add(feature)
 
     def remove_feature_at(self, x: int, y: int, feature: str) -> None:
         """Removes the specified feature at the the position specified by the x and y coordinates. Doesn't raise an error if feature is not present."""
 
         self.get_features_at(x, y).discard(feature)
 
-    def get_tile_view(self, x: int, y: int) -> list[list[set[str]]]:
-        """Cuts out the map tile at the specified coordinates. If coordinates outside the map are chosen, cuts out the closest tile instead.
+    def get_map_cutout(
+        self,
+        top_left_x: int,
+        top_left_y: int,
+        bottom_right_x: int,
+        bottom_right_y: int,
+        fill_squares_outside_map_with: set[str] | None = None,
+    ) -> list[list[set[str]]]:
+        """Returns a rectangular cutout of the map. If parts of the cutout are outside the map, those squares are optionally filled with the specified features.
 
         Args:
-            x: x-value of the tile
-            y: y-value of the tile
+            top_left_x: The x-value of the top left corner of the cutout.
+            top_left_y: The y-value of the top left corner of the cutout.
+            bottom_right_x: The x-value of the bottom right corner of the cutout.
+            bottom_right_y: The y-value of the bottom right corner of the cutout.
+            fill_squares_outside_map_with: Default None. Squares outside the map are filled with these features. If None, the squares are left empty.
 
         Returns:
-            A cutout from the map representing the tile at the specified coordinates.
+            A cutout from the map.
         """
 
-        # set max and min values in case the agent has left the map
-        x = max(x, 0)
-        x = min(x, self.tile_width - 1)
-        y = max(y, 0)
-        y = min(y, self.tile_height - 1)
-
-        # calculate the coordinates of the upper left corner of the tile.
-        tile_x = x * TILE_WIDTH
-        tile_y = y * TILE_HEIGHT
-        # cut the row of tiles
-        cut_map = self._map[tile_x : tile_x + TILE_WIDTH]
-        res = []
-        for row in cut_map:
-            res.append(row[tile_y : tile_y + TILE_HEIGHT])
-        return [
-            *zip(*res)
-        ]  # transpose the 2d array to match observations from before the map representation redesign
+        cutout = [
+            [set() for _ in range(bottom_right_y - top_left_y + 1)]
+            for _ in range(bottom_right_x - top_left_x + 1)
+        ]
+
+        for x in range(top_left_x, bottom_right_x + 1):
+            for y in range(top_left_y, bottom_right_y + 1):
+                if self.inside_map(x, y):
+                    cutout[x - top_left_x][y - top_left_y] = self.get_features_at(x, y)
+                elif fill_squares_outside_map_with is not None:
+                    cutout[x - top_left_x][
+                        y - top_left_y
+                    ] = fill_squares_outside_map_with
+
+        return cutout
+
+    def get_next_subgoal_direction(self, x: int, y: int) -> int:
+        """Returns the direction of the next subgoal from the specified position or -1 if no subgoal is on that tile.
+
+        Args:
+            x: x-value of the position.
+            y: y-value of the position.
+
+        Returns:
+            The direction of the next subgoal. (0: north, 1: east, 2: south, 3: west, -1: no subgoal found)
+        """
+
+        tile_x = int(x / TILE_WIDTH)
+        tile_y = int(y / TILE_HEIGHT)
+
+        direction = self.tile_coordinates_to_subgoal_directions.get(
+            (tile_x, tile_y), None
+        )
+
+        if direction is None:
+            return -1
+
+        return DIRECTIONS_TO_INTS[direction]
 
     def set_subgoals_to_used(self, x: int, y: int) -> None:
         """Marks the subgoal at the specified coordinates as used and recursively marks all directly adjacent subgoals as used as well.
 
         Args:
             x: x-value of the position
             y: y-value of the position
```

### Comparing `pgtg-0.2.0/pgtg/map_generator.py` & `pgtg-0.3.0/pgtg/map_generator.py`

 * *Files identical despite different names*

### Comparing `pgtg-0.2.0/pgtg/map_tiles_data.py` & `pgtg-0.3.0/pgtg/map_tiles_data.py`

 * *Files identical despite different names*

### Comparing `pgtg-0.2.0/pgtg/parser.py` & `pgtg-0.3.0/pgtg/parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,23 +8,24 @@
 from pgtg.constants import OBSTACLE_NAMES, TILE_HEIGHT, TILE_WIDTH
 from pgtg.map_generator import MapPlan
 from pgtg.map_tiles_data import OBSTACLE_MASKS, TILES, TRAFFIC_LANES
 
 
 def parse_map_object(
     map_plan: MapPlan,
-) -> tuple[int, int, list[list[set[str]]], int]:
+) -> tuple[int, int, list[list[set[str]]], int, dict[tuple[int, int], str]]:
     """Parses a map plan, to the important features of a episode map.
 
     Args:
         map_plan: The map to be parsed
 
     Returns:
-        A tuple (width, height, map, num_subgoals), where width and height are the dimensions of the map,
-        map represents the features of each tile, and num_subgoals is the number of subgoals in the map.
+        A tuple (width, height, map, num_subgoals, subgoal_directions), where width and height are the dimensions of the map,
+        map represents the features of each tile, num_subgoals is the number of subgoals in the map, and subgoal_directions
+        is a dictionary mapping tile coordinates to the direction of the subgoal on that tile.
     """
 
     graph = parse_tile_map_to_graph(map_plan)
 
     # finds the shortest path between the lower left tile and the upper right tile.
     shortest_path: list[tuple[int, int]] = graph.shortest_path(
         (0, map_plan.height - 1), (map_plan.width - 1, 0)
@@ -149,19 +150,23 @@
             # add the tile to the map
             for square_x in range(TILE_WIDTH):
                 for square_y in range(TILE_HEIGHT):
                     map[tile_x * TILE_WIDTH + square_x][
                         tile_y * TILE_HEIGHT + square_y
                     ] = current_tile[square_x][square_y]
 
+    # add the direction of the final goal
+    subgoal_coordinates_to_direction.update({shortest_path[-1]: "east"})
+
     return (
         map_plan.width * TILE_WIDTH,
         map_plan.height * TILE_HEIGHT,
         map,
-        len(subgoal_coordinates_to_direction) + 1,
+        len(subgoal_coordinates_to_direction),
+        subgoal_coordinates_to_direction,
     )
 
 
 def replace_features_in_tile(
     tile: list[list[set[str]]],
     old_feature: str,
     new_feature: str | None,
```

### Comparing `pgtg-0.2.0/pgtg/pics/beginning.png` & `pgtg-0.3.0/pgtg/pics/beginning.png`

 * *Files identical despite different names*

### Comparing `pgtg-0.2.0/pgtg/pics/road_break.png` & `pgtg-0.3.0/pgtg/pics/road_break.png`

 * *Files identical despite different names*

### Comparing `pgtg-0.2.0/pgtg/pics/road_left.png` & `pgtg-0.3.0/pgtg/pics/road_left.png`

 * *Files identical despite different names*

### Comparing `pgtg-0.2.0/pyproject.toml` & `pgtg-0.3.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 [tool.poetry]
 authors = [
   "Timo P. Gros <timopgros@cs.uni-saarland.de>",
-  "Joschka Groß <jgross@cs.uni-saarland.de>",
+  "Julius Kamp <juka00001@stud.uni-saarland.de>",
+  "Naya Rudolph <naya.rudolph00@gmail.com>",
+  "Mel Ditter <zitret17@gmail.com>",
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Operating System :: OS Independent",
   "Intended Audience :: Science/Research",
   "Topic :: Scientific/Engineering :: Artificial Intelligence",
 ]
 description = "Python simulation of a driving challange. Compatible with the Gymnasium API standard."
 name = "pgtg"
 readme = "README.md"
-version = "0.2.0"
+version = "0.3.0"
 
 [tool.poetry.dependencies]
 Pillow = "^8.4.0"
 matplotlib = "^3.4.3"
 numpy = "^1.26.3"
 python = ">=3.10,<3.11"
 jupyter = "^1.0.0"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pgtg-0.2.0/README.md` & `pgtg-0.3.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -8,30 +8,30 @@
 pip install pgtg
 ```
 
 ### Usage
 The easiest way to use pgtg is to create the environment with gymnasium:
 ```python
 import pgtg
-env = gymnasium.make("pgtg-v1")
+env = gymnasium.make("pgtg-v2")
 ```
 The package relies on ```import``` side-effects to register the environment
 name so, even though the package is never explicitly used, its import is
 necessary to access the environment.  
 
 If you want to access the environment constructor directly this is also possible:
 ```python
 from pgtg import PGTGEnv
 env = PGTGEnv()
 ```
 
 ## Environment
 ProcGrid Traffic Gym procedurally generates a map consisting of multiple preconstructed tiles or loads a map from a file. The goal is to drive from the start of the map to the end. The navigation task is not part of this environment, instead a shortest path is provided and marked on the map.  
 
-The environment is highly customizable, see the constructor documentation for more info.
+The environment is highly customizable, see the environment constructor for more info.
 
 ### Action Space
 ProcGrid Traffic Gym has a `Discrete(9)` action space.
 
 | Value | Meaning                   |
 |-------|---------------------------|
 | 0     | accelerate left and up    |
@@ -41,22 +41,23 @@
 | 4     | don't accelerate          |
 | 5     | accelerate down           |
 | 6     | accelerate right and up   |
 | 7     | accelerate right          |
 | 8     | accelerate right and down |
 
 ### Observation Space
-ProcGrid Traffic Gym has a `Dict` observation space that shows the 9x9 area the agent currently is inside.
+ProcGrid Traffic Gym has a `Dict` observation space that shows the 9x9 area the agent currently is inside or, if a sliding observation window is used, a area of the specified size centered on the agent.
 | Key | Type | Explanation |
 |-----|------|-------------|
-| "position" | `MultiDiscrete` | The x and y position of the agent within the observation window. |
-| "velocity" | `Box` | The velocity of the agent is x and y direction. |
-| "map" | `Dict` | The 9x9 are of the map the agent is currently inside. The keys are the name of the features (`"walls"`, `"goals"`, `"ice"`, `"broken road"`, `"sand"`, and `"traffic"`). Each item is a `MultiBinary` that encodes that feature as a hot one encoding. |
+| "position" | `MultiDiscrete` | The x and y position of the agent within the observation window or, if a sliding observation window is used, always `(0, 0)`. |
+| "velocity" | `Box` | The velocity of the agent in x and y direction. |
+| "map" | `Dict` | The current observation window. The keys are the name of the features (`"walls"`, `"goals"`, `"ice"`, `"broken road"`, `"sand"`, and `"traffic"`). Each item is a `MultiBinary` that encodes that feature as a hot one encoding. |
+| "next_subgoal_direction" | `Discrete(5)` | The direction of the next subgoal or `-1` if there is no next subgoal (most likely because the agent took a wrong turn). __This is disabled by default. It can be enabled with the `use_next_subgoal_direction` argument of the environment constructor.__|
 
-Most reinforcement learning implementations can't deal with `Dict` observations, thus it might be necessary to flatten the observations. This is easily doable with the `gymnasium.wrappers.FlattenObservation` wrapper:
+Most reinforcement learning implementations can't deal with `Dict` observations directly, thus it might be necessary to flatten the observations. This is easily doable with the `gymnasium.wrappers.FlattenObservation` wrapper:
 ```python
 from gymnasium.wrappers import FlattenObservation
 env = FlattenObservation(env)
 ```
 
 ### Reward
 Crossing a subgoal is rewarded with `+100 / number of subgoals` as is finishing the whole map. Moving into a wall or traffic is punished with `-100` and ends the episode. Standing still or moving to a already visited position can also penalized but is not per default. The reward values for each of this can be customized.
@@ -72,9 +73,17 @@
 | Name | Effect |
 |------|--------|
 | Ice | When driving over a square with ice, there is a chance the agent moves in a random direction instead of the expected one. |
 | Sand | When driving over sand, there is a chance that the agent is slowed, as the velocity is reset to 0. |
 | Broken road | When driving over broken road, there is a chance for the agent to get a flat tire. This slows the agent down, as the velocity is reset to 0 every step. A flat tire lasts until the end of the episode.|
 
 ## Version History
-- v0: initial release
-- v1: Sand now slows down with a customizable probability (default 20%) instead of always.
+### v0.1.0
+- initial release
+### v0.2.0
+- Sand now slows down with a customizable probability (default 20%) instead of always.
+- Bump environment version to v1 because the changes impact reproducibility with earlier versions.
+### v0.3.0
+- The x and y coordinates of observations are no longer swapped. This was the case for historical reasons but serves no use any more.
+- Adds the option to use a sliding observation window of variable size.
+- Adds the option to use the direction of the next subgoal as a additional observation.
+- Bump environment version to v2 because the changes impact reproducibility with earlier versions.
```

### Comparing `pgtg-0.2.0/PKG-INFO` & `pgtg-0.3.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgtg
-Version: 0.2.0
+Version: 0.3.0
 Summary: Python simulation of a driving challange. Compatible with the Gymnasium API standard.
 Author: Timo P. Gros
 Author-email: timopgros@cs.uni-saarland.de
 Requires-Python: >=3.10,<3.11
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
@@ -30,30 +30,30 @@
 pip install pgtg
 ```
 
 ### Usage
 The easiest way to use pgtg is to create the environment with gymnasium:
 ```python
 import pgtg
-env = gymnasium.make("pgtg-v1")
+env = gymnasium.make("pgtg-v2")
 ```
 The package relies on ```import``` side-effects to register the environment
 name so, even though the package is never explicitly used, its import is
 necessary to access the environment.  
 
 If you want to access the environment constructor directly this is also possible:
 ```python
 from pgtg import PGTGEnv
 env = PGTGEnv()
 ```
 
 ## Environment
 ProcGrid Traffic Gym procedurally generates a map consisting of multiple preconstructed tiles or loads a map from a file. The goal is to drive from the start of the map to the end. The navigation task is not part of this environment, instead a shortest path is provided and marked on the map.  
 
-The environment is highly customizable, see the constructor documentation for more info.
+The environment is highly customizable, see the environment constructor for more info.
 
 ### Action Space
 ProcGrid Traffic Gym has a `Discrete(9)` action space.
 
 | Value | Meaning                   |
 |-------|---------------------------|
 | 0     | accelerate left and up    |
@@ -63,22 +63,23 @@
 | 4     | don't accelerate          |
 | 5     | accelerate down           |
 | 6     | accelerate right and up   |
 | 7     | accelerate right          |
 | 8     | accelerate right and down |
 
 ### Observation Space
-ProcGrid Traffic Gym has a `Dict` observation space that shows the 9x9 area the agent currently is inside.
+ProcGrid Traffic Gym has a `Dict` observation space that shows the 9x9 area the agent currently is inside or, if a sliding observation window is used, a area of the specified size centered on the agent.
 | Key | Type | Explanation |
 |-----|------|-------------|
-| "position" | `MultiDiscrete` | The x and y position of the agent within the observation window. |
-| "velocity" | `Box` | The velocity of the agent is x and y direction. |
-| "map" | `Dict` | The 9x9 are of the map the agent is currently inside. The keys are the name of the features (`"walls"`, `"goals"`, `"ice"`, `"broken road"`, `"sand"`, and `"traffic"`). Each item is a `MultiBinary` that encodes that feature as a hot one encoding. |
+| "position" | `MultiDiscrete` | The x and y position of the agent within the observation window or, if a sliding observation window is used, always `(0, 0)`. |
+| "velocity" | `Box` | The velocity of the agent in x and y direction. |
+| "map" | `Dict` | The current observation window. The keys are the name of the features (`"walls"`, `"goals"`, `"ice"`, `"broken road"`, `"sand"`, and `"traffic"`). Each item is a `MultiBinary` that encodes that feature as a hot one encoding. |
+| "next_subgoal_direction" | `Discrete(5)` | The direction of the next subgoal or `-1` if there is no next subgoal (most likely because the agent took a wrong turn). __This is disabled by default. It can be enabled with the `use_next_subgoal_direction` argument of the environment constructor.__|
 
-Most reinforcement learning implementations can't deal with `Dict` observations, thus it might be necessary to flatten the observations. This is easily doable with the `gymnasium.wrappers.FlattenObservation` wrapper:
+Most reinforcement learning implementations can't deal with `Dict` observations directly, thus it might be necessary to flatten the observations. This is easily doable with the `gymnasium.wrappers.FlattenObservation` wrapper:
 ```python
 from gymnasium.wrappers import FlattenObservation
 env = FlattenObservation(env)
 ```
 
 ### Reward
 Crossing a subgoal is rewarded with `+100 / number of subgoals` as is finishing the whole map. Moving into a wall or traffic is punished with `-100` and ends the episode. Standing still or moving to a already visited position can also penalized but is not per default. The reward values for each of this can be customized.
@@ -94,9 +95,17 @@
 | Name | Effect |
 |------|--------|
 | Ice | When driving over a square with ice, there is a chance the agent moves in a random direction instead of the expected one. |
 | Sand | When driving over sand, there is a chance that the agent is slowed, as the velocity is reset to 0. |
 | Broken road | When driving over broken road, there is a chance for the agent to get a flat tire. This slows the agent down, as the velocity is reset to 0 every step. A flat tire lasts until the end of the episode.|
 
 ## Version History
-- v0: initial release
-- v1: Sand now slows down with a customizable probability (default 20%) instead of always.
+### v0.1.0
+- initial release
+### v0.2.0
+- Sand now slows down with a customizable probability (default 20%) instead of always.
+- Bump environment version to v1 because the changes impact reproducibility with earlier versions.
+### v0.3.0
+- The x and y coordinates of observations are no longer swapped. This was the case for historical reasons but serves no use any more.
+- Adds the option to use a sliding observation window of variable size.
+- Adds the option to use the direction of the next subgoal as a additional observation.
+- Bump environment version to v2 because the changes impact reproducibility with earlier versions.
```

