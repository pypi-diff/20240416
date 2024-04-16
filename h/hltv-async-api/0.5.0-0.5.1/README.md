# Comparing `tmp/hltv_async_api-0.5.0.tar.gz` & `tmp/hltv_async_api-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hltv_async_api-0.5.0.tar", max compression
+gzip compressed data, was "hltv_async_api-0.5.1.tar", max compression
```

## Comparing `hltv_async_api-0.5.0.tar` & `hltv_async_api-0.5.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      124 2024-04-15 21:04:14.467485 hltv_async_api-0.5.0/hltv_async_api/__init__.py
--rw-r--r--   0        0        0    37794 2024-04-15 21:33:45.834139 hltv_async_api-0.5.0/hltv_async_api/aiohltv.py
--rw-r--r--   0        0        0     1935 2024-04-03 12:53:56.200826 hltv_async_api-0.5.0/hltv_async_api/proxies.txt
--rw-r--r--   0        0        0     1091 2024-04-02 00:22:12.491888 hltv_async_api-0.5.0/LICENSE
--rw-r--r--   0        0        0      648 2024-04-15 21:34:36.417758 hltv_async_api-0.5.0/pyproject.toml
--rw-r--r--   0        0        0    15285 2024-04-15 21:33:45.841132 hltv_async_api-0.5.0/README.md
--rw-r--r--   0        0        0    15811 1970-01-01 00:00:00.000000 hltv_async_api-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      124 2024-04-16 15:56:41.976763 hltv_async_api-0.5.1/hltv_async_api/__init__.py
+-rw-r--r--   0        0        0    37792 2024-04-16 15:56:13.528920 hltv_async_api-0.5.1/hltv_async_api/aiohltv.py
+-rw-r--r--   0        0        0     1935 2024-04-03 12:53:56.200826 hltv_async_api-0.5.1/hltv_async_api/proxies.txt
+-rw-r--r--   0        0        0     1091 2024-04-02 00:22:12.491888 hltv_async_api-0.5.1/LICENSE
+-rw-r--r--   0        0        0      648 2024-04-16 15:56:41.983765 hltv_async_api-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0    15288 2024-04-15 21:37:37.703676 hltv_async_api-0.5.1/README.md
+-rw-r--r--   0        0        0    15814 1970-01-01 00:00:00.000000 hltv_async_api-0.5.1/PKG-INFO
```

### Comparing `hltv_async_api-0.5.0/hltv_async_api/aiohltv.py` & `hltv_async_api-0.5.1/hltv_async_api/aiohltv.py`

 * *Files 0% similar despite different names*

```diff
@@ -278,15 +278,15 @@
                             't1_id': t1_id,
                             't2_id': t2_id,
                             'maps': maps,
                             'rating': rating,
                             'event': event
                         })
 
-            if upcoming:
+            if future:
                 for i, date_div in enumerate(r.find_all('div', {'class': 'upcomingMatchesSection'}), start=1):
                     if i > days:
                         break
                     date_ = date_div.find('span', {'class': 'matchDayHeadline'}).text.split()[-1]
 
                     for match in date_div.find_all('div', {'class': 'upcomingMatch'}):
                         time_ = match.find('div', {'class': 'matchTime'}).text
```

### Comparing `hltv_async_api-0.5.0/hltv_async_api/proxies.txt` & `hltv_async_api-0.5.1/hltv_async_api/proxies.txt`

 * *Files identical despite different names*

### Comparing `hltv_async_api-0.5.0/LICENSE` & `hltv_async_api-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hltv_async_api-0.5.0/pyproject.toml` & `hltv_async_api-0.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hltv_async_api"
-version = "0.5.0"
+version = "0.5.1"
 authors = ["Akim Slys <akimslys2003@gmail.com>"]
 description = "Hltv-aio An unofficial asynchronous HLTV API Wrapper for Python"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `hltv_async_api-0.5.0/README.md` & `hltv_async_api-0.5.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
 
 * **get async def get(type: str, id: int | str | None = None, title: str | None = None, team1: str | None = None, team2: str | None = None):**
   (BETA) This method is not finished. Possible types 'events', 'matches', 'teams', also u can add id | title | team1 | team2, to parse more.
   ex. 
   
   ```
   
-  await hltv.get('matches', 2370773, 'res-regional-series-3-latam', 'FURIA', 'MIBR')
+  await hltv.get('matches', 2371201, 'res-regional-series-3-latam', 'IMPERIAL', 'MIBR')
   
   >>> (2371201, 0, 0, 'LIVE', [{'mapname': 'Vertigo', 'r_team1': '6', 'r_team2': '13'}, {'mapname': 'Mirage', 'r_team1': '-', 'r_team2': '-'}, {'mapname': 'Anubis', 'r_team1': '-', 'r_team2': '-'}], [])
   
   ```
 ---
 # Configs
```

### Comparing `hltv_async_api-0.5.0/PKG-INFO` & `hltv_async_api-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hltv_async_api
-Version: 0.5.0
+Version: 0.5.1
 Summary: Hltv-aio An unofficial asynchronous HLTV API Wrapper for Python
 Author: Akim Slys
 Author-email: akimslys2003@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -205,15 +205,15 @@
 
 * **get async def get(type: str, id: int | str | None = None, title: str | None = None, team1: str | None = None, team2: str | None = None):**
   (BETA) This method is not finished. Possible types 'events', 'matches', 'teams', also u can add id | title | team1 | team2, to parse more.
   ex. 
   
   ```
   
-  await hltv.get('matches', 2370773, 'res-regional-series-3-latam', 'FURIA', 'MIBR')
+  await hltv.get('matches', 2371201, 'res-regional-series-3-latam', 'IMPERIAL', 'MIBR')
   
   >>> (2371201, 0, 0, 'LIVE', [{'mapname': 'Vertigo', 'r_team1': '6', 'r_team2': '13'}, {'mapname': 'Mirage', 'r_team1': '-', 'r_team2': '-'}, {'mapname': 'Anubis', 'r_team1': '-', 'r_team2': '-'}], [])
   
   ```
 ---
 # Configs
```

