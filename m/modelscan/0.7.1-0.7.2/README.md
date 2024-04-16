# Comparing `tmp/modelscan-0.7.1.tar.gz` & `tmp/modelscan-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelscan-0.7.1.tar", max compression
+gzip compressed data, was "modelscan-0.7.2.tar", max compression
```

## Comparing `modelscan-0.7.1.tar` & `modelscan-0.7.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0    10754 2024-04-15 22:17:57.815445 modelscan-0.7.1/LICENSE
--rw-r--r--   0        0        0    12564 2024-04-15 22:17:57.815445 modelscan-0.7.1/README.md
--rw-r--r--   0        0        0      156 2024-04-15 22:17:57.831445 modelscan-0.7.1/modelscan/__init__.py
--rw-r--r--   0        0        0       22 2024-04-15 22:18:12.847517 modelscan-0.7.1/modelscan/_version.py
--rw-r--r--   0        0        0     6154 2024-04-15 22:17:57.831445 modelscan-0.7.1/modelscan/cli.py
--rw-r--r--   0        0        0     2455 2024-04-15 22:17:57.831445 modelscan-0.7.1/modelscan/error.py
--rw-r--r--   0        0        0     4697 2024-04-15 22:17:57.831445 modelscan-0.7.1/modelscan/issues.py
--rw-r--r--   0        0        0       84 2024-04-15 22:17:57.831445 modelscan-0.7.1/modelscan/middlewares/__init__.py
--rw-r--r--   0        0        0      585 2024-04-15 22:17:57.831445 modelscan-0.7.1/modelscan/middlewares/format_via_extension.py
--rw-r--r--   0        0        0     1757 2024-04-15 22:17:57.831445 modelscan-0.7.1/modelscan/middlewares/middleware.py
--rw-r--r--   0        0        0     1458 2024-04-15 22:17:57.831445 modelscan-0.7.1/modelscan/model.py
--rw-r--r--   0        0        0    13276 2024-04-15 22:17:57.831445 modelscan-0.7.1/modelscan/modelscan.py
--rw-r--r--   0        0        0     2993 2024-04-15 22:17:57.831445 modelscan-0.7.1/modelscan/reports.py
--rw-r--r--   0        0        0      377 2024-04-15 22:17:57.831445 modelscan-0.7.1/modelscan/scanners/__init__.py
--rw-r--r--   0        0        0        0 2024-04-15 22:17:57.831445 modelscan-0.7.1/modelscan/scanners/h5/__init__.py
--rw-r--r--   0        0        0     4611 2024-04-15 22:17:57.831445 modelscan-0.7.1/modelscan/scanners/h5/scan.py
--rw-r--r--   0        0        0        0 2024-04-15 22:17:57.831445 modelscan-0.7.1/modelscan/scanners/keras/__init__.py
--rw-r--r--   0        0        0     4451 2024-04-15 22:17:57.831445 modelscan-0.7.1/modelscan/scanners/keras/scan.py
--rw-r--r--   0        0        0        0 2024-04-15 22:17:57.831445 modelscan-0.7.1/modelscan/scanners/pickle/__init__.py
--rw-r--r--   0        0        0     1972 2024-04-15 22:17:57.831445 modelscan-0.7.1/modelscan/scanners/pickle/scan.py
--rw-r--r--   0        0        0        0 2024-04-15 22:17:57.831445 modelscan-0.7.1/modelscan/scanners/saved_model/__init__.py
--rw-r--r--   0        0        0     6853 2024-04-15 22:17:57.831445 modelscan-0.7.1/modelscan/scanners/saved_model/scan.py
--rw-r--r--   0        0        0     1652 2024-04-15 22:17:57.831445 modelscan-0.7.1/modelscan/scanners/scan.py
--rw-r--r--   0        0        0     4412 2024-04-15 22:17:57.831445 modelscan-0.7.1/modelscan/settings.py
--rw-r--r--   0        0        0      892 2024-04-15 22:17:57.831445 modelscan-0.7.1/modelscan/skip.py
--rw-r--r--   0        0        0     2591 2024-04-15 22:17:57.831445 modelscan-0.7.1/modelscan/tools/LICENSE
--rw-r--r--   0        0        0     3435 2024-04-15 22:17:57.831445 modelscan-0.7.1/modelscan/tools/cli_utils.py
--rw-r--r--   0        0        0     9598 2024-04-15 22:17:57.831445 modelscan-0.7.1/modelscan/tools/picklescanner.py
--rw-r--r--   0        0        0     2989 2024-04-15 22:17:57.831445 modelscan-0.7.1/modelscan/tools/utils.py
--rw-r--r--   0        0        0     1629 2024-04-15 22:18:13.203519 modelscan-0.7.1/pyproject.toml
--rw-r--r--   0        0        0    13840 1970-01-01 00:00:00.000000 modelscan-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0    10754 2024-04-15 23:00:01.848000 modelscan-0.7.2/LICENSE
+-rw-r--r--   0        0        0    12564 2024-04-15 23:00:01.848000 modelscan-0.7.2/README.md
+-rw-r--r--   0        0        0      156 2024-04-15 23:00:01.864000 modelscan-0.7.2/modelscan/__init__.py
+-rw-r--r--   0        0        0       22 2024-04-15 23:00:21.200141 modelscan-0.7.2/modelscan/_version.py
+-rw-r--r--   0        0        0     6154 2024-04-15 23:00:01.864000 modelscan-0.7.2/modelscan/cli.py
+-rw-r--r--   0        0        0     2455 2024-04-15 23:00:01.864000 modelscan-0.7.2/modelscan/error.py
+-rw-r--r--   0        0        0     4697 2024-04-15 23:00:01.864000 modelscan-0.7.2/modelscan/issues.py
+-rw-r--r--   0        0        0       84 2024-04-15 23:00:01.864000 modelscan-0.7.2/modelscan/middlewares/__init__.py
+-rw-r--r--   0        0        0      585 2024-04-15 23:00:01.864000 modelscan-0.7.2/modelscan/middlewares/format_via_extension.py
+-rw-r--r--   0        0        0     1757 2024-04-15 23:00:01.864000 modelscan-0.7.2/modelscan/middlewares/middleware.py
+-rw-r--r--   0        0        0     1458 2024-04-15 23:00:01.864000 modelscan-0.7.2/modelscan/model.py
+-rw-r--r--   0        0        0    13130 2024-04-15 23:00:01.864000 modelscan-0.7.2/modelscan/modelscan.py
+-rw-r--r--   0        0        0     2993 2024-04-15 23:00:01.864000 modelscan-0.7.2/modelscan/reports.py
+-rw-r--r--   0        0        0      377 2024-04-15 23:00:01.864000 modelscan-0.7.2/modelscan/scanners/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-15 23:00:01.864000 modelscan-0.7.2/modelscan/scanners/h5/__init__.py
+-rw-r--r--   0        0        0     4611 2024-04-15 23:00:01.864000 modelscan-0.7.2/modelscan/scanners/h5/scan.py
+-rw-r--r--   0        0        0        0 2024-04-15 23:00:01.864000 modelscan-0.7.2/modelscan/scanners/keras/__init__.py
+-rw-r--r--   0        0        0     4451 2024-04-15 23:00:01.864000 modelscan-0.7.2/modelscan/scanners/keras/scan.py
+-rw-r--r--   0        0        0        0 2024-04-15 23:00:01.864000 modelscan-0.7.2/modelscan/scanners/pickle/__init__.py
+-rw-r--r--   0        0        0     1972 2024-04-15 23:00:01.864000 modelscan-0.7.2/modelscan/scanners/pickle/scan.py
+-rw-r--r--   0        0        0        0 2024-04-15 23:00:01.864000 modelscan-0.7.2/modelscan/scanners/saved_model/__init__.py
+-rw-r--r--   0        0        0     6853 2024-04-15 23:00:01.864000 modelscan-0.7.2/modelscan/scanners/saved_model/scan.py
+-rw-r--r--   0        0        0     1652 2024-04-15 23:00:01.864000 modelscan-0.7.2/modelscan/scanners/scan.py
+-rw-r--r--   0        0        0     4412 2024-04-15 23:00:01.864000 modelscan-0.7.2/modelscan/settings.py
+-rw-r--r--   0        0        0      892 2024-04-15 23:00:01.864000 modelscan-0.7.2/modelscan/skip.py
+-rw-r--r--   0        0        0     2591 2024-04-15 23:00:01.864000 modelscan-0.7.2/modelscan/tools/LICENSE
+-rw-r--r--   0        0        0     3435 2024-04-15 23:00:01.864000 modelscan-0.7.2/modelscan/tools/cli_utils.py
+-rw-r--r--   0        0        0     9598 2024-04-15 23:00:01.864000 modelscan-0.7.2/modelscan/tools/picklescanner.py
+-rw-r--r--   0        0        0     2989 2024-04-15 23:00:01.864000 modelscan-0.7.2/modelscan/tools/utils.py
+-rw-r--r--   0        0        0     1629 2024-04-15 23:00:21.580145 modelscan-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0    13840 1970-01-01 00:00:00.000000 modelscan-0.7.2/PKG-INFO
```

### Comparing `modelscan-0.7.1/LICENSE` & `modelscan-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `modelscan-0.7.1/README.md` & `modelscan-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `modelscan-0.7.1/modelscan/cli.py` & `modelscan-0.7.2/modelscan/cli.py`

 * *Files identical despite different names*

### Comparing `modelscan-0.7.1/modelscan/error.py` & `modelscan-0.7.2/modelscan/error.py`

 * *Files identical despite different names*

### Comparing `modelscan-0.7.1/modelscan/issues.py` & `modelscan-0.7.2/modelscan/issues.py`

 * *Files identical despite different names*

### Comparing `modelscan-0.7.1/modelscan/middlewares/format_via_extension.py` & `modelscan-0.7.2/modelscan/middlewares/format_via_extension.py`

 * *Files identical despite different names*

### Comparing `modelscan-0.7.1/modelscan/middlewares/middleware.py` & `modelscan-0.7.2/modelscan/middlewares/middleware.py`

 * *Files identical despite different names*

### Comparing `modelscan-0.7.1/modelscan/model.py` & `modelscan-0.7.2/modelscan/model.py`

 * *Files identical despite different names*

### Comparing `modelscan-0.7.1/modelscan/modelscan.py` & `modelscan-0.7.2/modelscan/modelscan.py`

 * *Files 8% similar despite different names*

```diff
@@ -223,15 +223,15 @@
                 )
 
         return scanned
 
     def _generate_results(self) -> Dict[str, Any]:
         report: Dict[str, Any] = {}
 
