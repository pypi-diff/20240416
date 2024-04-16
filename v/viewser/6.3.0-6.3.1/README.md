# Comparing `tmp/viewser-6.3.0.tar.gz` & `tmp/viewser-6.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viewser-6.3.0.tar", max compression
+gzip compressed data, was "viewser-6.3.1.tar", max compression
```

## Comparing `viewser-6.3.0.tar` & `viewser-6.3.1.tar`

### file list

```diff
@@ -1,75 +1,75 @@
--rw-r--r--   0        0        0    19916 2024-03-28 13:41:16.638842 viewser-6.3.0/LICENSE
--rw-r--r--   0        0        0    16723 2024-03-28 13:41:16.638842 viewser-6.3.0/README.md
--rw-r--r--   0        0        0      878 2024-03-28 13:41:16.642842 viewser-6.3.0/pyproject.toml
--rw-r--r--   0        0        0       79 2024-03-28 13:41:16.642842 viewser-6.3.0/viewser/__init__.py
--rw-r--r--   0        0        0     1779 2024-03-28 13:41:16.642842 viewser-6.3.0/viewser/cli.py
--rw-r--r--   0        0        0        0 2024-03-28 13:41:16.642842 viewser-6.3.0/viewser/commands/__init__.py
--rw-r--r--   0        0        0       22 2024-03-28 13:41:16.642842 viewser-6.3.0/viewser/commands/config/__init__.py
--rw-r--r--   0        0        0     3184 2024-03-28 13:41:16.642842 viewser-6.3.0/viewser/commands/config/cli.py
--rw-r--r--   0        0        0       61 2024-03-28 13:41:16.642842 viewser-6.3.0/viewser/commands/documentation/__init__.py
--rw-r--r--   0        0        0     3497 2024-03-28 13:41:16.642842 viewser-6.3.0/viewser/commands/documentation/cli.py
--rw-r--r--   0        0        0     3484 2024-03-28 13:41:16.642842 viewser-6.3.0/viewser/commands/documentation/formatting.py
--rw-r--r--   0        0        0     2070 2024-03-28 13:41:16.642842 viewser-6.3.0/viewser/commands/documentation/operations.py
--rw-r--r--   0        0        0      909 2024-03-28 13:41:16.642842 viewser-6.3.0/viewser/commands/documentation/wrapped_views_doc.py
--rw-r--r--   0        0        0       21 2024-03-28 13:41:16.642842 viewser-6.3.0/viewser/commands/help/__init__.py
--rw-r--r--   0        0        0      790 2024-03-28 13:41:16.642842 viewser-6.3.0/viewser/commands/help/cli.py
--rw-r--r--   0        0        0      242 2024-03-28 13:41:16.642842 viewser-6.3.0/viewser/commands/help/operations.py
--rw-r--r--   0        0        0       22 2024-03-28 13:41:16.642842 viewser-6.3.0/viewser/commands/logs/__init__.py
--rw-r--r--   0        0        0      393 2024-03-28 13:41:16.642842 viewser-6.3.0/viewser/commands/logs/cli.py
--rw-r--r--   0        0        0       22 2024-03-28 13:41:16.642842 viewser-6.3.0/viewser/commands/model/__init__.py
--rw-r--r--   0        0        0     3531 2024-03-28 13:41:16.642842 viewser-6.3.0/viewser/commands/model/cli.py
--rw-r--r--   0        0        0      731 2024-03-28 13:41:16.642842 viewser-6.3.0/viewser/commands/model/formatting.py
--rw-r--r--   0        0        0        1 2024-03-28 13:41:16.642842 viewser-6.3.0/viewser/commands/model/models.py
--rw-r--r--   0        0        0       22 2024-03-28 13:41:16.642842 viewser-6.3.0/viewser/commands/notebooks/__init__.py
--rw-r--r--   0        0        0     1766 2024-03-28 13:41:16.642842 viewser-6.3.0/viewser/commands/notebooks/cli.py
--rw-r--r--   0        0        0     6167 2024-03-28 13:41:16.642842 viewser-6.3.0/viewser/commands/notebooks/operations.py
--rw-r--r--   0        0        0       60 2024-03-28 13:41:16.642842 viewser-6.3.0/viewser/commands/queryset/__init__.py
--rw-r--r--   0        0        0     2265 2024-03-28 13:41:16.642842 viewser-6.3.0/viewser/commands/queryset/cli.py
--rw-r--r--   0        0        0     1269 2024-03-28 13:41:16.642842 viewser-6.3.0/viewser/commands/queryset/formatting.py
--rw-r--r--   0        0        0      133 2024-03-28 13:41:16.642842 viewser-6.3.0/viewser/commands/queryset/models/__init__.py
--rw-r--r--   0        0        0     3059 2024-03-28 13:41:16.642842 viewser-6.3.0/viewser/commands/queryset/models/column.py
--rw-r--r--   0        0        0     6068 2024-03-28 13:41:16.642842 viewser-6.3.0/viewser/commands/queryset/models/queryset.py
--rw-r--r--   0        0        0     2285 2024-03-28 13:41:16.642842 viewser-6.3.0/viewser/commands/queryset/models/transform.py
--rw-r--r--   0        0        0      313 2024-03-28 13:41:16.642842 viewser-6.3.0/viewser/commands/queryset/models/util.py
--rw-r--r--   0        0        0     4909 2024-03-28 13:41:16.642842 viewser-6.3.0/viewser/commands/queryset/operations.py
--rw-r--r--   0        0        0      231 2024-03-28 13:41:16.642842 viewser-6.3.0/viewser/commands/queryset/queryset_list.py
--rw-r--r--   0        0        0       22 2024-03-28 13:41:16.642842 viewser-6.3.0/viewser/commands/system/__init__.py
--rw-r--r--   0        0        0     1816 2024-03-28 13:41:16.642842 viewser-6.3.0/viewser/commands/system/cli.py
--rw-r--r--   0        0        0     1371 2024-03-28 13:41:16.642842 viewser-6.3.0/viewser/commands/system/formatting.py
--rw-r--r--   0        0        0      481 2024-03-28 13:41:16.642842 viewser-6.3.0/viewser/commands/system/models.py
--rw-r--r--   0        0        0       73 2024-03-28 13:41:16.642842 viewser-6.3.0/viewser/error_handling/__init__.py
--rw-r--r--   0        0        0     3929 2024-03-28 13:41:16.642842 viewser-6.3.0/viewser/error_handling/checks.py
--rw-r--r--   0        0        0     2164 2024-03-28 13:41:16.642842 viewser-6.3.0/viewser/error_handling/error_handling.py
--rw-r--r--   0        0        0     7304 2024-03-28 13:41:16.646842 viewser-6.3.0/viewser/error_handling/errors.py
--rw-r--r--   0        0        0     6252 2024-03-28 13:41:16.646842 viewser-6.3.0/viewser/error_handling/exceptions.py
--rw-r--r--   0        0        0      205 2024-03-28 13:41:16.646842 viewser-6.3.0/viewser/hirearchical_dict.py
--rw-r--r--   0        0        0      706 2024-03-28 13:41:16.646842 viewser-6.3.0/viewser/operations.py
--rw-r--r--   0        0        0     5859 2024-03-28 13:41:16.646842 viewser-6.3.0/viewser/remotes.py
--rw-r--r--   0        0        0      868 2024-03-28 13:41:16.646842 viewser-6.3.0/viewser/settings/__init__.py
--rw-r--r--   0        0        0     4168 2024-03-28 13:41:16.646842 viewser-6.3.0/viewser/settings/config_resolver.py
--rw-r--r--   0        0        0      182 2024-03-28 13:41:16.646842 viewser-6.3.0/viewser/settings/db.py
--rw-r--r--   0        0        0      295 2024-03-28 13:41:16.646842 viewser-6.3.0/viewser/settings/defaults.py
--rw-r--r--   0        0        0       47 2024-03-28 13:41:16.646842 viewser-6.3.0/viewser/settings/exceptions.py
--rw-r--r--   0        0        0        1 2024-03-28 13:41:16.646842 viewser-6.3.0/viewser/settings/interactive.py
--rw-r--r--   0        0        0      389 2024-03-28 13:41:16.646842 viewser-6.3.0/viewser/settings/models.py
--rw-r--r--   0        0        0     1401 2024-03-28 13:41:16.646842 viewser-6.3.0/viewser/settings/static.py
--rw-r--r--   0        0        0      181 2024-03-28 13:41:16.646842 viewser-6.3.0/viewser/settings/validation.py
--rw-r--r--   0        0        0      387 2024-03-28 13:41:16.646842 viewser-6.3.0/viewser/storage/azure.py
--rw-r--r--   0        0        0     2443 2024-03-28 13:41:16.646842 viewser-6.3.0/viewser/storage/db.py
--rw-r--r--   0        0        0     1462 2024-03-28 13:41:16.646842 viewser-6.3.0/viewser/storage/metadata_storage_serializer.py
--rw-r--r--   0        0        0     1175 2024-03-28 13:41:16.646842 viewser-6.3.0/viewser/storage/model_object.py
--rw-r--r--   0        0        0        0 2024-03-28 13:41:16.646842 viewser-6.3.0/viewser/tui/__init__.py
--rw-r--r--   0        0        0      842 2024-03-28 13:41:16.646842 viewser-6.3.0/viewser/tui/animations.py
--rw-r--r--   0        0        0      322 2024-03-28 13:41:16.646842 viewser-6.3.0/viewser/tui/ascii_art.py
--rw-r--r--   0        0        0        0 2024-03-28 13:41:16.646842 viewser-6.3.0/viewser/tui/formatting/__init__.py
--rw-r--r--   0        0        0     3186 2024-03-28 13:41:16.646842 viewser-6.3.0/viewser/tui/formatting/abc.py
--rw-r--r--   0        0        0      144 2024-03-28 13:41:16.646842 viewser-6.3.0/viewser/tui/formatting/conventions.py
--rw-r--r--   0        0        0      830 2024-03-28 13:41:16.646842 viewser-6.3.0/viewser/tui/formatting/errors.py
--rw-r--r--   0        0        0      291 2024-03-28 13:41:16.646842 viewser-6.3.0/viewser/tui/formatting/formatters.py
--rw-r--r--   0        0        0      177 2024-03-28 13:41:16.646842 viewser-6.3.0/viewser/tui/formatting/generic_models.py
--rw-r--r--   0        0        0      196 2024-03-28 13:41:16.646842 viewser-6.3.0/viewser/tui/formatting/json_formatter.py
--rw-r--r--   0        0        0      443 2024-03-28 13:41:16.646842 viewser-6.3.0/viewser/tui/formatting/sections.py
--rw-r--r--   0        0        0      103 2024-03-28 13:41:16.646842 viewser-6.3.0/viewser/tui/formatting/styles.py
--rw-r--r--   0        0        0       32 2024-03-28 13:41:16.646842 viewser-6.3.0/viewser/tui/models.py
--rw-r--r--   0        0        0       82 2024-03-28 13:41:16.646842 viewser-6.3.0/viewser/tui/utils.py
--rw-r--r--   0        0        0    18058 1970-01-01 00:00:00.000000 viewser-6.3.0/PKG-INFO
+-rw-r--r--   0        0        0    19916 2024-04-15 14:38:22.693468 viewser-6.3.1/LICENSE
+-rw-r--r--   0        0        0    16854 2024-04-15 14:38:22.693468 viewser-6.3.1/README.md
+-rw-r--r--   0        0        0      878 2024-04-15 14:38:22.693468 viewser-6.3.1/pyproject.toml
+-rw-r--r--   0        0        0       79 2024-04-15 14:38:22.693468 viewser-6.3.1/viewser/__init__.py
+-rw-r--r--   0        0        0     1779 2024-04-15 14:38:22.693468 viewser-6.3.1/viewser/cli.py
+-rw-r--r--   0        0        0        0 2024-04-15 14:38:22.693468 viewser-6.3.1/viewser/commands/__init__.py
+-rw-r--r--   0        0        0       22 2024-04-15 14:38:22.693468 viewser-6.3.1/viewser/commands/config/__init__.py
+-rw-r--r--   0        0        0     3184 2024-04-15 14:38:22.693468 viewser-6.3.1/viewser/commands/config/cli.py
+-rw-r--r--   0        0        0       61 2024-04-15 14:38:22.693468 viewser-6.3.1/viewser/commands/documentation/__init__.py
+-rw-r--r--   0        0        0     3497 2024-04-15 14:38:22.693468 viewser-6.3.1/viewser/commands/documentation/cli.py
+-rw-r--r--   0        0        0     3484 2024-04-15 14:38:22.693468 viewser-6.3.1/viewser/commands/documentation/formatting.py
+-rw-r--r--   0        0        0     2070 2024-04-15 14:38:22.693468 viewser-6.3.1/viewser/commands/documentation/operations.py
+-rw-r--r--   0        0        0      909 2024-04-15 14:38:22.693468 viewser-6.3.1/viewser/commands/documentation/wrapped_views_doc.py
+-rw-r--r--   0        0        0       21 2024-04-15 14:38:22.693468 viewser-6.3.1/viewser/commands/help/__init__.py
+-rw-r--r--   0        0        0      790 2024-04-15 14:38:22.693468 viewser-6.3.1/viewser/commands/help/cli.py
+-rw-r--r--   0        0        0      242 2024-04-15 14:38:22.693468 viewser-6.3.1/viewser/commands/help/operations.py
+-rw-r--r--   0        0        0       22 2024-04-15 14:38:22.697468 viewser-6.3.1/viewser/commands/logs/__init__.py
+-rw-r--r--   0        0        0      393 2024-04-15 14:38:22.697468 viewser-6.3.1/viewser/commands/logs/cli.py
+-rw-r--r--   0        0        0       22 2024-04-15 14:38:22.697468 viewser-6.3.1/viewser/commands/model/__init__.py
+-rw-r--r--   0        0        0     3531 2024-04-15 14:38:22.697468 viewser-6.3.1/viewser/commands/model/cli.py
+-rw-r--r--   0        0        0      731 2024-04-15 14:38:22.697468 viewser-6.3.1/viewser/commands/model/formatting.py
+-rw-r--r--   0        0        0        1 2024-04-15 14:38:22.697468 viewser-6.3.1/viewser/commands/model/models.py
+-rw-r--r--   0        0        0       22 2024-04-15 14:38:22.697468 viewser-6.3.1/viewser/commands/notebooks/__init__.py
+-rw-r--r--   0        0        0     1766 2024-04-15 14:38:22.697468 viewser-6.3.1/viewser/commands/notebooks/cli.py
+-rw-r--r--   0        0        0     6167 2024-04-15 14:38:22.697468 viewser-6.3.1/viewser/commands/notebooks/operations.py
+-rw-r--r--   0        0        0       60 2024-04-15 14:38:22.697468 viewser-6.3.1/viewser/commands/queryset/__init__.py
+-rw-r--r--   0        0        0     2265 2024-04-15 14:38:22.697468 viewser-6.3.1/viewser/commands/queryset/cli.py
+-rw-r--r--   0        0        0     1269 2024-04-15 14:38:22.697468 viewser-6.3.1/viewser/commands/queryset/formatting.py
+-rw-r--r--   0        0        0      133 2024-04-15 14:38:22.697468 viewser-6.3.1/viewser/commands/queryset/models/__init__.py
+-rw-r--r--   0        0        0     3059 2024-04-15 14:38:22.697468 viewser-6.3.1/viewser/commands/queryset/models/column.py
+-rw-r--r--   0        0        0     6068 2024-04-15 14:38:22.697468 viewser-6.3.1/viewser/commands/queryset/models/queryset.py
+-rw-r--r--   0        0        0     2285 2024-04-15 14:38:22.697468 viewser-6.3.1/viewser/commands/queryset/models/transform.py
+-rw-r--r--   0        0        0      313 2024-04-15 14:38:22.697468 viewser-6.3.1/viewser/commands/queryset/models/util.py
+-rw-r--r--   0        0        0     4913 2024-04-15 14:38:22.697468 viewser-6.3.1/viewser/commands/queryset/operations.py
+-rw-r--r--   0        0        0      231 2024-04-15 14:38:22.697468 viewser-6.3.1/viewser/commands/queryset/queryset_list.py
+-rw-r--r--   0        0        0       22 2024-04-15 14:38:22.697468 viewser-6.3.1/viewser/commands/system/__init__.py
+-rw-r--r--   0        0        0     1816 2024-04-15 14:38:22.697468 viewser-6.3.1/viewser/commands/system/cli.py
+-rw-r--r--   0        0        0     1371 2024-04-15 14:38:22.697468 viewser-6.3.1/viewser/commands/system/formatting.py
+-rw-r--r--   0        0        0      481 2024-04-15 14:38:22.697468 viewser-6.3.1/viewser/commands/system/models.py
+-rw-r--r--   0        0        0       73 2024-04-15 14:38:22.697468 viewser-6.3.1/viewser/error_handling/__init__.py
+-rw-r--r--   0        0        0     3929 2024-04-15 14:38:22.697468 viewser-6.3.1/viewser/error_handling/checks.py
+-rw-r--r--   0        0        0     2164 2024-04-15 14:38:22.697468 viewser-6.3.1/viewser/error_handling/error_handling.py
+-rw-r--r--   0        0        0     7304 2024-04-15 14:38:22.697468 viewser-6.3.1/viewser/error_handling/errors.py
+-rw-r--r--   0        0        0     6252 2024-04-15 14:38:22.697468 viewser-6.3.1/viewser/error_handling/exceptions.py
+-rw-r--r--   0        0        0      205 2024-04-15 14:38:22.697468 viewser-6.3.1/viewser/hirearchical_dict.py
+-rw-r--r--   0        0        0      706 2024-04-15 14:38:22.697468 viewser-6.3.1/viewser/operations.py
+-rw-r--r--   0        0        0     5859 2024-04-15 14:38:22.697468 viewser-6.3.1/viewser/remotes.py
+-rw-r--r--   0        0        0      868 2024-04-15 14:38:22.697468 viewser-6.3.1/viewser/settings/__init__.py
+-rw-r--r--   0        0        0     4168 2024-04-15 14:38:22.697468 viewser-6.3.1/viewser/settings/config_resolver.py
+-rw-r--r--   0        0        0      182 2024-04-15 14:38:22.697468 viewser-6.3.1/viewser/settings/db.py
+-rw-r--r--   0        0        0      295 2024-04-15 14:38:22.697468 viewser-6.3.1/viewser/settings/defaults.py
+-rw-r--r--   0        0        0       47 2024-04-15 14:38:22.697468 viewser-6.3.1/viewser/settings/exceptions.py
+-rw-r--r--   0        0        0        1 2024-04-15 14:38:22.697468 viewser-6.3.1/viewser/settings/interactive.py
+-rw-r--r--   0        0        0      389 2024-04-15 14:38:22.697468 viewser-6.3.1/viewser/settings/models.py
+-rw-r--r--   0        0        0     1401 2024-04-15 14:38:22.697468 viewser-6.3.1/viewser/settings/static.py
+-rw-r--r--   0        0        0      181 2024-04-15 14:38:22.697468 viewser-6.3.1/viewser/settings/validation.py
+-rw-r--r--   0        0        0      387 2024-04-15 14:38:22.697468 viewser-6.3.1/viewser/storage/azure.py
+-rw-r--r--   0        0        0     2443 2024-04-15 14:38:22.697468 viewser-6.3.1/viewser/storage/db.py
+-rw-r--r--   0        0        0     1462 2024-04-15 14:38:22.697468 viewser-6.3.1/viewser/storage/metadata_storage_serializer.py
+-rw-r--r--   0        0        0     1175 2024-04-15 14:38:22.697468 viewser-6.3.1/viewser/storage/model_object.py
+-rw-r--r--   0        0        0        0 2024-04-15 14:38:22.697468 viewser-6.3.1/viewser/tui/__init__.py
+-rw-r--r--   0        0        0      842 2024-04-15 14:38:22.697468 viewser-6.3.1/viewser/tui/animations.py
+-rw-r--r--   0        0        0      322 2024-04-15 14:38:22.697468 viewser-6.3.1/viewser/tui/ascii_art.py
+-rw-r--r--   0        0        0        0 2024-04-15 14:38:22.697468 viewser-6.3.1/viewser/tui/formatting/__init__.py
+-rw-r--r--   0        0        0     3186 2024-04-15 14:38:22.697468 viewser-6.3.1/viewser/tui/formatting/abc.py
+-rw-r--r--   0        0        0      144 2024-04-15 14:38:22.697468 viewser-6.3.1/viewser/tui/formatting/conventions.py
+-rw-r--r--   0        0        0      830 2024-04-15 14:38:22.697468 viewser-6.3.1/viewser/tui/formatting/errors.py
+-rw-r--r--   0        0        0      291 2024-04-15 14:38:22.697468 viewser-6.3.1/viewser/tui/formatting/formatters.py
+-rw-r--r--   0        0        0      177 2024-04-15 14:38:22.701468 viewser-6.3.1/viewser/tui/formatting/generic_models.py
+-rw-r--r--   0        0        0      196 2024-04-15 14:38:22.701468 viewser-6.3.1/viewser/tui/formatting/json_formatter.py
+-rw-r--r--   0        0        0      443 2024-04-15 14:38:22.701468 viewser-6.3.1/viewser/tui/formatting/sections.py
+-rw-r--r--   0        0        0      103 2024-04-15 14:38:22.701468 viewser-6.3.1/viewser/tui/formatting/styles.py
+-rw-r--r--   0        0        0       32 2024-04-15 14:38:22.701468 viewser-6.3.1/viewser/tui/models.py
+-rw-r--r--   0        0        0       82 2024-04-15 14:38:22.701468 viewser-6.3.1/viewser/tui/utils.py
+-rw-r--r--   0        0        0    18189 1970-01-01 00:00:00.000000 viewser-6.3.1/PKG-INFO
```

### Comparing `viewser-6.3.0/LICENSE` & `viewser-6.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `viewser-6.3.0/README.md` & `viewser-6.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -50,31 +50,33 @@
 `viewser` functionality is exposed via a CLI on your system after installation.
 An overview of available commands can be seen by running `viewser --help`.
 
 The CLI is envisaged mainly as a tool to help users with issues such as selecting appropriate transforms, exploring the database, determining the level of analysis of a given feature, etc.
 
 ## Useful commands
 
-Show all tables in the database:
+Show all features in the database:
 
-`viewser tables list` 
+`viewser features list <loa>`
 
-Show columns in a particular table:
-
-`viewser tables show table-name`
+with <loa> being one of ['pgm', 'cm', 'pgy', 'cy', 'pg', 'c', 'am', 'a', 'ay', 'm', 'y']
 
 Show all transforms sorted by level of analysis:
 
 `viewser transforms list`
 
-Show docstring for a particular transform:
+Show all transforms available at a particular level of analysis:
+
+`viewser transforms at_loa <loa>`
 
-`viewser transforms show transform-name`
+with <loa> being one of ['any', 'country_month', 'priogrid_month', 'priogrid_year']
+
+Show docstring for a particular transform:
 
-(note that the transform name should be the full name, e.g. 'any/temporal.entropy')
+`viewser transforms show <transform-name>`
 
 ## Via API
 
 The full functionality of viewser is exposed via its API for use in scripts and notebooks
 
 The two fundamental objects used to define what data is fetched by the client are the *Queryset* and the *Column*, where a 
 Queryset consists of one or more Columns.
```

