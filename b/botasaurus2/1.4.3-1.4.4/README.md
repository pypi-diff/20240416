# Comparing `tmp/botasaurus2-1.4.3.tar.gz` & `tmp/botasaurus2-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botasaurus2-1.4.3.tar", max compression
+gzip compressed data, was "botasaurus2-1.4.4.tar", max compression
```

## Comparing `botasaurus2-1.4.3.tar` & `botasaurus2-1.4.4.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0      217 2024-03-15 22:38:58.098040 botasaurus2-1.4.3/AUTHORS
--rw-r--r--   0        0        0     1073 2024-03-15 22:38:58.098040 botasaurus2-1.4.3/LICENSE
--rw-r--r--   0        0        0    50976 2024-03-19 13:44:59.662333 botasaurus2-1.4.3/README.md
--rw-r--r--   0        0        0      854 2024-04-15 19:45:21.210506 botasaurus2-1.4.3/botasaurus/__init__.py
--rw-r--r--   0        0        0      211 2024-03-15 22:38:58.098040 botasaurus2-1.4.3/botasaurus/_id.py
--rw-r--r--   0        0        0     1034 2024-03-15 22:38:58.098040 botasaurus2-1.4.3/botasaurus/accept_google_cookies.py
--rw-r--r--   0        0        0    57750 2024-04-15 18:54:34.470840 botasaurus2-1.4.3/botasaurus/anti_detect_driver.py
--rw-r--r--   0        0        0     4485 2024-04-11 15:00:22.756112 botasaurus2-1.4.3/botasaurus/anti_detect_requests.py
--rw-r--r--   0        0        0     3549 2024-03-15 22:38:58.098040 botasaurus2-1.4.3/botasaurus/base_data.py
--rw-r--r--   0        0        0      800 2024-03-15 22:38:58.098040 botasaurus2-1.4.3/botasaurus/beep_utils.py
--rw-r--r--   0        0        0     2868 2024-04-12 14:30:05.866696 botasaurus2-1.4.3/botasaurus/botasaurus_storage.py
--rw-r--r--   0        0        0      944 2024-04-11 21:17:56.332972 botasaurus2-1.4.3/botasaurus/bt.py
--rw-r--r--   0        0        0     7486 2024-03-15 22:38:58.098040 botasaurus2-1.4.3/botasaurus/cache.py
--rw-r--r--   0        0        0     2114 2024-03-15 22:38:58.098040 botasaurus2-1.4.3/botasaurus/calc_max_parallel_browsers.py
--rw-r--r--   0        0        0    28154 2024-04-11 15:00:22.756112 botasaurus2-1.4.3/botasaurus/captcha.py
--rw-r--r--   0        0        0      566 2024-03-15 22:38:58.098040 botasaurus2-1.4.3/botasaurus/check_and_download_driver.py
--rw-r--r--   0        0        0      362 2024-03-15 22:38:58.098040 botasaurus2-1.4.3/botasaurus/chrome_launcher_adapter.py
--rw-r--r--   0        0        0    14871 2024-03-15 22:38:58.098040 botasaurus2-1.4.3/botasaurus/cl.py
--rw-r--r--   0        0        0      946 2024-03-15 22:38:58.098040 botasaurus2-1.4.3/botasaurus/close.py
--rw-r--r--   0        0        0      256 2024-03-20 15:48:31.573396 botasaurus2-1.4.3/botasaurus/constants.py
--rw-r--r--   0        0        0    15804 2024-04-16 18:43:06.058466 botasaurus2-1.4.3/botasaurus/create_driver_utils.py
--rw-r--r--   0        0        0    12609 2024-04-15 20:12:50.183439 botasaurus2-1.4.3/botasaurus/create_stealth_driver.py
--rw-r--r--   0        0        0     1820 2024-03-15 22:38:58.102041 botasaurus2-1.4.3/botasaurus/creators.py
--rw-r--r--   0        0        0     4130 2024-03-15 22:38:58.102041 botasaurus2-1.4.3/botasaurus/decorator_helpers.py
--rw-r--r--   0        0        0    39385 2024-04-15 21:45:09.835191 botasaurus2-1.4.3/botasaurus/decorators.py
--rw-r--r--   0        0        0      491 2024-03-15 22:38:58.102041 botasaurus2-1.4.3/botasaurus/decorators_utils.py
--rw-r--r--   0        0        0     1617 2024-03-15 22:38:58.102041 botasaurus2-1.4.3/botasaurus/download_driver.py
--rw-r--r--   0        0        0      459 2024-03-15 22:38:58.102041 botasaurus2-1.4.3/botasaurus/driver_about.py
--rw-r--r--   0        0        0       48 2024-03-15 22:38:58.102041 botasaurus2-1.4.3/botasaurus/exceptions.py
--rw-r--r--   0        0        0       84 2024-03-15 22:38:58.102041 botasaurus2-1.4.3/botasaurus/formats.py
--rw-r--r--   0        0        0    14839 2024-03-15 22:38:58.102041 botasaurus2-1.4.3/botasaurus/get_chrome_version.py
--rw-r--r--   0        0        0     8679 2024-04-11 15:00:22.756112 botasaurus2-1.4.3/botasaurus/got_adapter.py
--rw-r--r--   0        0        0     2438 2024-04-12 14:30:10.786777 botasaurus2-1.4.3/botasaurus/ip_utils.py
--rw-r--r--   0        0        0     1534 2024-03-15 22:38:58.102041 botasaurus2-1.4.3/botasaurus/list_utils.py
--rw-r--r--   0        0        0     3326 2024-04-11 20:48:02.911490 botasaurus2-1.4.3/botasaurus/local_storage.py
--rw-r--r--   0        0        0     1674 2024-03-15 22:38:58.102041 botasaurus2-1.4.3/botasaurus/local_storage_driver.py
--rw-r--r--   0        0        0       77 2024-03-15 22:38:58.102041 botasaurus2-1.4.3/botasaurus/opponent.py
--rw-r--r--   0        0        0     7343 2024-03-19 13:44:59.666333 botasaurus2-1.4.3/botasaurus/output.py
--rw-r--r--   0        0        0     4964 2024-04-12 14:01:33.922678 botasaurus2-1.4.3/botasaurus/profile.py
--rw-r--r--   0        0        0      352 2024-03-19 19:06:20.087339 botasaurus2-1.4.3/botasaurus/shortcuts.py
--rw-r--r--   0        0        0    22453 2024-03-15 22:38:58.102041 botasaurus2-1.4.3/botasaurus/sitemap.py
--rw-r--r--   0        0        0     2031 2024-03-19 13:44:59.666333 botasaurus2-1.4.3/botasaurus/str_utils.py
--rw-r--r--   0        0        0     6298 2024-03-15 22:38:58.102041 botasaurus2-1.4.3/botasaurus/temp_mail.py
--rw-r--r--   0        0        0       54 2024-03-15 22:38:58.102041 botasaurus2-1.4.3/botasaurus/usage.py
--rw-r--r--   0        0        0     7457 2024-03-15 22:38:58.102041 botasaurus2-1.4.3/botasaurus/user_agent.py
--rw-r--r--   0        0        0     4194 2024-03-15 22:38:58.102041 botasaurus2-1.4.3/botasaurus/user_generator.py
--rw-r--r--   0        0        0     8611 2024-04-15 14:50:43.118678 botasaurus2-1.4.3/botasaurus/utils.py
--rw-r--r--   0        0        0       57 2024-03-15 22:38:58.102041 botasaurus2-1.4.3/botasaurus/wait.py
--rw-r--r--   0        0        0     1183 2024-03-15 22:38:58.102041 botasaurus2-1.4.3/botasaurus/window_size.py
--rw-r--r--   0        0        0      848 2024-04-16 18:51:54.374735 botasaurus2-1.4.3/pyproject.toml
--rw-r--r--   0        0        0    52119 1970-01-01 00:00:00.000000 botasaurus2-1.4.3/PKG-INFO
+-rw-r--r--   0        0        0      217 2024-03-15 22:38:58.098040 botasaurus2-1.4.4/AUTHORS
+-rw-r--r--   0        0        0     1073 2024-03-15 22:38:58.098040 botasaurus2-1.4.4/LICENSE
+-rw-r--r--   0        0        0    50976 2024-03-19 13:44:59.662333 botasaurus2-1.4.4/README.md
+-rw-r--r--   0        0        0      854 2024-04-15 19:45:21.210506 botasaurus2-1.4.4/botasaurus/__init__.py
+-rw-r--r--   0        0        0      211 2024-03-15 22:38:58.098040 botasaurus2-1.4.4/botasaurus/_id.py
+-rw-r--r--   0        0        0     1034 2024-03-15 22:38:58.098040 botasaurus2-1.4.4/botasaurus/accept_google_cookies.py
+-rw-r--r--   0        0        0    57750 2024-04-15 18:54:34.470840 botasaurus2-1.4.4/botasaurus/anti_detect_driver.py
+-rw-r--r--   0        0        0     4485 2024-04-11 15:00:22.756112 botasaurus2-1.4.4/botasaurus/anti_detect_requests.py
+-rw-r--r--   0        0        0     3549 2024-03-15 22:38:58.098040 botasaurus2-1.4.4/botasaurus/base_data.py
+-rw-r--r--   0        0        0      800 2024-03-15 22:38:58.098040 botasaurus2-1.4.4/botasaurus/beep_utils.py
+-rw-r--r--   0        0        0     2868 2024-04-12 14:30:05.866696 botasaurus2-1.4.4/botasaurus/botasaurus_storage.py
+-rw-r--r--   0        0        0      944 2024-04-11 21:17:56.332972 botasaurus2-1.4.4/botasaurus/bt.py
+-rw-r--r--   0        0        0     7486 2024-03-15 22:38:58.098040 botasaurus2-1.4.4/botasaurus/cache.py
+-rw-r--r--   0        0        0     2114 2024-03-15 22:38:58.098040 botasaurus2-1.4.4/botasaurus/calc_max_parallel_browsers.py
+-rw-r--r--   0        0        0    28154 2024-04-11 15:00:22.756112 botasaurus2-1.4.4/botasaurus/captcha.py
+-rw-r--r--   0        0        0      566 2024-03-15 22:38:58.098040 botasaurus2-1.4.4/botasaurus/check_and_download_driver.py
+-rw-r--r--   0        0        0      362 2024-03-15 22:38:58.098040 botasaurus2-1.4.4/botasaurus/chrome_launcher_adapter.py
+-rw-r--r--   0        0        0    14871 2024-03-15 22:38:58.098040 botasaurus2-1.4.4/botasaurus/cl.py
+-rw-r--r--   0        0        0      946 2024-03-15 22:38:58.098040 botasaurus2-1.4.4/botasaurus/close.py
+-rw-r--r--   0        0        0      256 2024-03-20 15:48:31.573396 botasaurus2-1.4.4/botasaurus/constants.py
+-rw-r--r--   0        0        0    15794 2024-04-16 19:24:46.153005 botasaurus2-1.4.4/botasaurus/create_driver_utils.py
+-rw-r--r--   0        0        0    12609 2024-04-15 20:12:50.183439 botasaurus2-1.4.4/botasaurus/create_stealth_driver.py
+-rw-r--r--   0        0        0     1820 2024-03-15 22:38:58.102041 botasaurus2-1.4.4/botasaurus/creators.py
+-rw-r--r--   0        0        0     4130 2024-03-15 22:38:58.102041 botasaurus2-1.4.4/botasaurus/decorator_helpers.py
+-rw-r--r--   0        0        0    39385 2024-04-15 21:45:09.835191 botasaurus2-1.4.4/botasaurus/decorators.py
+-rw-r--r--   0        0        0      491 2024-03-15 22:38:58.102041 botasaurus2-1.4.4/botasaurus/decorators_utils.py
+-rw-r--r--   0        0        0     1617 2024-03-15 22:38:58.102041 botasaurus2-1.4.4/botasaurus/download_driver.py
+-rw-r--r--   0        0        0      459 2024-03-15 22:38:58.102041 botasaurus2-1.4.4/botasaurus/driver_about.py
+-rw-r--r--   0        0        0       48 2024-03-15 22:38:58.102041 botasaurus2-1.4.4/botasaurus/exceptions.py
+-rw-r--r--   0        0        0       84 2024-03-15 22:38:58.102041 botasaurus2-1.4.4/botasaurus/formats.py
+-rw-r--r--   0        0        0    14839 2024-03-15 22:38:58.102041 botasaurus2-1.4.4/botasaurus/get_chrome_version.py
+-rw-r--r--   0        0        0     8679 2024-04-11 15:00:22.756112 botasaurus2-1.4.4/botasaurus/got_adapter.py
+-rw-r--r--   0        0        0     2438 2024-04-12 14:30:10.786777 botasaurus2-1.4.4/botasaurus/ip_utils.py
+-rw-r--r--   0        0        0     1534 2024-03-15 22:38:58.102041 botasaurus2-1.4.4/botasaurus/list_utils.py
+-rw-r--r--   0        0        0     3326 2024-04-11 20:48:02.911490 botasaurus2-1.4.4/botasaurus/local_storage.py
+-rw-r--r--   0        0        0     1674 2024-03-15 22:38:58.102041 botasaurus2-1.4.4/botasaurus/local_storage_driver.py
+-rw-r--r--   0        0        0       77 2024-03-15 22:38:58.102041 botasaurus2-1.4.4/botasaurus/opponent.py
+-rw-r--r--   0        0        0     7343 2024-03-19 13:44:59.666333 botasaurus2-1.4.4/botasaurus/output.py
+-rw-r--r--   0        0        0     4964 2024-04-12 14:01:33.922678 botasaurus2-1.4.4/botasaurus/profile.py
+-rw-r--r--   0        0        0      352 2024-03-19 19:06:20.087339 botasaurus2-1.4.4/botasaurus/shortcuts.py
+-rw-r--r--   0        0        0    22453 2024-03-15 22:38:58.102041 botasaurus2-1.4.4/botasaurus/sitemap.py
+-rw-r--r--   0        0        0     2031 2024-03-19 13:44:59.666333 botasaurus2-1.4.4/botasaurus/str_utils.py
+-rw-r--r--   0        0        0     6298 2024-03-15 22:38:58.102041 botasaurus2-1.4.4/botasaurus/temp_mail.py
+-rw-r--r--   0        0        0       54 2024-03-15 22:38:58.102041 botasaurus2-1.4.4/botasaurus/usage.py
+-rw-r--r--   0        0        0     7457 2024-03-15 22:38:58.102041 botasaurus2-1.4.4/botasaurus/user_agent.py
+-rw-r--r--   0        0        0     4194 2024-03-15 22:38:58.102041 botasaurus2-1.4.4/botasaurus/user_generator.py
+-rw-r--r--   0        0        0     8611 2024-04-15 14:50:43.118678 botasaurus2-1.4.4/botasaurus/utils.py
+-rw-r--r--   0        0        0       57 2024-03-15 22:38:58.102041 botasaurus2-1.4.4/botasaurus/wait.py
+-rw-r--r--   0        0        0     1183 2024-03-15 22:38:58.102041 botasaurus2-1.4.4/botasaurus/window_size.py
+-rw-r--r--   0        0        0      848 2024-04-16 19:26:03.167945 botasaurus2-1.4.4/pyproject.toml
+-rw-r--r--   0        0        0    52119 1970-01-01 00:00:00.000000 botasaurus2-1.4.4/PKG-INFO
```

### Comparing `botasaurus2-1.4.3/LICENSE` & `botasaurus2-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.3/README.md` & `botasaurus2-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.3/botasaurus/__init__.py` & `botasaurus2-1.4.4/botasaurus/__init__.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.3/botasaurus/accept_google_cookies.py` & `botasaurus2-1.4.4/botasaurus/accept_google_cookies.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.3/botasaurus/anti_detect_driver.py` & `botasaurus2-1.4.4/botasaurus/anti_detect_driver.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.3/botasaurus/anti_detect_requests.py` & `botasaurus2-1.4.4/botasaurus/anti_detect_requests.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.3/botasaurus/base_data.py` & `botasaurus2-1.4.4/botasaurus/base_data.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.3/botasaurus/beep_utils.py` & `botasaurus2-1.4.4/botasaurus/beep_utils.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.3/botasaurus/botasaurus_storage.py` & `botasaurus2-1.4.4/botasaurus/botasaurus_storage.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.3/botasaurus/bt.py` & `botasaurus2-1.4.4/botasaurus/bt.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.3/botasaurus/cache.py` & `botasaurus2-1.4.4/botasaurus/cache.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.3/botasaurus/calc_max_parallel_browsers.py` & `botasaurus2-1.4.4/botasaurus/calc_max_parallel_browsers.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.3/botasaurus/captcha.py` & `botasaurus2-1.4.4/botasaurus/captcha.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.3/botasaurus/check_and_download_driver.py` & `botasaurus2-1.4.4/botasaurus/check_and_download_driver.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.3/botasaurus/cl.py` & `botasaurus2-1.4.4/botasaurus/cl.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.3/botasaurus/close.py` & `botasaurus2-1.4.4/botasaurus/close.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.3/botasaurus/create_driver_utils.py` & `botasaurus2-1.4.4/botasaurus/create_driver_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 def add_useragent(options, user_agent):
     if user_agent:
         options.add_argument(f'--user-agent={user_agent}')
 
 
 def create_profile_path(user_id, base_dir='.'):
     PROFILES_PATH = 'profiles'
