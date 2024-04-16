# Comparing `tmp/eencijfer-2024.2.4.tar.gz` & `tmp/eencijfer-2024.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eencijfer-2024.2.4.tar", max compression
+gzip compressed data, was "eencijfer-2024.3.0.tar", max compression
```

## Comparing `eencijfer-2024.2.4.tar` & `eencijfer-2024.3.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0     1069 2024-04-12 15:25:52.716827 eencijfer-2024.2.4/LICENSE
--rw-r--r--   0        0        0      925 2024-04-12 15:25:52.716827 eencijfer-2024.2.4/README.md
--rw-r--r--   0        0        0     1807 2024-04-12 15:25:52.716827 eencijfer-2024.2.4/eencijfer/__init__.py
--rw-r--r--   0        0        0       43 2024-04-12 15:25:52.716827 eencijfer-2024.2.4/eencijfer/assets/__init__.py
--rw-r--r--   0        0        0    11868 2024-04-12 15:25:52.716827 eencijfer-2024.2.4/eencijfer/assets/cohorten.py
--rw-r--r--   0        0        0     1891 2024-04-12 15:25:52.716827 eencijfer-2024.2.4/eencijfer/assets/eencijfer.py
--rw-r--r--   0        0        0     3174 2024-04-12 15:25:52.716827 eencijfer-2024.2.4/eencijfer/assets/eindexamencijfers.py
--rw-r--r--   0        0        0        0 2024-04-12 15:25:52.716827 eencijfer-2024.2.4/eencijfer/assets/transformations/__init__py
--rw-r--r--   0        0        0     2159 2024-04-12 15:25:52.716827 eencijfer-2024.2.4/eencijfer/assets/transformations/datasets/21RI/croho_naam_opleiding_faculteit.csv
--rw-r--r--   0        0        0     1639 2024-04-12 15:25:52.716827 eencijfer-2024.2.4/eencijfer/assets/transformations/diploma.py
--rw-r--r--   0        0        0       53 2024-04-12 15:25:52.716827 eencijfer-2024.2.4/eencijfer/assets/transformations/local_data.py
--rw-r--r--   0        0        0     7712 2024-04-12 15:25:52.716827 eencijfer-2024.2.4/eencijfer/assets/transformations/opleiding.py
--rw-r--r--   0        0        0     1455 2024-04-12 15:25:52.716827 eencijfer-2024.2.4/eencijfer/assets/transformations/postcodes.py
--rw-r--r--   0        0        0     1756 2024-04-12 15:25:52.716827 eencijfer-2024.2.4/eencijfer/assets/transformations/prestatieafspraken.py
--rw-r--r--   0        0        0     7437 2024-04-12 15:25:52.716827 eencijfer-2024.2.4/eencijfer/assets/transformations/vooropleiding.py
--rw-r--r--   0        0        0     4196 2024-04-12 15:25:52.716827 eencijfer-2024.2.4/eencijfer/cli.py
--rw-r--r--   0        0        0       61 2024-04-12 15:25:52.716827 eencijfer-2024.2.4/eencijfer/convert/__init__.py
--rw-r--r--   0        0        0     2712 2024-04-12 15:25:52.716827 eencijfer-2024.2.4/eencijfer/convert/column_converters.py
--rw-r--r--   0        0        0    10853 2024-04-12 15:25:52.716827 eencijfer-2024.2.4/eencijfer/convert/eencijfer.py
--rw-r--r--   0        0        0      710 2024-04-12 15:25:52.716827 eencijfer-2024.2.4/eencijfer/convert/import_definitions/Croho.csv
--rw-r--r--   0        0        0      716 2024-04-12 15:25:52.716827 eencijfer-2024.2.4/eencijfer/convert/import_definitions/Croho_vest.csv
--rw-r--r--   0        0        0      136 2024-04-12 15:25:52.716827 eencijfer-2024.2.4/eencijfer/convert/import_definitions/Dec_actuele_instelling.csv
--rw-r--r--   0        0        0      349 2024-04-12 15:25:52.716827 eencijfer-2024.2.4/eencijfer/convert/import_definitions/Dec_brinnummer.csv
--rw-r--r--   0        0        0      527 2024-04-12 15:25:52.716827 eencijfer-2024.2.4/eencijfer/convert/import_definitions/Dec_brinvestigingsnummer.csv
--rw-r--r--   0        0        0      128 2024-04-12 15:25:52.716827 eencijfer-2024.2.4/eencijfer/convert/import_definitions/Dec_ho-inst.csv
--rw-r--r--   0        0        0      284 2024-04-12 15:25:52.716827 eencijfer-2024.2.4/eencijfer/convert/import_definitions/Dec_ho_ISCED.csv
--rw-r--r--   0        0        0      126 2024-04-12 15:25:52.716827 eencijfer-2024.2.4/eencijfer/convert/import_definitions/Dec_isat.csv
--rw-r--r--   0        0        0      213 2024-04-12 15:25:52.716827 eencijfer-2024.2.4/eencijfer/convert/import_definitions/Dec_land_naar_herkomstindikking.csv
--rw-r--r--   0        0        0      264 2024-04-12 15:25:52.716827 eencijfer-2024.2.4/eencijfer/convert/import_definitions/Dec_landcode.csv
--rw-r--r--   0        0        0      282 2024-04-12 15:25:52.716827 eencijfer-2024.2.4/eencijfer/convert/import_definitions/Dec_nationaliteitscode.csv
--rw-r--r--   0        0        0      191 2024-04-12 15:25:52.716827 eencijfer-2024.2.4/eencijfer/convert/import_definitions/Dec_postcodecijfers_2023.csv
--rw-r--r--   0        0        0      191 2024-04-12 15:25:52.716827 eencijfer-2024.2.4/eencijfer/convert/import_definitions/Dec_postcodecijfers_2024.csv
--rw-r--r--   0        0        0      249 2024-04-12 15:25:52.716827 eencijfer-2024.2.4/eencijfer/convert/import_definitions/Dec_vakcode.csv
--rw-r--r--   0        0        0      237 2024-04-12 15:25:52.716827 eencijfer-2024.2.4/eencijfer/convert/import_definitions/Dec_vestnr_ho.csv
--rw-r--r--   0        0        0      237 2024-04-12 15:25:52.716827 eencijfer-2024.2.4/eencijfer/convert/import_definitions/Dec_vestnr_ho_compleet.csv
--rw-r--r--   0        0        0      213 2024-04-12 15:25:52.716827 eencijfer-2024.2.4/eencijfer/convert/import_definitions/Dec_vooropl.csv
--rw-r--r--   0        0        0      140 2024-04-12 15:25:52.716827 eencijfer-2024.2.4/eencijfer/convert/import_definitions/Dec_vopl.csv
--rw-r--r--   0        0        0     6232 2024-04-12 15:25:52.720827 eencijfer-2024.2.4/eencijfer/convert/import_definitions/EV____24.csv
--rw-r--r--   0        0        0     1058 2024-04-12 15:25:52.720827 eencijfer-2024.2.4/eencijfer/convert/import_definitions/VAKHAVW_____.csv
--rw-r--r--   0        0        0     6559 2024-04-12 15:25:52.720827 eencijfer-2024.2.4/eencijfer/convert/pii.py
--rw-r--r--   0        0        0       28 2024-04-12 15:25:52.720827 eencijfer-2024.2.4/eencijfer/io/__init__.py
--rw-r--r--   0        0        0     3528 2024-04-12 15:25:52.720827 eencijfer-2024.2.4/eencijfer/io/file.py
--rw-r--r--   0        0        0     2049 2024-04-12 15:25:52.720827 eencijfer-2024.2.4/eencijfer/settings.py
--rw-r--r--   0        0        0       33 2024-04-12 15:25:52.720827 eencijfer-2024.2.4/eencijfer/utils/__init__.py
--rw-r--r--   0        0        0     4054 2024-04-12 15:25:52.720827 eencijfer-2024.2.4/eencijfer/utils/detect_eencijfer_files.py
--rw-r--r--   0        0        0     2624 2024-04-12 15:25:52.720827 eencijfer-2024.2.4/eencijfer/utils/init.py
--rw-r--r--   0        0        0      991 2024-04-12 15:25:52.720827 eencijfer-2024.2.4/eencijfer/utils/local_data.py
--rw-r--r--   0        0        0     1944 2024-04-12 15:25:52.720827 eencijfer-2024.2.4/eencijfer/utils/qa.py
--rw-r--r--   0        0        0     2503 2024-04-12 15:25:52.720827 eencijfer-2024.2.4/pyproject.toml
--rw-r--r--   0        0        0       39 2024-04-12 15:25:52.720827 eencijfer-2024.2.4/tests/__init__.py
--rw-r--r--   0        0        0      450 2024-04-12 15:25:52.720827 eencijfer-2024.2.4/tests/test_cli.py
--rw-r--r--   0        0        0      541 2024-04-12 15:25:52.720827 eencijfer-2024.2.4/tests/test_eencijfer.py
--rw-r--r--   0        0        0     1832 1970-01-01 00:00:00.000000 eencijfer-2024.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-15 18:54:17.117254 eencijfer-2024.3.0/LICENSE
+-rw-r--r--   0        0        0      925 2024-04-15 18:54:17.117254 eencijfer-2024.3.0/README.md
+-rw-r--r--   0        0        0     1807 2024-04-15 18:54:17.117254 eencijfer-2024.3.0/eencijfer/__init__.py
+-rw-r--r--   0        0        0       43 2024-04-15 18:54:17.117254 eencijfer-2024.3.0/eencijfer/assets/__init__.py
+-rw-r--r--   0        0        0    11868 2024-04-15 18:54:17.117254 eencijfer-2024.3.0/eencijfer/assets/cohorten.py
+-rw-r--r--   0        0        0     1891 2024-04-15 18:54:17.117254 eencijfer-2024.3.0/eencijfer/assets/eencijfer.py
+-rw-r--r--   0        0        0     3174 2024-04-15 18:54:17.117254 eencijfer-2024.3.0/eencijfer/assets/eindexamencijfers.py
+-rw-r--r--   0        0        0        0 2024-04-15 18:54:17.117254 eencijfer-2024.3.0/eencijfer/assets/transformations/__init__py
+-rw-r--r--   0        0        0     2159 2024-04-15 18:54:17.117254 eencijfer-2024.3.0/eencijfer/assets/transformations/datasets/21RI/croho_naam_opleiding_faculteit.csv
+-rw-r--r--   0        0        0     1639 2024-04-15 18:54:17.117254 eencijfer-2024.3.0/eencijfer/assets/transformations/diploma.py
+-rw-r--r--   0        0        0       53 2024-04-15 18:54:17.117254 eencijfer-2024.3.0/eencijfer/assets/transformations/local_data.py
+-rw-r--r--   0        0        0     7712 2024-04-15 18:54:17.117254 eencijfer-2024.3.0/eencijfer/assets/transformations/opleiding.py
+-rw-r--r--   0        0        0     1455 2024-04-15 18:54:17.121254 eencijfer-2024.3.0/eencijfer/assets/transformations/postcodes.py
+-rw-r--r--   0        0        0     1756 2024-04-15 18:54:17.121254 eencijfer-2024.3.0/eencijfer/assets/transformations/prestatieafspraken.py
+-rw-r--r--   0        0        0     7437 2024-04-15 18:54:17.121254 eencijfer-2024.3.0/eencijfer/assets/transformations/vooropleiding.py
+-rw-r--r--   0        0        0     4432 2024-04-15 18:54:17.121254 eencijfer-2024.3.0/eencijfer/cli.py
+-rw-r--r--   0        0        0       61 2024-04-15 18:54:17.121254 eencijfer-2024.3.0/eencijfer/convert/__init__.py
+-rw-r--r--   0        0        0     2712 2024-04-15 18:54:17.121254 eencijfer-2024.3.0/eencijfer/convert/column_converters.py
+-rw-r--r--   0        0        0    10853 2024-04-15 18:54:17.121254 eencijfer-2024.3.0/eencijfer/convert/eencijfer.py
+-rw-r--r--   0        0        0      710 2024-04-15 18:54:17.121254 eencijfer-2024.3.0/eencijfer/convert/import_definitions/Croho.csv
+-rw-r--r--   0        0        0      716 2024-04-15 18:54:17.121254 eencijfer-2024.3.0/eencijfer/convert/import_definitions/Croho_vest.csv
+-rw-r--r--   0        0        0      136 2024-04-15 18:54:17.121254 eencijfer-2024.3.0/eencijfer/convert/import_definitions/Dec_actuele_instelling.csv
+-rw-r--r--   0        0        0      349 2024-04-15 18:54:17.121254 eencijfer-2024.3.0/eencijfer/convert/import_definitions/Dec_brinnummer.csv
+-rw-r--r--   0        0        0      527 2024-04-15 18:54:17.121254 eencijfer-2024.3.0/eencijfer/convert/import_definitions/Dec_brinvestigingsnummer.csv
+-rw-r--r--   0        0        0      128 2024-04-15 18:54:17.121254 eencijfer-2024.3.0/eencijfer/convert/import_definitions/Dec_ho-inst.csv
+-rw-r--r--   0        0        0      284 2024-04-15 18:54:17.121254 eencijfer-2024.3.0/eencijfer/convert/import_definitions/Dec_ho_ISCED.csv
+-rw-r--r--   0        0        0      126 2024-04-15 18:54:17.121254 eencijfer-2024.3.0/eencijfer/convert/import_definitions/Dec_isat.csv
+-rw-r--r--   0        0        0      213 2024-04-15 18:54:17.121254 eencijfer-2024.3.0/eencijfer/convert/import_definitions/Dec_land_naar_herkomstindikking.csv
+-rw-r--r--   0        0        0      264 2024-04-15 18:54:17.121254 eencijfer-2024.3.0/eencijfer/convert/import_definitions/Dec_landcode.csv
+-rw-r--r--   0        0        0      282 2024-04-15 18:54:17.121254 eencijfer-2024.3.0/eencijfer/convert/import_definitions/Dec_nationaliteitscode.csv
+-rw-r--r--   0        0        0      191 2024-04-15 18:54:17.121254 eencijfer-2024.3.0/eencijfer/convert/import_definitions/Dec_postcodecijfers_2023.csv
+-rw-r--r--   0        0        0      191 2024-04-15 18:54:17.121254 eencijfer-2024.3.0/eencijfer/convert/import_definitions/Dec_postcodecijfers_2024.csv
+-rw-r--r--   0        0        0      249 2024-04-15 18:54:17.121254 eencijfer-2024.3.0/eencijfer/convert/import_definitions/Dec_vakcode.csv
+-rw-r--r--   0        0        0      237 2024-04-15 18:54:17.121254 eencijfer-2024.3.0/eencijfer/convert/import_definitions/Dec_vestnr_ho.csv
+-rw-r--r--   0        0        0      237 2024-04-15 18:54:17.121254 eencijfer-2024.3.0/eencijfer/convert/import_definitions/Dec_vestnr_ho_compleet.csv
+-rw-r--r--   0        0        0      213 2024-04-15 18:54:17.121254 eencijfer-2024.3.0/eencijfer/convert/import_definitions/Dec_vooropl.csv
+-rw-r--r--   0        0        0      140 2024-04-15 18:54:17.121254 eencijfer-2024.3.0/eencijfer/convert/import_definitions/Dec_vopl.csv
+-rw-r--r--   0        0        0     6244 2024-04-15 18:54:17.121254 eencijfer-2024.3.0/eencijfer/convert/import_definitions/EV____24.csv
+-rw-r--r--   0        0        0     1058 2024-04-15 18:54:17.121254 eencijfer-2024.3.0/eencijfer/convert/import_definitions/VAKHAVW_____.csv
+-rw-r--r--   0        0        0     6543 2024-04-15 18:54:17.121254 eencijfer-2024.3.0/eencijfer/convert/pii.py
+-rw-r--r--   0        0        0       28 2024-04-15 18:54:17.121254 eencijfer-2024.3.0/eencijfer/io/__init__.py
+-rw-r--r--   0        0        0     3558 2024-04-15 18:54:17.121254 eencijfer-2024.3.0/eencijfer/io/file.py
+-rw-r--r--   0        0        0     2049 2024-04-15 18:54:17.121254 eencijfer-2024.3.0/eencijfer/settings.py
+-rw-r--r--   0        0        0       33 2024-04-15 18:54:17.121254 eencijfer-2024.3.0/eencijfer/utils/__init__.py
+-rw-r--r--   0        0        0     4054 2024-04-15 18:54:17.121254 eencijfer-2024.3.0/eencijfer/utils/detect_eencijfer_files.py
+-rw-r--r--   0        0        0     2624 2024-04-15 18:54:17.125254 eencijfer-2024.3.0/eencijfer/utils/init.py
+-rw-r--r--   0        0        0      991 2024-04-15 18:54:17.125254 eencijfer-2024.3.0/eencijfer/utils/local_data.py
+-rw-r--r--   0        0        0     1944 2024-04-15 18:54:17.125254 eencijfer-2024.3.0/eencijfer/utils/qa.py
+-rw-r--r--   0        0        0     2504 2024-04-15 18:54:17.125254 eencijfer-2024.3.0/pyproject.toml
+-rw-r--r--   0        0        0       39 2024-04-15 18:54:17.125254 eencijfer-2024.3.0/tests/__init__.py
+-rw-r--r--   0        0        0      450 2024-04-15 18:54:17.125254 eencijfer-2024.3.0/tests/test_cli.py
+-rw-r--r--   0        0        0      541 2024-04-15 18:54:17.125254 eencijfer-2024.3.0/tests/test_eencijfer.py
+-rw-r--r--   0        0        0     1832 1970-01-01 00:00:00.000000 eencijfer-2024.3.0/PKG-INFO
```

### Comparing `eencijfer-2024.2.4/LICENSE` & `eencijfer-2024.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.2.4/README.md` & `eencijfer-2024.3.0/README.md`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.2.4/eencijfer/__init__.py` & `eencijfer-2024.3.0/eencijfer/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Top-level package for eencijfer."""
 
 __author__ = """Bram Enning"""
 __email__ = 'bramenning@gmail.com'
-__version__ = '2024.2.4'
+__version__ = '2024.3.0'
 __app_name__ = 'eencijfer'
 
 import logging
 import shutil
 from importlib import import_module
 from pathlib import Path
```

