# Comparing `tmp/pylabeladjust-0.1.1.8.tar.gz` & `tmp/pylabeladjust-0.1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylabeladjust-0.1.1.8.tar", max compression
+gzip compressed data, was "pylabeladjust-0.1.1.9.tar", max compression
```

## Comparing `pylabeladjust-0.1.1.8.tar` & `pylabeladjust-0.1.1.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    35149 2024-04-12 15:51:27.765165 pylabeladjust-0.1.1.8/LICENSE
--rw-r--r--   0        0        0     6927 2024-04-16 09:14:02.278820 pylabeladjust-0.1.1.8/README.md
--rw-r--r--   0        0        0       61 2024-04-15 12:28:42.751523 pylabeladjust-0.1.1.8/pylabeladjust/__init__.py
--rw-r--r--   0        0        0    11855 2024-04-13 01:41:05.089290 pylabeladjust-0.1.1.8/pylabeladjust/core.py
--rw-r--r--   0        0        0      438 2024-04-16 09:15:08.980441 pylabeladjust-0.1.1.8/pyproject.toml
--rw-r--r--   0        0        0     7915 1970-01-01 00:00:00.000000 pylabeladjust-0.1.1.8/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-12 15:51:27.765165 pylabeladjust-0.1.1.9/LICENSE
+-rw-r--r--   0        0        0     6924 2024-04-16 09:25:22.824669 pylabeladjust-0.1.1.9/README.md
+-rw-r--r--   0        0        0       61 2024-04-15 12:28:42.751523 pylabeladjust-0.1.1.9/pylabeladjust/__init__.py
+-rw-r--r--   0        0        0    11855 2024-04-13 01:41:05.089290 pylabeladjust-0.1.1.9/pylabeladjust/core.py
+-rw-r--r--   0        0        0      438 2024-04-16 09:25:33.621587 pylabeladjust-0.1.1.9/pyproject.toml
+-rw-r--r--   0        0        0     7912 1970-01-01 00:00:00.000000 pylabeladjust-0.1.1.9/PKG-INFO
```

### Comparing `pylabeladjust-0.1.1.8/LICENSE` & `pylabeladjust-0.1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pylabeladjust-0.1.1.8/README.md` & `pylabeladjust-0.1.1.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -22,36 +22,36 @@
 # Usage
 
 The full usage of the package is demonstrated in the `examples.ipynb` notebook. Basic usage might look like this:
 
 
 ```
 fig, ax = plt.subplots(figsize=(15, 15))
-ax.scatter(data['x'], data['y'], s=20, alpha=.0, c='#a7510f') # plot a transparant scatterplot, to make the albels show up.
+ax.scatter(data['x'], data['y'], s=20, alpha=.0, c='#a7510f') # plot a transparant scatterplot, to make the labels show up.
 texts = []
 for i, row in data.iterrows():
     texts.append(ax.text(row['x'], row['y'], textwrap.fill(row['title'],25) , fontsize=row['fontsize'],ma='left',fontweight=row['fontweight'],zorder=10))
 fig.canvas.draw()
 
         
 rectangles_adjusted = adjust_texts(texts, speed=.03, max_iterations=250, margin_percentage=6, radius_scale=1.03)
 plt.show()
 ```
 
 
 Result:
 
-<img src="https://raw.githubusercontent.com/MNoichl/pylabeladjust/main/images/text_adjustment_results.png" width="672" />
+<img src="https://raw.githubusercontent.com/MNoichl/pylabeladjust/main/images/text_adjustment_result.png" width="672" />
 
 Here's what the parameters mean:
 
 
 * `texts` (List[matplotlib.text.Text]): A list of text objects to be adjusted.
 * `speed` (float, optional): The speed of the adjustment process (movement, measured on the scale of the data). If left blank, speed is set to halve the size of the mean text-width. If your labels end up all over the place, you might want to decrease this value. If it looks like the adjustment didn't change much, although the algorithm spent dozens of seconds optimizing, the value might need to be increased.
