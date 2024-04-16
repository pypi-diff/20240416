# Comparing `tmp/trm_woodburn-0.0.6.tar.gz` & `tmp/trm_woodburn-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trm_woodburn-0.0.6.tar", last modified: Mon Apr 15 21:41:59 2024, max compression
+gzip compressed data, was "trm_woodburn-0.0.7.tar", last modified: Mon Apr 15 21:50:30 2024, max compression
```

## Comparing `trm_woodburn-0.0.6.tar` & `trm_woodburn-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-15 21:41:59.236250 trm_woodburn-0.0.6/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     1054 2024-04-15 16:11:57.000000 trm_woodburn-0.0.6/LICENSE.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     7308 2024-04-15 21:41:59.236194 trm_woodburn-0.0.6/PKG-INFO
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     6829 2024-04-15 21:41:16.000000 trm_woodburn-0.0.6/README.md
--rw-r--r--   0 davidwoodburn   (501) staff       (20)       85 2022-10-17 18:56:07.000000 trm_woodburn-0.0.6/pyproject.toml
--rw-r--r--   0 davidwoodburn   (501) staff       (20)      601 2024-04-15 21:41:59.236465 trm_woodburn-0.0.6/setup.cfg
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-15 21:41:59.234597 trm_woodburn-0.0.6/src/
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-15 21:41:59.235259 trm_woodburn-0.0.6/src/trm/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)       50 2024-04-15 19:15:58.000000 trm_woodburn-0.0.6/src/trm/__init__.py
--rw-r--r--   0 davidwoodburn   (501) staff       (20)    19811 2024-04-15 21:32:23.000000 trm_woodburn-0.0.6/src/trm/trm.py
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-15 21:41:59.236020 trm_woodburn-0.0.6/src/trm_woodburn.egg-info/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     7308 2024-04-15 21:41:59.000000 trm_woodburn-0.0.6/src/trm_woodburn.egg-info/PKG-INFO
--rw-r--r--   0 davidwoodburn   (501) staff       (20)      280 2024-04-15 21:41:59.000000 trm_woodburn-0.0.6/src/trm_woodburn.egg-info/SOURCES.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        1 2024-04-15 21:41:59.000000 trm_woodburn-0.0.6/src/trm_woodburn.egg-info/dependency_links.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        6 2024-04-15 21:41:59.000000 trm_woodburn-0.0.6/src/trm_woodburn.egg-info/requires.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        4 2024-04-15 21:41:59.000000 trm_woodburn-0.0.6/src/trm_woodburn.egg-info/top_level.txt
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-15 21:50:30.701819 trm_woodburn-0.0.7/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     1054 2024-04-15 16:11:57.000000 trm_woodburn-0.0.7/LICENSE.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     6289 2024-04-15 21:50:30.701769 trm_woodburn-0.0.7/PKG-INFO
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     5810 2024-04-15 21:49:23.000000 trm_woodburn-0.0.7/README.md
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)       85 2022-10-17 18:56:07.000000 trm_woodburn-0.0.7/pyproject.toml
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)      601 2024-04-15 21:50:30.702037 trm_woodburn-0.0.7/setup.cfg
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-15 21:50:30.700169 trm_woodburn-0.0.7/src/
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-15 21:50:30.700844 trm_woodburn-0.0.7/src/trm/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)       50 2024-04-15 19:15:58.000000 trm_woodburn-0.0.7/src/trm/__init__.py
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)    19811 2024-04-15 21:32:23.000000 trm_woodburn-0.0.7/src/trm/trm.py
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-15 21:50:30.701586 trm_woodburn-0.0.7/src/trm_woodburn.egg-info/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     6289 2024-04-15 21:50:30.000000 trm_woodburn-0.0.7/src/trm_woodburn.egg-info/PKG-INFO
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)      280 2024-04-15 21:50:30.000000 trm_woodburn-0.0.7/src/trm_woodburn.egg-info/SOURCES.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        1 2024-04-15 21:50:30.000000 trm_woodburn-0.0.7/src/trm_woodburn.egg-info/dependency_links.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        6 2024-04-15 21:50:30.000000 trm_woodburn-0.0.7/src/trm_woodburn.egg-info/requires.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        4 2024-04-15 21:50:30.000000 trm_woodburn-0.0.7/src/trm_woodburn.egg-info/top_level.txt
```

### Comparing `trm_woodburn-0.0.6/LICENSE.txt` & `trm_woodburn-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `trm_woodburn-0.0.6/PKG-INFO` & `trm_woodburn-0.0.7/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 Metadata-Version: 2.1
 Name: trm-woodburn
-Version: 0.0.6
+Version: 0.0.7
 Summary: A library for pretty printing to the terminal
 Home-page: https://gitlab.com/davidwoodburn/trm
 Author: David Woodburn
 Author-email: david.woodburn@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: numpy
 
 # Terminal Utilities
 
+```python
+import trm
+```
+
 This library provides several functions for nicely printing data to the
 terminal. MatPlotLib is a very nice library, but it can be a bit tedious at
 times when all you want is something quick and dirty.
 
 -   Every separate plot needs to be introduced with a `plt.figure()` statement.
 -   Large sets of data can be slow to render.
 -   If you are working in full screen on the terminal, plots can pull you to
@@ -77,18 +81,14 @@
 
 If only one curve is being plotted, the characters will be written in whatever
 the default font color is set to in your terminal. If more than one curve is
 plotted, color will be used. The color map is blue, green, yellow, red, and
 magenta. If you have more than 5 curves (This is just a terminal-based plot; why
 would you do that?), then the colors will recyle.
 
-| Single curve    | Multiple curves |
-| --------------- | --------------- |
-| ![][fig_plot_1] | ![][fig_plot_5] |
-
 ## Bars
 
 ```python
 trm.bars(x, labels=None, width=COLS, show_zero=True)
 ```
 
 It can be convenient to plot a simple bar graph. The `x` input is the vector of
@@ -112,18 +112,14 @@
 
 The `heat` function will generate a heat map of the `matrix` input using 24
 shades of gray. Black is used for the lowest value and white for the highest
 value. If `trm.config.uni` is `True`, half-block characters from the Unicode
 table will be used. If it is `False`, two spaces per element of the matrix will
 be used.
 
-| With Unicode      | Without Unicode     |
-| ----------------- | ------------------- |
-| ![][fig_heat_uni] | ![][fig_heat_ascii] |
-
 ## Tables
 
 ```python
 trm.table(matrix, head=None, left=None, width=10, sep='  ')
 ```
 
 You can print a nicely spaced table of the `matrix` data. The `head` and `left`
@@ -145,18 +141,14 @@
 ```python
 trm.sparsity(matrix, label='')
 ```
 
 If all you want to see is the sparsity of a matrix, use this function. The
 `label` input will be placed in the bottom-right corner of the render.
 
-| With Unicode          | Without Unicode         |
-| --------------------- | ----------------------- |
-| ![][fig_sparsity_uni] | ![][fig_sparsity_ascii] |
-
 ## Progress bars
 
 ```python
 trm.progress(k, K, tic=None, width=None)
 ```
 
 There are many progress bar libraries available for Python. But, many of them
@@ -169,16 +161,7 @@
 stored in `tic` will be displayed. When the process is completed, the total
 elapsed time since `tic` will be displayed. If `width` is not provided, the full
 width of the current terminal window will be used.
 
 ```
  44% [/////////////////////----------------------------] -00:00:02.1
 ```
-
-
-[fig_heat_uni]: https://gitlab.com/davidwoodburn/trm/-/blob/main/figures/fig_heat_uni.png
-[fig_heat_ascii]: https://gitlab.com/davidwoodburn/trm/-/blob/main/figures/fig_heat_ascii.png
-[fig_plot]: https://gitlab.com/davidwoodburn/trm/-/blob/main/figures/fig_plot.png
-[fig_plot_1]: https://gitlab.com/davidwoodburn/trm/-/blob/main/figures/fig_plot_1.png
-[fig_plot_5]: https://gitlab.com/davidwoodburn/trm/-/blob/main/figures/fig_plot_5.png
-[fig_sparsity_uni]: https://gitlab.com/davidwoodburn/trm/-/blob/main/figures/fig_sparsity_uni.png
-[fig_sparsity_ascii]: https://gitlab.com/davidwoodburn/trm/-/blob/main/figures/fig_sparsity_ascii.png
```

### Comparing `trm_woodburn-0.0.6/README.md` & `trm_woodburn-0.0.7/src/trm_woodburn.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,28 @@
+Metadata-Version: 2.1
+Name: trm-woodburn
+Version: 0.0.7
+Summary: A library for pretty printing to the terminal
+Home-page: https://gitlab.com/davidwoodburn/trm
+Author: David Woodburn
+Author-email: david.woodburn@icloud.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+Requires-Dist: numpy
+
 # Terminal Utilities
 
+```python
+import trm
+```
+
 This library provides several functions for nicely printing data to the
 terminal. MatPlotLib is a very nice library, but it can be a bit tedious at
 times when all you want is something quick and dirty.
 
 -   Every separate plot needs to be introduced with a `plt.figure()` statement.
 -   Large sets of data can be slow to render.
 -   If you are working in full screen on the terminal, plots can pull you to
@@ -62,18 +81,14 @@
 
 If only one curve is being plotted, the characters will be written in whatever
 the default font color is set to in your terminal. If more than one curve is
 plotted, color will be used. The color map is blue, green, yellow, red, and
 magenta. If you have more than 5 curves (This is just a terminal-based plot; why
 would you do that?), then the colors will recyle.
 
-| Single curve    | Multiple curves |
-| --------------- | --------------- |
-| ![][fig_plot_1] | ![][fig_plot_5] |
-
 ## Bars
 
 ```python
 trm.bars(x, labels=None, width=COLS, show_zero=True)
 ```
 
 It can be convenient to plot a simple bar graph. The `x` input is the vector of
@@ -97,18 +112,14 @@
 
 The `heat` function will generate a heat map of the `matrix` input using 24
 shades of gray. Black is used for the lowest value and white for the highest
 value. If `trm.config.uni` is `True`, half-block characters from the Unicode
 table will be used. If it is `False`, two spaces per element of the matrix will
 be used.
 
-| With Unicode      | Without Unicode     |
-| ----------------- | ------------------- |
-| ![][fig_heat_uni] | ![][fig_heat_ascii] |
-
 ## Tables
 
 ```python
 trm.table(matrix, head=None, left=None, width=10, sep='  ')
 ```
 
 You can print a nicely spaced table of the `matrix` data. The `head` and `left`
@@ -130,18 +141,14 @@
 ```python
 trm.sparsity(matrix, label='')
 ```
 
 If all you want to see is the sparsity of a matrix, use this function. The
 `label` input will be placed in the bottom-right corner of the render.
 
-| With Unicode          | Without Unicode         |
-| --------------------- | ----------------------- |
-| ![][fig_sparsity_uni] | ![][fig_sparsity_ascii] |
-
 ## Progress bars
 
 ```python
 trm.progress(k, K, tic=None, width=None)
 ```
 
 There are many progress bar libraries available for Python. But, many of them
@@ -154,16 +161,7 @@
 stored in `tic` will be displayed. When the process is completed, the total
 elapsed time since `tic` will be displayed. If `width` is not provided, the full
 width of the current terminal window will be used.
 
 ```
  44% [/////////////////////----------------------------] -00:00:02.1
 ```
-
-
-[fig_heat_uni]: https://gitlab.com/davidwoodburn/trm/-/blob/main/figures/fig_heat_uni.png
-[fig_heat_ascii]: https://gitlab.com/davidwoodburn/trm/-/blob/main/figures/fig_heat_ascii.png
-[fig_plot]: https://gitlab.com/davidwoodburn/trm/-/blob/main/figures/fig_plot.png
-[fig_plot_1]: https://gitlab.com/davidwoodburn/trm/-/blob/main/figures/fig_plot_1.png
-[fig_plot_5]: https://gitlab.com/davidwoodburn/trm/-/blob/main/figures/fig_plot_5.png
-[fig_sparsity_uni]: https://gitlab.com/davidwoodburn/trm/-/blob/main/figures/fig_sparsity_uni.png
-[fig_sparsity_ascii]: https://gitlab.com/davidwoodburn/trm/-/blob/main/figures/fig_sparsity_ascii.png
```

### Comparing `trm_woodburn-0.0.6/setup.cfg` & `trm_woodburn-0.0.7/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = trm-woodburn
-version = 0.0.6
+version = 0.0.7
 author = David Woodburn
 author_email = david.woodburn@icloud.com
 description = A library for pretty printing to the terminal
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.com/davidwoodburn/trm
 classifiers =
```

### Comparing `trm_woodburn-0.0.6/src/trm/trm.py` & `trm_woodburn-0.0.7/src/trm/trm.py`

 * *Files identical despite different names*

### Comparing `trm_woodburn-0.0.6/src/trm_woodburn.egg-info/PKG-INFO` & `trm_woodburn-0.0.7/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,13 @@
-Metadata-Version: 2.1
-Name: trm-woodburn
-Version: 0.0.6
-Summary: A library for pretty printing to the terminal
-Home-page: https://gitlab.com/davidwoodburn/trm
-Author: David Woodburn
-Author-email: david.woodburn@icloud.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-Requires-Dist: numpy
-
 # Terminal Utilities
 
+```python
+import trm
+```
+
 This library provides several functions for nicely printing data to the
 terminal. MatPlotLib is a very nice library, but it can be a bit tedious at
 times when all you want is something quick and dirty.
 
 -   Every separate plot needs to be introduced with a `plt.figure()` statement.
 -   Large sets of data can be slow to render.
 -   If you are working in full screen on the terminal, plots can pull you to
@@ -77,18 +66,14 @@
 
 If only one curve is being plotted, the characters will be written in whatever
 the default font color is set to in your terminal. If more than one curve is
 plotted, color will be used. The color map is blue, green, yellow, red, and
 magenta. If you have more than 5 curves (This is just a terminal-based plot; why
 would you do that?), then the colors will recyle.
 
-| Single curve    | Multiple curves |
-| --------------- | --------------- |
-| ![][fig_plot_1] | ![][fig_plot_5] |
-
 ## Bars
 
 ```python
 trm.bars(x, labels=None, width=COLS, show_zero=True)
 ```
 
 It can be convenient to plot a simple bar graph. The `x` input is the vector of
@@ -112,18 +97,14 @@
 
 The `heat` function will generate a heat map of the `matrix` input using 24
 shades of gray. Black is used for the lowest value and white for the highest
 value. If `trm.config.uni` is `True`, half-block characters from the Unicode
 table will be used. If it is `False`, two spaces per element of the matrix will
 be used.
 
-| With Unicode      | Without Unicode     |
-| ----------------- | ------------------- |
-| ![][fig_heat_uni] | ![][fig_heat_ascii] |
-
 ## Tables
 
 ```python
 trm.table(matrix, head=None, left=None, width=10, sep='  ')
 ```
 
 You can print a nicely spaced table of the `matrix` data. The `head` and `left`
@@ -145,18 +126,14 @@
 ```python
 trm.sparsity(matrix, label='')
 ```
 
 If all you want to see is the sparsity of a matrix, use this function. The
 `label` input will be placed in the bottom-right corner of the render.
 
-| With Unicode          | Without Unicode         |
-| --------------------- | ----------------------- |
-| ![][fig_sparsity_uni] | ![][fig_sparsity_ascii] |
-
 ## Progress bars
 
 ```python
 trm.progress(k, K, tic=None, width=None)
 ```
 
 There are many progress bar libraries available for Python. But, many of them
@@ -169,16 +146,7 @@
 stored in `tic` will be displayed. When the process is completed, the total
 elapsed time since `tic` will be displayed. If `width` is not provided, the full
 width of the current terminal window will be used.
 
 ```
  44% [/////////////////////----------------------------] -00:00:02.1
 ```
-
-
-[fig_heat_uni]: https://gitlab.com/davidwoodburn/trm/-/blob/main/figures/fig_heat_uni.png
-[fig_heat_ascii]: https://gitlab.com/davidwoodburn/trm/-/blob/main/figures/fig_heat_ascii.png
-[fig_plot]: https://gitlab.com/davidwoodburn/trm/-/blob/main/figures/fig_plot.png
-[fig_plot_1]: https://gitlab.com/davidwoodburn/trm/-/blob/main/figures/fig_plot_1.png
-[fig_plot_5]: https://gitlab.com/davidwoodburn/trm/-/blob/main/figures/fig_plot_5.png
-[fig_sparsity_uni]: https://gitlab.com/davidwoodburn/trm/-/blob/main/figures/fig_sparsity_uni.png
-[fig_sparsity_ascii]: https://gitlab.com/davidwoodburn/trm/-/blob/main/figures/fig_sparsity_ascii.png
```

