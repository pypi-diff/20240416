# Comparing `tmp/l3c-0.1.0.tar.gz` & `tmp/l3c-0.1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "l3c-0.1.0.tar", last modified: Thu Feb 22 15:11:29 2024, max compression
+gzip compressed data, was "l3c-0.1.0.1.tar", last modified: Mon Apr 15 03:50:00 2024, max compression
```

## Comparing `l3c-0.1.0.tar` & `l3c-0.1.0.1.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxr-xr-x   0 wangfan04   (502) staff       (20)        0 2024-02-22 15:11:29.398918 l3c-0.1.0/
--rw-r--r--   0 wangfan04   (502) staff       (20)    11357 2023-02-23 10:00:57.000000 l3c-0.1.0/LICENSE
--rw-r--r--   0 wangfan04   (502) staff       (20)      951 2024-02-22 15:11:29.398782 l3c-0.1.0/PKG-INFO
--rw-r--r--   0 wangfan04   (502) staff       (20)      620 2023-02-27 11:35:59.000000 l3c-0.1.0/README.md
-drwxr-xr-x   0 wangfan04   (502) staff       (20)        0 2024-02-22 15:11:29.390383 l3c-0.1.0/l3c/
--rw-r--r--   0 wangfan04   (502) staff       (20)      762 2023-02-23 10:11:06.000000 l3c-0.1.0/l3c/__init__.py
-drwxr-xr-x   0 wangfan04   (502) staff       (20)        0 2024-02-22 15:11:29.391981 l3c-0.1.0/l3c/bandits/
--rw-r--r--   0 wangfan04   (502) staff       (20)      838 2023-02-23 10:11:06.000000 l3c-0.1.0/l3c/bandits/__init__.py
--rw-r--r--   0 wangfan04   (502) staff       (20)     2717 2023-02-23 10:11:06.000000 l3c-0.1.0/l3c/bandits/bandits_env.py
--rw-r--r--   0 wangfan04   (502) staff       (20)     1022 2023-02-23 10:32:50.000000 l3c-0.1.0/l3c/bandits/demo_thompson_sampling.py
-drwxr-xr-x   0 wangfan04   (502) staff       (20)        0 2024-02-22 15:11:29.392294 l3c-0.1.0/l3c/mazeworld/
--rw-r--r--   0 wangfan04   (502) staff       (20)     1714 2024-02-20 08:03:46.000000 l3c-0.1.0/l3c/mazeworld/__init__.py
-drwxr-xr-x   0 wangfan04   (502) staff       (20)        0 2024-02-22 15:11:29.393271 l3c-0.1.0/l3c/mazeworld/agents/
--rw-r--r--   0 wangfan04   (502) staff       (20)       45 2024-02-22 03:03:45.000000 l3c-0.1.0/l3c/mazeworld/agents/__init__.py
--rw-r--r--   0 wangfan04   (502) staff       (20)     2857 2024-02-22 12:10:38.000000 l3c-0.1.0/l3c/mazeworld/agents/agent_base.py
--rw-r--r--   0 wangfan04   (502) staff       (20)    11411 2024-02-22 14:05:10.000000 l3c-0.1.0/l3c/mazeworld/agents/smart_slam_agent.py
-drwxr-xr-x   0 wangfan04   (502) staff       (20)        0 2024-02-22 15:11:29.393868 l3c-0.1.0/l3c/mazeworld/demo/
--rw-r--r--   0 wangfan04   (502) staff       (20)        0 2024-02-22 12:15:15.000000 l3c-0.1.0/l3c/mazeworld/demo/__init__.py
--rw-r--r--   0 wangfan04   (502) staff       (20)     3609 2024-02-22 12:13:13.000000 l3c-0.1.0/l3c/mazeworld/demo/agent_play_demo.py
--rw-r--r--   0 wangfan04   (502) staff       (20)     3366 2024-02-22 14:53:11.000000 l3c-0.1.0/l3c/mazeworld/demo/keyboard_play_demo.py
-drwxr-xr-x   0 wangfan04   (502) staff       (20)        0 2024-02-22 15:11:29.396745 l3c-0.1.0/l3c/mazeworld/envs/
--rw-r--r--   0 wangfan04   (502) staff       (20)      258 2024-02-04 12:16:02.000000 l3c-0.1.0/l3c/mazeworld/envs/__init__.py
--rw-r--r--   0 wangfan04   (502) staff       (20)     3644 2023-02-23 10:11:06.000000 l3c-0.1.0/l3c/mazeworld/envs/dynamics.py
--rw-r--r--   0 wangfan04   (502) staff       (20)    14897 2024-02-22 08:51:32.000000 l3c-0.1.0/l3c/mazeworld/envs/maze_base.py
--rw-r--r--   0 wangfan04   (502) staff       (20)     6232 2024-02-20 02:01:17.000000 l3c-0.1.0/l3c/mazeworld/envs/maze_continuous_3d.py
--rw-r--r--   0 wangfan04   (502) staff       (20)     3345 2024-02-22 06:12:11.000000 l3c-0.1.0/l3c/mazeworld/envs/maze_discrete_2d.py
--rw-r--r--   0 wangfan04   (502) staff       (20)     6781 2024-02-21 08:57:49.000000 l3c-0.1.0/l3c/mazeworld/envs/maze_discrete_3d.py
--rw-r--r--   0 wangfan04   (502) staff       (20)     8859 2024-02-22 09:51:50.000000 l3c-0.1.0/l3c/mazeworld/envs/maze_env.py
--rw-r--r--   0 wangfan04   (502) staff       (20)     9184 2024-02-20 01:19:41.000000 l3c-0.1.0/l3c/mazeworld/envs/maze_task.py
--rw-r--r--   0 wangfan04   (502) staff       (20)    12358 2024-02-20 01:48:01.000000 l3c-0.1.0/l3c/mazeworld/envs/ray_caster_utils.py
-drwxr-xr-x   0 wangfan04   (502) staff       (20)        0 2024-02-22 15:11:29.397499 l3c-0.1.0/l3c/mazeworld/tests/
--rw-r--r--   0 wangfan04   (502) staff       (20)        0 2024-02-22 12:15:23.000000 l3c-0.1.0/l3c/mazeworld/tests/__init__.py
--rw-r--r--   0 wangfan04   (502) staff       (20)     2068 2024-02-04 15:06:43.000000 l3c-0.1.0/l3c/mazeworld/tests/test.py
--rw-r--r--   0 wangfan04   (502) staff       (20)     2390 2024-02-22 11:56:16.000000 l3c-0.1.0/l3c/mazeworld/tests/test_agent.py
-drwxr-xr-x   0 wangfan04   (502) staff       (20)        0 2024-02-22 15:11:29.398580 l3c-0.1.0/l3c/metalm/
--rw-r--r--   0 wangfan04   (502) staff       (20)     1080 2023-05-09 04:51:28.000000 l3c-0.1.0/l3c/metalm/__init__.py
--rw-r--r--   0 wangfan04   (502) staff       (20)     2294 2024-02-01 05:22:53.000000 l3c-0.1.0/l3c/metalm/data_generator.py
--rw-r--r--   0 wangfan04   (502) staff       (20)     4267 2024-02-01 05:22:53.000000 l3c-0.1.0/l3c/metalm/metalmv1.py
--rw-r--r--   0 wangfan04   (502) staff       (20)     5530 2024-02-01 05:22:53.000000 l3c-0.1.0/l3c/metalm/metalmv2.py
-drwxr-xr-x   0 wangfan04   (502) staff       (20)        0 2024-02-22 15:11:29.391422 l3c-0.1.0/l3c.egg-info/
--rw-r--r--   0 wangfan04   (502) staff       (20)      951 2024-02-22 15:11:29.000000 l3c-0.1.0/l3c.egg-info/PKG-INFO
--rw-r--r--   0 wangfan04   (502) staff       (20)     1043 2024-02-22 15:11:29.000000 l3c-0.1.0/l3c.egg-info/SOURCES.txt
--rw-r--r--   0 wangfan04   (502) staff       (20)        1 2024-02-22 15:11:29.000000 l3c-0.1.0/l3c.egg-info/dependency_links.txt
--rw-r--r--   0 wangfan04   (502) staff       (20)        1 2023-04-19 12:54:38.000000 l3c-0.1.0/l3c.egg-info/not-zip-safe
--rw-r--r--   0 wangfan04   (502) staff       (20)       84 2024-02-22 15:11:29.000000 l3c-0.1.0/l3c.egg-info/requires.txt
--rw-r--r--   0 wangfan04   (502) staff       (20)        4 2024-02-22 15:11:29.000000 l3c-0.1.0/l3c.egg-info/top_level.txt
--rw-r--r--   0 wangfan04   (502) staff       (20)       38 2024-02-22 15:11:29.398962 l3c-0.1.0/setup.cfg
--rwxr-xr-x   0 wangfan04   (502) staff       (20)     1812 2024-02-22 15:11:10.000000 l3c-0.1.0/setup.py
+drwxr-xr-x   0 wangfan04   (502) staff       (20)        0 2024-04-15 03:50:00.527685 l3c-0.1.0.1/
+-rw-r--r--   0 wangfan04   (502) staff       (20)    11357 2023-02-23 10:00:57.000000 l3c-0.1.0.1/LICENSE
+-rw-r--r--   0 wangfan04   (502) staff       (20)      953 2024-04-15 03:50:00.527458 l3c-0.1.0.1/PKG-INFO
+-rw-r--r--   0 wangfan04   (502) staff       (20)      620 2023-02-27 11:35:59.000000 l3c-0.1.0.1/README.md
+drwxr-xr-x   0 wangfan04   (502) staff       (20)        0 2024-04-15 03:50:00.509777 l3c-0.1.0.1/l3c/
+-rw-r--r--   0 wangfan04   (502) staff       (20)      762 2023-02-23 10:11:06.000000 l3c-0.1.0.1/l3c/__init__.py
+drwxr-xr-x   0 wangfan04   (502) staff       (20)        0 2024-04-15 03:50:00.513377 l3c-0.1.0.1/l3c/bandits/
+-rw-r--r--   0 wangfan04   (502) staff       (20)      838 2023-02-23 10:11:06.000000 l3c-0.1.0.1/l3c/bandits/__init__.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)     2717 2023-02-23 10:11:06.000000 l3c-0.1.0.1/l3c/bandits/bandits_env.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)     1022 2023-02-23 10:32:50.000000 l3c-0.1.0.1/l3c/bandits/demo_thompson_sampling.py
+drwxr-xr-x   0 wangfan04   (502) staff       (20)        0 2024-04-15 03:50:00.513841 l3c-0.1.0.1/l3c/mazeworld/
+-rw-r--r--   0 wangfan04   (502) staff       (20)     1714 2024-02-20 08:03:46.000000 l3c-0.1.0.1/l3c/mazeworld/__init__.py
+drwxr-xr-x   0 wangfan04   (502) staff       (20)        0 2024-04-15 03:50:00.515506 l3c-0.1.0.1/l3c/mazeworld/agents/
+-rw-r--r--   0 wangfan04   (502) staff       (20)       45 2024-02-22 03:03:45.000000 l3c-0.1.0.1/l3c/mazeworld/agents/__init__.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)     2857 2024-02-22 12:10:38.000000 l3c-0.1.0.1/l3c/mazeworld/agents/agent_base.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)    11413 2024-04-15 03:42:37.000000 l3c-0.1.0.1/l3c/mazeworld/agents/smart_slam_agent.py
+drwxr-xr-x   0 wangfan04   (502) staff       (20)        0 2024-04-15 03:50:00.517485 l3c-0.1.0.1/l3c/mazeworld/demo/
+-rw-r--r--   0 wangfan04   (502) staff       (20)        0 2024-02-22 12:15:15.000000 l3c-0.1.0.1/l3c/mazeworld/demo/__init__.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)     3609 2024-04-15 03:45:14.000000 l3c-0.1.0.1/l3c/mazeworld/demo/agent_play_demo.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)     3844 2024-02-26 06:25:37.000000 l3c-0.1.0.1/l3c/mazeworld/demo/dump_maze.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)     3366 2024-02-22 14:53:11.000000 l3c-0.1.0.1/l3c/mazeworld/demo/keyboard_play_demo.py
+drwxr-xr-x   0 wangfan04   (502) staff       (20)        0 2024-04-15 03:50:00.522372 l3c-0.1.0.1/l3c/mazeworld/envs/
+-rw-r--r--   0 wangfan04   (502) staff       (20)      258 2024-02-04 12:16:02.000000 l3c-0.1.0.1/l3c/mazeworld/envs/__init__.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)     3644 2023-02-23 10:11:06.000000 l3c-0.1.0.1/l3c/mazeworld/envs/dynamics.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)    14893 2024-03-13 07:44:10.000000 l3c-0.1.0.1/l3c/mazeworld/envs/maze_base.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)     6232 2024-02-20 02:01:17.000000 l3c-0.1.0.1/l3c/mazeworld/envs/maze_continuous_3d.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)     3345 2024-02-22 06:12:11.000000 l3c-0.1.0.1/l3c/mazeworld/envs/maze_discrete_2d.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)     6781 2024-03-13 07:38:50.000000 l3c-0.1.0.1/l3c/mazeworld/envs/maze_discrete_3d.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)     9168 2024-02-23 08:24:06.000000 l3c-0.1.0.1/l3c/mazeworld/envs/maze_env.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)     9184 2024-02-20 01:19:41.000000 l3c-0.1.0.1/l3c/mazeworld/envs/maze_task.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)    12358 2024-02-20 01:48:01.000000 l3c-0.1.0.1/l3c/mazeworld/envs/ray_caster_utils.py
+drwxr-xr-x   0 wangfan04   (502) staff       (20)        0 2024-04-15 03:50:00.523748 l3c-0.1.0.1/l3c/mazeworld/tests/
+-rw-r--r--   0 wangfan04   (502) staff       (20)        0 2024-02-22 12:15:23.000000 l3c-0.1.0.1/l3c/mazeworld/tests/__init__.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)     2068 2024-02-04 15:06:43.000000 l3c-0.1.0.1/l3c/mazeworld/tests/test.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)     2390 2024-02-22 11:56:16.000000 l3c-0.1.0.1/l3c/mazeworld/tests/test_agent.py
+drwxr-xr-x   0 wangfan04   (502) staff       (20)        0 2024-04-15 03:50:00.527003 l3c-0.1.0.1/l3c/metalm/
+-rw-r--r--   0 wangfan04   (502) staff       (20)     1080 2023-05-09 04:51:28.000000 l3c-0.1.0.1/l3c/metalm/__init__.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)     2294 2024-02-01 05:22:53.000000 l3c-0.1.0.1/l3c/metalm/data_generator.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)     4267 2024-02-01 05:22:53.000000 l3c-0.1.0.1/l3c/metalm/metalmv1.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)     5530 2024-02-01 05:22:53.000000 l3c-0.1.0.1/l3c/metalm/metalmv2.py
+drwxr-xr-x   0 wangfan04   (502) staff       (20)        0 2024-04-15 03:50:00.512007 l3c-0.1.0.1/l3c.egg-info/
+-rw-r--r--   0 wangfan04   (502) staff       (20)      953 2024-04-15 03:50:00.000000 l3c-0.1.0.1/l3c.egg-info/PKG-INFO
+-rw-r--r--   0 wangfan04   (502) staff       (20)     1075 2024-04-15 03:50:00.000000 l3c-0.1.0.1/l3c.egg-info/SOURCES.txt
+-rw-r--r--   0 wangfan04   (502) staff       (20)        1 2024-04-15 03:50:00.000000 l3c-0.1.0.1/l3c.egg-info/dependency_links.txt
+-rw-r--r--   0 wangfan04   (502) staff       (20)        1 2023-04-19 12:54:38.000000 l3c-0.1.0.1/l3c.egg-info/not-zip-safe
+-rw-r--r--   0 wangfan04   (502) staff       (20)       84 2024-04-15 03:50:00.000000 l3c-0.1.0.1/l3c.egg-info/requires.txt
+-rw-r--r--   0 wangfan04   (502) staff       (20)        4 2024-04-15 03:50:00.000000 l3c-0.1.0.1/l3c.egg-info/top_level.txt
+-rw-r--r--   0 wangfan04   (502) staff       (20)       38 2024-04-15 03:50:00.527801 l3c-0.1.0.1/setup.cfg
+-rwxr-xr-x   0 wangfan04   (502) staff       (20)     1814 2024-04-15 03:49:23.000000 l3c-0.1.0.1/setup.py
```

### Comparing `l3c-0.1.0/LICENSE` & `l3c-0.1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `l3c-0.1.0/PKG-INFO` & `l3c-0.1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: l3c
-Version: 0.1.0
+Version: 0.1.0.1
 Summary: L3C provide abundant environments for Lifelong Learning (L3) in Context.
 Home-page: https://github.com/FutureAGI/L3C
 Author: WorldEditors
 Author-email: 
 License: Apache
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `l3c-0.1.0/README.md` & `l3c-0.1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `l3c-0.1.0/l3c/__init__.py` & `l3c-0.1.0.1/l3c/__init__.py`

 * *Files identical despite different names*

