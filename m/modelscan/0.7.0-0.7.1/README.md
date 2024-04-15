# Comparing `tmp/modelscan-0.7.0.tar.gz` & `tmp/modelscan-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelscan-0.7.0.tar", max compression
+gzip compressed data, was "modelscan-0.7.1.tar", max compression
```

## Comparing `modelscan-0.7.0.tar` & `modelscan-0.7.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0    10754 2024-04-01 03:10:49.787867 modelscan-0.7.0/LICENSE
--rw-r--r--   0        0        0    12424 2024-04-01 03:10:49.791867 modelscan-0.7.0/README.md
--rw-r--r--   0        0        0      155 2024-04-01 03:10:49.803867 modelscan-0.7.0/modelscan/__init__.py
--rw-r--r--   0        0        0       22 2024-04-01 03:11:09.228044 modelscan-0.7.0/modelscan/_version.py
--rw-r--r--   0        0        0     6068 2024-04-01 03:10:49.803867 modelscan-0.7.0/modelscan/cli.py
--rw-r--r--   0        0        0     1033 2024-04-01 03:10:49.803867 modelscan-0.7.0/modelscan/error.py
--rw-r--r--   0        0        0     4697 2024-04-01 03:10:49.803867 modelscan-0.7.0/modelscan/issues.py
--rw-r--r--   0        0        0       84 2024-04-01 03:10:49.803867 modelscan-0.7.0/modelscan/middlewares/__init__.py
--rw-r--r--   0        0        0      585 2024-04-01 03:10:49.803867 modelscan-0.7.0/modelscan/middlewares/format_via_extension.py
--rw-r--r--   0        0        0     1757 2024-04-01 03:10:49.803867 modelscan-0.7.0/modelscan/middlewares/middleware.py
--rw-r--r--   0        0        0     1458 2024-04-01 03:10:49.803867 modelscan-0.7.0/modelscan/model.py
--rw-r--r--   0        0        0    14023 2024-04-01 03:10:49.803867 modelscan-0.7.0/modelscan/modelscan.py
--rw-r--r--   0        0        0     3032 2024-04-01 03:10:49.803867 modelscan-0.7.0/modelscan/reports.py
--rw-r--r--   0        0        0      377 2024-04-01 03:10:49.803867 modelscan-0.7.0/modelscan/scanners/__init__.py
--rw-r--r--   0        0        0        0 2024-04-01 03:10:49.803867 modelscan-0.7.0/modelscan/scanners/h5/__init__.py
--rw-r--r--   0        0        0     4702 2024-04-01 03:10:49.803867 modelscan-0.7.0/modelscan/scanners/h5/scan.py
--rw-r--r--   0        0        0        0 2024-04-01 03:10:49.803867 modelscan-0.7.0/modelscan/scanners/keras/__init__.py
--rw-r--r--   0        0        0     4686 2024-04-01 03:10:49.803867 modelscan-0.7.0/modelscan/scanners/keras/scan.py
--rw-r--r--   0        0        0        0 2024-04-01 03:10:49.803867 modelscan-0.7.0/modelscan/scanners/pickle/__init__.py
--rw-r--r--   0        0        0     1972 2024-04-01 03:10:49.803867 modelscan-0.7.0/modelscan/scanners/pickle/scan.py
--rw-r--r--   0        0        0        0 2024-04-01 03:10:49.803867 modelscan-0.7.0/modelscan/scanners/saved_model/__init__.py
--rw-r--r--   0        0        0     6923 2024-04-01 03:10:49.803867 modelscan-0.7.0/modelscan/scanners/saved_model/scan.py
--rw-r--r--   0        0        0     1667 2024-04-01 03:10:49.803867 modelscan-0.7.0/modelscan/scanners/scan.py
--rw-r--r--   0        0        0     3908 2024-04-01 03:10:49.803867 modelscan-0.7.0/modelscan/settings.py
--rw-r--r--   0        0        0     1016 2024-04-01 03:10:49.803867 modelscan-0.7.0/modelscan/skip.py
--rw-r--r--   0        0        0     2591 2024-04-01 03:10:49.803867 modelscan-0.7.0/modelscan/tools/LICENSE
--rw-r--r--   0        0        0     3435 2024-04-01 03:10:49.803867 modelscan-0.7.0/modelscan/tools/cli_utils.py
--rw-r--r--   0        0        0     9663 2024-04-01 03:10:49.803867 modelscan-0.7.0/modelscan/tools/picklescanner.py
--rw-r--r--   0        0        0     3028 2024-04-01 03:10:49.803867 modelscan-0.7.0/modelscan/tools/utils.py
--rw-r--r--   0        0        0     1629 2024-04-01 03:11:09.584047 modelscan-0.7.0/pyproject.toml
--rw-r--r--   0        0        0    13700 1970-01-01 00:00:00.000000 modelscan-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0    10754 2024-04-15 22:17:57.815445 modelscan-0.7.1/LICENSE
+-rw-r--r--   0        0        0    12564 2024-04-15 22:17:57.815445 modelscan-0.7.1/README.md
+-rw-r--r--   0        0        0      156 2024-04-15 22:17:57.831445 modelscan-0.7.1/modelscan/__init__.py
+-rw-r--r--   0        0        0       22 2024-04-15 22:18:12.847517 modelscan-0.7.1/modelscan/_version.py
+-rw-r--r--   0        0        0     6154 2024-04-15 22:17:57.831445 modelscan-0.7.1/modelscan/cli.py
+-rw-r--r--   0        0        0     2455 2024-04-15 22:17:57.831445 modelscan-0.7.1/modelscan/error.py
+-rw-r--r--   0        0        0     4697 2024-04-15 22:17:57.831445 modelscan-0.7.1/modelscan/issues.py
+-rw-r--r--   0        0        0       84 2024-04-15 22:17:57.831445 modelscan-0.7.1/modelscan/middlewares/__init__.py
+-rw-r--r--   0        0        0      585 2024-04-15 22:17:57.831445 modelscan-0.7.1/modelscan/middlewares/format_via_extension.py
+-rw-r--r--   0        0        0     1757 2024-04-15 22:17:57.831445 modelscan-0.7.1/modelscan/middlewares/middleware.py
+-rw-r--r--   0        0        0     1458 2024-04-15 22:17:57.831445 modelscan-0.7.1/modelscan/model.py
+-rw-r--r--   0        0        0    13276 2024-04-15 22:17:57.831445 modelscan-0.7.1/modelscan/modelscan.py
+-rw-r--r--   0        0        0     2993 2024-04-15 22:17:57.831445 modelscan-0.7.1/modelscan/reports.py
+-rw-r--r--   0        0        0      377 2024-04-15 22:17:57.831445 modelscan-0.7.1/modelscan/scanners/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-15 22:17:57.831445 modelscan-0.7.1/modelscan/scanners/h5/__init__.py
+-rw-r--r--   0        0        0     4611 2024-04-15 22:17:57.831445 modelscan-0.7.1/modelscan/scanners/h5/scan.py
+-rw-r--r--   0        0        0        0 2024-04-15 22:17:57.831445 modelscan-0.7.1/modelscan/scanners/keras/__init__.py
+-rw-r--r--   0        0        0     4451 2024-04-15 22:17:57.831445 modelscan-0.7.1/modelscan/scanners/keras/scan.py
+-rw-r--r--   0        0        0        0 2024-04-15 22:17:57.831445 modelscan-0.7.1/modelscan/scanners/pickle/__init__.py
+-rw-r--r--   0        0        0     1972 2024-04-15 22:17:57.831445 modelscan-0.7.1/modelscan/scanners/pickle/scan.py
+-rw-r--r--   0        0        0        0 2024-04-15 22:17:57.831445 modelscan-0.7.1/modelscan/scanners/saved_model/__init__.py
+-rw-r--r--   0        0        0     6853 2024-04-15 22:17:57.831445 modelscan-0.7.1/modelscan/scanners/saved_model/scan.py
+-rw-r--r--   0        0        0     1652 2024-04-15 22:17:57.831445 modelscan-0.7.1/modelscan/scanners/scan.py
+-rw-r--r--   0        0        0     4412 2024-04-15 22:17:57.831445 modelscan-0.7.1/modelscan/settings.py
+-rw-r--r--   0        0        0      892 2024-04-15 22:17:57.831445 modelscan-0.7.1/modelscan/skip.py
+-rw-r--r--   0        0        0     2591 2024-04-15 22:17:57.831445 modelscan-0.7.1/modelscan/tools/LICENSE
+-rw-r--r--   0        0        0     3435 2024-04-15 22:17:57.831445 modelscan-0.7.1/modelscan/tools/cli_utils.py
+-rw-r--r--   0        0        0     9598 2024-04-15 22:17:57.831445 modelscan-0.7.1/modelscan/tools/picklescanner.py
+-rw-r--r--   0        0        0     2989 2024-04-15 22:17:57.831445 modelscan-0.7.1/modelscan/tools/utils.py
+-rw-r--r--   0        0        0     1629 2024-04-15 22:18:13.203519 modelscan-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0    13840 1970-01-01 00:00:00.000000 modelscan-0.7.1/PKG-INFO
```

### Comparing `modelscan-0.7.0/LICENSE` & `modelscan-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `modelscan-0.7.0/README.md` & `modelscan-0.7.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 ```bash
 pip install modelscan
 ```
 
 With it installed, scan a model:
 
 ```bash
