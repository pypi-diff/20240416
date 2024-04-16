# Comparing `tmp/fa2_modified-0.3.7.tar.gz` & `tmp/fa2_modified-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fa2_modified-0.3.7.tar", last modified: Tue Apr 16 17:49:52 2024, max compression
+gzip compressed data, was "fa2_modified-0.3.8.tar", last modified: Tue Apr 16 17:52:56 2024, max compression
```

## Comparing `fa2_modified-0.3.7.tar` & `fa2_modified-0.3.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:49:52.781113 fa2_modified-0.3.7/
--rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-04-16 17:49:41.000000 fa2_modified-0.3.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-16 17:49:41.000000 fa2_modified-0.3.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7890 2024-04-16 17:49:52.781113 fa2_modified-0.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-04-16 17:49:41.000000 fa2_modified-0.3.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:49:52.777113 fa2_modified-0.3.7/examples/
--rw-r--r--   0 runner    (1001) docker     (127)   270891 2024-04-16 17:49:41.000000 fa2_modified-0.3.7/examples/forceatlas2-layout.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    80071 2024-04-16 17:49:41.000000 fa2_modified-0.3.7/examples/geometric_graph.png
--rw-r--r--   0 runner    (1001) docker     (127)    68224 2024-04-16 17:49:41.000000 fa2_modified-0.3.7/examples/grid_graph.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:49:52.777113 fa2_modified-0.3.7/fa2_modified/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-16 17:49:41.000000 fa2_modified-0.3.7/fa2_modified/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11259 2024-04-16 17:49:41.000000 fa2_modified-0.3.7/fa2_modified/fa2util.py
--rw-r--r--   0 runner    (1001) docker     (127)    11368 2024-04-16 17:49:41.000000 fa2_modified-0.3.7/fa2_modified/forceatlas2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:49:52.781113 fa2_modified-0.3.7/fa2_modified.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7890 2024-04-16 17:49:52.000000 fa2_modified-0.3.7/fa2_modified.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-16 17:49:52.000000 fa2_modified-0.3.7/fa2_modified.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 17:49:52.000000 fa2_modified-0.3.7/fa2_modified.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-16 17:49:52.000000 fa2_modified-0.3.7/fa2_modified.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-16 17:49:52.000000 fa2_modified-0.3.7/fa2_modified.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 17:49:52.781113 fa2_modified-0.3.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-04-16 17:49:41.000000 fa2_modified-0.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:52:56.869402 fa2_modified-0.3.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-04-16 17:52:46.000000 fa2_modified-0.3.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-16 17:52:46.000000 fa2_modified-0.3.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7890 2024-04-16 17:52:56.869402 fa2_modified-0.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-04-16 17:52:46.000000 fa2_modified-0.3.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:52:56.869402 fa2_modified-0.3.8/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)   270891 2024-04-16 17:52:46.000000 fa2_modified-0.3.8/examples/forceatlas2-layout.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    80071 2024-04-16 17:52:46.000000 fa2_modified-0.3.8/examples/geometric_graph.png
+-rw-r--r--   0 runner    (1001) docker     (127)    68224 2024-04-16 17:52:46.000000 fa2_modified-0.3.8/examples/grid_graph.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:52:56.869402 fa2_modified-0.3.8/fa2_modified/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-16 17:52:46.000000 fa2_modified-0.3.8/fa2_modified/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11259 2024-04-16 17:52:46.000000 fa2_modified-0.3.8/fa2_modified/fa2util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11368 2024-04-16 17:52:46.000000 fa2_modified-0.3.8/fa2_modified/forceatlas2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:52:56.869402 fa2_modified-0.3.8/fa2_modified.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7890 2024-04-16 17:52:56.000000 fa2_modified-0.3.8/fa2_modified.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-16 17:52:56.000000 fa2_modified-0.3.8/fa2_modified.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 17:52:56.000000 fa2_modified-0.3.8/fa2_modified.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-16 17:52:56.000000 fa2_modified-0.3.8/fa2_modified.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-16 17:52:56.000000 fa2_modified-0.3.8/fa2_modified.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 17:52:56.869402 fa2_modified-0.3.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-04-16 17:52:46.000000 fa2_modified-0.3.8/setup.py
```

### Comparing `fa2_modified-0.3.7/LICENSE` & `fa2_modified-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `fa2_modified-0.3.7/PKG-INFO` & `fa2_modified-0.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fa2_modified
-Version: 0.3.7
+Version: 0.3.8
 Summary: The fastest ForceAtlas2 algorithm for Python (and NetworkX)
 Home-page: https://github.com/AminAlam/forceatlas2_maintained
 Download-URL: https://github.com/AminAlam/forceatlas2_maintained/archive/refs/tags/V0.0.1.tar.gz
 Author: Bhargav Chippada, Amin Alam
 Keywords: forceatlas2,networkx,force-directed-graph,force-layout,graph
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

### Comparing `fa2_modified-0.3.7/README.md` & `fa2_modified-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `fa2_modified-0.3.7/examples/forceatlas2-layout.ipynb` & `fa2_modified-0.3.8/examples/forceatlas2-layout.ipynb`

 * *Files identical despite different names*

