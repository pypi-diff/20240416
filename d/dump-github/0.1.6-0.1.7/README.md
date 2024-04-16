# Comparing `tmp/dump_github-0.1.6-py3-none-any.whl.zip` & `tmp/dump_github-0.1.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 4684 bytes, number of entries: 10
+Zip file size: 4725 bytes, number of entries: 10
 -rw-rw-r--  2.0 unx       43 b- defN 24-Apr-10 18:26 dump_github/__init__.py
--rw-rw-r--  2.0 unx      715 b- defN 24-Apr-10 17:24 dump_github/lib.py
+-rw-rw-r--  2.0 unx      716 b- defN 24-Apr-16 12:58 dump_github/lib.py
 -rw-rw-r--  2.0 unx     1842 b- defN 24-Apr-11 11:40 dump_github/main.py
 -rw-rw-r--  2.0 unx      715 b- defN 24-Apr-10 17:24 dump_github/mylib.py
--rw-rw-r--  2.0 unx     1064 b- defN 24-Apr-11 11:44 dump_github-0.1.6.dist-info/LICENSE
--rw-rw-r--  2.0 unx     1287 b- defN 24-Apr-11 11:44 dump_github-0.1.6.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Apr-11 11:44 dump_github-0.1.6.dist-info/WHEEL
--rw-rw-r--  2.0 unx       50 b- defN 24-Apr-11 11:44 dump_github-0.1.6.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       12 b- defN 24-Apr-11 11:44 dump_github-0.1.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      809 b- defN 24-Apr-11 11:44 dump_github-0.1.6.dist-info/RECORD
-10 files, 6629 bytes uncompressed, 3296 bytes compressed:  50.3%
+-rw-rw-r--  2.0 unx     1064 b- defN 24-Apr-16 13:08 dump_github-0.1.7.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     1316 b- defN 24-Apr-16 13:08 dump_github-0.1.7.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Apr-16 13:08 dump_github-0.1.7.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       49 b- defN 24-Apr-16 13:08 dump_github-0.1.7.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       12 b- defN 24-Apr-16 13:08 dump_github-0.1.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      809 b- defN 24-Apr-16 13:08 dump_github-0.1.7.dist-info/RECORD
+10 files, 6658 bytes uncompressed, 3337 bytes compressed:  49.9%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: dump_github/main.py
 Comment: 
 
 Filename: dump_github/mylib.py
 Comment: 
 
-Filename: dump_github-0.1.6.dist-info/LICENSE
+Filename: dump_github-0.1.7.dist-info/LICENSE
 Comment: 
 
-Filename: dump_github-0.1.6.dist-info/METADATA
+Filename: dump_github-0.1.7.dist-info/METADATA
 Comment: 
 
-Filename: dump_github-0.1.6.dist-info/WHEEL
+Filename: dump_github-0.1.7.dist-info/WHEEL
 Comment: 
 
-Filename: dump_github-0.1.6.dist-info/entry_points.txt
+Filename: dump_github-0.1.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: dump_github-0.1.6.dist-info/top_level.txt
+Filename: dump_github-0.1.7.dist-info/top_level.txt
 Comment: 
 
-Filename: dump_github-0.1.6.dist-info/RECORD
+Filename: dump_github-0.1.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dump_github/lib.py

```diff
@@ -10,15 +10,15 @@
         response = requests.get(url, headers=headers)
     else:
         response = requests.get(url)
     if response.status_code == 200:
         repos = response.json()
         return repos
     else:
-        raise []
+        return []
 
 
 def serach_user_repos(username, token=""):
     page = 0
     res_repos = []
 
     while True:
```

## Comparing `dump_github-0.1.6.dist-info/LICENSE` & `dump_github-0.1.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `dump_github-0.1.6.dist-info/METADATA` & `dump_github-0.1.7.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 Metadata-Version: 2.1
 Name: dump-github
-Version: 0.1.6
+Version: 0.1.7
 Summary: This tool can be used to back up users' GitHub repositories in case they need them later.
 Home-page: https://github.com/core2002/dump_github
 Author: core2002
 Author-email: core2002@aliyun.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: argparse
 Requires-Dist: requests
 
 ### Github Dumper
 
 Github Dumper is a Python program designed to search for users' GitHub repositories and download the repositories. This tool can be used to back up users' GitHub repositories in case they need them later.
 
+**Install:**
+```
+pip install -U dump-github
+```
+
 **Usage:**
 ```
 usage: dump-github [-h] [-d] [-p] [--token TOKEN] [--limit_size LIMIT_SIZE] username
 
 Backup users github repo.
 
 positional arguments:
@@ -34,9 +38,7 @@
   -p, --print           only print urls
   --token TOKEN         github token
   --limit_size LIMIT_SIZE
                         limit size(MB) of download zip file, if 0 then no limit(default:100).
 
 https://github.com/Core2002/dump_github
 ```
-
-
```

