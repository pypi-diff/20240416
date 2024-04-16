# Comparing `tmp/harlequin-1.9.1.tar.gz` & `tmp/harlequin-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "harlequin-1.9.1.tar", max compression
+gzip compressed data, was "harlequin-1.9.2.tar", max compression
```

## Comparing `harlequin-1.9.1.tar` & `harlequin-1.9.2.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0     1068 2024-01-09 20:26:53.749330 harlequin-1.9.1/LICENSE
--rw-r--r--   0        0        0     4116 2024-01-09 20:26:53.749330 harlequin-1.9.1/README.md
--rw-r--r--   0        0        0     3207 2024-01-09 20:26:53.749330 harlequin-1.9.1/pyproject.toml
--rw-r--r--   0        0        0      440 2024-01-09 20:26:53.749330 harlequin-1.9.1/src/harlequin/__init__.py
--rw-r--r--   0        0        0       49 2024-01-09 20:26:53.749330 harlequin-1.9.1/src/harlequin/__main__.py
--rw-r--r--   0        0        0     7238 2024-01-09 20:26:53.749330 harlequin-1.9.1/src/harlequin/adapter.py
--rw-r--r--   0        0        0    21289 2024-01-09 20:26:53.749330 harlequin-1.9.1/src/harlequin/app.py
--rw-r--r--   0        0        0      290 2024-01-09 20:26:53.749330 harlequin-1.9.1/src/harlequin/autocomplete/__init__.py
--rw-r--r--   0        0        0     6239 2024-01-09 20:26:53.753330 harlequin-1.9.1/src/harlequin/autocomplete/completers.py
--rw-r--r--   0        0        0     2092 2024-01-09 20:26:53.753330 harlequin-1.9.1/src/harlequin/autocomplete/completion.py
--rw-r--r--   0        0        0     2413 2024-01-09 20:26:53.753330 harlequin-1.9.1/src/harlequin/autocomplete/constants.py
--rw-r--r--   0        0        0     1452 2024-01-09 20:26:53.753330 harlequin-1.9.1/src/harlequin/cache.py
--rw-r--r--   0        0        0     1606 2024-01-09 20:26:53.753330 harlequin-1.9.1/src/harlequin/catalog.py
--rw-r--r--   0        0        0     9514 2024-01-09 20:26:53.753330 harlequin-1.9.1/src/harlequin/cli.py
--rw-r--r--   0        0        0     5811 2024-01-09 20:26:53.753330 harlequin-1.9.1/src/harlequin/colors.py
--rw-r--r--   0        0        0      637 2024-01-09 20:26:53.753330 harlequin-1.9.1/src/harlequin/components/__init__.py
--rw-r--r--   0        0        0     9574 2024-01-09 20:26:53.753330 harlequin-1.9.1/src/harlequin/components/code_editor.py
--rw-r--r--   0        0        0     4531 2024-01-09 20:26:53.753330 harlequin-1.9.1/src/harlequin/components/data_catalog.py
--rw-r--r--   0        0        0     1654 2024-01-09 20:26:53.753330 harlequin-1.9.1/src/harlequin/components/error_modal.py
--rw-r--r--   0        0        0     8713 2024-01-09 20:26:53.753330 harlequin-1.9.1/src/harlequin/components/export_screen.py
--rw-r--r--   0        0        0     3126 2024-01-09 20:26:53.753330 harlequin-1.9.1/src/harlequin/components/help_screen.md
--rw-r--r--   0        0        0     2000 2024-01-09 20:26:53.753330 harlequin-1.9.1/src/harlequin/components/help_screen.py
--rw-r--r--   0        0        0     5765 2024-01-09 20:26:53.753330 harlequin-1.9.1/src/harlequin/components/results_viewer.py
--rw-r--r--   0        0        0     2493 2024-01-09 20:26:53.753330 harlequin-1.9.1/src/harlequin/components/run_query_bar.py
--rw-r--r--   0        0        0     5387 2024-01-09 20:26:53.753330 harlequin-1.9.1/src/harlequin/config.py
--rw-r--r--   0        0        0     8239 2024-01-09 20:26:53.753330 harlequin-1.9.1/src/harlequin/config_wizard.py
--rw-r--r--   0        0        0      274 2024-01-09 20:26:53.753330 harlequin-1.9.1/src/harlequin/copy_widgets.py
--rw-r--r--   0        0        0      939 2024-01-09 20:26:53.753330 harlequin-1.9.1/src/harlequin/exception.py
--rw-r--r--   0        0        0     7807 2024-01-09 20:26:53.753330 harlequin-1.9.1/src/harlequin/global.tcss
--rw-r--r--   0        0        0    17716 2024-01-09 20:26:53.753330 harlequin-1.9.1/src/harlequin/options.py
--rw-r--r--   0        0        0      711 2024-01-09 20:26:53.753330 harlequin-1.9.1/src/harlequin/plugins.py
--rw-r--r--   0        0        0        0 2024-01-09 20:26:53.753330 harlequin-1.9.1/src/harlequin/py.typed
--rw-r--r--   0        0        0     3528 2024-01-09 20:26:53.753330 harlequin-1.9.1/src/harlequin/windows_timezone.py
--rw-r--r--   0        0        0      227 2024-01-09 20:26:53.753330 harlequin-1.9.1/src/harlequin_duckdb/__init__.py
--rw-r--r--   0        0        0    18260 2024-01-09 20:26:53.753330 harlequin-1.9.1/src/harlequin_duckdb/adapter.py
--rw-r--r--   0        0        0     2032 2024-01-09 20:26:53.753330 harlequin-1.9.1/src/harlequin_duckdb/cli_options.py
--rw-r--r--   0        0        0     2476 2024-01-09 20:26:53.753330 harlequin-1.9.1/src/harlequin_duckdb/completions.py
--rw-r--r--   0        0        0     4659 2024-01-09 20:26:53.753330 harlequin-1.9.1/src/harlequin_duckdb/copy_formats.py
--rw-r--r--   0        0        0        0 2024-01-09 20:26:53.753330 harlequin-1.9.1/src/harlequin_duckdb/py.typed
--rw-r--r--   0        0        0      160 2024-01-09 20:26:53.753330 harlequin-1.9.1/src/harlequin_sqlite/__init__.py
--rw-r--r--   0        0        0    10268 2024-01-09 20:26:53.753330 harlequin-1.9.1/src/harlequin_sqlite/adapter.py
--rw-r--r--   0        0        0     3766 2024-01-09 20:26:53.753330 harlequin-1.9.1/src/harlequin_sqlite/cli_options.py
--rw-r--r--   0        0        0     5270 2024-01-09 20:26:53.753330 harlequin-1.9.1/src/harlequin_sqlite/completions.py
--rw-r--r--   0        0        0        0 2024-01-09 20:26:53.753330 harlequin-1.9.1/src/harlequin_sqlite/py.typed
--rw-r--r--   0        0        0     6073 1970-01-01 00:00:00.000000 harlequin-1.9.1/setup.py
--rw-r--r--   0        0        0     5656 1970-01-01 00:00:00.000000 harlequin-1.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-01-10 20:44:10.814474 harlequin-1.9.2/LICENSE
+-rw-r--r--   0        0        0     4116 2024-01-10 20:44:10.814474 harlequin-1.9.2/README.md
+-rw-r--r--   0        0        0     3288 2024-01-10 20:44:10.814474 harlequin-1.9.2/pyproject.toml
+-rw-r--r--   0        0        0      440 2024-01-10 20:44:10.814474 harlequin-1.9.2/src/harlequin/__init__.py
+-rw-r--r--   0        0        0       49 2024-01-10 20:44:10.814474 harlequin-1.9.2/src/harlequin/__main__.py
+-rw-r--r--   0        0        0     7238 2024-01-10 20:44:10.814474 harlequin-1.9.2/src/harlequin/adapter.py
+-rw-r--r--   0        0        0    21289 2024-01-10 20:44:10.814474 harlequin-1.9.2/src/harlequin/app.py
+-rw-r--r--   0        0        0      290 2024-01-10 20:44:10.814474 harlequin-1.9.2/src/harlequin/autocomplete/__init__.py
+-rw-r--r--   0        0        0     6239 2024-01-10 20:44:10.814474 harlequin-1.9.2/src/harlequin/autocomplete/completers.py
+-rw-r--r--   0        0        0     2092 2024-01-10 20:44:10.814474 harlequin-1.9.2/src/harlequin/autocomplete/completion.py
+-rw-r--r--   0        0        0     2413 2024-01-10 20:44:10.814474 harlequin-1.9.2/src/harlequin/autocomplete/constants.py
+-rw-r--r--   0        0        0     1452 2024-01-10 20:44:10.814474 harlequin-1.9.2/src/harlequin/cache.py
+-rw-r--r--   0        0        0     1606 2024-01-10 20:44:10.814474 harlequin-1.9.2/src/harlequin/catalog.py
+-rw-r--r--   0        0        0     9514 2024-01-10 20:44:10.814474 harlequin-1.9.2/src/harlequin/cli.py
+-rw-r--r--   0        0        0     5811 2024-01-10 20:44:10.814474 harlequin-1.9.2/src/harlequin/colors.py
+-rw-r--r--   0        0        0      637 2024-01-10 20:44:10.814474 harlequin-1.9.2/src/harlequin/components/__init__.py
+-rw-r--r--   0        0        0     9574 2024-01-10 20:44:10.814474 harlequin-1.9.2/src/harlequin/components/code_editor.py
+-rw-r--r--   0        0        0     4531 2024-01-10 20:44:10.814474 harlequin-1.9.2/src/harlequin/components/data_catalog.py
+-rw-r--r--   0        0        0     1654 2024-01-10 20:44:10.814474 harlequin-1.9.2/src/harlequin/components/error_modal.py
+-rw-r--r--   0        0        0     8713 2024-01-10 20:44:10.814474 harlequin-1.9.2/src/harlequin/components/export_screen.py
+-rw-r--r--   0        0        0     3126 2024-01-10 20:44:10.814474 harlequin-1.9.2/src/harlequin/components/help_screen.md
+-rw-r--r--   0        0        0     2000 2024-01-10 20:44:10.814474 harlequin-1.9.2/src/harlequin/components/help_screen.py
+-rw-r--r--   0        0        0     5765 2024-01-10 20:44:10.814474 harlequin-1.9.2/src/harlequin/components/results_viewer.py
+-rw-r--r--   0        0        0     2493 2024-01-10 20:44:10.814474 harlequin-1.9.2/src/harlequin/components/run_query_bar.py
+-rw-r--r--   0        0        0     5387 2024-01-10 20:44:10.814474 harlequin-1.9.2/src/harlequin/config.py
+-rw-r--r--   0        0        0     8239 2024-01-10 20:44:10.814474 harlequin-1.9.2/src/harlequin/config_wizard.py
+-rw-r--r--   0        0        0      274 2024-01-10 20:44:10.814474 harlequin-1.9.2/src/harlequin/copy_widgets.py
+-rw-r--r--   0        0        0      939 2024-01-10 20:44:10.814474 harlequin-1.9.2/src/harlequin/exception.py
+-rw-r--r--   0        0        0     7807 2024-01-10 20:44:10.814474 harlequin-1.9.2/src/harlequin/global.tcss
+-rw-r--r--   0        0        0    17716 2024-01-10 20:44:10.814474 harlequin-1.9.2/src/harlequin/options.py
+-rw-r--r--   0        0        0      711 2024-01-10 20:44:10.814474 harlequin-1.9.2/src/harlequin/plugins.py
+-rw-r--r--   0        0        0        0 2024-01-10 20:44:10.814474 harlequin-1.9.2/src/harlequin/py.typed
+-rw-r--r--   0        0        0     3528 2024-01-10 20:44:10.814474 harlequin-1.9.2/src/harlequin/windows_timezone.py
+-rw-r--r--   0        0        0      227 2024-01-10 20:44:10.814474 harlequin-1.9.2/src/harlequin_duckdb/__init__.py
+-rw-r--r--   0        0        0    18260 2024-01-10 20:44:10.818474 harlequin-1.9.2/src/harlequin_duckdb/adapter.py
+-rw-r--r--   0        0        0     2032 2024-01-10 20:44:10.818474 harlequin-1.9.2/src/harlequin_duckdb/cli_options.py
+-rw-r--r--   0        0        0     2476 2024-01-10 20:44:10.818474 harlequin-1.9.2/src/harlequin_duckdb/completions.py
+-rw-r--r--   0        0        0     4659 2024-01-10 20:44:10.818474 harlequin-1.9.2/src/harlequin_duckdb/copy_formats.py
+-rw-r--r--   0        0        0        0 2024-01-10 20:44:10.818474 harlequin-1.9.2/src/harlequin_duckdb/py.typed
+-rw-r--r--   0        0        0      160 2024-01-10 20:44:10.818474 harlequin-1.9.2/src/harlequin_sqlite/__init__.py
+-rw-r--r--   0        0        0    10268 2024-01-10 20:44:10.818474 harlequin-1.9.2/src/harlequin_sqlite/adapter.py
+-rw-r--r--   0        0        0     3766 2024-01-10 20:44:10.818474 harlequin-1.9.2/src/harlequin_sqlite/cli_options.py
+-rw-r--r--   0        0        0     5270 2024-01-10 20:44:10.818474 harlequin-1.9.2/src/harlequin_sqlite/completions.py
+-rw-r--r--   0        0        0        0 2024-01-10 20:44:10.818474 harlequin-1.9.2/src/harlequin_sqlite/py.typed
+-rw-r--r--   0        0        0     6112 1970-01-01 00:00:00.000000 harlequin-1.9.2/setup.py
+-rw-r--r--   0        0        0     5737 1970-01-01 00:00:00.000000 harlequin-1.9.2/PKG-INFO
```

### Comparing `harlequin-1.9.1/LICENSE` & `harlequin-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `harlequin-1.9.1/README.md` & `harlequin-1.9.2/README.md`

 * *Files identical despite different names*