### Comparing `eencijfer-2024.2.4/eencijfer/assets/cohorten.py` & `eencijfer-2024.3.0/eencijfer/assets/cohorten.py`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.2.4/eencijfer/assets/eencijfer.py` & `eencijfer-2024.3.0/eencijfer/assets/eencijfer.py`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.2.4/eencijfer/assets/eindexamencijfers.py` & `eencijfer-2024.3.0/eencijfer/assets/eindexamencijfers.py`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.2.4/eencijfer/assets/transformations/datasets/21RI/croho_naam_opleiding_faculteit.csv` & `eencijfer-2024.3.0/eencijfer/assets/transformations/datasets/21RI/croho_naam_opleiding_faculteit.csv`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.2.4/eencijfer/assets/transformations/diploma.py` & `eencijfer-2024.3.0/eencijfer/assets/transformations/diploma.py`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.2.4/eencijfer/assets/transformations/opleiding.py` & `eencijfer-2024.3.0/eencijfer/assets/transformations/opleiding.py`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.2.4/eencijfer/assets/transformations/postcodes.py` & `eencijfer-2024.3.0/eencijfer/assets/transformations/postcodes.py`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.2.4/eencijfer/assets/transformations/prestatieafspraken.py` & `eencijfer-2024.3.0/eencijfer/assets/transformations/prestatieafspraken.py`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.2.4/eencijfer/assets/transformations/vooropleiding.py` & `eencijfer-2024.3.0/eencijfer/assets/transformations/vooropleiding.py`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.2.4/eencijfer/cli.py` & `eencijfer-2024.3.0/eencijfer/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 """Console script for eencijfer."""
 
