# Comparing `tmp/data2rdf-2.0.0rc1.tar.gz` & `tmp/data2rdf-2.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data2rdf-2.0.0rc1.tar", last modified: Mon Apr 15 21:15:36 2024, max compression
+gzip compressed data, was "data2rdf-2.0.0rc2.tar", last modified: Tue Apr 16 07:59:01 2024, max compression
```

## Comparing `data2rdf-2.0.0rc1.tar` & `data2rdf-2.0.0rc2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:15:36.076108 data2rdf-2.0.0rc1/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1596 2024-04-15 21:15:31.000000 data2rdf-2.0.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4615 2024-04-15 21:15:36.076108 data2rdf-2.0.0rc1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     2505 2024-04-15 21:15:31.000000 data2rdf-2.0.0rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:15:36.068108 data2rdf-2.0.0rc1/data2rdf/
--rwxr-xr-x   0 runner    (1001) docker     (127)      448 2024-04-15 21:15:31.000000 data2rdf-2.0.0rc1/data2rdf/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1823 2024-04-15 21:15:31.000000 data2rdf-2.0.0rc1/data2rdf/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:15:36.072108 data2rdf-2.0.0rc1/data2rdf/models/
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-15 21:15:31.000000 data2rdf-2.0.0rc1/data2rdf/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6438 2024-04-15 21:15:31.000000 data2rdf-2.0.0rc1/data2rdf/models/mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:15:36.072108 data2rdf-2.0.0rc1/data2rdf/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-15 21:15:31.000000 data2rdf-2.0.0rc1/data2rdf/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-15 21:15:31.000000 data2rdf-2.0.0rc1/data2rdf/parsers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7837 2024-04-15 21:15:31.000000 data2rdf-2.0.0rc1/data2rdf/parsers/csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     7393 2024-04-15 21:15:31.000000 data2rdf-2.0.0rc1/data2rdf/parsers/excel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-15 21:15:31.000000 data2rdf-2.0.0rc1/data2rdf/parsers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:15:36.072108 data2rdf-2.0.0rc1/data2rdf/pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-15 21:15:31.000000 data2rdf-2.0.0rc1/data2rdf/pipelines/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5929 2024-04-15 21:15:31.000000 data2rdf-2.0.0rc1/data2rdf/pipelines/abox_scaffolding_pipeline.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5376 2024-04-15 21:15:31.000000 data2rdf-2.0.0rc1/data2rdf/pipelines/annotation_pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:15:36.072108 data2rdf-2.0.0rc1/data2rdf/qudt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 21:15:31.000000 data2rdf-2.0.0rc1/data2rdf/qudt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-15 21:15:31.000000 data2rdf-2.0.0rc1/data2rdf/qudt/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-15 21:15:31.000000 data2rdf-2.0.0rc1/data2rdf/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:15:36.076108 data2rdf-2.0.0rc1/data2rdf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4615 2024-04-15 21:15:36.000000 data2rdf-2.0.0rc1/data2rdf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-15 21:15:36.000000 data2rdf-2.0.0rc1/data2rdf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 21:15:36.000000 data2rdf-2.0.0rc1/data2rdf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-15 21:15:36.000000 data2rdf-2.0.0rc1/data2rdf.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-15 21:15:36.000000 data2rdf-2.0.0rc1/data2rdf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-15 21:15:36.000000 data2rdf-2.0.0rc1/data2rdf.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1916 2024-04-15 21:15:36.076108 data2rdf-2.0.0rc1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)      104 2024-04-15 21:15:31.000000 data2rdf-2.0.0rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:15:36.072108 data2rdf-2.0.0rc1/tests/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:15:31.000000 data2rdf-2.0.0rc1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:15:36.072108 data2rdf-2.0.0rc1/tests/csv_pipeline_test/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:15:31.000000 data2rdf-2.0.0rc1/tests/csv_pipeline_test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:15:36.072108 data2rdf-2.0.0rc1/tests/csv_pipeline_test/input/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:15:31.000000 data2rdf-2.0.0rc1/tests/csv_pipeline_test/input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-04-15 21:15:31.000000 data2rdf-2.0.0rc1/tests/csv_pipeline_test/test_parser.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2655 2024-04-15 21:15:31.000000 data2rdf-2.0.0rc1/tests/csv_pipeline_test/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-15 21:15:31.000000 data2rdf-2.0.0rc1/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-15 21:15:31.000000 data2rdf-2.0.0rc1/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:15:36.076108 data2rdf-2.0.0rc1/tests/xls_pipeline_test/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:15:31.000000 data2rdf-2.0.0rc1/tests/xls_pipeline_test/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2090 2024-04-15 21:15:31.000000 data2rdf-2.0.0rc1/tests/xls_pipeline_test/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-04-15 21:15:31.000000 data2rdf-2.0.0rc1/tests/xls_pipeline_test/test_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:59:01.448921 data2rdf-2.0.0rc2/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1596 2024-04-16 07:58:56.000000 data2rdf-2.0.0rc2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4615 2024-04-16 07:59:01.448921 data2rdf-2.0.0rc2/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2505 2024-04-16 07:58:56.000000 data2rdf-2.0.0rc2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:59:01.440921 data2rdf-2.0.0rc2/data2rdf/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      448 2024-04-16 07:58:56.000000 data2rdf-2.0.0rc2/data2rdf/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1882 2024-04-16 07:58:56.000000 data2rdf-2.0.0rc2/data2rdf/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:59:01.440921 data2rdf-2.0.0rc2/data2rdf/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-16 07:58:56.000000 data2rdf-2.0.0rc2/data2rdf/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6695 2024-04-16 07:58:56.000000 data2rdf-2.0.0rc2/data2rdf/models/mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:59:01.440921 data2rdf-2.0.0rc2/data2rdf/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-16 07:58:56.000000 data2rdf-2.0.0rc2/data2rdf/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-04-16 07:58:56.000000 data2rdf-2.0.0rc2/data2rdf/parsers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7837 2024-04-16 07:58:56.000000 data2rdf-2.0.0rc2/data2rdf/parsers/csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7393 2024-04-16 07:58:56.000000 data2rdf-2.0.0rc2/data2rdf/parsers/excel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-16 07:58:56.000000 data2rdf-2.0.0rc2/data2rdf/parsers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:59:01.440921 data2rdf-2.0.0rc2/data2rdf/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-16 07:58:56.000000 data2rdf-2.0.0rc2/data2rdf/pipelines/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5929 2024-04-16 07:58:56.000000 data2rdf-2.0.0rc2/data2rdf/pipelines/abox_scaffolding_pipeline.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5656 2024-04-16 07:58:56.000000 data2rdf-2.0.0rc2/data2rdf/pipelines/annotation_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:59:01.440921 data2rdf-2.0.0rc2/data2rdf/qudt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 07:58:56.000000 data2rdf-2.0.0rc2/data2rdf/qudt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-16 07:58:56.000000 data2rdf-2.0.0rc2/data2rdf/qudt/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-16 07:58:56.000000 data2rdf-2.0.0rc2/data2rdf/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:59:01.444921 data2rdf-2.0.0rc2/data2rdf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4615 2024-04-16 07:59:01.000000 data2rdf-2.0.0rc2/data2rdf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-16 07:59:01.000000 data2rdf-2.0.0rc2/data2rdf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 07:59:01.000000 data2rdf-2.0.0rc2/data2rdf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-16 07:59:01.000000 data2rdf-2.0.0rc2/data2rdf.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-16 07:59:01.000000 data2rdf-2.0.0rc2/data2rdf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-16 07:59:01.000000 data2rdf-2.0.0rc2/data2rdf.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1916 2024-04-16 07:59:01.448921 data2rdf-2.0.0rc2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      104 2024-04-16 07:58:56.000000 data2rdf-2.0.0rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:59:01.444921 data2rdf-2.0.0rc2/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:58:56.000000 data2rdf-2.0.0rc2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:59:01.444921 data2rdf-2.0.0rc2/tests/csv_pipeline_test/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:58:56.000000 data2rdf-2.0.0rc2/tests/csv_pipeline_test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:59:01.444921 data2rdf-2.0.0rc2/tests/csv_pipeline_test/input/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:58:56.000000 data2rdf-2.0.0rc2/tests/csv_pipeline_test/input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3105 2024-04-16 07:58:56.000000 data2rdf-2.0.0rc2/tests/csv_pipeline_test/test_parser.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3479 2024-04-16 07:58:56.000000 data2rdf-2.0.0rc2/tests/csv_pipeline_test/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-04-16 07:58:56.000000 data2rdf-2.0.0rc2/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-16 07:58:56.000000 data2rdf-2.0.0rc2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:59:01.444921 data2rdf-2.0.0rc2/tests/xls_pipeline_test/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:58:56.000000 data2rdf-2.0.0rc2/tests/xls_pipeline_test/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2754 2024-04-16 07:58:56.000000 data2rdf-2.0.0rc2/tests/xls_pipeline_test/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-04-16 07:58:56.000000 data2rdf-2.0.0rc2/tests/xls_pipeline_test/test_pipeline.py
```

### Comparing `data2rdf-2.0.0rc1/LICENSE` & `data2rdf-2.0.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc1/PKG-INFO` & `data2rdf-2.0.0rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data2rdf
-Version: 2.0.0rc1
+Version: 2.0.0rc2
 Summary: A generic pipeline that can be used to map raw data to RDF.
 Home-page: https://github.com/MI-FraunhoferIWM/data2rdf
 Author: Paul Zierep, Yoav Nahshon, Pablo de Andres, Deepu Krishnareddy, Matthias Büschelberger
 Author-email: matthias.bueschelberger@iwm.fraunhofer.de, yoav.nahshon@iwm.fraunhofer.de, pablo.de.andres@iwm.fraunhofer.de, deepu.krishnareddy@iwm.fraunhofer.de, matthias.bueschelberger@iwm.fraunhofer.de
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `data2rdf-2.0.0rc1/README.md` & `data2rdf-2.0.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc1/data2rdf/config.py` & `data2rdf-2.0.0rc2/data2rdf/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # The csv2rdf conversion requires a set of relations and classes to use for
 # the annotation these are defined separately, so that they can be easily
 # adapted.
 from typing import List, Optional, Union
 
-from pydantic import AnyUrl, Field
+from pydantic import AnyUrl, ConfigDict, Field
 from pydantic_settings import BaseSettings
 
 
 class Config(BaseSettings):
     """Data2RDF configuration"""
 
     qudt_units: AnyUrl = Field(
@@ -49,7 +49,9 @@
         description="Characters which should be removed from the input value for the unit",
     )
 
     unit_macro_location: int = Field(
         -1,
         description="Index where the marco for the unit in an excel cell might be located.",
     )
+
+    model_config = ConfigDict(extra="ignore")
```