### Comparing `l3c-0.1.0/l3c/bandits/__init__.py` & `l3c-0.1.0.1/l3c/bandits/__init__.py`

 * *Files identical despite different names*

### Comparing `l3c-0.1.0/l3c/bandits/bandits_env.py` & `l3c-0.1.0.1/l3c/bandits/bandits_env.py`

 * *Files identical despite different names*

### Comparing `l3c-0.1.0/l3c/bandits/demo_thompson_sampling.py` & `l3c-0.1.0.1/l3c/bandits/demo_thompson_sampling.py`

 * *Files identical despite different names*

### Comparing `l3c-0.1.0/l3c/mazeworld/__init__.py` & `l3c-0.1.0.1/l3c/mazeworld/__init__.py`

 * *Files identical despite different names*

### Comparing `l3c-0.1.0/l3c/mazeworld/agents/agent_base.py` & `l3c-0.1.0.1/l3c/mazeworld/agents/agent_base.py`

 * *Files identical despite different names*

### Comparing `l3c-0.1.0/l3c/mazeworld/agents/smart_slam_agent.py` & `l3c-0.1.0.1/l3c/mazeworld/agents/smart_slam_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -178,20 +178,20 @@
         req_ori = 2.0 * math.atan2(d_y, d_x) / PI
         deta_ori = req_ori - self._agent_ori
         deta_ori = int(deta_ori) % 4 + deta_ori - int(deta_ori)
         if(deta_ori > 2):
             deta_ori -= 4
         if(numpy.abs(deta_ori) < 0.2):
             return 4 #(0, 1)
