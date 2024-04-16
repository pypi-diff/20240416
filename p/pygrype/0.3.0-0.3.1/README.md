# Comparing `tmp/pygrype-0.3.0.tar.gz` & `tmp/pygrype-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygrype-0.3.0.tar", last modified: Wed Apr 10 13:44:29 2024, max compression
+gzip compressed data, was "pygrype-0.3.1.tar", last modified: Tue Apr 16 09:32:25 2024, max compression
```

## Comparing `pygrype-0.3.0.tar` & `pygrype-0.3.1.tar`

### file list

```diff
@@ -1,49 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:44:29.696793 pygrype-0.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:44:29.688793 pygrype-0.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:44:29.688793 pygrype-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-10 13:44:24.000000 pygrype-0.3.0/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-10 13:44:24.000000 pygrype-0.3.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-10 13:44:24.000000 pygrype-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-10 13:44:24.000000 pygrype-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-10 13:44:29.696793 pygrype-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-10 13:44:24.000000 pygrype-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:44:29.688793 pygrype-0.3.0/pygrype/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-10 13:44:24.000000 pygrype-0.3.0/pygrype/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:44:29.692793 pygrype-0.3.0/pygrype/core/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:44:29.692793 pygrype-0.3.0/pygrype/core/decorators/
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-10 13:44:24.000000 pygrype-0.3.0/pygrype/core/decorators/to_json.py
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-10 13:44:24.000000 pygrype-0.3.0/pygrype/core/grype_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:44:29.692793 pygrype-0.3.0/pygrype/core/list/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-10 13:44:24.000000 pygrype-0.3.0/pygrype/core/list/db_meta_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:44:29.696793 pygrype-0.3.0/pygrype/core/scan/
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-10 13:44:24.000000 pygrype-0.3.0/pygrype/core/scan/artifact.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-10 13:44:24.000000 pygrype-0.3.0/pygrype/core/scan/cvss.py
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-10 13:44:24.000000 pygrype-0.3.0/pygrype/core/scan/cvss_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-10 13:44:24.000000 pygrype-0.3.0/pygrype/core/scan/distro.py
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-10 13:44:24.000000 pygrype-0.3.0/pygrype/core/scan/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-10 13:44:24.000000 pygrype-0.3.0/pygrype/core/scan/location.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-10 13:44:24.000000 pygrype-0.3.0/pygrype/core/scan/match.py
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-10 13:44:24.000000 pygrype-0.3.0/pygrype/core/scan/match_details.py
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-10 13:44:24.000000 pygrype-0.3.0/pygrype/core/scan/match_details_found.py
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-10 13:44:24.000000 pygrype-0.3.0/pygrype/core/scan/match_details_searched_by.py
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-10 13:44:24.000000 pygrype-0.3.0/pygrype/core/scan/package.py
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-10 13:44:24.000000 pygrype-0.3.0/pygrype/core/scan/scan.py
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-10 13:44:24.000000 pygrype-0.3.0/pygrype/core/scan/scan_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-10 13:44:24.000000 pygrype-0.3.0/pygrype/core/scan/searched_by_distro.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-10 13:44:24.000000 pygrype-0.3.0/pygrype/core/scan/target.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-10 13:44:24.000000 pygrype-0.3.0/pygrype/core/scan/upstream.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-10 13:44:24.000000 pygrype-0.3.0/pygrype/core/scan/vulnerability.py
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-10 13:44:24.000000 pygrype-0.3.0/pygrype/core/scan/vulnerability_fix.py
--rw-r--r--   0 runner    (1001) docker     (127)     4752 2024-04-10 13:44:24.000000 pygrype-0.3.0/pygrype/grype.py
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-10 13:44:24.000000 pygrype-0.3.0/pygrype/grype_db.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:44:29.696793 pygrype-0.3.0/pygrype.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-10 13:44:29.000000 pygrype-0.3.0/pygrype.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-10 13:44:29.000000 pygrype-0.3.0/pygrype.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 13:44:29.000000 pygrype-0.3.0/pygrype.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-10 13:44:29.000000 pygrype-0.3.0/pygrype.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-10 13:44:29.000000 pygrype-0.3.0/pygrype.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-10 13:44:24.000000 pygrype-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-10 13:44:24.000000 pygrype-0.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 13:44:29.696793 pygrype-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:44:29.696793 pygrype-0.3.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-10 13:44:24.000000 pygrype-0.3.0/test/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:32:25.166613 pygrype-0.3.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:32:25.158614 pygrype-0.3.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:32:25.162613 pygrype-0.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-16 09:32:20.000000 pygrype-0.3.1/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-16 09:32:20.000000 pygrype-0.3.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-16 09:32:20.000000 pygrype-0.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-16 09:32:20.000000 pygrype-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-16 09:32:25.166613 pygrype-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-16 09:32:20.000000 pygrype-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:32:25.162613 pygrype-0.3.1/pygrype/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-16 09:32:20.000000 pygrype-0.3.1/pygrype/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:32:25.162613 pygrype-0.3.1/pygrype/core/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:32:25.162613 pygrype-0.3.1/pygrype/core/decorators/
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-16 09:32:20.000000 pygrype-0.3.1/pygrype/core/decorators/to_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-16 09:32:20.000000 pygrype-0.3.1/pygrype/core/grype_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:32:25.162613 pygrype-0.3.1/pygrype/core/list/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-16 09:32:20.000000 pygrype-0.3.1/pygrype/core/list/db_meta_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:32:25.166613 pygrype-0.3.1/pygrype/core/scan/
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-16 09:32:20.000000 pygrype-0.3.1/pygrype/core/scan/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-16 09:32:20.000000 pygrype-0.3.1/pygrype/core/scan/cvss.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-16 09:32:20.000000 pygrype-0.3.1/pygrype/core/scan/cvss_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-16 09:32:20.000000 pygrype-0.3.1/pygrype/core/scan/distro.py
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-16 09:32:20.000000 pygrype-0.3.1/pygrype/core/scan/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-16 09:32:20.000000 pygrype-0.3.1/pygrype/core/scan/location.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-16 09:32:20.000000 pygrype-0.3.1/pygrype/core/scan/match.py
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-16 09:32:20.000000 pygrype-0.3.1/pygrype/core/scan/match_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-16 09:32:20.000000 pygrype-0.3.1/pygrype/core/scan/match_details_found.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-16 09:32:20.000000 pygrype-0.3.1/pygrype/core/scan/match_details_searched_by.py
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-16 09:32:20.000000 pygrype-0.3.1/pygrype/core/scan/package.py
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-16 09:32:20.000000 pygrype-0.3.1/pygrype/core/scan/scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-16 09:32:20.000000 pygrype-0.3.1/pygrype/core/scan/scan_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-16 09:32:20.000000 pygrype-0.3.1/pygrype/core/scan/searched_by_distro.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-16 09:32:20.000000 pygrype-0.3.1/pygrype/core/scan/target.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-16 09:32:20.000000 pygrype-0.3.1/pygrype/core/scan/upstream.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-16 09:32:20.000000 pygrype-0.3.1/pygrype/core/scan/vulnerability.py
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-16 09:32:20.000000 pygrype-0.3.1/pygrype/core/scan/vulnerability_fix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4844 2024-04-16 09:32:20.000000 pygrype-0.3.1/pygrype/grype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-16 09:32:20.000000 pygrype-0.3.1/pygrype/grype_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-16 09:32:20.000000 pygrype-0.3.1/pygrype/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:32:25.166613 pygrype-0.3.1/pygrype.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-16 09:32:25.000000 pygrype-0.3.1/pygrype.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-16 09:32:25.000000 pygrype-0.3.1/pygrype.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 09:32:25.000000 pygrype-0.3.1/pygrype.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-16 09:32:25.000000 pygrype-0.3.1/pygrype.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-16 09:32:25.000000 pygrype-0.3.1/pygrype.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-16 09:32:20.000000 pygrype-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-16 09:32:20.000000 pygrype-0.3.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 09:32:25.166613 pygrype-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:32:25.166613 pygrype-0.3.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-16 09:32:20.000000 pygrype-0.3.1/test/test_version.py
```

### Comparing `pygrype-0.3.0/.github/workflows/python-package.yml` & `pygrype-0.3.1/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `pygrype-0.3.0/.github/workflows/python-publish.yml` & `pygrype-0.3.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pygrype-0.3.0/.gitignore` & `pygrype-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pygrype-0.3.0/LICENSE` & `pygrype-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pygrype-0.3.0/PKG-INFO` & `pygrype-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygrype
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python wrapper for Grype
 Author-email: Albert Simon <simon.albert75@gmail.com>
 License: MIT License
 Keywords: anchore,grype,security
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Framework :: IPython
```