-modelscan -p /path/to/model_file.h5
+modelscan -p /path/to/model_file.pkl
 ```
 
 ## Why You Should Scan Models
 
 Models are often created from automated pipelines, others may come from a data scientist’s laptop. In either case the model needs to move from one machine to another before it is used. That process of saving a model to disk is called serialization.
 
 A **Model Serialization Attack** is where malicious code is added to the contents of a model during serialization(saving) before distribution — a modern version of the Trojan Horse. 
@@ -101,14 +101,19 @@
 To include it in your project's dependencies so it is available for everyone, add it to your `requirements.txt`
 or `pyproject.toml` like this:
 
 ```toml
 modelscan = ">=0.1.1"
 ```
 
+Scanners for Tensorflow or HD5 formatted models require installation with extras:
+```bash
+pip install 'modelscan[ tensorflow, h5py ]'
+```
+
 ### Using ModelScan via CLI
 
 ModelScan supports the following arguments via the CLI:
 
 | Usage                                                                            | Argument         | Explanation                                             | 
 |----------------------------------------------------------------------------------|------------------|---------------------------------------------------------|
 | ```modelscan -h ```                                                              | -h or --help     | View usage help                                         |
```

### Comparing `modelscan-0.7.0/modelscan/cli.py` & `modelscan-0.7.1/modelscan/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 import sys
 import os
 from pathlib import Path
