# Comparing `tmp/vk_teams_async_bot-0.2.1.tar.gz` & `tmp/vk_teams_async_bot-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vk_teams_async_bot-0.2.1.tar", max compression
+gzip compressed data, was "vk_teams_async_bot-0.2.2.tar", max compression
```

## Comparing `vk_teams_async_bot-0.2.1.tar` & `vk_teams_async_bot-0.2.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1108 2023-12-28 10:42:15.574550 vk_teams_async_bot-0.2.1/LICENSE
--rw-r--r--   0        0        0     1241 2024-04-05 12:38:06.437147 vk_teams_async_bot-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     7032 2024-03-25 10:04:01.896611 vk_teams_async_bot-0.2.1/README.md
--rw-r--r--   0        0        0        0 2023-10-20 09:08:44.418623 vk_teams_async_bot-0.2.1/vk_teams_async_bot/__init__.py
--rw-r--r--   0        0        0    20547 2024-04-05 10:39:04.137243 vk_teams_async_bot-0.2.1/vk_teams_async_bot/bot.py
--rw-r--r--   0        0        0     4672 2024-04-05 11:45:45.756039 vk_teams_async_bot-0.2.1/vk_teams_async_bot/client_session.py
--rw-r--r--   0        0        0      848 2023-12-28 10:05:54.075146 vk_teams_async_bot-0.2.1/vk_teams_async_bot/constants.py
--rw-r--r--   0        0        0      700 2024-04-05 12:37:06.616281 vk_teams_async_bot-0.2.1/vk_teams_async_bot/dispatcher.py
--rw-r--r--   0        0        0       60 2024-03-25 13:41:10.135840 vk_teams_async_bot-0.2.1/vk_teams_async_bot/errors.py
--rw-r--r--   0        0        0     3200 2024-03-25 14:08:04.048523 vk_teams_async_bot-0.2.1/vk_teams_async_bot/events.py
--rw-r--r--   0        0        0     4763 2024-04-05 10:44:28.021696 vk_teams_async_bot-0.2.1/vk_teams_async_bot/filter.py
--rw-r--r--   0        0        0     2357 2024-03-25 13:41:10.159392 vk_teams_async_bot-0.2.1/vk_teams_async_bot/handler.py
--rw-r--r--   0        0        0     6086 2024-03-25 13:41:10.174905 vk_teams_async_bot-0.2.1/vk_teams_async_bot/helpers.py
--rw-r--r--   0        0        0      324 2024-03-25 14:12:50.638587 vk_teams_async_bot-0.2.1/vk_teams_async_bot/middleware.py
--rw-r--r--   0        0        0      260 2024-03-25 14:13:20.831674 vk_teams_async_bot-0.2.1/vk_teams_async_bot/schemas.py
--rw-r--r--   0        0        0     7060 2024-03-25 15:11:28.102016 vk_teams_async_bot-0.2.1/vk_teams_async_bot/state.py
--rw-r--r--   0        0        0      519 2023-12-21 14:07:29.369149 vk_teams_async_bot-0.2.1/vk_teams_async_bot/timer.py
--rw-r--r--   0        0        0     7476 1970-01-01 00:00:00.000000 vk_teams_async_bot-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1108 2023-12-28 10:42:15.574550 vk_teams_async_bot-0.2.2/LICENSE
+-rw-r--r--   0        0        0     1241 2024-04-16 10:20:00.658577 vk_teams_async_bot-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     7032 2024-03-25 10:04:01.896611 vk_teams_async_bot-0.2.2/README.md
+-rw-r--r--   0        0        0        0 2023-10-20 09:08:44.418623 vk_teams_async_bot-0.2.2/vk_teams_async_bot/__init__.py
+-rw-r--r--   0        0        0    20547 2024-04-16 10:16:48.278783 vk_teams_async_bot-0.2.2/vk_teams_async_bot/bot.py
+-rw-r--r--   0        0        0     4864 2024-04-16 10:16:38.504694 vk_teams_async_bot-0.2.2/vk_teams_async_bot/client_session.py
+-rw-r--r--   0        0        0      848 2023-12-28 10:05:54.075146 vk_teams_async_bot-0.2.2/vk_teams_async_bot/constants.py
+-rw-r--r--   0        0        0      700 2024-04-05 12:37:06.616281 vk_teams_async_bot-0.2.2/vk_teams_async_bot/dispatcher.py
+-rw-r--r--   0        0        0       60 2024-03-25 13:41:10.135840 vk_teams_async_bot-0.2.2/vk_teams_async_bot/errors.py
+-rw-r--r--   0        0        0     3200 2024-03-25 14:08:04.048523 vk_teams_async_bot-0.2.2/vk_teams_async_bot/events.py
+-rw-r--r--   0        0        0     4763 2024-04-05 10:44:28.021696 vk_teams_async_bot-0.2.2/vk_teams_async_bot/filter.py
+-rw-r--r--   0        0        0     2357 2024-03-25 13:41:10.159392 vk_teams_async_bot-0.2.2/vk_teams_async_bot/handler.py
+-rw-r--r--   0        0        0     6086 2024-03-25 13:41:10.174905 vk_teams_async_bot-0.2.2/vk_teams_async_bot/helpers.py
+-rw-r--r--   0        0        0      324 2024-03-25 14:12:50.638587 vk_teams_async_bot-0.2.2/vk_teams_async_bot/middleware.py
+-rw-r--r--   0        0        0      260 2024-03-25 14:13:20.831674 vk_teams_async_bot-0.2.2/vk_teams_async_bot/schemas.py
+-rw-r--r--   0        0        0     7060 2024-03-25 15:11:28.102016 vk_teams_async_bot-0.2.2/vk_teams_async_bot/state.py
+-rw-r--r--   0        0        0      519 2023-12-21 14:07:29.369149 vk_teams_async_bot-0.2.2/vk_teams_async_bot/timer.py
+-rw-r--r--   0        0        0     7476 1970-01-01 00:00:00.000000 vk_teams_async_bot-0.2.2/PKG-INFO
```

### Comparing `vk_teams_async_bot-0.2.1/LICENSE` & `vk_teams_async_bot-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vk_teams_async_bot-0.2.1/pyproject.toml` & `vk_teams_async_bot-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vk-teams-async-bot"
-version = "0.2.1"
+version = "0.2.2"
 description = ""
 authors = ["Александр Смирнов <alexsmi4444@gmail.com>"]
 readme = "README.md"
 packages = [{include = "vk_teams_async_bot"}]
 license = "MIT"
 repository = "https://github.com/Quakeer444/vk_teams_async_bot"