-        absolute_path = Path(self._input_path).resolve()
+        absolute_path = Path(self._input_path)
         if Path(self._input_path).is_file():
             absolute_path = Path(absolute_path).parent
 
         issues_by_severity = self._issues.group_by_severity()
         total_issue_count = len(self._issues.all_issues)
 
         report["summary"] = {"total_issues_by_severity": {}}
@@ -250,57 +250,57 @@
         report["summary"]["timestamp"] = datetime.now().isoformat()
 
         report["summary"]["scanned"] = {"total_scanned": len(self._scanned)}
 
         if self._scanned:
             scanned_files = []
             for file_name in self._scanned:
-                resolved_file = Path(file_name).resolve()
                 scanned_files.append(
-                    str(resolved_file.relative_to(Path(absolute_path)))
+                    str(Path(file_name).relative_to(Path(absolute_path)))
                 )
 
             report["summary"]["scanned"]["scanned_files"] = scanned_files
 
         if self._issues.all_issues:
             report["issues"] = [
                 issue.details.output_json() for issue in self._issues.all_issues
             ]
 
             for issue in report["issues"]:
-                resolved_file = Path(issue["source"]).resolve()
-                issue["source"] = str(resolved_file.relative_to(Path(absolute_path)))
+                issue["source"] = str(
+                    Path(issue["source"]).relative_to(Path(absolute_path))
+                )
         else:
             report["issues"] = []
 
         all_errors = []
         if self._errors:
             for error in self._errors:
                 error_information = error.to_dict()
                 if "source" in error_information:
