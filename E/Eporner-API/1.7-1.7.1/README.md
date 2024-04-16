# Comparing `tmp/eporner_api-1.7.tar.gz` & `tmp/eporner_api-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eporner_api-1.7.tar", last modified: Tue Apr 16 07:34:19 2024, max compression
+gzip compressed data, was "eporner_api-1.7.1.tar", last modified: Tue Apr 16 21:22:43 2024, max compression
```

## Comparing `eporner_api-1.7.tar` & `eporner_api-1.7.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 asuna     (1000) asuna     (1000)        0 2024-04-16 07:34:19.314179 eporner_api-1.7/
-drwxr-xr-x   0 asuna     (1000) asuna     (1000)        0 2024-04-16 07:34:19.314179 eporner_api-1.7/Eporner_API.egg-info/
--rw-r--r--   0 asuna     (1000) asuna     (1000)     3119 2024-04-16 07:34:19.000000 eporner_api-1.7/Eporner_API.egg-info/PKG-INFO
--rw-r--r--   0 asuna     (1000) asuna     (1000)      639 2024-04-16 07:34:19.000000 eporner_api-1.7/Eporner_API.egg-info/SOURCES.txt
--rw-r--r--   0 asuna     (1000) asuna     (1000)        1 2024-04-16 07:34:19.000000 eporner_api-1.7/Eporner_API.egg-info/dependency_links.txt
--rw-r--r--   0 asuna     (1000) asuna     (1000)       61 2024-04-16 07:34:19.000000 eporner_api-1.7/Eporner_API.egg-info/entry_points.txt
--rw-r--r--   0 asuna     (1000) asuna     (1000)       31 2024-04-16 07:34:19.000000 eporner_api-1.7/Eporner_API.egg-info/requires.txt
--rw-r--r--   0 asuna     (1000) asuna     (1000)       12 2024-04-16 07:34:19.000000 eporner_api-1.7/Eporner_API.egg-info/top_level.txt
--rw-r--r--   0 asuna     (1000) asuna     (1000)     7369 2024-04-05 09:20:27.000000 eporner_api-1.7/LICENSE
--rw-r--r--   0 asuna     (1000) asuna     (1000)     3119 2024-04-16 07:34:19.314179 eporner_api-1.7/PKG-INFO
-drwxr-xr-x   0 asuna     (1000) asuna     (1000)        0 2024-04-16 07:34:19.314179 eporner_api-1.7/eporner_api/
--rw-r--r--   0 asuna     (1000) asuna     (1000)        0 2024-04-05 09:20:27.000000 eporner_api-1.7/eporner_api/__init__.py
--rw-r--r--   0 asuna     (1000) asuna     (1000)    19610 2024-04-12 11:30:57.000000 eporner_api-1.7/eporner_api/eporner_api.py
-drwxr-xr-x   0 asuna     (1000) asuna     (1000)        0 2024-04-16 07:34:19.314179 eporner_api-1.7/eporner_api/modules/
--rw-r--r--   0 asuna     (1000) asuna     (1000)        0 2024-04-05 09:20:27.000000 eporner_api-1.7/eporner_api/modules/__init__.py
--rw-r--r--   0 asuna     (1000) asuna     (1000)     2740 2024-04-05 10:22:30.000000 eporner_api-1.7/eporner_api/modules/consts.py
--rw-r--r--   0 asuna     (1000) asuna     (1000)      426 2024-04-05 13:14:22.000000 eporner_api-1.7/eporner_api/modules/errors.py
--rw-r--r--   0 asuna     (1000) asuna     (1000)     2030 2024-04-05 09:20:27.000000 eporner_api-1.7/eporner_api/modules/locals.py
--rw-r--r--   0 asuna     (1000) asuna     (1000)      643 2024-04-05 09:20:27.000000 eporner_api-1.7/eporner_api/modules/progressbar.py
--rw-r--r--   0 asuna     (1000) asuna     (1000)      492 2024-04-05 09:20:27.000000 eporner_api-1.7/eporner_api/modules/sorting.py
-drwxr-xr-x   0 asuna     (1000) asuna     (1000)        0 2024-04-16 07:34:19.314179 eporner_api-1.7/eporner_api/tests/
--rw-r--r--   0 asuna     (1000) asuna     (1000)        0 2024-04-05 09:20:27.000000 eporner_api-1.7/eporner_api/tests/__init__.py
--rw-r--r--   0 asuna     (1000) asuna     (1000)      796 2024-04-05 09:20:27.000000 eporner_api-1.7/eporner_api/tests/test_category.py
--rw-r--r--   0 asuna     (1000) asuna     (1000)     1756 2024-04-05 09:20:27.000000 eporner_api-1.7/eporner_api/tests/test_pornstar.py
--rw-r--r--   0 asuna     (1000) asuna     (1000)     2098 2024-04-05 09:20:27.000000 eporner_api-1.7/eporner_api/tests/test_search.py
--rw-r--r--   0 asuna     (1000) asuna     (1000)     2302 2024-04-05 09:20:27.000000 eporner_api-1.7/eporner_api/tests/test_video.py
--rw-r--r--   0 asuna     (1000) asuna     (1000)       38 2024-04-16 07:34:19.314179 eporner_api-1.7/setup.cfg
--rw-r--r--   0 asuna     (1000) asuna     (1000)      935 2024-04-16 07:34:16.000000 eporner_api-1.7/setup.py
+drwxr-xr-x   0 asuna     (1000) asuna     (1000)        0 2024-04-16 21:22:43.335463 eporner_api-1.7.1/
+drwxr-xr-x   0 asuna     (1000) asuna     (1000)        0 2024-04-16 21:22:43.335463 eporner_api-1.7.1/Eporner_API.egg-info/
+-rw-r--r--   0 asuna     (1000) asuna     (1000)     3121 2024-04-16 21:22:43.000000 eporner_api-1.7.1/Eporner_API.egg-info/PKG-INFO
+-rw-r--r--   0 asuna     (1000) asuna     (1000)      639 2024-04-16 21:22:43.000000 eporner_api-1.7.1/Eporner_API.egg-info/SOURCES.txt
+-rw-r--r--   0 asuna     (1000) asuna     (1000)        1 2024-04-16 21:22:43.000000 eporner_api-1.7.1/Eporner_API.egg-info/dependency_links.txt
+-rw-r--r--   0 asuna     (1000) asuna     (1000)       61 2024-04-16 21:22:43.000000 eporner_api-1.7.1/Eporner_API.egg-info/entry_points.txt
+-rw-r--r--   0 asuna     (1000) asuna     (1000)       31 2024-04-16 21:22:43.000000 eporner_api-1.7.1/Eporner_API.egg-info/requires.txt
+-rw-r--r--   0 asuna     (1000) asuna     (1000)       12 2024-04-16 21:22:43.000000 eporner_api-1.7.1/Eporner_API.egg-info/top_level.txt
+-rw-r--r--   0 asuna     (1000) asuna     (1000)     7369 2024-02-08 15:55:11.000000 eporner_api-1.7.1/LICENSE
+-rw-r--r--   0 asuna     (1000) asuna     (1000)     3121 2024-04-16 21:22:43.335463 eporner_api-1.7.1/PKG-INFO
+drwxr-xr-x   0 asuna     (1000) asuna     (1000)        0 2024-04-16 21:22:43.335463 eporner_api-1.7.1/eporner_api/
+-rw-r--r--   0 asuna     (1000) asuna     (1000)        0 2024-02-08 15:55:11.000000 eporner_api-1.7.1/eporner_api/__init__.py
+-rw-r--r--   0 asuna     (1000) asuna     (1000)    19664 2024-04-16 21:21:18.000000 eporner_api-1.7.1/eporner_api/eporner_api.py
+drwxr-xr-x   0 asuna     (1000) asuna     (1000)        0 2024-04-16 21:22:43.335463 eporner_api-1.7.1/eporner_api/modules/
+-rw-r--r--   0 asuna     (1000) asuna     (1000)        0 2024-02-08 15:55:11.000000 eporner_api-1.7.1/eporner_api/modules/__init__.py
+-rw-r--r--   0 asuna     (1000) asuna     (1000)     2740 2024-04-13 18:47:33.000000 eporner_api-1.7.1/eporner_api/modules/consts.py
+-rw-r--r--   0 asuna     (1000) asuna     (1000)      426 2024-04-13 18:47:33.000000 eporner_api-1.7.1/eporner_api/modules/errors.py
+-rw-r--r--   0 asuna     (1000) asuna     (1000)     2030 2024-02-29 15:50:16.000000 eporner_api-1.7.1/eporner_api/modules/locals.py
+-rw-r--r--   0 asuna     (1000) asuna     (1000)      643 2024-02-08 15:55:11.000000 eporner_api-1.7.1/eporner_api/modules/progressbar.py
+-rw-r--r--   0 asuna     (1000) asuna     (1000)      492 2024-02-08 15:55:11.000000 eporner_api-1.7.1/eporner_api/modules/sorting.py
+drwxr-xr-x   0 asuna     (1000) asuna     (1000)        0 2024-04-16 21:22:43.335463 eporner_api-1.7.1/eporner_api/tests/
+-rw-r--r--   0 asuna     (1000) asuna     (1000)        0 2024-02-08 15:55:11.000000 eporner_api-1.7.1/eporner_api/tests/__init__.py
+-rw-r--r--   0 asuna     (1000) asuna     (1000)      796 2024-02-10 12:39:15.000000 eporner_api-1.7.1/eporner_api/tests/test_category.py
+-rw-r--r--   0 asuna     (1000) asuna     (1000)     1756 2024-02-16 12:52:56.000000 eporner_api-1.7.1/eporner_api/tests/test_pornstar.py
+-rw-r--r--   0 asuna     (1000) asuna     (1000)     2098 2024-02-08 15:55:11.000000 eporner_api-1.7.1/eporner_api/tests/test_search.py
+-rw-r--r--   0 asuna     (1000) asuna     (1000)     2302 2024-02-10 12:42:57.000000 eporner_api-1.7.1/eporner_api/tests/test_video.py
+-rw-r--r--   0 asuna     (1000) asuna     (1000)       38 2024-04-16 21:22:43.335463 eporner_api-1.7.1/setup.cfg
+-rw-r--r--   0 asuna     (1000) asuna     (1000)      937 2024-04-16 21:22:38.000000 eporner_api-1.7.1/setup.py
```

### Comparing `eporner_api-1.7/Eporner_API.egg-info/PKG-INFO` & `eporner_api-1.7.1/Eporner_API.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Eporner_API
-Version: 1.7
+Version: 1.7.1
 Summary: A Python API for the Porn Site Eporner.com
 Home-page: https://github.com/EchterAlsFake/EPorner_API
 Author: Johannes Habel
 Author-email: EchterAlsFake@proton.me
 License: LGPLv3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: Eporner_API Version: 1.7 Summary: A Python API for
