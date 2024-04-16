# Comparing `tmp/altair_express-0.1.8.tar.gz` & `tmp/altair_express-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "altair_express-0.1.8.tar", last modified: Mon Nov  7 15:56:10 2022, max compression
+gzip compressed data, was "altair_express-0.1.9.tar", last modified: Mon Nov  7 16:07:44 2022, max compression
```

## Comparing `altair_express-0.1.8.tar` & `altair_express-0.1.9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 dylanwootton   (501) staff       (20)        0 2022-11-07 15:56:10.812646 altair_express-0.1.8/
--rw-r--r--   0 dylanwootton   (501) staff       (20)      155 2022-11-01 20:59:20.000000 altair_express-0.1.8/AUTHORS.rst
--rw-r--r--   0 dylanwootton   (501) staff       (20)     3608 2022-11-01 20:59:20.000000 altair_express-0.1.8/CONTRIBUTING.rst
--rw-r--r--   0 dylanwootton   (501) staff       (20)       89 2022-11-01 20:59:20.000000 altair_express-0.1.8/HISTORY.rst
--rw-r--r--   0 dylanwootton   (501) staff       (20)     1072 2022-11-01 20:59:20.000000 altair_express-0.1.8/LICENSE
--rw-r--r--   0 dylanwootton   (501) staff       (20)      262 2022-11-01 20:59:20.000000 altair_express-0.1.8/MANIFEST.in
--rw-r--r--   0 dylanwootton   (501) staff       (20)     1791 2022-11-07 15:56:10.812801 altair_express-0.1.8/PKG-INFO
--rw-r--r--   0 dylanwootton   (501) staff       (20)      947 2022-11-01 20:59:20.000000 altair_express-0.1.8/README.rst
-drwxr-xr-x   0 dylanwootton   (501) staff       (20)        0 2022-11-07 15:56:10.798148 altair_express-0.1.8/altair_express/
--rw-r--r--   0 dylanwootton   (501) staff       (20)      238 2022-11-07 15:56:05.000000 altair_express-0.1.8/altair_express/__init__.py
--rw-r--r--   0 dylanwootton   (501) staff       (20)     2987 2022-11-07 15:12:34.000000 altair_express-0.1.8/altair_express/altair_express.py
--rw-r--r--   0 dylanwootton   (501) staff       (20)      420 2022-11-01 20:59:20.000000 altair_express-0.1.8/altair_express/cli.py
--rw-r--r--   0 dylanwootton   (501) staff       (20)     5240 2022-11-07 15:55:08.000000 altair_express-0.1.8/altair_express/distributional.py
--rw-r--r--   0 dylanwootton   (501) staff       (20)     1100 2022-11-07 15:47:29.000000 altair_express-0.1.8/altair_express/joint_plot.py
--rw-r--r--   0 dylanwootton   (501) staff       (20)     2328 2022-11-07 15:48:32.000000 altair_express-0.1.8/altair_express/pair_plot.py
--rw-r--r--   0 dylanwootton   (501) staff       (20)     1619 2022-11-07 15:54:24.000000 altair_express-0.1.8/altair_express/relational.py
--rw-r--r--   0 dylanwootton   (501) staff       (20)      974 2022-11-07 15:55:26.000000 altair_express-0.1.8/altair_express/utils.py
-drwxr-xr-x   0 dylanwootton   (501) staff       (20)        0 2022-11-07 15:56:10.800995 altair_express-0.1.8/altair_express.egg-info/
--rw-r--r--   0 dylanwootton   (501) staff       (20)     1791 2022-11-07 15:56:10.000000 altair_express-0.1.8/altair_express.egg-info/PKG-INFO
--rw-r--r--   0 dylanwootton   (501) staff       (20)      794 2022-11-07 15:56:10.000000 altair_express-0.1.8/altair_express.egg-info/SOURCES.txt
--rw-r--r--   0 dylanwootton   (501) staff       (20)        1 2022-11-07 15:56:10.000000 altair_express-0.1.8/altair_express.egg-info/dependency_links.txt
--rw-r--r--   0 dylanwootton   (501) staff       (20)       59 2022-11-07 15:56:10.000000 altair_express-0.1.8/altair_express.egg-info/entry_points.txt
--rw-r--r--   0 dylanwootton   (501) staff       (20)        1 2022-11-07 15:56:10.000000 altair_express-0.1.8/altair_express.egg-info/not-zip-safe
--rw-r--r--   0 dylanwootton   (501) staff       (20)       31 2022-11-07 15:56:10.000000 altair_express-0.1.8/altair_express.egg-info/requires.txt
--rw-r--r--   0 dylanwootton   (501) staff       (20)       15 2022-11-07 15:56:10.000000 altair_express-0.1.8/altair_express.egg-info/top_level.txt
-drwxr-xr-x   0 dylanwootton   (501) staff       (20)        0 2022-11-07 15:56:10.811089 altair_express-0.1.8/docs/
--rw-r--r--   0 dylanwootton   (501) staff       (20)      615 2022-11-01 20:59:20.000000 altair_express-0.1.8/docs/Makefile
--rw-r--r--   0 dylanwootton   (501) staff       (20)       28 2022-11-01 20:59:20.000000 altair_express-0.1.8/docs/authors.rst
--rwxr-xr-x   0 dylanwootton   (501) staff       (20)     4872 2022-11-01 20:59:20.000000 altair_express-0.1.8/docs/conf.py
--rw-r--r--   0 dylanwootton   (501) staff       (20)       33 2022-11-01 20:59:20.000000 altair_express-0.1.8/docs/contributing.rst
--rw-r--r--   0 dylanwootton   (501) staff       (20)       28 2022-11-01 20:59:20.000000 altair_express-0.1.8/docs/history.rst
--rw-r--r--   0 dylanwootton   (501) staff       (20)      311 2022-11-01 20:59:20.000000 altair_express-0.1.8/docs/index.rst
--rw-r--r--   0 dylanwootton   (501) staff       (20)     1170 2022-11-01 20:59:20.000000 altair_express-0.1.8/docs/installation.rst
--rw-r--r--   0 dylanwootton   (501) staff       (20)      776 2022-11-01 20:59:20.000000 altair_express-0.1.8/docs/make.bat
--rw-r--r--   0 dylanwootton   (501) staff       (20)       27 2022-11-01 20:59:20.000000 altair_express-0.1.8/docs/readme.rst
--rw-r--r--   0 dylanwootton   (501) staff       (20)       83 2022-11-01 20:59:20.000000 altair_express-0.1.8/docs/usage.rst
--rw-r--r--   0 dylanwootton   (501) staff       (20)      386 2022-11-07 15:56:10.813832 altair_express-0.1.8/setup.cfg
--rw-r--r--   0 dylanwootton   (501) staff       (20)     1457 2022-11-07 15:56:05.000000 altair_express-0.1.8/setup.py
-drwxr-xr-x   0 dylanwootton   (501) staff       (20)        0 2022-11-07 15:56:10.812336 altair_express-0.1.8/tests/
--rw-r--r--   0 dylanwootton   (501) staff       (20)       44 2022-11-01 20:59:20.000000 altair_express-0.1.8/tests/__init__.py
--rw-r--r--   0 dylanwootton   (501) staff       (20)      901 2022-11-01 20:59:20.000000 altair_express-0.1.8/tests/test_altair_express.py
+drwxr-xr-x   0 dylanwootton   (501) staff       (20)        0 2022-11-07 16:07:44.766252 altair_express-0.1.9/
+-rw-r--r--   0 dylanwootton   (501) staff       (20)      155 2022-11-01 20:59:20.000000 altair_express-0.1.9/AUTHORS.rst
+-rw-r--r--   0 dylanwootton   (501) staff       (20)     3608 2022-11-01 20:59:20.000000 altair_express-0.1.9/CONTRIBUTING.rst
+-rw-r--r--   0 dylanwootton   (501) staff       (20)       89 2022-11-01 20:59:20.000000 altair_express-0.1.9/HISTORY.rst
+-rw-r--r--   0 dylanwootton   (501) staff       (20)     1072 2022-11-01 20:59:20.000000 altair_express-0.1.9/LICENSE
+-rw-r--r--   0 dylanwootton   (501) staff       (20)      262 2022-11-01 20:59:20.000000 altair_express-0.1.9/MANIFEST.in
+-rw-r--r--   0 dylanwootton   (501) staff       (20)     1791 2022-11-07 16:07:44.766395 altair_express-0.1.9/PKG-INFO
+-rw-r--r--   0 dylanwootton   (501) staff       (20)      947 2022-11-01 20:59:20.000000 altair_express-0.1.9/README.rst
+drwxr-xr-x   0 dylanwootton   (501) staff       (20)        0 2022-11-07 16:07:44.757882 altair_express-0.1.9/altair_express/
+-rw-r--r--   0 dylanwootton   (501) staff       (20)      238 2022-11-07 16:07:36.000000 altair_express-0.1.9/altair_express/__init__.py
+-rw-r--r--   0 dylanwootton   (501) staff       (20)     2987 2022-11-07 15:12:34.000000 altair_express-0.1.9/altair_express/altair_express.py
+-rw-r--r--   0 dylanwootton   (501) staff       (20)      420 2022-11-01 20:59:20.000000 altair_express-0.1.9/altair_express/cli.py
+-rw-r--r--   0 dylanwootton   (501) staff       (20)     4527 2022-11-07 16:07:05.000000 altair_express-0.1.9/altair_express/distributional.py
+-rw-r--r--   0 dylanwootton   (501) staff       (20)     1100 2022-11-07 15:47:29.000000 altair_express-0.1.9/altair_express/joint_plot.py
+-rw-r--r--   0 dylanwootton   (501) staff       (20)     2328 2022-11-07 15:48:32.000000 altair_express-0.1.9/altair_express/pair_plot.py
+-rw-r--r--   0 dylanwootton   (501) staff       (20)     1619 2022-11-07 15:54:24.000000 altair_express-0.1.9/altair_express/relational.py
+-rw-r--r--   0 dylanwootton   (501) staff       (20)      974 2022-11-07 15:55:26.000000 altair_express-0.1.9/altair_express/utils.py
+drwxr-xr-x   0 dylanwootton   (501) staff       (20)        0 2022-11-07 16:07:44.760644 altair_express-0.1.9/altair_express.egg-info/
+-rw-r--r--   0 dylanwootton   (501) staff       (20)     1791 2022-11-07 16:07:44.000000 altair_express-0.1.9/altair_express.egg-info/PKG-INFO
+-rw-r--r--   0 dylanwootton   (501) staff       (20)      794 2022-11-07 16:07:44.000000 altair_express-0.1.9/altair_express.egg-info/SOURCES.txt
+-rw-r--r--   0 dylanwootton   (501) staff       (20)        1 2022-11-07 16:07:44.000000 altair_express-0.1.9/altair_express.egg-info/dependency_links.txt
+-rw-r--r--   0 dylanwootton   (501) staff       (20)       59 2022-11-07 16:07:44.000000 altair_express-0.1.9/altair_express.egg-info/entry_points.txt
+-rw-r--r--   0 dylanwootton   (501) staff       (20)        1 2022-11-07 16:07:44.000000 altair_express-0.1.9/altair_express.egg-info/not-zip-safe
+-rw-r--r--   0 dylanwootton   (501) staff       (20)       31 2022-11-07 16:07:44.000000 altair_express-0.1.9/altair_express.egg-info/requires.txt
+-rw-r--r--   0 dylanwootton   (501) staff       (20)       15 2022-11-07 16:07:44.000000 altair_express-0.1.9/altair_express.egg-info/top_level.txt
+drwxr-xr-x   0 dylanwootton   (501) staff       (20)        0 2022-11-07 16:07:44.765327 altair_express-0.1.9/docs/
+-rw-r--r--   0 dylanwootton   (501) staff       (20)      615 2022-11-01 20:59:20.000000 altair_express-0.1.9/docs/Makefile
+-rw-r--r--   0 dylanwootton   (501) staff       (20)       28 2022-11-01 20:59:20.000000 altair_express-0.1.9/docs/authors.rst
+-rwxr-xr-x   0 dylanwootton   (501) staff       (20)     4872 2022-11-01 20:59:20.000000 altair_express-0.1.9/docs/conf.py
+-rw-r--r--   0 dylanwootton   (501) staff       (20)       33 2022-11-01 20:59:20.000000 altair_express-0.1.9/docs/contributing.rst
+-rw-r--r--   0 dylanwootton   (501) staff       (20)       28 2022-11-01 20:59:20.000000 altair_express-0.1.9/docs/history.rst
+-rw-r--r--   0 dylanwootton   (501) staff       (20)      311 2022-11-01 20:59:20.000000 altair_express-0.1.9/docs/index.rst
+-rw-r--r--   0 dylanwootton   (501) staff       (20)     1170 2022-11-01 20:59:20.000000 altair_express-0.1.9/docs/installation.rst
+-rw-r--r--   0 dylanwootton   (501) staff       (20)      776 2022-11-01 20:59:20.000000 altair_express-0.1.9/docs/make.bat
+-rw-r--r--   0 dylanwootton   (501) staff       (20)       27 2022-11-01 20:59:20.000000 altair_express-0.1.9/docs/readme.rst
+-rw-r--r--   0 dylanwootton   (501) staff       (20)       83 2022-11-01 20:59:20.000000 altair_express-0.1.9/docs/usage.rst
+-rw-r--r--   0 dylanwootton   (501) staff       (20)      386 2022-11-07 16:07:44.767026 altair_express-0.1.9/setup.cfg
+-rw-r--r--   0 dylanwootton   (501) staff       (20)     1457 2022-11-07 16:07:36.000000 altair_express-0.1.9/setup.py
+drwxr-xr-x   0 dylanwootton   (501) staff       (20)        0 2022-11-07 16:07:44.765985 altair_express-0.1.9/tests/
+-rw-r--r--   0 dylanwootton   (501) staff       (20)       44 2022-11-01 20:59:20.000000 altair_express-0.1.9/tests/__init__.py
+-rw-r--r--   0 dylanwootton   (501) staff       (20)      901 2022-11-01 20:59:20.000000 altair_express-0.1.9/tests/test_altair_express.py
```

### Comparing `altair_express-0.1.8/CONTRIBUTING.rst` & `altair_express-0.1.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `altair_express-0.1.8/LICENSE` & `altair_express-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `altair_express-0.1.8/PKG-INFO` & `altair_express-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: altair_express
-Version: 0.1.8
+Version: 0.1.9
 Summary: Create interactive data visualizations in one line of code.
 Home-page: https://github.com/dwootton/altair_express
 Author: Dylan Wootton
 Author-email: dwootton@mit.edu
 License: MIT license
 Keywords: altair_express
 Platform: UNKNOWN
