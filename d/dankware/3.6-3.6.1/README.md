# Comparing `tmp/dankware-3.6.tar.gz` & `tmp/dankware-3.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dankware-3.6.tar", last modified: Sat Mar 30 15:16:29 2024, max compression
+gzip compressed data, was "dankware-3.6.1.tar", last modified: Tue Apr 16 05:56:54 2024, max compression
```

## Comparing `dankware-3.6.tar` & `dankware-3.6.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 15:16:29.962576 dankware-3.6/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-30 15:16:21.000000 dankware-3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    17017 2024-03-30 15:16:29.962576 dankware-3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15942 2024-03-30 15:16:21.000000 dankware-3.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 15:16:29.962576 dankware-3.6/dankware/
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-03-30 15:16:21.000000 dankware-3.6/dankware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-03-30 15:16:21.000000 dankware-3.6/dankware/ctypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3915 2024-03-30 15:16:21.000000 dankware-3.6/dankware/datetime.py
--rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-03-30 15:16:21.000000 dankware-3.6/dankware/multithread.py
--rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-03-30 15:16:21.000000 dankware-3.6/dankware/pillow.py
--rw-r--r--   0 runner    (1001) docker     (127)     4270 2024-03-30 15:16:21.000000 dankware-3.6/dankware/requests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-03-30 15:16:21.000000 dankware-3.6/dankware/terminal.py
--rw-r--r--   0 runner    (1001) docker     (127)    16764 2024-03-30 15:16:21.000000 dankware-3.6/dankware/text.py
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-03-30 15:16:21.000000 dankware-3.6/dankware/tkinter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-03-30 15:16:21.000000 dankware-3.6/dankware/traceback.py
--rw-r--r--   0 runner    (1001) docker     (127)     4834 2024-03-30 15:16:21.000000 dankware-3.6/dankware/winreg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 15:16:29.962576 dankware-3.6/dankware.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17017 2024-03-30 15:16:29.000000 dankware-3.6/dankware.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-03-30 15:16:29.000000 dankware-3.6/dankware.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 15:16:29.000000 dankware-3.6/dankware.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-30 15:16:29.000000 dankware-3.6/dankware.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-30 15:16:29.000000 dankware-3.6/dankware.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-30 15:16:29.962576 dankware-3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-03-30 15:16:21.000000 dankware-3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:56:54.500334 dankware-3.6.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-16 05:56:50.000000 dankware-3.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    17083 2024-04-16 05:56:54.500334 dankware-3.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15942 2024-04-16 05:56:50.000000 dankware-3.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:56:54.500334 dankware-3.6.1/dankware/
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-04-16 05:56:50.000000 dankware-3.6.1/dankware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-04-16 05:56:50.000000 dankware-3.6.1/dankware/ctypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-04-16 05:56:50.000000 dankware-3.6.1/dankware/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-04-16 05:56:50.000000 dankware-3.6.1/dankware/multithread.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-04-16 05:56:50.000000 dankware-3.6.1/dankware/pillow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-04-16 05:56:50.000000 dankware-3.6.1/dankware/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-16 05:56:50.000000 dankware-3.6.1/dankware/terminal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16764 2024-04-16 05:56:50.000000 dankware-3.6.1/dankware/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-16 05:56:50.000000 dankware-3.6.1/dankware/tkinter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-04-16 05:56:50.000000 dankware-3.6.1/dankware/traceback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4834 2024-04-16 05:56:50.000000 dankware-3.6.1/dankware/winreg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:56:54.500334 dankware-3.6.1/dankware.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17083 2024-04-16 05:56:54.000000 dankware-3.6.1/dankware.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-16 05:56:54.000000 dankware-3.6.1/dankware.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 05:56:54.000000 dankware-3.6.1/dankware.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-16 05:56:54.000000 dankware-3.6.1/dankware.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-16 05:56:54.000000 dankware-3.6.1/dankware.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 05:56:54.500334 dankware-3.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-16 05:56:50.000000 dankware-3.6.1/setup.py
```

### Comparing `dankware-3.6/LICENSE` & `dankware-3.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dankware-3.6/PKG-INFO` & `dankware-3.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dankware
-Version: 3.6
+Version: 3.6.1
 Summary: Python package with various features!
 Home-page: https://github.com/SirDank/dankware
 Author: SirDank
 Author-email: SirDankenstein@protonmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/SirDank/dankware
 Project-URL: Bug Tracker, https://github.com/SirDank/dankware/issues
@@ -19,14 +19,16 @@
 Classifier: Natural Language :: English
 Classifier: Topic :: Software Development
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: rich
 Requires-Dist: colorama
 Requires-Dist: requests
+Provides-Extra: extras
+Requires-Dist: pillow; extra == "extras"
 
 
 <p align="center">
   <b>~ Visits ~</b><br><br>
   <img src="https://profile-counter.glitch.me/dankware/count.svg" />
 </p>