### Comparing `pygrype-0.3.0/README.md` & `pygrype-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `pygrype-0.3.0/pygrype/grype.py` & `pygrype-0.3.1/pygrype/grype.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,38 +5,39 @@
 from typing import List
 
 from dacite import from_dict
 
 from pygrype.core.grype_version import GrypeVersion
 from pygrype.core.scan.scan import Scan
 from pygrype.grype_db import _GrypeDB
-
+from pygrype.logging import get_logger
 
 class Grype:
     """A class representing the Grype vulnerability scanner."""
 
     path: str
     db: _GrypeDB
+    logger: logging.Logger = get_logger()
 
     def __init__(self, path: str = 'grype') -> None:
         """Initialize the Grype object.
 
         Args:
             path (str, optional): The path to the Grype executable. Defaults to 'grype'.
 
         Raises:
             Exception: If Grype is not found at the specified path.
         """
         if not shutil.which(path):
-            logging.error(f'Grype was not found at: {path}')
+            self.logger.error(f'Grype was not found at: {path}')
             raise Exception(f'Grype was not found at: {path}')
         self.path = path
         self.db = _GrypeDB(self.path)
 
-        logging.info(f'Using Grype {self.version().version}')
+        self.logger.info(f'Using Grype {self.version().version}')
 
     def version(self) -> GrypeVersion:
         """Get the version of Grype.
 
         Returns:
             Dict: A dictionary containing the version information.
         """