-the Porn Site Eporner.com Home-page: https://github.com/EchterAlsFake/
+Metadata-Version: 2.1 Name: Eporner_API Version: 1.7.1 Summary: A Python API
+for the Porn Site Eporner.com Home-page: https://github.com/EchterAlsFake/
 EPorner_API Author: Johannes Habel Author-email: EchterAlsFake@proton.me
 License: LGPLv3 Classifier: License :: OSI Approved :: GNU Lesser General
 Public License v3 (LGPLv3) Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 requests Requires-Dist: bs4 Requires-Dist: lxml Requires-Dist: eaf_base_api
                            ************ EEPPoorrnneerr AAPPII ************
                     _[_D_o_w_n_l_o_a_d_s_]_[_C_o_d_e_Q_L_ _A_n_a_l_y_s_i_s_]_[_A_P_I_ _T_e_s_t_s_]
```

### Comparing `eporner_api-1.7/Eporner_API.egg-info/SOURCES.txt` & `eporner_api-1.7.1/Eporner_API.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eporner_api-1.7/LICENSE` & `eporner_api-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `eporner_api-1.7/PKG-INFO` & `eporner_api-1.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Eporner_API
-Version: 1.7
+Version: 1.7.1
 Summary: A Python API for the Porn Site Eporner.com
 Home-page: https://github.com/EchterAlsFake/EPorner_API
 Author: Johannes Habel
 Author-email: EchterAlsFake@proton.me
 License: LGPLv3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: Eporner_API Version: 1.7 Summary: A Python API for
-the Porn Site Eporner.com Home-page: https://github.com/EchterAlsFake/
+Metadata-Version: 2.1 Name: Eporner_API Version: 1.7.1 Summary: A Python API
+for the Porn Site Eporner.com Home-page: https://github.com/EchterAlsFake/
 EPorner_API Author: Johannes Habel Author-email: EchterAlsFake@proton.me
 License: LGPLv3 Classifier: License :: OSI Approved :: GNU Lesser General
 Public License v3 (LGPLv3) Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 requests Requires-Dist: bs4 Requires-Dist: lxml Requires-Dist: eaf_base_api
                            ************ EEPPoorrnneerr AAPPII ************
                     _[_D_o_w_n_l_o_a_d_s_]_[_C_o_d_e_Q_L_ _A_n_a_l_y_s_i_s_]_[_A_P_I_ _T_e_s_t_s_]
```

