# Comparing `tmp/agdiff-0.0.1.tar.gz` & `tmp/agdiff-0.0.2.tar.gz`

## Comparing `agdiff-0.0.1.tar` & `agdiff-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rwxr-xr-x   0        0        0      154 2020-02-02 00:00:00.000000 agdiff-0.0.1/run_tests.sh
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 agdiff-0.0.1/.github/dependabot.yml
--rw-r--r--   0        0        0     2989 2020-02-02 00:00:00.000000 agdiff-0.0.1/.github/workflows/build.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 agdiff-0.0.1/src/agdiff/__init__.py
--rw-r--r--   0        0        0     7168 2020-02-02 00:00:00.000000 agdiff-0.0.1/src/agdiff/main.py
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 agdiff-0.0.1/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 agdiff-0.0.1/LICENSE
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 agdiff-0.0.1/README.md
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 agdiff-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 agdiff-0.0.1/PKG-INFO
+-rwxr-xr-x   0        0        0      154 2020-02-02 00:00:00.000000 agdiff-0.0.2/run_tests.sh
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 agdiff-0.0.2/.github/dependabot.yml
+-rw-r--r--   0        0        0     2989 2020-02-02 00:00:00.000000 agdiff-0.0.2/.github/workflows/build.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 agdiff-0.0.2/src/agdiff/__init__.py
+-rw-r--r--   0        0        0     7195 2020-02-02 00:00:00.000000 agdiff-0.0.2/src/agdiff/main.py
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 agdiff-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 agdiff-0.0.2/LICENSE
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 agdiff-0.0.2/README.md
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 agdiff-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 agdiff-0.0.2/PKG-INFO
```

### Comparing `agdiff-0.0.1/.github/workflows/build.yml` & `agdiff-0.0.2/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `agdiff-0.0.1/src/agdiff/main.py` & `agdiff-0.0.2/src/agdiff/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -242,9 +242,13 @@
 
 @app.command()
 def main(input_path_str: str):
     input_path = Path(input_path_str)
     _traverse(input_path)
 
 
-if __name__ == "__main__":
+def _main():
     typer.run(main)
+
+
+if __name__ == "__main__":
+    _main()
```

### Comparing `agdiff-0.0.1/LICENSE` & `agdiff-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `agdiff-0.0.1/pyproject.toml` & `agdiff-0.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "agdiff"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
     { name="Scott Belden", email="scottabelden@gmail.com" },
 ]
 description = "A tool for doing diffs over an air gap"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
@@ -29,13 +29,16 @@
     "ruff",
     "pyright",
     "pytest",
     "pytest-cov",
     "build",
 ]
 
+[project.scripts]
+agdiff = "agdiff.main:_main"
+
 [tool.pyright]
 typeCheckingMode = "strict"
 include = ["src"]
 executionEnvironments = [
   { root = "src" }
-]
+]
```

### Comparing `agdiff-0.0.1/PKG-INFO` & `agdiff-0.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: agdiff
-Version: 0.0.1
+Version: 0.0.2
 Summary: A tool for doing diffs over an air gap
 Project-URL: Homepage, https://github.com/scottbelden/agdiff
 Project-URL: Issues, https://github.com/scottbelden/agdiff/issues
 Author-email: Scott Belden <scottabelden@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