-* `adjust_by_size` (bool, optional): Whether to adjust the texts based on their sizes. Defaults to True. This makes the positions of large text-blocks more robust, and shuffles smaller ones around more, which can result in a structurally more convincing layout, and speeds up the algorithms. You should check that small stuff didn't get shuffled awayy *too* far though. 
+* `adjust_by_size` (bool, optional): Whether to adjust the texts based on their sizes. Defaults to True. This makes the positions of large text-blocks more robust, and shuffles smaller ones around more, which can result in a structurally more convincing layout, and speeds up the algorithms. You should check that small stuff didn't get shuffled away *too* far though. 
 * `radius_scale` (float, optional): The scale factor for the radius used in the adjustment process. Defaults to 1.1.
 * `max_iterations` (int, optional): The maximum number of iterations for the adjustment process. Defaults to 200. Increase if your layout still has overlaps after running the adjustment. This can usually be increased liberally because once there is little overlap anymore, the remaining iterations are very fast.
 * `plot_progress` (bool, optional): Whether to print out plots of the progress of the adjustment process. Defaults to False, and is mostly useful for debugging.
 * `margin_percentage` (int, optional): The percentage of margin to be added around the adjusted texts. Calculated from the width of rectangles. Defaults to 10.
 * `return_optimization_process` (bool, optional): Whether to return the optimization process, a list of dataframes of all the positions the texts went through in the optimization process. Defaults to False.
 
 The function edits your `texts` object in place, so you can just resume plotting. It also will return a dataframe of the new positions, and if `return_optimization_process` is set to true, a list of dataframes of the intermediate steps.
@@ -65,15 +65,15 @@
 rectangles_adjusted, optimization_process = adjust_labels(data, adjust_by_size=True, radius_scale=1.1, max_iterations=250, margin_percentage=5, return_optimization_process=True)
 ```
 
 The parameters of this function are:
 
 * `rectangle_data` (DataFrame): A `pandas`-dataframe, with the columns `x`,`y`,`height`,`width`.
 * `speed` (float, optional): The speed of the adjustment process (movement, measured on the scale of the data). If left blank, speed is set to halve the size of the mean text-width. If your labels end up all over the place, you might want to decrease this value. If it looks like the adjustment didn't change much, although the algorithm spent dozens of seconds optimizing, the value might need to be increased.
-* `adjust_by_size` (bool, optional): Whether to adjust the texts based on their sizes. Defaults to True. This makes the positions of large text-blocks more robust, and shuffles smaller ones around more, which can result in a structurally more convincing layout, and speeds up the algorithms. You should check that small stuff didn't get shuffled awayy *too* far though. 
+* `adjust_by_size` (bool, optional): Whether to adjust the texts based on their sizes. Defaults to True. This makes the positions of large text-blocks more robust, and shuffles smaller ones around more, which can result in a structurally more convincing layout, and speeds up the algorithms. You should check that small stuff didn't get shuffled away *too* far though. 
 * `radius_scale` (float, optional): The scale factor for the radius used in the adjustment process. Defaults to 1.1.
 * `max_iterations` (int, optional): The maximum number of iterations for the adjustment process. Defaults to 200. Increase if your layout still has overlaps after running the adjustment. This can usually be increased liberally because once there is little overlap anymore, the remaining iterations are very fast.
 * `plot_progress` (bool, optional): Whether to print out plots of the progress of the adjustment process. Defaults to False, and is mostly useful for debugging.
 * `margin_percentage` (int, optional): The percentage of margin to be added around the adjusted texts. Calculated from the width of rectangles. Defaults to 10.
 * `return_optimization_process` (bool, optional): Whether to return the optimization process, a list of dataframes of all the positions the texts went through in the optimization process. Defaults to False.
```

### Comparing `pylabeladjust-0.1.1.8/pylabeladjust/core.py` & `pylabeladjust-0.1.1.9/pylabeladjust/core.py`

 * *Files identical despite different names*

### Comparing `pylabeladjust-0.1.1.8/PKG-INFO` & `pylabeladjust-0.1.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylabeladjust
-Version: 0.1.1.8
+Version: 0.1.1.9
 Summary: `pylabeladjust` is a port of Gephi's Label-Adjust algorithm to python.
 License: MIT
 Author: MNoichl
 Author-email: noichlmax@hotmail.co.uk
 Requires-Python: >=3.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -47,36 +47,36 @@
 # Usage
 
 The full usage of the package is demonstrated in the `examples.ipynb` notebook. Basic usage might look like this:
 
 
 ```
 fig, ax = plt.subplots(figsize=(15, 15))
-ax.scatter(data['x'], data['y'], s=20, alpha=.0, c='#a7510f') # plot a transparant scatterplot, to make the albels show up.
+ax.scatter(data['x'], data['y'], s=20, alpha=.0, c='#a7510f') # plot a transparant scatterplot, to make the labels show up.
 texts = []
 for i, row in data.iterrows():
     texts.append(ax.text(row['x'], row['y'], textwrap.fill(row['title'],25) , fontsize=row['fontsize'],ma='left',fontweight=row['fontweight'],zorder=10))
 fig.canvas.draw()
 
         
 rectangles_adjusted = adjust_texts(texts, speed=.03, max_iterations=250, margin_percentage=6, radius_scale=1.03)
 plt.show()
 ```
 
 
 Result:
 
