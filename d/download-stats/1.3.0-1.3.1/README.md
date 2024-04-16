# Comparing `tmp/download_stats-1.3.0.tar.gz` & `tmp/download_stats-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "download_stats-1.3.0.tar", last modified: Tue Jul  4 07:21:17 2023, max compression
+gzip compressed data, was "download_stats-1.3.1.tar", last modified: Tue Apr 16 11:15:30 2024, max compression
```

## Comparing `download_stats-1.3.0.tar` & `download_stats-1.3.1.tar`

### file list

```diff
@@ -1,33 +1,31 @@
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-04 07:21:17.772064 download_stats-1.3.0/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)    11357 2023-07-04 06:21:07.000000 download_stats-1.3.0/LICENSE
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      150 2023-07-04 06:21:07.000000 download_stats-1.3.0/MANIFEST.in
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     3290 2023-07-04 07:21:17.772064 download_stats-1.3.0/PKG-INFO
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     2468 2023-07-04 07:20:05.000000 download_stats-1.3.0/README.md
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-04 07:21:17.760062 download_stats-1.3.0/assets/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)    15299 2023-07-04 06:21:07.000000 download_stats-1.3.0/assets/compare.png
--rw-rw-r--   0 appinv    (1000) appinv    (1000)    68629 2023-07-04 06:21:07.000000 download_stats-1.3.0/assets/download_stats.png
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-04 07:21:17.764063 download_stats-1.3.0/reqs/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)       73 2023-07-04 06:39:03.000000 download_stats-1.3.0/reqs/app.in
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1331 2023-07-04 06:39:12.000000 download_stats-1.3.0/reqs/app.txt
--rw-rw-r--   0 appinv    (1000) appinv    (1000)       22 2023-07-04 06:21:07.000000 download_stats-1.3.0/reqs/dev.in
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1840 2023-07-04 06:21:07.000000 download_stats-1.3.0/reqs/dev.txt
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      217 2023-07-04 07:21:17.772064 download_stats-1.3.0/setup.cfg
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     3578 2023-07-04 07:20:54.000000 download_stats-1.3.0/setup.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-04 07:21:17.756062 download_stats-1.3.0/src/
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-04 07:21:17.768063 download_stats-1.3.0/src/download_stats/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      170 2023-07-04 06:21:07.000000 download_stats-1.3.0/src/download_stats/__init__.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-04 07:21:17.772064 download_stats-1.3.0/src/download_stats/__pycache__/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      397 2023-07-04 06:27:00.000000 download_stats-1.3.0/src/download_stats/__pycache__/__init__.cpython-311.pyc
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     6794 2023-07-04 07:18:03.000000 download_stats-1.3.0/src/download_stats/__pycache__/main.cpython-311.pyc
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     4428 2023-07-04 07:17:24.000000 download_stats-1.3.0/src/download_stats/__pycache__/pepy.cpython-311.pyc
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     2931 2023-07-04 06:27:00.000000 download_stats-1.3.0/src/download_stats/__pycache__/pypistats.cpython-311.pyc
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     3210 2023-07-04 07:18:00.000000 download_stats-1.3.0/src/download_stats/main.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     2487 2023-07-04 07:16:57.000000 download_stats-1.3.0/src/download_stats/pepy.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1790 2023-07-04 06:21:07.000000 download_stats-1.3.0/src/download_stats/pypistats.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-04 07:21:17.768063 download_stats-1.3.0/src/download_stats.egg-info/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     3290 2023-07-04 07:21:17.000000 download_stats-1.3.0/src/download_stats.egg-info/PKG-INFO
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      731 2023-07-04 07:21:17.000000 download_stats-1.3.0/src/download_stats.egg-info/SOURCES.txt
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        1 2023-07-04 07:21:17.000000 download_stats-1.3.0/src/download_stats.egg-info/dependency_links.txt
--rw-rw-r--   0 appinv    (1000) appinv    (1000)       61 2023-07-04 07:21:17.000000 download_stats-1.3.0/src/download_stats.egg-info/entry_points.txt
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      444 2023-07-04 07:21:17.000000 download_stats-1.3.0/src/download_stats.egg-info/requires.txt
--rw-rw-r--   0 appinv    (1000) appinv    (1000)       15 2023-07-04 07:21:17.000000 download_stats-1.3.0/src/download_stats.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:15:30.716811 download_stats-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-16 11:15:26.000000 download_stats-1.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-16 11:15:26.000000 download_stats-1.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3384 2024-04-16 11:15:30.716811 download_stats-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-16 11:15:26.000000 download_stats-1.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:15:30.716811 download_stats-1.3.1/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)    15299 2024-04-16 11:15:26.000000 download_stats-1.3.1/assets/compare.png
+-rw-r--r--   0 runner    (1001) docker     (127)    68629 2024-04-16 11:15:26.000000 download_stats-1.3.1/assets/download_stats.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:15:30.716811 download_stats-1.3.1/reqs/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-16 11:15:26.000000 download_stats-1.3.1/reqs/app.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-16 11:15:26.000000 download_stats-1.3.1/reqs/app.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-16 11:15:26.000000 download_stats-1.3.1/reqs/dev.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-16 11:15:26.000000 download_stats-1.3.1/reqs/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-16 11:15:30.720811 download_stats-1.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-04-16 11:15:26.000000 download_stats-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:15:30.712811 download_stats-1.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:15:30.716811 download_stats-1.3.1/src/download_stats/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-16 11:15:26.000000 download_stats-1.3.1/src/download_stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-04-16 11:15:26.000000 download_stats-1.3.1/src/download_stats/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-04-16 11:15:26.000000 download_stats-1.3.1/src/download_stats/pepy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-04-16 11:15:26.000000 download_stats-1.3.1/src/download_stats/pypistats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:15:30.716811 download_stats-1.3.1/src/download_stats.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3384 2024-04-16 11:15:30.000000 download_stats-1.3.1/src/download_stats.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-16 11:15:30.000000 download_stats-1.3.1/src/download_stats.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 11:15:30.000000 download_stats-1.3.1/src/download_stats.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-16 11:15:30.000000 download_stats-1.3.1/src/download_stats.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-16 11:15:30.000000 download_stats-1.3.1/src/download_stats.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-16 11:15:30.000000 download_stats-1.3.1/src/download_stats.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:15:30.716811 download_stats-1.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-16 11:15:26.000000 download_stats-1.3.1/tests/test_pepy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-16 11:15:26.000000 download_stats-1.3.1/tests/test_pypistats.py
```

### Comparing `download_stats-1.3.0/LICENSE` & `download_stats-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `download_stats-1.3.0/PKG-INFO` & `download_stats-1.3.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 Metadata-Version: 2.1
 Name: download_stats
-Version: 1.3.0
+Version: 1.3.1
 Summary: Download stats for Python packages
-Home-page: UNKNOWN
 Author-email: arj.python@gmail.com
-License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/Abdur-RahmaanJ/download-stats/issues
 Project-URL: Source, https://github.com/Abdur-RahmaanJ/download-stats/
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: rich
+Requires-Dist: selenium
+Requires-Dist: webdriver_manager>=3.8.6
+Requires-Dist: latest_user_agents>=0.0.3
+Requires-Dist: requests
 
 # download-stats
 
 View your pypi download stats
 
 # cli
 
@@ -130,8 +132,7 @@
         {"category": "Linux", "date": "2022-08-31", "downloads": 3},
     ],
     "package": "shopyo",
     "type": "system_downloads",
 }
 
 ```