-        elif(numpy.abs(deta_ori) > 1.8 and self._god_info[path[1]] >=0 and self._mask_info[path[1]]>0):
-            return 3 #(0, -1)
         elif(deta_ori < 0):
-            return 2 #(-1, 0)
+            return 1 #(-1, 0)
         else:
-            return 1 #(1, 0)
+            return 2 #(1, 0)
+        #elif(numpy.abs(deta_ori) > 1.8 and self._god_info[path[1]] >=0 and self._mask_info[path[1]]>0):
+        #    return 3 #(0, -1)
 
     def path_to_action_cont3d(self, path):
         if(len(path) < 2):
             d_x = path[0][0] + 0.5 - self._cur_grid_float[0]
             d_y = path[0][1] + 0.5 - self._cur_grid_float[1]
             deta_s = numpy.sqrt(d_x ** 2 + d_y ** 2)
             if(deta_s < 0.20):
@@ -203,15 +203,15 @@
         req_ori = 2.0 * math.atan2(d_y, d_x) / PI
         deta_ori = req_ori - self._agent_ori
         deta_ori = int(deta_ori) % 4 + deta_ori - int(deta_ori)
         if(deta_ori > 2):
             deta_ori -= 4
         if(numpy.abs(deta_ori) < 0.50):
             spd = min(deta_s, 1.0)
