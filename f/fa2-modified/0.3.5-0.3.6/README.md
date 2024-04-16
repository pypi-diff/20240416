# Comparing `tmp/fa2_modified-0.3.5.tar.gz` & `tmp/fa2_modified-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fa2_modified-0.3.5.tar", last modified: Sun Mar 17 15:26:55 2024, max compression
+gzip compressed data, was "fa2_modified-0.3.6.tar", last modified: Tue Apr 16 17:34:02 2024, max compression
```

## Comparing `fa2_modified-0.3.5.tar` & `fa2_modified-0.3.6.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxr-xr-x   0 amin      (1000) amin      (1000)        0 2024-03-17 15:26:55.240471 fa2_modified-0.3.5/
--rw-r--r--   0 amin      (1000) amin      (1000)    35141 2024-03-17 09:13:42.000000 fa2_modified-0.3.5/LICENSE
--rw-r--r--   0 amin      (1000) amin      (1000)       64 2024-03-17 09:13:42.000000 fa2_modified-0.3.5/MANIFEST.in
--rw-r--r--   0 amin      (1000) amin      (1000)     7885 2024-03-17 15:26:55.240471 fa2_modified-0.3.5/PKG-INFO
--rw-r--r--   0 amin      (1000) amin      (1000)     6859 2024-03-17 10:34:44.000000 fa2_modified-0.3.5/README.md
-drwxr-xr-x   0 amin      (1000) amin      (1000)        0 2024-03-17 15:26:55.240471 fa2_modified-0.3.5/examples/
--rw-r--r--   0 amin      (1000) amin      (1000)   270891 2024-03-17 09:13:42.000000 fa2_modified-0.3.5/examples/forceatlas2-layout.ipynb
--rw-r--r--   0 amin      (1000) amin      (1000)    80071 2024-03-17 09:13:42.000000 fa2_modified-0.3.5/examples/geometric_graph.png
--rw-r--r--   0 amin      (1000) amin      (1000)    68224 2024-03-17 09:13:42.000000 fa2_modified-0.3.5/examples/grid_graph.png
-drwxr-xr-x   0 amin      (1000) amin      (1000)        0 2024-03-17 15:26:55.240471 fa2_modified-0.3.5/fa2_modified/
--rw-r--r--   0 amin      (1000) amin      (1000)       27 2024-03-17 09:13:42.000000 fa2_modified-0.3.5/fa2_modified/__init__.py
--rw-r--r--   0 amin      (1000) amin      (1000)   612259 2024-03-17 15:16:26.000000 fa2_modified-0.3.5/fa2_modified/fa2util.c
--rw-r--r--   0 amin      (1000) amin      (1000)    11259 2024-03-17 09:13:42.000000 fa2_modified-0.3.5/fa2_modified/fa2util.py
--rw-r--r--   0 amin      (1000) amin      (1000)    11369 2024-03-17 09:13:42.000000 fa2_modified-0.3.5/fa2_modified/forceatlas2.py
-drwxr-xr-x   0 amin      (1000) amin      (1000)        0 2024-03-17 15:26:55.240471 fa2_modified-0.3.5/fa2_modified.egg-info/
--rw-r--r--   0 amin      (1000) amin      (1000)     7885 2024-03-17 15:26:55.000000 fa2_modified-0.3.5/fa2_modified.egg-info/PKG-INFO
--rw-r--r--   0 amin      (1000) amin      (1000)      404 2024-03-17 15:26:55.000000 fa2_modified-0.3.5/fa2_modified.egg-info/SOURCES.txt
--rw-r--r--   0 amin      (1000) amin      (1000)        1 2024-03-17 15:26:55.000000 fa2_modified-0.3.5/fa2_modified.egg-info/dependency_links.txt
--rw-r--r--   0 amin      (1000) amin      (1000)       62 2024-03-17 15:26:55.000000 fa2_modified-0.3.5/fa2_modified.egg-info/requires.txt
--rw-r--r--   0 amin      (1000) amin      (1000)       13 2024-03-17 15:26:55.000000 fa2_modified-0.3.5/fa2_modified.egg-info/top_level.txt
--rw-r--r--   0 amin      (1000) amin      (1000)       38 2024-03-17 15:26:55.240471 fa2_modified-0.3.5/setup.cfg
--rw-r--r--   0 amin      (1000) amin      (1000)     2797 2024-03-17 15:24:52.000000 fa2_modified-0.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:34:02.644633 fa2_modified-0.3.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-04-16 17:33:50.000000 fa2_modified-0.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-16 17:33:50.000000 fa2_modified-0.3.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7890 2024-04-16 17:34:02.644633 fa2_modified-0.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-04-16 17:33:50.000000 fa2_modified-0.3.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:34:02.640633 fa2_modified-0.3.6/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)   270891 2024-04-16 17:33:50.000000 fa2_modified-0.3.6/examples/forceatlas2-layout.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    80071 2024-04-16 17:33:50.000000 fa2_modified-0.3.6/examples/geometric_graph.png
+-rw-r--r--   0 runner    (1001) docker     (127)    68224 2024-04-16 17:33:50.000000 fa2_modified-0.3.6/examples/grid_graph.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:34:02.644633 fa2_modified-0.3.6/fa2_modified/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-16 17:33:50.000000 fa2_modified-0.3.6/fa2_modified/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11259 2024-04-16 17:33:50.000000 fa2_modified-0.3.6/fa2_modified/fa2util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11368 2024-04-16 17:33:50.000000 fa2_modified-0.3.6/fa2_modified/forceatlas2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:34:02.644633 fa2_modified-0.3.6/fa2_modified.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7890 2024-04-16 17:34:02.000000 fa2_modified-0.3.6/fa2_modified.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-16 17:34:02.000000 fa2_modified-0.3.6/fa2_modified.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 17:34:02.000000 fa2_modified-0.3.6/fa2_modified.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-16 17:34:02.000000 fa2_modified-0.3.6/fa2_modified.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-16 17:34:02.000000 fa2_modified-0.3.6/fa2_modified.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 17:34:02.644633 fa2_modified-0.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-04-16 17:33:50.000000 fa2_modified-0.3.6/setup.py
```

### Comparing `fa2_modified-0.3.5/LICENSE` & `fa2_modified-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fa2_modified-0.3.5/PKG-INFO` & `fa2_modified-0.3.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: fa2_modified
-Version: 0.3.5
+Version: 0.3.6
 Summary: The fastest ForceAtlas2 algorithm for Python (and NetworkX)
 Home-page: https://github.com/AminAlam/forceatlas2_maintained
 Download-URL: https://github.com/AminAlam/forceatlas2_maintained/archive/refs/tags/V0.0.1.tar.gz
 Author: Bhargav Chippada, Amin Alam
 Keywords: forceatlas2,networkx,force-directed-graph,force-layout,graph