-                    resolved_file = Path(error_information["source"]).resolve()
                     error_information["source"] = str(
-                        resolved_file.relative_to(Path(absolute_path))
+                        Path(error_information["source"]).relative_to(
+                            Path(absolute_path)
+                        )
                     )
 
                 all_errors.append(error_information)
 
         report["errors"] = all_errors
 
         report["summary"]["skipped"] = {"total_skipped": len(self._skipped)}
 
         all_skipped_files = []
         if self._skipped:
             for skipped_file in self._skipped:
                 skipped_file_information = {}
                 skipped_file_information["category"] = str(skipped_file.category.name)
                 skipped_file_information["description"] = str(skipped_file.message)
-                resolved_file = Path(skipped_file.source).resolve()
                 skipped_file_information["source"] = str(
-                    resolved_file.relative_to(Path(absolute_path))
+                    Path(skipped_file.source).relative_to(Path(absolute_path))
                 )
                 all_skipped_files.append(skipped_file_information)
 
         report["summary"]["skipped"]["skipped_files"] = all_skipped_files
 
         return report
```

### Comparing `modelscan-0.7.1/modelscan/reports.py` & `modelscan-0.7.2/modelscan/reports.py`

 * *Files identical despite different names*

### Comparing `modelscan-0.7.1/modelscan/scanners/h5/scan.py` & `modelscan-0.7.2/modelscan/scanners/h5/scan.py`

 * *Files identical despite different names*

### Comparing `modelscan-0.7.1/modelscan/scanners/keras/scan.py` & `modelscan-0.7.2/modelscan/scanners/keras/scan.py`

 * *Files identical despite different names*

### Comparing `modelscan-0.7.1/modelscan/scanners/pickle/scan.py` & `modelscan-0.7.2/modelscan/scanners/pickle/scan.py`

 * *Files identical despite different names*

### Comparing `modelscan-0.7.1/modelscan/scanners/saved_model/scan.py` & `modelscan-0.7.2/modelscan/scanners/saved_model/scan.py`

 * *Files identical despite different names*

### Comparing `modelscan-0.7.1/modelscan/scanners/scan.py` & `modelscan-0.7.2/modelscan/scanners/scan.py`

 * *Files identical despite different names*

### Comparing `modelscan-0.7.1/modelscan/settings.py` & `modelscan-0.7.2/modelscan/settings.py`

 * *Files identical despite different names*

### Comparing `modelscan-0.7.1/modelscan/skip.py` & `modelscan-0.7.2/modelscan/skip.py`

 * *Files identical despite different names*

### Comparing `modelscan-0.7.1/modelscan/tools/LICENSE` & `modelscan-0.7.2/modelscan/tools/LICENSE`

 * *Files identical despite different names*

### Comparing `modelscan-0.7.1/modelscan/tools/cli_utils.py` & `modelscan-0.7.2/modelscan/tools/cli_utils.py`

 * *Files identical despite different names*

### Comparing `modelscan-0.7.1/modelscan/tools/picklescanner.py` & `modelscan-0.7.2/modelscan/tools/picklescanner.py`

 * *Files identical despite different names*

### Comparing `modelscan-0.7.1/modelscan/tools/utils.py` & `modelscan-0.7.2/modelscan/tools/utils.py`

 * *Files identical despite different names*

### Comparing `modelscan-0.7.1/pyproject.toml` & `modelscan-0.7.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "modelscan"
-version = "0.7.1"
+version = "0.7.2"
 description = "The modelscan package is a cli tool for detecting unsafe operations in model files across various model serialization formats."
 authors = ["ProtectAI <community@protectai.com>"]
 license = "Apache License 2.0"
 readme = "README.md"
 packages = [{ include = "modelscan" }]
 exclude = ["tests/*", "Makefile"]
```

### Comparing `modelscan-0.7.1/PKG-INFO` & `modelscan-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelscan
-Version: 0.7.1
+Version: 0.7.2
 Summary: The modelscan package is a cli tool for detecting unsafe operations in model files across various model serialization formats.
 License: Apache-2.0
 Author: ProtectAI
 Author-email: community@protectai.com
 Requires-Python: >=3.8,<3.13
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

