# Comparing `tmp/ssb_datadoc-0.8.3.tar.gz` & `tmp/ssb_datadoc-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssb_datadoc-0.8.3.tar", max compression
+gzip compressed data, was "ssb_datadoc-0.9.0.tar", max compression
```

## Comparing `ssb_datadoc-0.8.3.tar` & `ssb_datadoc-0.9.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0     1073 2024-04-03 12:53:52.041906 ssb_datadoc-0.8.3/LICENSE
--rw-r--r--   0        0        0     3034 2024-04-03 12:53:52.041906 ssb_datadoc-0.8.3/README.md
--rw-r--r--   0        0        0     5188 2024-04-03 12:54:04.289871 ssb_datadoc-0.8.3/pyproject.toml
--rw-r--r--   0        0        0       85 2024-04-03 12:53:52.045906 ssb_datadoc-0.8.3/src/datadoc/__init__.py
--rw-r--r--   0        0        0     6015 2024-04-03 12:53:52.045906 ssb_datadoc-0.8.3/src/datadoc/app.py
--rw-r--r--   0        0        0      154 2024-04-03 12:53:52.045906 ssb_datadoc-0.8.3/src/datadoc/assets/app_style.css
--rw-r--r--   0        0        0    80523 2024-04-03 12:53:52.045906 ssb_datadoc-0.8.3/src/datadoc/assets/bootstrap-icons.css
--rw-r--r--   0        0        0   163874 2024-04-03 12:53:52.045906 ssb_datadoc-0.8.3/src/datadoc/assets/bootstrap.min.css
--rw-r--r--   0        0        0    52127 2024-04-03 12:53:52.045906 ssb_datadoc-0.8.3/src/datadoc/assets/bundle.css
--rw-r--r--   0        0        0      390 2024-04-03 12:53:52.045906 ssb_datadoc-0.8.3/src/datadoc/assets/controlbar_style.css
--rw-r--r--   0        0        0   137124 2024-04-03 12:53:52.045906 ssb_datadoc-0.8.3/src/datadoc/assets/fonts/bootstrap-icons.woff
--rw-r--r--   0        0        0   102536 2024-04-03 12:53:52.045906 ssb_datadoc-0.8.3/src/datadoc/assets/fonts/bootstrap-icons.woff2
--rw-r--r--   0        0        0      218 2024-04-03 12:53:52.045906 ssb_datadoc-0.8.3/src/datadoc/assets/header.css
--rw-r--r--   0        0        0     1296 2024-04-03 12:53:52.045906 ssb_datadoc-0.8.3/src/datadoc/assets/workspace_style.css
--rw-r--r--   0        0        0      131 2024-04-03 12:53:52.045906 ssb_datadoc-0.8.3/src/datadoc/assets/workspace_tab.css
--rw-r--r--   0        0        0       56 2024-04-03 12:53:52.045906 ssb_datadoc-0.8.3/src/datadoc/backend/__init__.py
--rw-r--r--   0        0        0     5635 2024-04-03 12:53:52.045906 ssb_datadoc-0.8.3/src/datadoc/backend/code_list.py
--rw-r--r--   0        0        0    13540 2024-04-03 12:53:52.045906 ssb_datadoc-0.8.3/src/datadoc/backend/dapla_dataset_path_info.py
--rw-r--r--   0        0        0    11054 2024-04-03 12:53:52.045906 ssb_datadoc-0.8.3/src/datadoc/backend/datadoc_metadata.py
--rw-r--r--   0        0        0     7491 2024-04-03 12:53:52.045906 ssb_datadoc-0.8.3/src/datadoc/backend/dataset_parser.py
--rw-r--r--   0        0        0       83 2024-04-03 12:53:52.045906 ssb_datadoc-0.8.3/src/datadoc/backend/external_sources/__init__.py
--rw-r--r--   0        0        0     1681 2024-04-03 12:53:52.045906 ssb_datadoc-0.8.3/src/datadoc/backend/external_sources/external_sources.py
--rw-r--r--   0        0        0     5321 2024-04-03 12:53:52.045906 ssb_datadoc-0.8.3/src/datadoc/backend/model_backwards_compatibility.py
--rw-r--r--   0        0        0     5828 2024-04-03 12:53:52.045906 ssb_datadoc-0.8.3/src/datadoc/backend/statistic_subject_mapping.py
--rw-r--r--   0        0        0     2500 2024-04-03 12:53:52.045906 ssb_datadoc-0.8.3/src/datadoc/backend/user_info.py
--rw-r--r--   0        0        0     3730 2024-04-03 12:53:52.045906 ssb_datadoc-0.8.3/src/datadoc/config.py
--rw-r--r--   0        0        0     6184 2024-04-03 12:53:52.045906 ssb_datadoc-0.8.3/src/datadoc/enums.py
--rw-r--r--   0        0        0       52 2024-04-03 12:53:52.045906 ssb_datadoc-0.8.3/src/datadoc/frontend/__init__.py
--rw-r--r--   0        0        0      310 2024-04-03 12:53:52.045906 ssb_datadoc-0.8.3/src/datadoc/frontend/callbacks/__init__.py
--rw-r--r--   0        0        0     7865 2024-04-03 12:53:52.045906 ssb_datadoc-0.8.3/src/datadoc/frontend/callbacks/dataset.py
--rw-r--r--   0        0        0    13456 2024-04-03 12:53:52.045906 ssb_datadoc-0.8.3/src/datadoc/frontend/callbacks/register_callbacks.py
--rw-r--r--   0        0        0     5623 2024-04-03 12:53:52.045906 ssb_datadoc-0.8.3/src/datadoc/frontend/callbacks/utils.py
--rw-r--r--   0        0        0     5466 2024-04-03 12:53:52.045906 ssb_datadoc-0.8.3/src/datadoc/frontend/callbacks/variables.py
--rw-r--r--   0        0        0      190 2024-04-03 12:53:52.045906 ssb_datadoc-0.8.3/src/datadoc/frontend/components/__init__.py
--rw-r--r--   0        0        0     1063 2024-04-03 12:53:52.045906 ssb_datadoc-0.8.3/src/datadoc/frontend/components/alerts.py
--rw-r--r--   0        0        0     5414 2024-04-03 12:53:52.045906 ssb_datadoc-0.8.3/src/datadoc/frontend/components/builders.py
--rw-r--r--   0        0        0     2502 2024-04-03 12:53:52.045906 ssb_datadoc-0.8.3/src/datadoc/frontend/components/control_bars.py
--rw-r--r--   0        0        0     1101 2024-04-03 12:53:52.045906 ssb_datadoc-0.8.3/src/datadoc/frontend/components/dataset_tab.py
--rw-r--r--   0        0        0     1734 2024-04-03 12:53:52.045906 ssb_datadoc-0.8.3/src/datadoc/frontend/components/variables_tab.py
--rw-r--r--   0        0        0       74 2024-04-03 12:53:52.049906 ssb_datadoc-0.8.3/src/datadoc/frontend/fields/__init__.py
--rw-r--r--   0        0        0     8725 2024-04-03 12:53:52.049906 ssb_datadoc-0.8.3/src/datadoc/frontend/fields/display_base.py
--rw-r--r--   0        0        0    13438 2024-04-03 12:53:52.049906 ssb_datadoc-0.8.3/src/datadoc/frontend/fields/display_dataset.py
--rw-r--r--   0        0        0     8336 2024-04-03 12:53:52.049906 ssb_datadoc-0.8.3/src/datadoc/frontend/fields/display_variables.py
--rw-r--r--   0        0        0       72 2024-04-03 12:53:52.049906 ssb_datadoc-0.8.3/src/datadoc/logging_configuration/__init__.py
--rw-r--r--   0        0        0     1586 2024-04-03 12:53:52.049906 ssb_datadoc-0.8.3/src/datadoc/logging_configuration/json_formatter.py
--rw-r--r--   0        0        0     1747 2024-04-03 12:53:52.049906 ssb_datadoc-0.8.3/src/datadoc/logging_configuration/logging_config.py
--rw-r--r--   0        0        0        0 2024-04-03 12:53:52.049906 ssb_datadoc-0.8.3/src/datadoc/py.typed
--rw-r--r--   0        0        0      898 2024-04-03 12:53:52.049906 ssb_datadoc-0.8.3/src/datadoc/state.py
--rw-r--r--   0        0        0     2153 2024-04-03 12:53:52.049906 ssb_datadoc-0.8.3/src/datadoc/utils.py
--rw-r--r--   0        0        0      220 2024-04-03 12:53:52.049906 ssb_datadoc-0.8.3/src/datadoc/wsgi.py
--rw-r--r--   0        0        0     4583 1970-01-01 00:00:00.000000 ssb_datadoc-0.8.3/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-04-08 13:31:02.621467 ssb_datadoc-0.9.0/LICENSE
+-rw-r--r--   0        0        0     3034 2024-04-08 13:31:02.621467 ssb_datadoc-0.9.0/README.md
+-rw-r--r--   0        0        0     5188 2024-04-08 13:31:11.873447 ssb_datadoc-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0       85 2024-04-08 13:31:02.625467 ssb_datadoc-0.9.0/src/datadoc/__init__.py
+-rw-r--r--   0        0        0     6135 2024-04-08 13:31:02.625467 ssb_datadoc-0.9.0/src/datadoc/app.py
+-rw-r--r--   0        0        0      154 2024-04-08 13:31:02.625467 ssb_datadoc-0.9.0/src/datadoc/assets/app_style.css
+-rw-r--r--   0        0        0    80523 2024-04-08 13:31:02.625467 ssb_datadoc-0.9.0/src/datadoc/assets/bootstrap-icons.css
+-rw-r--r--   0        0        0   163874 2024-04-08 13:31:02.625467 ssb_datadoc-0.9.0/src/datadoc/assets/bootstrap.min.css
+-rw-r--r--   0        0        0    52127 2024-04-08 13:31:02.625467 ssb_datadoc-0.9.0/src/datadoc/assets/bundle.css
+-rw-r--r--   0        0        0      390 2024-04-08 13:31:02.625467 ssb_datadoc-0.9.0/src/datadoc/assets/controlbar_style.css
+-rw-r--r--   0        0        0   137124 2024-04-08 13:31:02.625467 ssb_datadoc-0.9.0/src/datadoc/assets/fonts/bootstrap-icons.woff
+-rw-r--r--   0        0        0   102536 2024-04-08 13:31:02.625467 ssb_datadoc-0.9.0/src/datadoc/assets/fonts/bootstrap-icons.woff2
+-rw-r--r--   0        0        0      218 2024-04-08 13:31:02.625467 ssb_datadoc-0.9.0/src/datadoc/assets/header.css
+-rw-r--r--   0        0        0     1349 2024-04-08 13:31:02.625467 ssb_datadoc-0.9.0/src/datadoc/assets/workspace_style.css
+-rw-r--r--   0        0        0      131 2024-04-08 13:31:02.625467 ssb_datadoc-0.9.0/src/datadoc/assets/workspace_tab.css
+-rw-r--r--   0        0        0       56 2024-04-08 13:31:02.625467 ssb_datadoc-0.9.0/src/datadoc/backend/__init__.py
+-rw-r--r--   0        0        0     5635 2024-04-08 13:31:02.629467 ssb_datadoc-0.9.0/src/datadoc/backend/code_list.py
+-rw-r--r--   0        0        0    15985 2024-04-08 13:31:02.629467 ssb_datadoc-0.9.0/src/datadoc/backend/dapla_dataset_path_info.py
+-rw-r--r--   0        0        0    10998 2024-04-08 13:31:02.629467 ssb_datadoc-0.9.0/src/datadoc/backend/datadoc_metadata.py
+-rw-r--r--   0        0        0     7491 2024-04-08 13:31:02.629467 ssb_datadoc-0.9.0/src/datadoc/backend/dataset_parser.py
+-rw-r--r--   0        0        0       83 2024-04-08 13:31:02.629467 ssb_datadoc-0.9.0/src/datadoc/backend/external_sources/__init__.py
+-rw-r--r--   0        0        0     1681 2024-04-08 13:31:02.629467 ssb_datadoc-0.9.0/src/datadoc/backend/external_sources/external_sources.py
+-rw-r--r--   0        0        0     5321 2024-04-08 13:31:02.629467 ssb_datadoc-0.9.0/src/datadoc/backend/model_backwards_compatibility.py
+-rw-r--r--   0        0        0     5828 2024-04-08 13:31:02.629467 ssb_datadoc-0.9.0/src/datadoc/backend/statistic_subject_mapping.py
+-rw-r--r--   0        0        0     2500 2024-04-08 13:31:02.629467 ssb_datadoc-0.9.0/src/datadoc/backend/user_info.py
+-rw-r--r--   0        0        0     3916 2024-04-08 13:31:02.629467 ssb_datadoc-0.9.0/src/datadoc/config.py
+-rw-r--r--   0        0        0     6184 2024-04-08 13:31:02.629467 ssb_datadoc-0.9.0/src/datadoc/enums.py
+-rw-r--r--   0        0        0       52 2024-04-08 13:31:02.629467 ssb_datadoc-0.9.0/src/datadoc/frontend/__init__.py
+-rw-r--r--   0        0        0      310 2024-04-08 13:31:02.629467 ssb_datadoc-0.9.0/src/datadoc/frontend/callbacks/__init__.py
+-rw-r--r--   0        0        0     8236 2024-04-08 13:31:02.629467 ssb_datadoc-0.9.0/src/datadoc/frontend/callbacks/dataset.py
+-rw-r--r--   0        0        0    12672 2024-04-08 13:31:02.629467 ssb_datadoc-0.9.0/src/datadoc/frontend/callbacks/register_callbacks.py
+-rw-r--r--   0        0        0     5623 2024-04-08 13:31:02.629467 ssb_datadoc-0.9.0/src/datadoc/frontend/callbacks/utils.py
+-rw-r--r--   0        0        0     7018 2024-04-08 13:31:02.629467 ssb_datadoc-0.9.0/src/datadoc/frontend/callbacks/variables.py
+-rw-r--r--   0        0        0      190 2024-04-08 13:31:02.629467 ssb_datadoc-0.9.0/src/datadoc/frontend/components/__init__.py
+-rw-r--r--   0        0        0     1367 2024-04-08 13:31:02.629467 ssb_datadoc-0.9.0/src/datadoc/frontend/components/alerts.py
+-rw-r--r--   0        0        0     5626 2024-04-08 13:31:02.629467 ssb_datadoc-0.9.0/src/datadoc/frontend/components/builders.py
+-rw-r--r--   0        0        0     2502 2024-04-08 13:31:02.629467 ssb_datadoc-0.9.0/src/datadoc/frontend/components/control_bars.py
+-rw-r--r--   0        0        0     1101 2024-04-08 13:31:02.629467 ssb_datadoc-0.9.0/src/datadoc/frontend/components/dataset_tab.py
+-rw-r--r--   0        0        0     1746 2024-04-08 13:31:02.629467 ssb_datadoc-0.9.0/src/datadoc/frontend/components/variables_tab.py
+-rw-r--r--   0        0        0       74 2024-04-08 13:31:02.629467 ssb_datadoc-0.9.0/src/datadoc/frontend/fields/__init__.py
+-rw-r--r--   0        0        0     8662 2024-04-08 13:31:02.629467 ssb_datadoc-0.9.0/src/datadoc/frontend/fields/display_base.py
+-rw-r--r--   0        0        0    13487 2024-04-08 13:31:02.629467 ssb_datadoc-0.9.0/src/datadoc/frontend/fields/display_dataset.py
+-rw-r--r--   0        0        0     8450 2024-04-08 13:31:02.629467 ssb_datadoc-0.9.0/src/datadoc/frontend/fields/display_variables.py
+-rw-r--r--   0        0        0       72 2024-04-08 13:31:02.629467 ssb_datadoc-0.9.0/src/datadoc/logging_configuration/__init__.py
+-rw-r--r--   0        0        0     1586 2024-04-08 13:31:02.629467 ssb_datadoc-0.9.0/src/datadoc/logging_configuration/json_formatter.py
+-rw-r--r--   0        0        0     1747 2024-04-08 13:31:02.629467 ssb_datadoc-0.9.0/src/datadoc/logging_configuration/logging_config.py
+-rw-r--r--   0        0        0        0 2024-04-08 13:31:02.629467 ssb_datadoc-0.9.0/src/datadoc/py.typed
+-rw-r--r--   0        0        0      898 2024-04-08 13:31:02.629467 ssb_datadoc-0.9.0/src/datadoc/state.py
+-rw-r--r--   0        0        0     2153 2024-04-08 13:31:02.629467 ssb_datadoc-0.9.0/src/datadoc/utils.py
+-rw-r--r--   0        0        0      220 2024-04-08 13:31:02.629467 ssb_datadoc-0.9.0/src/datadoc/wsgi.py
+-rw-r--r--   0        0        0     4583 1970-01-01 00:00:00.000000 ssb_datadoc-0.9.0/PKG-INFO
```

### Comparing `ssb_datadoc-0.8.3/LICENSE` & `ssb_datadoc-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ssb_datadoc-0.8.3/README.md` & `ssb_datadoc-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `ssb_datadoc-0.8.3/pyproject.toml` & `ssb_datadoc-0.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ssb-datadoc"
-version = "0.8.3"
+version = "0.9.0"
 description = "Document dataset metadata. For use in Statistics Norway's metadata system."
 authors = ["Statistics Norway <stat-dev@ssb.no>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/statisticsnorway/datadoc"
 repository = "https://github.com/statisticsnorway/datadoc"
 documentation = "https://statisticsnorway.github.io/datadoc"
```