-        elif(numpy.abs(deta_ori) > 1.50):
+        elif(numpy.abs(deta_ori) > 1.95):
             spd = - min(deta_s, 1.0)
         else:
             spd = 0.0
         if(deta_ori < 0):
             turn = - min(numpy.abs(deta_ori), 1.0)
         else:
             turn = min(numpy.abs(deta_ori), 1.0)
```

### Comparing `l3c-0.1.0/l3c/mazeworld/demo/agent_play_demo.py` & `l3c-0.1.0.1/l3c/mazeworld/demo/agent_play_demo.py`

 * *Files identical despite different names*

### Comparing `l3c-0.1.0/l3c/mazeworld/demo/keyboard_play_demo.py` & `l3c-0.1.0.1/l3c/mazeworld/demo/keyboard_play_demo.py`

 * *Files identical despite different names*

### Comparing `l3c-0.1.0/l3c/mazeworld/envs/dynamics.py` & `l3c-0.1.0.1/l3c/mazeworld/envs/dynamics.py`

 * *Files identical despite different names*

### Comparing `l3c-0.1.0/l3c/mazeworld/envs/maze_base.py` & `l3c-0.1.0.1/l3c/mazeworld/envs/maze_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
     def refresh_command(self):
         """
         Update the command for selecting the target to navigate
         At the same time, update the instant_rewards
         Valid only for ``NAVIGATION`` mode
         """