-<img src="https://raw.githubusercontent.com/MNoichl/pylabeladjust/main/images/text_adjustment_results.png" width="672" />
+<img src="https://raw.githubusercontent.com/MNoichl/pylabeladjust/main/images/text_adjustment_result.png" width="672" />
 
 Here's what the parameters mean:
 
 
 * `texts` (List[matplotlib.text.Text]): A list of text objects to be adjusted.
 * `speed` (float, optional): The speed of the adjustment process (movement, measured on the scale of the data). If left blank, speed is set to halve the size of the mean text-width. If your labels end up all over the place, you might want to decrease this value. If it looks like the adjustment didn't change much, although the algorithm spent dozens of seconds optimizing, the value might need to be increased.
-* `adjust_by_size` (bool, optional): Whether to adjust the texts based on their sizes. Defaults to True. This makes the positions of large text-blocks more robust, and shuffles smaller ones around more, which can result in a structurally more convincing layout, and speeds up the algorithms. You should check that small stuff didn't get shuffled awayy *too* far though. 
+* `adjust_by_size` (bool, optional): Whether to adjust the texts based on their sizes. Defaults to True. This makes the positions of large text-blocks more robust, and shuffles smaller ones around more, which can result in a structurally more convincing layout, and speeds up the algorithms. You should check that small stuff didn't get shuffled away *too* far though. 
 * `radius_scale` (float, optional): The scale factor for the radius used in the adjustment process. Defaults to 1.1.
 * `max_iterations` (int, optional): The maximum number of iterations for the adjustment process. Defaults to 200. Increase if your layout still has overlaps after running the adjustment. This can usually be increased liberally because once there is little overlap anymore, the remaining iterations are very fast.
 * `plot_progress` (bool, optional): Whether to print out plots of the progress of the adjustment process. Defaults to False, and is mostly useful for debugging.
 * `margin_percentage` (int, optional): The percentage of margin to be added around the adjusted texts. Calculated from the width of rectangles. Defaults to 10.
 * `return_optimization_process` (bool, optional): Whether to return the optimization process, a list of dataframes of all the positions the texts went through in the optimization process. Defaults to False.
 
 The function edits your `texts` object in place, so you can just resume plotting. It also will return a dataframe of the new positions, and if `return_optimization_process` is set to true, a list of dataframes of the intermediate steps.
@@ -90,15 +90,15 @@
 rectangles_adjusted, optimization_process = adjust_labels(data, adjust_by_size=True, radius_scale=1.1, max_iterations=250, margin_percentage=5, return_optimization_process=True)
 ```
 
 The parameters of this function are:
 
 * `rectangle_data` (DataFrame): A `pandas`-dataframe, with the columns `x`,`y`,`height`,`width`.
 * `speed` (float, optional): The speed of the adjustment process (movement, measured on the scale of the data). If left blank, speed is set to halve the size of the mean text-width. If your labels end up all over the place, you might want to decrease this value. If it looks like the adjustment didn't change much, although the algorithm spent dozens of seconds optimizing, the value might need to be increased.
-* `adjust_by_size` (bool, optional): Whether to adjust the texts based on their sizes. Defaults to True. This makes the positions of large text-blocks more robust, and shuffles smaller ones around more, which can result in a structurally more convincing layout, and speeds up the algorithms. You should check that small stuff didn't get shuffled awayy *too* far though. 
+* `adjust_by_size` (bool, optional): Whether to adjust the texts based on their sizes. Defaults to True. This makes the positions of large text-blocks more robust, and shuffles smaller ones around more, which can result in a structurally more convincing layout, and speeds up the algorithms. You should check that small stuff didn't get shuffled away *too* far though. 
 * `radius_scale` (float, optional): The scale factor for the radius used in the adjustment process. Defaults to 1.1.
 * `max_iterations` (int, optional): The maximum number of iterations for the adjustment process. Defaults to 200. Increase if your layout still has overlaps after running the adjustment. This can usually be increased liberally because once there is little overlap anymore, the remaining iterations are very fast.
 * `plot_progress` (bool, optional): Whether to print out plots of the progress of the adjustment process. Defaults to False, and is mostly useful for debugging.
 * `margin_percentage` (int, optional): The percentage of margin to be added around the adjusted texts. Calculated from the width of rectangles. Defaults to 10.
 * `return_optimization_process` (bool, optional): Whether to return the optimization process, a list of dataframes of all the positions the texts went through in the optimization process. Defaults to False.
```

