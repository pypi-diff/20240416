# Comparing `tmp/scratchattach-1.6.2.tar.gz` & `tmp/scratchattach-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scratchattach-1.6.2.tar", last modified: Tue Feb 27 20:09:06 2024, max compression
+gzip compressed data, was "scratchattach-1.6.3.tar", last modified: Tue Apr 16 18:52:02 2024, max compression
```

## Comparing `scratchattach-1.6.2.tar` & `scratchattach-1.6.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-02-27 20:09:06.332418 scratchattach-1.6.2/
--rw-rw-rw-   0        0        0     1101 2024-02-27 18:22:17.000000 scratchattach-1.6.2/LICENSE
--rw-rw-rw-   0        0        0     4019 2024-02-27 20:09:06.331421 scratchattach-1.6.2/PKG-INFO
--rw-rw-rw-   0        0        0     3309 2024-02-27 18:22:17.000000 scratchattach-1.6.2/README.md
-drwxrwxrwx   0        0        0        0 2024-02-27 20:09:06.300781 scratchattach-1.6.2/scratchattach/
--rw-rw-rw-   0        0        0     2797 2024-02-27 18:22:18.000000 scratchattach-1.6.2/scratchattach/__init__.py
--rw-rw-rw-   0        0        0    20732 2024-02-27 19:23:30.000000 scratchattach-1.6.2/scratchattach/cloud.py
--rw-rw-rw-   0        0        0    24801 2024-02-27 19:21:10.000000 scratchattach-1.6.2/scratchattach/cloud_requests.py
--rw-rw-rw-   0        0        0     2600 2024-02-27 19:12:10.000000 scratchattach-1.6.2/scratchattach/encoder.py
--rw-rw-rw-   0        0        0     4221 2024-02-27 18:22:18.000000 scratchattach-1.6.2/scratchattach/exceptions.py
--rw-rw-rw-   0        0        0    10508 2024-02-27 18:22:18.000000 scratchattach-1.6.2/scratchattach/forum.py
--rw-rw-rw-   0        0        0    30624 2024-02-27 19:52:42.000000 scratchattach-1.6.2/scratchattach/project.py
--rw-rw-rw-   0        0        0    22550 2024-02-27 19:23:35.000000 scratchattach-1.6.2/scratchattach/session.py
--rw-rw-rw-   0        0        0    20487 2024-02-27 18:51:45.000000 scratchattach-1.6.2/scratchattach/studio.py
--rw-rw-rw-   0        0        0    34892 2024-02-27 18:49:16.000000 scratchattach-1.6.2/scratchattach/user.py
-drwxrwxrwx   0        0        0        0 2024-02-27 20:09:06.321410 scratchattach-1.6.2/scratchattach.egg-info/
--rw-rw-rw-   0        0        0     4019 2024-02-27 20:09:05.000000 scratchattach-1.6.2/scratchattach.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      463 2024-02-27 20:09:06.000000 scratchattach-1.6.2/scratchattach.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-27 20:09:05.000000 scratchattach-1.6.2/scratchattach.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2024-02-27 20:09:05.000000 scratchattach-1.6.2/scratchattach.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-02-27 20:09:05.000000 scratchattach-1.6.2/scratchattach.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-27 20:09:06.332418 scratchattach-1.6.2/setup.cfg
--rw-rw-rw-   0        0        0     1085 2024-02-27 20:08:43.000000 scratchattach-1.6.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 18:52:02.650414 scratchattach-1.6.3/
+-rw-rw-rw-   0        0        0     1101 2023-09-02 14:18:05.000000 scratchattach-1.6.3/LICENSE
+-rw-rw-rw-   0        0        0     4042 2024-04-16 18:52:02.649406 scratchattach-1.6.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3309 2023-09-04 01:43:11.000000 scratchattach-1.6.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-16 18:52:02.633878 scratchattach-1.6.3/scratchattach/
+-rw-rw-rw-   0        0        0     2719 2023-09-16 14:17:22.000000 scratchattach-1.6.3/scratchattach/__init__.py
+-rw-rw-rw-   0        0        0    20823 2024-04-16 18:51:10.000000 scratchattach-1.6.3/scratchattach/cloud.py
+-rw-rw-rw-   0        0        0    24874 2024-04-16 18:08:07.000000 scratchattach-1.6.3/scratchattach/cloud_requests.py
+-rw-rw-rw-   0        0        0     2600 2024-04-16 18:08:07.000000 scratchattach-1.6.3/scratchattach/encoder.py
+-rw-rw-rw-   0        0        0     4221 2023-10-25 12:34:35.000000 scratchattach-1.6.3/scratchattach/exceptions.py
+-rw-rw-rw-   0        0        0    10508 2023-09-04 01:29:36.000000 scratchattach-1.6.3/scratchattach/forum.py
+-rw-rw-rw-   0        0        0    31197 2024-04-16 18:33:18.000000 scratchattach-1.6.3/scratchattach/project.py
+-rw-rw-rw-   0        0        0    22000 2023-09-30 18:44:30.000000 scratchattach-1.6.3/scratchattach/session.py
+-rw-rw-rw-   0        0        0    20487 2024-04-16 18:08:07.000000 scratchattach-1.6.3/scratchattach/studio.py
+-rw-rw-rw-   0        0        0    34892 2023-11-24 17:38:57.000000 scratchattach-1.6.3/scratchattach/user.py
+drwxrwxrwx   0        0        0        0 2024-04-16 18:52:02.649406 scratchattach-1.6.3/scratchattach.egg-info/
+-rw-rw-rw-   0        0        0     4042 2024-04-16 18:52:02.000000 scratchattach-1.6.3/scratchattach.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      463 2024-04-16 18:52:02.000000 scratchattach-1.6.3/scratchattach.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 18:52:02.000000 scratchattach-1.6.3/scratchattach.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2024-04-16 18:52:02.000000 scratchattach-1.6.3/scratchattach.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-16 18:52:02.000000 scratchattach-1.6.3/scratchattach.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-16 18:52:02.650414 scratchattach-1.6.3/setup.cfg
+-rw-rw-rw-   0        0        0     1108 2024-04-16 18:50:58.000000 scratchattach-1.6.3/setup.py
```

### Comparing `scratchattach-1.6.2/LICENSE` & `scratchattach-1.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `scratchattach-1.6.2/PKG-INFO` & `scratchattach-1.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: scratchattach
-Version: 1.6.2
-Summary: An Scratch API Wrapper for scratch.mit.edu
+Version: 1.6.3
+Summary: An Scratch API Wrapper for scra tch.mit.edu
 Home-page: https://github.com/TimMcCool/scratchattach
 Author: TimMcCool
-Author-email: 
+Author-email: timkrome2006@gmail.com
 Keywords: scratch api,scratchattach,scratch api python,scratch python,scratch for python,scratch,scratch cloud,scratch cloud variables,scratch bot
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `scratchattach-1.6.2/README.md` & `scratchattach-1.6.3/README.md`

 * *Files identical despite different names*

### Comparing `scratchattach-1.6.2/scratchattach/__init__.py` & `scratchattach-1.6.3/scratchattach/__init__.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,78 +1,78 @@
-from .cloud import *
-from .user import *
-from .session import *
-from .project import *
-from .studio import *
-from .cloud_requests import *
-from .forum import *
-from .encoder import *
-
-def get_news(*, limit=10, offset=0):
-    return requests.get(f"https://api.scratch.mit.edu/news?limit={limit}&offset={offset}").json()
-
-def featured_projects():
-    return requests.get("https://api.scratch.mit.edu/proxy/featured").json()["community_featured_projects"]
-
-def featured_studios():
-    return requests.get("https://api.scratch.mit.edu/proxy/featured").json()["community_featured_studios"]
-
-def top_loved():
-    return requests.get("https://api.scratch.mit.edu/proxy/featured").json()["community_most_loved_projects"]
-
-def top_remixed():
-    return requests.get("https://api.scratch.mit.edu/proxy/featured").json()["community_most_remixed_projects"]
-
-def newest_projects():
-    return requests.get("https://api.scratch.mit.edu/proxy/featured").json()["community_newest_projects"]
-
-def curated_projects():
-    return requests.get("https://api.scratch.mit.edu/proxy/featured").json()["curator_top_projects"]
-
-def design_studio_projects():
-    return requests.get("https://api.scratch.mit.edu/proxy/featured").json()["scratch_design_studio"]
-
-def search_posts(*, query, order="newest", page=0):
-    try:
-        data = requests.get(f"https://scratchdb.lefty.one/v3/forum/search?q={query}&o={order}&page={page}").json()["posts"]
-        return_data = []
-        for o in data:
-            a = forum.ForumPost(id = o["id"])
-            a._update_from_dict(o)
-            return_data.append(a)
-        return return_data
-    except Exception:
-        return []
-
-def total_site_stats():
-    data = requests.get("https://scratch.mit.edu/statistics/data/daily/").json()
-    data.pop("_TS")
-    return data
-
-def monthly_site_traffic():
-    data = requests.get("https://scratch.mit.edu/statistics/data/monthly-ga/").json()
-    data.pop("_TS")
-    return data
-
-def country_counts():
-    return requests.get("https://scratch.mit.edu/statistics/data/monthly/").json()["country_distribution"]
-
-def age_distribution():
-    data = requests.get("https://scratch.mit.edu/statistics/data/monthly/").json()["age_distribution_data"][0]["values"]
-    return_data = {}
-    for value in data:
-        return_data[value["x"]] = value["y"]
-    return return_data
-
-def get_health():
-    return requests.get("https://api.scratch.mit.edu/health").json()
-
-def get_csrf_token():
-    """
-    Generates a scratchcsrftoken using Scratch's API.
-
-    Returns:
-        str: The generated scratchcsrftoken
-    """
-    return requests.get(
-        "https://scratch.mit.edu/csrf_token/"
-    ).headers["set-cookie"].split(";")[3][len(" Path=/, scratchcsrftoken="):]
+from .cloud import *
+from .user import *
+from .session import *
+from .project import *
+from .studio import *
+from .cloud_requests import *
+from .forum import *
+from .encoder import *
+
+def get_news(*, limit=10, offset=0):
+    return requests.get(f"https://api.scratch.mit.edu/news?limit={limit}&offset={offset}").json()
+
+def featured_projects():
+    return requests.get("https://api.scratch.mit.edu/proxy/featured").json()["community_featured_projects"]
+
+def featured_studios():
+    return requests.get("https://api.scratch.mit.edu/proxy/featured").json()["community_featured_studios"]
+
+def top_loved():
+    return requests.get("https://api.scratch.mit.edu/proxy/featured").json()["community_most_loved_projects"]
+
+def top_remixed():
+    return requests.get("https://api.scratch.mit.edu/proxy/featured").json()["community_most_remixed_projects"]
+
+def newest_projects():
+    return requests.get("https://api.scratch.mit.edu/proxy/featured").json()["community_newest_projects"]
+
+def curated_projects():
+    return requests.get("https://api.scratch.mit.edu/proxy/featured").json()["curator_top_projects"]
+
+def design_studio_projects():
+    return requests.get("https://api.scratch.mit.edu/proxy/featured").json()["scratch_design_studio"]
+
+def search_posts(*, query, order="newest", page=0):
+    try:
+        data = requests.get(f"https://scratchdb.lefty.one/v3/forum/search?q={query}&o={order}&page={page}").json()["posts"]
+        return_data = []
+        for o in data:
+            a = forum.ForumPost(id = o["id"])
+            a._update_from_dict(o)
+            return_data.append(a)
+        return return_data
+    except Exception:
+        return []
+
+def total_site_stats():
+    data = requests.get("https://scratch.mit.edu/statistics/data/daily/").json()
+    data.pop("_TS")
+    return data
+
+def monthly_site_traffic():
+    data = requests.get("https://scratch.mit.edu/statistics/data/monthly-ga/").json()
+    data.pop("_TS")
+    return data
+
+def country_counts():
+    return requests.get("https://scratch.mit.edu/statistics/data/monthly/").json()["country_distribution"]
+
+def age_distribution():
+    data = requests.get("https://scratch.mit.edu/statistics/data/monthly/").json()["age_distribution_data"][0]["values"]
+    return_data = {}
+    for value in data:
+        return_data[value["x"]] = value["y"]
+    return return_data
+
+def get_health():
+    return requests.get("https://api.scratch.mit.edu/health").json()
+
+def get_csrf_token():
+    """
+    Generates a scratchcsrftoken using Scratch's API.
+
+    Returns:
+        str: The generated scratchcsrftoken
+    """
+    return requests.get(
+        "https://scratch.mit.edu/csrf_token/"
+    ).headers["set-cookie"].split(";")[3][len(" Path=/, scratchcsrftoken="):]
```

### Comparing `scratchattach-1.6.2/scratchattach/cloud.py` & `scratchattach-1.6.3/scratchattach/cloud.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,15 @@
         if not (value in [True, False, float('inf'), -float('inf')]):
             value = str(value)
             if len(value) > 256:
                 warnings.warn("invalid cloud var (too long): "+str(value), Warning)
                 raise(exceptions.InvalidCloudValue)
             x = value.replace(".", "")
             x = x.replace("-", "")