@@ -107,15 +108,15 @@
         if platform:
             args += ['--platform', platform]
         if scope:
             args += ['--scope', scope]
         if show_supressed:
             args.append('--show-supressed')
 
-        logging.debug(f'Running: {args}')
+        self.logger.debug(f'Running: {args}')
 
         process = subprocess.run(
             args=args,
             capture_output=True
         )
 
         data = json.loads(process.stdout)
```

### Comparing `pygrype-0.3.0/pygrype/grype_db.py` & `pygrype-0.3.1/pygrype/grype_db.py`

 * *Files identical despite different names*

### Comparing `pygrype-0.3.0/pygrype.egg-info/PKG-INFO` & `pygrype-0.3.1/pygrype.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygrype
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python wrapper for Grype
 Author-email: Albert Simon <simon.albert75@gmail.com>
 License: MIT License
 Keywords: anchore,grype,security
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Framework :: IPython
```

### Comparing `pygrype-0.3.0/pygrype.egg-info/SOURCES.txt` & `pygrype-0.3.1/pygrype.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 pyproject.toml
 requirements.txt
 .github/workflows/python-package.yml
 .github/workflows/python-publish.yml
 pygrype/__init__.py
 pygrype/grype.py
 pygrype/grype_db.py
+pygrype/logging.py
 pygrype.egg-info/PKG-INFO
 pygrype.egg-info/SOURCES.txt
 pygrype.egg-info/dependency_links.txt
 pygrype.egg-info/requires.txt
 pygrype.egg-info/top_level.txt
 pygrype/core/grype_version.py
 pygrype/core/decorators/to_json.py
```

### Comparing `pygrype-0.3.0/pyproject.toml` & `pygrype-0.3.1/pyproject.toml`

 * *Files identical despite different names*

