# Comparing `tmp/venv-modulefile-0.1.4.tar.gz` & `tmp/venv-modulefile-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/volatile/catA/rl222169/softs/custom_venv/venv-modulefile/dist/tmpbx1x118q/venv-modulefile-0.1.4.tar", last modified: Wed Sep  6 10:17:10 2023, max compression
+gzip compressed data, was "/volatile/catA/rl222169/softs/custom_venv/venv-modulefile/dist/tmp00a4m8hm/venv-modulefile-0.1.5.tar", last modified: Tue Apr 16 10:40:54 2024, max compression
```

## Comparing `venv-modulefile-0.1.4.tar` & `venv-modulefile-0.1.5.tar`

### file list

```diff
@@ -1,27 +1,31 @@
-drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2023-09-06 10:17:10.000000 venv-modulefile-0.1.4/
-drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2023-09-06 10:17:10.000000 venv-modulefile-0.1.4/src/
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     2899 2023-09-06 09:44:52.000000 venv-modulefile-0.1.4/src/README.md
-drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2023-09-06 10:17:10.000000 venv-modulefile-0.1.4/src/venv_modulefile.egg-info/
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     4043 2023-09-06 10:17:10.000000 venv-modulefile-0.1.4/src/venv_modulefile.egg-info/PKG-INFO
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      567 2023-09-06 10:17:10.000000 venv-modulefile-0.1.4/src/venv_modulefile.egg-info/SOURCES.txt
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      241 2023-09-06 10:17:10.000000 venv-modulefile-0.1.4/src/venv_modulefile.egg-info/requires.txt
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      807 2023-09-06 10:17:10.000000 venv-modulefile-0.1.4/src/venv_modulefile.egg-info/entry_points.txt
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)        1 2023-09-06 10:17:10.000000 venv-modulefile-0.1.4/src/venv_modulefile.egg-info/dependency_links.txt
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)        8 2023-09-06 10:17:10.000000 venv-modulefile-0.1.4/src/venv_modulefile.egg-info/top_level.txt
-drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2023-09-06 10:17:10.000000 venv-modulefile-0.1.4/src/venvmod/
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)        6 2023-09-06 10:15:43.000000 venv-modulefile-0.1.4/src/venvmod/VERSION
-drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2023-09-06 10:17:10.000000 venv-modulefile-0.1.4/src/venvmod/commands/
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)    11077 2023-09-06 09:44:52.000000 venv-modulefile-0.1.4/src/venvmod/commands/append_module.py
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     3825 2023-09-06 09:44:52.000000 venv-modulefile-0.1.4/src/venvmod/commands/__init__.py
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     5049 2023-09-06 09:44:52.000000 venv-modulefile-0.1.4/src/venvmod/commands/create_module.py
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     1715 2023-09-06 09:44:52.000000 venv-modulefile-0.1.4/src/venvmod/commands/test_imports.py
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     1624 2023-09-06 09:44:52.000000 venv-modulefile-0.1.4/src/venvmod/tools.py
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)    10672 2023-09-06 10:13:18.000000 venv-modulefile-0.1.4/src/venvmod/modulefile.py
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      247 2023-09-06 09:44:52.000000 venv-modulefile-0.1.4/src/venvmod/__init__.py
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     1302 2023-09-06 09:44:52.000000 venv-modulefile-0.1.4/LICENSE.md
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)       81 2023-09-06 09:44:52.000000 venv-modulefile-0.1.4/pyproject.toml
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     9606 2023-09-06 09:44:52.000000 venv-modulefile-0.1.4/setup.py
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      959 2023-09-06 09:44:52.000000 venv-modulefile-0.1.4/README.md
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)       38 2023-09-06 10:17:10.000000 venv-modulefile-0.1.4/setup.cfg
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     4043 2023-09-06 10:17:10.000000 venv-modulefile-0.1.4/PKG-INFO
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)       22 2023-09-06 09:44:52.000000 venv-modulefile-0.1.4/MANIFEST.in
+drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2024-04-16 10:40:54.000000 venv-modulefile-0.1.5/
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     9786 2024-04-16 09:35:06.000000 venv-modulefile-0.1.5/setup.py
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     1302 2023-12-08 12:27:33.000000 venv-modulefile-0.1.5/LICENSE.md
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      193 2024-04-16 09:01:17.000000 venv-modulefile-0.1.5/MANIFEST.in
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)       81 2023-12-08 12:27:33.000000 venv-modulefile-0.1.5/pyproject.toml
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      959 2023-12-08 12:27:33.000000 venv-modulefile-0.1.5/README.md
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)       38 2024-04-16 10:40:54.000000 venv-modulefile-0.1.5/setup.cfg
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     4043 2024-04-16 10:40:54.000000 venv-modulefile-0.1.5/PKG-INFO
+drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2024-04-16 10:40:54.000000 venv-modulefile-0.1.5/src/
+drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2024-04-16 10:40:54.000000 venv-modulefile-0.1.5/src/venvmod/
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      247 2024-04-16 10:01:25.000000 venv-modulefile-0.1.5/src/venvmod/__init__.py
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     1624 2023-12-08 12:27:33.000000 venv-modulefile-0.1.5/src/venvmod/tools.py
+drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2024-04-16 10:40:54.000000 venv-modulefile-0.1.5/src/venvmod/commands/
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     3825 2023-12-08 12:27:33.000000 venv-modulefile-0.1.5/src/venvmod/commands/__init__.py
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     5049 2023-12-08 12:27:33.000000 venv-modulefile-0.1.5/src/venvmod/commands/create_module.py
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     1715 2023-12-08 12:27:33.000000 venv-modulefile-0.1.5/src/venvmod/commands/test_imports.py
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)    11077 2023-12-08 12:27:33.000000 venv-modulefile-0.1.5/src/venvmod/commands/append_module.py
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)    11302 2024-04-16 10:22:44.000000 venv-modulefile-0.1.5/src/venvmod/modulefile.py
+drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2024-04-16 10:40:54.000000 venv-modulefile-0.1.5/src/venvmod/modulefiles_src/
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)  2231175 2024-02-20 12:00:21.000000 venv-modulefile-0.1.5/src/venvmod/modulefiles_src/modules-5.4.0.tar.gz
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)  2135014 2023-06-27 18:51:07.000000 venv-modulefile-0.1.5/src/venvmod/modulefiles_src/modules-5.3.1.tar.gz
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)  2021637 2022-11-08 06:06:08.000000 venv-modulefile-0.1.5/src/venvmod/modulefiles_src/modules-5.2.0.tar.gz
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)        6 2024-04-16 10:28:29.000000 venv-modulefile-0.1.5/src/venvmod/VERSION
+drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2024-04-16 10:40:54.000000 venv-modulefile-0.1.5/src/venv_modulefile.egg-info/
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)        8 2024-04-16 10:40:54.000000 venv-modulefile-0.1.5/src/venv_modulefile.egg-info/top_level.txt
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      241 2024-04-16 10:40:54.000000 venv-modulefile-0.1.5/src/venv_modulefile.egg-info/requires.txt
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)        1 2024-04-16 10:40:54.000000 venv-modulefile-0.1.5/src/venv_modulefile.egg-info/dependency_links.txt
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      714 2024-04-16 10:40:54.000000 venv-modulefile-0.1.5/src/venv_modulefile.egg-info/SOURCES.txt
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     4043 2024-04-16 10:40:54.000000 venv-modulefile-0.1.5/src/venv_modulefile.egg-info/PKG-INFO
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      807 2024-04-16 10:40:54.000000 venv-modulefile-0.1.5/src/venv_modulefile.egg-info/entry_points.txt
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     2899 2023-12-08 12:27:33.000000 venv-modulefile-0.1.5/src/README.md
```

### Comparing `venv-modulefile-0.1.4/src/README.md` & `venv-modulefile-0.1.5/src/README.md`

 * *Files identical despite different names*

### Comparing `venv-modulefile-0.1.4/src/venv_modulefile.egg-info/PKG-INFO` & `venv-modulefile-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: venv-modulefile
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python venv extension using Modulefile
 Home-page: https://github.com/code-coupling/venv-modulefile
 Author: R. Lenain
 Author-email: roland.lenain@cea.fr
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/code-coupling/venv-modulefile/issues
 Project-URL: Doc, https://venv-modulefile.readthedocs.io/en/latest/index.html