```

### Comparing `dankware-3.6/README.md` & `dankware-3.6.1/README.md`

 * *Files identical despite different names*

### Comparing `dankware-3.6/dankware/__init__.py` & `dankware-3.6.1/dankware/__init__.py`

 * *Files identical despite different names*

### Comparing `dankware-3.6/dankware/ctypes.py` & `dankware-3.6.1/dankware/ctypes.py`

 * *Files identical despite different names*

### Comparing `dankware-3.6/dankware/datetime.py` & `dankware-3.6.1/dankware/datetime.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         if seconds < 2592000:
             weeks = int(seconds / 604800)
             if mini: return f"{weeks}w"
             return f"{weeks} week{'s' if weeks > 1 else ''}"
 
         if seconds < 31536000:
             months = int(seconds / 2592000)
-            if mini: return f"{months}m"
+            if mini: return f"{months}mo"
             return f"{months} month{'s' if months > 1 else ''}"
 
         years = int(seconds / 31536000)
         if mini: return f"{years}y"
         return f"{years} year{'s' if years > 1 else ''}"
 
     if "default" in interval:
```

### Comparing `dankware-3.6/dankware/multithread.py` & `dankware-3.6.1/dankware/multithread.py`

 * *Files identical despite different names*

### Comparing `dankware-3.6/dankware/pillow.py` & `dankware-3.6.1/dankware/pillow.py`

 * *Files identical despite different names*

### Comparing `dankware-3.6/dankware/requests.py` & `dankware-3.6.1/dankware/requests.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,17 @@
     from dankware import github_downloads
     for _ in github_downloads("SirDank/dank.tool"): print(_)
     ```
     """
 
     response = requests.get(f"https://api.github.com/repos/{user_repo}/releases/latest", headers = {"User-Agent": "dankware"}, timeout=3).json()
 
-    return tuple(data["browser_download_url"] for data in response["assets"])
+    if response.status_code == 200:
+        return tuple(data["browser_download_url"] for data in response["assets"])
+    raise RuntimeError(f"Failed to get latest release from github: [{response.status_code}] {response.reason}")
 
 def github_file_selector(user_repo: str, filter_mode: str, filter_iterable: list[str] | tuple[str]) -> tuple[str]:
 
     """
     
     This function is used to filter the output from github_downloads()
```

### Comparing `dankware-3.6/dankware/terminal.py` & `dankware-3.6.1/dankware/terminal.py`

 * *Files identical despite different names*

### Comparing `dankware-3.6/dankware/text.py` & `dankware-3.6.1/dankware/text.py`

 * *Files identical despite different names*

### Comparing `dankware-3.6/dankware/tkinter.py` & `dankware-3.6.1/dankware/tkinter.py`

 * *Files identical despite different names*

### Comparing `dankware-3.6/dankware/traceback.py` & `dankware-3.6.1/dankware/traceback.py`

 * *Files identical despite different names*

### Comparing `dankware-3.6/dankware/winreg.py` & `dankware-3.6.1/dankware/winreg.py`

 * *Files identical despite different names*

### Comparing `dankware-3.6/dankware.egg-info/PKG-INFO` & `dankware-3.6.1/dankware.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dankware
-Version: 3.6
+Version: 3.6.1
 Summary: Python package with various features!
 Home-page: https://github.com/SirDank/dankware
 Author: SirDank
 Author-email: SirDankenstein@protonmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/SirDank/dankware
 Project-URL: Bug Tracker, https://github.com/SirDank/dankware/issues
@@ -19,14 +19,16 @@
 Classifier: Natural Language :: English
 Classifier: Topic :: Software Development
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: rich
 Requires-Dist: colorama
 Requires-Dist: requests
+Provides-Extra: extras
+Requires-Dist: pillow; extra == "extras"
 
 
 <p align="center">
   <b>~ Visits ~</b><br><br>
   <img src="https://profile-counter.glitch.me/dankware/count.svg" />
 </p>
```

### Comparing `dankware-3.6/setup.py` & `dankware-3.6.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
 
     license = "MIT",
     name = "dankware",
-    version = "3.6",
+    version = "3.6.1",
     author = "SirDank",
 
     author_email = "SirDankenstein@protonmail.com",
     description = "Python package with various features!",
     long_description = open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type = "text/markdown",
     url = "https://github.com/SirDank/dankware",
@@ -43,13 +43,14 @@
         "Intended Audience :: Developers",
         "Natural Language :: English",
         "Topic :: Software Development",
     ],
 
     package_dir = {"": "."},
     packages = find_packages(where = "."),
+    extras_require={'extras': ['pillow']},
     install_requires = [
         "rich",
         "colorama",
         "requests",
-    ],
+    ]
 )
```

