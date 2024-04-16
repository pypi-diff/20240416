# Comparing `tmp/quadratic_function_solver_kemulk-0.0.1.tar.gz` & `tmp/quadratic_function_solver_kemulk-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quadratic_function_solver_kemulk-0.0.1.tar", last modified: Tue Apr 16 16:31:45 2024, max compression
+gzip compressed data, was "quadratic_function_solver_kemulk-0.0.2.tar", last modified: Tue Apr 16 17:59:24 2024, max compression
```

## Comparing `quadratic_function_solver_kemulk-0.0.1.tar` & `quadratic_function_solver_kemulk-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 16:31:45.801157 quadratic_function_solver_kemulk-0.0.1/
--rw-rw-rw-   0        0        0     1050 2024-04-16 16:28:04.000000 quadratic_function_solver_kemulk-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      764 2024-04-16 16:31:45.799155 quadratic_function_solver_kemulk-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      215 2024-04-16 16:26:46.000000 quadratic_function_solver_kemulk-0.0.1/README.md
--rw-rw-rw-   0        0        0      531 2024-04-16 16:24:27.000000 quadratic_function_solver_kemulk-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-16 16:31:45.801157 quadratic_function_solver_kemulk-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-16 16:31:45.787144 quadratic_function_solver_kemulk-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-04-16 16:31:45.792148 quadratic_function_solver_kemulk-0.0.1/src/quadratic_function_solver_kemulk/
--rw-rw-rw-   0        0        0        0 2024-04-16 15:21:25.000000 quadratic_function_solver_kemulk-0.0.1/src/quadratic_function_solver_kemulk/__init__.py
--rw-rw-rw-   0        0        0       49 2024-04-16 16:14:06.000000 quadratic_function_solver_kemulk-0.0.1/src/quadratic_function_solver_kemulk/quadratic_function_solver.py
-drwxrwxrwx   0        0        0        0 2024-04-16 16:31:45.798154 quadratic_function_solver_kemulk-0.0.1/src/quadratic_function_solver_kemulk.egg-info/
--rw-rw-rw-   0        0        0      764 2024-04-16 16:31:45.000000 quadratic_function_solver_kemulk-0.0.1/src/quadratic_function_solver_kemulk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      387 2024-04-16 16:31:45.000000 quadratic_function_solver_kemulk-0.0.1/src/quadratic_function_solver_kemulk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 16:31:45.000000 quadratic_function_solver_kemulk-0.0.1/src/quadratic_function_solver_kemulk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2024-04-16 16:31:45.000000 quadratic_function_solver_kemulk-0.0.1/src/quadratic_function_solver_kemulk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-16 17:59:24.127431 quadratic_function_solver_kemulk-0.0.2/
+-rw-rw-rw-   0        0        0     1050 2024-04-16 16:28:04.000000 quadratic_function_solver_kemulk-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      764 2024-04-16 17:59:24.126429 quadratic_function_solver_kemulk-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      215 2024-04-16 16:26:46.000000 quadratic_function_solver_kemulk-0.0.2/README.md
+-rw-rw-rw-   0        0        0      531 2024-04-16 17:58:56.000000 quadratic_function_solver_kemulk-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-16 17:59:24.128431 quadratic_function_solver_kemulk-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-16 17:59:24.114133 quadratic_function_solver_kemulk-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2024-04-16 17:59:24.116135 quadratic_function_solver_kemulk-0.0.2/src/quadratic_function_solver_kemulk/
+-rw-rw-rw-   0        0        0        0 2024-04-16 15:21:25.000000 quadratic_function_solver_kemulk-0.0.2/src/quadratic_function_solver_kemulk/__init__.py
+-rw-rw-rw-   0        0        0      628 2024-04-16 17:57:48.000000 quadratic_function_solver_kemulk-0.0.2/src/quadratic_function_solver_kemulk/quadratic_function_solver.py
+drwxrwxrwx   0        0        0        0 2024-04-16 17:59:24.125429 quadratic_function_solver_kemulk-0.0.2/src/quadratic_function_solver_kemulk.egg-info/
+-rw-rw-rw-   0        0        0      764 2024-04-16 17:59:24.000000 quadratic_function_solver_kemulk-0.0.2/src/quadratic_function_solver_kemulk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      387 2024-04-16 17:59:24.000000 quadratic_function_solver_kemulk-0.0.2/src/quadratic_function_solver_kemulk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 17:59:24.000000 quadratic_function_solver_kemulk-0.0.2/src/quadratic_function_solver_kemulk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2024-04-16 17:59:24.000000 quadratic_function_solver_kemulk-0.0.2/src/quadratic_function_solver_kemulk.egg-info/top_level.txt
```

### Comparing `quadratic_function_solver_kemulk-0.0.1/LICENSE` & `quadratic_function_solver_kemulk-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `quadratic_function_solver_kemulk-0.0.1/PKG-INFO` & `quadratic_function_solver_kemulk-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quadratic_function_solver_kemulk
-Version: 0.0.1
+Version: 0.0.2
 Summary: Package for solving quadratic function
 Author-email: Example Author <author@example.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `quadratic_function_solver_kemulk-0.0.1/src/quadratic_function_solver_kemulk.egg-info/PKG-INFO` & `quadratic_function_solver_kemulk-0.0.2/src/quadratic_function_solver_kemulk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quadratic_function_solver_kemulk
-Version: 0.0.1
+Version: 0.0.2
 Summary: Package for solving quadratic function
 Author-email: Example Author <author@example.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