-        if(self.task_type is not "NAVIGATION"):
+        if(self.task_type != "NAVIGATION"):
             return
         if(self._command is not None):
             x,y = self._landmarks_coordinates[self._command]
             self._instant_rewards[x, y] = 0.0
 
         self._commands_sequence_idx += 1
         if(self._commands_sequence_idx > len(self._commands_sequence) - 1):
@@ -191,15 +191,15 @@
         Cover landmarks with white in case it is not refreshed
         """
         for landmarks_id, (x,y) in enumerate(self._landmarks_coordinates):
             if(self._landmarks_refresh_countdown[landmarks_id] > self._landmarks_refresh_interval):
                 pygame.draw.rect(scr, landmarks_color(landmarks_id), 
                         (x * self._render_cell_size + offset[0], y * self._render_cell_size + offset[1],
                         self._render_cell_size, self._render_cell_size), width=0)
-        if(self.task_type is "SURVIVAL"):
+        if(self.task_type == "SURVIVAL"):
             txt_life = self._font.render("Life: %f"%self._life, 0, pygame.Color("green"))
             scr.blit(txt_life,(offset[0] + 90, offset[1] + 10))
 
     def render_localmap(self, scr, offset):
         """
         Cover landmarks with white in case it is not refreshed
         """
```

### Comparing `l3c-0.1.0/l3c/mazeworld/envs/maze_continuous_3d.py` & `l3c-0.1.0.1/l3c/mazeworld/envs/maze_continuous_3d.py`

 * *Files identical despite different names*

### Comparing `l3c-0.1.0/l3c/mazeworld/envs/maze_discrete_2d.py` & `l3c-0.1.0.1/l3c/mazeworld/envs/maze_discrete_2d.py`

 * *Files identical despite different names*

### Comparing `l3c-0.1.0/l3c/mazeworld/envs/maze_discrete_3d.py` & `l3c-0.1.0.1/l3c/mazeworld/envs/maze_discrete_3d.py`

 * *Files identical despite different names*

### Comparing `l3c-0.1.0/l3c/mazeworld/envs/maze_env.py` & `l3c-0.1.0.1/l3c/mazeworld/envs/maze_env.py`

 * *Files 6% similar despite different names*

```diff
@@ -81,14 +81,17 @@
 
     def render(self, mode="human"):
         if(mode != "human"):
             raise NotImplementedError("Only human mode is supported")
         if(self.enable_render):
             self.key_done, self.keyboard_press = self.maze_core.render_update()
 
+    def get_loc_map(self, map_range=2):
+        return self.maze_core.get_loc_map(map_rang=map_range)
+
     def save_trajectory(self, file_name):
         self.maze_core.render_trajectory(file_name)
 
 class MazeWorldContinuous3D(gym.Env):
     def __init__(self, 
             enable_render=True,
             render_scale=480,
@@ -159,14 +162,17 @@
 
     def render(self, mode="human"):
         if(mode != "human"):
             raise NotImplementedError("Only human mode is supported")
         if(self.enable_render):
             self.key_done, self.keyboard_press = self.maze_core.render_update()
 
+    def get_loc_map(self, map_range=2):
+        return self.maze_core.get_loc_map(map_rang=map_range)
+
     def save_trajectory(self, file_name):
         self.maze_core.render_trajectory(file_name)
 
 class MazeWorldDiscrete2D(gym.Env):
     def __init__(self,
             enable_render=True,
             render_scale=480,
@@ -228,9 +234,12 @@
 
     def render(self, mode="human"):
         if(mode != "human"):
             raise NotImplementedError("Only human mode is supported")
         if(self.enable_render):
             self.key_done, self.keyboard_press = self.maze_core.render_update()
 
+    def get_loc_map(self, map_range=2):
+        return self.maze_core.get_loc_map(map_rang=map_range)
+
     def save_trajectory(self, file_name, additional=None):
         self.maze_core.render_trajectory(file_name, additional=additional)
```

### Comparing `l3c-0.1.0/l3c/mazeworld/envs/maze_task.py` & `l3c-0.1.0.1/l3c/mazeworld/envs/maze_task.py`

 * *Files identical despite different names*

### Comparing `l3c-0.1.0/l3c/mazeworld/envs/ray_caster_utils.py` & `l3c-0.1.0.1/l3c/mazeworld/envs/ray_caster_utils.py`

 * *Files identical despite different names*

### Comparing `l3c-0.1.0/l3c/mazeworld/tests/test.py` & `l3c-0.1.0.1/l3c/mazeworld/tests/test.py`

 * *Files identical despite different names*

### Comparing `l3c-0.1.0/l3c/mazeworld/tests/test_agent.py` & `l3c-0.1.0.1/l3c/mazeworld/tests/test_agent.py`

 * *Files identical despite different names*

### Comparing `l3c-0.1.0/l3c/metalm/__init__.py` & `l3c-0.1.0.1/l3c/metalm/__init__.py`

 * *Files identical despite different names*

### Comparing `l3c-0.1.0/l3c/metalm/data_generator.py` & `l3c-0.1.0.1/l3c/metalm/data_generator.py`

 * *Files identical despite different names*

### Comparing `l3c-0.1.0/l3c/metalm/metalmv1.py` & `l3c-0.1.0.1/l3c/metalm/metalmv1.py`

 * *Files identical despite different names*

### Comparing `l3c-0.1.0/l3c/metalm/metalmv2.py` & `l3c-0.1.0.1/l3c/metalm/metalmv2.py`

 * *Files identical despite different names*

### Comparing `l3c-0.1.0/l3c.egg-info/PKG-INFO` & `l3c-0.1.0.1/l3c.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: l3c
-Version: 0.1.0
+Version: 0.1.0.1
 Summary: L3C provide abundant environments for Lifelong Learning (L3) in Context.
 Home-page: https://github.com/FutureAGI/L3C
 Author: WorldEditors
 Author-email: 
 License: Apache
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `l3c-0.1.0/l3c.egg-info/SOURCES.txt` & `l3c-0.1.0.1/l3c.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 l3c/bandits/demo_thompson_sampling.py
 l3c/mazeworld/__init__.py
 l3c/mazeworld/agents/__init__.py
 l3c/mazeworld/agents/agent_base.py
 l3c/mazeworld/agents/smart_slam_agent.py
 l3c/mazeworld/demo/__init__.py
 l3c/mazeworld/demo/agent_play_demo.py
+l3c/mazeworld/demo/dump_maze.py
 l3c/mazeworld/demo/keyboard_play_demo.py
 l3c/mazeworld/envs/__init__.py
 l3c/mazeworld/envs/dynamics.py
 l3c/mazeworld/envs/maze_base.py
 l3c/mazeworld/envs/maze_continuous_3d.py
 l3c/mazeworld/envs/maze_discrete_2d.py
 l3c/mazeworld/envs/maze_discrete_3d.py
```

### Comparing `l3c-0.1.0/setup.py` & `l3c-0.1.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import io
 from setuptools import setup, find_packages
 
-__version__ = '0.1.0'
+__version__ = '0.1.0.1'
 
 with io.open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='l3c',
     version=__version__,
```