```

### Comparing `altair_express-0.1.8/README.rst` & `altair_express-0.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `altair_express-0.1.8/altair_express/altair_express.py` & `altair_express-0.1.9/altair_express/altair_express.py`

 * *Files identical despite different names*

### Comparing `altair_express-0.1.8/altair_express/distributional.py` & `altair_express-0.1.9/altair_express/distributional.py`

 * *Files 12% similar despite different names*

```diff
@@ -32,15 +32,15 @@
               ) 
     layers['bg'] = alt.Chart(data).mark_bar(color='lightgray').encode(
         alt.X(f'{x}:Q', bin=True, axis=xAxis),alt.Y('count()',axis=yAxis)
       )
     
     if interactive:
 
-      x_brush = alt.selection_interval(encodings=['x'],resolve="union",name='x_brush')
+      x_brush = alt.selection_interval(encodings=['x'],resolve="union",name='brush')
       
       if isinstance(interactive,alt.Selection):
         x_brush = interactive     
       
       layers['fg'] =  layers['fg'].add_selection(x_brush)
       filters.append(x_brush)
 
@@ -51,39 +51,22 @@
               ) 
     layers['bg'] = alt.Chart(data).mark_bar(color='lightgray').encode(
         alt.Y(f'{y}:Q', bin=True, axis=yAxis),alt.X('count()',axis=xAxis)
       )
     
     if interactive:
 
-      y_brush = alt.selection_interval(encodings=['y'],resolve="union",name='y_brush')
+      y_brush = alt.selection_interval(encodings=['y'],resolve="union",name='brush')
       
       if isinstance(interactive,alt.Selection):
         y_brush = interactive     
 
       
       layers['fg'] =  layers['fg'].add_selection(y_brush)
       filters.append(y_brush)
-
-      print(len(filters))
-
-    
-  # elif x is None and y is not None:
-
-  #   chart =  alt.Chart(data).mark_bar(color=fill).encode(
-  #     alt.Y(f'{y}:Q', bin=True, axis=yAxis),alt.X('count()',axis=xAxis)
-  #       )
-  #   if interactive:
-  #     y_brush = alt.selection_interval(encodings=['y'],resolve="global",name='y_brush')
-  #     if isinstance(interactive,alt.Selection):
-  #       y_brush = interactive 
-  #     chart = chart.mark_bar(color='lightgray')
-  #     chart = chart + alt.Chart(data).mark_bar(color=fill).encode(
-  #         alt.Y(f'{y}:Q', bin=True, axis=yAxis),alt.X('count()',axis=xAxis)
-  #     ).add_selection(y_brush).transform_filter(y_brush)
   
 
   if filters:
      for filter in filters:
         layers['fg'] = layers['fg'].transform_filter(filter)
 
   chart = layers['bg'] + layers['fg'] 
@@ -112,15 +95,14 @@
 
   for index,variable in enumerate(facet_vars):
     # filter to unique value
     base = alt.Chart(data=data)
 
     # filter to only one variable
     if variable is not None:
-      print(f'filtering to {variable}')
       base=base.transform_filter(
           alt.FieldEqualPredicate(field=groupby, equal=variable)
       )
 
     if yAxis is None:
       if index == 0:
         yAxis = alt.Axis(grid=False, ticks=True)
```