### Comparing `eporner_api-1.7/eporner_api/eporner_api.py` & `eporner_api-1.7.1/eporner_api/eporner_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -547,27 +547,27 @@
     parser.add_argument("--use-title", metavar="True,False", type=bool,
                         help="Whether to apply video title automatically to output path or not", required=True)
 
     args = parser.parse_args()
 
     if args.download:
         client = Client()
-        video = client.get_video(args.download)
+        video = client.get_video(args.download, enable_html_scraping=True)
         path = Core().return_path(args=args, video=video)
         video.download(quality=args.quality, path=path)
 
     if args.file:
         videos = []
         client = Client()
 
         with open(args.file, "r") as file:
             content = file.read().splitlines()
 
         for url in content:
-            videos.append(client.get_video(url))
+            videos.append(client.get_video(url, enable_html_scraping=True))
 
         for video in videos:
             path = Core().return_path(args=args, video=video)
             video.download(quality=args.quality, path=path)
 
 
 if __name__ == "__main__":
```

### Comparing `eporner_api-1.7/eporner_api/modules/consts.py` & `eporner_api-1.7.1/eporner_api/modules/consts.py`

 * *Files identical despite different names*

### Comparing `eporner_api-1.7/eporner_api/modules/locals.py` & `eporner_api-1.7.1/eporner_api/modules/locals.py`

 * *Files identical despite different names*

### Comparing `eporner_api-1.7/eporner_api/modules/progressbar.py` & `eporner_api-1.7.1/eporner_api/modules/progressbar.py`

 * *Files identical despite different names*

### Comparing `eporner_api-1.7/eporner_api/tests/test_category.py` & `eporner_api-1.7.1/eporner_api/tests/test_category.py`

 * *Files identical despite different names*

### Comparing `eporner_api-1.7/eporner_api/tests/test_pornstar.py` & `eporner_api-1.7.1/eporner_api/tests/test_pornstar.py`

 * *Files identical despite different names*

### Comparing `eporner_api-1.7/eporner_api/tests/test_search.py` & `eporner_api-1.7.1/eporner_api/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `eporner_api-1.7/eporner_api/tests/test_video.py` & `eporner_api-1.7.1/eporner_api/tests/test_video.py`

 * *Files identical despite different names*

### Comparing `eporner_api-1.7/setup.py` & `eporner_api-1.7.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="Eporner_API",
-    version="1.7",
+    version="1.7.1",
     packages=find_packages(),
     install_requires=[
         "requests", "bs4", "lxml", "eaf_base_api"
     ],
     entry_points={
         'console_scripts': ['eporner_api=eporner_api.eporner_api:main'
             # If you want to create any executable scripts
```

