# Comparing `tmp/pynovnc-1.1.3.tar.gz` & `tmp/pynovnc-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynovnc-1.1.3.tar", last modified: Sun Apr 14 07:11:36 2024, max compression
+gzip compressed data, was "pynovnc-1.1.4.tar", last modified: Tue Apr 16 13:07:45 2024, max compression
```

## Comparing `pynovnc-1.1.3.tar` & `pynovnc-1.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 07:11:36.567448 pynovnc-1.1.3/
--rw-r--r--   0 root         (0) root         (0)     1125 2024-04-14 07:11:36.566448 pynovnc-1.1.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      733 2024-04-14 07:11:27.000000 pynovnc-1.1.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 07:11:36.564448 pynovnc-1.1.3/pynovnc/
--rw-rw-rw-   0 root         (0) root         (0)      348 2024-04-14 07:11:27.000000 pynovnc-1.1.3/pynovnc/Main.py
--rw-rw-rw-   0 root         (0) root         (0)     2918 2024-04-14 07:11:27.000000 pynovnc-1.1.3/pynovnc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 07:11:36.566448 pynovnc-1.1.3/pynovnc.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1125 2024-04-14 07:11:36.000000 pynovnc-1.1.3/pynovnc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      242 2024-04-14 07:11:36.000000 pynovnc-1.1.3/pynovnc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-14 07:11:36.000000 pynovnc-1.1.3/pynovnc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       46 2024-04-14 07:11:36.000000 pynovnc-1.1.3/pynovnc.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-04-14 07:11:36.000000 pynovnc-1.1.3/pynovnc.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-14 07:11:36.000000 pynovnc-1.1.3/pynovnc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-14 07:11:36.567448 pynovnc-1.1.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3019 2024-04-14 07:11:27.000000 pynovnc-1.1.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 13:07:45.650290 pynovnc-1.1.4/
+-rw-r--r--   0 root         (0) root         (0)     1125 2024-04-16 13:07:45.649290 pynovnc-1.1.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      733 2024-04-16 13:07:36.000000 pynovnc-1.1.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 13:07:45.648290 pynovnc-1.1.4/pynovnc/
+-rw-rw-rw-   0 root         (0) root         (0)      348 2024-04-16 13:07:36.000000 pynovnc-1.1.4/pynovnc/Main.py
+-rw-rw-rw-   0 root         (0) root         (0)     3025 2024-04-16 13:07:36.000000 pynovnc-1.1.4/pynovnc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 13:07:45.649290 pynovnc-1.1.4/pynovnc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1125 2024-04-16 13:07:45.000000 pynovnc-1.1.4/pynovnc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      242 2024-04-16 13:07:45.000000 pynovnc-1.1.4/pynovnc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 13:07:45.000000 pynovnc-1.1.4/pynovnc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2024-04-16 13:07:45.000000 pynovnc-1.1.4/pynovnc.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-04-16 13:07:45.000000 pynovnc-1.1.4/pynovnc.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-16 13:07:45.000000 pynovnc-1.1.4/pynovnc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-16 13:07:45.650290 pynovnc-1.1.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3019 2024-04-16 13:07:36.000000 pynovnc-1.1.4/setup.py
```

### Comparing `pynovnc-1.1.3/PKG-INFO` & `pynovnc-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynovnc
-Version: 1.1.3
+Version: 1.1.4
 Summary: Python Package made by Mhadhbi Issam . 
 Home-page: https://gitlab.com/isampypi/pynovnc
 Author: Mhadhbi Issam
 Author-email: mhadhbixissam@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pynovnc Version: 1.1.3 Summary: Python Package made
+Metadata-Version: 2.1 Name: pynovnc Version: 1.1.4 Summary: Python Package made
 by Mhadhbi Issam . Home-page: https://gitlab.com/isampypi/pynovnc Author:
 Mhadhbi Issam Author-email: mhadhbixissam@gmail.com Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Description-Content-Type: text/
 markdown Requires-Dist: bashi # pynovnc _C_o_l_a_b ## Install Requiements : ```bash
 apt install -y --fix-missing xserver-xephyr x11vnc xvfb novnc net-tools x11-
 apps x11-xkb-utils gedit tightvncserver x11-utils gnumeric ``` ## Installation
```

### Comparing `pynovnc-1.1.3/README.md` & `pynovnc-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pynovnc-1.1.3/pynovnc/__init__.py` & `pynovnc-1.1.4/pynovnc/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,28 +42,28 @@
 
 
     def kill(self) :
         self.process.kill()
         print(f">_$ Application  {self.name } killed ")
 
 class VirtualDisplay :
-    def __init__(self,port= 0 , w = 1280 , h  = 1080,dp = 24 ) :
+    def __init__(self,port= 0 , w = 1280 , h  = 1080,dp = 24 , vncport = None , rfbport = None ) :
         self.id , self.w , self.h , self.dp = port , w , h , dp
         self.x11vnc_options =  [
                 "-quiet",
                 "-cursor",
                 "-localhost",
                 "-nopw",
                 "-forever",
                 "-shared",
                 "-enablehttpproxy" ,
                 "--multiptr"
                 ]
-        self.rfbport = portpicker.pick_unused_port()
-        self.vncport = portpicker.pick_unused_port()
+        self.rfbport = rfbport if vncport is not None else portpicker.pick_unused_port() 
+        self.vncport = vncport if vncport is not None else portpicker.pick_unused_port()
         self.app = None
 
     def start(self) :
         print(f">_$ Virtual Display {self.id} opened ")
         self.xvfb  = subprocess.Popen(["Xvfb", f":{self.id}", f"-screen", f"0", f"{self.w}x{self.h}x{self.dp}"])
         time.sleep(1)
         self.x11vnc = X11vnc(self.rfbport , options = self.x11vnc_options)
```

### Comparing `pynovnc-1.1.3/pynovnc.egg-info/PKG-INFO` & `pynovnc-1.1.4/pynovnc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynovnc
-Version: 1.1.3
+Version: 1.1.4
 Summary: Python Package made by Mhadhbi Issam . 
 Home-page: https://gitlab.com/isampypi/pynovnc
 Author: Mhadhbi Issam
 Author-email: mhadhbixissam@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pynovnc Version: 1.1.3 Summary: Python Package made
+Metadata-Version: 2.1 Name: pynovnc Version: 1.1.4 Summary: Python Package made
 by Mhadhbi Issam . Home-page: https://gitlab.com/isampypi/pynovnc Author:
 Mhadhbi Issam Author-email: mhadhbixissam@gmail.com Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Description-Content-Type: text/
 markdown Requires-Dist: bashi # pynovnc _C_o_l_a_b ## Install Requiements : ```bash
 apt install -y --fix-missing xserver-xephyr x11vnc xvfb novnc net-tools x11-
 apps x11-xkb-utils gedit tightvncserver x11-utils gnumeric ``` ## Installation
```

### Comparing `pynovnc-1.1.3/setup.py` & `pynovnc-1.1.4/setup.py`

 * *Files identical despite different names*

