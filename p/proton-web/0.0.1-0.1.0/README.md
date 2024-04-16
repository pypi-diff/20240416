# Comparing `tmp/proton_web-0.0.1.tar.gz` & `tmp/proton_web-0.1.0.tar.gz`

## Comparing `proton_web-0.0.1.tar` & `proton_web-0.1.0.tar`

### file list

```diff
@@ -1,20 +1,24 @@
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 proton_web-0.0.1/docs/mkdocs.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 proton_web-0.0.1/docs/requirements.txt
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 proton_web-0.0.1/docs/docs/index.md
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 proton_web-0.0.1/docs/docs/Getting Started/installation.md
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 proton_web-0.0.1/docs/docs/Getting Started/intro.md
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 proton_web-0.0.1/docs/docs/PyHTML/basics.md
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 proton_web-0.0.1/examples/index.html
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 proton_web-0.0.1/examples/test.py
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 proton_web-0.0.1/proton/__init__.py
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 proton_web-0.0.1/proton/__main__.py
--rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 proton_web-0.0.1/proton/document.py
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 proton_web-0.0.1/proton/js.py
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 proton_web-0.0.1/proton/runpython.js
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 proton_web-0.0.1/proton/utils.py
--rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 proton_web-0.0.1/proton/window.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 proton_web-0.0.1/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 proton_web-0.0.1/LICENSE
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 proton_web-0.0.1/README.md
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 proton_web-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 proton_web-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 proton_web-0.1.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 proton_web-0.1.0/docs/mkdocs.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 proton_web-0.1.0/docs/requirements.txt
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 proton_web-0.1.0/docs/docs/Contributing.md
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 proton_web-0.1.0/docs/docs/index.md
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 proton_web-0.1.0/docs/docs/Getting Started/installation.md
+-rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 proton_web-0.1.0/docs/docs/Getting Started/intro.md
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 proton_web-0.1.0/docs/docs/PyHTML/basics.md
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 proton_web-0.1.0/examples/index.html
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 proton_web-0.1.0/examples/test.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 proton_web-0.1.0/examples/example_project/src/main.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 proton_web-0.1.0/examples/example_project/web/index.html
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 proton_web-0.1.0/proton/__init__.py
+-rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 proton_web-0.1.0/proton/__main__.py
+-rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 proton_web-0.1.0/proton/document.py
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 proton_web-0.1.0/proton/js.py
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 proton_web-0.1.0/proton/runpython.js
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 proton_web-0.1.0/proton/utils.py
+-rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 proton_web-0.1.0/proton/window.py
+-rw-r--r--   0        0        0     3286 2020-02-02 00:00:00.000000 proton_web-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 proton_web-0.1.0/LICENSE
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 proton_web-0.1.0/README.md
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 proton_web-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 proton_web-0.1.0/PKG-INFO
```

### Comparing `proton_web-0.0.1/docs/mkdocs.yml` & `proton_web-0.1.0/docs/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `proton_web-0.0.1/docs/docs/Getting Started/installation.md` & `proton_web-0.1.0/docs/docs/Getting Started/installation.md`

 * *Files identical despite different names*

### Comparing `proton_web-0.0.1/examples/index.html` & `proton_web-0.1.0/examples/index.html`

 * *Files identical despite different names*

### Comparing `proton_web-0.0.1/proton/document.py` & `proton_web-0.1.0/proton/document.py`

 * *Files identical despite different names*

### Comparing `proton_web-0.0.1/proton/window.py` & `proton_web-0.1.0/proton/window.py`

 * *Files identical despite different names*

### Comparing `proton_web-0.0.1/.gitignore` & `proton_web-0.1.0/.gitignore`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
 *.so
 
+
 # Distribution / packaging
 .Python
 build/
 develop-eggs/
 dist/
 downloads/
 eggs/
@@ -28,14 +29,19 @@
 
 # PyInstaller
 #  Usually these files are written by a python script from a template
 #  before PyInstaller builds the exe, so as to inject date/other infos into it.
 *.manifest
 *.spec
 
+# Nuitka
+*.build
+*.dist
+*.onefile-build
+
 # Installer logs
 pip-log.txt
 pip-delete-this-directory.txt
 
 # Unit test / coverage reports
 htmlcov/
 .tox/
```

### Comparing `proton_web-0.0.1/LICENSE` & `proton_web-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `proton_web-0.0.1/pyproject.toml` & `proton_web-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Topic :: Internet :: WWW/HTTP",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
-dependencies = ["pywebview", "typer"]
+dependencies = ["pywebview", "typer", "nuitka"]
 keywords = ["webview", "ui", "pywebview", "eel", "html", "css", "js", "javascript"]
 [project.urls]
 Homepage = "https://github.com/Xanderplayz16/proton"
 Issues = "https://github.com/Xanderplayz16/proton/issues"
 
 [tool.hatch.version]
 path = "proton/__init__.py"
```

### Comparing `proton_web-0.0.1/PKG-INFO` & `proton_web-0.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.3
 Name: proton_web
-Version: 0.0.1
+Version: 0.1.0
 Summary: A high-level, easy to use and modern web-application framework.
 Project-URL: Homepage, https://github.com/Xanderplayz16/proton
 Project-URL: Issues, https://github.com/Xanderplayz16/proton/issues
 Author-email: Xanderplayz16 <xandermckay@proton.me>
 License-File: LICENSE
 Keywords: css,eel,html,javascript,js,pywebview,ui,webview
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Internet :: WWW/HTTP
 Requires-Python: >=3.11
+Requires-Dist: nuitka
 Requires-Dist: pywebview
 Requires-Dist: typer
 Description-Content-Type: text/markdown
 
 # Proton
```

