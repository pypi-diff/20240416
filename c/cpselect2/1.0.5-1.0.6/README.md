# Comparing `tmp/cpselect2-1.0.5.tar.gz` & `tmp/cpselect2-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpselect2-1.0.5.tar", max compression
+gzip compressed data, was "cpselect2-1.0.6.tar", max compression
```

## Comparing `cpselect2-1.0.5.tar` & `cpselect2-1.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1071 2024-04-09 14:16:55.754384 cpselect2-1.0.5/LICENSE
--rw-r--r--   0        0        0     1945 2024-04-09 14:16:55.754384 cpselect2-1.0.5/README.md
--rw-r--r--   0        0        0       31 2024-04-09 14:16:55.754384 cpselect2-1.0.5/cpselect2/__init__.py
--rw-r--r--   0        0        0    15496 2024-04-09 14:16:55.754384 cpselect2-1.0.5/cpselect2/cpselect.py
--rw-r--r--   0        0        0     2104 2024-04-09 14:16:55.754384 cpselect2-1.0.5/cpselect2/help.html
--rw-r--r--   0        0        0      900 2024-04-09 14:16:55.754384 cpselect2-1.0.5/cpselect2/img/backforwardbutton.png
--rw-r--r--   0        0        0    32924 2024-04-09 14:16:55.754384 cpselect2-1.0.5/cpselect2/img/cpselect32.ico
--rw-r--r--   0        0        0      739 2024-04-09 14:16:55.754384 cpselect2-1.0.5/cpselect2/img/homebutton.png
--rw-r--r--   0        0        0     2121 2024-04-09 14:16:55.754384 cpselect2-1.0.5/cpselect2/img/navbuttons.PNG
--rw-r--r--   0        0        0      691 2024-04-09 14:16:55.754384 cpselect2-1.0.5/cpselect2/img/panzoombutton.png
--rw-r--r--   0        0        0      895 2024-04-09 14:16:55.754384 cpselect2-1.0.5/cpselect2/img/zoomboxbutton.png
--rw-r--r--   0        0        0        0 2024-04-09 14:16:55.754384 cpselect2-1.0.5/cpselect2/test/__init__.py
--rw-r--r--   0        0        0      402 2024-04-09 14:16:55.754384 cpselect2-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     2594 1970-01-01 00:00:00.000000 cpselect2-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-04-16 21:17:50.636802 cpselect2-1.0.6/LICENSE
+-rw-r--r--   0        0        0     1945 2024-04-16 21:17:50.636802 cpselect2-1.0.6/README.md
+-rw-r--r--   0        0        0       32 2024-04-16 21:17:50.636802 cpselect2-1.0.6/cpselect2/__init__.py
+-rw-r--r--   0        0        0    15496 2024-04-16 21:17:50.636802 cpselect2-1.0.6/cpselect2/cpselect.py
+-rw-r--r--   0        0        0     2104 2024-04-16 21:17:50.636802 cpselect2-1.0.6/cpselect2/help.html
+-rw-r--r--   0        0        0      900 2024-04-16 21:17:50.636802 cpselect2-1.0.6/cpselect2/img/backforwardbutton.png
+-rw-r--r--   0        0        0    32924 2024-04-16 21:17:50.636802 cpselect2-1.0.6/cpselect2/img/cpselect32.ico
+-rw-r--r--   0        0        0      739 2024-04-16 21:17:50.636802 cpselect2-1.0.6/cpselect2/img/homebutton.png
+-rw-r--r--   0        0        0     2121 2024-04-16 21:17:50.636802 cpselect2-1.0.6/cpselect2/img/navbuttons.PNG
+-rw-r--r--   0        0        0      691 2024-04-16 21:17:50.636802 cpselect2-1.0.6/cpselect2/img/panzoombutton.png
+-rw-r--r--   0        0        0      895 2024-04-16 21:17:50.636802 cpselect2-1.0.6/cpselect2/img/zoomboxbutton.png
+-rw-r--r--   0        0        0        0 2024-04-16 21:17:50.636802 cpselect2-1.0.6/cpselect2/test/__init__.py
+-rw-r--r--   0        0        0      402 2024-04-16 21:17:50.636802 cpselect2-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2594 1970-01-01 00:00:00.000000 cpselect2-1.0.6/PKG-INFO
```

### Comparing `cpselect2-1.0.5/LICENSE` & `cpselect2-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cpselect2-1.0.5/README.md` & `cpselect2-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `cpselect2-1.0.5/cpselect2/cpselect.py` & `cpselect2-1.0.6/cpselect2/cpselect.py`

 * *Files identical despite different names*

### Comparing `cpselect2-1.0.5/cpselect2/help.html` & `cpselect2-1.0.6/cpselect2/help.html`

 * *Files identical despite different names*

### Comparing `cpselect2-1.0.5/cpselect2/img/backforwardbutton.png` & `cpselect2-1.0.6/cpselect2/img/backforwardbutton.png`

 * *Files identical despite different names*

### Comparing `cpselect2-1.0.5/cpselect2/img/cpselect32.ico` & `cpselect2-1.0.6/cpselect2/img/cpselect32.ico`

 * *Files identical despite different names*

### Comparing `cpselect2-1.0.5/cpselect2/img/homebutton.png` & `cpselect2-1.0.6/cpselect2/img/homebutton.png`

 * *Files identical despite different names*

### Comparing `cpselect2-1.0.5/cpselect2/img/navbuttons.PNG` & `cpselect2-1.0.6/cpselect2/img/navbuttons.PNG`

 * *Files identical despite different names*

### Comparing `cpselect2-1.0.5/cpselect2/img/panzoombutton.png` & `cpselect2-1.0.6/cpselect2/img/panzoombutton.png`

 * *Files identical despite different names*

### Comparing `cpselect2-1.0.5/cpselect2/img/zoomboxbutton.png` & `cpselect2-1.0.6/cpselect2/img/zoomboxbutton.png`

 * *Files identical despite different names*

### Comparing `cpselect2-1.0.5/PKG-INFO` & `cpselect2-1.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpselect2
-Version: 1.0.5
+Version: 1.0.6
 Summary: Matlab's cpselect alternative for Python
 License: MIT
 Author: arunoruto
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

