# Comparing `tmp/pyprland-2.2.7.tar.gz` & `tmp/pyprland-2.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyprland-2.2.7.tar", max compression
+gzip compressed data, was "pyprland-2.2.8.tar", max compression
```

## Comparing `pyprland-2.2.7.tar` & `pyprland-2.2.8.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1070 2024-02-16 16:53:56.731771 pyprland-2.2.7/LICENSE
--rw-r--r--   0        0        0     4458 2024-04-14 21:04:51.031595 pyprland-2.2.7/README.md
--rw-r--r--   0        0        0        0 2024-03-03 01:47:24.891034 pyprland-2.2.7/pyprland/__init__.py
--rw-r--r--   0        0        0        0 2024-03-03 01:47:24.891034 pyprland-2.2.7/pyprland/adapters/__init__.py
--rw-r--r--   0        0        0      400 2024-04-05 20:13:47.397221 pyprland-2.2.7/pyprland/adapters/colors.py
--rw-r--r--   0        0        0     4377 2024-03-03 01:47:24.894367 pyprland-2.2.7/pyprland/adapters/menus.py
--rw-r--r--   0        0        0     1395 2024-04-08 20:00:16.866561 pyprland-2.2.7/pyprland/adapters/units.py
--rwxr-xr-x   0        0        0    16724 2024-04-15 19:22:23.194940 pyprland-2.2.7/pyprland/command.py
--rw-r--r--   0        0        0     7573 2024-04-13 21:52:18.927484 pyprland-2.2.7/pyprland/common.py
--rw-r--r--   0        0        0     7197 2024-04-12 17:07:08.504043 pyprland-2.2.7/pyprland/ipc.py
--rw-r--r--   0        0        0       45 2024-03-03 01:47:24.897701 pyprland-2.2.7/pyprland/plugins/__init__.py
--rw-r--r--   0        0        0      106 2024-03-03 01:47:24.897701 pyprland-2.2.7/pyprland/plugins/experimental.py
--rw-r--r--   0        0        0     1647 2024-04-15 15:21:49.122927 pyprland-2.2.7/pyprland/plugins/expose.py
--rw-r--r--   0        0        0     1386 2024-03-30 16:09:04.631012 pyprland-2.2.7/pyprland/plugins/fetch_client_menu.py
--rw-r--r--   0        0        0     2018 2024-04-14 20:56:27.261784 pyprland-2.2.7/pyprland/plugins/gbar.py
--rw-r--r--   0        0        0     2589 2024-04-09 20:50:41.034540 pyprland-2.2.7/pyprland/plugins/interface.py
--rw-r--r--   0        0        0     7972 2024-03-03 01:47:24.917701 pyprland-2.2.7/pyprland/plugins/layout_center.py
--rw-r--r--   0        0        0     1677 2024-03-03 01:47:24.901034 pyprland-2.2.7/pyprland/plugins/lost_windows.py
--rw-r--r--   0        0        0     1239 2024-04-03 21:48:38.877707 pyprland-2.2.7/pyprland/plugins/magnify.py
--rw-r--r--   0        0        0     8680 2024-04-13 18:26:06.759226 pyprland-2.2.7/pyprland/plugins/monitors.py
--rw-r--r--   0        0        0     3922 2024-03-03 01:47:24.904368 pyprland-2.2.7/pyprland/plugins/monitors_v0.py
--rw-r--r--   0        0        0     1770 2024-04-13 21:52:18.890816 pyprland-2.2.7/pyprland/plugins/pyprland.py
--rw-r--r--   0        0        0    26132 2024-04-14 20:57:42.622754 pyprland-2.2.7/pyprland/plugins/scratchpads/__init__.py
--rw-r--r--   0        0        0     2641 2024-04-12 17:24:50.007112 pyprland-2.2.7/pyprland/plugins/scratchpads/animations.py
--rw-r--r--   0        0        0     2106 2024-04-12 17:23:41.858277 pyprland-2.2.7/pyprland/plugins/scratchpads/helpers.py
--rw-r--r--   0        0        0     3436 2024-04-12 17:21:22.436949 pyprland-2.2.7/pyprland/plugins/scratchpads/lookup.py
--rw-r--r--   0        0        0     4136 2024-04-12 17:19:16.255742 pyprland-2.2.7/pyprland/plugins/scratchpads/objects.py
--rw-r--r--   0        0        0     1058 2024-03-03 01:47:24.907701 pyprland-2.2.7/pyprland/plugins/shift_monitors.py
--rw-r--r--   0        0        0     4161 2024-04-09 15:53:04.519223 pyprland-2.2.7/pyprland/plugins/shortcuts_menu.py
--rw-r--r--   0        0        0     3983 2024-04-09 21:03:19.309538 pyprland-2.2.7/pyprland/plugins/system_notifier.py
--rw-r--r--   0        0        0      519 2024-03-03 01:47:24.911034 pyprland-2.2.7/pyprland/plugins/toggle_dpms.py
--rw-r--r--   0        0        0     1063 2024-03-03 01:47:24.917701 pyprland-2.2.7/pyprland/plugins/toggle_special.py
--rw-r--r--   0        0        0     5335 2024-04-13 18:20:53.870052 pyprland-2.2.7/pyprland/plugins/wallpapers.py
--rw-r--r--   0        0        0     2559 2024-04-14 20:57:42.622754 pyprland-2.2.7/pyprland/plugins/workspaces_follow_focus.py
--rw-r--r--   0        0        0      725 2024-04-15 19:22:23.184940 pyprland-2.2.7/pyproject.toml
--rw-r--r--   0        0        0     4997 1970-01-01 00:00:00.000000 pyprland-2.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-02-16 16:53:56.731771 pyprland-2.2.8/LICENSE
+-rw-r--r--   0        0        0     4458 2024-04-14 21:04:51.031595 pyprland-2.2.8/README.md
+-rw-r--r--   0        0        0        0 2024-03-03 01:47:24.891034 pyprland-2.2.8/pyprland/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-03 01:47:24.891034 pyprland-2.2.8/pyprland/adapters/__init__.py
+-rw-r--r--   0        0        0      400 2024-04-05 20:13:47.397221 pyprland-2.2.8/pyprland/adapters/colors.py
+-rw-r--r--   0        0        0     4377 2024-03-03 01:47:24.894367 pyprland-2.2.8/pyprland/adapters/menus.py
+-rw-r--r--   0        0        0     1395 2024-04-08 20:00:16.866561 pyprland-2.2.8/pyprland/adapters/units.py
+-rwxr-xr-x   0        0        0    16724 2024-04-16 20:54:29.573076 pyprland-2.2.8/pyprland/command.py
+-rw-r--r--   0        0        0     7574 2024-04-16 20:17:47.161668 pyprland-2.2.8/pyprland/common.py
+-rw-r--r--   0        0        0     7197 2024-04-12 17:07:08.504043 pyprland-2.2.8/pyprland/ipc.py
+-rw-r--r--   0        0        0       45 2024-03-03 01:47:24.897701 pyprland-2.2.8/pyprland/plugins/__init__.py
+-rw-r--r--   0        0        0      106 2024-03-03 01:47:24.897701 pyprland-2.2.8/pyprland/plugins/experimental.py
+-rw-r--r--   0        0        0     1647 2024-04-15 15:21:49.122927 pyprland-2.2.8/pyprland/plugins/expose.py
+-rw-r--r--   0        0        0     1386 2024-03-30 16:09:04.631012 pyprland-2.2.8/pyprland/plugins/fetch_client_menu.py
+-rw-r--r--   0        0        0     2018 2024-04-14 20:56:27.261784 pyprland-2.2.8/pyprland/plugins/gbar.py
+-rw-r--r--   0        0        0     2589 2024-04-09 20:50:41.034540 pyprland-2.2.8/pyprland/plugins/interface.py
+-rw-r--r--   0        0        0     7972 2024-03-03 01:47:24.917701 pyprland-2.2.8/pyprland/plugins/layout_center.py
+-rw-r--r--   0        0        0     1677 2024-03-03 01:47:24.901034 pyprland-2.2.8/pyprland/plugins/lost_windows.py
+-rw-r--r--   0        0        0     1239 2024-04-03 21:48:38.877707 pyprland-2.2.8/pyprland/plugins/magnify.py
+-rw-r--r--   0        0        0     8680 2024-04-13 18:26:06.759226 pyprland-2.2.8/pyprland/plugins/monitors.py
+-rw-r--r--   0        0        0     3922 2024-03-03 01:47:24.904368 pyprland-2.2.8/pyprland/plugins/monitors_v0.py
+-rw-r--r--   0        0        0     1770 2024-04-13 21:52:18.890816 pyprland-2.2.8/pyprland/plugins/pyprland.py
+-rw-r--r--   0        0        0    26132 2024-04-14 20:57:42.622754 pyprland-2.2.8/pyprland/plugins/scratchpads/__init__.py
+-rw-r--r--   0        0        0     2641 2024-04-12 17:24:50.007112 pyprland-2.2.8/pyprland/plugins/scratchpads/animations.py
+-rw-r--r--   0        0        0     2106 2024-04-12 17:23:41.858277 pyprland-2.2.8/pyprland/plugins/scratchpads/helpers.py
+-rw-r--r--   0        0        0     3436 2024-04-12 17:21:22.436949 pyprland-2.2.8/pyprland/plugins/scratchpads/lookup.py
+-rw-r--r--   0        0        0     4136 2024-04-12 17:19:16.255742 pyprland-2.2.8/pyprland/plugins/scratchpads/objects.py
+-rw-r--r--   0        0        0     1058 2024-03-03 01:47:24.907701 pyprland-2.2.8/pyprland/plugins/shift_monitors.py
+-rw-r--r--   0        0        0     4161 2024-04-09 15:53:04.519223 pyprland-2.2.8/pyprland/plugins/shortcuts_menu.py
+-rw-r--r--   0        0        0     3983 2024-04-09 21:03:19.309538 pyprland-2.2.8/pyprland/plugins/system_notifier.py
+-rw-r--r--   0        0        0      519 2024-03-03 01:47:24.911034 pyprland-2.2.8/pyprland/plugins/toggle_dpms.py
+-rw-r--r--   0        0        0     1063 2024-03-03 01:47:24.917701 pyprland-2.2.8/pyprland/plugins/toggle_special.py
+-rw-r--r--   0        0        0     5335 2024-04-13 18:20:53.870052 pyprland-2.2.8/pyprland/plugins/wallpapers.py
+-rw-r--r--   0        0        0     2559 2024-04-14 20:57:42.622754 pyprland-2.2.8/pyprland/plugins/workspaces_follow_focus.py
+-rw-r--r--   0        0        0      725 2024-04-16 20:54:29.563076 pyprland-2.2.8/pyproject.toml
+-rw-r--r--   0        0        0     4997 1970-01-01 00:00:00.000000 pyprland-2.2.8/PKG-INFO
```

### Comparing `pyprland-2.2.7/LICENSE` & `pyprland-2.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.7/README.md` & `pyprland-2.2.8/README.md`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.7/pyprland/adapters/menus.py` & `pyprland-2.2.8/pyprland/adapters/menus.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.7/pyprland/adapters/units.py` & `pyprland-2.2.8/pyprland/adapters/units.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.7/pyprland/command.py` & `pyprland-2.2.8/pyprland/command.py`

 * *Files 0% similar despite different names*

