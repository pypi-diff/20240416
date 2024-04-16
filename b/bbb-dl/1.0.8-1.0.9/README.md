# Comparing `tmp/bbb-dl-1.0.8.tar.gz` & `tmp/bbb-dl-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bbb-dl-1.0.8.tar", last modified: Sun Dec 10 07:46:44 2023, max compression
+gzip compressed data, was "bbb-dl-1.0.9.tar", last modified: Fri Mar 29 09:03:51 2024, max compression
```

## Comparing `bbb-dl-1.0.8.tar` & `bbb-dl-1.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 07:46:44.618140 bbb-dl-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)      421 2023-12-10 07:46:36.000000 bbb-dl-1.0.8/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2023-12-10 07:46:36.000000 bbb-dl-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10249 2023-12-10 07:46:44.618140 bbb-dl-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9360 2023-12-10 07:46:36.000000 bbb-dl-1.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 07:46:44.618140 bbb-dl-1.0.8/bbb_dl/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-10 07:46:36.000000 bbb-dl-1.0.8/bbb_dl/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11835 2023-12-10 07:46:36.000000 bbb-dl-1.0.8/bbb_dl/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)    10969 2023-12-10 07:46:36.000000 bbb-dl-1.0.8/bbb_dl/ffmpeg.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    58937 2023-12-10 07:46:36.000000 bbb-dl-1.0.8/bbb_dl/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    20968 2023-12-10 07:46:36.000000 bbb-dl-1.0.8/bbb_dl/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-12-10 07:46:36.000000 bbb-dl-1.0.8/bbb_dl/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 07:46:44.618140 bbb-dl-1.0.8/bbb_dl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10249 2023-12-10 07:46:44.000000 bbb-dl-1.0.8/bbb_dl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      361 2023-12-10 07:46:44.000000 bbb-dl-1.0.8/bbb_dl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-10 07:46:44.000000 bbb-dl-1.0.8/bbb_dl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       77 2023-12-10 07:46:44.000000 bbb-dl-1.0.8/bbb_dl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-10 07:46:44.000000 bbb-dl-1.0.8/bbb_dl.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       89 2023-12-10 07:46:44.000000 bbb-dl-1.0.8/bbb_dl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-12-10 07:46:44.000000 bbb-dl-1.0.8/bbb_dl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      121 2023-12-10 07:46:36.000000 bbb-dl-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-10 07:46:44.618140 bbb-dl-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2023-12-10 07:46:36.000000 bbb-dl-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 09:03:51.396159 bbb-dl-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-03-29 09:03:43.000000 bbb-dl-1.0.9/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-03-29 09:03:43.000000 bbb-dl-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11052 2024-03-29 09:03:51.396159 bbb-dl-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10163 2024-03-29 09:03:43.000000 bbb-dl-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 09:03:51.392159 bbb-dl-1.0.9/bbb_dl/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 09:03:43.000000 bbb-dl-1.0.9/bbb_dl/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11835 2024-03-29 09:03:43.000000 bbb-dl-1.0.9/bbb_dl/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10969 2024-03-29 09:03:43.000000 bbb-dl-1.0.9/bbb_dl/ffmpeg.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    58937 2024-03-29 09:03:43.000000 bbb-dl-1.0.9/bbb_dl/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20968 2024-03-29 09:03:43.000000 bbb-dl-1.0.9/bbb_dl/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-29 09:03:43.000000 bbb-dl-1.0.9/bbb_dl/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 09:03:51.396159 bbb-dl-1.0.9/bbb_dl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11052 2024-03-29 09:03:51.000000 bbb-dl-1.0.9/bbb_dl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-03-29 09:03:51.000000 bbb-dl-1.0.9/bbb_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 09:03:51.000000 bbb-dl-1.0.9/bbb_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-29 09:03:51.000000 bbb-dl-1.0.9/bbb_dl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 09:03:51.000000 bbb-dl-1.0.9/bbb_dl.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-29 09:03:51.000000 bbb-dl-1.0.9/bbb_dl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-29 09:03:51.000000 bbb-dl-1.0.9/bbb_dl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-03-29 09:03:43.000000 bbb-dl-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 09:03:51.396159 bbb-dl-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-03-29 09:03:43.000000 bbb-dl-1.0.9/setup.py
```

### Comparing `bbb-dl-1.0.8/LICENSE` & `bbb-dl-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bbb-dl-1.0.8/PKG-INFO` & `bbb-dl-1.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbb-dl
-Version: 1.0.8
+Version: 1.0.9
 Summary: Big Blue Button Downloader that downloads a BBB lesson as MP4 video
 Home-page: https://github.com/C0D3D3V/bbb-dl
 Author: C0D3D3V
 License: GPL-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