-Platform: manylinux2014_x86_64
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
@@ -19,15 +18,16 @@
 Requires-Dist: scipy
 Requires-Dist: tqdm
 Provides-Extra: networkx
 Requires-Dist: networkx; extra == "networkx"
 Provides-Extra: igraph
 Requires-Dist: python-igraph; extra == "igraph"
 
-## ForceAtlas2 for Python3 (maintained version))
+## ForceAtlas2 for Python3 (modified/maintained version)
+
 
 A port of Gephi's Force Atlas 2 layout algorithm to Python 3 (Python 3.9) (with a wrapper for NetworkX and igraph). This is the fastest python implementation available with most of the features complete. It also supports Barnes Hut approximation for maximum speedup.
 
 ForceAtlas2 is a very fast layout algorithm for force-directed graphs. It's used to spatialize a **weighted undirected** graph in 2D (Edge weight defines the strength of the connection). The implementation is based on this [paper](http://journals.plos.org/plosone/article?id=10.1371/journal.pone.0098679) and the corresponding [gephi-java-code](https://github.com/gephi/gephi/blob/master/modules/LayoutPlugin/src/main/java/org/gephi/layout/plugin/forceAtlas2/ForceAtlas2.java). Its really quick compared to the fruchterman reingold algorithm (spring layout) of networkx and scales well to high number of nodes (>10000).
 
 <p align="center" text-align="center">
     <b>Spatialize a random Geometric Graph</b>
