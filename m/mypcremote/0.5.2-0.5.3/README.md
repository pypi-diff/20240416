# Comparing `tmp/mypcremote-0.5.2.tar.gz` & `tmp/mypcremote-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypcremote-0.5.2.tar", last modified: Mon Apr 15 11:19:14 2024, max compression
+gzip compressed data, was "mypcremote-0.5.3.tar", last modified: Tue Apr 16 12:30:38 2024, max compression
```

## Comparing `mypcremote-0.5.2.tar` & `mypcremote-0.5.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 11:19:14.034178 mypcremote-0.5.2/
--rw-rw-rw-   0        0        0     1092 2024-04-15 07:22:18.000000 mypcremote-0.5.2/LICENSE
--rw-rw-rw-   0        0        0     3825 2024-04-15 11:19:14.033178 mypcremote-0.5.2/PKG-INFO
--rw-rw-rw-   0        0        0     2812 2024-04-15 08:04:42.000000 mypcremote-0.5.2/README.md
--rw-rw-rw-   0        0        0     1233 2024-04-15 11:15:43.000000 mypcremote-0.5.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-15 11:19:14.034178 mypcremote-0.5.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-15 11:19:13.979840 mypcremote-0.5.2/src/
-drwxrwxrwx   0        0        0        0 2024-04-15 11:19:13.993275 mypcremote-0.5.2/src/mypcremote/
--rw-rw-rw-   0        0        0     2106 2024-04-15 11:06:09.000000 mypcremote-0.5.2/src/mypcremote/__main__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 11:19:14.030138 mypcremote-0.5.2/src/mypcremote/commands/
--rw-rw-rw-   0        0        0        0 2023-11-10 12:39:58.000000 mypcremote-0.5.2/src/mypcremote/commands/__init__.py
--rw-rw-rw-   0        0        0      453 2023-11-12 15:27:05.000000 mypcremote-0.5.2/src/mypcremote/commands/beep.py
--rw-rw-rw-   0        0        0      671 2023-11-11 11:31:42.000000 mypcremote-0.5.2/src/mypcremote/commands/camera.py
--rw-rw-rw-   0        0        0      547 2023-11-11 11:30:48.000000 mypcremote-0.5.2/src/mypcremote/commands/clear.py
--rw-rw-rw-   0        0        0      628 2023-11-12 14:41:43.000000 mypcremote-0.5.2/src/mypcremote/commands/hybernate.py
--rw-rw-rw-   0        0        0     1588 2023-11-12 14:20:10.000000 mypcremote-0.5.2/src/mypcremote/commands/kill.py
--rw-rw-rw-   0        0        0      694 2023-11-24 17:15:03.000000 mypcremote-0.5.2/src/mypcremote/commands/location.py
--rw-rw-rw-   0        0        0      690 2023-11-11 11:30:21.000000 mypcremote-0.5.2/src/mypcremote/commands/lock.py
--rw-rw-rw-   0        0        0     1528 2023-11-13 05:53:39.000000 mypcremote-0.5.2/src/mypcremote/commands/notify.py
--rw-rw-rw-   0        0        0      518 2023-11-13 08:29:30.000000 mypcremote-0.5.2/src/mypcremote/commands/openurl.py
--rw-rw-rw-   0        0        0      145 2023-11-12 14:45:38.000000 mypcremote-0.5.2/src/mypcremote/commands/ping.py
--rw-rw-rw-   0        0        0      710 2023-11-11 11:30:01.000000 mypcremote-0.5.2/src/mypcremote/commands/reboot.py
--rw-rw-rw-   0        0        0      410 2023-11-11 11:29:27.000000 mypcremote-0.5.2/src/mypcremote/commands/screenshot.py
--rw-rw-rw-   0        0        0      763 2023-11-11 11:28:54.000000 mypcremote-0.5.2/src/mypcremote/commands/shutdown.py
--rw-rw-rw-   0        0        0      717 2023-11-11 11:28:24.000000 mypcremote-0.5.2/src/mypcremote/commands/sleep.py
--rw-rw-rw-   0        0        0      676 2023-11-11 14:09:49.000000 mypcremote-0.5.2/src/mypcremote/commands/speak.py
--rw-rw-rw-   0        0        0      692 2023-11-11 11:28:42.000000 mypcremote-0.5.2/src/mypcremote/commands/status.py
--rw-rw-rw-   0        0        0      440 2023-11-11 11:26:35.000000 mypcremote-0.5.2/src/mypcremote/commands/terminal.py
--rw-rw-rw-   0        0        0      210 2023-11-13 08:33:07.000000 mypcremote-0.5.2/src/mypcremote/commands/terminate.py
--rw-rw-rw-   0        0        0     1005 2023-11-12 14:31:11.000000 mypcremote-0.5.2/src/mypcremote/commands/upload.py
--rw-rw-rw-   0        0        0     1081 2023-11-11 11:27:07.000000 mypcremote-0.5.2/src/mypcremote/commands/voicecall.py
--rw-rw-rw-   0        0        0     1387 2023-11-12 13:56:04.000000 mypcremote-0.5.2/src/mypcremote/commands/volume.py
-drwxrwxrwx   0        0        0        0 2024-04-15 11:19:14.032194 mypcremote-0.5.2/src/mypcremote.egg-info/
--rw-rw-rw-   0        0        0     3825 2024-04-15 11:19:13.000000 mypcremote-0.5.2/src/mypcremote.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1048 2024-04-15 11:19:13.000000 mypcremote-0.5.2/src/mypcremote.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 11:19:13.000000 mypcremote-0.5.2/src/mypcremote.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2024-04-15 11:19:13.000000 mypcremote-0.5.2/src/mypcremote.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      129 2024-04-15 11:19:13.000000 mypcremote-0.5.2/src/mypcremote.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-15 11:19:13.000000 mypcremote-0.5.2/src/mypcremote.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-16 12:30:38.440480 mypcremote-0.5.3/
+-rw-rw-rw-   0        0        0     1092 2024-04-15 07:22:18.000000 mypcremote-0.5.3/LICENSE
+-rw-rw-rw-   0        0        0     3825 2024-04-16 12:30:38.439410 mypcremote-0.5.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2812 2024-04-15 08:04:42.000000 mypcremote-0.5.3/README.md
+-rw-rw-rw-   0        0        0     1233 2024-04-16 12:24:07.000000 mypcremote-0.5.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-16 12:30:38.441451 mypcremote-0.5.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-16 12:30:38.392419 mypcremote-0.5.3/src/
+drwxrwxrwx   0        0        0        0 2024-04-16 12:30:38.397480 mypcremote-0.5.3/src/mypcremote/
+-rw-rw-rw-   0        0        0       35 2024-04-16 12:15:51.000000 mypcremote-0.5.3/src/mypcremote/__main__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 12:30:38.436810 mypcremote-0.5.3/src/mypcremote/commands/
+-rw-rw-rw-   0        0        0        0 2023-11-10 12:39:58.000000 mypcremote-0.5.3/src/mypcremote/commands/__init__.py
+-rw-rw-rw-   0        0        0      453 2023-11-12 15:27:05.000000 mypcremote-0.5.3/src/mypcremote/commands/beep.py
+-rw-rw-rw-   0        0        0      671 2023-11-11 11:31:42.000000 mypcremote-0.5.3/src/mypcremote/commands/camera.py
+-rw-rw-rw-   0        0        0      547 2023-11-11 11:30:48.000000 mypcremote-0.5.3/src/mypcremote/commands/clear.py
+-rw-rw-rw-   0        0        0      628 2023-11-12 14:41:43.000000 mypcremote-0.5.3/src/mypcremote/commands/hybernate.py
+-rw-rw-rw-   0        0        0     1588 2023-11-12 14:20:10.000000 mypcremote-0.5.3/src/mypcremote/commands/kill.py
+-rw-rw-rw-   0        0        0      694 2023-11-24 17:15:03.000000 mypcremote-0.5.3/src/mypcremote/commands/location.py
+-rw-rw-rw-   0        0        0      690 2023-11-11 11:30:21.000000 mypcremote-0.5.3/src/mypcremote/commands/lock.py
+-rw-rw-rw-   0        0        0     1528 2023-11-13 05:53:39.000000 mypcremote-0.5.3/src/mypcremote/commands/notify.py
+-rw-rw-rw-   0        0        0      518 2023-11-13 08:29:30.000000 mypcremote-0.5.3/src/mypcremote/commands/openurl.py
+-rw-rw-rw-   0        0        0      145 2023-11-12 14:45:38.000000 mypcremote-0.5.3/src/mypcremote/commands/ping.py
+-rw-rw-rw-   0        0        0      710 2023-11-11 11:30:01.000000 mypcremote-0.5.3/src/mypcremote/commands/reboot.py
+-rw-rw-rw-   0        0        0      410 2023-11-11 11:29:27.000000 mypcremote-0.5.3/src/mypcremote/commands/screenshot.py
+-rw-rw-rw-   0        0        0      763 2023-11-11 11:28:54.000000 mypcremote-0.5.3/src/mypcremote/commands/shutdown.py
+-rw-rw-rw-   0        0        0      717 2023-11-11 11:28:24.000000 mypcremote-0.5.3/src/mypcremote/commands/sleep.py
+-rw-rw-rw-   0        0        0      676 2023-11-11 14:09:49.000000 mypcremote-0.5.3/src/mypcremote/commands/speak.py
+-rw-rw-rw-   0        0        0      692 2023-11-11 11:28:42.000000 mypcremote-0.5.3/src/mypcremote/commands/status.py
+-rw-rw-rw-   0        0        0      440 2023-11-11 11:26:35.000000 mypcremote-0.5.3/src/mypcremote/commands/terminal.py
+-rw-rw-rw-   0        0        0      210 2023-11-13 08:33:07.000000 mypcremote-0.5.3/src/mypcremote/commands/terminate.py
+-rw-rw-rw-   0        0        0     1005 2023-11-12 14:31:11.000000 mypcremote-0.5.3/src/mypcremote/commands/upload.py
+-rw-rw-rw-   0        0        0     1081 2023-11-11 11:27:07.000000 mypcremote-0.5.3/src/mypcremote/commands/voicecall.py
+-rw-rw-rw-   0        0        0     1387 2023-11-12 13:56:04.000000 mypcremote-0.5.3/src/mypcremote/commands/volume.py
+drwxrwxrwx   0        0        0        0 2024-04-16 12:30:38.438792 mypcremote-0.5.3/src/mypcremote.egg-info/
+-rw-rw-rw-   0        0        0     3825 2024-04-16 12:30:38.000000 mypcremote-0.5.3/src/mypcremote.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1048 2024-04-16 12:30:38.000000 mypcremote-0.5.3/src/mypcremote.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 12:30:38.000000 mypcremote-0.5.3/src/mypcremote.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2024-04-16 12:30:38.000000 mypcremote-0.5.3/src/mypcremote.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      129 2024-04-16 12:30:38.000000 mypcremote-0.5.3/src/mypcremote.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-16 12:30:38.000000 mypcremote-0.5.3/src/mypcremote.egg-info/top_level.txt
```

### Comparing `mypcremote-0.5.2/LICENSE` & `mypcremote-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mypcremote-0.5.2/PKG-INFO` & `mypcremote-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mypcremote
-Version: 0.5.2
+Version: 0.5.3
 Summary: A good package to let your computer remote controlled using Discord
 Author-email: Zain Ul Abidin <zain26134@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/Zedstron/My-PC-Remote
 Project-URL: Issues, https://github.com/Zedstron/My-PC-Remote/issues
 Keywords: discord,remote,remote-pc,pccontrol,pc-remote,screen-sharing,remote-access,remote-control,pc-management,pc-administration,computer-access,computer-control
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mypcremote-0.5.2/README.md` & `mypcremote-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `mypcremote-0.5.2/pyproject.toml` & `mypcremote-0.5.3/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mypcremote"
-version = "0.5.2"
+version = "0.5.3"
 
 authors = [
   { name="Zain Ul Abidin", email="zain26134@gmail.com" }
 ]
 
 keywords = [
     "discord",
```

