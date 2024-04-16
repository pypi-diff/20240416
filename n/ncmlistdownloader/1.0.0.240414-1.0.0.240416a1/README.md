# Comparing `tmp/ncmlistdownloader-1.0.0.240414.tar.gz` & `tmp/ncmlistdownloader-1.0.0.240416a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ncmlistdownloader-1.0.0.240414.tar", last modified: Sun Apr 14 14:46:02 2024, max compression
+gzip compressed data, was "ncmlistdownloader-1.0.0.240416a1.tar", last modified: Tue Apr 16 14:58:22 2024, max compression
```

## Comparing `ncmlistdownloader-1.0.0.240414.tar` & `ncmlistdownloader-1.0.0.240416a1.tar`

### file list

```diff
@@ -1,30 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-04-14 14:46:02.837665 ncmlistdownloader-1.0.0.240414/
--rw-rw-rw-   0        0        0    35181 2024-03-07 09:37:50.000000 ncmlistdownloader-1.0.0.240414/LICENSE
--rw-rw-rw-   0        0        0     1409 2024-04-14 14:46:02.822032 ncmlistdownloader-1.0.0.240414/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-14 14:46:02.784289 ncmlistdownloader-1.0.0.240414/ncmlistdownloader/
--rw-rw-rw-   0        0        0     1263 2024-04-14 14:42:21.000000 ncmlistdownloader-1.0.0.240414/ncmlistdownloader/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-14 14:46:02.799906 ncmlistdownloader-1.0.0.240414/ncmlistdownloader/cmd/
--rw-rw-rw-   0        0        0        0 2024-04-13 04:27:21.000000 ncmlistdownloader-1.0.0.240414/ncmlistdownloader/cmd/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-13 04:27:37.000000 ncmlistdownloader-1.0.0.240414/ncmlistdownloader/cmd/module.py
-drwxrwxrwx   0        0        0        0 2024-04-14 14:46:02.822032 ncmlistdownloader-1.0.0.240414/ncmlistdownloader/common/
--rw-rw-rw-   0        0        0     2859 2024-04-10 14:43:02.000000 ncmlistdownloader-1.0.0.240414/ncmlistdownloader/common/__init__.py
--rw-rw-rw-   0        0        0     2325 2024-04-14 14:36:25.000000 ncmlistdownloader-1.0.0.240414/ncmlistdownloader/common/encode_sec_key.py
--rw-rw-rw-   0        0        0     2184 2024-04-14 14:42:02.000000 ncmlistdownloader-1.0.0.240414/ncmlistdownloader/common/global_args.py
--rw-rw-rw-   0        0        0     1784 2024-04-06 14:26:30.000000 ncmlistdownloader-1.0.0.240414/ncmlistdownloader/common/thread_test.py
-drwxrwxrwx   0        0        0        0 2024-04-14 14:46:02.822032 ncmlistdownloader-1.0.0.240414/ncmlistdownloader/downloader/
--rw-rw-rw-   0        0        0     6526 2024-04-06 14:26:30.000000 ncmlistdownloader-1.0.0.240414/ncmlistdownloader/downloader/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-14 14:46:02.822032 ncmlistdownloader-1.0.0.240414/ncmlistdownloader/editer/
--rw-rw-rw-   0        0        0     3929 2024-04-06 14:26:30.000000 ncmlistdownloader-1.0.0.240414/ncmlistdownloader/editer/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-14 14:46:02.822032 ncmlistdownloader-1.0.0.240414/ncmlistdownloader/playlist/
--rw-rw-rw-   0        0        0     1956 2024-04-14 14:42:29.000000 ncmlistdownloader-1.0.0.240414/ncmlistdownloader/playlist/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-14 14:46:02.822032 ncmlistdownloader-1.0.0.240414/ncmlistdownloader/song/
--rw-rw-rw-   0        0        0     7481 2024-04-12 15:08:55.000000 ncmlistdownloader-1.0.0.240414/ncmlistdownloader/song/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-14 14:46:02.822032 ncmlistdownloader-1.0.0.240414/ncmlistdownloader.egg-info/
--rw-rw-rw-   0        0        0     1409 2024-04-14 14:46:02.000000 ncmlistdownloader-1.0.0.240414/ncmlistdownloader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      672 2024-04-14 14:46:02.000000 ncmlistdownloader-1.0.0.240414/ncmlistdownloader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-14 14:46:02.000000 ncmlistdownloader-1.0.0.240414/ncmlistdownloader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2024-04-14 14:46:02.000000 ncmlistdownloader-1.0.0.240414/ncmlistdownloader.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       37 2024-04-14 14:46:02.000000 ncmlistdownloader-1.0.0.240414/ncmlistdownloader.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-14 14:46:02.000000 ncmlistdownloader-1.0.0.240414/ncmlistdownloader.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-14 14:46:02.837665 ncmlistdownloader-1.0.0.240414/setup.cfg
--rw-rw-rw-   0        0        0     1756 2024-04-14 14:39:59.000000 ncmlistdownloader-1.0.0.240414/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 14:58:22.168530 ncmlistdownloader-1.0.0.240416a1/
+-rw-rw-rw-   0        0        0    35181 2024-03-07 09:37:50.000000 ncmlistdownloader-1.0.0.240416a1/LICENSE
+-rw-rw-rw-   0        0        0     1399 2024-04-16 14:58:22.164530 ncmlistdownloader-1.0.0.240416a1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-16 14:58:22.106611 ncmlistdownloader-1.0.0.240416a1/ncmlistdownloader/
+-rw-rw-rw-   0        0        0     1263 2024-04-14 14:42:21.000000 ncmlistdownloader-1.0.0.240416a1/ncmlistdownloader/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 14:58:22.129037 ncmlistdownloader-1.0.0.240416a1/ncmlistdownloader/cmd/
+-rw-rw-rw-   0        0        0     2373 2024-04-16 14:56:43.000000 ncmlistdownloader-1.0.0.240416a1/ncmlistdownloader/cmd/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 14:58:22.142589 ncmlistdownloader-1.0.0.240416a1/ncmlistdownloader/common/
+-rw-rw-rw-   0        0        0     2859 2024-04-10 14:43:02.000000 ncmlistdownloader-1.0.0.240416a1/ncmlistdownloader/common/__init__.py
+-rw-rw-rw-   0        0        0     2325 2024-04-14 14:36:25.000000 ncmlistdownloader-1.0.0.240416a1/ncmlistdownloader/common/encode_sec_key.py
+-rw-rw-rw-   0        0        0     2184 2024-04-14 14:42:02.000000 ncmlistdownloader-1.0.0.240416a1/ncmlistdownloader/common/global_args.py
+-rw-rw-rw-   0        0        0     1784 2024-04-06 14:26:30.000000 ncmlistdownloader-1.0.0.240416a1/ncmlistdownloader/common/thread_test.py
+drwxrwxrwx   0        0        0        0 2024-04-16 14:58:22.145610 ncmlistdownloader-1.0.0.240416a1/ncmlistdownloader/downloader/
+-rw-rw-rw-   0        0        0     6526 2024-04-06 14:26:30.000000 ncmlistdownloader-1.0.0.240416a1/ncmlistdownloader/downloader/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 14:58:22.151568 ncmlistdownloader-1.0.0.240416a1/ncmlistdownloader/editer/
+-rw-rw-rw-   0        0        0     3929 2024-04-06 14:26:30.000000 ncmlistdownloader-1.0.0.240416a1/ncmlistdownloader/editer/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 14:58:22.155554 ncmlistdownloader-1.0.0.240416a1/ncmlistdownloader/playlist/
+-rw-rw-rw-   0        0        0     2145 2024-04-16 14:56:43.000000 ncmlistdownloader-1.0.0.240416a1/ncmlistdownloader/playlist/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 14:58:22.158556 ncmlistdownloader-1.0.0.240416a1/ncmlistdownloader/song/
+-rw-rw-rw-   0        0        0     7481 2024-04-12 15:08:55.000000 ncmlistdownloader-1.0.0.240416a1/ncmlistdownloader/song/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 14:58:22.162541 ncmlistdownloader-1.0.0.240416a1/ncmlistdownloader.egg-info/
+-rw-rw-rw-   0        0        0     1399 2024-04-16 14:58:22.000000 ncmlistdownloader-1.0.0.240416a1/ncmlistdownloader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      640 2024-04-16 14:58:22.000000 ncmlistdownloader-1.0.0.240416a1/ncmlistdownloader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 14:58:22.000000 ncmlistdownloader-1.0.0.240416a1/ncmlistdownloader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2024-04-16 14:58:22.000000 ncmlistdownloader-1.0.0.240416a1/ncmlistdownloader.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       37 2024-04-16 14:58:22.000000 ncmlistdownloader-1.0.0.240416a1/ncmlistdownloader.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-16 14:58:22.000000 ncmlistdownloader-1.0.0.240416a1/ncmlistdownloader.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-16 14:58:22.169519 ncmlistdownloader-1.0.0.240416a1/setup.cfg
+-rw-rw-rw-   0        0        0     1758 2024-04-16 14:58:11.000000 ncmlistdownloader-1.0.0.240416a1/setup.py
```

### Comparing `ncmlistdownloader-1.0.0.240414/LICENSE` & `ncmlistdownloader-1.0.0.240416a1/LICENSE`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.0.240414/PKG-INFO` & `ncmlistdownloader-1.0.0.240416a1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: ncmlistdownloader
-Version: 1.0.0.240414
+Version: 1.0.0.240416a1
 Summary: 获取网易云音乐歌单数据，下载音乐，主动添加元信息。
 Home-page: https://gitee.com/Cooooldwind/163ListDownloader_NexT
 Author: CooooldWind_
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Customer Service
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: Communications :: File Sharing
 Classifier: Topic :: Internet
 Classifier: Topic :: Multimedia
 Classifier: Topic :: Multimedia :: Graphics
```