### Comparing `harlequin-1.9.1/pyproject.toml` & `harlequin-1.9.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "harlequin"
-version = "1.9.1"
+version = "1.9.2"
 description = "The SQL IDE for Your Terminal."
 authors = ["Ted Conbeer <tconbeer@users.noreply.github.com>"]
 license = "MIT"
 homepage = "https://harlequin.sh"
 repository = "https://github.com/tconbeer/harlequin"
 readme = "README.md"
 packages = [
@@ -38,14 +38,15 @@
 tomli = { version = "^2.0.1", python = "<3.11.0" }
 tomlkit = "^0.12.3"
 questionary = "^2.0.1"
 
 # database adapters (optional installs for extras)
 harlequin-postgres = { version = "^0.2", optional = true }
 harlequin-mysql = { version = "^0.1", optional = true }
+harlequin-odbc = { version = "^0.1", optional = true }
 harlequin-bigquery = { version = "^1.0", optional = true }
 harlequin-trino = { version = "^0.1", optional = true }
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.3.1"
 textual-dev = "^1.0.1"
 harlequin-postgres = "^0.2"
@@ -66,14 +67,15 @@
 
 [tool.poetry.scripts]
 harlequin = "harlequin.cli:harlequin"
 
 [tool.poetry.extras]
 postgres = ["harlequin-postgres"]
 mysql = ["harlequin-mysql"]
+odbc = ["harlequin-odbc"]
 bigquery = ["harlequin-bigquery"]
 trino = ["harlequin-trino"]
 
 [tool.poetry.plugins."harlequin.adapter"]
 duckdb = "harlequin_duckdb:DuckDbAdapter"
 sqlite = "harlequin_sqlite:HarlequinSqliteAdapter"
```

### Comparing `harlequin-1.9.1/src/harlequin/adapter.py` & `harlequin-1.9.2/src/harlequin/adapter.py`

 * *Files identical despite different names*

### Comparing `harlequin-1.9.1/src/harlequin/app.py` & `harlequin-1.9.2/src/harlequin/app.py`

 * *Files identical despite different names*

### Comparing `harlequin-1.9.1/src/harlequin/autocomplete/completers.py` & `harlequin-1.9.2/src/harlequin/autocomplete/completers.py`

 * *Files identical despite different names*

### Comparing `harlequin-1.9.1/src/harlequin/autocomplete/completion.py` & `harlequin-1.9.2/src/harlequin/autocomplete/completion.py`

 * *Files identical despite different names*

### Comparing `harlequin-1.9.1/src/harlequin/autocomplete/constants.py` & `harlequin-1.9.2/src/harlequin/autocomplete/constants.py`

 * *Files identical despite different names*

### Comparing `harlequin-1.9.1/src/harlequin/cache.py` & `harlequin-1.9.2/src/harlequin/cache.py`

 * *Files identical despite different names*

### Comparing `harlequin-1.9.1/src/harlequin/catalog.py` & `harlequin-1.9.2/src/harlequin/catalog.py`

 * *Files identical despite different names*

### Comparing `harlequin-1.9.1/src/harlequin/cli.py` & `harlequin-1.9.2/src/harlequin/cli.py`

 * *Files identical despite different names*

### Comparing `harlequin-1.9.1/src/harlequin/colors.py` & `harlequin-1.9.2/src/harlequin/colors.py`

 * *Files identical despite different names*

### Comparing `harlequin-1.9.1/src/harlequin/components/__init__.py` & `harlequin-1.9.2/src/harlequin/components/__init__.py`

 * *Files identical despite different names*

### Comparing `harlequin-1.9.1/src/harlequin/components/code_editor.py` & `harlequin-1.9.2/src/harlequin/components/code_editor.py`

 * *Files identical despite different names*

### Comparing `harlequin-1.9.1/src/harlequin/components/data_catalog.py` & `harlequin-1.9.2/src/harlequin/components/data_catalog.py`

 * *Files identical despite different names*

### Comparing `harlequin-1.9.1/src/harlequin/components/error_modal.py` & `harlequin-1.9.2/src/harlequin/components/error_modal.py`

 * *Files identical despite different names*

### Comparing `harlequin-1.9.1/src/harlequin/components/export_screen.py` & `harlequin-1.9.2/src/harlequin/components/export_screen.py`

 * *Files identical despite different names*

### Comparing `harlequin-1.9.1/src/harlequin/components/help_screen.md` & `harlequin-1.9.2/src/harlequin/components/help_screen.md`

 * *Files identical despite different names*

### Comparing `harlequin-1.9.1/src/harlequin/components/help_screen.py` & `harlequin-1.9.2/src/harlequin/components/help_screen.py`

 * *Files identical despite different names*

### Comparing `harlequin-1.9.1/src/harlequin/components/results_viewer.py` & `harlequin-1.9.2/src/harlequin/components/results_viewer.py`

 * *Files identical despite different names*

### Comparing `harlequin-1.9.1/src/harlequin/components/run_query_bar.py` & `harlequin-1.9.2/src/harlequin/components/run_query_bar.py`

 * *Files identical despite different names*

### Comparing `harlequin-1.9.1/src/harlequin/config.py` & `harlequin-1.9.2/src/harlequin/config.py`

 * *Files identical despite different names*

### Comparing `harlequin-1.9.1/src/harlequin/config_wizard.py` & `harlequin-1.9.2/src/harlequin/config_wizard.py`

 * *Files identical despite different names*

### Comparing `harlequin-1.9.1/src/harlequin/exception.py` & `harlequin-1.9.2/src/harlequin/exception.py`

 * *Files identical despite different names*

### Comparing `harlequin-1.9.1/src/harlequin/global.tcss` & `harlequin-1.9.2/src/harlequin/global.tcss`

 * *Files identical despite different names*

### Comparing `harlequin-1.9.1/src/harlequin/options.py` & `harlequin-1.9.2/src/harlequin/options.py`

 * *Files identical despite different names*

### Comparing `harlequin-1.9.1/src/harlequin/plugins.py` & `harlequin-1.9.2/src/harlequin/plugins.py`

 * *Files identical despite different names*

### Comparing `harlequin-1.9.1/src/harlequin/windows_timezone.py` & `harlequin-1.9.2/src/harlequin/windows_timezone.py`

 * *Files identical despite different names*

### Comparing `harlequin-1.9.1/src/harlequin_duckdb/adapter.py` & `harlequin-1.9.2/src/harlequin_duckdb/adapter.py`

 * *Files identical despite different names*

### Comparing `harlequin-1.9.1/src/harlequin_duckdb/cli_options.py` & `harlequin-1.9.2/src/harlequin_duckdb/cli_options.py`

 * *Files identical despite different names*

### Comparing `harlequin-1.9.1/src/harlequin_duckdb/completions.py` & `harlequin-1.9.2/src/harlequin_duckdb/completions.py`

 * *Files identical despite different names*

### Comparing `harlequin-1.9.1/src/harlequin_duckdb/copy_formats.py` & `harlequin-1.9.2/src/harlequin_duckdb/copy_formats.py`

 * *Files identical despite different names*

### Comparing `harlequin-1.9.1/src/harlequin_sqlite/adapter.py` & `harlequin-1.9.2/src/harlequin_sqlite/adapter.py`

 * *Files identical despite different names*

### Comparing `harlequin-1.9.1/src/harlequin_sqlite/cli_options.py` & `harlequin-1.9.2/src/harlequin_sqlite/cli_options.py`

 * *Files identical despite different names*

### Comparing `harlequin-1.9.1/src/harlequin_sqlite/completions.py` & `harlequin-1.9.2/src/harlequin_sqlite/completions.py`

 * *Files identical despite different names*

### Comparing `harlequin-1.9.1/setup.py` & `harlequin-1.9.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,26 +30,27 @@
  'tomlkit>=0.12.3,<0.13.0']
 
 extras_require = \
 {':python_full_version < "3.10.0"': ['importlib_metadata>=4.6.0'],
  ':python_full_version < "3.11.0"': ['tomli>=2.0.1,<3.0.0'],
  'bigquery': ['harlequin-bigquery>=1.0,<2.0'],
  'mysql': ['harlequin-mysql>=0.1,<0.2'],
+ 'odbc': ['harlequin-odbc>=0.1,<0.2'],
  'postgres': ['harlequin-postgres>=0.2,<0.3'],
  'trino': ['harlequin-trino>=0.1,<0.2']}
 
 entry_points = \
 {'console_scripts': ['harlequin = harlequin.cli:harlequin'],
  'harlequin.adapter': ['duckdb = harlequin_duckdb:DuckDbAdapter',
                        'sqlite = harlequin_sqlite:HarlequinSqliteAdapter'],
  'pygments.styles': ['harlequin = harlequin.colors:HarlequinPygmentsStyle']}
 
 setup_kwargs = {
     'name': 'harlequin',
-    'version': '1.9.1',
+    'version': '1.9.2',
     'description': 'The SQL IDE for Your Terminal.',
     'long_description': '# Harlequin\n\n[![PyPI](https://img.shields.io/pypi/v/harlequin)](https://pypi.org/project/harlequin/)\n\n![PyPI - Python Version](https://img.shields.io/pypi/pyversions/harlequin)\n![Runs on Linux | MacOS | Windows](https://img.shields.io/badge/runs%20on-Linux%20%7C%20MacOS%20%7C%20Windows-blue)\n\nThe SQL IDE for Your Terminal.\n\n![Harlequin](./harlequin.svg)\n\n## Installing Harlequin\n\nAfter installing Python 3.8 or above, install Harlequin using `pip` or `pipx` with:\n\n```bash\npipx install harlequin\n```\n\n## Using Harlequin with DuckDB\n\nFrom any shell, to open one or more DuckDB database files:\n\n```bash\nharlequin "path/to/duck.db" "another_duck.db"\n```\n\nTo open an in-memory DuckDB session, run Harlequin with no arguments:\n\n```bash\nharlequin\n```\n\nIf you want to control the version of DuckDB that Harlequin uses, see the [Troubleshooting](troubleshooting/duckdb-version-mismatch) page.\n\n## Using Harlequin with SQLite and Other Adapters\n\nHarlequin also ships with a SQLite3 adapter. You can open one or more SQLite database files with:\n\n```bash\nharlequin -a sqlite "path/to/sqlite.db" "another_sqlite.db"\n```\n\nLike DuckDB, you can also open an in-memory database by omitting the paths:\n\n```bash\nharlequin -a sqlite\n```\n\nOther adapters can be installed using `pip install <adapter package>` or `pipx inject harlequin <adapter package>`, depending on how you installed Harlequin. For a list of known adapters provided either by the Harlequin maintainers or the broader community, see the [adapters](https://harlequin.sh/docs/adapters) page in the docs.\n\n## Getting Help\n\nTo view all command-line options for Harlequin and all installed adapters, after installation, simply type:\n\n```bash\nharlequin --help\n```\n\nTo view a list of all key bindings (keyboard shortcuts) within the app, press <Key>F1</Key>. You can also view this list outside the app [in the docs](https://harlequin.sh/docs/bindings).\n\n## More info at [harlequin.sh](https://harlequin.sh)\n\nVisit [harlequin.sh](https://harlequin.sh) for an overview of features and full documentation.\n\n## Contributing\n\nThanks for your interest in Harlequin! Harlequin is primarily maintained by [Ted Conbeer](https://github.com/tconbeer), but he welcomes all contributions and is looking for additional maintainers!\n\n### Providing Feedback\n\nWe\'d love to hear from you! [Open an Issue](https://github.com/tconbeer/harlequin/issues/new) to request new features, report bugs, or say hello.\n\n### Setting up Your Dev Environment and Running Tests\n\n1. Install Poetry v1.2 or higher if you don\'t have it already. You may also need or want pyenv, make, and gcc.\n1. Fork this repo, and then clone the fork into a directory (let\'s call it `harlequin`), then `cd harlequin`.\n1. Use `poetry install --sync` to install the project (editable) and its dependencies (including all test and dev dependencies) into a new virtual env.\n1. Use `poetry shell` to spawn a subshell.\n1. Type `make` to run all tests and linters, or run `pytest`, `black .`, `ruff . --fix`, and `mypy` individually.\n\n### Opening PRs\n\n1. PRs should be motivated by an open issue. If there isn\'t already an issue describing the feature or bug, [open one](https://github.com/tconbeer/harlequin/issues/new). Do this before you write code, so you don\'t waste time on something that won\'t get merged.\n2. Ideally new features and bug fixes would be tested, to prevent future regressions. Textual provides a test harness that we use to test features of Harlequin. You can find some examples in the `tests` directory of this project. Please include a test in your PR, but if you can\'t figure it out, open a PR to ask for help.\n2. Open a PR from your fork to the `main` branch of `tconbeer/harlequin`. In the PR description, link to the open issue, and then write a few sentences about **why** you wrote the code you did: explain your design, etc.\n3. Ted may ask you to make changes, or he may make them for you. Don\'t take this the wrong way -- he values your contributions, but he knows this isn\'t your job, either, so if it\'s faster for him, he may push a commit to your branch or create a new branch from your commits.\n',
     'author': 'Ted Conbeer',
     'author_email': 'tconbeer@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://harlequin.sh',
```

### Comparing `harlequin-1.9.1/PKG-INFO` & `harlequin-1.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 Metadata-Version: 2.1
 Name: harlequin
-Version: 1.9.1
+Version: 1.9.2
 Summary: The SQL IDE for Your Terminal.
 Home-page: https://harlequin.sh
 License: MIT
 Author: Ted Conbeer
 Author-email: tconbeer@users.noreply.github.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: bigquery
 Provides-Extra: mysql
+Provides-Extra: odbc
 Provides-Extra: postgres
 Provides-Extra: trino
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: duckdb (>=0.8.0)
 Requires-Dist: harlequin-bigquery (>=1.0,<2.0); extra == "bigquery"
 Requires-Dist: harlequin-mysql (>=0.1,<0.2); extra == "mysql"
+Requires-Dist: harlequin-odbc (>=0.1,<0.2); extra == "odbc"
 Requires-Dist: harlequin-postgres (>=0.2,<0.3); extra == "postgres"
 Requires-Dist: harlequin-trino (>=0.1,<0.2); extra == "trino"
 Requires-Dist: importlib_metadata (>=4.6.0); python_full_version < "3.10.0"
 Requires-Dist: platformdirs (>=3.10,<5.0)
 Requires-Dist: pyperclip (>=1.8.2,<2.0.0)
 Requires-Dist: questionary (>=2.0.1,<3.0.0)
 Requires-Dist: rich-click (>=1.7.1,<2.0.0)
```