### Comparing `ssb_datadoc-0.8.3/src/datadoc/app.py` & `ssb_datadoc-0.9.0/src/datadoc/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from datadoc import state
 from datadoc.backend.code_list import CodeList
 from datadoc.backend.datadoc_metadata import DataDocMetadata
 from datadoc.backend.statistic_subject_mapping import StatisticSubjectMapping
 from datadoc.enums import SupportedLanguages
 from datadoc.frontend.callbacks.register_callbacks import register_callbacks
 from datadoc.frontend.components.alerts import dataset_validation_error
+from datadoc.frontend.components.alerts import naming_convention_warning
 from datadoc.frontend.components.alerts import opened_dataset_error
 from datadoc.frontend.components.alerts import opened_dataset_success
 from datadoc.frontend.components.alerts import saved_metadata_success
 from datadoc.frontend.components.alerts import variables_validation_error
 from datadoc.frontend.components.control_bars import build_controls_bar
 from datadoc.frontend.components.control_bars import build_language_dropdown
 from datadoc.frontend.components.control_bars import header
@@ -61,14 +62,15 @@
                     progress_bar,
                     build_controls_bar(),
                     variables_validation_error,
                     dataset_validation_error,
                     opened_dataset_error,
                     saved_metadata_success,
                     opened_dataset_success,