@@ -36,15 +36,15 @@
   <img width="460" height="300" src="https://raw.githubusercontent.com/bhargavchippada/forceatlas2/master/examples/geometric_graph.png" alt="Geometric Graph">
 </p>
 
 ## Installation
 
 Install from pip:
 
-    pip install fa2
+    pip install fa2_modified
 
 To build and install run from source:
 
     python setup.py install
 
 **Cython is highly recommended if you are buidling from source as it will speed up by a factor of 10-100x depending on the graph**
 
@@ -62,15 +62,15 @@
 </p>
 <p align="center">
   <img width="460" height="300" src="https://raw.githubusercontent.com/bhargavchippada/forceatlas2/master/examples/grid_graph.png" alt="Grid Graph">
 </p>
 
 ## Usage
 
-from fa2 import ForceAtlas2
+from fa2_modified import ForceAtlas2
 
 Create a ForceAtlas2 object with the appropriate settings. ForceAtlas2 class contains three important methods:
 ```python
 forceatlas2 (G, pos, iterations)
 # G is a graph in 2D numpy ndarray format (or) scipy sparse matrix format. You can set the edge weights (> 0) in the matrix
 # pos is a numpy array (Nx2) of initial positions of nodes
 # iterations is num of iterations to run the algorithm
@@ -91,15 +91,15 @@
 # weight_attr denotes the weight attribute's name in G.es, None by default
 # returns an igraph layout
 ```
 Below is an example usage. You can also see the feature settings of ForceAtlas2 class.
 
 ```python
 import networkx as nx
-from fa2 import ForceAtlas2
+from fa2_modified import ForceAtlas2
 import matplotlib.pyplot as plt
 
 G = nx.random_geometric_graph(400, 0.2)
 
 forceatlas2 = ForceAtlas2(
                         # Behavior alternatives
                         outboundAttractionDistribution=True,  # Dissuade hubs
```

### Comparing `fa2_modified-0.3.5/README.md` & `fa2_modified-0.3.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-## ForceAtlas2 for Python3 (maintained version))
+## ForceAtlas2 for Python3 (modified/maintained version)
+
 
 A port of Gephi's Force Atlas 2 layout algorithm to Python 3 (Python 3.9) (with a wrapper for NetworkX and igraph). This is the fastest python implementation available with most of the features complete. It also supports Barnes Hut approximation for maximum speedup.
 
 ForceAtlas2 is a very fast layout algorithm for force-directed graphs. It's used to spatialize a **weighted undirected** graph in 2D (Edge weight defines the strength of the connection). The implementation is based on this [paper](http://journals.plos.org/plosone/article?id=10.1371/journal.pone.0098679) and the corresponding [gephi-java-code](https://github.com/gephi/gephi/blob/master/modules/LayoutPlugin/src/main/java/org/gephi/layout/plugin/forceAtlas2/ForceAtlas2.java). Its really quick compared to the fruchterman reingold algorithm (spring layout) of networkx and scales well to high number of nodes (>10000).
 
 <p align="center" text-align="center">
     <b>Spatialize a random Geometric Graph</b>
@@ -11,15 +12,15 @@
   <img width="460" height="300" src="https://raw.githubusercontent.com/bhargavchippada/forceatlas2/master/examples/geometric_graph.png" alt="Geometric Graph">
 </p>
 
 ## Installation
 
 Install from pip:
 
-    pip install fa2
+    pip install fa2_modified
 
 To build and install run from source:
 
     python setup.py install
 
 **Cython is highly recommended if you are buidling from source as it will speed up by a factor of 10-100x depending on the graph**
 
@@ -37,15 +38,15 @@
 </p>
 <p align="center">
   <img width="460" height="300" src="https://raw.githubusercontent.com/bhargavchippada/forceatlas2/master/examples/grid_graph.png" alt="Grid Graph">
 </p>
 
 ## Usage
 
