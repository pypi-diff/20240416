# Comparing `tmp/datakarkhana-0.0.3.tar.gz` & `tmp/datakarkhana-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datakarkhana-0.0.3.tar", last modified: Fri Apr 12 17:43:43 2024, max compression
+gzip compressed data, was "datakarkhana-0.1.0.tar", last modified: Tue Apr 16 07:21:06 2024, max compression
```

## Comparing `datakarkhana-0.0.3.tar` & `datakarkhana-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:43:43.392785 datakarkhana-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-12 17:43:39.000000 datakarkhana-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-12 17:43:43.392785 datakarkhana-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-12 17:43:39.000000 datakarkhana-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:43:43.388785 datakarkhana-0.0.3/data_karkhana/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 17:43:39.000000 datakarkhana-0.0.3/data_karkhana/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-04-12 17:43:39.000000 datakarkhana-0.0.3/data_karkhana/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-04-12 17:43:39.000000 datakarkhana-0.0.3/data_karkhana/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:43:43.388785 datakarkhana-0.0.3/datakarkhana.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-12 17:43:43.000000 datakarkhana-0.0.3/datakarkhana.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-12 17:43:43.000000 datakarkhana-0.0.3/datakarkhana.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 17:43:43.000000 datakarkhana-0.0.3/datakarkhana.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-12 17:43:43.000000 datakarkhana-0.0.3/datakarkhana.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-12 17:43:43.000000 datakarkhana-0.0.3/datakarkhana.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 17:43:43.392785 datakarkhana-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-12 17:43:39.000000 datakarkhana-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:21:06.701106 datakarkhana-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-16 07:21:01.000000 datakarkhana-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-16 07:21:06.701106 datakarkhana-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-16 07:21:01.000000 datakarkhana-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:21:06.701106 datakarkhana-0.1.0/data_karkhana/
+-rw-r--r--   0 runner    (1001) docker     (127)     4812 2024-04-16 07:21:01.000000 datakarkhana-0.1.0/data_karkhana/Downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4185 2024-04-16 07:21:01.000000 datakarkhana-0.1.0/data_karkhana/Peer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-04-16 07:21:01.000000 datakarkhana-0.1.0/data_karkhana/Tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6479 2024-04-16 07:21:01.000000 datakarkhana-0.1.0/data_karkhana/Uploader.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 07:21:01.000000 datakarkhana-0.1.0/data_karkhana/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-04-16 07:21:01.000000 datakarkhana-0.1.0/data_karkhana/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-04-16 07:21:01.000000 datakarkhana-0.1.0/data_karkhana/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:21:06.701106 datakarkhana-0.1.0/datakarkhana.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-16 07:21:06.000000 datakarkhana-0.1.0/datakarkhana.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-16 07:21:06.000000 datakarkhana-0.1.0/datakarkhana.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 07:21:06.000000 datakarkhana-0.1.0/datakarkhana.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-16 07:21:06.000000 datakarkhana-0.1.0/datakarkhana.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-16 07:21:06.000000 datakarkhana-0.1.0/datakarkhana.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 07:21:06.701106 datakarkhana-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-16 07:21:01.000000 datakarkhana-0.1.0/setup.py
```

### Comparing `datakarkhana-0.0.3/LICENSE` & `datakarkhana-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `datakarkhana-0.0.3/PKG-INFO` & `datakarkhana-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datakarkhana
-Version: 0.0.3
+Version: 0.1.0
 Summary: A peer-to-peer file sharing system
 Home-page: https://github.com/timsinashok/data_karkhana
 Author: Yaghyesh Ghimire, Manoj Dhakal, Mahmud Faisal , Ashok Timsina
 Author-email: md5121@nyu.edu, yg2810@nyu.edu, fm2357@nyu.edu, ashoktimsina147181@gmail.com
 Project-URL: Bug Reports, https://github.com/timsinashok/data_karkhana/issues
 Project-URL: Source, https://github.com/timsinashok/data_karkhana
 Keywords: peer peer-to-peer file sharing alice bob
```

### Comparing `datakarkhana-0.0.3/data_karkhana/main.py` & `datakarkhana-0.1.0/data_karkhana/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import sys
-from Users import Tracker
-from Users import Peer
-from Users import Uploader
-from Users import Downloader
+from data_karkhana.Tracker import Tracker
+from data_karkhana.Peer import FileTransferHandler
+from data_karkhana.Uploader import uploader
+from data_karkhana.Downloader import Downloader
 import socket
 
 def main():
     print("Choose a role:")
     print("1. Tracker")
     print("2. Uploader")
     print("3. Downloader")
@@ -67,8 +67,8 @@
 
 def get_ip():
     s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
     s.connect(('8.8.8.8', 1))  # connect() for UDP doesn't send packets
     return s.getsockname()[0]
 
 if __name__ == "__main__":
-    main()
+    main()
```

### Comparing `datakarkhana-0.0.3/data_karkhana/setup.py` & `datakarkhana-0.1.0/data_karkhana/setup.py`

 * *Files identical despite different names*

### Comparing `datakarkhana-0.0.3/datakarkhana.egg-info/PKG-INFO` & `datakarkhana-0.1.0/datakarkhana.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datakarkhana
-Version: 0.0.3
+Version: 0.1.0
 Summary: A peer-to-peer file sharing system
 Home-page: https://github.com/timsinashok/data_karkhana
 Author: Yaghyesh Ghimire, Manoj Dhakal, Mahmud Faisal , Ashok Timsina
 Author-email: md5121@nyu.edu, yg2810@nyu.edu, fm2357@nyu.edu, ashoktimsina147181@gmail.com
 Project-URL: Bug Reports, https://github.com/timsinashok/data_karkhana/issues
 Project-URL: Source, https://github.com/timsinashok/data_karkhana
 Keywords: peer peer-to-peer file sharing alice bob
```

### Comparing `datakarkhana-0.0.3/setup.py` & `datakarkhana-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='datakarkhana',  # Replace 'your_package' with the name of your package
-    version='0.0.3',
+    version='0.1.0',
     description='A peer-to-peer file sharing system',
     long_description='Datakarkhana is a peer-to-peer file sharing system which works on a hybrid peer-to-peer and client-server model. ',
     long_description_content_type='text/markdown',
     url='https://github.com/timsinashok/data_karkhana',  # Replace with the URL of your package repository
     author='Yaghyesh Ghimire, Manoj Dhakal, Mahmud Faisal , Ashok Timsina',  # List all authors separated by commas
     author_email='md5121@nyu.edu, yg2810@nyu.edu, fm2357@nyu.edu, ashoktimsina147181@gmail.com',  # List all author emails separated by commas
     classifiers=[
```