+                    naming_convention_warning,
                     dbc.Tabs(
                         id="tabs",
                         class_name="ssb-tabs",
                         children=tabs_children,
                     ),
                 ],
                 className="main-content-app",
```

### Comparing `ssb_datadoc-0.8.3/src/datadoc/assets/bootstrap-icons.css` & `ssb_datadoc-0.9.0/src/datadoc/assets/bootstrap-icons.css`

 * *Files identical despite different names*

### Comparing `ssb_datadoc-0.8.3/src/datadoc/assets/bootstrap.min.css` & `ssb_datadoc-0.9.0/src/datadoc/assets/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `ssb_datadoc-0.8.3/src/datadoc/assets/bundle.css` & `ssb_datadoc-0.9.0/src/datadoc/assets/bundle.css`

 * *Files identical despite different names*

### Comparing `ssb_datadoc-0.8.3/src/datadoc/assets/fonts/bootstrap-icons.woff` & `ssb_datadoc-0.9.0/src/datadoc/assets/fonts/bootstrap-icons.woff`

 * *Files identical despite different names*

### Comparing `ssb_datadoc-0.8.3/src/datadoc/assets/fonts/bootstrap-icons.woff2` & `ssb_datadoc-0.9.0/src/datadoc/assets/fonts/bootstrap-icons.woff2`

 * *Files identical despite different names*

