# Comparing `tmp/yfjpscraper-0.4.0.tar.gz` & `tmp/yfjpscraper-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yfjpscraper-0.4.0.tar", last modified: Wed Sep 27 00:41:36 2023, max compression
+gzip compressed data, was "yfjpscraper-0.4.1.tar", last modified: Tue Apr 16 00:34:18 2024, max compression
```

## Comparing `yfjpscraper-0.4.0.tar` & `yfjpscraper-0.4.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 zenbook   (1000) zenbook   (1000)        0 2023-09-27 00:41:36.983609 yfjpscraper-0.4.0/
--rw-rw-r--   0 zenbook   (1000) zenbook   (1000)      192 2023-09-27 00:41:36.983609 yfjpscraper-0.4.0/PKG-INFO
--rw-rw-r--   0 zenbook   (1000) zenbook   (1000)      292 2021-05-26 00:02:57.000000 yfjpscraper-0.4.0/README.md
--rw-rw-r--   0 zenbook   (1000) zenbook   (1000)      350 2022-02-16 05:54:12.000000 yfjpscraper-0.4.0/README.rst
--rw-rw-r--   0 zenbook   (1000) zenbook   (1000)       38 2023-09-27 00:41:36.983609 yfjpscraper-0.4.0/setup.cfg
--rw-rw-r--   0 zenbook   (1000) zenbook   (1000)      342 2023-09-27 00:41:17.000000 yfjpscraper-0.4.0/setup.py
-drwxrwxr-x   0 zenbook   (1000) zenbook   (1000)        0 2023-09-27 00:41:36.979609 yfjpscraper-0.4.0/yfjpscraper/
--rw-rw-r--   0 zenbook   (1000) zenbook   (1000)     5274 2023-09-27 00:40:48.000000 yfjpscraper-0.4.0/yfjpscraper/__init__.py
--rw-rw-r--   0 zenbook   (1000) zenbook   (1000)     4200 2022-11-29 05:35:45.000000 yfjpscraper-0.4.0/yfjpscraper/parser.py
-drwxrwxr-x   0 zenbook   (1000) zenbook   (1000)        0 2023-09-27 00:41:36.983609 yfjpscraper-0.4.0/yfjpscraper.egg-info/
--rw-rw-r--   0 zenbook   (1000) zenbook   (1000)      192 2023-09-27 00:41:36.000000 yfjpscraper-0.4.0/yfjpscraper.egg-info/PKG-INFO
--rw-rw-r--   0 zenbook   (1000) zenbook   (1000)      249 2023-09-27 00:41:36.000000 yfjpscraper-0.4.0/yfjpscraper.egg-info/SOURCES.txt
--rw-rw-r--   0 zenbook   (1000) zenbook   (1000)        1 2023-09-27 00:41:36.000000 yfjpscraper-0.4.0/yfjpscraper.egg-info/dependency_links.txt
--rw-rw-r--   0 zenbook   (1000) zenbook   (1000)       17 2023-09-27 00:41:36.000000 yfjpscraper-0.4.0/yfjpscraper.egg-info/requires.txt
--rw-rw-r--   0 zenbook   (1000) zenbook   (1000)       12 2023-09-27 00:41:36.000000 yfjpscraper-0.4.0/yfjpscraper.egg-info/top_level.txt
+drwxrwxr-x   0 zenbook   (1000) zenbook   (1000)        0 2024-04-16 00:34:18.337831 yfjpscraper-0.4.1/
+-rw-rw-r--   0 zenbook   (1000) zenbook   (1000)      192 2024-04-16 00:34:18.337831 yfjpscraper-0.4.1/PKG-INFO
+-rw-rw-r--   0 zenbook   (1000) zenbook   (1000)      292 2021-05-26 00:02:57.000000 yfjpscraper-0.4.1/README.md
+-rw-rw-r--   0 zenbook   (1000) zenbook   (1000)      350 2022-02-16 05:54:12.000000 yfjpscraper-0.4.1/README.rst
+-rw-rw-r--   0 zenbook   (1000) zenbook   (1000)       38 2024-04-16 00:34:18.337831 yfjpscraper-0.4.1/setup.cfg
+-rw-rw-r--   0 zenbook   (1000) zenbook   (1000)      342 2024-04-16 00:23:00.000000 yfjpscraper-0.4.1/setup.py
+drwxrwxr-x   0 zenbook   (1000) zenbook   (1000)        0 2024-04-16 00:34:18.333831 yfjpscraper-0.4.1/yfjpscraper/
+-rw-rw-r--   0 zenbook   (1000) zenbook   (1000)     5294 2024-04-16 00:23:21.000000 yfjpscraper-0.4.1/yfjpscraper/__init__.py
+-rw-rw-r--   0 zenbook   (1000) zenbook   (1000)     4200 2022-11-29 05:35:45.000000 yfjpscraper-0.4.1/yfjpscraper/parser.py
+drwxrwxr-x   0 zenbook   (1000) zenbook   (1000)        0 2024-04-16 00:34:18.333831 yfjpscraper-0.4.1/yfjpscraper.egg-info/
+-rw-rw-r--   0 zenbook   (1000) zenbook   (1000)      192 2024-04-16 00:34:18.000000 yfjpscraper-0.4.1/yfjpscraper.egg-info/PKG-INFO
+-rw-rw-r--   0 zenbook   (1000) zenbook   (1000)      249 2024-04-16 00:34:18.000000 yfjpscraper-0.4.1/yfjpscraper.egg-info/SOURCES.txt
+-rw-rw-r--   0 zenbook   (1000) zenbook   (1000)        1 2024-04-16 00:34:18.000000 yfjpscraper-0.4.1/yfjpscraper.egg-info/dependency_links.txt
+-rw-rw-r--   0 zenbook   (1000) zenbook   (1000)       17 2024-04-16 00:34:18.000000 yfjpscraper-0.4.1/yfjpscraper.egg-info/requires.txt
+-rw-rw-r--   0 zenbook   (1000) zenbook   (1000)       12 2024-04-16 00:34:18.000000 yfjpscraper-0.4.1/yfjpscraper.egg-info/top_level.txt
```

### Comparing `yfjpscraper-0.4.0/yfjpscraper/__init__.py` & `yfjpscraper-0.4.1/yfjpscraper/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,15 +150,15 @@
         "User-Agent": "Mozilla/5.0 (X11; Ubuntu; Linux x86_64; rv:95.0) Gecko/20100101 Firefox/95.0",
         "Accept-Language": "ja,en-US;q=0.7,en;q=0.3",
         "Connection": "keep-alive",
         "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,*/*;q=0.8",
         "Accept-Encoding": "gzip, deflate, br",
     }
     session = kanirequests.KaniRequests(
-        headers=headers, proxy=proxy
+        headers=headers, proxy=proxy, default_timeout=30
     )
     root_url = f"https://finance.yahoo.co.jp/quote/{tick_id}/history"
     result = session.get(root_url)
     if result.status_code != 200:
         raise HTTPError(f"status code is {result.status_code} url:{root_url}")
     if "indicesJwtToken" in result.text:
         return get_data_futures(session, result, tick_id, start_dt, end_dt)
```

### Comparing `yfjpscraper-0.4.0/yfjpscraper/parser.py` & `yfjpscraper-0.4.1/yfjpscraper/parser.py`

 * *Files identical despite different names*

