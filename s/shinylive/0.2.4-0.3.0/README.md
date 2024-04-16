# Comparing `tmp/shinylive-0.2.4.tar.gz` & `tmp/shinylive-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shinylive-0.2.4.tar", last modified: Fri Mar  8 18:08:41 2024, max compression
+gzip compressed data, was "shinylive-0.3.0.tar", last modified: Tue Apr 16 17:10:10 2024, max compression
```

## Comparing `shinylive-0.2.4.tar` & `shinylive-0.3.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 18:08:41.320878 shinylive-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-03-08 18:08:27.000000 shinylive-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-03-08 18:08:41.320878 shinylive-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3402 2024-03-08 18:08:27.000000 shinylive-0.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-03-08 18:08:41.320878 shinylive-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-08 18:08:27.000000 shinylive-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 18:08:41.320878 shinylive-0.2.4/shinylive/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-08 18:08:27.000000 shinylive-0.2.4/shinylive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4390 2024-03-08 18:08:27.000000 shinylive-0.2.4/shinylive/_app_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     7957 2024-03-08 18:08:27.000000 shinylive-0.2.4/shinylive/_assets.py
--rw-r--r--   0 runner    (1001) docker     (127)    19120 2024-03-08 18:08:27.000000 shinylive-0.2.4/shinylive/_deps.py
--rw-r--r--   0 runner    (1001) docker     (127)     4043 2024-03-08 18:08:27.000000 shinylive-0.2.4/shinylive/_export.py
--rw-r--r--   0 runner    (1001) docker     (127)    17783 2024-03-08 18:08:27.000000 shinylive-0.2.4/shinylive/_main.py
--rw-r--r--   0 runner    (1001) docker     (127)    25124 2024-03-08 18:08:27.000000 shinylive-0.2.4/shinylive/_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     4139 2024-03-08 18:08:27.000000 shinylive-0.2.4/shinylive/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 18:08:41.320878 shinylive-0.2.4/shinylive/_version/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-03-08 18:08:27.000000 shinylive-0.2.4/shinylive/_version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 18:08:27.000000 shinylive-0.2.4/shinylive/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 18:08:41.320878 shinylive-0.2.4/shinylive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-03-08 18:08:41.000000 shinylive-0.2.4/shinylive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-03-08 18:08:41.000000 shinylive-0.2.4/shinylive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 18:08:41.000000 shinylive-0.2.4/shinylive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-08 18:08:41.000000 shinylive-0.2.4/shinylive.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 18:08:41.000000 shinylive-0.2.4/shinylive.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-03-08 18:08:41.000000 shinylive-0.2.4/shinylive.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-08 18:08:41.000000 shinylive-0.2.4/shinylive.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:10:10.550255 shinylive-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-16 17:09:52.000000 shinylive-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-04-16 17:10:10.550255 shinylive-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3402 2024-04-16 17:09:52.000000 shinylive-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-04-16 17:10:10.550255 shinylive-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 17:09:52.000000 shinylive-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:10:10.550255 shinylive-0.3.0/shinylive/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-16 17:09:52.000000 shinylive-0.3.0/shinylive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4390 2024-04-16 17:09:52.000000 shinylive-0.3.0/shinylive/_app_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7989 2024-04-16 17:09:52.000000 shinylive-0.3.0/shinylive/_assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19194 2024-04-16 17:09:52.000000 shinylive-0.3.0/shinylive/_deps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4043 2024-04-16 17:09:52.000000 shinylive-0.3.0/shinylive/_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17783 2024-04-16 17:09:52.000000 shinylive-0.3.0/shinylive/_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25113 2024-04-16 17:09:52.000000 shinylive-0.3.0/shinylive/_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4139 2024-04-16 17:09:52.000000 shinylive-0.3.0/shinylive/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:10:10.550255 shinylive-0.3.0/shinylive/_version/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-16 17:09:52.000000 shinylive-0.3.0/shinylive/_version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 17:09:52.000000 shinylive-0.3.0/shinylive/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:10:10.550255 shinylive-0.3.0/shinylive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-04-16 17:10:10.000000 shinylive-0.3.0/shinylive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-16 17:10:10.000000 shinylive-0.3.0/shinylive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 17:10:10.000000 shinylive-0.3.0/shinylive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-16 17:10:10.000000 shinylive-0.3.0/shinylive.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 17:10:10.000000 shinylive-0.3.0/shinylive.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-16 17:10:10.000000 shinylive-0.3.0/shinylive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-16 17:10:10.000000 shinylive-0.3.0/shinylive.egg-info/top_level.txt
```

### Comparing `shinylive-0.2.4/LICENSE` & `shinylive-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `shinylive-0.2.4/PKG-INFO` & `shinylive-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shinylive
-Version: 0.2.4
+Version: 0.3.0
 Summary: Run Shiny applications running Python in the browser.
 Home-page: https://github.com/posit-dev/py-shinylive
 Author: Winston Chang
 Author-email: winston@posit.co
 License: MIT
 Project-URL: Bug Tracker, https://github.com/posit-dev/py-shinylive/issues
 Project-URL: Documentation, https://github.com/posit-dev/py-shinylive
```

