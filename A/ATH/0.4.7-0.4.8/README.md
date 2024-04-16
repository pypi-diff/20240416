# Comparing `tmp/ATH-0.4.7.tar.gz` & `tmp/ATH-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ATH-0.4.7.tar", last modified: Sat Mar 16 16:00:06 2024, max compression
+gzip compressed data, was "ATH-0.4.8.tar", last modified: Tue Apr 16 16:04:44 2024, max compression
```

## Comparing `ATH-0.4.7.tar` & `ATH-0.4.8.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-03-16 16:00:06.079580 ATH-0.4.7/
-drwxrwxrwx   0        0        0        0 2024-03-16 16:00:06.063289 ATH-0.4.7/ATH/
--rw-rw-rw-   0        0        0     1287 2024-03-03 12:52:16.000000 ATH-0.4.7/ATH/DB_read.py
--rw-rw-rw-   0        0        0      914 2024-03-02 12:38:15.000000 ATH-0.4.7/ATH/DB_send.py
--rw-rw-rw-   0        0        0      392 2024-03-16 15:58:03.000000 ATH-0.4.7/ATH/__init__.py
--rw-rw-rw-   0        0        0      172 2024-03-16 15:51:41.000000 ATH-0.4.7/ATH/abc123_2.py
--rw-rw-rw-   0        0        0      125 2024-03-01 17:00:39.000000 ATH-0.4.7/ATH/arithmetic_average.py
--rw-rw-rw-   0        0        0      528 2024-03-07 17:24:38.000000 ATH-0.4.7/ATH/calculator.py
--rw-rw-rw-   0        0        0      196 2024-03-05 13:23:48.000000 ATH-0.4.7/ATH/env.py
--rw-rw-rw-   0        0        0      368 2024-03-03 20:21:14.000000 ATH-0.4.7/ATH/get_current_time.py
--rw-rw-rw-   0        0        0       73 2024-02-29 15:44:39.000000 ATH-0.4.7/ATH/owl.py
--rw-rw-rw-   0        0        0      347 2024-03-07 15:18:29.000000 ATH-0.4.7/ATH/qr.py
--rw-rw-rw-   0        0        0      430 2024-02-29 15:58:56.000000 ATH-0.4.7/ATH/safe.py
--rw-rw-rw-   0        0        0      113 2024-02-28 18:40:56.000000 ATH-0.4.7/ATH/scr_shot.py
--rw-rw-rw-   0        0        0      312 2024-03-03 17:45:47.000000 ATH-0.4.7/ATH/scr_shot_telegram.py
--rw-rw-rw-   0        0        0       96 2024-02-29 13:36:04.000000 ATH-0.4.7/ATH/sq_root.py
--rw-rw-rw-   0        0        0     1115 2024-03-09 07:09:07.000000 ATH-0.4.7/ATH/tts.py
--rw-rw-rw-   0        0        0       58 2024-03-03 20:32:05.000000 ATH-0.4.7/ATH/wait.py
--rw-rw-rw-   0        0        0       78 2024-03-06 13:59:40.000000 ATH-0.4.7/ATH/write.py
-drwxrwxrwx   0        0        0        0 2024-03-16 16:00:06.076144 ATH-0.4.7/ATH.egg-info/
--rw-rw-rw-   0        0        0      460 2024-03-16 16:00:06.000000 ATH-0.4.7/ATH.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      408 2024-03-16 16:00:06.000000 ATH-0.4.7/ATH.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-16 16:00:06.000000 ATH-0.4.7/ATH.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      125 2024-03-16 16:00:06.000000 ATH-0.4.7/ATH.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-03-16 16:00:06.000000 ATH-0.4.7/ATH.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      460 2024-03-16 16:00:06.078575 ATH-0.4.7/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-03-16 16:00:06.080709 ATH-0.4.7/setup.cfg
--rw-rw-rw-   0        0        0      413 2024-03-16 15:59:50.000000 ATH-0.4.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 16:04:44.648032 ATH-0.4.8/
+drwxrwxrwx   0        0        0        0 2024-04-16 16:04:44.619516 ATH-0.4.8/ATH/
+-rw-rw-rw-   0        0        0     1287 2024-03-03 12:52:16.000000 ATH-0.4.8/ATH/DB_read.py
+-rw-rw-rw-   0        0        0      914 2024-03-02 12:38:15.000000 ATH-0.4.8/ATH/DB_send.py
+-rw-rw-rw-   0        0        0      417 2024-04-16 16:04:30.000000 ATH-0.4.8/ATH/__init__.py
+-rw-rw-rw-   0        0        0      172 2024-03-16 15:51:41.000000 ATH-0.4.8/ATH/abc123_2.py
+-rw-rw-rw-   0        0        0      125 2024-03-01 17:00:39.000000 ATH-0.4.8/ATH/arithmetic_average.py
+-rw-rw-rw-   0        0        0      528 2024-03-07 17:24:38.000000 ATH-0.4.8/ATH/calculator.py
+-rw-rw-rw-   0        0        0      196 2024-03-05 13:23:48.000000 ATH-0.4.8/ATH/env.py
+-rw-rw-rw-   0        0        0      368 2024-03-03 20:21:14.000000 ATH-0.4.8/ATH/get_current_time.py
+-rw-rw-rw-   0        0        0       73 2024-02-29 15:44:39.000000 ATH-0.4.8/ATH/owl.py
+-rw-rw-rw-   0        0        0      347 2024-03-07 15:18:29.000000 ATH-0.4.8/ATH/qr.py
+-rw-rw-rw-   0        0        0      430 2024-02-29 15:58:56.000000 ATH-0.4.8/ATH/safe.py
+-rw-rw-rw-   0        0        0      113 2024-02-28 18:40:56.000000 ATH-0.4.8/ATH/scr_shot.py
+-rw-rw-rw-   0        0        0      312 2024-03-03 17:45:47.000000 ATH-0.4.8/ATH/scr_shot_telegram.py
+-rw-rw-rw-   0        0        0       96 2024-02-29 13:36:04.000000 ATH-0.4.8/ATH/sq_root.py
+-rw-rw-rw-   0        0        0      167 2024-04-16 15:53:44.000000 ATH-0.4.8/ATH/telegram.py
+-rw-rw-rw-   0        0        0     1115 2024-03-09 07:09:07.000000 ATH-0.4.8/ATH/tts.py
+-rw-rw-rw-   0        0        0       58 2024-03-03 20:32:05.000000 ATH-0.4.8/ATH/wait.py
+-rw-rw-rw-   0        0        0       78 2024-03-06 13:59:40.000000 ATH-0.4.8/ATH/write.py
+drwxrwxrwx   0        0        0        0 2024-04-16 16:04:44.643306 ATH-0.4.8/ATH.egg-info/
+-rw-rw-rw-   0        0        0      460 2024-04-16 16:04:44.000000 ATH-0.4.8/ATH.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      424 2024-04-16 16:04:44.000000 ATH-0.4.8/ATH.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 16:04:44.000000 ATH-0.4.8/ATH.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      125 2024-04-16 16:04:44.000000 ATH-0.4.8/ATH.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-04-16 16:04:44.000000 ATH-0.4.8/ATH.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      460 2024-04-16 16:04:44.646142 ATH-0.4.8/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-16 16:04:44.649916 ATH-0.4.8/setup.cfg
+-rw-rw-rw-   0        0        0      413 2024-04-16 15:58:16.000000 ATH-0.4.8/setup.py
```

### Comparing `ATH-0.4.7/ATH/DB_read.py` & `ATH-0.4.8/ATH/DB_read.py`

 * *Files identical despite different names*

### Comparing `ATH-0.4.7/ATH/DB_send.py` & `ATH-0.4.8/ATH/DB_send.py`

 * *Files identical despite different names*

### Comparing `ATH-0.4.7/ATH/calculator.py` & `ATH-0.4.8/ATH/calculator.py`

 * *Files identical despite different names*

### Comparing `ATH-0.4.7/ATH/tts.py` & `ATH-0.4.8/ATH/tts.py`

 * *Files identical despite different names*