### Comparing `ncmlistdownloader-1.0.0.240414/ncmlistdownloader/__init__.py` & `ncmlistdownloader-1.0.0.240416a1/ncmlistdownloader/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.0.240414/ncmlistdownloader/common/__init__.py` & `ncmlistdownloader-1.0.0.240416a1/ncmlistdownloader/common/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.0.240414/ncmlistdownloader/common/encode_sec_key.py` & `ncmlistdownloader-1.0.0.240416a1/ncmlistdownloader/common/encode_sec_key.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.0.240414/ncmlistdownloader/common/global_args.py` & `ncmlistdownloader-1.0.0.240416a1/ncmlistdownloader/common/global_args.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.0.240414/ncmlistdownloader/common/thread_test.py` & `ncmlistdownloader-1.0.0.240416a1/ncmlistdownloader/common/thread_test.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.0.240414/ncmlistdownloader/downloader/__init__.py` & `ncmlistdownloader-1.0.0.240416a1/ncmlistdownloader/downloader/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.0.240414/ncmlistdownloader/editer/__init__.py` & `ncmlistdownloader-1.0.0.240416a1/ncmlistdownloader/editer/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.0.240414/ncmlistdownloader/playlist/__init__.py` & `ncmlistdownloader-1.0.0.240416a1/ncmlistdownloader/playlist/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 '''
 ncmlistdownloader/playlist/__init__.py