-from fa2 import ForceAtlas2
+from fa2_modified import ForceAtlas2
 
 Create a ForceAtlas2 object with the appropriate settings. ForceAtlas2 class contains three important methods:
 ```python
 forceatlas2 (G, pos, iterations)
 # G is a graph in 2D numpy ndarray format (or) scipy sparse matrix format. You can set the edge weights (> 0) in the matrix
 # pos is a numpy array (Nx2) of initial positions of nodes
 # iterations is num of iterations to run the algorithm
@@ -66,15 +67,15 @@
 # weight_attr denotes the weight attribute's name in G.es, None by default
 # returns an igraph layout
 ```
 Below is an example usage. You can also see the feature settings of ForceAtlas2 class.
 
 ```python
 import networkx as nx
-from fa2 import ForceAtlas2
+from fa2_modified import ForceAtlas2
 import matplotlib.pyplot as plt
 
 G = nx.random_geometric_graph(400, 0.2)
 
 forceatlas2 = ForceAtlas2(
                         # Behavior alternatives
                         outboundAttractionDistribution=True,  # Dissuade hubs
```

### Comparing `fa2_modified-0.3.5/examples/forceatlas2-layout.ipynb` & `fa2_modified-0.3.6/examples/forceatlas2-layout.ipynb`

 * *Files identical despite different names*

### Comparing `fa2_modified-0.3.5/examples/geometric_graph.png` & `fa2_modified-0.3.6/examples/geometric_graph.png`

 * *Files identical despite different names*

### Comparing `fa2_modified-0.3.5/examples/grid_graph.png` & `fa2_modified-0.3.6/examples/grid_graph.png`

 * *Files identical despite different names*

### Comparing `fa2_modified-0.3.5/fa2_modified/fa2util.py` & `fa2_modified-0.3.6/fa2_modified/fa2util.py`

 * *Files identical despite different names*

### Comparing `fa2_modified-0.3.5/fa2_modified/forceatlas2.py` & `fa2_modified-0.3.6/fa2_modified/forceatlas2.py`

 * *Files 0% similar despite different names*

```diff
@@ -241,15 +241,15 @@
             cynetworkx = None
 
         assert (
             isinstance(G, networkx.classes.graph.Graph)
             or (cynetworkx and isinstance(G, cynetworkx.classes.graph.Graph))
         ), "Not a networkx graph"
         assert isinstance(pos, dict) or (pos is None), "pos must be specified as a dictionary, as in networkx"
-        M = networkx.to_scipy_sparse_matrix(G, dtype='f', format='lil', weight=weight_attr)
+        M = networkx.to_scipy_sparse_array(G, dtype='f', format='lil', weight=weight_attr)
         if pos is None:
             l = self.forceatlas2(M, pos=None, iterations=iterations)
         else:
             poslist = numpy.asarray([pos[i] for i in G.nodes()])
             l = self.forceatlas2(M, pos=poslist, iterations=iterations)
         return dict(zip(G.nodes(), l))
```

### Comparing `fa2_modified-0.3.5/fa2_modified.egg-info/PKG-INFO` & `fa2_modified-0.3.6/fa2_modified.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: fa2_modified
-Version: 0.3.5
+Version: 0.3.6
 Summary: The fastest ForceAtlas2 algorithm for Python (and NetworkX)
 Home-page: https://github.com/AminAlam/forceatlas2_maintained
 Download-URL: https://github.com/AminAlam/forceatlas2_maintained/archive/refs/tags/V0.0.1.tar.gz
 Author: Bhargav Chippada, Amin Alam
 Keywords: forceatlas2,networkx,force-directed-graph,force-layout,graph
-Platform: manylinux2014_x86_64
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
@@ -19,15 +18,16 @@
 Requires-Dist: scipy
 Requires-Dist: tqdm
 Provides-Extra: networkx
 Requires-Dist: networkx; extra == "networkx"
 Provides-Extra: igraph
 Requires-Dist: python-igraph; extra == "igraph"
 