```diff
@@ -391,15 +391,15 @@
 
 
 async def run_client():
     "Runs the client (CLI)"
     manager = Pyprland()
 
     if sys.argv[1] == "version":
-        print("2.2.7")  # Automatically updated version
+        print("2.2.8")  # Automatically updated version
         return
 
     if sys.argv[1] == "edit":
         editor = os.environ.get("EDITOR", os.environ.get("VISUAL", "vi"))
         filename = os.path.expanduser(CONFIG_FILE)
         run_interactive_program(f'{editor} "{filename}"')
         sys.argv[1] = "reload"
```

### Comparing `pyprland-2.2.7/pyprland/common.py` & `pyprland-2.2.8/pyprland/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -81,30 +81,31 @@
     except OSError:
         pass
     finally:
         # Restore terminal settings
         termios.tcsetattr(sys.stdin, termios.TCSANOW, termios.tcgetattr(0))
 
 
-def merge(obj1, obj2):
+def merge(merged, obj2):
     """
     Merges the content of d2 into d1
+    Eg:
+        merge({"a": {"b": 1}}, {"a": {"c": 2}}) == {"a": {"b": 1, "c": 2}}
 
     Args:
-    - obj1 (dict): First dictionary to merge (will be updated).
+    - merged (dict): First dictionary to merge (will be updated).
     - obj2 (dict): Second dictionary to merge
 
     Returns:
     - dict: Merged dictionary
     """