-
```

### Comparing `download_stats-1.3.0/README.md` & `download_stats-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `download_stats-1.3.0/assets/compare.png` & `download_stats-1.3.1/assets/compare.png`

 * *Files identical despite different names*

### Comparing `download_stats-1.3.0/assets/download_stats.png` & `download_stats-1.3.1/assets/download_stats.png`

 * *Files identical despite different names*

### Comparing `download_stats-1.3.0/reqs/app.txt` & `download_stats-1.3.1/reqs/app.txt`

 * *Files 8% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     # via trio
 packaging==23.1
     # via webdriver-manager
 pygments==2.13.0
     # via rich
 pysocks==1.7.1
     # via urllib3
-python-dotenv==0.20.0
+python-dotenv==1.0.1
     # via webdriver-manager
 requests==2.28.1
     # via
     #   -r reqs/app.in
     #   latest-user-agents
     #   webdriver-manager
 rich==12.5.1
```

### Comparing `download_stats-1.3.0/reqs/dev.txt` & `download_stats-1.3.1/reqs/dev.txt`

 * *Files identical despite different names*

### Comparing `download_stats-1.3.0/setup.py` & `download_stats-1.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 
 # Get the long description from the README file
 with open(os.path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 setup(
     name="download_stats",  # Required
-    version="1.3.0",  # Required
+    version="1.3.1",  # Required
     description="Download stats for Python packages",  # Optional
     long_description=long_description,  # Optional
     long_description_content_type="text/markdown",  # Optional (see note above)
     # url="https://github.com/Abdur-RahmaanJ/greenBerry",  # Optional
     # author="Abdur-Rahmaan Janhangeer & contributors",  # Optional
     author_email="arj.python@gmail.com",  # Optional
     # Classifiers help users find your project by categorizing it.
@@ -75,15 +75,15 @@
     #
     # packages=find_packages(exclude=['contrib', 'docs', 'tests']),  # Required
     python_requires=">=3.7",
     include_package_data=True,
     # install_requires=open(os.path.join(here, "reqs", "app.txt"), encoding="utf-8")
     # .read()
     # .split("\n"),  # Optional
-    install_requires=open(os.path.join(here, "reqs", "app.txt"), encoding="utf-8")
+    install_requires=open(os.path.join(here, "reqs", "app.in"), encoding="utf-8")
         .read()
         .split("\n"),
     # extras_require={
     #     "dev": open(os.path.join(here, "reqs", "dev.txt"), encoding="utf-8")
     #     .read()
     #     .split("\n"),
     # },
```

### Comparing `download_stats-1.3.0/src/download_stats/main.py` & `download_stats-1.3.1/src/download_stats/main.py`

 * *Files identical despite different names*

### Comparing `download_stats-1.3.0/src/download_stats/pepy.py` & `download_stats-1.3.1/src/download_stats/pepy.py`

 * *Files identical despite different names*

### Comparing `download_stats-1.3.0/src/download_stats/pypistats.py` & `download_stats-1.3.1/src/download_stats/pypistats.py`

 * *Files identical despite different names*

### Comparing `download_stats-1.3.0/src/download_stats.egg-info/PKG-INFO` & `download_stats-1.3.1/src/download_stats.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 Metadata-Version: 2.1
-Name: download-stats
-Version: 1.3.0
+Name: download_stats
+Version: 1.3.1
 Summary: Download stats for Python packages
-Home-page: UNKNOWN
 Author-email: arj.python@gmail.com
-License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/Abdur-RahmaanJ/download-stats/issues
 Project-URL: Source, https://github.com/Abdur-RahmaanJ/download-stats/
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: rich
+Requires-Dist: selenium
+Requires-Dist: webdriver_manager>=3.8.6
+Requires-Dist: latest_user_agents>=0.0.3
+Requires-Dist: requests
 
 # download-stats
 
 View your pypi download stats
 
 # cli
 
@@ -130,8 +132,7 @@
         {"category": "Linux", "date": "2022-08-31", "downloads": 3},
     ],
     "package": "shopyo",
     "type": "system_downloads",
 }
 
 ```
-
```

### Comparing `download_stats-1.3.0/src/download_stats.egg-info/SOURCES.txt` & `download_stats-1.3.1/src/download_stats.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -15,11 +15,9 @@
 src/download_stats/pypistats.py
 src/download_stats.egg-info/PKG-INFO
 src/download_stats.egg-info/SOURCES.txt
 src/download_stats.egg-info/dependency_links.txt
 src/download_stats.egg-info/entry_points.txt
 src/download_stats.egg-info/requires.txt
 src/download_stats.egg-info/top_level.txt
-src/download_stats/__pycache__/__init__.cpython-311.pyc
-src/download_stats/__pycache__/main.cpython-311.pyc
-src/download_stats/__pycache__/pepy.cpython-311.pyc
-src/download_stats/__pycache__/pypistats.cpython-311.pyc
+tests/test_pepy.py
+tests/test_pypistats.py
```