### Comparing `viewser-6.3.0/pyproject.toml` & `viewser-6.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "viewser"
-version = "6.3.0"
+version = "6.3.1"
 description = "The Views 3 CLI tool"
 authors = ["peder2911 <pglandsverk@gmail.com>"]
 readme = "README.md"
 homepage = "https://www.github.com/prio-data/viewser"
 license = "CC-BY-NC"
 
 [tool.poetry.dependencies]
```

### Comparing `viewser-6.3.0/viewser/cli.py` & `viewser-6.3.1/viewser/cli.py`

 * *Files identical despite different names*

### Comparing `viewser-6.3.0/viewser/commands/config/cli.py` & `viewser-6.3.1/viewser/commands/config/cli.py`

 * *Files identical despite different names*

### Comparing `viewser-6.3.0/viewser/commands/documentation/cli.py` & `viewser-6.3.1/viewser/commands/documentation/cli.py`

 * *Files identical despite different names*

### Comparing `viewser-6.3.0/viewser/commands/documentation/formatting.py` & `viewser-6.3.1/viewser/commands/documentation/formatting.py`

 * *Files identical despite different names*

### Comparing `viewser-6.3.0/viewser/commands/documentation/operations.py` & `viewser-6.3.1/viewser/commands/documentation/operations.py`

 * *Files identical despite different names*

### Comparing `viewser-6.3.0/viewser/commands/documentation/wrapped_views_doc.py` & `viewser-6.3.1/viewser/commands/documentation/wrapped_views_doc.py`

 * *Files identical despite different names*

### Comparing `viewser-6.3.0/viewser/commands/help/cli.py` & `viewser-6.3.1/viewser/commands/help/cli.py`

 * *Files identical despite different names*

### Comparing `viewser-6.3.0/viewser/commands/model/cli.py` & `viewser-6.3.1/viewser/commands/model/cli.py`

 * *Files identical despite different names*

### Comparing `viewser-6.3.0/viewser/commands/model/formatting.py` & `viewser-6.3.1/viewser/commands/model/formatting.py`

 * *Files identical despite different names*

### Comparing `viewser-6.3.0/viewser/commands/notebooks/cli.py` & `viewser-6.3.1/viewser/commands/notebooks/cli.py`

 * *Files identical despite different names*

### Comparing `viewser-6.3.0/viewser/commands/notebooks/operations.py` & `viewser-6.3.1/viewser/commands/notebooks/operations.py`

 * *Files identical despite different names*

### Comparing `viewser-6.3.0/viewser/commands/queryset/cli.py` & `viewser-6.3.1/viewser/commands/queryset/cli.py`

 * *Files identical despite different names*

### Comparing `viewser-6.3.0/viewser/commands/queryset/formatting.py` & `viewser-6.3.1/viewser/commands/queryset/formatting.py`

 * *Files identical despite different names*

### Comparing `viewser-6.3.0/viewser/commands/queryset/models/column.py` & `viewser-6.3.1/viewser/commands/queryset/models/column.py`

 * *Files identical despite different names*

### Comparing `viewser-6.3.0/viewser/commands/queryset/models/queryset.py` & `viewser-6.3.1/viewser/commands/queryset/models/queryset.py`

 * *Files identical despite different names*

### Comparing `viewser-6.3.0/viewser/commands/queryset/models/transform.py` & `viewser-6.3.1/viewser/commands/queryset/models/transform.py`

 * *Files identical despite different names*

### Comparing `viewser-6.3.0/viewser/commands/queryset/operations.py` & `viewser-6.3.1/viewser/commands/queryset/operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,27 +62,29 @@
         ====
 
         returns:
             Optional[List[str]]: Returns a list of queryset name if operation succeeds.
 
         """
 
-        response = requests.request(method="GET", url=f'{self._remote_url}/querysets')
+        response = requests.request(method="GET", url=f'{self._remote_url}')
 
         qs_list = queryset_list.QuerysetList()
 
         qs_list.querysets = response.content
 
         return qs_list
 
     def publish(self, queryset: queryset_schema.Queryset, overwrite: bool = True) -> requests.Response:
 
         method = "POST"
 
-        url = self._remote_url + "/querysets?" + parse.urlencode({"overwrite": overwrite})
+        print(self._remote_url)
+
+        url = self._remote_url + "?" + parse.urlencode({"overwrite": overwrite})
 
         request_kwargs = {"headers": {}}
 
         request_kwargs.update({"data": json.dumps(queryset.dict())})
 
         request_kwargs["headers"].update({"Content-Type": "application/json"})
 
@@ -90,15 +92,15 @@
 
         return response
 
     def delete(self, name: str) -> requests.Response:
 
         method = "DELETE"
 
-        url = self._remote_url + f"/querysets{name}"
+        url = self._remote_url + f"/{name}"
 
         response = requests.request(method=method, url=url)
 
         return response
 
     def _fetch(self, max_retries: int, base_url: str, name: str) -> pd.DataFrame:
         """