### Comparing `mypcremote-0.5.2/src/mypcremote/commands/camera.py` & `mypcremote-0.5.3/src/mypcremote/commands/camera.py`

 * *Files identical despite different names*

### Comparing `mypcremote-0.5.2/src/mypcremote/commands/clear.py` & `mypcremote-0.5.3/src/mypcremote/commands/clear.py`

 * *Files identical despite different names*

### Comparing `mypcremote-0.5.2/src/mypcremote/commands/hybernate.py` & `mypcremote-0.5.3/src/mypcremote/commands/hybernate.py`

 * *Files identical despite different names*

### Comparing `mypcremote-0.5.2/src/mypcremote/commands/kill.py` & `mypcremote-0.5.3/src/mypcremote/commands/kill.py`

 * *Files identical despite different names*

### Comparing `mypcremote-0.5.2/src/mypcremote/commands/location.py` & `mypcremote-0.5.3/src/mypcremote/commands/location.py`

 * *Files identical despite different names*

### Comparing `mypcremote-0.5.2/src/mypcremote/commands/lock.py` & `mypcremote-0.5.3/src/mypcremote/commands/lock.py`

 * *Files identical despite different names*

### Comparing `mypcremote-0.5.2/src/mypcremote/commands/notify.py` & `mypcremote-0.5.3/src/mypcremote/commands/notify.py`

 * *Files identical despite different names*