-            if not x.isnumeric():
+            if not (x.isnumeric() or x == ""):
                 warnings.warn("invalid cloud var (not numeric): "+str(value), Warning)
                 raise(exceptions.InvalidCloudValue)
         while self._ratelimited_until + 0.1 >= time.time():
             pass
         try:
             self._send_packet(
                 {
@@ -157,15 +157,16 @@
         try:
             if cloud_host is None:
                 cloud_host = "wss://clouddata.turbowarp.org/"
                 self.cloud_host = cloud_host
             self.websocket.connect(
                 cloud_host,
                 enable_multithread=True,
-                timeout = self._ws_timeout
+                timeout = self._ws_timeout,
+                headers = {"User-Agent":"scratchattach/1.6.3"}
             )
         except Exception:
             raise(exceptions.ConnectionError)
         self._connect_timestamp = time.time()
 
 
     def set_var(self, variable, value):
@@ -177,15 +178,15 @@
             value (str): The value the cloud variable should be set to
         """
         variable = variable.replace("☁ ", "")
         if not (value is True or value is False or value in [float('inf'), -float('inf')]):
             value = str(value)
             x = value.replace(".", "")
             x = x.replace("-", "")
-            if not x.isnumeric():
+            if not (x.isnumeric() or x == ""):
                 if self.allow_non_numeric is False:
                     raise(exceptions.InvalidCloudValue)
 
         while self._ratelimited_until + 0.005 > time.time():
             pass
         try:
             self._send_packet(
```

### Comparing `scratchattach-1.6.2/scratchattach/cloud_requests.py` & `scratchattach-1.6.3/scratchattach/cloud_requests.py`

 * *Files 0% similar despite different names*

```diff
@@ -283,15 +283,16 @@
                 time.sleep(0.1)
 
         self.idle_since = time.time()
 
     def run(self,
             thread=False,
             data_from_websocket=True,
-            no_packet_loss=False):
+            no_packet_loss=False,
+            daemon=False):
         '''
         Starts the request handler.
         
         Args:
             thread: Whether the request handler should be run in a thread.
             data_from_websocket: Whether the websocket should be used to detect requests.
             no_packet_loss: Whether the request handler should reconnect to the cloud websocket before responding to a request, this can help to avoid packet loss.
@@ -314,15 +315,17 @@
         else:
             events = []
         self.cloud_events = events
         if thread:
             thread = Thread(
                 target=self._run,
                 args=[events],
-                kwargs={"data_from_websocket": data_from_websocket})
+                kwargs={"data_from_websocket": data_from_websocket},
+                daemon=daemon
+            )
             thread.start()
         else:
             self._run(events, data_from_websocket=data_from_websocket)
     
     def stop(self):
         """
         Permanently stops the cloud request handler and all background threads with cloud events.
```

### Comparing `scratchattach-1.6.2/scratchattach/encoder.py` & `scratchattach-1.6.3/scratchattach/encoder.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.6.2/scratchattach/exceptions.py` & `scratchattach-1.6.3/scratchattach/exceptions.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.6.2/scratchattach/forum.py` & `scratchattach-1.6.3/scratchattach/forum.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.6.2/scratchattach/project.py` & `scratchattach-1.6.3/scratchattach/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,23 +157,31 @@
         """
         if self._session is not None:
             project = requests.get(
                 f"https://api.scratch.mit.edu/projects/{self.id}",
                 headers = {
                     "user-agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/100.0.4896.88 Safari/537.36",
                     "x-token": self._session.xtoken,
+                    "Pragma" : "no-cache",
+                    "Cache-Control" : "no-cache"
                 }
             )
             if "429" in str(project):
                 return "429"
             if project.text == '{\n  "response": "Too many requests"\n}':
                 return "429"
             project = project.json()
         else:
-            project = requests.get(f"https://api.scratch.mit.edu/projects/{self.id}")
+            project = requests.get(f"https://api.scratch.mit.edu/projects/{self.id}",
+                headers = {
+                    "user-agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/100.0.4896.88 Safari/537.36",
+                    "Pragma" : "no-cache",
+                    "Cache-Control" : "no-cache"
+                }
+            )
             if "429" in str(project):
                 return "429"
             if project.text == '{\n  "response": "Too many requests"\n}':
                 return "429"
             project = project.json()
         if "code" in list(project.keys()):
             return False
@@ -284,28 +292,32 @@
         Returns:
             list<dict>: A list containing the requested comments as dicts.
         """
 
         comments = []
         while len(comments) < limit:
             r = requests.get(
-                f"https://api.scratch.mit.edu/users/{self.author}/projects/{self.id}/comments/?limit={min(40, limit-len(comments))}&offset={offset}&cachebust={random.randint(0,9999)}"
+                f"https://api.scratch.mit.edu/users/{self.author}/projects/{self.id}/comments/?limit={min(40, limit-len(comments))}&offset={offset}&cachebust={random.randint(0,9999)}",
+                headers = self._headers,
+                cookies = self._cookies
             ).json()
             if len(r) != 40:
                 comments = comments + r
                 break
             offset += 40
             comments = comments + r
         return comments
 
     def get_comment_replies(self, *, comment_id, limit=40, offset=0):
         comments = []
         while len(comments) < limit:
             r = requests.get(
-                f"https://api.scratch.mit.edu/users/{self.author}/projects/{self.id}/comments/{comment_id}/replies?limit={min(40, limit-len(comments))}&offset={offset}&cachebust=&cachebust={random.randint(0,9999)}"
+                f"https://api.scratch.mit.edu/users/{self.author}/projects/{self.id}/comments/{comment_id}/replies?limit={min(40, limit-len(comments))}&offset={offset}&cachebust=&cachebust={random.randint(0,9999)}",
+                headers = self._headers,
+                cookies = self._cookies
             ).json()
             if len(r) != 40:
                 comments = comments + r
                 break
             offset += 40
             comments = comments + r
         return comments
```

### Comparing `scratchattach-1.6.2/scratchattach/session.py` & `scratchattach-1.6.3/scratchattach/session.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,550 +1,550 @@
-#----- Connecting to a Scratch account
-
-import json
-import re
-import requests
-import warnings
-
-from . import user
-from . import cloud
-from . import project
-from . import exceptions
-from . import studio
-from . import forum
-
-headers = {
-    'user-agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/75.0.3770.142 Safari/537.36',
-    "x-csrftoken": "a",
-    "x-requested-with": "XMLHttpRequest",
-    "referer": "https://scratch.mit.edu",
-}
-
-class Session():
-
-    '''
-    Represents a Scratch log in / session. Stores authentication data (session id and xtoken).
-
-    Attributes:
-
-    :.session_id: The session id associated with the login
-
-    :.xtoken: The xtoken associated with the login
-
-    :.email: The email address associated with the logged in account
-
-    :.new_scratcher: Returns True if the associated account is a Scratcher
-
-    :.mute_status: Information about commenting restrictions of the associated account
-
-    :.banned: Returns True if the associated account is banned
-    '''
-    
-    def __init__(self, session_id, *, username=None):
-
-        self.session_id = str(session_id)
-        self._username = username
-        self._headers = headers
-        self._cookies = {
-            "scratchsessionsid" : self.session_id,
-            "scratchcsrftoken" : "a",
-            "scratchlanguage" : "en",
-            "accept": "application/json",
-            "Content-Type": "application/json",
-        }
-        self._get_xtoken()
-        try:
-            self._headers.pop("Cookie")
-        except Exception: pass
-
-    def _get_csrftoken(self):
-        r = requests.get("https://scratch.mit.edu/csrf_token/").headers
-        print(r)
-        csrftoken = r["Set-Cookie"].split("scratchcsrftoken=")[1].split(";")[0]
-        self._headers["x-csrftoken"] = csrftoken
-        self._cookies["scratchcsrftoken"] = csrftoken
-
-    def _get_xtoken(self):
-
-        # this will fetch the account token
-        try:
-            response = json.loads(requests.post(
-                "https://scratch.mit.edu/session",
-                headers = {
-                    'user-agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/75.0.3770.142 Safari/537.36',
-                    "x-csrftoken": "a",
-                    "x-requested-with": "XMLHttpRequest",
-                    "referer": "https://scratch.mit.edu",
-                },
-                cookies = {
-                    "scratchsessionsid" : self.session_id,
-                    "scratchcsrftoken" : "a",
-                    "scratchlanguage" : "en"
-                }
-            ).text)
-
-            self.xtoken = response['user']['token']
-            self._headers["X-Token"] = self.xtoken
-            self.email = response["user"]["email"]
-            self.new_scratcher = response["permissions"]["new_scratcher"]
-            self.mute_status = response["permissions"]["mute_status"]
-            self._username = response["user"]["username"]
-            self.banned = response["user"]["banned"]
-            if self.banned:
-                warnings.warn(f"Warning: The account {self._username} you logged in to is BANNED. Some features may not work properly.")
-
-        except Exception:
-            if self._username is None:
-                print("Warning: Logged in, but couldn't fetch XToken.\nSome features (including cloud variables) will not work properly. To get cloud variables to work, provide a username argument: Session('session_id', username='username')\nIf you're using an online IDE (like replit.com) Scratch possibly banned its IP adress.")
-            else:
-                print(f"Warning: Logged in as {self._username}, but couldn't fetch XToken. Cloud variables will still work, but other features may not work properly.\nIf you're using an online IDE (like replit.com) Scratch possibly banned its IP adress.")
-            self.xtoken = ""
-
-    def get_linked_user(self):
-        '''
-        Gets the user associated with the log in / session.
-
-        Returns:
-            scratchattach.user.User: Object representing the user associated with the log in / session.
-        '''
-        if not "_user" in self.__dict__:
-            self._user = self.connect_user(self._username)
-        return self._user
-
-    def mystuff_projects(self, ordering, *, page=1, sort_by="", descending=True):
-        '''
-        Gets the projects from the "My stuff" page.
-
-        Args:
-            ordering (str): Possible values for this parameter are "all", "shared", "unshared" and "trashed"
-        
-        Keyword Arguments:
-            page (int): The page of the "My Stuff" projects that should be returned
-            sort_by (str): The key the projects should be sorted based on. Possible values for this parameter are "" (then the projects are sorted based on last modified), "view_count", love_count", "remixers_count" (then the projects are sorted based on remix count) and "title" (then the projects are sorted based on title)
-            descending (boolean): Determines if the element with the highest key value (the key is specified in the sort_by argument) should be returned first. Defaults to True.
-      
-        Returns:
-            list<dict>: A list with the projects from the "My Stuff" page, each project is represented by a dict.
-        '''
-        if descending:
-            ascsort = ""
-            descsort = sort_by
-        else:
-            ascsort = sort_by
-            descsort = ""
-        try:
-            targets = requests.get(
-                f"https://scratch.mit.edu/site-api/projects/{ordering}/?page={page}&ascsort={ascsort}&descsort={descsort}",
-                headers = headers,
-                cookies = self._cookies,
-            ).json()
-            projects = []
-            for target in targets:
-                projects.append(
-                    dict(
-                        author = self._username,
-                        created = target["fields"]["datetime_created"],
-                        last_modified = target["fields"]["datetime_modified"],
-                        share_date = target["fields"]["datetime_shared"],
-                        shared = target["fields"]["isPublished"],
-                        id = target["pk"],
-                        thumbnail_url = "https://uploads.scratch.mit.edu"+target["fields"]["uncached_thumbnail_url"][1:],
-                        favorites = target["fields"]["favorite_count"],
-                        loves = target["fields"]["love_count"],
-                        remixes = target["fields"]["remixers_count"],
-                        views = target["fields"]["view_count"],
-                        thumbnail_name = target["fields"]["thumbnail"],
-                        title = target["fields"]["title"],
-                        url = "https://scratch.mit.edu/projects/" + str(target["pk"]),
-                        comment_count = target["fields"]["commenters_count"],
-                    )
-                )
-            return projects
-        except Exception:
-            raise(exceptions.FetchError)
-
-    def get_mystuff_projects(self, ordering, *, page=1, sort_by="", descending=True):
-        '''
-        Alternate name for :meth:`scratchattach.session.Session.mystuff_projects`. See the documentation of this function.
-        '''
-        return self.mystuff_projects(ordering, page=page, sort_by=sort_by, descending=descending)
-
-    def messages(self, *, limit=40, offset=0):
-        '''
-        Returns the messages.
-
-        Returns:
-            list<dict>: List that contains all messages as dicts.
-        '''
-        return requests.get(
-            f"https://api.scratch.mit.edu/users/{self._username}/messages?limit={limit}&offset={offset}",
-            headers = self._headers,
-            cookies = self._cookies,
-        ).json()
-
-    def clear_messages(self):
-        '''
-        Clears all messages.
-        '''
-        return requests.post(
-            "https://scratch.mit.edu/site-api/messages/messages-clear/",
-            headers = self._headers,
-            cookies = self._cookies,
-        ).text
-
-    def message_count(self):
-        '''
-        Returns the message count.
-
-        Returns:
-            int: message count
-        '''
-        return json.loads(requests.get(f"https://api.scratch.mit.edu/users/{self._username}/messages/count/", headers = {'user-agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.3c6 (KHTML, like Gecko) Chrome/75.0.3770.142 Safari/537.36',}).text)["count"]
-
-    def get_feed(self, *, limit=20, offset=0):
-        '''
-        Returns the "What's happening" section (frontpage).
-
-        Returns:
-            list<dict>: List that contains all "What's happening" entries as dicts
-        '''
-        return requests.get(
-            f"https://api.scratch.mit.edu/users/{self._username}/following/users/activity?limit={limit}&offset={offset}",
-            headers = self._headers,
-            cookies = self._cookies
-        ).json()
-
-    '''def create_project(self): # not working
-
-        try:
-
-            return self.connect_project(requests.post(
-                "https://projects.scratch.mit.edu/",
-                headers = headers,
-                cookies = self._cookies
-            ).json()["content-name"])
-        except Exception:
-            raise(exceptions.FetchError)
-    ''' 
-    ''' # these APIs are always empty
-    def created_by_followed_users(self, *, limit=40, offset=0):
-        r = requests.get(
-            f"https://api.scratch.mit.edu/users/{self._username}/following/users/projects?limit={limit}&offset={offset}",
-            headers = self._headers,
-            cookies = self._cookies
-        ).json()
-        projects = []
-
-        for project in r:
-            p = project.Project()
-            p._update_from_dict(project)
-            projects.append(p)
-        return projects
-
-    def added_to_followed_studios(self, *, limit=40, offset=0):
-        r = requests.get(
-            f"https://api.scratch.mit.edu/users/{self._username}/following/studios/projects?limit={limit}&offset={offset}",
-            headers = self._headers,
-            cookies = self._cookies
-        ).json()
-        projects = []
-
-        for project in r:
-            p = project.Project()
-            p._update_from_dict(project)
-            projects.append(p)
-        return projects
-    '''
-
-    def loved_by_followed_users(self, *, limit=40, offset=0):
-        '''
-        Returns the "Projects loved by Scratchers I'm following" section (frontpage).
-
-        Returns:
-            list<scratchattach.project.Project>: List that contains all "Projects loved by Scratchers I'm following" entries as Project objects
-        '''
-        r = requests.get(
-            f"https://api.scratch.mit.edu/users/{self._username}/following/users/loves?limit={limit}&offset={offset}",
-            headers = self._headers,
-            cookies = self._cookies
-        ).json()
-        projects = []
-
-        for project_dict in r:
-            p = project.Project(_session = self)
-            p._update_from_dict(project_dict)
-            projects.append(p)
-        return projects
-
-    def search_projects(self, *, query="", mode="trending", language="en", limit=40, offset=0):
-        '''
-        Uses the Scratch search to search projects.
-
-        Keyword arguments:
-            query (str): The query that will be searched.
-            mode (str): Has to be one of these values: "trending", "popular" or "recent". Defaults to "trending".
-            language (str): A language abbreviation, defaults to "en". (Depending on the language used on the Scratch website, Scratch displays you different results.)
-            limit (int): Max. amount of returned projects.
-            offset (int): Offset of the first returned project.
-
-        Returns:
-            list<scratchattach.project.Project>: List that contains the search results.
-        '''
-        r = requests.get(f"https://api.scratch.mit.edu/search/projects?limit={limit}&offset={offset}&language={language}&mode={mode}&q={query}").json()
-        projects = []
-
-        for project_dict in r:
-            p = project.Project(_session = self)
-            p._update_from_dict(project_dict)
-            projects.append(p)
-        return projects
-    def explore_projects(self, *, query="*", mode="trending", language="en", limit=40, offset=0):
-        '''
-        Gets projects from the explore page.
-
-        Keyword arguments:
-            query (str): Specifies the tag of the explore page. To get the projects from the "All" tag, set this argument to "*".
-            mode (str): Has to be one of these values: "trending", "popular" or "recent". Defaults to "trending".
-            language (str): A language abbreviation, defaults to "en". (Depending on the language used on the Scratch website, Scratch displays you different explore pages.)
-            limit (int): Max. amount of returned projects.
-            offset (int): Offset of the first returned project.
-
-        Returns:
-            list<scratchattach.project.Project>: List that contains the explore page projects.
-        '''
-        r = requests.get(f"https://api.scratch.mit.edu/explore/projects?limit={limit}&offset={offset}&language={language}&mode={mode}&q={query}").json()
-        projects = []
-
-        for project_dict in r:
-            p = project.Project(_session = self)
-            p._update_from_dict(project_dict)
-            projects.append(p)
-        return projects
-
-
-    def backpack(self,limit=20, offset=0):
-        '''
-        Lists the assets that are in the backpack of the user associated with the session.
-
-        Returns:
-            list<dict>: List that contains the backpack items as dicts
-        '''
-        return requests.get(
-            f"https://backpack.scratch.mit.edu/{self._username}?limit={limit}&offset={offset}",
-            headers = self._headers,
-        ).json()
-
-    def delete_from_backpack(self, asset_id):
-        '''
-        Deletes an asset from the backpack.
-
-        Args:
-            asset_id: ID of the asset that will be deleted.
-        '''
-        return requests.delete(
-            f"https://backpack.scratch.mit.edu/{self._username}/{asset_id}",
-            headers = self._headers,
-        ).json()
-
-    def connect_cloud(self, project_id_arg=None, *, project_id=None):
-        '''
-        Connects to the cloud variables of a project.
-
-        Args:
-            project_id (str): ID of the project that will be connected to.
-
-        Returns:
-            scratchattach.cloud.CloudConnection: An object that represents the created connection and allows you to set cloud variables
-        '''
-        if project_id is None:
-            project_id = project_id_arg
-        if project_id is None:
-            return None
-
-        return cloud.CloudConnection(username = self._username, session_id = self.session_id, project_id = int(project_id))
-
-    def connect_tw_cloud(self, project_id_arg=None, *, project_id=None):
-        return cloud.connect_tw_cloud(project_id_arg, project_id=project_id)
-
-    def connect_user(self, username):
-        """
-        Gets a user.
-
-        Args:
-            username (str): Username of the requested user
-
-        Returns:
-            scratchattach.user.User: An object that represents the requested user and allows you to perform actions on the user (like user.follow)
-        """
-        try:
-            _user = user.User(username=username, _session=self)
-            if _user.update() == "429":
-                raise(exceptions.Response429("Your network is blocked or rate-limited by Scratch.\nIf you're using an online IDE like replit.com, try running the code on your computer."))
-            return _user
-        except KeyError:
-            return None
-        except Exception as e:
-            raise(e)
-
-    def connect_project(self, project_id):
-        """
-        Gets a project.
-
-        Args:
-            project_id (int): ID of the requested project
-
-        Returns:
-            scratchattach.project.Project: An object that represents the requested project and allows you to perform actions on the project (like project.love)
-        """
-        try:
-            _project = project.Project(id=int(project_id), _session=self)
-            u = _project.update()
-            if u == "429":
-                raise(exceptions.Response429("Your network is blocked or rate-limited by Scratch.\nIf you're using an online IDE like replit.com, try running the code on your computer."))
-            if not u:
-                _project = project.PartialProject(id=int(project_id))
-            return _project
-        except KeyError:
-            return None
-        except Exception as e:
-            raise(e)
-
-    def connect_studio(self, studio_id):
-        """
-        Gets a studio.
-
-        Args:
-            studio_id (int): ID of the requested studio
-
-        Returns:
-            scratchattach.studio.Studio: An object that represents the requested studio and allows you to perform actions on the studio (like studio.follow)
-        """
-        try:
-            _studio = studio.Studio(id=int(studio_id), _session=self)
-            if _studio.update() == "429":
-                raise(exceptions.Response429("Your network is blocked or rate-limited by Scratch.\nIf you're using an online IDE like replit.com, try running the code on your computer."))
-            return _studio
-        except KeyError:
-            return None
-        except Exception as e:
-            raise(e)
-
-    def connect_topic(self, topic_id):
-        """
-        Gets a forum topic. Data fetched from ScratchDB.
-
-        Args:
-            topic_id (int): ID of the requested forum topic (can be found in the browser URL bar)
-
-        Returns:
-            scratchattach.forum.ForumTopic: An object that represents the requested forum topic
-        """
-
-        try:
-            topic = forum.ForumTopic(id=int(topic_id), _session=self)
-            topic.update()
-            return topic
-        except KeyError:
-            return None
-
-    def connect_topic_list(self, category_name, *, page=0, include_deleted=False):
-        """
-        Gets the topics from a forum category. Data fetched from ScratchDB.
-
-        Args:
-            category_name (str): Name of the forum category
-        
-        Keyword Arguments:
-            page (str): Page of the category topics that should be returned
-            include_deleted (boolean): Whether deleted topics should be returned too
-
-        Returns:
-            list<scratchattach.forum.ForumTopic>: A list containing the forum topics from the specified category
-        """
-        category_name.replace(" ", "%20")
-        if include_deleted:
-            filter = 0
-        else:
-            filter = 1
-        try:
-            data = requests.get(f"https://scratchdb.lefty.one/v3/forum/category/topics/{category_name}/{page}?detail=1&filter={filter}").json()
-            return_data = []
-            for topic in data:
-                t = forum.ForumTopic(id = topic["id"], _session=self)
-                t._update_from_dict(topic)
-                return_data.append(t)
-            return return_data
-        except Exception:
-            return None
-
-    def connect_post(self, post_id):
-
-        """
-        Gets a forum post. Data fetched from ScratchDB.
-
-        Args:
-            post_id (int): ID of the requested forum post
-
-        Returns:
-            scratchattach.forum.ForumPost: An object that represents the requested forum post
-        """
-
-        try:
-            post = forum.ForumPost(id=int(post_id), _session=self)
-            post.update()
-            return post
-        except KeyError:
-            return None
-
-    def search_posts(self, *, query, order="newest", page=0):
-        try:
-            data = requests.get(f"https://scratchdb.lefty.one/v3/forum/search?q={query}&o={order}&page={page}").json()["posts"]
-            return_data = []
-            for o in data:
-                a = forum.ForumPost(id = o["id"], _session = self._session)
-                a._update_from_dict(o)
-                return_data.append(a)
-            return return_data
-        except Exception:
-            return []
-
-    def upload_asset(asset):
-        data = asset if isinstance(asset, bytes) else open(asset, "rb").read()
-
-        if isinstance(asset, str):
-            file_ext = pathlib.Path(asset).suffix
-
-        requests.post(
-            f"https://assets.scratch.mit.edu/{hashlib.md5(data).hexdigest()}.{file_ext}",
-            headers=self._headers,
-            data=data,
-        )
-    
-# ------ #
-
-def login(username, password):
-    """
-    Creates a session / log in to the Scratch website with the specified username and password. 
-
-    This method will first create a session id, then it will fetch the xtoken and other information using the created session id.
-    If the log in fails, it will raise scratchattach.exceptions.LoginFailure.
-    If the login succeeds but fetching the xtoken fails, it will not raise an exception but display a warning. If the accout logged in to is banned, it will also display a warning.
-
-    Args:
-        username (str)
-        password (str)
-    
-    Returns:
-        scratchattach.session.Session: An object that represents the created log in / session
-    """
-    data = json.dumps({"username": username, "password": password})
-    _headers = headers
-    _headers["Cookie"] = "scratchcsrftoken=a;scratchlanguage=en;"
-    request = requests.post(
-        "https://scratch.mit.edu/login/", data=data, headers=_headers
-    )
-    try:
-        session_id = str(re.search('"(.*)"', request.headers["Set-Cookie"]).group())
-    except Exception:
-        raise exceptions.LoginFailure("Either the provided authentication data is wrong or your network is banned from Scratch.\n\nIf you're using an online IDE (like replit.com) Scratch possibly banned its IP adress. In this case, try logging in with your session id: https://github.com/TimMcCool/scratchattach/wiki#logging-in")
-    session = Session(session_id, username=username)
-    return session
+#----- Connecting to a Scratch account
+
+import json
+import re
+import requests
+import warnings
+
+from . import user
+from . import cloud
+from . import project
+from . import exceptions
+from . import studio
+from . import forum
+
+headers = {
+    'user-agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/75.0.3770.142 Safari/537.36',
+    "x-csrftoken": "a",
+    "x-requested-with": "XMLHttpRequest",
+    "referer": "https://scratch.mit.edu",
+}
+
+class Session():
+
+    '''
+    Represents a Scratch log in / session. Stores authentication data (session id and xtoken).
+
+    Attributes:
+
+    :.session_id: The session id associated with the login
+
+    :.xtoken: The xtoken associated with the login
+
+    :.email: The email address associated with the logged in account
+
+    :.new_scratcher: Returns True if the associated account is a Scratcher
+
+    :.mute_status: Information about commenting restrictions of the associated account
+
+    :.banned: Returns True if the associated account is banned
+    '''
+    
+    def __init__(self, session_id, *, username=None):
+
+        self.session_id = str(session_id)
+        self._username = username
+        self._headers = headers
+        self._cookies = {
+            "scratchsessionsid" : self.session_id,
+            "scratchcsrftoken" : "a",
+            "scratchlanguage" : "en",
+            "accept": "application/json",
+            "Content-Type": "application/json",
+        }
+        self._get_xtoken()
+        try:
+            self._headers.pop("Cookie")
+        except Exception: pass
+
+    def _get_csrftoken(self):
+        r = requests.get("https://scratch.mit.edu/csrf_token/").headers
+        print(r)
+        csrftoken = r["Set-Cookie"].split("scratchcsrftoken=")[1].split(";")[0]
+        self._headers["x-csrftoken"] = csrftoken
+        self._cookies["scratchcsrftoken"] = csrftoken
+
+    def _get_xtoken(self):
+
+        # this will fetch the account token
+        try:
+            response = json.loads(requests.post(
+                "https://scratch.mit.edu/session",
+                headers = {
+                    'user-agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/75.0.3770.142 Safari/537.36',
+                    "x-csrftoken": "a",
+                    "x-requested-with": "XMLHttpRequest",
+                    "referer": "https://scratch.mit.edu",
+                },
+                cookies = {
+                    "scratchsessionsid" : self.session_id,
+                    "scratchcsrftoken" : "a",
+                    "scratchlanguage" : "en"
+                }
+            ).text)
+
+            self.xtoken = response['user']['token']
+            self._headers["X-Token"] = self.xtoken
+            self.email = response["user"]["email"]
+            self.new_scratcher = response["permissions"]["new_scratcher"]
+            self.mute_status = response["permissions"]["mute_status"]
+            self._username = response["user"]["username"]
+            self.banned = response["user"]["banned"]
+            if self.banned:
+                warnings.warn(f"Warning: The account {self._username} you logged in to is BANNED. Some features may not work properly.")
+
+        except Exception:
+            if self._username is None:
+                print("Warning: Logged in, but couldn't fetch XToken.\nSome features (including cloud variables) will not work properly. To get cloud variables to work, provide a username argument: Session('session_id', username='username')\nIf you're using an online IDE (like replit.com) Scratch possibly banned its IP adress.")
+            else:
+                print(f"Warning: Logged in as {self._username}, but couldn't fetch XToken. Cloud variables will still work, but other features may not work properly.\nIf you're using an online IDE (like replit.com) Scratch possibly banned its IP adress.")
+            self.xtoken = ""
+
+    def get_linked_user(self):
+        '''
+        Gets the user associated with the log in / session.
+
+        Returns:
+            scratchattach.user.User: Object representing the user associated with the log in / session.
+        '''
+        if not "_user" in self.__dict__:
+            self._user = self.connect_user(self._username)
+        return self._user
+
+    def mystuff_projects(self, ordering, *, page=1, sort_by="", descending=True):
+        '''
+        Gets the projects from the "My stuff" page.
+
+        Args:
+            ordering (str): Possible values for this parameter are "all", "shared", "unshared" and "trashed"
+        
+        Keyword Arguments:
+            page (int): The page of the "My Stuff" projects that should be returned
+            sort_by (str): The key the projects should be sorted based on. Possible values for this parameter are "" (then the projects are sorted based on last modified), "view_count", love_count", "remixers_count" (then the projects are sorted based on remix count) and "title" (then the projects are sorted based on title)
+            descending (boolean): Determines if the element with the highest key value (the key is specified in the sort_by argument) should be returned first. Defaults to True.
+      
+        Returns:
+            list<dict>: A list with the projects from the "My Stuff" page, each project is represented by a dict.
+        '''
+        if descending:
+            ascsort = ""
+            descsort = sort_by
+        else:
+            ascsort = sort_by
+            descsort = ""
+        try:
+            targets = requests.get(
+                f"https://scratch.mit.edu/site-api/projects/{ordering}/?page={page}&ascsort={ascsort}&descsort={descsort}",
+                headers = headers,
+                cookies = self._cookies,
+            ).json()
+            projects = []
+            for target in targets:
+                projects.append(
+                    dict(
+                        author = self._username,
+                        created = target["fields"]["datetime_created"],
+                        last_modified = target["fields"]["datetime_modified"],
+                        share_date = target["fields"]["datetime_shared"],
+                        shared = target["fields"]["isPublished"],
+                        id = target["pk"],
+                        thumbnail_url = "https://uploads.scratch.mit.edu"+target["fields"]["uncached_thumbnail_url"][1:],
+                        favorites = target["fields"]["favorite_count"],
+                        loves = target["fields"]["love_count"],
+                        remixes = target["fields"]["remixers_count"],
+                        views = target["fields"]["view_count"],
+                        thumbnail_name = target["fields"]["thumbnail"],
+                        title = target["fields"]["title"],
+                        url = "https://scratch.mit.edu/projects/" + str(target["pk"]),
+                        comment_count = target["fields"]["commenters_count"],
+                    )
+                )
+            return projects
+        except Exception:
+            raise(exceptions.FetchError)
+
+    def get_mystuff_projects(self, ordering, *, page=1, sort_by="", descending=True):
+        '''
+        Alternate name for :meth:`scratchattach.session.Session.mystuff_projects`. See the documentation of this function.
+        '''
+        return self.mystuff_projects(ordering, page=page, sort_by=sort_by, descending=descending)
+
+    def messages(self, *, limit=40, offset=0):
+        '''
+        Returns the messages.
+
+        Returns:
+            list<dict>: List that contains all messages as dicts.
+        '''
+        return requests.get(
+            f"https://api.scratch.mit.edu/users/{self._username}/messages?limit={limit}&offset={offset}",
+            headers = self._headers,
+            cookies = self._cookies,
+        ).json()
+
+    def clear_messages(self):
+        '''
+        Clears all messages.
+        '''
+        return requests.post(
+            "https://scratch.mit.edu/site-api/messages/messages-clear/",
+            headers = self._headers,
+            cookies = self._cookies,
+        ).text
+
+    def message_count(self):
+        '''
+        Returns the message count.
+
+        Returns:
+            int: message count
+        '''
+        return json.loads(requests.get(f"https://api.scratch.mit.edu/users/{self._username}/messages/count/", headers = {'user-agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.3c6 (KHTML, like Gecko) Chrome/75.0.3770.142 Safari/537.36',}).text)["count"]
+
+    def get_feed(self, *, limit=20, offset=0):
+        '''
+        Returns the "What's happening" section (frontpage).
+
+        Returns:
+            list<dict>: List that contains all "What's happening" entries as dicts
+        '''
+        return requests.get(
+            f"https://api.scratch.mit.edu/users/{self._username}/following/users/activity?limit={limit}&offset={offset}",
+            headers = self._headers,
+            cookies = self._cookies
+        ).json()
+
+    '''def create_project(self): # not working
+
+        try:
+
+            return self.connect_project(requests.post(
+                "https://projects.scratch.mit.edu/",
+                headers = headers,
+                cookies = self._cookies
+            ).json()["content-name"])
+        except Exception:
+            raise(exceptions.FetchError)
+    ''' 
+    ''' # these APIs are always empty
+    def created_by_followed_users(self, *, limit=40, offset=0):
+        r = requests.get(
+            f"https://api.scratch.mit.edu/users/{self._username}/following/users/projects?limit={limit}&offset={offset}",
+            headers = self._headers,
+            cookies = self._cookies
+        ).json()
+        projects = []
+
+        for project in r:
+            p = project.Project()
+            p._update_from_dict(project)
+            projects.append(p)
+        return projects
+
+    def added_to_followed_studios(self, *, limit=40, offset=0):
+        r = requests.get(
+            f"https://api.scratch.mit.edu/users/{self._username}/following/studios/projects?limit={limit}&offset={offset}",
+            headers = self._headers,
+            cookies = self._cookies
+        ).json()
+        projects = []
+
+        for project in r:
+            p = project.Project()
+            p._update_from_dict(project)
+            projects.append(p)
+        return projects
+    '''
+
+    def loved_by_followed_users(self, *, limit=40, offset=0):
+        '''
+        Returns the "Projects loved by Scratchers I'm following" section (frontpage).
+
+        Returns:
+            list<scratchattach.project.Project>: List that contains all "Projects loved by Scratchers I'm following" entries as Project objects
+        '''
+        r = requests.get(
+            f"https://api.scratch.mit.edu/users/{self._username}/following/users/loves?limit={limit}&offset={offset}",
+            headers = self._headers,
+            cookies = self._cookies
+        ).json()
+        projects = []
+
+        for project_dict in r:
+            p = project.Project(_session = self)
+            p._update_from_dict(project_dict)
+            projects.append(p)
+        return projects
+
+    def search_projects(self, *, query="", mode="trending", language="en", limit=40, offset=0):
+        '''
+        Uses the Scratch search to search projects.
+
+        Keyword arguments:
+            query (str): The query that will be searched.
+            mode (str): Has to be one of these values: "trending", "popular" or "recent". Defaults to "trending".
+            language (str): A language abbreviation, defaults to "en". (Depending on the language used on the Scratch website, Scratch displays you different results.)
+            limit (int): Max. amount of returned projects.
+            offset (int): Offset of the first returned project.
+
+        Returns:
+            list<scratchattach.project.Project>: List that contains the search results.
+        '''
+        r = requests.get(f"https://api.scratch.mit.edu/search/projects?limit={limit}&offset={offset}&language={language}&mode={mode}&q={query}").json()
+        projects = []
+
+        for project_dict in r:
+            p = project.Project(_session = self)
+            p._update_from_dict(project_dict)
+            projects.append(p)
+        return projects
+    def explore_projects(self, *, query="*", mode="trending", language="en", limit=40, offset=0):
+        '''
+        Gets projects from the explore page.
+
+        Keyword arguments:
+            query (str): Specifies the tag of the explore page. To get the projects from the "All" tag, set this argument to "*".
+            mode (str): Has to be one of these values: "trending", "popular" or "recent". Defaults to "trending".
+            language (str): A language abbreviation, defaults to "en". (Depending on the language used on the Scratch website, Scratch displays you different explore pages.)
+            limit (int): Max. amount of returned projects.
+            offset (int): Offset of the first returned project.
+
+        Returns:
+            list<scratchattach.project.Project>: List that contains the explore page projects.
+        '''
+        r = requests.get(f"https://api.scratch.mit.edu/explore/projects?limit={limit}&offset={offset}&language={language}&mode={mode}&q={query}").json()
+        projects = []
+
+        for project_dict in r:
+            p = project.Project(_session = self)
+            p._update_from_dict(project_dict)
+            projects.append(p)
+        return projects
+
+
+    def backpack(self,limit=20, offset=0):
+        '''
+        Lists the assets that are in the backpack of the user associated with the session.
+
+        Returns:
+            list<dict>: List that contains the backpack items as dicts
+        '''
+        return requests.get(
+            f"https://backpack.scratch.mit.edu/{self._username}?limit={limit}&offset={offset}",
+            headers = self._headers,
+        ).json()
+
+    def delete_from_backpack(self, asset_id):
+        '''
+        Deletes an asset from the backpack.
+
+        Args:
+            asset_id: ID of the asset that will be deleted.
+        '''
+        return requests.delete(
+            f"https://backpack.scratch.mit.edu/{self._username}/{asset_id}",
+            headers = self._headers,
+        ).json()
+
+    def connect_cloud(self, project_id_arg=None, *, project_id=None):
+        '''
+        Connects to the cloud variables of a project.
+
+        Args:
+            project_id (str): ID of the project that will be connected to.
+
+        Returns:
+            scratchattach.cloud.CloudConnection: An object that represents the created connection and allows you to set cloud variables
+        '''
+        if project_id is None:
+            project_id = project_id_arg
+        if project_id is None:
+            return None
+
+        return cloud.CloudConnection(username = self._username, session_id = self.session_id, project_id = int(project_id))
+
+    def connect_tw_cloud(self, project_id_arg=None, *, project_id=None):
+        return cloud.connect_tw_cloud(project_id_arg, project_id=project_id)
+
+    def connect_user(self, username):
+        """
+        Gets a user.
+
+        Args:
+            username (str): Username of the requested user
+
+        Returns:
+            scratchattach.user.User: An object that represents the requested user and allows you to perform actions on the user (like user.follow)
+        """
+        try:
+            _user = user.User(username=username, _session=self)
+            if _user.update() == "429":
+                raise(exceptions.Response429("Your network is blocked or rate-limited by Scratch.\nIf you're using an online IDE like replit.com, try running the code on your computer."))
+            return _user
+        except KeyError:
+            return None
+        except Exception as e:
+            raise(e)
+
+    def connect_project(self, project_id):
+        """
+        Gets a project.
+
+        Args:
+            project_id (int): ID of the requested project
+
+        Returns:
+            scratchattach.project.Project: An object that represents the requested project and allows you to perform actions on the project (like project.love)
+        """
+        try:
+            _project = project.Project(id=int(project_id), _session=self)
+            u = _project.update()
+            if u == "429":
+                raise(exceptions.Response429("Your network is blocked or rate-limited by Scratch.\nIf you're using an online IDE like replit.com, try running the code on your computer."))
+            if not u:
+                _project = project.PartialProject(id=int(project_id))
+            return _project
+        except KeyError:
+            return None
+        except Exception as e:
+            raise(e)
+
+    def connect_studio(self, studio_id):
+        """
+        Gets a studio.
+
+        Args:
+            studio_id (int): ID of the requested studio
+
+        Returns:
+            scratchattach.studio.Studio: An object that represents the requested studio and allows you to perform actions on the studio (like studio.follow)
+        """
+        try:
+            _studio = studio.Studio(id=int(studio_id), _session=self)
+            if _studio.update() == "429":
+                raise(exceptions.Response429("Your network is blocked or rate-limited by Scratch.\nIf you're using an online IDE like replit.com, try running the code on your computer."))
+            return _studio
+        except KeyError:
+            return None
+        except Exception as e:
+            raise(e)
+
+    def connect_topic(self, topic_id):
+        """
+        Gets a forum topic. Data fetched from ScratchDB.
+
+        Args:
+            topic_id (int): ID of the requested forum topic (can be found in the browser URL bar)
+
+        Returns:
+            scratchattach.forum.ForumTopic: An object that represents the requested forum topic
+        """
+
+        try:
+            topic = forum.ForumTopic(id=int(topic_id), _session=self)
+            topic.update()
+            return topic
+        except KeyError:
+            return None
+
+    def connect_topic_list(self, category_name, *, page=0, include_deleted=False):
+        """
+        Gets the topics from a forum category. Data fetched from ScratchDB.
+
+        Args:
+            category_name (str): Name of the forum category
+        
+        Keyword Arguments:
+            page (str): Page of the category topics that should be returned
+            include_deleted (boolean): Whether deleted topics should be returned too
+
+        Returns:
+            list<scratchattach.forum.ForumTopic>: A list containing the forum topics from the specified category
+        """
+        category_name.replace(" ", "%20")
+        if include_deleted:
+            filter = 0
+        else:
+            filter = 1
+        try:
+            data = requests.get(f"https://scratchdb.lefty.one/v3/forum/category/topics/{category_name}/{page}?detail=1&filter={filter}").json()
+            return_data = []
+            for topic in data:
+                t = forum.ForumTopic(id = topic["id"], _session=self)
+                t._update_from_dict(topic)
+                return_data.append(t)
+            return return_data
+        except Exception:
+            return None
+
+    def connect_post(self, post_id):
+
+        """
+        Gets a forum post. Data fetched from ScratchDB.
+
+        Args:
+            post_id (int): ID of the requested forum post
+
+        Returns:
+            scratchattach.forum.ForumPost: An object that represents the requested forum post
+        """
+
+        try:
+            post = forum.ForumPost(id=int(post_id), _session=self)
+            post.update()
+            return post
+        except KeyError:
+            return None
+
+    def search_posts(self, *, query, order="newest", page=0):
+        try:
+            data = requests.get(f"https://scratchdb.lefty.one/v3/forum/search?q={query}&o={order}&page={page}").json()["posts"]
+            return_data = []
+            for o in data:
+                a = forum.ForumPost(id = o["id"], _session = self._session)
+                a._update_from_dict(o)
+                return_data.append(a)
+            return return_data
+        except Exception:
+            return []
+
+    def upload_asset(asset):
+        data = asset if isinstance(asset, bytes) else open(asset, "rb").read()
+
+        if isinstance(asset, str):
+            file_ext = pathlib.Path(asset).suffix
+
+        requests.post(
+            f"https://assets.scratch.mit.edu/{hashlib.md5(data).hexdigest()}.{file_ext}",
+            headers=self._headers,
+            data=data,
+        )
+    
+# ------ #
+
+def login(username, password):
+    """
+    Creates a session / log in to the Scratch website with the specified username and password. 
+
+    This method will first create a session id, then it will fetch the xtoken and other information using the created session id.
+    If the log in fails, it will raise scratchattach.exceptions.LoginFailure.
+    If the login succeeds but fetching the xtoken fails, it will not raise an exception but display a warning. If the accout logged in to is banned, it will also display a warning.
+
+    Args:
+        username (str)
+        password (str)
+    
+    Returns:
+        scratchattach.session.Session: An object that represents the created log in / session
+    """
+    data = json.dumps({"username": username, "password": password})
+    _headers = headers
+    _headers["Cookie"] = "scratchcsrftoken=a;scratchlanguage=en;"
+    request = requests.post(
+        "https://scratch.mit.edu/login/", data=data, headers=_headers
+    )
+    try:
+        session_id = str(re.search('"(.*)"', request.headers["Set-Cookie"]).group())
+    except Exception:
+        raise exceptions.LoginFailure("Either the provided authentication data is wrong or your network is banned from Scratch.\n\nIf you're using an online IDE (like replit.com) Scratch possibly banned its IP adress. In this case, try logging in with your session id: https://github.com/TimMcCool/scratchattach/wiki#logging-in")
+    session = Session(session_id, username=username)
+    return session
```

### Comparing `scratchattach-1.6.2/scratchattach/studio.py` & `scratchattach-1.6.3/scratchattach/studio.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.6.2/scratchattach/user.py` & `scratchattach-1.6.3/scratchattach/user.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.6.2/scratchattach.egg-info/PKG-INFO` & `scratchattach-1.6.3/scratchattach.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: scratchattach
-Version: 1.6.2
-Summary: An Scratch API Wrapper for scratch.mit.edu
+Version: 1.6.3
+Summary: An Scratch API Wrapper for scra tch.mit.edu
 Home-page: https://github.com/TimMcCool/scratchattach
 Author: TimMcCool
-Author-email: 
+Author-email: timkrome2006@gmail.com
 Keywords: scratch api,scratchattach,scratch api python,scratch python,scratch for python,scratch,scratch cloud,scratch cloud variables,scratch bot
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `scratchattach-1.6.2/setup.py` & `scratchattach-1.6.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '1.6.2'
-DESCRIPTION = 'An Scratch API Wrapper for scratch.mit.edu'
+VERSION = '1.6.3'
+DESCRIPTION = 'An Scratch API Wrapper for scra tch.mit.edu'
 LONG_DESCRIPTION = DESCRIPTION
 
 # Setting up
 setup(
     name="scratchattach",
     version=VERSION,
     author="TimMcCool",
-    author_email="",
+    author_email="timkrome2006@gmail.com",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=open('README.md').read(),
     packages=find_packages(),
     install_requires=["websocket-client","numpy","requests","bs4"],
     keywords=['scratch api', 'scratchattach', 'scratch api python', 'scratch python', 'scratch for python', 'scratch', 'scratch cloud', 'scratch cloud variables', 'scratch bot'],
     url='https://github.com/TimMcCool/scratchattach',
```