### Comparing `shinylive-0.2.4/README.md` & `shinylive-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `shinylive-0.2.4/setup.cfg` & `shinylive-0.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `shinylive-0.2.4/shinylive/_app_json.py` & `shinylive-0.3.0/shinylive/_app_json.py`

 * *Files identical despite different names*

### Comparing `shinylive-0.2.4/shinylive/_assets.py` & `shinylive-0.3.0/shinylive/_assets.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,17 +63,20 @@
     """
     Returns the directory containing cached Shinylive assets, for a particular version
     of Shinylive.
     """
     return os.path.join(shinylive_cache_dir(), "shinylive-" + version)
 
 
-def repodata_json_file(version: str = SHINYLIVE_ASSETS_VERSION) -> Path:
+def pyodide_lock_json_file(version: str = SHINYLIVE_ASSETS_VERSION) -> Path:
     return (
-        Path(shinylive_assets_dir(version)) / "shinylive" / "pyodide" / "repodata.json"
+        Path(shinylive_assets_dir(version))
+        / "shinylive"
+        / "pyodide"
+        / "pyodide-lock.json"
     )
 
 
 def codeblock_to_json_file() -> str:
     p = Path(shinylive_assets_dir()) / "scripts" / "codeblock-to-json.js"
     return str(p)
```

### Comparing `shinylive-0.2.4/shinylive/_deps.py` & `shinylive-0.3.0/shinylive/_deps.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,48 +16,51 @@
 # https://peps.python.org/pep-0655/#usage-in-python-3-11
 if sys.version_info >= (3, 11):
     from typing import NotRequired, TypedDict
 else:
     from typing_extensions import NotRequired, TypedDict
 
 from ._app_json import FileContentJson
-from ._assets import ensure_shinylive_assets, repodata_json_file, shinylive_assets_dir
+from ._assets import (
+    ensure_shinylive_assets,
+    pyodide_lock_json_file,
+    shinylive_assets_dir,
+)
 from ._version import SHINYLIVE_ASSETS_VERSION
 
 # Files in Pyodide that should always be included.
 BASE_PYODIDE_FILES = {
-    "pyodide_py.tar",
     "pyodide.asm.js",
-    "pyodide.asm.data",
     "pyodide.asm.wasm",
-    "repodata.json",
+    "python_stdlib.zip",
+    "pyodide-lock.json",
 }
 
 # Packages that should always be included in a Shinylive deployment.
 BASE_PYODIDE_PACKAGES = {"distutils", "micropip", "ssl"}
 AssetType = Literal["base", "python", "r"]
 
 
 # =============================================================================
-# Data structures used in pyodide/repodata.json
+# Data structures used in pyodide/pyodide-lock.json
 # =============================================================================
 # Note: This block of code is copied from /scripts/pyodide_packages.py
 class PyodidePackageInfo(TypedDict):
     name: str
     version: str
     file_name: str
     install_dir: Literal["lib", "site"]
     sha256: str
     depends: list[str]
     imports: list[str]
     unvendored_tests: NotRequired[bool]
 
 
-# The package information structure used by Pyodide's repodata.json.
-class PyodideRepodataFile(TypedDict):
+# The package information structure used by Pyodide's pyodide-lock.json.
+class PyodideLockFile(TypedDict):
     info: dict[str, str]
     packages: dict[str, PyodidePackageInfo]
 
 
 # =============================================================================
 # HTML Dependency types
 # =============================================================================
@@ -84,17 +87,17 @@
 
 # =============================================================================
 # Conversion functions
 # =============================================================================
 def _dep_names_to_pyodide_pkg_infos(
     dep_names: Iterable[str],
 ) -> list[PyodidePackageInfo]:
-    repodata = _pyodide_repodata()
+    pyodide_lock = _pyodide_lock_data()
     pkg_infos: list[PyodidePackageInfo] = [
-        copy.deepcopy(repodata["packages"][dep_name]) for dep_name in dep_names
+        copy.deepcopy(pyodide_lock["packages"][dep_name]) for dep_name in dep_names
     ]
     return pkg_infos
 
 
 def _pyodide_pkg_info_to_quarto_html_dep_item(
     pkg: PyodidePackageInfo,
 ) -> HtmlDepItem:
@@ -386,56 +389,56 @@
 # =============================================================================
 def _find_recursive_deps(
     pkgs: Iterable[str],
     verbose_print: Callable[..., None] = lambda *args: None,
 ) -> list[str]:
     """
     Given a list of packages, recursively find all dependencies that are contained in
-    repodata.json. This returns a list of all dependencies, including the original
+    pyodide-lock.json. This returns a list of all dependencies, including the original
     packages passed in.
     """
-    repodata = _pyodide_repodata()
+    pyodide_lock = _pyodide_lock_data()
     deps = list(pkgs)
     i = 0
     while i < len(deps):
         dep = deps[i]
