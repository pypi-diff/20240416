# Comparing `tmp/trm_woodburn-0.0.7.tar.gz` & `tmp/trm_woodburn-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trm_woodburn-0.0.7.tar", last modified: Mon Apr 15 21:50:30 2024, max compression
+gzip compressed data, was "trm_woodburn-0.0.8.tar", last modified: Tue Apr 16 03:27:23 2024, max compression
```

## Comparing `trm_woodburn-0.0.7.tar` & `trm_woodburn-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-15 21:50:30.701819 trm_woodburn-0.0.7/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     1054 2024-04-15 16:11:57.000000 trm_woodburn-0.0.7/LICENSE.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     6289 2024-04-15 21:50:30.701769 trm_woodburn-0.0.7/PKG-INFO
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     5810 2024-04-15 21:49:23.000000 trm_woodburn-0.0.7/README.md
--rw-r--r--   0 davidwoodburn   (501) staff       (20)       85 2022-10-17 18:56:07.000000 trm_woodburn-0.0.7/pyproject.toml
--rw-r--r--   0 davidwoodburn   (501) staff       (20)      601 2024-04-15 21:50:30.702037 trm_woodburn-0.0.7/setup.cfg
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-15 21:50:30.700169 trm_woodburn-0.0.7/src/
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-15 21:50:30.700844 trm_woodburn-0.0.7/src/trm/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)       50 2024-04-15 19:15:58.000000 trm_woodburn-0.0.7/src/trm/__init__.py
--rw-r--r--   0 davidwoodburn   (501) staff       (20)    19811 2024-04-15 21:32:23.000000 trm_woodburn-0.0.7/src/trm/trm.py
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-15 21:50:30.701586 trm_woodburn-0.0.7/src/trm_woodburn.egg-info/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     6289 2024-04-15 21:50:30.000000 trm_woodburn-0.0.7/src/trm_woodburn.egg-info/PKG-INFO
--rw-r--r--   0 davidwoodburn   (501) staff       (20)      280 2024-04-15 21:50:30.000000 trm_woodburn-0.0.7/src/trm_woodburn.egg-info/SOURCES.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        1 2024-04-15 21:50:30.000000 trm_woodburn-0.0.7/src/trm_woodburn.egg-info/dependency_links.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        6 2024-04-15 21:50:30.000000 trm_woodburn-0.0.7/src/trm_woodburn.egg-info/requires.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        4 2024-04-15 21:50:30.000000 trm_woodburn-0.0.7/src/trm_woodburn.egg-info/top_level.txt
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-16 03:27:23.983184 trm_woodburn-0.0.8/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     1054 2024-04-15 16:11:57.000000 trm_woodburn-0.0.8/LICENSE.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     6454 2024-04-16 03:27:23.983130 trm_woodburn-0.0.8/PKG-INFO
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     5975 2024-04-16 03:26:34.000000 trm_woodburn-0.0.8/README.md
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)       85 2022-10-17 18:56:07.000000 trm_woodburn-0.0.8/pyproject.toml
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)      601 2024-04-16 03:27:23.983411 trm_woodburn-0.0.8/setup.cfg
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-16 03:27:23.981143 trm_woodburn-0.0.8/src/
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-16 03:27:23.982070 trm_woodburn-0.0.8/src/trm/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)       50 2024-04-15 19:15:58.000000 trm_woodburn-0.0.8/src/trm/__init__.py
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)    20816 2024-04-16 03:24:23.000000 trm_woodburn-0.0.8/src/trm/trm.py
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-16 03:27:23.982939 trm_woodburn-0.0.8/src/trm_woodburn.egg-info/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     6454 2024-04-16 03:27:23.000000 trm_woodburn-0.0.8/src/trm_woodburn.egg-info/PKG-INFO
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)      280 2024-04-16 03:27:23.000000 trm_woodburn-0.0.8/src/trm_woodburn.egg-info/SOURCES.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        1 2024-04-16 03:27:23.000000 trm_woodburn-0.0.8/src/trm_woodburn.egg-info/dependency_links.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        6 2024-04-16 03:27:23.000000 trm_woodburn-0.0.8/src/trm_woodburn.egg-info/requires.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        4 2024-04-16 03:27:23.000000 trm_woodburn-0.0.8/src/trm_woodburn.egg-info/top_level.txt
```

### Comparing `trm_woodburn-0.0.7/LICENSE.txt` & `trm_woodburn-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `trm_woodburn-0.0.7/PKG-INFO` & `trm_woodburn-0.0.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trm-woodburn
-Version: 0.0.7
+Version: 0.0.8
 Summary: A library for pretty printing to the terminal
 Home-page: https://gitlab.com/davidwoodburn/trm
 Author: David Woodburn
 Author-email: david.woodburn@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -35,15 +35,15 @@
 These are all excuses to use this library. But, the biggest reason to use this
 library is that the terminal is cool, and the more you can do you work in the
 terminal the better.
 
 ## Plots
 
 ```python
