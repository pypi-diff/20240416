# Comparing `tmp/data2rdf-2.0.0rc2.tar.gz` & `tmp/data2rdf-2.0.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data2rdf-2.0.0rc2.tar", last modified: Tue Apr 16 07:59:01 2024, max compression
+gzip compressed data, was "data2rdf-2.0.0rc3.tar", last modified: Tue Apr 16 11:29:24 2024, max compression
```

## Comparing `data2rdf-2.0.0rc2.tar` & `data2rdf-2.0.0rc3.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:59:01.448921 data2rdf-2.0.0rc2/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1596 2024-04-16 07:58:56.000000 data2rdf-2.0.0rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4615 2024-04-16 07:59:01.448921 data2rdf-2.0.0rc2/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     2505 2024-04-16 07:58:56.000000 data2rdf-2.0.0rc2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:59:01.440921 data2rdf-2.0.0rc2/data2rdf/
--rwxr-xr-x   0 runner    (1001) docker     (127)      448 2024-04-16 07:58:56.000000 data2rdf-2.0.0rc2/data2rdf/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1882 2024-04-16 07:58:56.000000 data2rdf-2.0.0rc2/data2rdf/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:59:01.440921 data2rdf-2.0.0rc2/data2rdf/models/
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-16 07:58:56.000000 data2rdf-2.0.0rc2/data2rdf/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6695 2024-04-16 07:58:56.000000 data2rdf-2.0.0rc2/data2rdf/models/mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:59:01.440921 data2rdf-2.0.0rc2/data2rdf/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-16 07:58:56.000000 data2rdf-2.0.0rc2/data2rdf/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-04-16 07:58:56.000000 data2rdf-2.0.0rc2/data2rdf/parsers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7837 2024-04-16 07:58:56.000000 data2rdf-2.0.0rc2/data2rdf/parsers/csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     7393 2024-04-16 07:58:56.000000 data2rdf-2.0.0rc2/data2rdf/parsers/excel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-16 07:58:56.000000 data2rdf-2.0.0rc2/data2rdf/parsers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:59:01.440921 data2rdf-2.0.0rc2/data2rdf/pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-16 07:58:56.000000 data2rdf-2.0.0rc2/data2rdf/pipelines/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5929 2024-04-16 07:58:56.000000 data2rdf-2.0.0rc2/data2rdf/pipelines/abox_scaffolding_pipeline.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5656 2024-04-16 07:58:56.000000 data2rdf-2.0.0rc2/data2rdf/pipelines/annotation_pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:59:01.440921 data2rdf-2.0.0rc2/data2rdf/qudt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 07:58:56.000000 data2rdf-2.0.0rc2/data2rdf/qudt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-16 07:58:56.000000 data2rdf-2.0.0rc2/data2rdf/qudt/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-16 07:58:56.000000 data2rdf-2.0.0rc2/data2rdf/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:59:01.444921 data2rdf-2.0.0rc2/data2rdf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4615 2024-04-16 07:59:01.000000 data2rdf-2.0.0rc2/data2rdf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-16 07:59:01.000000 data2rdf-2.0.0rc2/data2rdf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 07:59:01.000000 data2rdf-2.0.0rc2/data2rdf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-16 07:59:01.000000 data2rdf-2.0.0rc2/data2rdf.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-16 07:59:01.000000 data2rdf-2.0.0rc2/data2rdf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-16 07:59:01.000000 data2rdf-2.0.0rc2/data2rdf.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1916 2024-04-16 07:59:01.448921 data2rdf-2.0.0rc2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)      104 2024-04-16 07:58:56.000000 data2rdf-2.0.0rc2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:59:01.444921 data2rdf-2.0.0rc2/tests/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:58:56.000000 data2rdf-2.0.0rc2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:59:01.444921 data2rdf-2.0.0rc2/tests/csv_pipeline_test/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:58:56.000000 data2rdf-2.0.0rc2/tests/csv_pipeline_test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:59:01.444921 data2rdf-2.0.0rc2/tests/csv_pipeline_test/input/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:58:56.000000 data2rdf-2.0.0rc2/tests/csv_pipeline_test/input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3105 2024-04-16 07:58:56.000000 data2rdf-2.0.0rc2/tests/csv_pipeline_test/test_parser.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3479 2024-04-16 07:58:56.000000 data2rdf-2.0.0rc2/tests/csv_pipeline_test/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-04-16 07:58:56.000000 data2rdf-2.0.0rc2/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-16 07:58:56.000000 data2rdf-2.0.0rc2/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:59:01.444921 data2rdf-2.0.0rc2/tests/xls_pipeline_test/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:58:56.000000 data2rdf-2.0.0rc2/tests/xls_pipeline_test/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2754 2024-04-16 07:58:56.000000 data2rdf-2.0.0rc2/tests/xls_pipeline_test/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-04-16 07:58:56.000000 data2rdf-2.0.0rc2/tests/xls_pipeline_test/test_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:29:24.944334 data2rdf-2.0.0rc3/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1596 2024-04-16 11:29:18.000000 data2rdf-2.0.0rc3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4615 2024-04-16 11:29:24.944334 data2rdf-2.0.0rc3/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2505 2024-04-16 11:29:18.000000 data2rdf-2.0.0rc3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:29:24.936334 data2rdf-2.0.0rc3/data2rdf/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      448 2024-04-16 11:29:18.000000 data2rdf-2.0.0rc3/data2rdf/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1882 2024-04-16 11:29:18.000000 data2rdf-2.0.0rc3/data2rdf/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:29:24.940334 data2rdf-2.0.0rc3/data2rdf/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-16 11:29:18.000000 data2rdf-2.0.0rc3/data2rdf/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6695 2024-04-16 11:29:18.000000 data2rdf-2.0.0rc3/data2rdf/models/mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:29:24.940334 data2rdf-2.0.0rc3/data2rdf/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-16 11:29:18.000000 data2rdf-2.0.0rc3/data2rdf/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-04-16 11:29:18.000000 data2rdf-2.0.0rc3/data2rdf/parsers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8498 2024-04-16 11:29:18.000000 data2rdf-2.0.0rc3/data2rdf/parsers/csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9636 2024-04-16 11:29:18.000000 data2rdf-2.0.0rc3/data2rdf/parsers/excel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-04-16 11:29:18.000000 data2rdf-2.0.0rc3/data2rdf/parsers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:29:24.940334 data2rdf-2.0.0rc3/data2rdf/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-16 11:29:18.000000 data2rdf-2.0.0rc3/data2rdf/pipelines/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5929 2024-04-16 11:29:18.000000 data2rdf-2.0.0rc3/data2rdf/pipelines/abox_scaffolding_pipeline.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5656 2024-04-16 11:29:18.000000 data2rdf-2.0.0rc3/data2rdf/pipelines/annotation_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:29:24.940334 data2rdf-2.0.0rc3/data2rdf/qudt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 11:29:18.000000 data2rdf-2.0.0rc3/data2rdf/qudt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-16 11:29:18.000000 data2rdf-2.0.0rc3/data2rdf/qudt/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-16 11:29:18.000000 data2rdf-2.0.0rc3/data2rdf/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-16 11:29:18.000000 data2rdf-2.0.0rc3/data2rdf/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:29:24.944334 data2rdf-2.0.0rc3/data2rdf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4615 2024-04-16 11:29:24.000000 data2rdf-2.0.0rc3/data2rdf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-16 11:29:24.000000 data2rdf-2.0.0rc3/data2rdf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 11:29:24.000000 data2rdf-2.0.0rc3/data2rdf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-16 11:29:24.000000 data2rdf-2.0.0rc3/data2rdf.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-16 11:29:24.000000 data2rdf-2.0.0rc3/data2rdf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-16 11:29:24.000000 data2rdf-2.0.0rc3/data2rdf.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1916 2024-04-16 11:29:24.944334 data2rdf-2.0.0rc3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      104 2024-04-16 11:29:18.000000 data2rdf-2.0.0rc3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:29:24.940334 data2rdf-2.0.0rc3/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:29:18.000000 data2rdf-2.0.0rc3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:29:24.940334 data2rdf-2.0.0rc3/tests/csv_pipeline_test/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:29:18.000000 data2rdf-2.0.0rc3/tests/csv_pipeline_test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:29:24.940334 data2rdf-2.0.0rc3/tests/csv_pipeline_test/input/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:29:18.000000 data2rdf-2.0.0rc3/tests/csv_pipeline_test/input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5494 2024-04-16 11:29:18.000000 data2rdf-2.0.0rc3/tests/csv_pipeline_test/test_parser.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4972 2024-04-16 11:29:18.000000 data2rdf-2.0.0rc3/tests/csv_pipeline_test/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-04-16 11:29:18.000000 data2rdf-2.0.0rc3/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-16 11:29:18.000000 data2rdf-2.0.0rc3/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:29:24.944334 data2rdf-2.0.0rc3/tests/xls_pipeline_test/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:29:18.000000 data2rdf-2.0.0rc3/tests/xls_pipeline_test/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6059 2024-04-16 11:29:18.000000 data2rdf-2.0.0rc3/tests/xls_pipeline_test/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-04-16 11:29:18.000000 data2rdf-2.0.0rc3/tests/xls_pipeline_test/test_pipeline.py
```

### Comparing `data2rdf-2.0.0rc2/LICENSE` & `data2rdf-2.0.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc2/PKG-INFO` & `data2rdf-2.0.0rc3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data2rdf
-Version: 2.0.0rc2
+Version: 2.0.0rc3
 Summary: A generic pipeline that can be used to map raw data to RDF.
 Home-page: https://github.com/MI-FraunhoferIWM/data2rdf
 Author: Paul Zierep, Yoav Nahshon, Pablo de Andres, Deepu Krishnareddy, Matthias Büschelberger
 Author-email: matthias.bueschelberger@iwm.fraunhofer.de, yoav.nahshon@iwm.fraunhofer.de, pablo.de.andres@iwm.fraunhofer.de, deepu.krishnareddy@iwm.fraunhofer.de, matthias.bueschelberger@iwm.fraunhofer.de
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `data2rdf-2.0.0rc2/README.md` & `data2rdf-2.0.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc2/data2rdf/config.py` & `data2rdf-2.0.0rc3/data2rdf/config.py`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc2/data2rdf/models/mapping.py` & `data2rdf-2.0.0rc3/data2rdf/models/mapping.py`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc2/data2rdf/parsers/base.py` & `data2rdf-2.0.0rc3/data2rdf/parsers/base.py`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc2/data2rdf/parsers/csv.py` & `data2rdf-2.0.0rc3/data2rdf/parsers/csv.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 """CSV Parser for data2rdf"""
 
