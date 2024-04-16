# Comparing `tmp/fritzbox-tray-1.0.68.tar.gz` & `tmp/fritzbox-tray-1.0.69.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fritzbox-tray-1.0.68.tar", last modified: Wed Feb 28 13:12:50 2024, max compression
+gzip compressed data, was "fritzbox-tray-1.0.69.tar", last modified: Tue Apr 16 11:19:02 2024, max compression
```

## Comparing `fritzbox-tray-1.0.68.tar` & `fritzbox-tray-1.0.69.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-02-28 13:12:50.323198 fritzbox-tray-1.0.68/
--rw-rw-rw-   0        0        0    35823 2023-01-08 18:15:51.000000 fritzbox-tray-1.0.68/LICENSE
--rw-rw-rw-   0        0        0     4121 2024-02-28 13:12:50.321196 fritzbox-tray-1.0.68/PKG-INFO
--rw-rw-rw-   0        0        0     3058 2023-10-03 18:29:21.000000 fritzbox-tray-1.0.68/README.md
--rw-rw-rw-   0        0        0       42 2024-02-28 13:12:50.323198 fritzbox-tray-1.0.68/setup.cfg
--rw-rw-rw-   0        0        0     2637 2024-02-28 13:06:16.000000 fritzbox-tray-1.0.68/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-28 13:12:50.279757 fritzbox-tray-1.0.68/src/
-drwxrwxrwx   0        0        0        0 2024-02-28 13:12:50.294490 fritzbox-tray-1.0.68/src/fritzbox_tray/
--rw-rw-rw-   0        0        0        0 2023-01-07 15:15:29.000000 fritzbox-tray-1.0.68/src/fritzbox_tray/__init__.py
--rw-rw-rw-   0        0        0     5067 2023-10-03 17:38:19.000000 fritzbox-tray-1.0.68/src/fritzbox_tray/__main__.py
-drwxrwxrwx   0        0        0        0 2024-02-28 13:12:50.316198 fritzbox-tray-1.0.68/src/fritzbox_tray/resources/
--rw-rw-rw-   0        0        0   121004 2023-01-08 16:34:44.000000 fritzbox-tray-1.0.68/src/fritzbox_tray/resources/ft.ico
-drwxrwxrwx   0        0        0        0 2024-02-28 13:12:50.314198 fritzbox-tray-1.0.68/src/fritzbox_tray.egg-info/
--rw-rw-rw-   0        0        0     4121 2024-02-28 13:12:50.000000 fritzbox-tray-1.0.68/src/fritzbox_tray.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      369 2024-02-28 13:12:50.000000 fritzbox-tray-1.0.68/src/fritzbox_tray.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-28 13:12:50.000000 fritzbox-tray-1.0.68/src/fritzbox_tray.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2024-02-28 13:12:50.000000 fritzbox-tray-1.0.68/src/fritzbox_tray.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      129 2024-02-28 13:12:50.000000 fritzbox-tray-1.0.68/src/fritzbox_tray.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-02-28 13:12:50.000000 fritzbox-tray-1.0.68/src/fritzbox_tray.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-16 11:19:02.926128 fritzbox-tray-1.0.69/
+-rw-rw-rw-   0        0        0    35823 2023-01-08 18:15:51.000000 fritzbox-tray-1.0.69/LICENSE
+-rw-rw-rw-   0        0        0     4121 2024-04-16 11:19:02.923125 fritzbox-tray-1.0.69/PKG-INFO
+-rw-rw-rw-   0        0        0     3058 2023-10-03 18:29:21.000000 fritzbox-tray-1.0.69/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-16 11:19:02.926128 fritzbox-tray-1.0.69/setup.cfg
+-rw-rw-rw-   0        0        0     2637 2024-04-16 11:02:59.000000 fritzbox-tray-1.0.69/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 11:19:02.874039 fritzbox-tray-1.0.69/src/
+drwxrwxrwx   0        0        0        0 2024-04-16 11:19:02.891631 fritzbox-tray-1.0.69/src/fritzbox_tray/
+-rw-rw-rw-   0        0        0        0 2023-01-07 15:15:29.000000 fritzbox-tray-1.0.69/src/fritzbox_tray/__init__.py
+-rw-rw-rw-   0        0        0     5067 2023-10-03 17:38:19.000000 fritzbox-tray-1.0.69/src/fritzbox_tray/__main__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 11:19:02.917127 fritzbox-tray-1.0.69/src/fritzbox_tray/resources/
+-rw-rw-rw-   0        0        0   121004 2023-01-08 16:34:44.000000 fritzbox-tray-1.0.69/src/fritzbox_tray/resources/ft.ico
+drwxrwxrwx   0        0        0        0 2024-04-16 11:19:02.914609 fritzbox-tray-1.0.69/src/fritzbox_tray.egg-info/
+-rw-rw-rw-   0        0        0     4121 2024-04-16 11:19:02.000000 fritzbox-tray-1.0.69/src/fritzbox_tray.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      369 2024-04-16 11:19:02.000000 fritzbox-tray-1.0.69/src/fritzbox_tray.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 11:19:02.000000 fritzbox-tray-1.0.69/src/fritzbox_tray.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2024-04-16 11:19:02.000000 fritzbox-tray-1.0.69/src/fritzbox_tray.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      129 2024-04-16 11:19:02.000000 fritzbox-tray-1.0.69/src/fritzbox_tray.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-16 11:19:02.000000 fritzbox-tray-1.0.69/src/fritzbox_tray.egg-info/top_level.txt
```

### Comparing `fritzbox-tray-1.0.68/LICENSE` & `fritzbox-tray-1.0.69/LICENSE`

 * *Files identical despite different names*

### Comparing `fritzbox-tray-1.0.68/PKG-INFO` & `fritzbox-tray-1.0.69/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fritzbox-tray
-Version: 1.0.68
+Version: 1.0.69
 Summary: A system tray application for interacting with FRITZ!Box devices.
 Home-page: https://github.com/aviolaris/fritzbox-tray
 Author: Andreas Violaris
 Keywords: fritz,fritzbox,fritz-box,fritzbox-tray,fritzbox_tray,avm-fritz,tray,python,pypi,python3,tray,tray-application,pypi-package,tray-app
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `fritzbox-tray-1.0.68/README.md` & `fritzbox-tray-1.0.69/README.md`

 * *Files identical despite different names*

