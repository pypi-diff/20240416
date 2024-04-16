# Comparing `tmp/bigrandomgraphs-0.0.3.tar.gz` & `tmp/bigrandomgraphs-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigrandomgraphs-0.0.3.tar", last modified: Wed Feb 28 13:46:11 2024, max compression
+gzip compressed data, was "bigrandomgraphs-0.0.4.tar", last modified: Tue Apr 16 13:46:56 2024, max compression
```

## Comparing `bigrandomgraphs-0.0.3.tar` & `bigrandomgraphs-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 phys3smithj  (1001) phys3smithj  (1001)        0 2024-02-28 13:46:11.553427 bigrandomgraphs-0.0.3/
--rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)      163 2023-08-06 22:08:22.000000 bigrandomgraphs-0.0.3/CMakeLists.txt
--rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)      244 2024-02-28 13:46:11.549427 bigrandomgraphs-0.0.3/PKG-INFO
--rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)       74 2023-08-06 21:01:36.000000 bigrandomgraphs-0.0.3/README.md
-drwxrwxr-x   0 phys3smithj  (1001) phys3smithj  (1001)        0 2024-02-28 13:46:11.549427 bigrandomgraphs-0.0.3/bigrandomgraphs.egg-info/
--rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)      244 2024-02-28 13:46:11.000000 bigrandomgraphs-0.0.3/bigrandomgraphs.egg-info/PKG-INFO
--rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)      317 2024-02-28 13:46:11.000000 bigrandomgraphs-0.0.3/bigrandomgraphs.egg-info/SOURCES.txt
--rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)        1 2024-02-28 13:46:11.000000 bigrandomgraphs-0.0.3/bigrandomgraphs.egg-info/dependency_links.txt
--rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)        1 2023-08-07 21:37:24.000000 bigrandomgraphs-0.0.3/bigrandomgraphs.egg-info/not-zip-safe
--rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)       16 2024-02-28 13:46:11.000000 bigrandomgraphs-0.0.3/bigrandomgraphs.egg-info/top_level.txt
--rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)       38 2024-02-28 13:46:11.553427 bigrandomgraphs-0.0.3/setup.cfg
--rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)     3377 2024-02-28 13:45:37.000000 bigrandomgraphs-0.0.3/setup.py
-drwxrwxr-x   0 phys3smithj  (1001) phys3smithj  (1001)        0 2024-02-28 13:46:11.549427 bigrandomgraphs-0.0.3/src/
--rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)       20 2023-08-06 21:18:03.000000 bigrandomgraphs-0.0.3/src/__init__.py
--rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)    15860 2024-02-28 13:38:42.000000 bigrandomgraphs-0.0.3/src/generate_model.cpp
--rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)     9065 2024-02-28 13:30:47.000000 bigrandomgraphs-0.0.3/src/wrapper_bindings.cpp
--rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)     8115 2023-08-04 09:15:08.000000 bigrandomgraphs-0.0.3/test.py
+drwxrwxr-x   0 phys3smithj  (1001) phys3smithj  (1001)        0 2024-04-16 13:46:56.548130 bigrandomgraphs-0.0.4/
+-rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)      163 2023-08-06 22:08:22.000000 bigrandomgraphs-0.0.4/CMakeLists.txt
+-rw-r--r--   0 phys3smithj  (1001) phys3smithj  (1001)      147 2024-04-16 13:46:56.548130 bigrandomgraphs-0.0.4/PKG-INFO
+-rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)       74 2023-08-06 21:01:36.000000 bigrandomgraphs-0.0.4/README.md
+drwxrwxr-x   0 phys3smithj  (1001) phys3smithj  (1001)        0 2024-04-16 13:46:56.548130 bigrandomgraphs-0.0.4/bigrandomgraphs.egg-info/
+-rw-r--r--   0 phys3smithj  (1001) phys3smithj  (1001)      147 2024-04-16 13:46:56.000000 bigrandomgraphs-0.0.4/bigrandomgraphs.egg-info/PKG-INFO
+-rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)      317 2024-04-16 13:46:56.000000 bigrandomgraphs-0.0.4/bigrandomgraphs.egg-info/SOURCES.txt
+-rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)        1 2024-04-16 13:46:56.000000 bigrandomgraphs-0.0.4/bigrandomgraphs.egg-info/dependency_links.txt
+-rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)        1 2023-08-07 21:37:24.000000 bigrandomgraphs-0.0.4/bigrandomgraphs.egg-info/not-zip-safe
+-rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)       16 2024-04-16 13:46:56.000000 bigrandomgraphs-0.0.4/bigrandomgraphs.egg-info/top_level.txt
+-rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)       38 2024-04-16 13:46:56.548130 bigrandomgraphs-0.0.4/setup.cfg
+-rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)     3377 2024-04-16 13:38:43.000000 bigrandomgraphs-0.0.4/setup.py
+drwxrwxr-x   0 phys3smithj  (1001) phys3smithj  (1001)        0 2024-04-16 13:46:56.548130 bigrandomgraphs-0.0.4/src/
+-rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)       20 2023-08-06 21:18:03.000000 bigrandomgraphs-0.0.4/src/__init__.py
+-rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)    15860 2024-02-28 13:38:42.000000 bigrandomgraphs-0.0.4/src/generate_model.cpp
+-rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)     8980 2024-04-16 13:44:59.000000 bigrandomgraphs-0.0.4/src/wrapper_bindings.cpp
+-rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)     8115 2023-08-04 09:15:08.000000 bigrandomgraphs-0.0.4/test.py
```

### Comparing `bigrandomgraphs-0.0.3/setup.py` & `bigrandomgraphs-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         if not os.path.exists(self.build_temp):
             os.makedirs(self.build_temp)
         subprocess.check_call(['cmake', ext.sourcedir] + cmake_args, cwd=self.build_temp, env=env)
         subprocess.check_call(['cmake', '--build', '.'] + build_args, cwd=self.build_temp)
 
 setup(
     name='bigrandomgraphs',
-    version='0.0.3',
+    version='0.0.4',
     author='Jason P. Smith',
     description='Python package for fast creation of large random graphs',
     ext_modules=[CMakeExtension('bigrandomgraphs')],
     cmdclass=dict(build_ext=CMakeBuild),
     packages=['bigrandomgraphs'],
     package_dir={'bigrandomgraphs': './src/'},
     zip_safe=False,
```

### Comparing `bigrandomgraphs-0.0.3/src/generate_model.cpp` & `bigrandomgraphs-0.0.4/src/generate_model.cpp`

 * *Files identical despite different names*

### Comparing `bigrandomgraphs-0.0.3/src/wrapper_bindings.cpp` & `bigrandomgraphs-0.0.4/src/wrapper_bindings.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
   m.def("ER", [](int n, double p, int threads, uint64_t seed1, uint64_t seed2){
       //intialise vectors
       std::vector<std::thread> t(threads - 1);
       std::vector<std::vector<vertex_t>> row(threads);
       std::vector<std::vector<vertex_t>> col(threads);
 
       std::vector<std::pair<uint64_t,uint64_t>> new_seeds = hash_seeds(seed1,seed2,threads);
-      for(auto i : new_seeds){ std::cout << i.first << " " << i.second << std::endl;}
+
       //Start each thread
       for (size_t index = 0; index < threads - 1; ++index){
           t[index] = std::thread(&add_edges_ER, index, n, threads, p, std::ref(row[index]),
                                    std::ref(col[index]), new_seeds[index].first, new_seeds[index].second);
       }
       add_edges_ER(threads-1, n, threads, p, std::ref(row[threads-1]),std::ref(col[threads-1]),
                                new_seeds[threads-1].first, new_seeds[threads-1].second);
```

### Comparing `bigrandomgraphs-0.0.3/test.py` & `bigrandomgraphs-0.0.4/test.py`

 * *Files identical despite different names*