### Comparing `ssb_datadoc-0.8.3/src/datadoc/assets/workspace_style.css` & `ssb_datadoc-0.9.0/src/datadoc/assets/workspace_style.css`

 * *Files 6% similar despite different names*

```diff
@@ -77,7 +77,11 @@
 .form-check.ssb-checkbox{
     align-self: center;
 }
 
 .form-check{
     padding-left: 0;
 }
+
+label.form-check-label{
+    padding-left: 0.5rem;
+}
```

### Comparing `ssb_datadoc-0.8.3/src/datadoc/backend/code_list.py` & `ssb_datadoc-0.9.0/src/datadoc/backend/code_list.py`

 * *Files identical despite different names*

### Comparing `ssb_datadoc-0.8.3/src/datadoc/backend/dapla_dataset_path_info.py` & `ssb_datadoc-0.9.0/src/datadoc/backend/dapla_dataset_path_info.py`

 * *Files 14% similar despite different names*

```diff
@@ -288,54 +288,78 @@
     def __init__(self, dataset_path: str | os.PathLike[str]) -> None:
         """Digest the path so that it's ready for further parsing."""
         self.dataset_path = pathlib.Path(dataset_path)
         self.dataset_name_sections = self.dataset_path.stem.split("_")
         self._period_strings = self._extract_period_strings(self.dataset_name_sections)
 
     @staticmethod
-    def _extract_period_strings(dataset_name_sections: list[str]) -> list[str]:
-        """Extract period strings from dataset name sections.
-
-        Iterates over the dataset name sections and returns a list of strings
-        that match the year regex, stripping the first character. This extracts
-        the year periods from the dataset name.
+    def _get_period_string_indices(dataset_name_sections: list[str]) -> list[int]:
+        """Get all the indices at which period strings are found.
 
         Examples:
-        >>> DaplaDatasetPathInfo._extract_period_strings(['p2022', 'kommune', 'v1'])
-        ['2022']
+        >>> DaplaDatasetPathInfo._get_period_string_indices(['kommune', 'p2022', 'v1'])
+        [1]
 
-        >>> DaplaDatasetPathInfo._extract_period_strings(['p2022-01', 'p2023-06', 'kommune', 'v1'])
-        ['2022-01', '2023-06']
+        >>> DaplaDatasetPathInfo._get_period_string_indices(['kommune', 'p2022-01', 'p2023-06', 'v1'])
+        [1, 2]
 
-        >>> DaplaDatasetPathInfo._extract_period_strings(['p1990Q1', 'kommune', 'v1'])
-        ['1990Q1']
+        >>> DaplaDatasetPathInfo._get_period_string_indices(['kommune', 'p1990Q1', 'v1'])
+        [1]
 
-        >>> DaplaDatasetPathInfo._extract_period_strings(['varehandel','v1']) # No date will return empty string
+        >>> DaplaDatasetPathInfo._get_period_string_indices(['varehandel','v1'])
         []
-
         """
 
         def insert_p(regex: str) -> str:
             r"""Insert a p as the second character.
 
             Examples:
             >>> insert_p(r"^\d{4}[H]\d{1}$")
             '^p\d{4}[H]\d{1}$'
             """
             return regex[:1] + "p" + regex[1:]
 
         return [
-            x[1:]
-            for x in dataset_name_sections
+            i
+            for i, x in enumerate(dataset_name_sections)
             if any(
                 re.match(insert_p(date_format.regex_pattern), x)
                 for date_format in SUPPORTED_DATE_FORMATS
             )
         ]
 
+    @staticmethod
+    def _extract_period_strings(dataset_name_sections: list[str]) -> list[str]:
+        """Extract period strings from dataset name sections.
+
+        Iterates over the dataset name sections and returns a list of strings
+        that match the year regex, stripping the first character. This extracts
+        the year periods from the dataset name.
+
+        Examples:
+        >>> DaplaDatasetPathInfo._extract_period_strings(['p2022', 'kommune', 'v1'])
+        ['2022']
+
+        >>> DaplaDatasetPathInfo._extract_period_strings(['p2022-01', 'p2023-06', 'kommune', 'v1'])
+        ['2022-01', '2023-06']
+
+        >>> DaplaDatasetPathInfo._extract_period_strings(['p1990Q1', 'kommune', 'v1'])
+        ['1990Q1']
+
+        >>> DaplaDatasetPathInfo._extract_period_strings(['varehandel','v1'])
+        []
+
+        """
+        return [
+            dataset_name_sections[i][1:]
+            for i in DaplaDatasetPathInfo._get_period_string_indices(
+                dataset_name_sections,
+            )
+        ]
+
     def _extract_period_string_from_index(self, index: int) -> str | None:
         try:
             return self._period_strings[index]
         except IndexError:
             return None
 
     def _extract_norwegian_dataset_state_path_part(
@@ -344,14 +368,46 @@
     ) -> set:
         norwegian_dataset_state_path_part = dataset_state.get_value_for_language(
             SupportedLanguages.NORSK_BOKMÅL,
         ).lower()
         return {norwegian_dataset_state_path_part.replace(" ", x) for x in ["-", "_"]}
 
     @property
+    def dataset_short_name(
+        self,
+    ) -> str | None:
+        """Extract the dataset short name from the filepath.
+
+        The dataset short name is defined as the first section of the stem, up to the period information,
+        or the version information if no period information is present.
+
+        Examples:
+        >>> DaplaDatasetPathInfo('prosjekt/befolkning/klargjorte_data/person_data_v1.parquet').dataset_short_name
+        person_data
+        >>> DaplaDatasetPathInfo('befolkning/inndata/sykepenger_p2022Q1_p2022Q2_v23.parquet').dataset_short_name
+        sykepenger
+        >>> DaplaDatasetPathInfo('my_data/simple_dataset_name.parquet').dataset_short_name
+        simple_dataset_name
+        """
+        if self.contains_data_from or self.contains_data_until:
+            short_name_sections = self.dataset_name_sections[
+                : min(
+                    DaplaDatasetPathInfo._get_period_string_indices(
+                        self.dataset_name_sections,
+                    ),
+                )
+            ]
+        elif self.dataset_version:
+            short_name_sections = self.dataset_name_sections[:-1]
+        else:
+            short_name_sections = self.dataset_name_sections
+
+        return "_".join(short_name_sections)
+
+    @property
     def contains_data_from(self) -> datetime.date | None:
         """The earliest date from which data in the dataset is relevant for."""
         period_string = self._extract_period_string_from_index(0)
         if not period_string or (
             len(self._period_strings) > 1 and period_string > self._period_strings[1]
         ):
             return None
@@ -446,7 +502,19 @@
                 dataset_state,
             )
             dataset_path_parts = list(self.dataset_path.parts)
             for i in dataset_state_names:
                 if i in dataset_path_parts and dataset_path_parts.index(i) != 0:
                     return dataset_path_parts[dataset_path_parts.index(i) - 1]
         return None
+
+    def path_complies_with_naming_standard(self) -> bool:
+        """Checks if path is valid according to SSB standard."""
+        if (
+            self.dataset_state
+            and self.statistic_short_name
+            and self.contains_data_from
+            and self.contains_data_until
+            and self.dataset_version
+        ):
+            return True
+        return False
```