@@ -18,15 +18,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
 Requires-Dist: aiofiles>=22.1.0
 Requires-Dist: aiohttp>=3.8.3
 Requires-Dist: colorama>=0.4.6
 Requires-Dist: playwright>=1.29.0
-Requires-Dist: python-ffmpeg>=1.0.16
+Requires-Dist: python-ffmpeg>=2.0.10
 
 # Big Blue Button (BBB) Downloader
 
 Downloads a BBB lesson as MP4 video.
 The assembled video includes:
 
 - shared audio and webcams video
@@ -44,14 +44,27 @@
 3. Run: `pip install --user bbb-dl`
 4. Run `playwright install chromium`
 
 5. Run `bbb-dl --help` to see all options
 
 If you ever need to update `bbb-dl` run: `pip install -U bbb-dl`
 
+#### Alternatively use an virtual enviroment
+
+1. Install [Python](https://www.python.org/) >=3.7 and [git](https://git-scm.com/downloads)
+2. Install  `virtualenv`: `pip install virtualenv`
+3. Create a directory where you wish to install ebsco-dl. Open a terminal in the desired directory
+4. Clone this repository into that folder: `git clone https://github.com/C0D3D3V/bbb-dl.git .`
+5. Run `virtualenv venv` to create the virtual environment (on Windows use `venv\Scripts\activate`)
+6. Run `source venv/bin/activate` to activate the virtual environment (on Windows use `venv\Scripts\activate`)
+7. Install `bbb-dl`: `pip install .`
+8. Install [ffmpeg](https://github.com/C0D3D3V/Moodle-Downloader-2/wiki/Installing-ffmpeg)
+9. Run `playwright install chromium`
+10. Run `bbb-dl --help` to see all options
+
 ### Usage
 
 **Temporary files are default stored in the application data folder** 
 
 - The `--backup` option uses the same location
 - You can change this location with the `--working-dir` option
 - On Windows, the folder is located in `%localappdata%\bbb-dl`
```

### Comparing `bbb-dl-1.0.8/README.md` & `bbb-dl-1.0.9/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -18,14 +18,27 @@
 3. Run: `pip install --user bbb-dl`
 4. Run `playwright install chromium`
 
 5. Run `bbb-dl --help` to see all options
 
 If you ever need to update `bbb-dl` run: `pip install -U bbb-dl`
 
+#### Alternatively use an virtual enviroment
+
+1. Install [Python](https://www.python.org/) >=3.7 and [git](https://git-scm.com/downloads)
+2. Install  `virtualenv`: `pip install virtualenv`
+3. Create a directory where you wish to install ebsco-dl. Open a terminal in the desired directory
+4. Clone this repository into that folder: `git clone https://github.com/C0D3D3V/bbb-dl.git .`
+5. Run `virtualenv venv` to create the virtual environment (on Windows use `venv\Scripts\activate`)
+6. Run `source venv/bin/activate` to activate the virtual environment (on Windows use `venv\Scripts\activate`)
+7. Install `bbb-dl`: `pip install .`
+8. Install [ffmpeg](https://github.com/C0D3D3V/Moodle-Downloader-2/wiki/Installing-ffmpeg)
+9. Run `playwright install chromium`
+10. Run `bbb-dl --help` to see all options
+
 ### Usage
 
 **Temporary files are default stored in the application data folder** 
 
 - The `--backup` option uses the same location
 - You can change this location with the `--working-dir` option
 - On Windows, the folder is located in `%localappdata%\bbb-dl`
```

### Comparing `bbb-dl-1.0.8/bbb_dl/batch.py` & `bbb-dl-1.0.9/bbb_dl/batch.py`

 * *Files identical despite different names*

### Comparing `bbb-dl-1.0.8/bbb_dl/ffmpeg.py` & `bbb-dl-1.0.9/bbb_dl/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `bbb-dl-1.0.8/bbb_dl/main.py` & `bbb-dl-1.0.9/bbb_dl/main.py`

 * *Files identical despite different names*

### Comparing `bbb-dl-1.0.8/bbb_dl/utils.py` & `bbb-dl-1.0.9/bbb_dl/utils.py`

 * *Files identical despite different names*

### Comparing `bbb-dl-1.0.8/bbb_dl.egg-info/PKG-INFO` & `bbb-dl-1.0.9/bbb_dl.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbb-dl
-Version: 1.0.8
+Version: 1.0.9
 Summary: Big Blue Button Downloader that downloads a BBB lesson as MP4 video
 Home-page: https://github.com/C0D3D3V/bbb-dl
 Author: C0D3D3V
 License: GPL-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
@@ -18,15 +18,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
 Requires-Dist: aiofiles>=22.1.0
 Requires-Dist: aiohttp>=3.8.3
 Requires-Dist: colorama>=0.4.6
 Requires-Dist: playwright>=1.29.0
-Requires-Dist: python-ffmpeg>=1.0.16
+Requires-Dist: python-ffmpeg>=2.0.10
 
 # Big Blue Button (BBB) Downloader
 
 Downloads a BBB lesson as MP4 video.
 The assembled video includes:
 
 - shared audio and webcams video
@@ -44,14 +44,27 @@
 3. Run: `pip install --user bbb-dl`
 4. Run `playwright install chromium`
 
 5. Run `bbb-dl --help` to see all options
 
 If you ever need to update `bbb-dl` run: `pip install -U bbb-dl`
 
+#### Alternatively use an virtual enviroment
+
+1. Install [Python](https://www.python.org/) >=3.7 and [git](https://git-scm.com/downloads)
+2. Install  `virtualenv`: `pip install virtualenv`
+3. Create a directory where you wish to install ebsco-dl. Open a terminal in the desired directory
+4. Clone this repository into that folder: `git clone https://github.com/C0D3D3V/bbb-dl.git .`
+5. Run `virtualenv venv` to create the virtual environment (on Windows use `venv\Scripts\activate`)
+6. Run `source venv/bin/activate` to activate the virtual environment (on Windows use `venv\Scripts\activate`)
+7. Install `bbb-dl`: `pip install .`
+8. Install [ffmpeg](https://github.com/C0D3D3V/Moodle-Downloader-2/wiki/Installing-ffmpeg)
+9. Run `playwright install chromium`
+10. Run `bbb-dl --help` to see all options
+
 ### Usage
 
 **Temporary files are default stored in the application data folder** 
 
 - The `--backup` option uses the same location
 - You can change this location with the `--working-dir` option
 - On Windows, the folder is located in `%localappdata%\bbb-dl`
```

### Comparing `bbb-dl-1.0.8/setup.py` & `bbb-dl-1.0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     },
     python_requires='>=3.7',
     install_requires=[
         'aiofiles>=22.1.0',
         'aiohttp>=3.8.3',
         'colorama>=0.4.6',
         'playwright>=1.29.0',
-        'python-ffmpeg>=1.0.16',
+        'python-ffmpeg>=2.0.10',
     ],
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: End Users/Desktop',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3 :: Only',
         'Topic :: Education',
```