-        if dep not in repodata["packages"]:
+        if dep not in pyodide_lock["packages"]:
             # TODO: Need to distinguish between built-in packages and external ones in
             # requirements.txt.
             verbose_print(
-                f"  {dep} not in repodata.json. Assuming it is in base Pyodide or in requirements.txt."
+                f"  {dep} not in pyodide-lock.json. Assuming it is in base Pyodide or in requirements.txt."
             )
             deps.remove(dep)
             continue
 
-        dep_deps = set(repodata["packages"][dep]["depends"])
+        dep_deps = set(pyodide_lock["packages"][dep]["depends"])
         new_deps = dep_deps.difference(deps)
         deps.extend(new_deps)
         i += 1
 
     return deps
 
 
 def _dep_name_to_dep_file(dep_name: str) -> str:
     """
     Given the name of a dependency, like "pandas", return the name of the .whl file,
     like "pandas-1.4.2-cp310-cp310-emscripten_3_1_14_wasm32.whl".
     """
-    repodata = _pyodide_repodata()
-    return repodata["packages"][dep_name]["file_name"]
+    pyodide_lock = _pyodide_lock_data()
+    return pyodide_lock["packages"][dep_name]["file_name"]
 
 
 def _dep_names_to_dep_files(dep_names: list[str]) -> list[str]:
     """
     Given a list of dependency names, like ["pandas"], return a list with the names of
-    corresponding .whl files (from data in repodata.json), like
+    corresponding .whl files (from data in pyodide-lock.json), like
     ["pandas-1.4.2-cp310-cp310-emscripten_3_1_14_wasm32.whl"].
     """
-    repodata = _pyodide_repodata()
-    dep_files = [repodata["packages"][x]["file_name"] for x in dep_names]
+    pyodide_lock = _pyodide_lock_data()
+    dep_files = [pyodide_lock["packages"][x]["file_name"] for x in dep_names]
     return dep_files
 
 
 def _find_import_app_contents(app_contents: list[FileContentJson]) -> set[str]:
     """
     Given an app.json file, find packages that are imported.
     """
@@ -490,32 +493,32 @@
 @functools.lru_cache
 def _module_to_package_mappings() -> dict[str, str]:
     """
     Return a dictionary that maps module names to package names. This is needed because
     sometimes the module name and package name are different. For example, the module
     name is "cv2", but the package name is "opencv-python".
     """
-    repodata = _pyodide_repodata()
+    pyodide_lock = _pyodide_lock_data()
     module_to_package: dict[str, str] = {}
-    for pkg_name, pkg_info in repodata["packages"].items():
+    for pkg_name, pkg_info in pyodide_lock["packages"].items():
         modules = pkg_info["imports"]
         for module in modules:
             module_to_package[module] = pkg_name
 
     return module_to_package
 
 
 @functools.lru_cache
-def _pyodide_repodata() -> PyodideRepodataFile:
+def _pyodide_lock_data() -> PyodideLockFile:
     """
-    Read in the Pyodide repodata.json file and return the contents. The result is
+    Read in the Pyodide pyodide-lock.json file and return the contents. The result is
     cached, so if the file changes, it won't register until the Python session is
     restarted.
     """
-    with open(repodata_json_file(), "r") as f:
+    with open(pyodide_lock_json_file(), "r") as f:
         return json.load(f)
 
 
 # From pyodide._base.find_imports
 def _find_imports(source: str) -> list[str]:
     """
     Finds the imports in a Python source code string
```

### Comparing `shinylive-0.2.4/shinylive/_export.py` & `shinylive-0.3.0/shinylive/_export.py`

 * *Files identical despite different names*

### Comparing `shinylive-0.2.4/shinylive/_main.py` & `shinylive-0.3.0/shinylive/_main.py`

 * *Files identical despite different names*

### Comparing `shinylive-0.2.4/shinylive/_url.py` & `shinylive-0.3.0/shinylive/_url.py`

 * *Files 0% similar despite different names*

```diff
@@ -749,8 +749,8 @@
 
 
 def lzstring_file_bundle(file_bundle: list[FileContentJson]) -> str:
     from lzstring import LZString  # type: ignore[reportMissingTypeStubs]
 
     file_json = json.dumps(file_bundle)
     file_lz = LZString.compressToEncodedURIComponent(file_json)  # type: ignore[reportUnknownMemberType]
-    return cast(str, file_lz)
+    return file_lz
```

### Comparing `shinylive-0.2.4/shinylive/_utils.py` & `shinylive-0.3.0/shinylive/_utils.py`

 * *Files identical despite different names*

### Comparing `shinylive-0.2.4/shinylive.egg-info/PKG-INFO` & `shinylive-0.3.0/shinylive.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shinylive
-Version: 0.2.4
+Version: 0.3.0
 Summary: Run Shiny applications running Python in the browser.
 Home-page: https://github.com/posit-dev/py-shinylive
 Author: Winston Chang
 Author-email: winston@posit.co
 License: MIT
 Project-URL: Bug Tracker, https://github.com/posit-dev/py-shinylive/issues
 Project-URL: Documentation, https://github.com/posit-dev/py-shinylive
```