### Comparing `ssb_datadoc-0.8.3/src/datadoc/backend/datadoc_metadata.py` & `ssb_datadoc-0.9.0/src/datadoc/backend/datadoc_metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,14 @@
         metadata_document_path: str | None = None,
     ) -> None:
         """Read in a dataset if supplied, otherwise naively instantiate the class."""
         self._statistic_subject_mapping = statistic_subject_mapping
         self.metadata_document: pathlib.Path | CloudPath | None = None
         self.container: model.MetadataContainer | None = None
         self.dataset_path: pathlib.Path | CloudPath | None = None
-        self.short_name: str | None = None
         self.dataset = model.Dataset()
         self.variables: list = []
         self.variables_lookup: dict[str, model.Variable] = {}
         if metadata_document_path:
             # In this case the user has specified an independent metadata document for editing
             # without a dataset.
             self.metadata_document = self._open_path(metadata_document_path)
@@ -172,24 +171,24 @@
         dapla_dataset_path_info = DaplaDatasetPathInfo(dataset)
 
         subject_field = self._statistic_subject_mapping.get_secondary_subject(
             dapla_dataset_path_info.statistic_short_name,
         )
 
         self.dataset = model.Dataset(
-            short_name=self.dataset_path.stem if self.dataset_path else None,
+            short_name=dapla_dataset_path_info.dataset_short_name,
             dataset_state=dapla_dataset_path_info.dataset_state,
             dataset_status=DataSetStatus.DRAFT,
             assessment=self.get_assessment_by_state(
                 dapla_dataset_path_info.dataset_state,
             ),
             version=dapla_dataset_path_info.dataset_version,
             contains_data_from=str(dapla_dataset_path_info.contains_data_from),
             contains_data_until=str(dapla_dataset_path_info.contains_data_until),
-            data_source_path=self.dataset_path,
+            file_path=str(self.dataset_path),
             metadata_created_by=user_info.get_user_info_for_current_platform().short_email,
             # TODO @mmwinther: Remove multiple_language_support once the model is updated.
             # https://github.com/statisticsnorway/ssb-datadoc-model/issues/41
             subject_field=model.LanguageStringType(
                 en=subject_field,
                 nb=subject_field,
                 nn=subject_field,
```

### Comparing `ssb_datadoc-0.8.3/src/datadoc/backend/dataset_parser.py` & `ssb_datadoc-0.9.0/src/datadoc/backend/dataset_parser.py`

 * *Files identical despite different names*

### Comparing `ssb_datadoc-0.8.3/src/datadoc/backend/external_sources/external_sources.py` & `ssb_datadoc-0.9.0/src/datadoc/backend/external_sources/external_sources.py`

 * *Files identical despite different names*

### Comparing `ssb_datadoc-0.8.3/src/datadoc/backend/model_backwards_compatibility.py` & `ssb_datadoc-0.9.0/src/datadoc/backend/model_backwards_compatibility.py`

 * *Files identical despite different names*

### Comparing `ssb_datadoc-0.8.3/src/datadoc/backend/statistic_subject_mapping.py` & `ssb_datadoc-0.9.0/src/datadoc/backend/statistic_subject_mapping.py`

 * *Files identical despite different names*

### Comparing `ssb_datadoc-0.8.3/src/datadoc/backend/user_info.py` & `ssb_datadoc-0.9.0/src/datadoc/backend/user_info.py`

 * *Files identical despite different names*

### Comparing `ssb_datadoc-0.8.3/src/datadoc/config.py` & `ssb_datadoc-0.9.0/src/datadoc/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -129,7 +129,12 @@
     """The code for the Unit Type code list in Klass."""
     return int(_get_config_item("DATADOC_UNIT_CODE") or 702)
 
 
 def get_organisational_unit_code() -> int | None:
     """The code for the organisational units code list in Klass."""
     return int(_get_config_item("DATADOC_ORGANISATIONAL_UNIT_CODE") or 83)
+
+
+def get_dapla_manual_naming_standard_url() -> str | None:
+    """Get the URL to naming standard in the DAPLA manual."""
+    return _get_config_item("DAPLA_MANUAL_NAMING_STANDARD_URL")
```

### Comparing `ssb_datadoc-0.8.3/src/datadoc/enums.py` & `ssb_datadoc-0.9.0/src/datadoc/enums.py`

 * *Files identical despite different names*

### Comparing `ssb_datadoc-0.8.3/src/datadoc/frontend/callbacks/dataset.py` & `ssb_datadoc-0.9.0/src/datadoc/frontend/callbacks/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import logging
 import traceback
 from typing import TYPE_CHECKING
 
 from pydantic import ValidationError
 
 from datadoc import state
+from datadoc.backend.dapla_dataset_path_info import DaplaDatasetPathInfo
 from datadoc.backend.datadoc_metadata import DataDocMetadata
 from datadoc.enums import (
     SupportedLanguages,  # noqa: TCH001 import is needed for docs build
 )
 from datadoc.frontend.callbacks.utils import MetadataInputTypes
 from datadoc.frontend.callbacks.utils import find_existing_language_string
 from datadoc.frontend.callbacks.utils import get_dataset_path
@@ -49,40 +50,44 @@
         dataset_path=str(dataset) if dataset else None,
     )
 
 
 def open_dataset_handling(
     n_clicks: int,
     file_path: str,
-) -> tuple[bool, bool, str, str]:
+) -> tuple[bool, bool, bool, str, str]:
     """Handle errors and other logic around opening a dataset file."""
     if file_path:
         file_path = file_path.strip()