### Comparing `data2rdf-2.0.0rc1/data2rdf/models/mapping.py` & `data2rdf-2.0.0rc2/data2rdf/models/mapping.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,22 @@
     )
 
     @property
     def suffix(cls) -> str:
         """Return suffix for individal"""
         return str(cls.iri).split(cls.config.separator)[-1]
 
+    @field_validator("config")
+    @classmethod
+    def validate_config(cls, value: Union[Dict[str, Any], Config]) -> Config:
+        """Validate configuration"""
+        if isinstance(value, dict):
+            value = Config(**value)
+        return value
+
 
 class ClassConceptMapping(BasicConceptMapping):
     """Mapping for a concept coming from the mapping file"""
 
     unit: Optional[Union[str, AnyUrl]] = Field(
         None, description="Symbol or QUDT IRI for the mapping"
     )
```

### Comparing `data2rdf-2.0.0rc1/data2rdf/parsers/base.py` & `data2rdf-2.0.0rc2/data2rdf/parsers/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Data2RDF base model for parsers"""
 
 import json
 from abc import abstractmethod
 from typing import TYPE_CHECKING, Any, Dict, Union
 
-from pydantic import BaseModel, Field, PrivateAttr
+from pydantic import BaseModel, Field, PrivateAttr, field_validator
 from rdflib import Graph
 
 from data2rdf import ClassConceptMapping, Config
 
 if TYPE_CHECKING:
     from typing import List
 
@@ -65,14 +65,22 @@
         """Metadata as flat json - without units and iris.
         Useful e.g. for the custom properties of the DSMS."""
         return {
             str(metadatum.iri).split(cls.config.separator)[-1]: metadatum.value
             for metadatum in cls.general_metadata
         }
 
+    @field_validator("config")
+    @classmethod
+    def validate_config(cls, value: Union[Dict[str, Any], Config]) -> Config:
+        """Validate configuration"""
+        if isinstance(value, dict):
+            value = Config(**value)
+        return value
+
     @classmethod
     @abstractmethod
     def run_parser(cls, self) -> "DataParser":
         """Model validator with mode = 'after' to run the parser."""
 
     @property
     @abstractmethod
```

### Comparing `data2rdf-2.0.0rc1/data2rdf/parsers/csv.py` & `data2rdf-2.0.0rc2/data2rdf/parsers/csv.py`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc1/data2rdf/parsers/excel.py` & `data2rdf-2.0.0rc2/data2rdf/parsers/excel.py`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc1/data2rdf/parsers/utils.py` & `data2rdf-2.0.0rc2/data2rdf/parsers/utils.py`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc1/data2rdf/pipelines/abox_scaffolding_pipeline.py` & `data2rdf-2.0.0rc2/data2rdf/pipelines/abox_scaffolding_pipeline.py`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc1/data2rdf/pipelines/annotation_pipeline.py` & `data2rdf-2.0.0rc2/data2rdf/pipelines/annotation_pipeline.py`

 * *Files 10% similar despite different names*

```diff
@@ -44,27 +44,35 @@
     )
 
     parser_args: Dict[str, Any] = Field(
         {},
         description="A dict with specific arguments for the parser. Is passed to the parser as kwargs.",
     )
 
-    config: Config = Field(
+    config: Union[Dict[str, Any], Config] = Field(
         default_factory=Config, description="Configuration object"
     )
 
     extra_triples: Optional[Union[str, Graph]] = Field(
         None,
         description="Filepath or rdflib-object for a Graph with extra triples for the resulting pipeline graph.",
     )
 
     model_config = ConfigDict(
         arbitrary_types_allowed=True, use_enum_values=True
     )
 
+    @field_validator("config")
+    @classmethod
+    def validate_config(cls, value: Union[Dict[str, Any], Config]) -> Config:
+        """Validate configuration"""
+        if isinstance(value, dict):
+            value = Config(**value)
+        return value
+
     @field_validator("extra_triples")
     @classmethod
     def validate_extra_triples(
         cls, value: Optional[Union[str, Graph]], info: ValidationInfo
     ) -> Graph:
         """Validate extra triples."""
         config = info.data.get("config")
```

### Comparing `data2rdf-2.0.0rc1/data2rdf/qudt/utils.py` & `data2rdf-2.0.0rc2/data2rdf/qudt/utils.py`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc1/data2rdf.egg-info/PKG-INFO` & `data2rdf-2.0.0rc2/data2rdf.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data2rdf
-Version: 2.0.0rc1
+Version: 2.0.0rc2
 Summary: A generic pipeline that can be used to map raw data to RDF.
 Home-page: https://github.com/MI-FraunhoferIWM/data2rdf
 Author: Paul Zierep, Yoav Nahshon, Pablo de Andres, Deepu Krishnareddy, Matthias Büschelberger
 Author-email: matthias.bueschelberger@iwm.fraunhofer.de, yoav.nahshon@iwm.fraunhofer.de, pablo.de.andres@iwm.fraunhofer.de, deepu.krishnareddy@iwm.fraunhofer.de, matthias.bueschelberger@iwm.fraunhofer.de
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `data2rdf-2.0.0rc1/data2rdf.egg-info/SOURCES.txt` & `data2rdf-2.0.0rc2/data2rdf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc1/data2rdf.egg-info/requires.txt` & `data2rdf-2.0.0rc2/data2rdf.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc1/setup.cfg` & `data2rdf-2.0.0rc2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = data2rdf
-version = v2.0.0rc1
+version = v2.0.0rc2
 description = A generic pipeline that can be used to map raw data to RDF.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/MI-FraunhoferIWM/data2rdf
 author = Paul Zierep, Yoav Nahshon, Pablo de Andres, Deepu Krishnareddy, Matthias Büschelberger
 author_email = matthias.bueschelberger@iwm.fraunhofer.de, yoav.nahshon@iwm.fraunhofer.de, pablo.de.andres@iwm.fraunhofer.de, deepu.krishnareddy@iwm.fraunhofer.de, matthias.bueschelberger@iwm.fraunhofer.de
 license = BSD-3-Clause
```

### Comparing `data2rdf-2.0.0rc1/tests/csv_pipeline_test/test_parser.py` & `data2rdf-2.0.0rc2/tests/xls_pipeline_test/test_parser.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,75 +6,88 @@
 import pytest
 
 test_folder = os.path.dirname(os.path.abspath(__file__))
 working_folder = os.path.join(test_folder, "input")
 output_folder = os.path.join(test_folder, "output")
 
 mapping_folder = os.path.join(working_folder, "mapping")
-raw_data = os.path.join(working_folder, "data", "DX56_D_FZ2_WR00_43.TXT")
-expected = os.path.join(output_folder, "output_csv_parser.ttl")
-
-parser_args = {"header_sep": "\t", "column_sep": "\t", "header_length": 20}
+raw_data = os.path.join(working_folder, "data", "AFZ1-Fz-S1Q.xlsm")
+expected = os.path.join(output_folder, "output_excel_parser.ttl")
 
 metadata = {
-    "TestingFacility": "institute_1",
-    "ProjectNumber": "123456",
-    "ProjectName": "proj_name_1",
-    "TimeStamp": "44335.4",
-    "MachineData": "maschine_1",
-    "ForceMeasuringDevice": "Kraftaufnehmer_1",
-    "DisplacementTransducer": "Wegaufnehmer_1",
-    "TestStandard": "ISO-XX",
+    "ProjectNumber": "Projekt_1",
+    "TimeStamp": "2016-10-11 00:00:00",
+    "MachineData": "M_1",
     "Material": "Werkstoff_1",
-    "SpecimenType": "Probentyp_1",
-    "Tester": "abc",
-    "SampleIdentifier-2": "Probentyp_2",
-    "OriginalGaugeLength": 80,
-    "ParallelLength": 120,
-    "SpecimenThickness": 1.55,
-    "SpecimenWidth": 20.04,
-    "TestingRate": 0.1,
-    "Preload": 2,
-    "Temperature": 22,
-    "Remark": "",
+    "SpecimenType": "Fz 10x20",
+    "Tester": "Fe",
+    "SampleIdentifier-2": "123456",
+    "OriginalGaugeLength": 15,
+    "SpecimenThickness": 1.5,
+    "SpecimenWidth": 9.5,
+    "TestingRate": 0.02,
+    "Temperature": 25,
+    "Remark": "None",
 }
 
 
+normal_config = {"graph_identifier": "https://www.example.org"}
+bad_config = {"graph_identifier": "https://www.example.org", "foorbar": 123}
+
+
+@pytest.mark.parametrize("config", [normal_config, bad_config])
+def test_csv_parser_config(config) -> None:
+    from rdflib import Graph
+
+    from data2rdf.parsers import ExcelParser
+
+    parser = ExcelParser(
+        raw_data=raw_data,
+        mapping=os.path.join(mapping_folder, "tensile_test_mapping.json"),
+        config=config,
+    )
+    expected_graph = Graph()
+    expected_graph.parse(expected)
+
+    assert parser.graph.isomorphic(expected_graph)
+    assert str(parser.graph.identifier) == config["graph_identifier"]
+
+
 @pytest.mark.parametrize("extension", ["xlsx", "json", dict])
-def test_parser(extension) -> None:
+def test_parser_excel(extension) -> None:
     from rdflib import Graph
 
-    from data2rdf.models.mapping import PropertyMapping, QuantityMapping
-    from data2rdf.parsers.csv import CSVParser
+    from data2rdf.models import PropertyMapping, QuantityMapping
+    from data2rdf.parsers import ExcelParser
 
     if isinstance(extension, str):
         mapping = os.path.join(
             mapping_folder, f"tensile_test_mapping.{extension}"
         )
 
     else:
         path = os.path.join(mapping_folder, "tensile_test_mapping.json")
         with open(path, encoding="utf-8") as file:
             mapping = json.load(file)
 
-    parser = CSVParser(raw_data=raw_data, mapping=mapping, **parser_args)
+    parser = ExcelParser(raw_data=raw_data, mapping=mapping)
 
-    assert len(parser.general_metadata) == 20
+    assert len(parser.general_metadata) == 13
     for row in parser.general_metadata:
         assert isinstance(row, QuantityMapping) or isinstance(
             row, PropertyMapping
         )
 
     assert len(parser.time_series_metadata) == 6
     for row in parser.time_series_metadata:
         assert isinstance(row, QuantityMapping)
 
     assert len(parser.time_series) == 6
     for row in parser.time_series.values():
-        assert len(row) == 5734
+        assert len(row) == 460
         assert isinstance(row, list)
 
     expected_graph = Graph()
     expected_graph.parse(expected)
 
     assert parser.graph.isomorphic(expected_graph)
```

### Comparing `data2rdf-2.0.0rc1/tests/csv_pipeline_test/test_pipeline.py` & `data2rdf-2.0.0rc2/tests/xls_pipeline_test/test_pipeline.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,44 +10,64 @@
 
 template = os.path.join(
     working_folder,
     "method-graph",
     "tensile_test_method_v6.mod.ttl",
 )
 mapping_folder = os.path.join(working_folder, "mapping")
-raw_data = os.path.join(working_folder, "data", "DX56_D_FZ2_WR00_43.TXT")
+raw_data = os.path.join(working_folder, "data", "AFZ1-Fz-S1Q.xlsm")
 expected = os.path.join(output_folder, "output_pipeline.ttl")
 
-parser_args = {"header_sep": "\t", "column_sep": "\t", "header_length": 20}
+
 metadata = {
-    "TestingFacility": "institute_1",
-    "ProjectNumber": "123456",
-    "ProjectName": "proj_name_1",
-    "TimeStamp": "44335.4",
-    "MachineData": "maschine_1",
-    "ForceMeasuringDevice": "Kraftaufnehmer_1",
-    "DisplacementTransducer": "Wegaufnehmer_1",
-    "TestStandard": "ISO-XX",
+    "ProjectNumber": "Projekt_1",
+    "TimeStamp": "2016-10-11 00:00:00",
+    "MachineData": "M_1",
     "Material": "Werkstoff_1",
-    "SpecimenType": "Probentyp_1",
-    "Tester": "abc",
-    "SampleIdentifier-2": "Probentyp_2",
-    "OriginalGaugeLength": 80,
-    "ParallelLength": 120,
-    "SpecimenThickness": 1.55,
-    "SpecimenWidth": 20.04,
-    "TestingRate": 0.1,
-    "Preload": 2,
-    "Temperature": 22,
-    "Remark": "",
+    "SpecimenType": "Fz 10x20",
+    "Tester": "Fe",
+    "SampleIdentifier-2": "123456",
+    "OriginalGaugeLength": 15,
+    "SpecimenThickness": 1.5,
+    "SpecimenWidth": 9.5,
+    "TestingRate": 0.02,
+    "Temperature": 25,
+    "Remark": "None",
 }
 
 
+normal_config = {"graph_identifier": "https://www.example.org"}
+bad_config = {"graph_identifier": "https://www.example.org", "foorbar": 123}
+
+
+@pytest.mark.parametrize("config", [normal_config, bad_config])
+def test_csv_pipeline_config(config) -> None:
+    from rdflib import Graph
+
+    from data2rdf import (  # isort:skip
+        AnnotationPipeline,
+        Parser,
+    )
+
+    pipeline = AnnotationPipeline(
+        raw_data=raw_data,
+        mapping=os.path.join(mapping_folder, "tensile_test_mapping.json"),
+        parser=Parser.excel,
+        extra_triples=template,
+        config=config,
+    )
+    expected_graph = Graph()
+    expected_graph.parse(expected)
+
+    assert pipeline.graph.isomorphic(expected_graph)
+    assert str(pipeline.graph.identifier) == config["graph_identifier"]
+
+
 @pytest.mark.parametrize("extension", ["xlsx", "json", dict])
-def test_csv_pipeline(extension) -> None:
+def test_excel_pipeline(extension) -> None:
     from rdflib import Graph
 
     from data2rdf import (  # isort:skip
         AnnotationPipeline,
         Parser,
         PropertyMapping,
         QuantityMapping,
@@ -62,32 +82,31 @@
         path = os.path.join(mapping_folder, "tensile_test_mapping.json")
         with open(path, encoding="utf-8") as file:
             mapping = json.load(file)
 
     pipeline = AnnotationPipeline(
         raw_data=raw_data,
         mapping=mapping,
-        parser=Parser.csv,
-        parser_args=parser_args,
+        parser=Parser.excel,
         extra_triples=template,
     )
 
-    assert len(pipeline.general_metadata) == 20
+    assert len(pipeline.general_metadata) == 13
     for row in pipeline.general_metadata:
         assert isinstance(row, QuantityMapping) or isinstance(
             row, PropertyMapping
         )
 
     assert len(pipeline.time_series_metadata) == 6
     for row in pipeline.time_series_metadata:
         assert isinstance(row, QuantityMapping)
 
     assert len(pipeline.time_series) == 6
     for row in pipeline.time_series.values():
-        assert len(row) == 5734
+        assert len(row) == 460
         assert isinstance(row, list)
 
     expected_graph = Graph()
     expected_graph.parse(expected)
 
     assert pipeline.graph.isomorphic(expected_graph)
```

### Comparing `data2rdf-2.0.0rc1/tests/test_utils.py` & `data2rdf-2.0.0rc2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc1/tests/xls_pipeline_test/test_parser.py` & `data2rdf-2.0.0rc2/tests/csv_pipeline_test/test_parser.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,66 +6,97 @@
 import pytest
 
 test_folder = os.path.dirname(os.path.abspath(__file__))
 working_folder = os.path.join(test_folder, "input")
 output_folder = os.path.join(test_folder, "output")
 
 mapping_folder = os.path.join(working_folder, "mapping")
-raw_data = os.path.join(working_folder, "data", "AFZ1-Fz-S1Q.xlsm")
-expected = os.path.join(output_folder, "output_excel_parser.ttl")
+raw_data = os.path.join(working_folder, "data", "DX56_D_FZ2_WR00_43.TXT")
+expected = os.path.join(output_folder, "output_csv_parser.ttl")
+
+parser_args = {"header_sep": "\t", "column_sep": "\t", "header_length": 20}
 
 metadata = {
-    "ProjectNumber": "Projekt_1",
-    "TimeStamp": "2016-10-11 00:00:00",
-    "MachineData": "M_1",
+    "TestingFacility": "institute_1",
+    "ProjectNumber": "123456",
+    "ProjectName": "proj_name_1",
+    "TimeStamp": "44335.4",
+    "MachineData": "maschine_1",
+    "ForceMeasuringDevice": "Kraftaufnehmer_1",
+    "DisplacementTransducer": "Wegaufnehmer_1",
+    "TestStandard": "ISO-XX",
     "Material": "Werkstoff_1",
-    "SpecimenType": "Fz 10x20",
-    "Tester": "Fe",
-    "SampleIdentifier-2": "123456",
-    "OriginalGaugeLength": 15,
-    "SpecimenThickness": 1.5,
-    "SpecimenWidth": 9.5,
-    "TestingRate": 0.02,
-    "Temperature": 25,
-    "Remark": "None",
+    "SpecimenType": "Probentyp_1",
+    "Tester": "abc",
+    "SampleIdentifier-2": "Probentyp_2",
+    "OriginalGaugeLength": 80,
+    "ParallelLength": 120,
+    "SpecimenThickness": 1.55,
+    "SpecimenWidth": 20.04,
+    "TestingRate": 0.1,
+    "Preload": 2,
+    "Temperature": 22,
+    "Remark": "",
 }
 
+normal_config = {"graph_identifier": "https://www.example.org"}
+bad_config = {"graph_identifier": "https://www.example.org", "foorbar": 123}
+
+
+@pytest.mark.parametrize("config", [normal_config, bad_config])
+def test_csv_parser_config(config) -> None:
+    from rdflib import Graph
+
+    from data2rdf.parsers import CSVParser
+
+    parser = CSVParser(
+        raw_data=raw_data,
+        mapping=os.path.join(mapping_folder, "tensile_test_mapping.json"),
+        **parser_args,
+        config=config,
+    )
+    expected_graph = Graph()
+    expected_graph.parse(expected)
+
+    assert parser.graph.isomorphic(expected_graph)
+    assert str(parser.graph.identifier) == config["graph_identifier"]
+
 
 @pytest.mark.parametrize("extension", ["xlsx", "json", dict])
-def test_parser(extension) -> None:
+def test_parser_csv(extension) -> None:
     from rdflib import Graph
 
-    from data2rdf.models.mapping import PropertyMapping, QuantityMapping
-    from data2rdf.parsers.excel import ExcelParser
+    from data2rdf.models import PropertyMapping, QuantityMapping
+    from data2rdf.parsers import CSVParser
 
     if isinstance(extension, str):
         mapping = os.path.join(
             mapping_folder, f"tensile_test_mapping.{extension}"
         )
 
     else:
         path = os.path.join(mapping_folder, "tensile_test_mapping.json")
         with open(path, encoding="utf-8") as file:
             mapping = json.load(file)
 
-    parser = ExcelParser(raw_data=raw_data, mapping=mapping)
+    parser = CSVParser(raw_data=raw_data, mapping=mapping, **parser_args)
 
-    assert len(parser.general_metadata) == 13
+    assert len(parser.general_metadata) == 20
     for row in parser.general_metadata:
         assert isinstance(row, QuantityMapping) or isinstance(
             row, PropertyMapping
         )
 
     assert len(parser.time_series_metadata) == 6
     for row in parser.time_series_metadata:
         assert isinstance(row, QuantityMapping)
 
     assert len(parser.time_series) == 6
     for row in parser.time_series.values():
-        assert len(row) == 460
+        assert len(row) == 5734
         assert isinstance(row, list)
 
     expected_graph = Graph()
     expected_graph.parse(expected)
 
     assert parser.graph.isomorphic(expected_graph)
```