-from typing import Optional, Dict, Any
+from typing import Optional
 from tomlkit import parse
 
 import click
 
 from modelscan.modelscan import ModelScan
 from modelscan._version import __version__
 from modelscan.settings import (
@@ -83,15 +83,15 @@
     "-o",
     "--output-file",
     type=click.Path(),
     default=None,
     help="Optional file name for output report",
 )
 @cli.command(
-    help="[Default] Scan a model file or diretory for ability to execute suspicious actions. "
+    help="[Default] Scan a model file or directory for ability to execute suspicious actions. "
 )  # type: ignore
 @click.pass_context
 def scan(
     ctx: click.Context,
     log: str,
     path: Optional[str],
     show_skipped: bool,
@@ -108,15 +108,15 @@
     settings_file_path = Path(
         settings_file if settings_file else f"{os.getcwd()}/modelscan-settings.toml"
     )
 
     settings = DEFAULT_SETTINGS
 
     if settings_file_path and settings_file_path.is_file():
-        with open(settings_file_path) as sf:
+        with open(settings_file_path, encoding="utf-8") as sf:
             settings = parse(sf.read()).unwrap()
             click.echo(f"Detected settings file. Using {settings_file_path}. \n")
     else:
         click.echo(
             f"No settings file detected at {settings_file_path}. Using defaults. \n"
         )
 
@@ -128,15 +128,15 @@
             raise FileNotFoundError(f"Path {path} does not exist")
         else:
             modelscan.scan(path)
     else:
         raise click.UsageError("Command line must include a path")
 
     # Report scan results
-    if reporting_format is not "custom":
+    if reporting_format != "custom":
         modelscan._settings["reporting"]["module"] = DEFAULT_REPORTING_MODULES[
             reporting_format
         ]
 
     modelscan._settings["reporting"]["settings"]["show_skipped"] = show_skipped
     modelscan._settings["reporting"]["settings"]["output_file"] = output_file
 
@@ -170,24 +170,25 @@
     working_dir = os.getcwd()
     settings_path = os.path.join(working_dir, "modelscan-settings.toml")
 
     if location:
         settings_path = location
 
     try:
-        open(settings_path)
+        open(settings_path, encoding="utf-8")
         if force:
-            with open(settings_path, "w") as settings_file:
+            with open(settings_path, mode="w", encoding="utf-8") as settings_file:
                 settings_file.write(SettingsUtils.get_default_settings_as_toml())
         else:
             logger.warning(
-                f"{settings_path} file already exists. Please use `--force` flag if you intend to overwrite it."
+                "%s file already exists. Please use `--force` flag if you intend to overwrite it.",
+                settings_path,
             )
     except FileNotFoundError:
-        with open(settings_path, "w") as settings_file:
+        with open(settings_path, mode="w", encoding="utf-8") as settings_file:
             settings_file.write(SettingsUtils.get_default_settings_as_toml())
 
 
 def main() -> None:
     try:
         result = cli.main(standalone_mode=False)
```

### Comparing `modelscan-0.7.0/modelscan/issues.py` & `modelscan-0.7.1/modelscan/issues.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
         )
 
     def print(self) -> None:
         issue_description = self.code.name
         if self.code == IssueCode.UNSAFE_OPERATOR:
             issue_description = "Unsafe operator"
         else:
-            logger.error(f"No issue description for issue code ${self.code}")
+            logger.error("No issue description for issue code %s", self.code)
 
         print(f"\n{issue_description} found:")
         print(f"  - Severity: {self.severity.name}")
         for output_line in self.details.output_lines():
             print(f"  - {output_line}")
```

### Comparing `modelscan-0.7.0/modelscan/middlewares/format_via_extension.py` & `modelscan-0.7.1/modelscan/middlewares/format_via_extension.py`

 * *Files identical despite different names*

### Comparing `modelscan-0.7.0/modelscan/middlewares/middleware.py` & `modelscan-0.7.1/modelscan/middlewares/middleware.py`

 * *Files identical despite different names*

### Comparing `modelscan-0.7.0/modelscan/model.py` & `modelscan-0.7.1/modelscan/model.py`

 * *Files identical despite different names*

### Comparing `modelscan-0.7.0/modelscan/modelscan.py` & `modelscan-0.7.1/modelscan/modelscan.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,21 @@
 from modelscan.settings import DEFAULT_SETTINGS
 
 from pathlib import Path
 from typing import List, Union, Dict, Any, Optional, Generator
 from datetime import datetime
 import zipfile
 
-from modelscan.error import ModelScanError, ErrorCategories
+from modelscan.error import (
+    ModelScanError,
+    PathError,
+    ErrorBase,
+    ModelScanScannerError,
+    NestedZipError,
+)
 from modelscan.skip import ModelScanSkipped, SkipCategories
 from modelscan.issues import Issues, IssueSeverity
 from modelscan.scanners.scan import ScanBase
 from modelscan._version import __version__
 from modelscan.tools.utils import _is_zipfile
 from modelscan.model import Model
 from modelscan.middlewares.middleware import MiddlewarePipeline, MiddlewareImportError
@@ -23,15 +29,15 @@
 class ModelScan:
     def __init__(
         self,
         settings: Dict[str, Any] = DEFAULT_SETTINGS,
     ) -> None:
         # Output
         self._issues = Issues()
-        self._errors: List[ModelScanError] = []
+        self._errors: List[ErrorBase] = []
         self._init_errors: List[ModelScanError] = []
         self._skipped: List[ModelScanSkipped] = []
         self._scanned: List[str] = []
         self._input_path: str = ""
 
         # Scanners
         self._scanners_to_run: List[ScanBase] = []