### Comparing `fritzbox-tray-1.0.68/setup.py` & `fritzbox-tray-1.0.69/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     long_description = f.read()
 
 with open('requirements.txt', encoding='utf-8') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='fritzbox-tray',
-    version='1.0.68',
+    version='1.0.69',
     packages=find_namespace_packages(where="src"),
     package_dir={"": "src"},
     package_data={
         "fritzbox_tray": ["*.py"],
         "fritzbox_tray.resources": ["*.ico"],
     },
     description='A system tray application for interacting with FRITZ!Box devices.',
```

### Comparing `fritzbox-tray-1.0.68/src/fritzbox_tray/__main__.py` & `fritzbox-tray-1.0.69/src/fritzbox_tray/__main__.py`

 * *Files identical despite different names*

### Comparing `fritzbox-tray-1.0.68/src/fritzbox_tray/resources/ft.ico` & `fritzbox-tray-1.0.69/src/fritzbox_tray/resources/ft.ico`

 * *Files identical despite different names*

### Comparing `fritzbox-tray-1.0.68/src/fritzbox_tray.egg-info/PKG-INFO` & `fritzbox-tray-1.0.69/src/fritzbox_tray.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fritzbox-tray
-Version: 1.0.68
+Version: 1.0.69
 Summary: A system tray application for interacting with FRITZ!Box devices.
 Home-page: https://github.com/aviolaris/fritzbox-tray
 Author: Andreas Violaris
 Keywords: fritz,fritzbox,fritz-box,fritzbox-tray,fritzbox_tray,avm-fritz,tray,python,pypi,python3,tray,tray-application,pypi-package,tray-app
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Operating System :: Microsoft :: Windows
```

