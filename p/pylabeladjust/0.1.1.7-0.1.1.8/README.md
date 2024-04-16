# Comparing `tmp/pylabeladjust-0.1.1.7.tar.gz` & `tmp/pylabeladjust-0.1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylabeladjust-0.1.1.7.tar", max compression
+gzip compressed data, was "pylabeladjust-0.1.1.8.tar", max compression
```

## Comparing `pylabeladjust-0.1.1.7.tar` & `pylabeladjust-0.1.1.8.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    35149 2024-04-12 15:51:27.765165 pylabeladjust-0.1.1.7/LICENSE
--rw-r--r--   0        0        0     4067 2024-04-15 20:18:51.282089 pylabeladjust-0.1.1.7/README.md
--rw-r--r--   0        0        0       61 2024-04-15 12:28:42.751523 pylabeladjust-0.1.1.7/pylabeladjust/__init__.py
--rw-r--r--   0        0        0    11855 2024-04-13 01:41:05.089290 pylabeladjust-0.1.1.7/pylabeladjust/core.py
--rw-r--r--   0        0        0      434 2024-04-15 20:30:58.912202 pylabeladjust-0.1.1.7/pyproject.toml
--rw-r--r--   0        0        0     5055 1970-01-01 00:00:00.000000 pylabeladjust-0.1.1.7/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-12 15:51:27.765165 pylabeladjust-0.1.1.8/LICENSE
+-rw-r--r--   0        0        0     6927 2024-04-16 09:14:02.278820 pylabeladjust-0.1.1.8/README.md
+-rw-r--r--   0        0        0       61 2024-04-15 12:28:42.751523 pylabeladjust-0.1.1.8/pylabeladjust/__init__.py
+-rw-r--r--   0        0        0    11855 2024-04-13 01:41:05.089290 pylabeladjust-0.1.1.8/pylabeladjust/core.py
+-rw-r--r--   0        0        0      438 2024-04-16 09:15:08.980441 pylabeladjust-0.1.1.8/pyproject.toml
+-rw-r--r--   0        0        0     7915 1970-01-01 00:00:00.000000 pylabeladjust-0.1.1.8/PKG-INFO
```

### Comparing `pylabeladjust-0.1.1.7/LICENSE` & `pylabeladjust-0.1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pylabeladjust-0.1.1.7/README.md` & `pylabeladjust-0.1.1.8/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # pylabeladjust
 
