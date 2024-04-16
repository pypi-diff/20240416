# Comparing `tmp/ocx_databinding-2.6.3.tar.gz` & `tmp/ocx_databinding-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocx_databinding-2.6.3.tar", max compression
+gzip compressed data, was "ocx_databinding-2.7.0.tar", max compression
```

## Comparing `ocx_databinding-2.6.3.tar` & `ocx_databinding-2.7.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1066 2024-03-11 07:54:21.887187 ocx_databinding-2.6.3/LICENSE
--rw-r--r--   0        0        0     3387 2024-03-11 07:54:21.887187 ocx_databinding-2.6.3/README.md
--rw-r--r--   0        0        0      180 2024-03-11 07:54:21.887187 ocx_databinding-2.6.3/ocx_databinding/__init__.py
--rw-r--r--   0        0        0     2292 2024-03-11 07:54:21.887187 ocx_databinding-2.6.3/ocx_databinding/cli.py
--rw-r--r--   0        0        0     5588 2024-03-11 07:54:21.887187 ocx_databinding-2.6.3/ocx_databinding/generator.py
--rw-r--r--   0        0        0     2176 2024-03-11 07:54:21.887187 ocx_databinding-2.6.3/pyproject.toml
--rw-r--r--   0        0        0     4078 1970-01-01 00:00:00.000000 ocx_databinding-2.6.3/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-16 13:21:40.182127 ocx_databinding-2.7.0/LICENSE
+-rw-r--r--   0        0        0     3389 2024-04-16 13:21:40.182127 ocx_databinding-2.7.0/README.md
+-rw-r--r--   0        0        0      180 2024-04-16 13:21:40.182127 ocx_databinding-2.7.0/ocx_databinding/__init__.py
+-rw-r--r--   0        0        0     2292 2024-04-16 13:21:40.182127 ocx_databinding-2.7.0/ocx_databinding/cli.py
+-rw-r--r--   0        0        0     5589 2024-04-16 13:21:40.182127 ocx_databinding-2.7.0/ocx_databinding/generator.py
+-rw-r--r--   0        0        0     2175 2024-04-16 13:21:40.182127 ocx_databinding-2.7.0/pyproject.toml
+-rw-r--r--   0        0        0     4129 1970-01-01 00:00:00.000000 ocx_databinding-2.7.0/PKG-INFO
```

### Comparing `ocx_databinding-2.6.3/LICENSE` & `ocx_databinding-2.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ocx_databinding-2.6.3/README.md` & `ocx_databinding-2.7.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -76,8 +76,8 @@
          1531 __init__.py
 
 The CLI generates a single  package, meaning that any imported schemas are ignored, see [xsdata](https://xsdata.readthedocs.io/en/latest/) if more detailed control of the databinding is necessary.
 The databindings are also versioned by creating a package name with the version string. This allows us to have multiple databindings representing different schema versions.
 
 ## API documentation
 
-[API](https://ocxstandard.github.io/ocx-generator/)
+[API](https://ocxstandard.github.io/ocx-databinding/)
```

### Comparing `ocx_databinding-2.6.3/ocx_databinding/cli.py` & `ocx_databinding-2.7.0/ocx_databinding/cli.py`

 * *Files identical despite different names*

### Comparing `ocx_databinding-2.6.3/ocx_databinding/generator.py` & `ocx_databinding-2.7.0/ocx_databinding/generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
     source: Union[str, Path],
     package_name: str,
     version: str,
     structure_style: str = "single-package",
     docstring_style: str = "Google",
     stdout: bool = False,
     recursive: bool = True,
-    slots: bool = True,
+    slots: bool = False,
 ) -> bool:
     """
     Call xsdata subprocess to generate Python data bindings.
 
     Args:
         source: The source URL or local file path of the XML schema.
         package_name: The name of the package to generate.
```

### Comparing `ocx_databinding-2.6.3/pyproject.toml` & `ocx_databinding-2.7.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "ocx_databinding"
-version = "2.6.3"
+version = "2.7.0"
 description = "Python CLI for managing OCX schema databinding and versioning according to PEP 440."
 authors = ["ocastrup <ole.christian.astrup@dnv.com>"]
 readme = "README.md"
 packages = [{include = "ocx_databinding"}]
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.9"
 packaging = "^23.1"
 tbump = '*'
 xsdata = "23.8"
 lxml = "*"
 soap = "*"
 typer = "*"
 loguru = "*"
@@ -45,15 +45,15 @@
 databinding = "ocx_databinding.cli:main"
 
 [tool.tbump]
 # Uncomment this if your project is hosted on GitHub:
 github_url = "https://github.com/OCXStandard/ocx-databinding"
 
 [tool.tbump.version]
-current = "2.6.3"
+current = "2.7.0"
 
 # Example of a semver regexp.
 # Make sure this matches current_version before
 # using tbump
 regex = '''
   (?P<major>\d+)
   \.
```

### Comparing `ocx_databinding-2.6.3/PKG-INFO` & `ocx_databinding-2.7.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: ocx_databinding
-Version: 2.6.3
+Version: 2.7.0
 Summary: Python CLI for managing OCX schema databinding and versioning according to PEP 440.
 Author: ocastrup
 Author-email: ole.christian.astrup@dnv.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: loguru
 Requires-Dist: lxml
 Requires-Dist: packaging (>=23.1,<24.0)
 Requires-Dist: soap
@@ -97,9 +98,9 @@
          1531 __init__.py
 
 The CLI generates a single  package, meaning that any imported schemas are ignored, see [xsdata](https://xsdata.readthedocs.io/en/latest/) if more detailed control of the databinding is necessary.
 The databindings are also versioned by creating a package name with the version string. This allows us to have multiple databindings representing different schema versions.
 
 ## API documentation
 
-[API](https://ocxstandard.github.io/ocx-generator/)
+[API](https://ocxstandard.github.io/ocx-databinding/)
```