```

### Comparing `venv-modulefile-0.1.4/src/venv_modulefile.egg-info/entry_points.txt` & `venv-modulefile-0.1.5/src/venv_modulefile.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `venv-modulefile-0.1.4/src/venvmod/commands/append_module.py` & `venv-modulefile-0.1.5/src/venvmod/commands/append_module.py`

 * *Files identical despite different names*

### Comparing `venv-modulefile-0.1.4/src/venvmod/commands/__init__.py` & `venv-modulefile-0.1.5/src/venvmod/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `venv-modulefile-0.1.4/src/venvmod/commands/create_module.py` & `venv-modulefile-0.1.5/src/venvmod/commands/create_module.py`

 * *Files identical despite different names*

### Comparing `venv-modulefile-0.1.4/src/venvmod/commands/test_imports.py` & `venv-modulefile-0.1.5/src/venvmod/commands/test_imports.py`

 * *Files identical despite different names*

### Comparing `venv-modulefile-0.1.4/src/venvmod/tools.py` & `venv-modulefile-0.1.5/src/venvmod/tools.py`

 * *Files identical despite different names*

### Comparing `venv-modulefile-0.1.4/src/venvmod/modulefile.py` & `venv-modulefile-0.1.5/src/venvmod/modulefile.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Environment module modification/installation."""
 
 import os
 import shutil