### Comparing `altair_express-0.1.8/altair_express/joint_plot.py` & `altair_express-0.1.9/altair_express/joint_plot.py`

 * *Files identical despite different names*

### Comparing `altair_express-0.1.8/altair_express/pair_plot.py` & `altair_express-0.1.9/altair_express/pair_plot.py`

 * *Files identical despite different names*

### Comparing `altair_express-0.1.8/altair_express/relational.py` & `altair_express-0.1.9/altair_express/relational.py`

 * *Files identical despite different names*

### Comparing `altair_express-0.1.8/altair_express/utils.py` & `altair_express-0.1.9/altair_express/utils.py`

 * *Files identical despite different names*

### Comparing `altair_express-0.1.8/altair_express.egg-info/PKG-INFO` & `altair_express-0.1.9/altair_express.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: altair-express
-Version: 0.1.8
+Version: 0.1.9
 Summary: Create interactive data visualizations in one line of code.
 Home-page: https://github.com/dwootton/altair_express
 Author: Dylan Wootton
 Author-email: dwootton@mit.edu
 License: MIT license
 Keywords: altair_express
 Platform: UNKNOWN
```

### Comparing `altair_express-0.1.8/altair_express.egg-info/SOURCES.txt` & `altair_express-0.1.9/altair_express.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `altair_express-0.1.8/docs/Makefile` & `altair_express-0.1.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `altair_express-0.1.8/docs/conf.py` & `altair_express-0.1.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `altair_express-0.1.8/docs/installation.rst` & `altair_express-0.1.9/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `altair_express-0.1.8/docs/make.bat` & `altair_express-0.1.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `altair_express-0.1.8/setup.py` & `altair_express-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,10 +40,10 @@
     include_package_data=True,
     keywords='altair_express',
     name='altair_express',
     packages=find_packages(include=['altair_express', 'altair_express.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/dwootton/altair_express',
-    version='0.1.8',
+    version='0.1.9',
     zip_safe=False,
 )
```

### Comparing `altair_express-0.1.8/tests/test_altair_express.py` & `altair_express-0.1.9/tests/test_altair_express.py`

 * *Files identical despite different names*