-trm.plot(x, y=None, label='', rows=1, cols=1)
+trm.plot(x, y=None, label='', rows=1, cols=1, equal=0)
 ```
 
 The plot function will render all the data points defined by `x` and `y` to the
 terminal. The inputs `x` and `y` can be vectors or matrices. If they are
 matrices, each row is treated as a separate curve.
 
 The shapes of `x` and `y` do not have to be the same, but they must be
@@ -81,14 +81,17 @@
 
 If only one curve is being plotted, the characters will be written in whatever
 the default font color is set to in your terminal. If more than one curve is
 plotted, color will be used. The color map is blue, green, yellow, red, and
 magenta. If you have more than 5 curves (This is just a terminal-based plot; why
 would you do that?), then the colors will recyle.
 
+If you want equal axis scaling, set `equal` to `1`. However, since terminal
+fonts are not always the same aspect ratio, you can adjust this value to tune.
+
 ## Bars
 
 ```python
 trm.bars(x, labels=None, width=COLS, show_zero=True)
 ```
 
 It can be convenient to plot a simple bar graph. The `x` input is the vector of
```

### Comparing `trm_woodburn-0.0.7/README.md` & `trm_woodburn-0.0.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 These are all excuses to use this library. But, the biggest reason to use this
 library is that the terminal is cool, and the more you can do you work in the
 terminal the better.
 
 ## Plots
 
 ```python
-trm.plot(x, y=None, label='', rows=1, cols=1)
+trm.plot(x, y=None, label='', rows=1, cols=1, equal=0)
 ```
 
 The plot function will render all the data points defined by `x` and `y` to the
 terminal. The inputs `x` and `y` can be vectors or matrices. If they are
 matrices, each row is treated as a separate curve.
 
 The shapes of `x` and `y` do not have to be the same, but they must be
@@ -66,14 +66,17 @@
 
 If only one curve is being plotted, the characters will be written in whatever
 the default font color is set to in your terminal. If more than one curve is
 plotted, color will be used. The color map is blue, green, yellow, red, and
 magenta. If you have more than 5 curves (This is just a terminal-based plot; why
 would you do that?), then the colors will recyle.
 
+If you want equal axis scaling, set `equal` to `1`. However, since terminal
+fonts are not always the same aspect ratio, you can adjust this value to tune.
+
 ## Bars
 
 ```python
 trm.bars(x, labels=None, width=COLS, show_zero=True)
 ```
 
 It can be convenient to plot a simple bar graph. The `x` input is the vector of
```

### Comparing `trm_woodburn-0.0.7/setup.cfg` & `trm_woodburn-0.0.8/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = trm-woodburn
-version = 0.0.7
+version = 0.0.8
 author = David Woodburn
 author_email = david.woodburn@icloud.com
 description = A library for pretty printing to the terminal
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.com/davidwoodburn/trm
 classifiers =
```

### Comparing `trm_woodburn-0.0.7/src/trm/trm.py` & `trm_woodburn-0.0.8/src/trm/trm.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,17 +32,18 @@
 import numpy as np
 
 
 class config:
     uni = True # flag to use unicode characters
     cols = 60 # default column width
     rows = 20 # default row height