```

### Comparing `viewser-6.3.0/viewser/commands/system/cli.py` & `viewser-6.3.1/viewser/commands/system/cli.py`

 * *Files identical despite different names*

### Comparing `viewser-6.3.0/viewser/commands/system/formatting.py` & `viewser-6.3.1/viewser/commands/system/formatting.py`

 * *Files identical despite different names*

### Comparing `viewser-6.3.0/viewser/error_handling/checks.py` & `viewser-6.3.1/viewser/error_handling/checks.py`

 * *Files identical despite different names*

### Comparing `viewser-6.3.0/viewser/error_handling/error_handling.py` & `viewser-6.3.1/viewser/error_handling/error_handling.py`

 * *Files identical despite different names*

### Comparing `viewser-6.3.0/viewser/error_handling/errors.py` & `viewser-6.3.1/viewser/error_handling/errors.py`

 * *Files identical despite different names*

### Comparing `viewser-6.3.0/viewser/error_handling/exceptions.py` & `viewser-6.3.1/viewser/error_handling/exceptions.py`

 * *Files identical despite different names*

### Comparing `viewser-6.3.0/viewser/operations.py` & `viewser-6.3.1/viewser/operations.py`

 * *Files identical despite different names*

### Comparing `viewser-6.3.0/viewser/remotes.py` & `viewser-6.3.1/viewser/remotes.py`

 * *Files identical despite different names*

### Comparing `viewser-6.3.0/viewser/settings/__init__.py` & `viewser-6.3.1/viewser/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `viewser-6.3.0/viewser/settings/config_resolver.py` & `viewser-6.3.1/viewser/settings/config_resolver.py`

 * *Files identical despite different names*