@@ -42,21 +48,15 @@
     def _load_middlewares(self) -> None:
         try:
             self._middleware_pipeline = MiddlewarePipeline.from_settings(
                 self._settings["middlewares"] or {}
             )
         except MiddlewareImportError as e:
             logger.exception(e)
-            self._init_errors.append(
-                ModelScanError(
-                    "MiddlewarePipeline",
-                    ErrorCategories.MODEL_SCAN,
-                    f"Error loading middlewares: {e}",
-                )
-            )
+            self._init_errors.append(ModelScanError(f"Error loading middlewares: {e}"))
 
     def _load_scanners(self) -> None:
         for scanner_path, scanner_settings in self._settings["scanners"].items():
             if (
                 "enabled" in scanner_settings.keys()
                 and self._settings["scanners"][scanner_path]["enabled"]
             ):
@@ -66,38 +66,29 @@
                         name=modulename, package=classname
                     )
 
                     scanner_class: ScanBase = getattr(imported_module, classname)
                     self._scanners_to_run.append(scanner_class)
 
                 except Exception as e:
-                    logger.error(f"Error importing scanner {scanner_path}")
+                    logger.error("Error importing scanner %s", scanner_path)
                     self._init_errors.append(
                         ModelScanError(
-                            scanner_path,
-                            ErrorCategories.MODEL_SCAN,
-                            f"Error importing scanner: {e}",
+                            f"Error importing scanner {scanner_path}: {e}",
                         )
                     )
 
     def _iterate_models(self, model_path: Path) -> Generator[Model, None, None]:
         if not model_path.exists():
-            logger.error(f"Path {model_path} does not exist")
-            self._errors.append(
-                ModelScanError(
-                    "ModelScan",
-                    ErrorCategories.PATH,
-                    "Path is not valid",
-                    str(model_path),
-                )
-            )
+            logger.error("Path %s does not exist", model_path)
+            self._errors.append(PathError("Path is not valid", model_path))
 
         files = [model_path]
         if model_path.is_dir():