### Comparing `mypcremote-0.5.2/src/mypcremote/commands/openurl.py` & `mypcremote-0.5.3/src/mypcremote/commands/openurl.py`

 * *Files identical despite different names*

### Comparing `mypcremote-0.5.2/src/mypcremote/commands/reboot.py` & `mypcremote-0.5.3/src/mypcremote/commands/reboot.py`

 * *Files identical despite different names*

### Comparing `mypcremote-0.5.2/src/mypcremote/commands/shutdown.py` & `mypcremote-0.5.3/src/mypcremote/commands/shutdown.py`

 * *Files identical despite different names*

### Comparing `mypcremote-0.5.2/src/mypcremote/commands/sleep.py` & `mypcremote-0.5.3/src/mypcremote/commands/sleep.py`

 * *Files identical despite different names*

### Comparing `mypcremote-0.5.2/src/mypcremote/commands/speak.py` & `mypcremote-0.5.3/src/mypcremote/commands/speak.py`

 * *Files identical despite different names*

### Comparing `mypcremote-0.5.2/src/mypcremote/commands/status.py` & `mypcremote-0.5.3/src/mypcremote/commands/status.py`

 * *Files identical despite different names*

### Comparing `mypcremote-0.5.2/src/mypcremote/commands/upload.py` & `mypcremote-0.5.3/src/mypcremote/commands/upload.py`

 * *Files identical despite different names*

### Comparing `mypcremote-0.5.2/src/mypcremote/commands/voicecall.py` & `mypcremote-0.5.3/src/mypcremote/commands/voicecall.py`

 * *Files identical despite different names*

### Comparing `mypcremote-0.5.2/src/mypcremote/commands/volume.py` & `mypcremote-0.5.3/src/mypcremote/commands/volume.py`

 * *Files identical despite different names*

### Comparing `mypcremote-0.5.2/src/mypcremote.egg-info/PKG-INFO` & `mypcremote-0.5.3/src/mypcremote.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mypcremote
-Version: 0.5.2
+Version: 0.5.3
 Summary: A good package to let your computer remote controlled using Discord
 Author-email: Zain Ul Abidin <zain26134@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/Zedstron/My-PC-Remote
 Project-URL: Issues, https://github.com/Zedstron/My-PC-Remote/issues
 Keywords: discord,remote,remote-pc,pccontrol,pc-remote,screen-sharing,remote-access,remote-control,pc-management,pc-administration,computer-access,computer-control
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mypcremote-0.5.2/src/mypcremote.egg-info/SOURCES.txt` & `mypcremote-0.5.3/src/mypcremote.egg-info/SOURCES.txt`

 * *Files identical despite different names*