-
     try:
         state.metadata = open_file(file_path)
     except FileNotFoundError:
         logger.exception("File %s not found", str(file_path))
         return (
             False,
             True,
+            False,
             f"Filen '{file_path}' finnes ikke.",
             state.current_metadata_language.value,
         )
     except Exception as e:  # noqa: BLE001
         return (
             False,
             True,
+            False,
             "\n".join(traceback.format_exception_only(type(e), e)),
             state.current_metadata_language.value,
         )
     if n_clicks and n_clicks > 0:
-        return True, False, "", state.current_metadata_language.value
-
-    return False, False, "", state.current_metadata_language.value
+        dapla_dataset_path_info = DaplaDatasetPathInfo(file_path)
+        if not dapla_dataset_path_info.path_complies_with_naming_standard():
+            return (True, False, True, "", state.current_metadata_language.value)
+        return True, False, False, "", state.current_metadata_language.value
+    # no message
+    return False, False, False, "", state.current_metadata_language.value
 
 
 def process_keyword(value: str) -> list[str]:
     """Convert a comma separated string to a list of strings.
 
     e.g. 'a,b ,c' -> ['a', 'b', 'c']
     """
```

### Comparing `ssb_datadoc-0.8.3/src/datadoc/frontend/callbacks/register_callbacks.py` & `ssb_datadoc-0.9.0/src/datadoc/frontend/callbacks/register_callbacks.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,30 +21,27 @@
 from datadoc.enums import SupportedLanguages
 from datadoc.frontend.callbacks.dataset import accept_dataset_metadata_date_input
 from datadoc.frontend.callbacks.dataset import accept_dataset_metadata_input
 from datadoc.frontend.callbacks.dataset import open_dataset_handling
 from datadoc.frontend.callbacks.utils import update_global_language_state
 from datadoc.frontend.callbacks.variables import accept_variable_metadata_date_input
 from datadoc.frontend.callbacks.variables import accept_variable_metadata_input
+from datadoc.frontend.callbacks.variables import populate_variables_workspace
 from datadoc.frontend.components.builders import build_dataset_edit_section
-from datadoc.frontend.components.builders import build_edit_section
-from datadoc.frontend.components.builders import build_ssb_accordion
 from datadoc.frontend.components.dataset_tab import SECTION_WRAPPER_ID
 from datadoc.frontend.components.variables_tab import ACCORDION_WRAPPER_ID
 from datadoc.frontend.components.variables_tab import VARIABLES_INFORMATION_ID
 from datadoc.frontend.fields.display_base import DATASET_METADATA_DATE_INPUT
 from datadoc.frontend.fields.display_base import DATASET_METADATA_INPUT
 from datadoc.frontend.fields.display_base import VARIABLES_METADATA_DATE_INPUT
 from datadoc.frontend.fields.display_base import VARIABLES_METADATA_INPUT
 from datadoc.frontend.fields.display_dataset import NON_EDITABLE_DATASET_METADATA
 from datadoc.frontend.fields.display_dataset import OBLIGATORY_EDITABLE_DATASET_METADATA
 from datadoc.frontend.fields.display_dataset import OPTIONAL_DATASET_METADATA
 from datadoc.frontend.fields.display_dataset import DatasetIdentifiers
-from datadoc.frontend.fields.display_variables import OBLIGATORY_VARIABLES_METADATA
-from datadoc.frontend.fields.display_variables import OPTIONAL_VARIABLES_METADATA
 from datadoc.frontend.fields.display_variables import VariableIdentifiers
 
 if TYPE_CHECKING:
     import dash_bootstrap_components as dbc
 
     from datadoc.frontend.callbacks.utils import MetadataInputTypes
 