-`pylabeladjust` is a port of Gephi's Label-Adjust algorithm to python. It makes labels in matplotlib-plots not overlap by carefully pushing them apart, as illustrated by this video:
+`pylabeladjust` is a port of [Gephi's really good Label-Adjust](https://github.com/gephi/gephi/blob/760df9a6a8389c63fb6df524cbff9003975d57aa/modules/LayoutPlugin/src/main/java/org/gephi/layout/plugin/labelAdjust/LabelAdjust.java) algorithm by Mathieu Jacomy to python. It makes labels in matplotlib-plots not overlap by carefully pushing them apart, as illustrated by this video:
 
 <img src="https://raw.githubusercontent.com/MNoichl/pylabeladjust/main/images/layout_process_texts.gif" width="672" />
 
-Pylabeladjust uses `pyqtree` in the background to be efficient. The setup of the `pylabeladjust`-plotting code takes inspiration from `adjust_text`. this package
+Pylabeladjust uses [`pyqtree`](https://github.com/karimbahgat/Pyqtree), by Karim Bahgat, in the background for efficient overlap-querying. The setup of the `pylabeladjust`-plotting code takes inspiration from [`adjust_text`](https://github.com/Phlya/adjustText), by Ilya Flyamer.
 
 # When to use `pylabeladjust`
 
-`pylabeladjust` currently is meant for cases in which it is fine for your labels to move a little bit as in network-graphics or UMAP/t-SNE-plots, without any additional constraints. It should be able to handle cases where you have large numbers (1000+) of labels with a lot of overlap in reasonably small amounts of time. This makes it an alternative to `adjust_text` for this specific use-case, which in my experience struggles with many-abel/large overlap scenarios. If you need your labels to conform to more complicated constraints, like not overlapping particular points you might want to look into `adjust_text` and ... , which both can be very useful!
+`pylabeladjust` currently is meant for cases in which it is fine for your labels to move around little bit as in network-graphics or UMAP/t-SNE-plots, without any additional constraints. It should be able to handle cases where you have large numbers (1000+) of labels with a lot of overlap in reasonably small amounts of time. This makes it an alternative to `adjust_text` for this specific use-case. If you need your labels to conform to more complicated constraints, like not overlapping particular points you might want to look into [`adjust_text`](https://github.com/Phlya/adjustText) or [`textalloc`](https://github.com/ckjellson/textalloc) , which both can be very useful!
 
 
 # Installation
 
 Installation should be straightforward using:
 
 ````
@@ -36,22 +36,51 @@
 rectangles_adjusted = adjust_texts(texts, speed=.03, max_iterations=250, margin_percentage=6, radius_scale=1.03)
 plt.show()
 ```
 
 
 Result:
 
-<img src="images/before_after_texts.gif" width="672" />
+<img src="https://raw.githubusercontent.com/MNoichl/pylabeladjust/main/images/text_adjustment_results.png" width="672" />
 
 Here's what the parameters mean:
 
 
 * `texts` (List[matplotlib.text.Text]): A list of text objects to be adjusted.
-* speed (float, optional): The speed of the adjustment process (movement, measured on the scale of the data). If left blank, speed is set to halve the size of the mean text-width. If your labels end up all over the place, you might want to decrease this value. If it looks like the adjustment didn't change much, although the algorithm spent dozens of seconds optimizing, the value might need to be increased.
-* adjust_by_size (bool, optional): Whether to adjust the texts based on their sizes. Defaults to True. This makes the positions of large text-blocks more robust, and shuffles smaller ones around more, which can result in a structurally more convincing layout, and speeds up the algorithms. You should check that small stuff didn't get shuffled awayy *too* far though. 
-* radius_scale (float, optional): The scale factor for the radius used in the adjustment process. Defaults to 1.1.
-* max_iterations (int, optional): The maximum number of iterations for the adjustment process. Defaults to 200. Increase if your layout still has overlaps after running the adjustment. This can usually be increased liberally because once there is little overlap anymore, the remaining iterations are very fast.
-* plot_progress (bool, optional): Whether to print out plots of the progress of the adjustment process. Defaults to False, and is mostly useful for debugging.
-* margin_percentage (int, optional): The percentage of margin to be added around the adjusted texts. Calculated from the width of rectangles. Defaults to 10.
-* return_optimization_process (bool, optional): Whether to return the optimization process, a list of dataframes of all the positions the texts went through in the optimization process. Defaults to False.
+* `speed` (float, optional): The speed of the adjustment process (movement, measured on the scale of the data). If left blank, speed is set to halve the size of the mean text-width. If your labels end up all over the place, you might want to decrease this value. If it looks like the adjustment didn't change much, although the algorithm spent dozens of seconds optimizing, the value might need to be increased.
+* `adjust_by_size` (bool, optional): Whether to adjust the texts based on their sizes. Defaults to True. This makes the positions of large text-blocks more robust, and shuffles smaller ones around more, which can result in a structurally more convincing layout, and speeds up the algorithms. You should check that small stuff didn't get shuffled awayy *too* far though. 
+* `radius_scale` (float, optional): The scale factor for the radius used in the adjustment process. Defaults to 1.1.
+* `max_iterations` (int, optional): The maximum number of iterations for the adjustment process. Defaults to 200. Increase if your layout still has overlaps after running the adjustment. This can usually be increased liberally because once there is little overlap anymore, the remaining iterations are very fast.
+* `plot_progress` (bool, optional): Whether to print out plots of the progress of the adjustment process. Defaults to False, and is mostly useful for debugging.
+* `margin_percentage` (int, optional): The percentage of margin to be added around the adjusted texts. Calculated from the width of rectangles. Defaults to 10.
+* `return_optimization_process` (bool, optional): Whether to return the optimization process, a list of dataframes of all the positions the texts went through in the optimization process. Defaults to False.
 
-The function edits your `texts` object in place, so you can just resume plotting. It also will return a dataframe of the new positions, and if `return_optimization_process` is set to true, a list of dataframes of the intermediate steps.
+The function edits your `texts` object in place, so you can just resume plotting. It also will return a dataframe of the new positions, and if `return_optimization_process` is set to true, a list of dataframes of the intermediate steps.
+
+
+
+We can also adjust rectangles which are not labels directly. In that case, the function expects a `pandas`-dataframe, with the columns `x`,`y`,`height`,`width`.
+The syntax will look very similar to above:
+
+```
+rectangles_adjusted, optimization_process = adjust_labels(data, adjust_by_size=True, radius_scale=1.1, max_iterations=250, margin_percentage=5, return_optimization_process=True)
+```
+
+The parameters of this function are:
+
+* `rectangle_data` (DataFrame): A `pandas`-dataframe, with the columns `x`,`y`,`height`,`width`.
+* `speed` (float, optional): The speed of the adjustment process (movement, measured on the scale of the data). If left blank, speed is set to halve the size of the mean text-width. If your labels end up all over the place, you might want to decrease this value. If it looks like the adjustment didn't change much, although the algorithm spent dozens of seconds optimizing, the value might need to be increased.
+* `adjust_by_size` (bool, optional): Whether to adjust the texts based on their sizes. Defaults to True. This makes the positions of large text-blocks more robust, and shuffles smaller ones around more, which can result in a structurally more convincing layout, and speeds up the algorithms. You should check that small stuff didn't get shuffled awayy *too* far though. 
+* `radius_scale` (float, optional): The scale factor for the radius used in the adjustment process. Defaults to 1.1.
+* `max_iterations` (int, optional): The maximum number of iterations for the adjustment process. Defaults to 200. Increase if your layout still has overlaps after running the adjustment. This can usually be increased liberally because once there is little overlap anymore, the remaining iterations are very fast.
+* `plot_progress` (bool, optional): Whether to print out plots of the progress of the adjustment process. Defaults to False, and is mostly useful for debugging.
+* `margin_percentage` (int, optional): The percentage of margin to be added around the adjusted texts. Calculated from the width of rectangles. Defaults to 10.
+* `return_optimization_process` (bool, optional): Whether to return the optimization process, a list of dataframes of all the positions the texts went through in the optimization process. Defaults to False.
+
+
+<img src="https://raw.githubusercontent.com/MNoichl/pylabeladjust/main/images/layout_process_rectangles.gif" width="672" />
+
+
+
+# To-Do
+* Early stopping
+* Speed decay (?)
```

### Comparing `pylabeladjust-0.1.1.7/pylabeladjust/core.py` & `pylabeladjust-0.1.1.8/pylabeladjust/core.py`

 * *Files identical despite different names*