-    path = Path(base_dir) / f'{PROFILES_PATH}/{user_id}'
+    path = Path(base_dir) / f'{PROFILES_PATH}'
     # path = relative_path(path, 0)
     return path
 
 
 def delete_corrupted_files(user_id):
     is_success = silentremove(
         f'{create_profile_path(user_id)}/SingletonCookie')
```

### Comparing `botasaurus2-1.4.3/botasaurus/create_stealth_driver.py` & `botasaurus2-1.4.4/botasaurus/create_stealth_driver.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.3/botasaurus/creators.py` & `botasaurus2-1.4.4/botasaurus/creators.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.3/botasaurus/decorator_helpers.py` & `botasaurus2-1.4.4/botasaurus/decorator_helpers.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.3/botasaurus/decorators.py` & `botasaurus2-1.4.4/botasaurus/decorators.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.3/botasaurus/download_driver.py` & `botasaurus2-1.4.4/botasaurus/download_driver.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.3/botasaurus/get_chrome_version.py` & `botasaurus2-1.4.4/botasaurus/get_chrome_version.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.3/botasaurus/got_adapter.py` & `botasaurus2-1.4.4/botasaurus/got_adapter.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.3/botasaurus/ip_utils.py` & `botasaurus2-1.4.4/botasaurus/ip_utils.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.3/botasaurus/list_utils.py` & `botasaurus2-1.4.4/botasaurus/list_utils.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.3/botasaurus/local_storage.py` & `botasaurus2-1.4.4/botasaurus/local_storage.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.3/botasaurus/local_storage_driver.py` & `botasaurus2-1.4.4/botasaurus/local_storage_driver.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.3/botasaurus/output.py` & `botasaurus2-1.4.4/botasaurus/output.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.3/botasaurus/profile.py` & `botasaurus2-1.4.4/botasaurus/profile.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.3/botasaurus/sitemap.py` & `botasaurus2-1.4.4/botasaurus/sitemap.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.3/botasaurus/str_utils.py` & `botasaurus2-1.4.4/botasaurus/str_utils.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.3/botasaurus/temp_mail.py` & `botasaurus2-1.4.4/botasaurus/temp_mail.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.3/botasaurus/user_agent.py` & `botasaurus2-1.4.4/botasaurus/user_agent.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.3/botasaurus/user_generator.py` & `botasaurus2-1.4.4/botasaurus/user_generator.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.3/botasaurus/utils.py` & `botasaurus2-1.4.4/botasaurus/utils.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.3/botasaurus/window_size.py` & `botasaurus2-1.4.4/botasaurus/window_size.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.3/pyproject.toml` & `botasaurus2-1.4.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "botasaurus2"
-version = "1.4.3"
+version = "1.4.4"
 description = "Patching fork of botasaurus, The All in One Framework to build Awesome Scrapers."
 authors = ["Chetan Jain <chetan@omkar.cloud>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "botasaurus", from = "."}]
 
 [tool.poetry.dependencies]
```

### Comparing `botasaurus2-1.4.3/PKG-INFO` & `botasaurus2-1.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botasaurus2
-Version: 1.4.3
+Version: 1.4.4
 Summary: Patching fork of botasaurus, The All in One Framework to build Awesome Scrapers.
 License: MIT
 Author: Chetan Jain
 Author-email: chetan@omkar.cloud
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: botasaurus2 Version: 1.4.3 Summary: Patching fork
+Metadata-Version: 2.1 Name: botasaurus2 Version: 1.4.4 Summary: Patching fork
 of botasaurus, The All in One Framework to build Awesome Scrapers. License: MIT
 Author: Chetan Jain Author-email: chetan@omkar.cloud Requires-Python:
 >=3.10,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Requires-Dist: aigents (>=0.5.0,<0.6.0)
 Requires-Dist: beautifulsoup4 (>=4.11.2,<5.0.0) Requires-Dist: botasaurus-
```