### Comparing `viewser-6.3.0/viewser/settings/static.py` & `viewser-6.3.1/viewser/settings/static.py`

 * *Files identical despite different names*

### Comparing `viewser-6.3.0/viewser/storage/db.py` & `viewser-6.3.1/viewser/storage/db.py`

 * *Files identical despite different names*

### Comparing `viewser-6.3.0/viewser/storage/metadata_storage_serializer.py` & `viewser-6.3.1/viewser/storage/metadata_storage_serializer.py`

 * *Files identical despite different names*

### Comparing `viewser-6.3.0/viewser/storage/model_object.py` & `viewser-6.3.1/viewser/storage/model_object.py`

 * *Files identical despite different names*

### Comparing `viewser-6.3.0/viewser/tui/animations.py` & `viewser-6.3.1/viewser/tui/animations.py`

 * *Files identical despite different names*

### Comparing `viewser-6.3.0/viewser/tui/formatting/abc.py` & `viewser-6.3.1/viewser/tui/formatting/abc.py`

 * *Files identical despite different names*

### Comparing `viewser-6.3.0/viewser/tui/formatting/errors.py` & `viewser-6.3.1/viewser/tui/formatting/errors.py`

 * *Files identical despite different names*

### Comparing `viewser-6.3.0/PKG-INFO` & `viewser-6.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viewser
-Version: 6.3.0
+Version: 6.3.1
 Summary: The Views 3 CLI tool
 Home-page: https://www.github.com/prio-data/viewser
 License: CC-BY-NC
 Author: peder2911
 Author-email: pglandsverk@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
