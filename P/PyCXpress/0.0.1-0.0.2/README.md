# Comparing `tmp/pycxpress-0.0.1.tar.gz` & `tmp/pycxpress-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycxpress-0.0.1.tar", max compression
+gzip compressed data, was "pycxpress-0.0.2.tar", max compression
```

## Comparing `pycxpress-0.0.1.tar` & `pycxpress-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,12 @@
--rw-r--r--   0        0        0     1066 2024-04-13 13:58:04.979715 pycxpress-0.0.1/LICENSE
--rw-r--r--   0        0        0     2324 2024-04-13 13:58:04.979715 pycxpress-0.0.1/README.md
--rw-r--r--   0        0        0     3849 2024-04-13 13:58:04.979715 pycxpress-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      648 2024-04-13 13:58:04.979715 pycxpress-0.0.1/src/PyCXpress/__init__.py
--rw-r--r--   0        0        0     1686 2024-04-13 13:58:04.979715 pycxpress-0.0.1/src/PyCXpress/__main__.py
--rw-r--r--   0        0        0     3543 1970-01-01 00:00:00.000000 pycxpress-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-16 17:07:22.680355 pycxpress-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2324 2024-04-16 17:07:22.680355 pycxpress-0.0.2/README.md
+-rw-r--r--   0        0        0      872 2024-04-16 17:07:22.680355 pycxpress-0.0.2/example/Makefile
+-rw-r--r--   0        0        0     1503 2024-04-16 17:07:22.680355 pycxpress-0.0.2/example/main.cpp
+-rw-r--r--   0        0        0     2215 2024-04-16 17:07:22.680355 pycxpress-0.0.2/example/model.py
+-rw-r--r--   0        0        0     3949 2024-04-16 17:07:22.680355 pycxpress-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1070 2024-04-16 17:07:22.680355 pycxpress-0.0.2/src/PyCXpress/__init__.py
+-rw-r--r--   0        0        0      979 2024-04-16 17:07:22.680355 pycxpress-0.0.2/src/PyCXpress/__main__.py
+-rw-r--r--   0        0        0     5369 2024-04-16 17:07:22.680355 pycxpress-0.0.2/src/PyCXpress/core.py
+-rw-r--r--   0        0        0     6998 2024-04-16 17:07:22.684355 pycxpress-0.0.2/src/cpp/PyCXpress.hpp
+-rw-r--r--   0        0        0      849 2024-04-16 17:07:22.684355 pycxpress-0.0.2/src/cpp/Utils.hpp
+-rw-r--r--   0        0        0     3536 1970-01-01 00:00:00.000000 pycxpress-0.0.2/PKG-INFO
```

### Comparing `pycxpress-0.0.1/LICENSE` & `pycxpress-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pycxpress-0.0.1/README.md` & `pycxpress-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pycxpress-0.0.1/pyproject.toml` & `pycxpress-0.0.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "PyCXpress"
-version = "0.0.1"
+version = "0.0.2"
 description = "PyCXpress is a high-performance hybrid framework that seamlessly integrates Python and C++ to harness the flexibility of Python and the speed of C++ for efficient and expressive computation, particularly in the realm of deep learning and numerical computing."
 readme = "README.md"
 authors = ["chaoqing <chaoqingwang.nick@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/chaoqing/PyCXpress"
 homepage = "https://github.com/chaoqing/PyCXpress"
 packages = [
     { include = "PyCXpress", from = "src" },
 ]
+include = [
+    { path = "src/cpp/", format = ["sdist", "wheel"] },
+    { path = "example/", format = ["sdist", "wheel"] },
+]
+
 
 # Keywords description https://python-poetry.org/docs/pyproject/#keywords
 keywords = []  #! Update me
 
 # Pypi classifiers: https://pypi.org/classifiers/
 classifiers = [  #! Update me
   "Development Status :: 3 - Alpha",
@@ -29,21 +34,21 @@
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
 ]
 
 [tool.poetry.scripts]
 # Entry points for the package https://python-poetry.org/docs/pyproject/#scripts
-"PyCXpress" = "PyCXpress.__main__:app"
+"PyCXpress" = "PyCXpress.__main__:main"
 
 [tool.poetry.dependencies]
 python = "^3.8"
+pybind11 = "^2.12.0"
+numpy = "^1.22"
 
-typer = {extras = ["all"], version = "^0.12.3"}
-rich = "^13.7.1"
 
 [tool.poetry.dev-dependencies]
 bandit = "^1.7.1"
 black = {version = "^24.4", allow-prereleases = true}
 darglint = "^1.8.1"
 isort = {extras = ["colors"], version = "^5.10.1"}
 mypy = "^1.0"
```

### Comparing `pycxpress-0.0.1/PKG-INFO` & `pycxpress-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyCXpress
-Version: 0.0.1
+Version: 0.0.2
 Summary: PyCXpress is a high-performance hybrid framework that seamlessly integrates Python and C++ to harness the flexibility of Python and the speed of C++ for efficient and expressive computation, particularly in the realm of deep learning and numerical computing.
 Home-page: https://github.com/chaoqing/PyCXpress
 License: MIT
 Author: chaoqing
 Author-email: chaoqingwang.nick@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -14,16 +14,16 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: rich (>=13.7.1,<14.0.0)
-Requires-Dist: typer[all] (>=0.12.3,<0.13.0)
+Requires-Dist: numpy (>=1.22,<2.0)
+Requires-Dist: pybind11 (>=2.12.0,<3.0.0)
 Project-URL: Repository, https://github.com/chaoqing/PyCXpress
 Description-Content-Type: text/markdown
 
 # PyCXpress
 
 <div align="center">
```