-            logger.debug(f"Path {str(model_path)} is a directory")
+            logger.debug("Path %s is a directory", str(model_path))
             files = [f for f in model_path.rglob("*") if Path.is_file(f)]
 
         for file in files:
             with Model(file) as model:
                 yield model
 
                 if (
@@ -111,28 +102,26 @@
                     with zipfile.ZipFile(model.get_stream(), "r") as zip:
                         file_names = zip.namelist()
                         for file_name in file_names:
                             with zip.open(file_name, "r") as file_io:
                                 file_name = f"{model.get_source()}:{file_name}"
                                 if _is_zipfile(file_name, data=file_io):
                                     self._errors.append(
-                                        ModelScanError(
-                                            "ModelScan",
-                                            ErrorCategories.NESTED_ZIP,
+                                        NestedZipError(
                                             "ModelScan does not support nested zip files.",
-                                            file_name,
+                                            Path(file_name),
                                         )
                                     )
                                     continue
 
                                 yield Model(file_name, file_io)
                 except zipfile.BadZipFile as e:
                     logger.debug(
-                        f"Skipping zip file {str(model.get_source())}, due to error",
-                        e,
+                        "Skipping zip file %s, due to error",
+                        str(model.get_source()),
                         exc_info=True,
                     )
                     self._skipped.append(
                         ModelScanSkipped(
                             "ModelScan",
                             SkipCategories.BAD_ZIP,
                             f"Skipping zip file due to error: {e}",
@@ -185,30 +174,34 @@
         for scan_class in self._scanners_to_run:
             scanner = scan_class(self._settings)  # type: ignore[operator]
 
             try:
                 scan_results = scanner.scan(model)
             except Exception as e:
                 logger.error(
-                    f"Error encountered from scanner {scanner.full_name()} with path {str(model.get_source())}: {e}"
+                    "Error encountered from scanner %s with path %s: %s",
+                    scanner.full_name(),
+                    str(model.get_source()),
+                    e,
                 )
                 self._errors.append(
-                    ModelScanError(
+                    ModelScanScannerError(
                         scanner.full_name(),
-                        ErrorCategories.MODEL_SCAN,
-                        f"Error encountered from scanner {scanner.full_name()}: {e}",
-                        str(model.get_source()),
+                        str(e),
+                        model,
                     )
                 )
                 continue
 
             if scan_results is not None:
                 scanned = True
                 logger.info(
-                    f"Scanning {model.get_source()} using {scanner.full_name()} model scan"
+                    "Scanning %s using %s model scan",
+                    model.get_source(),
+                    scanner.full_name(),
                 )
                 if scan_results.errors:
                     self._errors.extend(scan_results.errors)
                 elif scan_results.issues:
                     self._scanned.append(str(model.get_source()))
                     self._issues.add_issues(scan_results.issues)
 
@@ -220,15 +213,15 @@
         if not scanned:
             all_skipped_files = [skipped.source for skipped in self._skipped]
             if str(model.get_source()) not in all_skipped_files:
                 self._skipped.append(
                     ModelScanSkipped(
                         "ModelScan",
                         SkipCategories.SCAN_NOT_SUPPORTED,
-                        f"Model Scan did not scan file",
+                        "Model Scan did not scan file",
                         str(model.get_source()),
                     )
                 )
 
         return scanned
 
     def _generate_results(self) -> Dict[str, Any]:
@@ -278,20 +271,17 @@
                 issue["source"] = str(resolved_file.relative_to(Path(absolute_path)))
         else:
             report["issues"] = []
 
         all_errors = []
         if self._errors:
             for error in self._errors:
-                error_information = {}
-                error_information["category"] = str(error.category.name)
-                if error.message:
-                    error_information["description"] = error.message
-                if error.source is not None:
-                    resolved_file = Path(error.source).resolve()
+                error_information = error.to_dict()
+                if "source" in error_information:
+                    resolved_file = Path(error_information["source"]).resolve()
                     error_information["source"] = str(
                         resolved_file.relative_to(Path(absolute_path))
                     )
 
                 all_errors.append(error_information)
 
         report["errors"] = all_errors
@@ -339,31 +329,27 @@
                 name=modulename, package=classname
             )
 
             report_class = getattr(imported_module, classname)
             scan_report = report_class.generate(scan=self, settings=report_settings)
 
         except Exception as e:
-            logger.error(f"Error generating report using {reporting_module}: {e}")
+            logger.error("Error generating report using %s: %s", reporting_module, e)
             self._errors.append(
-                ModelScanError(
-                    "ModelScan",
-                    ErrorCategories.MODEL_SCAN,
-                    f"Error generating report using {reporting_module}: {e}",
-                )
+                ModelScanError(f"Error generating report using {reporting_module}: {e}")
             )
 
         return scan_report
 
     @property
     def issues(self) -> Issues:
         return self._issues
 
     @property
-    def errors(self) -> List[ModelScanError]:
+    def errors(self) -> List[ErrorBase]:
         return self._errors
 
     @property
     def scanned(self) -> List[str]:
         return self._scanned
 
     @property
```

### Comparing `modelscan-0.7.0/modelscan/reports.py` & `modelscan-0.7.1/modelscan/reports.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 import logging
 import json
 from typing import Optional, Dict, Any
 
 from rich import print
 
 from modelscan.modelscan import ModelScan
-from modelscan.error import Error
-from modelscan.issues import Issues, IssueSeverity
+from modelscan.issues import IssueSeverity
 
 logger = logging.getLogger("modelscan")
 
 
 class Report(metaclass=abc.ABCMeta):
     """
     Abstract base class for different reporting modules.
@@ -29,29 +28,29 @@
         Generate report for the given codebase.
         Derived classes must provide implementation of this method.
 
         :param issues: Instance of Issues object
 
         :param errors: Any errors that occurred during the scan.
         """
-        raise NotImplemented
+        raise NotImplementedError
 
 
 class ConsoleReport(Report):
     @staticmethod
     def generate(
         scan: ModelScan,
         settings: Dict[str, Any] = {},
     ) -> None:
         issues_by_severity = scan.issues.group_by_severity()
         print("\n[blue]--- Summary ---")
         total_issue_count = len(scan.issues.all_issues)
         if total_issue_count > 0:
             print(f"\nTotal Issues: {total_issue_count}")
-            print(f"\nTotal Issues By Severity:\n")
+            print("\nTotal Issues By Severity:\n")
             for severity in IssueSeverity:
                 if severity.name in issues_by_severity:
                     print(
                         f"    - {severity.name}: {len(issues_by_severity[severity.name])}"
                     )
                 else:
                     print(f"    - {severity.name}: [green]0")
@@ -72,15 +71,15 @@
 
         if len(scan.skipped) > 0:
             print("\n[blue]--- Skipped --- ")
             print(
                 f"\nTotal skipped: {len(scan.skipped)} - run with --show-skipped to see the full list."
             )
             if settings["show_skipped"]:
-                print(f"\nSkipped files list:\n")
+                print("\nSkipped files list:\n")
                 for file_name in scan.skipped:
                     print(str(file_name))
 
 
 class JSONReport(Report):
     @staticmethod
     def generate(
```

### Comparing `modelscan-0.7.0/modelscan/scanners/h5/scan.py` & `modelscan-0.7.1/modelscan/scanners/h5/scan.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,18 @@
 try:
     import h5py
 
     h5py_installed = True
 except ImportError:
     h5py_installed = False
 
-from modelscan.error import ModelScanError, ErrorCategories
+from modelscan.error import (
+    DependencyError,
+    JsonDecodeError,
+)
 from modelscan.skip import ModelScanSkipped, SkipCategories
 from modelscan.scanners.scan import ScanResults
 from modelscan.scanners.saved_model.scan import SavedModelLambdaDetectScan
 from modelscan.model import Model
 
 logger = logging.getLogger("modelscan")
 
@@ -28,18 +31,18 @@
             return None
 
         dep_error = self.handle_binary_dependencies()
         if dep_error:
             return ScanResults(
                 [],
                 [
-                    ModelScanError(
+                    DependencyError(
                         self.name(),
-                        ErrorCategories.DEPENDENCY,
                         f"To use {self.full_name()}, please install modelscan with h5py extras. `pip install 'modelscan[ h5py ]'` if you are using pip.",
+                        model,
                     )
                 ],
                 [],
             )
 
         results = self._scan_keras_h5_file(model)
         if results:
@@ -54,19 +57,18 @@
             if operators_in_model is None:
                 return None
 
             if "JSONDecodeError" in operators_in_model:
                 return ScanResults(
                     [],
                     [
-                        ModelScanError(
+                        JsonDecodeError(
                             self.name(),
-                            ErrorCategories.JSON_DECODE,
-                            f"Not a valid JSON data",
-                            str(model.get_source()),
+                            "Not a valid JSON data",
+                            model,
                         )
                     ],
                     [],
                 )
             return H5LambdaDetectScan._check_for_unsafe_tf_keras_operator(
                 module_name=machine_learning_library_name,
                 raw_operator=operators_in_model,
@@ -79,15 +81,15 @@
             return ScanResults(
                 [],
                 [],
                 [
                     ModelScanSkipped(
                         self.name(),
                         SkipCategories.MODEL_CONFIG,
-                        f"Model Config not found",
+                        "Model Config not found",
                         str(model.get_source()),
                     )
                 ],
             )
 
     def _check_model_config(self, model: Model) -> bool:
         with h5py.File(model.get_stream()) as model_hdf5:
@@ -98,15 +100,15 @@
                 return False
 
     def _get_keras_h5_operator_names(self, model: Model) -> Optional[List[Any]]:
         # Todo: source isn't guaranteed to be a file
 
         with h5py.File(model.get_stream()) as model_hdf5:
             try:
-                if not "model_config" in model_hdf5.attrs.keys():
+                if "model_config" not in model_hdf5.attrs.keys():
                     return None
 
                 model_config = json.loads(model_hdf5.attrs.get("model_config", {}))
                 layers = model_config.get("config", {}).get("layers", {})
                 lambda_layers = []
                 for layer in layers:
                     if layer.get("class_name", {}) == "Lambda":
@@ -124,15 +126,15 @@
 
         return []
 
     def handle_binary_dependencies(
         self, settings: Optional[Dict[str, Any]] = None
     ) -> Optional[str]:
         if not h5py_installed:
-            return ErrorCategories.DEPENDENCY.name
+            return DependencyError.name()
         return None
 
     @staticmethod
     def name() -> str:
         return "hdf5"
 
     @staticmethod
```

### Comparing `modelscan-0.7.0/modelscan/scanners/keras/scan.py` & `modelscan-0.7.1/modelscan/scanners/keras/scan.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import json
 import zipfile
 import logging
-from pathlib import Path
-from typing import IO, List, Union, Optional
+from typing import List, Optional
 
 
-from modelscan.error import ModelScanError, ErrorCategories
+from modelscan.error import DependencyError, ModelScanScannerError, JsonDecodeError
 from modelscan.skip import ModelScanSkipped, SkipCategories
 from modelscan.scanners.scan import ScanResults
 from modelscan.scanners.saved_model.scan import SavedModelLambdaDetectScan
 from modelscan.model import Model
 
 
 logger = logging.getLogger("modelscan")
@@ -21,18 +20,18 @@
             return None
 
         dep_error = self.handle_binary_dependencies()
         if dep_error:
             return ScanResults(
                 [],
                 [
-                    ModelScanError(
+                    DependencyError(
                         self.name(),
-                        ErrorCategories.DEPENDENCY,
                         f"To use {self.full_name()}, please install modelscan with tensorflow extras. `pip install 'modelscan[ tensorflow ]'` if you are using pip.",
+                        model,
                     )
                 ],
                 [],
             )
 
         try:
             with zipfile.ZipFile(model.get_stream(), "r") as zip:
@@ -60,19 +59,18 @@
                 ],
             )
 
         # Added return to pass the failing mypy test: Missing return statement
         return ScanResults(
             [],
             [
-                ModelScanError(
+                ModelScanScannerError(
                     self.name(),
-                    ErrorCategories.MODEL_SCAN,  # Giving a generic error category as this return is added to pass mypy
-                    f"Unable to scan .keras file",  # Not sure if this is a representative message for ModelScanError
-                    str(model.get_source()),
+                    "Unable to scan .keras file",  # Not sure if this is a representative message for ModelScanError
+                    model,
                 )
             ],
             [],
         )
 
     def _scan_keras_config_file(self, model: Model) -> ScanResults:
         machine_learning_library_name = "Keras"
@@ -85,19 +83,18 @@
             logger.error(
                 f"Not a valid JSON data from source: {model.get_source()}, error: {e}"
             )
 
             return ScanResults(
                 [],
                 [
-                    ModelScanError(
+                    JsonDecodeError(
                         self.name(),
-                        ErrorCategories.JSON_DECODE,
-                        f"Not a valid JSON data",
-                        str(model.get_source()),
+                        "Not a valid JSON data",
+                        model,
                     )
                 ],
                 [],
             )
 
         if operators_in_model:
             return KerasLambdaDetectScan._check_for_unsafe_tf_keras_operator(
```

### Comparing `modelscan-0.7.0/modelscan/scanners/pickle/scan.py` & `modelscan-0.7.1/modelscan/scanners/pickle/scan.py`

 * *Files identical despite different names*

### Comparing `modelscan-0.7.0/modelscan/scanners/saved_model/scan.py` & `modelscan-0.7.1/modelscan/scanners/saved_model/scan.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 # scan pb files for both tensorflow and keras
 
 import json
 import logging
-from pathlib import Path
 
-from typing import IO, List, Set, Union, Optional, Dict, Any
+from typing import List, Set, Optional, Dict, Any
 
 try:
     import tensorflow
     from tensorflow.core.protobuf.saved_model_pb2 import SavedModel
     from tensorflow.python.keras.protobuf.saved_metadata_pb2 import SavedMetadata
 
     tensorflow_installed = True
 except ImportError:
     tensorflow_installed = False
 
 
-from modelscan.error import ModelScanError, ErrorCategories
+from modelscan.error import (
+    DependencyError,
+    JsonDecodeError,
+)
 from modelscan.issues import Issue, IssueCode, IssueSeverity, OperatorIssueDetails
 from modelscan.scanners.scan import ScanBase, ScanResults
 from modelscan.model import Model
 
 logger = logging.getLogger("modelscan")
 
 
@@ -33,18 +35,18 @@
             return None
 
         dep_error = self.handle_binary_dependencies()
         if dep_error:
             return ScanResults(
                 [],
                 [
-                    ModelScanError(
+                    DependencyError(
                         self.name(),
-                        ErrorCategories.DEPENDENCY,
                         f"To use {self.full_name()}, please install modelscan with tensorflow extras. `pip install 'modelscan[ tensorflow ]'` if you are using pip.",
+                        model,
                     )
                 ],
                 [],
             )
 
         results = self._scan(model)
 
@@ -58,15 +60,17 @@
     def _check_for_unsafe_tf_keras_operator(
         module_name: str,
         raw_operator: List[str],
         model: Model,
         unsafe_operators: Dict[str, Any],
     ) -> ScanResults:
         issues: List[Issue] = []
-        all_operators = tensorflow.raw_ops.__dict__.keys()
+        all_operators = (
+            tensorflow.raw_ops.__dict__.keys() if tensorflow_installed else []
+        )
         all_safe_operators = [
             operator for operator in list(all_operators) if operator[0] != "_"
         ]
 
         for op in raw_operator:
             if op in unsafe_operators:
                 severity = IssueSeverity[unsafe_operators[op]]
@@ -89,15 +93,15 @@
             )
         return ScanResults(issues, [], [])
 
     def handle_binary_dependencies(
         self, settings: Optional[Dict[str, Any]] = None
     ) -> Optional[str]:
         if not tensorflow_installed:
-            return ErrorCategories.DEPENDENCY.name
+            return DependencyError.name()
         return None
 
     @staticmethod
     def name() -> str:
         return "saved_model"
 
     @staticmethod
@@ -114,19 +118,18 @@
         machine_learning_library_name = "Keras"
         operators_in_model = self._get_keras_pb_operator_names(model)
         if operators_in_model:
             if "JSONDecodeError" in operators_in_model:
                 return ScanResults(
                     [],
                     [
-                        ModelScanError(
+                        JsonDecodeError(
                             self.name(),
-                            ErrorCategories.JSON_DECODE,
-                            f"Not a valid JSON data",
-                            str(model.get_source()),
+                            "Not a valid JSON data",
+                            model,
                         )
                     ],
                     [],
                 )
 
         return SavedModelScan._check_for_unsafe_tf_keras_operator(
             machine_learning_library_name,
```

### Comparing `modelscan-0.7.0/modelscan/scanners/scan.py` & `modelscan-0.7.1/modelscan/scanners/scan.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import abc
 from typing import List, Optional, Any, Dict
 
-from modelscan.error import ModelScanError
+from modelscan.error import ErrorBase
 from modelscan.skip import ModelScanSkipped
 from modelscan.issues import Issue
 from modelscan.model import Model
 
 
 class ScanResults:
     issues: List[Issue]
-    errors: List[ModelScanError]
+    errors: List[ErrorBase]
     skipped: List[ModelScanSkipped]
 
     def __init__(
         self,
         issues: List[Issue],
-        errors: List[ModelScanError],
+        errors: List[ErrorBase],
         skipped: List[ModelScanSkipped],
     ) -> None:
         self.issues = issues
         self.errors = errors
         self.skipped = skipped
```

### Comparing `modelscan-0.7.0/modelscan/settings.py` & `modelscan-0.7.1/modelscan/settings.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,39 +11,53 @@
 
 DEFAULT_SETTINGS = {
     "modelscan_version": __version__,
     "supported_zip_extensions": [".zip", ".npz"],
     "scanners": {
         "modelscan.scanners.H5LambdaDetectScan": {
             "enabled": True,
+            "supported_extensions": [".h5"],
         },
         "modelscan.scanners.KerasLambdaDetectScan": {
             "enabled": True,
+            "supported_extensions": [".keras"],
         },
         "modelscan.scanners.SavedModelLambdaDetectScan": {
             "enabled": True,
+            "supported_extensions": [".pb"],
             "unsafe_keras_operators": {
                 "Lambda": "MEDIUM",
             },
         },
         "modelscan.scanners.SavedModelTensorflowOpScan": {
             "enabled": True,
+            "supported_extensions": [".pb"],
             "unsafe_tf_operators": {
                 "ReadFile": "HIGH",
                 "WriteFile": "HIGH",
             },
         },
         "modelscan.scanners.NumpyUnsafeOpScan": {
             "enabled": True,
+            "supported_extensions": [".npy"],
         },
         "modelscan.scanners.PickleUnsafeOpScan": {
             "enabled": True,
+            "supported_extensions": [
+                ".pkl",
+                ".pickle",
+                ".joblib",
+                ".dill",
+                ".dat",
+                ".data",
+            ],
         },
         "modelscan.scanners.PyTorchUnsafeOpScan": {
             "enabled": True,
+            "supported_extensions": [".bin", ".pt", ".pth", ".ckpt"],
         },
     },
     "middlewares": {
         "modelscan.middlewares.FormatViaExtensionMiddleware": {
             "formats": {
                 "tf": [".pb"],
                 "tf_saved_model": [".pb"],
```

### Comparing `modelscan-0.7.0/modelscan/skip.py` & `modelscan-0.7.1/modelscan/skip.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,10 @@
-import abc
 import logging
 from enum import Enum
-from pathlib import Path
-from typing import Any, List, Union, Dict, Optional
 
-from collections import defaultdict
 
 logger = logging.getLogger("modelscan")
 
 
 class SkipCategories(Enum):
     SCAN_NOT_SUPPORTED = 1
     BAD_ZIP = 2
```

### Comparing `modelscan-0.7.0/modelscan/tools/LICENSE` & `modelscan-0.7.1/modelscan/tools/LICENSE`

 * *Files identical despite different names*

### Comparing `modelscan-0.7.0/modelscan/tools/cli_utils.py` & `modelscan-0.7.1/modelscan/tools/cli_utils.py`

 * *Files identical despite different names*

### Comparing `modelscan-0.7.0/modelscan/tools/picklescanner.py` & `modelscan-0.7.1/modelscan/tools/picklescanner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 import pickletools  # nosec
 from tarfile import TarError
 from typing import IO, Any, Dict, List, Set, Tuple, Union, Optional
 
 import numpy as np
 
-from modelscan.error import ModelScanError, ErrorCategories
+from modelscan.error import ModelScanError, PickleGenopsError
 from modelscan.skip import ModelScanSkipped, SkipCategories
 from modelscan.issues import Issue, IssueCode, IssueSeverity, OperatorIssueDetails
 from modelscan.scanners.scan import ScanResults
 from modelscan.model import Model
 
 logger = logging.getLogger("modelscan")
 
@@ -135,19 +135,18 @@
                 e.globals,
                 model,
                 settings,
             )
         return ScanResults(
             issues,
             [
-                ModelScanError(
+                PickleGenopsError(
                     scan_name,
-                    ErrorCategories.PICKLE_GENOPS,
                     f"Parsing error: {e}",
-                    str(model.get_source()),
+                    model,
                 )
             ],
             [],
         )
     logger.debug("Global imports in %s: %s", model, raw_globals, settings)
     return _build_scan_result_from_raw_globals(raw_globals, model, settings)
 
@@ -256,14 +255,14 @@
         return ScanResults(
             [],
             [],
             [
                 ModelScanSkipped(
                     scan_name,
                     SkipCategories.MAGIC_NUMBER,
-                    f"Invalid magic number",
+                    "Invalid magic number",
                     str(model.get_source()),
                 )
             ],
         )
 
     return scan_pickle_bytes(model, settings, scan_name, multiple_pickles=False)
```

### Comparing `modelscan-0.7.0/modelscan/tools/utils.py` & `modelscan-0.7.1/modelscan/tools/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-import http.client
 import io
-import urllib.parse
 from pathlib import Path
 from pickletools import genops  # nosec
 from typing import IO, Optional, Union
 
 
 class InvalidMagicError(Exception):
     def __init__(self, provided_magic: Optional[int], magic: int, file: str):
```

### Comparing `modelscan-0.7.0/pyproject.toml` & `modelscan-0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "modelscan"
-version = "0.7.0"
+version = "0.7.1"
 description = "The modelscan package is a cli tool for detecting unsafe operations in model files across various model serialization formats."
 authors = ["ProtectAI <community@protectai.com>"]
 license = "Apache License 2.0"
 readme = "README.md"
 packages = [{ include = "modelscan" }]
 exclude = ["tests/*", "Makefile"]
 
@@ -26,15 +26,15 @@
 
 [tool.poetry.extras]
 tensorflow = ["tensorflow", "tensorflow-macos"]
 h5py = ["h5py"]
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.4.0"
-bandit = { version = "1.7.5", extras = ["toml"] }
+bandit = { version = "1.7.8", extras = ["toml"] }
 mypy = "^1.4.1"
 requests = "^2.31.0"
 aiohttp = "^3.8.5"
 dill = "^0.3.7"
 types-requests = ">1.26"
 torch = "^2.1.2"
```

### Comparing `modelscan-0.7.0/PKG-INFO` & `modelscan-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelscan
-Version: 0.7.0
+Version: 0.7.1
 Summary: The modelscan package is a cli tool for detecting unsafe operations in model files across various model serialization formats.
 License: Apache-2.0
 Author: ProtectAI
 Author-email: community@protectai.com
 Requires-Python: >=3.8,<3.13
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -54,15 +54,15 @@
 ```bash
 pip install modelscan
 ```
 
 With it installed, scan a model:
 
 ```bash
-modelscan -p /path/to/model_file.h5
+modelscan -p /path/to/model_file.pkl
 ```
 
 ## Why You Should Scan Models
 
 Models are often created from automated pipelines, others may come from a data scientist’s laptop. In either case the model needs to move from one machine to another before it is used. That process of saving a model to disk is called serialization.
 
 A **Model Serialization Attack** is where malicious code is added to the contents of a model during serialization(saving) before distribution — a modern version of the Trojan Horse. 
@@ -128,14 +128,19 @@
 To include it in your project's dependencies so it is available for everyone, add it to your `requirements.txt`
 or `pyproject.toml` like this:
 
 ```toml
 modelscan = ">=0.1.1"
 ```
 
+Scanners for Tensorflow or HD5 formatted models require installation with extras:
+```bash
+pip install 'modelscan[ tensorflow, h5py ]'
+```
+
 ### Using ModelScan via CLI
 
 ModelScan supports the following arguments via the CLI:
 
 | Usage                                                                            | Argument         | Explanation                                             | 
 |----------------------------------------------------------------------------------|------------------|---------------------------------------------------------|
 | ```modelscan -h ```                                                              | -h or --help     | View usage help                                         |
```