@@ -106,23 +103,24 @@
             ctx.triggered[0]["value"],
             ctx.triggered_id["id"],
         )
 
     @app.callback(
         Output("opened-dataset-success", "is_open"),
         Output("opened-dataset-error", "is_open"),
+        Output("opened-dataset_warning", "is_open"),
         Output("opened-dataset-error-explanation", "children"),
         Output("language-dropdown", "value"),  # Used to force reload of metadata
         Input("open-button", "n_clicks"),
         State("dataset-path-input", "value"),
     )
     def callback_open_dataset(
         n_clicks: int,
         dataset_path: str,
-    ) -> tuple[bool, bool, str, str]:
+    ) -> tuple[bool, bool, bool, str, str]:
         """Open a dataset.
 
         Shows an alert on success or failure.
 
         To trigger reload of data in the UI, we update the
         language dropdown. This is a hack and could be replaced
         by a more formal mechanism.
@@ -138,61 +136,46 @@
         language: str,  # noqa: ARG001 Dash requires arguments for all Inputs
     ) -> str:
         return f"Datasettet inneholder {len(state.metadata.variables)} variabler."
 
     @app.callback(
         Output(ACCORDION_WRAPPER_ID, "children"),
         Input("language-dropdown", "value"),
+        Input("search-variables", "value"),
         prevent_initial_call=True,
     )
     def callback_populate_variables_workspace(
         language: str,
+        search_query: str,
     ) -> list:
-        """Create variable workspace with accordions for variables."""
+        """Create variable workspace with accordions for variables.
+
+        Allows for filtering which variables are displayed via the search box.
+        """
         update_global_language_state(SupportedLanguages(language))
-        logger.info("Populating new variables workspace")
-        return [
-            build_ssb_accordion(
-                variable.short_name,
-                {
-                    "type": "variables-accordion",
-                    "id": f"{variable.short_name}-{language}",  # Insert language into the ID to invalidate browser caches
-                },
-                variable.short_name,
-                children=[
-                    build_edit_section(
-                        OBLIGATORY_VARIABLES_METADATA,
-                        "Obligatorisk",
-                        variable,
-                        state.current_metadata_language.value,
-                    ),
-                    build_edit_section(
-                        OPTIONAL_VARIABLES_METADATA,
-                        "Anbefalt",
-                        variable,
-                        state.current_metadata_language.value,
-                    ),
-                ],
-            )
-            for variable in list(state.metadata.variables)
-        ]
+        logger.debug("Populating variables workspace. Search query: %s", search_query)
+        return populate_variables_workspace(
+            state.metadata.variables,
+            state.current_metadata_language,
+            search_query,
+        )
 
     @app.callback(
         Output(SECTION_WRAPPER_ID, "children"),
         Input("language-dropdown", "value"),
         Input("open-button", "n_clicks"),
         prevent_initial_call=True,
     )
     def callback_populate_dataset_workspace(
         language: str,
         n_clicks: int,
     ) -> list:
         """Create dataset workspace with sections."""
         update_global_language_state(SupportedLanguages(language))
-        logger.info("Populating new dataset workspace")
+        logger.debug("Populating dataset workspace")
         if n_clicks:
             return [
                 build_dataset_edit_section(
                     "Obligatorisk",
                     OBLIGATORY_EDITABLE_DATASET_METADATA,
                     state.current_metadata_language,
                     state.metadata.dataset,
```

### Comparing `ssb_datadoc-0.8.3/src/datadoc/frontend/callbacks/utils.py` & `ssb_datadoc-0.9.0/src/datadoc/frontend/callbacks/utils.py`

 * *Files identical despite different names*

### Comparing `ssb_datadoc-0.8.3/src/datadoc/frontend/callbacks/variables.py` & `ssb_datadoc-0.9.0/src/datadoc/frontend/callbacks/variables.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,25 +7,69 @@
 
 from pydantic import ValidationError
 
 from datadoc import state
 from datadoc.frontend.callbacks.utils import MetadataInputTypes
 from datadoc.frontend.callbacks.utils import find_existing_language_string
 from datadoc.frontend.callbacks.utils import parse_and_validate_dates
+from datadoc.frontend.components.builders import build_edit_section
+from datadoc.frontend.components.builders import build_ssb_accordion
 from datadoc.frontend.fields.display_variables import (
     MULTIPLE_LANGUAGE_VARIABLES_METADATA,
 )
+from datadoc.frontend.fields.display_variables import OBLIGATORY_VARIABLES_METADATA
+from datadoc.frontend.fields.display_variables import OPTIONAL_VARIABLES_METADATA
 from datadoc.frontend.fields.display_variables import VariableIdentifiers
 
 if TYPE_CHECKING:
+    from datadoc_model import model
     from datadoc_model.model import LanguageStringType
 
+    from datadoc.enums import SupportedLanguages
+
 logger = logging.getLogger(__name__)
 
 
+def populate_variables_workspace(
+    variables: list[model.Variable],
+    language: SupportedLanguages,
+    search_query: str,
+) -> list:
+    """Create variable workspace with accordions for variables.
+
+    Allows for filtering which variables are displayed via the search box.
+    """
+    return [
+        build_ssb_accordion(
+            variable.short_name or "",
+            {
+                "type": "variables-accordion",
+                "id": f"{variable.short_name}-{language.value}",  # Insert language into the ID to invalidate browser caches
+            },
+            variable.short_name or "",
+            children=[
+                build_edit_section(
+                    OBLIGATORY_VARIABLES_METADATA,
+                    "Obligatorisk",
+                    variable,
+                    language.value,
+                ),
+                build_edit_section(
+                    OPTIONAL_VARIABLES_METADATA,
+                    "Anbefalt",
+                    variable,
+                    language.value,
+                ),
+            ],
+        )
+        for variable in variables
+        if search_query in (variable.short_name or "")
+    ]
+
+
 def handle_multi_language_metadata(
     metadata_field: str,
     new_value: MetadataInputTypes | LanguageStringType,
     updated_row_id: str,
 ) -> MetadataInputTypes | LanguageStringType:
     """Handle updates to fields which support multiple languages."""
     if new_value is None:
```

### Comparing `ssb_datadoc-0.8.3/src/datadoc/frontend/components/builders.py` & `ssb_datadoc-0.9.0/src/datadoc/frontend/components/builders.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 
 
 class AlertTypes(Enum):
     """Types of alerts."""
 
     SUCCESS = auto()
     WARNING = auto()
+    ERROR = auto()
 
 
 @dataclass
 class AlertType:
     """Attributes of a concrete alert type."""
 
     alert_class_name: str
@@ -38,17 +39,21 @@
     @staticmethod
     def get_type(alert_type: AlertTypes) -> AlertType:
         """Get a concrete alert type based on the given enum values."""
         return ALERT_TYPES[alert_type]
 
 
 ALERT_TYPES = {
+    AlertTypes.ERROR: AlertType(
+        alert_class_name="ssb-dialog error",
+        color="danger",
+    ),
     AlertTypes.WARNING: AlertType(
         alert_class_name="ssb-dialog warning",
-        color="danger",
+        color="warning",
     ),
     AlertTypes.SUCCESS: AlertType(
         alert_class_name="ssb-dialog",
         color="success",
     ),
 }
 
@@ -69,14 +74,15 @@
     alert_type: AlertTypes,
     alert_identifier: str,
     title: str,
     content_identifier: str,
     message: str | None = None,
     *,
     start_open: bool = False,
+    link: str | None = None,
 ) -> dbc.Alert:
     """Make a Dash Alert according to SSBs Design System."""
     alert = AlertType.get_type(alert_type)
     return dbc.Alert(
         id=alert_identifier,
         is_open=start_open,
         dismissable=True,
@@ -87,14 +93,15 @@
             html.H5(
                 title,
             ),
             html.P(
                 id=content_identifier,
                 children=message,
             ),
+            html.A(link, href=link, target="_blank"),
         ],
         style={"width": "70%"},
     )
 
 
 def build_input_field_section(
     metadata_fields: list[VariablesFieldTypes],
```

### Comparing `ssb_datadoc-0.8.3/src/datadoc/frontend/components/control_bars.py` & `ssb_datadoc-0.9.0/src/datadoc/frontend/components/control_bars.py`

 * *Files identical despite different names*

### Comparing `ssb_datadoc-0.8.3/src/datadoc/frontend/components/dataset_tab.py` & `ssb_datadoc-0.9.0/src/datadoc/frontend/components/dataset_tab.py`

 * *Files identical despite different names*

### Comparing `ssb_datadoc-0.8.3/src/datadoc/frontend/components/variables_tab.py` & `ssb_datadoc-0.9.0/src/datadoc/frontend/components/variables_tab.py`

 * *Files 12% similar despite different names*

```diff
@@ -32,16 +32,16 @@
                         ssb.Paragraph(
                             id=VARIABLES_INFORMATION_ID,
                             className="workspace-info-paragraph",
                         ),
                         ssb.Input(
                             label="Søk i variabler",
                             searchField=True,
-                            disabled=True,
-                            placeholder="Kommer...",
+                            disabled=False,
+                            placeholder="Variabel kortnavn...",
                             id="search-variables",
                             n_submit=0,
                             value="",
                         ),
                     ],
                     className="workspace-header",
                 ),
```

### Comparing `ssb_datadoc-0.8.3/src/datadoc/frontend/fields/display_base.py` & `ssb_datadoc-0.9.0/src/datadoc/frontend/fields/display_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 import re
 import typing as t
 from dataclasses import dataclass
 from dataclasses import field
 from typing import TYPE_CHECKING
 from typing import Any
 
-import dash_bootstrap_components as dbc
 import ssb_dash_components as ssb
 from dash import dcc
 
 from datadoc import state
 from datadoc.enums import SupportedLanguages
 from datadoc.frontend.callbacks.utils import get_language_strings_enum
 
@@ -224,24 +223,24 @@
     value_getter: Callable[[BaseModel, str], Any] = get_standard_metadata
 
     def render(
         self,
         variable_id: dict,
         language: str,  # noqa: ARG002 Required by Dash
         variable: model.Variable,
-    ) -> dbc.Checkbox:
+    ) -> ssb.Checkbox:
         """Build Checkbox component."""
         value = self.value_getter(variable, self.identifier)
-        return dbc.Checkbox(
+        return ssb.Checkbox(
             label=self.display_name,
             id=variable_id,
             disabled=not self.editable,
-            label_class_name="ssb-checkbox checkbox-label",
-            class_name="ssb-checkbox",
             value=value,
+            showDescription=True,
+            description=self.description,
         )
 
 
 VariablesFieldTypes = (
     MetadataInputField
     | MetadataDropdownField
     | MetadataCheckboxField
```

### Comparing `ssb_datadoc-0.8.3/src/datadoc/frontend/fields/display_dataset.py` & `ssb_datadoc-0.9.0/src/datadoc/frontend/fields/display_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -252,14 +252,15 @@
     ),
     DatasetIdentifiers.FILE_PATH: MetadataInputField(
         identifier=DatasetIdentifiers.FILE_PATH.value,
         display_name="Filsti",
         description="Filstien inneholder datasettets navn og stien til hvor det er lagret.",
         obligatory=True,
         editable=False,
+        value_getter=get_metadata_and_stringify,
     ),
     DatasetIdentifiers.METADATA_CREATED_DATE: MetadataInputField(
         identifier=DatasetIdentifiers.METADATA_CREATED_DATE.value,
         display_name="Dato opprettet",
         description="Opprettet dato for metadata om datasettet",
         obligatory=True,
         editable=False,
```

### Comparing `ssb_datadoc-0.8.3/src/datadoc/frontend/fields/display_variables.py` & `ssb_datadoc-0.9.0/src/datadoc/frontend/fields/display_variables.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,15 @@
         url=True,
         obligatory=True,
         type="url",
     ),
     VariableIdentifiers.DIRECT_PERSON_IDENTIFYING: MetadataCheckboxField(
         identifier=VariableIdentifiers.DIRECT_PERSON_IDENTIFYING.value,
         display_name="Direkte personidentifiserende informasjon",
-        description="Direkte personidentifiserende informasjon (DPI)",
+        description="Velges hvis variabelen inneholder informasjon som innebærer at enkeltpersoner kan identifiseres. Gjelder ikke hvis kolonnen er pseudonymisert eller anonymisert.",
         obligatory=True,
     ),
     VariableIdentifiers.DATA_SOURCE: MetadataInputField(
         identifier=VariableIdentifiers.DATA_SOURCE.value,
         display_name="Datakilde",
         description="Datakilde. Settes på datasettnivå, men kan overstyres på variabelforekomstnivå.",
         multiple_language_support=True,
```

### Comparing `ssb_datadoc-0.8.3/src/datadoc/logging_configuration/json_formatter.py` & `ssb_datadoc-0.9.0/src/datadoc/logging_configuration/json_formatter.py`

 * *Files identical despite different names*

### Comparing `ssb_datadoc-0.8.3/src/datadoc/logging_configuration/logging_config.py` & `ssb_datadoc-0.9.0/src/datadoc/logging_configuration/logging_config.py`

 * *Files identical despite different names*

### Comparing `ssb_datadoc-0.8.3/src/datadoc/state.py` & `ssb_datadoc-0.9.0/src/datadoc/state.py`

 * *Files identical despite different names*

### Comparing `ssb_datadoc-0.8.3/src/datadoc/utils.py` & `ssb_datadoc-0.9.0/src/datadoc/utils.py`

 * *Files identical despite different names*

### Comparing `ssb_datadoc-0.8.3/PKG-INFO` & `ssb_datadoc-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssb-datadoc
-Version: 0.8.3
+Version: 0.9.0
 Summary: Document dataset metadata. For use in Statistics Norway's metadata system.
 Home-page: https://github.com/statisticsnorway/datadoc
 License: MIT
 Author: Statistics Norway
 Author-email: stat-dev@ssb.no
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
```