+import sys
 from pathlib import Path
 import pathlib
 import subprocess
 import tarfile
 
 from packaging import version
 import requests
@@ -103,23 +104,34 @@
                                 f" found {self._version_or_path}."
                         )
             build_directory = self._cache_directory / f"modules-{self._version_or_path}"
             if not build_directory.exists():
                 cwd = os.getcwd()
                 os.chdir(self._cache_directory)
                 try:
-                    file = tarfile.open(  # pylint: disable=consider-using-with
-                        fileobj=requests.get(
-                            url="https://github.com/cea-hpc/modules/releases/download/"
-                                f"v{self._version_or_path}/modules-{self._version_or_path}.tar.gz",
-                            stream=True,
-                            timeout=120.0).raw,
-                        mode="r|gz")
+                    tar_file = (Path(__file__).parent.absolute().resolve() /
+                                "modulefiles_src" / f"modules-{self._version_or_path}.tar.gz")
+                    if tar_file.exists():
+                        file = tarfile.open(  # pylint: disable=consider-using-with
+                            tar_file,
+                            mode="r|gz")
+                    else:
+                        file = tarfile.open(  # pylint: disable=consider-using-with
+                            fileobj=requests.get(
+                                url="https://github.com/cea-hpc/modules/releases/download/"
+                                    f"v{self._version_or_path}/"
+                                    f"modules-{self._version_or_path}.tar.gz",
+                                stream=True,
+                                timeout=120.0).raw,
+                            mode="r|gz")
                     try:
-                        file.extractall()
+                        if sys.version_info >= (3, 8):
+                            file.extractall(filter='data')
+                        else:
+                            file.extractall()
                     finally:
                         file.close()
                 finally:
                     os.chdir(cwd)
 
         pipe = subprocess.PIPE if not verbose else None
         for command in [[f"{build_directory}/configure",
```

### Comparing `venv-modulefile-0.1.4/LICENSE.md` & `venv-modulefile-0.1.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `venv-modulefile-0.1.4/setup.py` & `venv-modulefile-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,15 +161,18 @@
                  "pytest-html>=3.2.0",
                  "pytest-sugar>=0.9.6",
                  "pytest-xdist>=3.0.2", ],
     },
     # If there are data files included in your packages that need to be
     # installed, specify them here.
     package_data={  # Optional
-        "venvmod": ["VERSION"],
+        "venvmod": ["VERSION",
+                    "modulefiles_src/modules-5.2.0.tar.gz",
+                    "modulefiles_src/modules-5.3.1.tar.gz",
+                    "modulefiles_src/modules-5.4.0.tar.gz"],
     },
     # Entry points. The following would provide a command called `sample` which
     # executes the function `main` from this package when invoked:
     entry_points={  # Optional
         "console_scripts": [
             "venvmod-initialize=venvmod.commands.create_module:initialize",
             "venvmod-add-appli=venvmod.commands.create_module:add_appli",
```

### Comparing `venv-modulefile-0.1.4/README.md` & `venv-modulefile-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `venv-modulefile-0.1.4/PKG-INFO` & `venv-modulefile-0.1.5/src/venv_modulefile.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: venv-modulefile
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python venv extension using Modulefile
 Home-page: https://github.com/code-coupling/venv-modulefile
 Author: R. Lenain
 Author-email: roland.lenain@cea.fr
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/code-coupling/venv-modulefile/issues
 Project-URL: Doc, https://venv-modulefile.readthedocs.io/en/latest/index.html
```