+    ar = 2.1 # aspect ratio of characters
 
 
-def plot(x, y=None, label='', rows=1, cols=1):
+def plot(x, y=None, label='', rows=1, cols=1, equal=0):
     """
     Create a text-based plot of the path defined by (`x`, `y`) using characters.
     If the size of the terminal can be found, that will be used for sizing the
     plot. Otherwise, the default dimensions (config.cols, config.rows) will be
     used. Note that this function does not plot connecting lines, only the
     points specified by the (`x`, `y`) pairs.
 
@@ -58,14 +59,19 @@
         Text to place at top of the plot, centered in the border.
     rows : int, default 1
         Desired number of rows if greater than 1 or fraction of existing rows if
         less than 1.
     cols : int, default 1
         Desired number of columns if greater than 1 or fraction of existing
         columns if less than 1.
+    equal : float, default 0
+        Axis scaling, `y` to `x`. A value of 0 leaves the scaling alone. A value
+        of 1 would approximate equal axis scaling. However, because the aspect
+        ratio of characters in the terminal is not exactly 2 to 1, this value
+        can be adjusted to compensate.
     """
 
     # Get the terminal window size.
     try: # Try to get the true size.
         term_cols, term_rows = os.get_terminal_size()
         use_color = True
     except: # If getting terminal size fails, use default values.
@@ -114,14 +120,33 @@
         x_max += eps
     y_min = np.nanmin(y)
     y_max = np.nanmax(y)
     if y_min == y_max:
         y_min -= eps
         y_max += eps
 
+    # Apply axis scaling.
+    if equal != 0:
+        x_scale = (1/config.ar)*cols/(x_max - x_min)
+        y_scale = rows/(y_max - y_min)
+        print(x_scale)
+        print(y_scale)
+        if x_scale*equal < y_scale:
+            y_scale = x_scale*equal
+            y_span = rows/y_scale
+            y_mid = (y_max + y_min)*0.5
+            y_min = y_mid - y_span*0.5
+            y_max = y_mid + y_span*0.5
+        elif y_scale < x_scale*equal:
+            x_scale = y_scale/equal
+            x_span = (1/config.ar)*cols/x_scale
+            x_mid = (x_max + x_min)*0.5
+            x_min = x_mid - x_span*0.5
+            x_max = x_mid + x_span*0.5
+
     # Expand the limits to align zero with the nearest half row so that the zero
     # marker is true.
     if (y_min < 0) and (y_max > 0):
         idx_zero = round((rows - 1.0/subrows)
             * y_max/(y_max - y_min) - 0.5)*subrows + subrows/2
         slope = max((subrows*rows - 1 - idx_zero)/y_min,
             -idx_zero/y_max)
```

### Comparing `trm_woodburn-0.0.7/src/trm_woodburn.egg-info/PKG-INFO` & `trm_woodburn-0.0.8/src/trm_woodburn.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trm-woodburn
-Version: 0.0.7
+Version: 0.0.8
 Summary: A library for pretty printing to the terminal
 Home-page: https://gitlab.com/davidwoodburn/trm
 Author: David Woodburn
 Author-email: david.woodburn@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -35,15 +35,15 @@
 These are all excuses to use this library. But, the biggest reason to use this
 library is that the terminal is cool, and the more you can do you work in the
 terminal the better.
 
 ## Plots
 
 ```python
-trm.plot(x, y=None, label='', rows=1, cols=1)
+trm.plot(x, y=None, label='', rows=1, cols=1, equal=0)
 ```
 
 The plot function will render all the data points defined by `x` and `y` to the
 terminal. The inputs `x` and `y` can be vectors or matrices. If they are
 matrices, each row is treated as a separate curve.
 
 The shapes of `x` and `y` do not have to be the same, but they must be
@@ -81,14 +81,17 @@
 
 If only one curve is being plotted, the characters will be written in whatever
 the default font color is set to in your terminal. If more than one curve is
 plotted, color will be used. The color map is blue, green, yellow, red, and
 magenta. If you have more than 5 curves (This is just a terminal-based plot; why
 would you do that?), then the colors will recyle.
 
+If you want equal axis scaling, set `equal` to `1`. However, since terminal
+fonts are not always the same aspect ratio, you can adjust this value to tune.
+
 ## Bars
 
 ```python
 trm.bars(x, labels=None, width=COLS, show_zero=True)
 ```
 
 It can be convenient to plot a simple bar graph. The `x` input is the vector of
```