-Core.Ver.1.0.0.240414
+Core.Ver.1.0.0.240416a1
 Author: CooooldWind_
 '''
 from ncmlistdownloader.common import *
 from ncmlistdownloader.common.encode_sec_key import *
 from ncmlistdownloader.common.global_args import *
 from ncmlistdownloader.song import *
 import threading
@@ -23,35 +23,38 @@
         self.title = ""
 
     def get_info(self, cookies = None):
         self.raw_info = NeteaseParams(url = PLAYLIST_API,
                                       encode_data = {
                                           'csrf_token': '',
                                           'id': self.id,
-                                      }).get_resource(cookies = cookies)['playlist']
-        self.creator_id = self.raw_info['userId']
-        self.track_count = self.raw_info['trackCount']
-        self.creator = self.raw_info['creator']['nickname']
-        self.title = self.raw_info['name']
-        for i in self.raw_info['trackIds']:
+                                      }).get_resource(cookies = cookies)
+        if self.raw_info['code'] != 200:
+            return -1
+        self.creator_id = self.raw_info['playlist']['userId']
+        self.track_count = self.raw_info['playlist']['trackCount']
+        self.creator = self.raw_info['playlist']['creator']['nickname']
+        self.title = self.raw_info['playlist']['name']
+        for i in self.raw_info['playlist']['trackIds']:
             self.track_id.append(str(i['id']))
         for truck_id in self.track_id:
             self.track.append(Song(id = truck_id))
         return self.raw_info
     
     def get_detail_info(self):
         threads: list[threading.Thread] = []
         for i in self.track:
             thread = threading.Thread(target = i.multi_get_info)
             thread.start()
             threads.append(thread)
 
-    def auto_get_info(self):
-        self.get_info()
-        self.get_detail_info()
+    def auto_get_info(self, cookies = dict()):
+        if self.get_info(cookies = cookies) != -1:
+            self.get_detail_info()
+        else: return -1
 
     def done_sum(self):
         count = 0
         for i in self.track:
             if i.is_get == True:
                 count += 1
         return count
```

### Comparing `ncmlistdownloader-1.0.0.240414/ncmlistdownloader/song/__init__.py` & `ncmlistdownloader-1.0.0.240416a1/ncmlistdownloader/song/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.0.240414/ncmlistdownloader.egg-info/PKG-INFO` & `ncmlistdownloader-1.0.0.240416a1/ncmlistdownloader.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: ncmlistdownloader
-Version: 1.0.0.240414
+Version: 1.0.0.240416a1
 Summary: 获取网易云音乐歌单数据，下载音乐，主动添加元信息。
 Home-page: https://gitee.com/Cooooldwind/163ListDownloader_NexT
 Author: CooooldWind_
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Customer Service
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: Communications :: File Sharing
 Classifier: Topic :: Internet
 Classifier: Topic :: Multimedia
 Classifier: Topic :: Multimedia :: Graphics
```

### Comparing `ncmlistdownloader-1.0.0.240414/ncmlistdownloader.egg-info/SOURCES.txt` & `ncmlistdownloader-1.0.0.240416a1/ncmlistdownloader.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 ncmlistdownloader.egg-info/PKG-INFO
 ncmlistdownloader.egg-info/SOURCES.txt
 ncmlistdownloader.egg-info/dependency_links.txt
 ncmlistdownloader.egg-info/entry_points.txt
 ncmlistdownloader.egg-info/requires.txt
 ncmlistdownloader.egg-info/top_level.txt
 ncmlistdownloader/cmd/__init__.py
-ncmlistdownloader/cmd/module.py
 ncmlistdownloader/common/__init__.py
 ncmlistdownloader/common/encode_sec_key.py
 ncmlistdownloader/common/global_args.py
 ncmlistdownloader/common/thread_test.py
 ncmlistdownloader/downloader/__init__.py
 ncmlistdownloader/editer/__init__.py
 ncmlistdownloader/playlist/__init__.py
```

### Comparing `ncmlistdownloader-1.0.0.240414/setup.py` & `ncmlistdownloader-1.0.0.240416a1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 setup(
     classifiers = [
         # 发展时期
-        # 'Development Status :: 3 - Alpha',
+        'Development Status :: 3 - Alpha',
         # 'Development Status :: 4 - Beta',
-        'Development Status :: 5 - Production/Stable',
+        # 'Development Status :: 5 - Production/Stable',
         # 开发的目标用户
         'Intended Audience :: Customer Service',
         'Intended Audience :: Developers',
         'Intended Audience :: End Users/Desktop',
         # 属于什么类型
         'Topic :: Communications :: File Sharing',
         'Topic :: Internet',
@@ -26,15 +26,15 @@
 		'Programming Language :: Python :: 3.8',
 		'Programming Language :: Python :: 3.9',
 		'Programming Language :: Python :: 3.10',
 		'Programming Language :: Python :: 3.11',
 		'Programming Language :: Python :: 3.12',
     ],
     name = 'ncmlistdownloader',
-    version = "1.0.0.240414",
+    version = "1.0.0.240416a1",
     description = '获取网易云音乐歌单数据，下载音乐，主动添加元信息。',
     author = 'CooooldWind_',
     url = 'https://gitee.com/Cooooldwind/163ListDownloader_NexT',
     packages = find_packages(),
     install_requires = ['pycryptodome','pillow','mutagen','requests',],
     entry_points = {'console_scripts': ['ncmlistdownloader = ncmlistdownloader.__init__:main']},
 )
```