+import logging
+import shutil
 from pathlib import Path
 from typing import Optional
 
 import typer
 from typing_extensions import Annotated
 
 from eencijfer import APP_NAME, CONFIG_FILE, __version__
 from eencijfer.assets.cohorten import create_cohorten_met_indicatoren
 from eencijfer.assets.eencijfer import _create_eencijfer_df
 from eencijfer.assets.eindexamencijfers import _create_eindexamencijfer_df
 from eencijfer.convert.eencijfer import _convert_to_parquet
 from eencijfer.convert.pii import _replace_all_pgn_with_pseudo_id_remove_pii_local_id
-from eencijfer.io.file import ExportFormat, _convert_to_export_format_remove_parquet, _save_to_file
+from eencijfer.io.file import ExportFormat, _convert_to_export_format, _save_to_file
 from eencijfer.settings import config
 from eencijfer.utils.init import _create_default_config
 from eencijfer.utils.qa import compare_eencijfer_files_and_definitions
 
+logger = logging.getLogger(__name__)
+
 app = typer.Typer(name="eencijfer", help="ETL-tool for Dutch eencijfer", no_args_is_help=True)
 
 
 def _version_callback(value: bool) -> None:
     """Gives version nummber.
 
     Args:
@@ -70,30 +74,38 @@
     add_local_id: Annotated[bool, typer.Option("--add-local-id/--do-not-add-local-id", "-s/-S")] = False,
 ):
     """Convert eencijfer-files to desired exportformat, with or without PII."""
 
     source_dir = config.getpath('default', 'source_dir')
 
     result_dir = config.getpath('default', 'result_dir')
+
+    working_dir = result_dir / '.temp_dir'
+
     if not result_dir.is_dir():
         Path(result_dir).mkdir(parents=True, exist_ok=True)
 
+    if not working_dir.is_dir():
+        Path(working_dir).mkdir(parents=True, exist_ok=True)
+
     _convert_to_parquet(
         source_dir=source_dir,
-        result_dir=result_dir,
+        result_dir=working_dir,
         export_format=ExportFormat.parquet,
         use_column_converters=use_column_converters,
     )
 
     _replace_all_pgn_with_pseudo_id_remove_pii_local_id(
-        export_format=ExportFormat.parquet, remove_pii=remove_pii, add_local_id=add_local_id
+        eencijfer_dir=working_dir, remove_pii=remove_pii, add_local_id=add_local_id
     )
 
-    if export_format.value != 'parquet':
-        _convert_to_export_format_remove_parquet(result_dir=result_dir, export_format=export_format)
+    _convert_to_export_format(source_dir=working_dir, result_dir=result_dir, export_format=export_format)
+
+    logger.debug(f'Removing working dir {working_dir}')
+    shutil.rmtree(working_dir)
 
 
 @app.command()
 def qa():
     """Show overlap between eencijfer-files and definitions."""
     overlap = compare_eencijfer_files_and_definitions()
     typer.echo(overlap)
```

### Comparing `eencijfer-2024.2.4/eencijfer/convert/column_converters.py` & `eencijfer-2024.3.0/eencijfer/convert/column_converters.py`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.2.4/eencijfer/convert/eencijfer.py` & `eencijfer-2024.3.0/eencijfer/convert/eencijfer.py`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.2.4/eencijfer/convert/import_definitions/Croho.csv` & `eencijfer-2024.3.0/eencijfer/convert/import_definitions/Croho.csv`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.2.4/eencijfer/convert/import_definitions/Croho_vest.csv` & `eencijfer-2024.3.0/eencijfer/convert/import_definitions/Croho_vest.csv`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.2.4/eencijfer/convert/import_definitions/Dec_brinvestigingsnummer.csv` & `eencijfer-2024.3.0/eencijfer/convert/import_definitions/Dec_brinvestigingsnummer.csv`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.2.4/eencijfer/convert/import_definitions/EV____24.csv` & `eencijfer-2024.3.0/eencijfer/convert/import_definitions/EV____24.csv`

 * *Files 3% similar despite different names*

```diff
@@ -13,25 +13,25 @@
 MaandExamenresultaat,38,2,convert_to_int64
 BekostigingCode,40,1,convert_to_object
 EersteJaarAanDezeInstelling,41,4,convert_to_int64
 Inschrijvingsvorm,45,1,convert_to_object
 SoortHogerOnderwijs,46,3,convert_to_object
 OpleidingActueelEquivalent,49,5,convert_to_object
 OpleidingHistorischEquivalent,54,5,convert_to_object
-CrohoOnderdeelActueleOpleiding,59,1,convert_to_int64
-CrohoSubonderdeelActueleOpleiding,60,2,convert_to_int64
+CrohoOnderdeelActueleOpleiding,59,1,convert_to_object
+CrohoSubonderdeelActueleOpleiding,60,2,convert_to_object
 TypeHogerOnderwijsBinnenSoortHogerOnderwijs,62,2,convert_to_object
 OpleidingsfaseActueel,64,1,convert_to_object
 IndicatieActiefOpPeildatum,65,1,convert_to_int64
-SoortInschrijvingHogerOnderwijs,66,1,convert_to_int64
-SoortInschrijvingSoortHo,67,1,convert_to_int64
-SoortInschrijvingTypeHoBinnenSoortHo,68,1,convert_to_int64
-SoortInschrijvingOpleidingActueelEquivalent,69,1,convert_to_int64
-SoortInschrijvingActueleInstelling,70,1,convert_to_int64
-SoortInschrijvingActueleOpleidingInstelling,71,1,convert_to_int64
+SoortInschrijvingHogerOnderwijs,66,1,convert_to_object
+SoortInschrijvingSoortHo,67,1,convert_to_object
+SoortInschrijvingTypeHoBinnenSoortHo,68,1,convert_to_object
+SoortInschrijvingOpleidingActueelEquivalent,69,1,convert_to_object
+SoortInschrijvingActueleInstelling,70,1,convert_to_object
+SoortInschrijvingActueleOpleidingInstelling,71,1,convert_to_object
 VerblijfsjaarHogerOnderwijs,72,2,convert_to_int64
 VerblijfsjaarSoortHo,74,2,convert_to_int64
 VerblijfsjaarTypeHoBinnenSoortHo,76,2,convert_to_int64
 IndicatieEerstejaarsOplActueelEquivalent,78,1,convert_to_int64
 IndicatieEerstejaarsActueleInstelling,79,1,convert_to_int64
 IndicatieEerstejaarsActueleOplInstelling,80,1,convert_to_int64
 EersteJaarInHetHogerOnderwijs,81,4,convert_to_int64
@@ -71,18 +71,18 @@
 IndicatieEerstejrsActInstTypeHoBinnenSoortHo,198,1,convert_to_int64
 ActueleInstellingVoorBesturenfusies,199,4,convert_to_object
 SoortInschrijvingTypeHoBinnenHo,203,1,convert_to_int64
 VerblijfsjaarTypeHoBinnenHo,204,2,convert_to_int64
 PostcodecijfersStudentOp1Oktober,206,4,convert_to_int64
 PostcodecijfersVanDeHoogsteVooroplVoorHetHo,210,4,convert_to_int64
 GemEindcijferVoVanDeHoogsteVooroplVoorHetHo,214,3,convert_to_int64
-SoortInschrijvingContinuHogerOnderwijs,217,1,convert_to_int64
-SoortInschrijvingContinuSoortHo,218,1,convert_to_int64
-SoortInschrijvingContinuActueleInstelling,219,1,convert_to_int64
-SoortInschrijvingContinuTypeHoBinnenHo,220,1,convert_to_int64
+SoortInschrijvingContinuHogerOnderwijs,217,1,convert_to_object
+SoortInschrijvingContinuSoortHo,218,1,convert_to_object
+SoortInschrijvingContinuActueleInstelling,219,1,convert_to_object
+SoortInschrijvingContinuTypeHoBinnenHo,220,1,convert_to_object
 IndicatieEerstejaarsContinuHogerOnderwijs,221,1,convert_to_int64
 IndicatieEerstejaarsContinuSoortHo,222,1,convert_to_int64
 IndicatieEerstejaarsContinuActueleInstelling,223,1,convert_to_int64
 IndicatieEerstejaarsContinuTypeHoBinnenHo,224,1,convert_to_int64
 IndicatieSoortProgramma,225,1,convert_to_int64
 DatumInschrijving,226,8,convert_to_date
 DatumUitschrijving,234,8,convert_to_date
```

### Comparing `eencijfer-2024.2.4/eencijfer/convert/import_definitions/VAKHAVW_____.csv` & `eencijfer-2024.3.0/eencijfer/convert/import_definitions/VAKHAVW_____.csv`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.2.4/eencijfer/convert/pii.py` & `eencijfer-2024.3.0/eencijfer/convert/pii.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 """Tools for removing PII."""
 
-import configparser
 import logging
 from pathlib import Path
 
 import numpy as np
 import pandas as pd
 
 from eencijfer.io.file import ExportFormat, _save_to_file
-from eencijfer.settings import config
 from eencijfer.utils.detect_eencijfer_files import _get_eencijfer_datafile, _get_eindexamen_datafile
 from eencijfer.utils.local_data import _add_local_id
 
 logger = logging.getLogger(__name__)
 
 NEW_IDENTIFIER_SUFFIX = "_new"
 
@@ -120,43 +118,46 @@
     if len(fields_in_data_to_be_emptied) == 0:
         logger.debug(f"...no column found with names {sensitive_fields}, nothing to be removed.")
 
     return data
 
 
 def _replace_all_pgn_with_pseudo_id_remove_pii_local_id(
-    config: configparser.ConfigParser = config,
-    export_format=ExportFormat.parquet,
+    eencijfer_dir: Path,
     remove_pii: bool = True,
     add_local_id: bool = False,
 ) -> None:
     """Replaces id's with pseudo-id's, removes PII, adds local-'s.
 
     Args:
-        config (configparser.ConfigParser, optional): _description_. Defaults to config.
-        export_format (str, optional): Format in which file is saved. Defaults to 'parquet'.
+        eencijfer_dir (Path): Path to directory with eencijfer-parquet-files.
+        remove_pii (bool, optional): Remove person identifiable information. Defaults to True.
+        add_local_id (bool, optional): Add local id. Defaults to False.
+
+    Raises:
+        Exception: _description_
+        Exception: _description_
 
     Returns:
-        None: Saves files to result_dir.
+        None: Overwrite files to eencijfer_dir.
     """
 
     logger.debug('Replacing pgns and removing pii.')
-    result_dir = config.getpath('default', 'result_dir')
 
-    eencijfer_fname = _get_eencijfer_datafile(result_dir)
+    eencijfer_fname = _get_eencijfer_datafile(eencijfer_dir)
     if eencijfer_fname is None:
         raise Exception("No eencijfer-file found.")
-    eencijfer_fpath = Path(result_dir / eencijfer_fname).with_suffix(f'.{export_format.value}')
+    eencijfer_fpath = Path(eencijfer_dir / eencijfer_fname).with_suffix('.parquet')
     eencijfer = pd.read_parquet(eencijfer_fpath)
 
-    vakken_fname = _get_eindexamen_datafile(result_dir)
+    vakken_fname = _get_eindexamen_datafile(eencijfer_dir)
     if vakken_fname is None:
         raise Exception("No eindexamen-file found.")
 
-    vakken_fpath = Path(result_dir / vakken_fname).with_suffix(f'.{export_format.value}')
+    vakken_fpath = Path(eencijfer_dir / vakken_fname).with_suffix('.parquet')
     vakken = pd.read_parquet(vakken_fpath)
 
     if add_local_id:
         logger.info('Adding local_id to eencijfer and vakken.')
         eencijfer = _add_local_id(eencijfer)
         vakken = _add_local_id(vakken)
 
@@ -169,13 +170,13 @@
         eencijfer = _replace_pgn_with_pseudo_id(eencijfer, koppeltabel)
         eencijfer = _empty_id_fields(eencijfer)
 
         logger.info(f'...removing pgn from {vakken_fpath}')
         vakken = _replace_pgn_with_pseudo_id(vakken, koppeltabel)
         vakken = _empty_id_fields(vakken)
 
-    logger.info(f"Saving {eencijfer_fname} to {result_dir}")
-    _save_to_file(eencijfer, fname=eencijfer_fname, dir=result_dir, export_format=export_format)
+    logger.info(f"Overwriting {eencijfer_fname} to {eencijfer_dir}")
+    _save_to_file(eencijfer, fname=eencijfer_fname, dir=eencijfer_dir, export_format=ExportFormat.parquet)
 
-    logger.info(f"Saving {vakken_fname} to {result_dir}")
-    _save_to_file(vakken, fname=vakken_fname, dir=result_dir, export_format=export_format)
+    logger.info(f"Saving {vakken_fname} to {eencijfer_dir}")
+    _save_to_file(vakken, fname=vakken_fname, dir=eencijfer_dir, export_format=ExportFormat.parquet)
     return None
```

### Comparing `eencijfer-2024.2.4/eencijfer/io/file.py` & `eencijfer-2024.3.0/eencijfer/io/file.py`

 * *Files 7% similar despite different names*

```diff
@@ -61,25 +61,26 @@
         target_fpath = Path(fpath).with_suffix('.xlsx')
         logger.info(f"Saving {fname} to {target_fpath}...")
         df.to_excel(target_fpath, index=False)
 
     return None
 
 
-def _convert_to_export_format_remove_parquet(result_dir: Path, export_format: ExportFormat = ExportFormat.parquet):
+def _convert_to_export_format(source_dir: Path, result_dir: Path, export_format: ExportFormat = ExportFormat.parquet):
     """Convert files in directory to exportformat.
 
     Args:
-        result_dir (Path): _description_. Defaults to None.
+        source_dir (Path): Path to directory with parquet files. Defaults to None.
+        result_dir (Path): Path to directory with files in export-format. Defaults to None.
         export_format (ExportFormat, optional): _description_. Defaults to ExportFormat.parquet.
 
     Returns:
         None: None
     """
-    eencijfer_files = _get_list_of_eencijfer_files_in_dir(result_dir)
+    eencijfer_files = _get_list_of_eencijfer_files_in_dir(source_dir)
 
     if eencijfer_files is None:
         raise Exception('No eencijfer-files found!')
 
     for file in eencijfer_files:
         target_fpath = Path(result_dir / file.name).with_suffix(f".{export_format.value}")
 
@@ -97,17 +98,14 @@
             raw_data = pd.read_parquet(file)
 
             if len(raw_data) > 0:
                 logger.debug(f"...reading {file.name} succeeded.")
                 logger.debug(f"...saving to {target_fpath}.")
                 _save_to_file(raw_data, dir=result_dir, fname=file.stem, export_format=export_format)
 
-                logger.debug(f"...removing {file}.")
-                Path.unlink(file)
-
             else:
                 logger.info(f"...there does not seem to be data in {file.name}!")
         except Exception as e:
             logger.warning(f"...inlezen van {file.name} mislukt.")
             logger.warning(f"{e}")
 
         logger.info("**************************************")
```

### Comparing `eencijfer-2024.2.4/eencijfer/settings.py` & `eencijfer-2024.3.0/eencijfer/settings.py`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.2.4/eencijfer/utils/detect_eencijfer_files.py` & `eencijfer-2024.3.0/eencijfer/utils/detect_eencijfer_files.py`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.2.4/eencijfer/utils/init.py` & `eencijfer-2024.3.0/eencijfer/utils/init.py`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.2.4/eencijfer/utils/local_data.py` & `eencijfer-2024.3.0/eencijfer/utils/local_data.py`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.2.4/eencijfer/utils/qa.py` & `eencijfer-2024.3.0/eencijfer/utils/qa.py`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.2.4/pyproject.toml` & `eencijfer-2024.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "eencijfer"
-version = "2024.2.4"
+version = "2024.3.0"
 homepage = "https://github.com/enningb/eencijfer"
 description = "ETL-tool for Dutch eencijfer."
 authors = ["Bram Enning <bramenning@gmail.com>"]
 readme = "README.md"
 license =  "MIT"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
@@ -86,15 +86,15 @@
 #skip_glob = docs/conf.py
 
 
 [tool.mypy]
 disable_error_code = ["attr-defined"]
 
 [tool.bumpversion]
-current_version = "2024.2.4"
+current_version = "2024.3.0"
 commit = true
 commit_args = "--no-verify"
 tag = true
 tag_name = "{new_version}"
 allow_dirty = true
 parse = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)(\\.(?P<dev>post)\\d+\\.dev\\d+)?"
 message = "Version updated from {current_version} to {new_version}"
@@ -110,12 +110,13 @@
 
 
 
 
 
 
 
+
 
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `eencijfer-2024.2.4/tests/test_eencijfer.py` & `eencijfer-2024.3.0/tests/test_eencijfer.py`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.2.4/PKG-INFO` & `eencijfer-2024.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eencijfer
-Version: 2024.2.4
+Version: 2024.3.0
 Summary: ETL-tool for Dutch eencijfer.
 Home-page: https://github.com/enningb/eencijfer
 License: MIT
 Author: Bram Enning
 Author-email: bramenning@gmail.com
 Requires-Python: >=3.9.0,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