@@ -86,31 +86,33 @@
 `viewser` functionality is exposed via a CLI on your system after installation.
 An overview of available commands can be seen by running `viewser --help`.
 
 The CLI is envisaged mainly as a tool to help users with issues such as selecting appropriate transforms, exploring the database, determining the level of analysis of a given feature, etc.
 
 ## Useful commands
 
-Show all tables in the database:
+Show all features in the database:
 
-`viewser tables list` 
+`viewser features list <loa>`
 
-Show columns in a particular table:
-
-`viewser tables show table-name`
+with <loa> being one of ['pgm', 'cm', 'pgy', 'cy', 'pg', 'c', 'am', 'a', 'ay', 'm', 'y']
 
 Show all transforms sorted by level of analysis:
 
 `viewser transforms list`
 
-Show docstring for a particular transform:
+Show all transforms available at a particular level of analysis:
+
+`viewser transforms at_loa <loa>`
 
-`viewser transforms show transform-name`
+with <loa> being one of ['any', 'country_month', 'priogrid_month', 'priogrid_year']
+
+Show docstring for a particular transform:
 
-(note that the transform name should be the full name, e.g. 'any/temporal.entropy')
+`viewser transforms show <transform-name>`
 
 ## Via API
 
 The full functionality of viewser is exposed via its API for use in scripts and notebooks
 
 The two fundamental objects used to define what data is fetched by the client are the *Queryset* and the *Column*, where a 
 Queryset consists of one or more Columns.
```