-## ForceAtlas2 for Python3 (maintained version))
+## ForceAtlas2 for Python3 (modified/maintained version)
+
 
 A port of Gephi's Force Atlas 2 layout algorithm to Python 3 (Python 3.9) (with a wrapper for NetworkX and igraph). This is the fastest python implementation available with most of the features complete. It also supports Barnes Hut approximation for maximum speedup.
 
 ForceAtlas2 is a very fast layout algorithm for force-directed graphs. It's used to spatialize a **weighted undirected** graph in 2D (Edge weight defines the strength of the connection). The implementation is based on this [paper](http://journals.plos.org/plosone/article?id=10.1371/journal.pone.0098679) and the corresponding [gephi-java-code](https://github.com/gephi/gephi/blob/master/modules/LayoutPlugin/src/main/java/org/gephi/layout/plugin/forceAtlas2/ForceAtlas2.java). Its really quick compared to the fruchterman reingold algorithm (spring layout) of networkx and scales well to high number of nodes (>10000).
 
 <p align="center" text-align="center">
     <b>Spatialize a random Geometric Graph</b>
@@ -36,15 +36,15 @@
   <img width="460" height="300" src="https://raw.githubusercontent.com/bhargavchippada/forceatlas2/master/examples/geometric_graph.png" alt="Geometric Graph">
 </p>
 
 ## Installation
 
 Install from pip:
 
-    pip install fa2
+    pip install fa2_modified
 
 To build and install run from source:
 
     python setup.py install
 
 **Cython is highly recommended if you are buidling from source as it will speed up by a factor of 10-100x depending on the graph**
 
@@ -62,15 +62,15 @@
 </p>
 <p align="center">
   <img width="460" height="300" src="https://raw.githubusercontent.com/bhargavchippada/forceatlas2/master/examples/grid_graph.png" alt="Grid Graph">
 </p>
 
 ## Usage
 
-from fa2 import ForceAtlas2
+from fa2_modified import ForceAtlas2
 
 Create a ForceAtlas2 object with the appropriate settings. ForceAtlas2 class contains three important methods:
 ```python
 forceatlas2 (G, pos, iterations)
 # G is a graph in 2D numpy ndarray format (or) scipy sparse matrix format. You can set the edge weights (> 0) in the matrix
 # pos is a numpy array (Nx2) of initial positions of nodes
 # iterations is num of iterations to run the algorithm
@@ -91,15 +91,15 @@
 # weight_attr denotes the weight attribute's name in G.es, None by default
 # returns an igraph layout
 ```
 Below is an example usage. You can also see the feature settings of ForceAtlas2 class.
 
 ```python
 import networkx as nx
-from fa2 import ForceAtlas2
+from fa2_modified import ForceAtlas2
 import matplotlib.pyplot as plt
 
 G = nx.random_geometric_graph(400, 0.2)
 
 forceatlas2 = ForceAtlas2(
                         # Behavior alternatives
                         outboundAttractionDistribution=True,  # Dissuade hubs
```

### Comparing `fa2_modified-0.3.5/setup.py` & `fa2_modified-0.3.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 # Uncomment the following line if you want to install without optimizations
 # opts = {"py_modules": ["fa2.fa2util"]}
 
 print(">>>> Starting to install!\n")
 
 setup(
     name='fa2_modified',
-    version='0.3.5',
+    version='0.3.6',
     description='The fastest ForceAtlas2 algorithm for Python (and NetworkX)',
     long_description_content_type='text/markdown',
     long_description=long_description,
     author='Bhargav Chippada, Amin Alam',
     url='https://github.com/AminAlam/forceatlas2_maintained',
     download_url='https://github.com/AminAlam/forceatlas2_maintained/archive/refs/tags/V0.0.1.tar.gz',
     keywords=['forceatlas2', 'networkx', 'force-directed-graph', 'force-layout', 'graph'],
@@ -65,11 +65,10 @@
         'Programming Language :: Python :: 3'
     ],
     install_requires=['numpy', 'scipy', 'tqdm'],
     extras_require={
         'networkx': ['networkx'],
         'igraph': ['python-igraph']
     },
-    platforms=["manylinux2014_x86_64"],
     include_package_data=True,
     **opts
 )
```