```

### Comparing `vk_teams_async_bot-0.2.1/README.md` & `vk_teams_async_bot-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `vk_teams_async_bot-0.2.1/vk_teams_async_bot/bot.py` & `vk_teams_async_bot-0.2.2/vk_teams_async_bot/bot.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,16 +28,16 @@
     """
 
     def __init__(
         self,
         bot_token: str,
         url: str = "https://api.internal.myteam.mail.ru",
         base_path="/bot/v1/",
-        timeout_session: Seconds = 25,
-        poll_time: Seconds = 20,
+        timeout_session: Seconds = 30,
+        poll_time: Seconds = 15,
         last_event_id: int = 0,
     ):
         """
 
         :param bot_token: Bot token
         :param url: Server Bot API
         :param base_path: Base path
```

### Comparing `vk_teams_async_bot-0.2.1/vk_teams_async_bot/client_session.py` & `vk_teams_async_bot-0.2.2/vk_teams_async_bot/client_session.py`

 * *Files 9% similar despite different names*

```diff
@@ -84,14 +84,17 @@
                     case _:
                         logger.info(f"{response.status} {response_json}")
 
                 return response_json
 
             return None
 
+        except asyncio.TimeoutError:
+            logger.error(f"Timeout error {endpoint=}")
+
         except aiohttp.ClientResponseError as err:
             if err.status >= 500:
                 raise ResponseStatus500orHigherError(err)
             logger.error(err)
             raise
 
         except Exception as err:
@@ -135,14 +138,17 @@
                     case _:
                         logger.info(f"{response.status} {response_json}")
 
                 return response_json
 
             return None
 
+        except asyncio.TimeoutError:
+            logger.error(f"Timeout error {endpoint=}")
+
         except aiohttp.ClientResponseError as err:
             if err.status >= 500:
                 raise ResponseStatus500orHigherError(err)
             logger.error(err)
             raise
 
         except Exception as err:
```

### Comparing `vk_teams_async_bot-0.2.1/vk_teams_async_bot/constants.py` & `vk_teams_async_bot-0.2.2/vk_teams_async_bot/constants.py`

 * *Files identical despite different names*

### Comparing `vk_teams_async_bot-0.2.1/vk_teams_async_bot/dispatcher.py` & `vk_teams_async_bot-0.2.2/vk_teams_async_bot/dispatcher.py`

 * *Files identical despite different names*

### Comparing `vk_teams_async_bot-0.2.1/vk_teams_async_bot/events.py` & `vk_teams_async_bot-0.2.2/vk_teams_async_bot/events.py`

 * *Files identical despite different names*

### Comparing `vk_teams_async_bot-0.2.1/vk_teams_async_bot/filter.py` & `vk_teams_async_bot-0.2.2/vk_teams_async_bot/filter.py`

 * *Files identical despite different names*

### Comparing `vk_teams_async_bot-0.2.1/vk_teams_async_bot/handler.py` & `vk_teams_async_bot-0.2.2/vk_teams_async_bot/handler.py`

 * *Files identical despite different names*

### Comparing `vk_teams_async_bot-0.2.1/vk_teams_async_bot/helpers.py` & `vk_teams_async_bot-0.2.2/vk_teams_async_bot/helpers.py`

 * *Files identical despite different names*

### Comparing `vk_teams_async_bot-0.2.1/vk_teams_async_bot/state.py` & `vk_teams_async_bot-0.2.2/vk_teams_async_bot/state.py`

 * *Files identical despite different names*

### Comparing `vk_teams_async_bot-0.2.1/vk_teams_async_bot/timer.py` & `vk_teams_async_bot-0.2.2/vk_teams_async_bot/timer.py`

 * *Files identical despite different names*

### Comparing `vk_teams_async_bot-0.2.1/PKG-INFO` & `vk_teams_async_bot-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vk-teams-async-bot
-Version: 0.2.1
+Version: 0.2.2
 Summary: 
 Home-page: https://github.com/Quakeer444/vk_teams_async_bot
 License: MIT
 Author: Александр Смирнов
 Author-email: alexsmi4444@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