+import warnings
 from io import StringIO
 from typing import TYPE_CHECKING, Any
 
 import pandas as pd
 from pydantic import Field, model_validator
 
 from data2rdf.models.mapping import (
     ClassConceptMapping,
     PropertyMapping,
     QuantityMapping,
 )
 from data2rdf.utils import make_prefix
+from data2rdf.warnings import MappingMissmatchWarning
 
 from .base import DataParser
-from .utils import _load_mapping_file, _strip_unit
+from .utils import _strip_unit, load_mapping_file
 
 if TYPE_CHECKING:
     from typing import Dict
 
 
 class CSVParser(DataParser):
     """
@@ -141,15 +143,15 @@
     @classmethod
     def run_parser(cls, self: "CSVParser") -> "CSVParser":
         """
         Parse metadata, time series metadata and time series
         """
 
         datafile: str = cls._load_data_file(self)
-        mapping: "Dict[str, ClassConceptMapping]" = _load_mapping_file(
+        mapping: "Dict[str, ClassConceptMapping]" = load_mapping_file(
             self.mapping, self.config, ClassConceptMapping
         )
 
         time_series: pd.DataFrame = cls._parse_time_series(self).dropna()
 
         # iterate over general metadata
         header = ["key", "value", "unit"]
@@ -163,59 +165,73 @@
             row = line.split(self.header_sep)
             metadatum = dict(zip(header, row))
 
             # get the match from the mapping
             key = metadatum.get("key")
             mapping_match = mapping.get(key)
 
-            # get unit
-            unit = mapping_match.unit or metadatum.get("unit") or None
-            if unit:
-                unit = _strip_unit(unit, self.config.remove_from_unit)
-
-            # instanciate model
-            model_data = {
-                "key": key,
-                "value": metadatum.get("value"),
-                "unit": unit,
-                "iri": mapping_match.iri,
-                "annotation": mapping_match.annotation or None,
-            }
-            if model_data.get("unit"):
-                model = QuantityMapping(**model_data)
+            # only map the data if a match is found
+            if mapping_match:
+                # get unit
+                unit = mapping_match.unit or metadatum.get("unit") or None
+                if unit:
+                    unit = _strip_unit(unit, self.config.remove_from_unit)
+
+                # instanciate model
+                model_data = {
+                    "key": key,
+                    "value": metadatum.get("value"),
+                    "unit": unit,
+                    "iri": mapping_match.iri,
+                    "annotation": mapping_match.annotation or None,
+                }
+                if model_data.get("unit"):
+                    model = QuantityMapping(**model_data)
+                else:
+                    model = PropertyMapping(**model_data)
+                self._general_metadata.append(model)
             else:
-                model = PropertyMapping(**model_data)
-            self._general_metadata.append(model)
+                warnings.warn(
+                    f"No match found in mapping for key `{key}`",
+                    MappingMissmatchWarning,
+                )
 
             if l_count == self.header_length - 1:
                 break
 
         # parse time series data and meta data
         self._time_series_metadata = []
         self._time_series = {}
         for key in time_series:
             # get matching mapping
             mapping_match = mapping.get(key)
 
-            # get unit
-            unit = mapping_match.unit or time_series[key].iloc[0] or None
-            if unit:
-                unit = _strip_unit(unit, self.config.remove_from_unit)
-
-            # assign model
-            model_data = {
-                "key": key,
-                "unit": unit,
-                "iri": mapping_match.iri,
-                "annotation": mapping_match.annotation or None,
-            }
-            self.time_series_metadata.append(QuantityMapping(**model_data))
+            if mapping_match:
+                # get unit
+                unit = mapping_match.unit or time_series[key].iloc[0] or None
+                if unit:
+                    unit = _strip_unit(unit, self.config.remove_from_unit)
+
+                # assign model
+                model_data = {
+                    "key": key,
+                    "unit": unit,
+                    "iri": mapping_match.iri,
+                    "annotation": mapping_match.annotation or None,
+                }
+                self.time_series_metadata.append(QuantityMapping(**model_data))
+
+                # assign time series data
+                self._time_series[key] = time_series[key][1:].to_list()
 
-            # assign time series data
-            self._time_series[key] = time_series[key][1:].to_list()
+            else:
+                warnings.warn(
+                    f"No match found in mapping for key `{key}`",
+                    MappingMissmatchWarning,
+                )
 
     @classmethod
     def _load_data_file(cls, self: "CSVParser") -> StringIO:
         with open(self.raw_data, encoding=self.config.encoding) as file:
             return StringIO(file.read())
 
     @classmethod
```

### Comparing `data2rdf-2.0.0rc2/data2rdf/parsers/utils.py` & `data2rdf-2.0.0rc3/data2rdf/parsers/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,45 @@
 """Data2RDF parser utilities"""
 
 import json
 from typing import TYPE_CHECKING
 
 import pandas as pd
 
+from data2rdf import Config
+
 if TYPE_CHECKING:
     from typing import Any, Dict, List, Union
 
-    from data2rdf import Config
-
 
-def _load_mapping_file(
+def load_mapping_file(
     mapping: "Union[str, Dict[str, Any]]",
-    config: "Config",
-    pydantic_model: "Any",
+    config: "Config" = Config(),
+    model_callable: "Any" = dict,
 ) -> "Dict[str, Any]":
+    """
+    Load a mapping file and transform its contents into a dictionary format.
+
+    Parameters:
+        mapping (Union[str, Dict[str, Any]]): Path to the mapping file (either a string representing the file path or a dictionary containing the mapping directly).
+        config (Config, optional): Configuration settings for loading the file. Defaults to Config().
+        model_callable (Any, optional): Callable object used to transform each row of the mapping file into the desired format. Defaults to dict.
+
+    Returns:
+        Dict[str, Any]: A dictionary containing the loaded mapping data.
+
+    Raises:
+        TypeError: If the `mapping` parameter is not of type `str` or `dict`, or if the file type for mapping is not supported.
+
+    Note:
+        - For Excel files (.xlsx), the 'sameas' sheet is read from the Excel file.
+        The contents are then transformed into a dictionary where each row corresponds to a key-value pair.
+        - For JSON files (.json), the entire file is loaded as a dictionary.
+        - If `mapping` is already a dictionary, it is returned as is.
+    """
     if not isinstance(mapping, (str, dict)):
         raise TypeError(
             f"""Mapping file must be of type `{str}` or `{dict}`,
             not `{type(mapping)}`."""
         )
     if isinstance(mapping, str):
         if mapping.endswith("xlsx"):
@@ -35,15 +55,15 @@
             }
         elif mapping.endswith("json"):
             with open(mapping, encoding=config.encoding) as file:
                 model = json.load(file)
         else:
             raise TypeError("File type for mapping not supported!")
 
-        result = {key: pydantic_model(**row) for key, row in model.items()}
+        result = {key: model_callable(**row) for key, row in model.items()}
     if isinstance(mapping, dict):
         result = mapping
     return result
 
 
 def _strip_unit(symbol: str, char_list: "List[str]") -> str:
     for char in char_list:
```

### Comparing `data2rdf-2.0.0rc2/data2rdf/pipelines/abox_scaffolding_pipeline.py` & `data2rdf-2.0.0rc3/data2rdf/pipelines/abox_scaffolding_pipeline.py`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc2/data2rdf/pipelines/annotation_pipeline.py` & `data2rdf-2.0.0rc3/data2rdf/pipelines/annotation_pipeline.py`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc2/data2rdf/qudt/utils.py` & `data2rdf-2.0.0rc3/data2rdf/qudt/utils.py`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc2/data2rdf/utils.py` & `data2rdf-2.0.0rc3/data2rdf/utils.py`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc2/data2rdf.egg-info/PKG-INFO` & `data2rdf-2.0.0rc3/data2rdf.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data2rdf
-Version: 2.0.0rc2
+Version: 2.0.0rc3
 Summary: A generic pipeline that can be used to map raw data to RDF.
 Home-page: https://github.com/MI-FraunhoferIWM/data2rdf
 Author: Paul Zierep, Yoav Nahshon, Pablo de Andres, Deepu Krishnareddy, Matthias Büschelberger
 Author-email: matthias.bueschelberger@iwm.fraunhofer.de, yoav.nahshon@iwm.fraunhofer.de, pablo.de.andres@iwm.fraunhofer.de, deepu.krishnareddy@iwm.fraunhofer.de, matthias.bueschelberger@iwm.fraunhofer.de
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `data2rdf-2.0.0rc2/data2rdf.egg-info/SOURCES.txt` & `data2rdf-2.0.0rc3/data2rdf.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
 data2rdf/__init__.py
 data2rdf/config.py
 data2rdf/utils.py
+data2rdf/warnings.py
 data2rdf.egg-info/PKG-INFO
 data2rdf.egg-info/SOURCES.txt
 data2rdf.egg-info/dependency_links.txt
 data2rdf.egg-info/entry_points.txt
 data2rdf.egg-info/requires.txt
 data2rdf.egg-info/top_level.txt
 data2rdf/models/__init__.py
```

### Comparing `data2rdf-2.0.0rc2/data2rdf.egg-info/requires.txt` & `data2rdf-2.0.0rc3/data2rdf.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc2/setup.cfg` & `data2rdf-2.0.0rc3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = data2rdf
-version = v2.0.0rc2
+version = v2.0.0rc3
 description = A generic pipeline that can be used to map raw data to RDF.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/MI-FraunhoferIWM/data2rdf
 author = Paul Zierep, Yoav Nahshon, Pablo de Andres, Deepu Krishnareddy, Matthias Büschelberger
 author_email = matthias.bueschelberger@iwm.fraunhofer.de, yoav.nahshon@iwm.fraunhofer.de, pablo.de.andres@iwm.fraunhofer.de, deepu.krishnareddy@iwm.fraunhofer.de, matthias.bueschelberger@iwm.fraunhofer.de
 license = BSD-3-Clause
```

### Comparing `data2rdf-2.0.0rc2/tests/csv_pipeline_test/test_pipeline.py` & `data2rdf-2.0.0rc3/tests/csv_pipeline_test/test_pipeline.py`

 * *Files 20% similar despite different names*

```diff
@@ -41,14 +41,66 @@
     "Remark": "",
 }
 
 normal_config = {"graph_identifier": "https://www.example.org"}
 bad_config = {"graph_identifier": "https://www.example.org", "foorbar": 123}
 
 
+def test_csv_pipeline_bad_mapping() -> None:
+    from rdflib import Graph
+
+    from data2rdf import AnnotationPipeline, Parser
+
+    parser = AnnotationPipeline(
+        raw_data=raw_data,
+        mapping=os.path.join(mapping_folder, "bad_tensile_test_mapping.json"),
+        parser=Parser.csv,
+        parser_args=parser_args,
+        extra_triples=template,
+    )
+    expected_graph = Graph()
+    expected_graph.parse(expected)
+
+    assert parser.graph.isomorphic(expected_graph)
+
+
+def test_csv_pipeline_no_match_in_mapping() -> None:
+    from rdflib import Graph
+
+    from data2rdf import AnnotationPipeline, Parser
+    from data2rdf.warnings import MappingMissmatchWarning
+
+    with pytest.warns(UserWarning, match="No match found") as warnings:
+        parser = AnnotationPipeline(
+            raw_data=os.path.join(
+                working_folder, "data", "BAD_DX56_D_FZ2_WR00_43.TXT"
+            ),
+            parser=Parser.csv,
+            extra_triples=template,
+            mapping=os.path.join(mapping_folder, "tensile_test_mapping.json"),
+            parser_args={
+                "header_sep": "\t",
+                "column_sep": "\t",
+                "header_length": 21,
+            },
+        )
+
+    missmatches = [
+        warning
+        for warning in warnings
+        if warning.category == MappingMissmatchWarning
+    ]
+    assert len(missmatches) == 1
+
+    expected_graph = Graph()
+    expected_graph.parse(expected)
+
+    assert parser.graph.isomorphic(expected_graph)
+
+
 @pytest.mark.parametrize("config", [normal_config, bad_config])
 def test_csv_pipeline_config(config) -> None:
     from rdflib import Graph
 
     from data2rdf import (  # isort:skip
         AnnotationPipeline,
         Parser,
```

### Comparing `data2rdf-2.0.0rc2/tests/test_models.py` & `data2rdf-2.0.0rc3/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc2/tests/test_utils.py` & `data2rdf-2.0.0rc3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc2/tests/xls_pipeline_test/test_pipeline.py` & `data2rdf-2.0.0rc3/tests/xls_pipeline_test/test_pipeline.py`

 * *Files 26% similar despite different names*

```diff
@@ -27,49 +27,64 @@
     "Tester": "Fe",
     "SampleIdentifier-2": "123456",
     "OriginalGaugeLength": 15,
     "SpecimenThickness": 1.5,
     "SpecimenWidth": 9.5,
     "TestingRate": 0.02,
     "Temperature": 25,
-    "Remark": "None",
 }
 
 
 normal_config = {"graph_identifier": "https://www.example.org"}
 bad_config = {"graph_identifier": "https://www.example.org", "foorbar": 123}
 
 
 @pytest.mark.parametrize("config", [normal_config, bad_config])
 def test_csv_pipeline_config(config) -> None:
     from rdflib import Graph
 
+    from data2rdf.warnings import MappingMissmatchWarning
+
     from data2rdf import (  # isort:skip
         AnnotationPipeline,
         Parser,
     )
 
-    pipeline = AnnotationPipeline(
-        raw_data=raw_data,
-        mapping=os.path.join(mapping_folder, "tensile_test_mapping.json"),
-        parser=Parser.excel,
-        extra_triples=template,
-        config=config,
-    )
+    with pytest.warns(
+        MappingMissmatchWarning, match="Concept with key"
+    ) as warnings:
+        pipeline = AnnotationPipeline(
+            raw_data=raw_data,
+            mapping=os.path.join(mapping_folder, "tensile_test_mapping.json"),
+            parser=Parser.excel,
+            extra_triples=template,
+            config=config,
+        )
+
+    missmatches = [
+        warning
+        for warning in warnings
+        if warning.category == MappingMissmatchWarning
+    ]
+    assert len(missmatches) == 1
+
     expected_graph = Graph()
     expected_graph.parse(expected)
 
     assert pipeline.graph.isomorphic(expected_graph)
     assert str(pipeline.graph.identifier) == config["graph_identifier"]
+    assert pipeline.plain_metadata == metadata
 
 
 @pytest.mark.parametrize("extension", ["xlsx", "json", dict])
 def test_excel_pipeline(extension) -> None:
     from rdflib import Graph
 
+    from data2rdf.warnings import MappingMissmatchWarning
+
     from data2rdf import (  # isort:skip
         AnnotationPipeline,
         Parser,
         PropertyMapping,
         QuantityMapping,
     )
 
@@ -79,22 +94,32 @@
         )
 
     else:
         path = os.path.join(mapping_folder, "tensile_test_mapping.json")
         with open(path, encoding="utf-8") as file:
             mapping = json.load(file)
 
-    pipeline = AnnotationPipeline(
-        raw_data=raw_data,
-        mapping=mapping,
-        parser=Parser.excel,
-        extra_triples=template,
-    )
+    with pytest.warns(
+        MappingMissmatchWarning, match="Concept with key"
+    ) as warnings:
+        pipeline = AnnotationPipeline(
+            raw_data=raw_data,
+            mapping=mapping,
+            parser=Parser.excel,
+            extra_triples=template,
+        )
+
+    missmatches = [
+        warning
+        for warning in warnings
+        if warning.category == MappingMissmatchWarning
+    ]
+    assert len(missmatches) == 1
 
-    assert len(pipeline.general_metadata) == 13
+    assert len(pipeline.general_metadata) == 12
     for row in pipeline.general_metadata:
         assert isinstance(row, QuantityMapping) or isinstance(
             row, PropertyMapping
         )
 
     assert len(pipeline.time_series_metadata) == 6
     for row in pipeline.time_series_metadata:
```