### Comparing `fa2_modified-0.3.7/examples/geometric_graph.png` & `fa2_modified-0.3.8/examples/geometric_graph.png`

 * *Files identical despite different names*

### Comparing `fa2_modified-0.3.7/examples/grid_graph.png` & `fa2_modified-0.3.8/examples/grid_graph.png`

 * *Files identical despite different names*

### Comparing `fa2_modified-0.3.7/fa2_modified/fa2util.py` & `fa2_modified-0.3.8/fa2_modified/fa2util.py`

 * *Files identical despite different names*

### Comparing `fa2_modified-0.3.7/fa2_modified/forceatlas2.py` & `fa2_modified-0.3.8/fa2_modified/forceatlas2.py`

 * *Files identical despite different names*

### Comparing `fa2_modified-0.3.7/fa2_modified.egg-info/PKG-INFO` & `fa2_modified-0.3.8/fa2_modified.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fa2_modified
-Version: 0.3.7
+Version: 0.3.8
 Summary: The fastest ForceAtlas2 algorithm for Python (and NetworkX)
 Home-page: https://github.com/AminAlam/forceatlas2_maintained
 Download-URL: https://github.com/AminAlam/forceatlas2_maintained/archive/refs/tags/V0.0.1.tar.gz
 Author: Bhargav Chippada, Amin Alam
 Keywords: forceatlas2,networkx,force-directed-graph,force-layout,graph
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

### Comparing `fa2_modified-0.3.7/setup.py` & `fa2_modified-0.3.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 # Uncomment the following line if you want to install without optimizations
 # opts = {"py_modules": ["fa2.fa2util"]}
 
 print(">>>> Starting to install!\n")
 
 setup(
     name='fa2_modified',
-    version='0.3.7',
+    version='0.3.8',
     description='The fastest ForceAtlas2 algorithm for Python (and NetworkX)',
     long_description_content_type='text/markdown',
     long_description=long_description,
     author='Bhargav Chippada, Amin Alam',
     url='https://github.com/AminAlam/forceatlas2_maintained',
     download_url='https://github.com/AminAlam/forceatlas2_maintained/archive/refs/tags/V0.0.1.tar.gz',
     keywords=['forceatlas2', 'networkx', 'force-directed-graph', 'force-layout', 'graph'],
@@ -66,10 +66,10 @@
     ],
     install_requires=['numpy', 'scipy', 'tqdm'],
     extras_require={
         'networkx': ['networkx'],
         'igraph': ['python-igraph']
     },
     include_package_data=True,
-    package_data={'fa2': ['fa2util.c']},
+    package_data={'fa2_modified': ['fa2util.c']},
     **opts
 )
```