-    merged = obj1.copy()  # Make a shallow copy of the first dictionary
     for key, value in obj2.items():
         if key in merged and isinstance(merged[key], dict) and isinstance(value, dict):
             # If both values are dictionaries, recursively merge them
-            merged[key] = merge(merged[key], value)
+            merge(merged[key], value)
         elif (
             key in merged and isinstance(merged[key], list) and isinstance(value, list)
         ):
             # If both values are lists, concatenate them
             merged[key] += value
         else:
             # Otherwise, update the value or add the key-value pair
```

### Comparing `pyprland-2.2.7/pyprland/ipc.py` & `pyprland-2.2.8/pyprland/ipc.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.7/pyprland/plugins/expose.py` & `pyprland-2.2.8/pyprland/plugins/expose.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.7/pyprland/plugins/fetch_client_menu.py` & `pyprland-2.2.8/pyprland/plugins/fetch_client_menu.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.7/pyprland/plugins/gbar.py` & `pyprland-2.2.8/pyprland/plugins/gbar.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.7/pyprland/plugins/interface.py` & `pyprland-2.2.8/pyprland/plugins/interface.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.7/pyprland/plugins/layout_center.py` & `pyprland-2.2.8/pyprland/plugins/layout_center.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.7/pyprland/plugins/lost_windows.py` & `pyprland-2.2.8/pyprland/plugins/lost_windows.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.7/pyprland/plugins/magnify.py` & `pyprland-2.2.8/pyprland/plugins/magnify.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.7/pyprland/plugins/monitors.py` & `pyprland-2.2.8/pyprland/plugins/monitors.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.7/pyprland/plugins/monitors_v0.py` & `pyprland-2.2.8/pyprland/plugins/monitors_v0.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.7/pyprland/plugins/pyprland.py` & `pyprland-2.2.8/pyprland/plugins/pyprland.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.7/pyprland/plugins/scratchpads/__init__.py` & `pyprland-2.2.8/pyprland/plugins/scratchpads/__init__.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.7/pyprland/plugins/scratchpads/animations.py` & `pyprland-2.2.8/pyprland/plugins/scratchpads/animations.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.7/pyprland/plugins/scratchpads/helpers.py` & `pyprland-2.2.8/pyprland/plugins/scratchpads/helpers.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.7/pyprland/plugins/scratchpads/lookup.py` & `pyprland-2.2.8/pyprland/plugins/scratchpads/lookup.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.7/pyprland/plugins/scratchpads/objects.py` & `pyprland-2.2.8/pyprland/plugins/scratchpads/objects.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.7/pyprland/plugins/shift_monitors.py` & `pyprland-2.2.8/pyprland/plugins/shift_monitors.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.7/pyprland/plugins/shortcuts_menu.py` & `pyprland-2.2.8/pyprland/plugins/shortcuts_menu.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.7/pyprland/plugins/system_notifier.py` & `pyprland-2.2.8/pyprland/plugins/system_notifier.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.7/pyprland/plugins/toggle_dpms.py` & `pyprland-2.2.8/pyprland/plugins/toggle_dpms.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.7/pyprland/plugins/toggle_special.py` & `pyprland-2.2.8/pyprland/plugins/toggle_special.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.7/pyprland/plugins/wallpapers.py` & `pyprland-2.2.8/pyprland/plugins/wallpapers.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.7/pyprland/plugins/workspaces_follow_focus.py` & `pyprland-2.2.8/pyprland/plugins/workspaces_follow_focus.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.7/pyproject.toml` & `pyprland-2.2.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyprland"
-version = "2.2.7"
+version = "2.2.8"
 description = "Hyperland plugin system - batteries included"
 authors = ["fdev31 <fdev31@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pyprland"}]
 homepage = "https://github.com/hyprland-community/pyprland/"
```

### Comparing `pyprland-2.2.7/PKG-INFO` & `pyprland-2.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyprland
-Version: 2.2.7
+Version: 2.2.8
 Summary: Hyperland plugin system - batteries included
 Home-page: https://github.com/hyprland-community/pyprland/
 License: MIT
 Author: fdev31
 Author-email: fdev31@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

