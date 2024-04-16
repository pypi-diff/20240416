# Comparing `tmp/mxops-2.1.0.tar.gz` & `tmp/mxops-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mxops-2.1.0.tar", last modified: Fri Mar  1 19:52:40 2024, max compression
+gzip compressed data, was "mxops-2.2.0.tar", last modified: Tue Apr 16 16:44:16 2024, max compression
```

## Comparing `mxops-2.1.0.tar` & `mxops-2.2.0.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 19:52:40.546605 mxops-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-03-01 19:52:00.000000 mxops-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5144 2024-03-01 19:52:40.546605 mxops-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4139 2024-03-01 19:52:00.000000 mxops-2.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 19:52:40.538605 mxops-2.1.0/mxops/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-03-01 19:52:00.000000 mxops-2.1.0/mxops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-03-01 19:52:00.000000 mxops-2.1.0/mxops/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 19:52:40.542605 mxops-2.1.0/mxops/analyze/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-03-01 19:52:00.000000 mxops-2.1.0/mxops/analyze/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3799 2024-03-01 19:52:00.000000 mxops-2.1.0/mxops/analyze/agglomerate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4809 2024-03-01 19:52:00.000000 mxops-2.1.0/mxops/analyze/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-03-01 19:52:00.000000 mxops-2.1.0/mxops/analyze/fetching.py
--rw-r--r--   0 runner    (1001) docker     (127)     6872 2024-03-01 19:52:00.000000 mxops-2.1.0/mxops/analyze/plots.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 19:52:40.542605 mxops-2.1.0/mxops/config/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-03-01 19:52:00.000000 mxops-2.1.0/mxops/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-03-01 19:52:00.000000 mxops-2.1.0/mxops/config/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     5606 2024-03-01 19:52:00.000000 mxops-2.1.0/mxops/config/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 19:52:40.542605 mxops-2.1.0/mxops/data/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-03-01 19:52:00.000000 mxops-2.1.0/mxops/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-03-01 19:52:00.000000 mxops-2.1.0/mxops/data/analyze_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     6742 2024-03-01 19:52:00.000000 mxops-2.1.0/mxops/data/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    25500 2024-03-01 19:52:00.000000 mxops-2.1.0/mxops/data/execution_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-03-01 19:52:00.000000 mxops-2.1.0/mxops/data/path.py
--rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-03-01 19:52:00.000000 mxops-2.1.0/mxops/data/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-03-01 19:52:00.000000 mxops-2.1.0/mxops/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     8930 2024-03-01 19:52:00.000000 mxops-2.1.0/mxops/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 19:52:40.546605 mxops-2.1.0/mxops/execution/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-01 19:52:00.000000 mxops-2.1.0/mxops/execution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-03-01 19:52:00.000000 mxops-2.1.0/mxops/execution/account.py
--rw-r--r--   0 runner    (1001) docker     (127)     5413 2024-03-01 19:52:00.000000 mxops-2.1.0/mxops/execution/checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-03-01 19:52:00.000000 mxops-2.1.0/mxops/execution/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-03-01 19:52:00.000000 mxops-2.1.0/mxops/execution/msc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8944 2024-03-01 19:52:00.000000 mxops-2.1.0/mxops/execution/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-03-01 19:52:00.000000 mxops-2.1.0/mxops/execution/scene.py
--rw-r--r--   0 runner    (1001) docker     (127)    54205 2024-03-01 19:52:00.000000 mxops-2.1.0/mxops/execution/steps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-03-01 19:52:00.000000 mxops-2.1.0/mxops/execution/token_management.py
--rw-r--r--   0 runner    (1001) docker     (127)     5488 2024-03-01 19:52:00.000000 mxops-2.1.0/mxops/execution/token_management_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     9760 2024-03-01 19:52:00.000000 mxops-2.1.0/mxops/execution/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 19:52:40.546605 mxops-2.1.0/mxops/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-01 19:52:00.000000 mxops-2.1.0/mxops/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-03-01 19:52:00.000000 mxops-2.1.0/mxops/resources/data_parser_help.txt
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-03-01 19:52:00.000000 mxops-2.1.0/mxops/resources/default_config.ini
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-03-01 19:52:00.000000 mxops-2.1.0/mxops/resources/parser_help.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 19:52:40.546605 mxops-2.1.0/mxops/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-03-01 19:52:00.000000 mxops-2.1.0/mxops/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-03-01 19:52:00.000000 mxops-2.1.0/mxops/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-03-01 19:52:00.000000 mxops-2.1.0/mxops/utils/msc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 19:52:40.546605 mxops-2.1.0/mxops.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5144 2024-03-01 19:52:40.000000 mxops-2.1.0/mxops.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-03-01 19:52:40.000000 mxops-2.1.0/mxops.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 19:52:40.000000 mxops-2.1.0/mxops.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-01 19:52:40.000000 mxops-2.1.0/mxops.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-03-01 19:52:40.000000 mxops-2.1.0/mxops.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-01 19:52:40.000000 mxops-2.1.0/mxops.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-03-01 19:52:00.000000 mxops-2.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-03-01 19:52:00.000000 mxops-2.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-03-01 19:52:40.546605 mxops-2.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 19:52:40.546605 mxops-2.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-03-01 19:52:00.000000 mxops-2.1.0/tests/test_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     7934 2024-03-01 19:52:00.000000 mxops-2.1.0/tests/test_data_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     3292 2024-03-01 19:52:00.000000 mxops-2.1.0/tests/test_execution_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-03-01 19:52:00.000000 mxops-2.1.0/tests/test_instantiate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-03-01 19:52:00.000000 mxops-2.1.0/tests/test_raise_tx_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-03-01 19:52:00.000000 mxops-2.1.0/tests/test_steps.py
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-03-01 19:52:00.000000 mxops-2.1.0/tests/test_token_management.py
--rw-r--r--   0 runner    (1001) docker     (127)    10690 2024-03-01 19:52:00.000000 mxops-2.1.0/tests/test_transfers_extraction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-03-01 19:52:00.000000 mxops-2.1.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:44:16.654097 mxops-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-04-16 16:43:36.000000 mxops-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5144 2024-04-16 16:44:16.654097 mxops-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4139 2024-04-16 16:43:36.000000 mxops-2.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:44:16.642097 mxops-2.2.0/mxops/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-16 16:43:36.000000 mxops-2.2.0/mxops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-16 16:43:36.000000 mxops-2.2.0/mxops/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:44:16.646097 mxops-2.2.0/mxops/analyze/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-16 16:43:36.000000 mxops-2.2.0/mxops/analyze/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3799 2024-04-16 16:43:36.000000 mxops-2.2.0/mxops/analyze/agglomerate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4809 2024-04-16 16:43:36.000000 mxops-2.2.0/mxops/analyze/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-04-16 16:43:36.000000 mxops-2.2.0/mxops/analyze/fetching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6872 2024-04-16 16:43:36.000000 mxops-2.2.0/mxops/analyze/plots.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:44:16.646097 mxops-2.2.0/mxops/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-16 16:43:36.000000 mxops-2.2.0/mxops/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-04-16 16:43:36.000000 mxops-2.2.0/mxops/config/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5722 2024-04-16 16:43:36.000000 mxops-2.2.0/mxops/config/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:44:16.646097 mxops-2.2.0/mxops/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-16 16:43:36.000000 mxops-2.2.0/mxops/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-16 16:43:36.000000 mxops-2.2.0/mxops/data/analyze_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7756 2024-04-16 16:43:36.000000 mxops-2.2.0/mxops/data/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27444 2024-04-16 16:43:36.000000 mxops-2.2.0/mxops/data/execution_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-04-16 16:43:36.000000 mxops-2.2.0/mxops/data/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-04-16 16:43:36.000000 mxops-2.2.0/mxops/data/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-16 16:43:36.000000 mxops-2.2.0/mxops/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8930 2024-04-16 16:43:36.000000 mxops-2.2.0/mxops/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:44:16.650097 mxops-2.2.0/mxops/execution/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-16 16:43:36.000000 mxops-2.2.0/mxops/execution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-04-16 16:43:36.000000 mxops-2.2.0/mxops/execution/account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5413 2024-04-16 16:43:36.000000 mxops-2.2.0/mxops/execution/checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-04-16 16:43:36.000000 mxops-2.2.0/mxops/execution/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-04-16 16:43:36.000000 mxops-2.2.0/mxops/execution/msc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8944 2024-04-16 16:43:36.000000 mxops-2.2.0/mxops/execution/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-04-16 16:43:36.000000 mxops-2.2.0/mxops/execution/scene.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54205 2024-04-16 16:43:36.000000 mxops-2.2.0/mxops/execution/steps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-16 16:43:36.000000 mxops-2.2.0/mxops/execution/token_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5488 2024-04-16 16:43:36.000000 mxops-2.2.0/mxops/execution/token_management_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9760 2024-04-16 16:43:36.000000 mxops-2.2.0/mxops/execution/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:44:16.650097 mxops-2.2.0/mxops/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-16 16:43:36.000000 mxops-2.2.0/mxops/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-04-16 16:43:36.000000 mxops-2.2.0/mxops/resources/data_parser_help.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-16 16:43:36.000000 mxops-2.2.0/mxops/resources/default_config.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-16 16:43:36.000000 mxops-2.2.0/mxops/resources/parser_help.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:44:16.650097 mxops-2.2.0/mxops/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-16 16:43:36.000000 mxops-2.2.0/mxops/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-16 16:43:36.000000 mxops-2.2.0/mxops/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-04-16 16:43:36.000000 mxops-2.2.0/mxops/utils/msc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:44:16.654097 mxops-2.2.0/mxops.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5144 2024-04-16 16:44:16.000000 mxops-2.2.0/mxops.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-04-16 16:44:16.000000 mxops-2.2.0/mxops.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 16:44:16.000000 mxops-2.2.0/mxops.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-16 16:44:16.000000 mxops-2.2.0/mxops.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-16 16:44:16.000000 mxops-2.2.0/mxops.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-16 16:44:16.000000 mxops-2.2.0/mxops.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-16 16:43:36.000000 mxops-2.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-16 16:43:36.000000 mxops-2.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-16 16:44:16.654097 mxops-2.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:44:16.654097 mxops-2.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7113 2024-04-16 16:43:36.000000 mxops-2.2.0/tests/test_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7934 2024-04-16 16:43:36.000000 mxops-2.2.0/tests/test_data_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-04-16 16:43:36.000000 mxops-2.2.0/tests/test_execution_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-04-16 16:43:36.000000 mxops-2.2.0/tests/test_instantiate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-04-16 16:43:36.000000 mxops-2.2.0/tests/test_raise_tx_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-16 16:43:36.000000 mxops-2.2.0/tests/test_steps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-16 16:43:36.000000 mxops-2.2.0/tests/test_token_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10690 2024-04-16 16:43:36.000000 mxops-2.2.0/tests/test_transfers_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-16 16:43:36.000000 mxops-2.2.0/tests/test_utils.py
```

### Comparing `mxops-2.1.0/LICENSE` & `mxops-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mxops-2.1.0/PKG-INFO` & `mxops-2.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mxops
-Version: 2.1.0
+Version: 2.2.0
 Summary: Python package to automate MultiversX smart contracts deployment and contract interactions in general
 Author: Etienne Wallet
 Project-URL: Homepage, https://github.com/Catenscia/MxOps
 Keywords: elrond,multiversx,smart-contract,devops,tests
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mxops-2.1.0/README.md` & `mxops-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `mxops-2.1.0/mxops/__main__.py` & `mxops-2.2.0/mxops/__main__.py`

 * *Files identical despite different names*

### Comparing `mxops-2.1.0/mxops/analyze/agglomerate.py` & `mxops-2.2.0/mxops/analyze/agglomerate.py`

 * *Files identical despite different names*

### Comparing `mxops-2.1.0/mxops/analyze/cli.py` & `mxops-2.2.0/mxops/analyze/cli.py`

 * *Files identical despite different names*

### Comparing `mxops-2.1.0/mxops/analyze/fetching.py` & `mxops-2.2.0/mxops/analyze/fetching.py`

 * *Files identical despite different names*

### Comparing `mxops-2.1.0/mxops/analyze/plots.py` & `mxops-2.2.0/mxops/analyze/plots.py`

 * *Files identical despite different names*

### Comparing `mxops-2.1.0/mxops/config/cli.py` & `mxops-2.2.0/mxops/config/cli.py`

 * *Files identical despite different names*

### Comparing `mxops-2.1.0/mxops/config/config.py` & `mxops-2.2.0/mxops/config/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,17 +36,15 @@
         if config_path is not None:
             with open(config_path.as_posix(), "r", encoding="utf-8") as config_file:
                 self.__config.read_file(config_file)
         else:
             default_config = files("mxops.resources").joinpath("default_config.ini")
             self.__config.read_string(default_config.read_text())
 
-        self.__network_config = ProxyNetworkProvider(
-            self.get("PROXY")
-        ).get_network_config()
+        self.__network_config: Optional[NetworkConfig] = None
 
     def get_network(self) -> NetworkEnum:
         """
         Return the network of the config
 
         :return: network used
         :rtype: NetworkEnum
@@ -56,14 +54,18 @@
     def get_network_config(self) -> NetworkConfig:
         """
         Return the loaded network config
 
         :return: network config
         :rtype: NetworkConfig
         """
+        if self.__network_config is None:
+            self.__network_config = ProxyNetworkProvider(
+                self.get("PROXY")
+            ).get_network_config()
         return self.__network_config
 
     def get(self, option: str) -> str:
         """
         return the specified option for the current environment
 
         :param option: option to get from the config file
```

### Comparing `mxops-2.1.0/mxops/data/analyze_data.py` & `mxops-2.2.0/mxops/data/analyze_data.py`

 * *Files identical despite different names*

### Comparing `mxops-2.1.0/mxops/data/cli.py` & `mxops-2.2.0/mxops/data/cli.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 """
 author: Etienne Wallet
 
 This module contains the cli for the data subpackage
 """
+
 from argparse import (
     _SubParsersAction,
     ArgumentError,
     ArgumentParser,
     Namespace,
     RawDescriptionHelpFormatter,
 )
 import argparse
 from typing import Literal
 
 from importlib_resources import files
 
 from mxops.data import path
 from mxops.config.config import Config
-from mxops.data.execution_data import ScenarioData, delete_scenario_data
+from mxops.data.execution_data import (
+    ScenarioData,
+    clone_scenario_data,
+    delete_scenario_data,
+)
 from mxops.data.utils import json_dumps
 from mxops.enums import parse_network_enum
 from mxops.utils.logger import get_logger
 
 
 LOGGER = get_logger("data cli")
 
@@ -140,15 +145,45 @@
         help="Name of the checkpoint of the scenario to create/load/delete",
     )
 
     checkpoint_parser.add_argument(
         "-a",
         "--action",
         type=valid_checkpoint_action,
-        help="Name of the checkpoint of the scenario to create/load/delete",
+        help="Name of the checkpoint action to perform",
+    )
+
+    # add a clone command
+    clone_parser = data_subparsers_actions.add_parser("clone")
+    clone_parser.add_argument(
+        "-n",
+        "--network",
+        help="Name of the network to use",
+        type=parse_network_enum,
+        required=True,
+    )
+
+    clone_parser.add_argument(
+        "-s", "--source-scenario", help="Name of the source scenario"
+    )
+
+    clone_parser.add_argument(
+        "-d", "--destination-scenario", help="Name of the destination scenario"
+    )
+
+    clone_parser.add_argument(
+        "-c",
+        "--source-checkpoint",
+        required=False,
+        help="Name of the checkpoint of the source scenario",
+        default="",
+    )
+
+    clone_parser.add_argument(
+        "-y", "--yes", action="store_true", help="Skip confirmation step"
     )
 
 
 def valid_checkpoint_action(action: str) -> Literal["create", "load", "delete"]:
     """
     validate the action value for the checkpoint subparser
 
@@ -213,9 +248,16 @@
             scenario.save()
             LOGGER.info(f"Checkpoint {args.checkpoint} loaded")
         elif args.action == "delete":
             delete_scenario_data(args.scenario, args.checkpoint)
             LOGGER.info(f"Checkpoint {args.checkpoint} deleted")
         else:
             raise ArgumentError(None, f"Unkown checkpoint action: {args.action}")
+    elif sub_command == "clone":
+        clone_scenario_data(
+            args.source_scenario,
+            args.destination_scenario,
+            args.source_checkpoint,
+            not args.yes,
+        )
     else:
         raise ArgumentError(None, f"Unkown command: {args.command}")
```

### Comparing `mxops-2.1.0/mxops/data/execution_data.py` & `mxops-2.2.0/mxops/data/execution_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 """
 author: Etienne Wallet
 
 This module contains the functions to load, write and update scenario data
 """
+
 from __future__ import annotations
 from copy import deepcopy
 from dataclasses import asdict, dataclass, field, is_dataclass
 import os
 from pathlib import Path
 import re
 import time
 from typing import Any, Dict, List, Optional
 
 from mxpyserializer.abi_serializer import AbiSerializer
 
 from mxops.config.config import Config
-from mxops.data.path import get_all_checkpoints_names, get_scenario_file_path
+from mxops.data.path import (
+    get_all_checkpoints_names,
+    get_scenario_file_path,
+)
 from mxops import enums as mxops_enums
 from mxops import errors
 from mxops.data.utils import json_dump, json_load
 from mxops.utils.logger import get_logger
 
 
 LOGGER = get_logger("data")
@@ -435,16 +439,14 @@
         self.tokens_data[token_data.name] = token_data
 
     def get_value(self, value_key: str) -> Any:
         """
         Search within tokens data, contracts data and scenario saved values,
         the value saved under the provided key
 
-        :param root_name: contract id or token name that hosts the value
-        :type root_name: str
         :param value_key: key under which the value is savedd
         :type value_key: str
         :return: value saved
         :rtype: Any
         """
         parsed_value_key = parse_value_key(value_key)
         if len(parsed_value_key) > 1:
@@ -636,15 +638,20 @@
         except FileNotFoundError as err:
             raise errors.UnknownScenario(scenario_name) from err
         config = Config.get_config()
         network = config.get_network()
         description = f"scenario {scenario_name}"
         if checkpoint_name != "":
             description += f" checkpoint {checkpoint_name}"
-        LOGGER.info(f"{checkpoint_name} loaded for network {network.value}")
+        if cls._instance.name != scenario_name:
+            raise RuntimeError(
+                f"Loaded scenario name {cls._instance.name} is different from"
+                f" the saved name {scenario_name}"
+            )
+        LOGGER.info(f"{description} loaded for network {network.value}")
 
     @classmethod
     def create_scenario(cls, scenario_name: str):
         """
         Create a scenario data while checking for a pre existing instance.
 
         :param scenario_name: name of the scenario to create
@@ -722,7 +729,52 @@
                 print("User aborted deletion")
                 continue
         try:
             os.remove(scenario_path.as_posix())
             LOGGER.info(f"The data of the {description} has been deleted")
         except FileNotFoundError:
             LOGGER.warning(f"The {description} does not have any data recorded")
+
+
+def clone_scenario_data(
+    source_scenario_name: str,
+    destination_scenario_name: str,
+    source_checkpoint_name: str = "",
+    ask_confirmation: bool = True,
+):
+    """
+    Delete locally save data for a given scenario
+
+    :param source_scenario_name: name of the scenario to copy
+    :type source_scenario_name: str
+    :param destination_scenario_name: name of the scenario that will be a copy
+    :type destination_scenario_name: str
+    :param source_checkpoint_name: checkpoint's name of the source scenario.
+    :type source_checkpoint_name: str, defaults to empty string
+    :param ask_confirmation: if a deletion confirmation should be asked,
+                             defaults to True
+    :type ask_confirmation: bool
+    """
+    source_path = get_scenario_file_path(source_scenario_name, source_checkpoint_name)
+    ScenarioData.load_scenario(source_scenario_name, source_checkpoint_name)
+    scenario = ScenarioData.get()
+    scenario.name = destination_scenario_name
+    if ask_confirmation:
+        source_description = f"scenario {source_scenario_name}"
+        if source_checkpoint_name != "":
+            source_description += f" checkpoint {source_checkpoint_name}"
+        destination_description = f"scenario {destination_scenario_name}"
+        message = (
+            f"Confirm the copy of the {source_description} located at "
+            f"{source_path.as_posix()} to overwrite any data for "
+            f"{destination_description}. (y/n)"
+        )
+        if input(message).lower() not in ("y", "yes"):
+            print("User aborted copy")
+            return
+
+    delete_scenario_data(destination_scenario_name, "", False)
+    scenario.save()
+    LOGGER.info(
+        f"The data of the {source_description} has been copied to "
+        f"{destination_description}"
+    )
```

### Comparing `mxops-2.1.0/mxops/data/path.py` & `mxops-2.2.0/mxops/data/path.py`

 * *Files identical despite different names*

### Comparing `mxops-2.1.0/mxops/data/utils.py` & `mxops-2.2.0/mxops/data/utils.py`

 * *Files identical despite different names*

### Comparing `mxops-2.1.0/mxops/enums.py` & `mxops-2.2.0/mxops/enums.py`

 * *Files identical despite different names*

### Comparing `mxops-2.1.0/mxops/errors.py` & `mxops-2.2.0/mxops/errors.py`

 * *Files identical despite different names*

### Comparing `mxops-2.1.0/mxops/execution/account.py` & `mxops-2.2.0/mxops/execution/account.py`

 * *Files identical despite different names*

### Comparing `mxops-2.1.0/mxops/execution/checks.py` & `mxops-2.2.0/mxops/execution/checks.py`

 * *Files identical despite different names*

### Comparing `mxops-2.1.0/mxops/execution/cli.py` & `mxops-2.2.0/mxops/execution/cli.py`

 * *Files identical despite different names*

### Comparing `mxops-2.1.0/mxops/execution/msc.py` & `mxops-2.2.0/mxops/execution/msc.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 author: Etienne Wallet
 
 Various elements for the execution sub package
 """
+
 from __future__ import annotations
 from dataclasses import dataclass
 from typing import Any, Optional, Union
 
 from mxops.execution import utils
 from mxops.utils import msc
 
@@ -83,25 +84,27 @@
         """
         Evaluate the attribute of the instance dynamically and return the
         corresponding expected transfer
 
         :return: instance dynamically evaluated
         :rtype: ExpectedTransfer
         """
-        evaluations = {}
-        attributes_to_extract = ["sender", "receiver", "token_identifier", "amount"]
-        for attribute_name in attributes_to_extract:
-            extracted_value = utils.retrieve_value_from_string(
-                str(getattr(self, attribute_name))
-            )
-            evaluations[attribute_name] = extracted_value
+        sender = utils.get_address_instance(self.sender).bech32()
+        receiver = utils.get_address_instance(self.receiver).bech32()
+        token_identifier = utils.retrieve_value_from_string(str(self.token_identifier))
+        amount = utils.retrieve_value_from_string(str(self.amount))
         hex_nonce = self.get_hex_nonce()
         if hex_nonce is not None:
-            evaluations["token_identifier"] += "-" + hex_nonce
-        return ExpectedTransfer(**evaluations)
+            token_identifier += "-" + hex_nonce
+        return ExpectedTransfer(
+            sender=sender,
+            receiver=receiver,
+            token_identifier=token_identifier,
+            amount=amount,
+        )
 
     def __eq__(self, other: Any) -> bool:
         evaluated_self = self.get_dynamic_evaluated()
         if isinstance(other, OnChainTransfer):
             evaluated_other = other
         elif isinstance(other, ExpectedTransfer):
             evaluated_other = other.get_dynamic_evaluated()
```

### Comparing `mxops-2.1.0/mxops/execution/network.py` & `mxops-2.2.0/mxops/execution/network.py`

 * *Files identical despite different names*

### Comparing `mxops-2.1.0/mxops/execution/scene.py` & `mxops-2.2.0/mxops/execution/scene.py`

 * *Files identical despite different names*

### Comparing `mxops-2.1.0/mxops/execution/steps.py` & `mxops-2.2.0/mxops/execution/steps.py`

 * *Files identical despite different names*

### Comparing `mxops-2.1.0/mxops/execution/token_management.py` & `mxops-2.2.0/mxops/execution/token_management.py`

 * *Files identical despite different names*

### Comparing `mxops-2.1.0/mxops/execution/token_management_factory.py` & `mxops-2.2.0/mxops/execution/token_management_factory.py`

 * *Files identical despite different names*

### Comparing `mxops-2.1.0/mxops/execution/utils.py` & `mxops-2.2.0/mxops/execution/utils.py`

 * *Files identical despite different names*

### Comparing `mxops-2.1.0/mxops/resources/data_parser_help.txt` & `mxops-2.2.0/mxops/resources/data_parser_help.txt`

 * *Files 8% similar despite different names*

```diff
@@ -2,29 +2,39 @@
 
 mxops data [SUBCOMMAND] [OPTIONS]
 
 Available sub-commands:
 
     get         ->  Print recorded contract data for the current env
                     Required:
-                        -n, --network           name of the network to consider (mainnet, devnet, testnet, localnet)
+                        -n, --network               name of the network to consider (mainnet, devnet, testnet, localnet)
                     Options:
-                        -p, --path              display the root path for the user data
-                        -l, --list              print all the scenarios names
-                        -s, --scenario          print the data saved for a scenario
-                        -c, --checkpoint        name of the checkpoint to use for the scenario
+                        -p, --path                  display the root path for the user data
+                        -l, --list                  print all the scenarios names
+                        -s, --scenario              print the data saved for a scenario
+                        -c, --checkpoint            name of the checkpoint to use for the scenario
 
     delete      ->  Delete locally saved data for a specified network
                     Required:
-                        -n, --network           name of the network to consider (mainnet, devnet, testnet, localnet)
+                        -n, --network               name of the network to consider (mainnet, devnet, testnet, localnet)
                     Options:
-                        -s, --scenario          name of the scenario to delete
-                        -c, --checkpoint        name of the checkpoint to use for the scenario
-                        -a, --all               delete all scenarios for the specified network
-                        -y, --yes               skip confirmation step
+                        -s, --scenario              name of the scenario to delete
+                        -c, --checkpoint            name of the checkpoint to use for the scenario
+                        -a, --all                   delete all scenarios for the specified network
+                        -y, --yes                   skip confirmation step
 
     checkpoint  ->  Delete locally saved data for a specified network
                     Required:
-                        -n, --network           name of the network to consider (mainnet, devnet, testnet, localnet)
-                        -s, --scenario          name of the scenario to delete
-                        -c, --checkpoint        name of the checkpoint to use for the scenario
-                        -a, --action            one of ["create", "load", "delete"]
+                        -n, --network               name of the network to consider (mainnet, devnet, testnet, localnet)
+                        -s, --scenario              name of the scenario to delete
+                        -c, --checkpoint            name of the checkpoint to use for the scenario
+                        -a, --action                one of ["create", "load", "delete"]
+
+    clone       -> Copy the content of a scenario to another (complete overwrite)
+                    Required:
+                        -n, --network               name of the network to consider (mainnet, devnet, testnet, localnet)
+                        -s, --source-scenario       name of the scenario to delete
+                        -d, --destination-scenario  name of the scenario to delete
+                    Options:
+                        -c, --source-checkpoint     name of the checkpoint to use for the scenario
+                        -y, --yes                   skip confirmation step
+
```

### Comparing `mxops-2.1.0/mxops/resources/default_config.ini` & `mxops-2.2.0/mxops/resources/default_config.ini`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 [DEFAULT]
 PROXY=http://localhost:7950
-CHAIN=local-testnet
+CHAIN=localnet
 TX_TIMEOUT=100
 TX_REFRESH_PERIOD=3
 BASE_ISSUING_COST=50000000000000000
 MAX_QUERY_ATTEMPTS=3
 API_RATE_LIMIT=2
 
 [LOCAL]
 PROXY=http://localhost:7950
-CHAIN=local-testnet
+API=http://localhost:3001
+EXPLORER_URL=http://localhost:3002
+CHAIN=localnet
 
 [DEV]
 PROXY=https://devnet-gateway.multiversx.com
 API=https://devnet-api.multiversx.com
 EXPLORER_URL=https://devnet-explorer.multiversx.com
 CHAIN=D
 API_RATE_LIMIT=5
```

### Comparing `mxops-2.1.0/mxops/resources/parser_help.txt` & `mxops-2.2.0/mxops/resources/parser_help.txt`

 * *Files identical despite different names*

### Comparing `mxops-2.1.0/mxops/utils/logger.py` & `mxops-2.2.0/mxops/utils/logger.py`

 * *Files identical despite different names*

### Comparing `mxops-2.1.0/mxops/utils/msc.py` & `mxops-2.2.0/mxops/utils/msc.py`

 * *Files identical despite different names*

### Comparing `mxops-2.1.0/mxops.egg-info/PKG-INFO` & `mxops-2.2.0/mxops.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mxops
-Version: 2.1.0
+Version: 2.2.0
 Summary: Python package to automate MultiversX smart contracts deployment and contract interactions in general
 Author: Etienne Wallet
 Project-URL: Homepage, https://github.com/Catenscia/MxOps
 Keywords: elrond,multiversx,smart-contract,devops,tests
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mxops-2.1.0/mxops.egg-info/SOURCES.txt` & `mxops-2.2.0/mxops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mxops-2.1.0/pyproject.toml` & `mxops-2.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "mxops"
-version = "2.1.0"
+version = "2.2.0"
 authors = [
   {name="Etienne Wallet"},
 ]
 description = "Python package to automate MultiversX smart contracts deployment and contract interactions in general"
 readme = "README.md"
 keywords = ["elrond", "multiversx", "smart-contract", "devops", "tests"]
 classifiers = [
```

### Comparing `mxops-2.1.0/setup.cfg` & `mxops-2.2.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 2.1.0
+current_version = 2.2.0
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(-(?P<release>\w+)(?P<build>\d+))?
 serialize = 
 	{major}.{minor}.{patch}-{release}{build}
 	{major}.{minor}.{patch}
 
 [bumpversion:part:release]
 first_value = dev
```

### Comparing `mxops-2.1.0/tests/test_data_io.py` & `mxops-2.2.0/tests/test_data_io.py`

 * *Files identical despite different names*

### Comparing `mxops-2.1.0/tests/test_execution_utils.py` & `mxops-2.2.0/tests/test_execution_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 
     # Then
     assert retrieved_value == 7458
 
 
 def test_value_from_config():
     # Given
-    expected_value = "local-testnet"
+    expected_value = "localnet"
     value_name = "CHAIN"
 
     # When
     arg = f"&{value_name}"
     retrieved_value = utils.retrieve_value_from_config(arg)
 
     # Then
```

### Comparing `mxops-2.1.0/tests/test_instantiate.py` & `mxops-2.2.0/tests/test_instantiate.py`

 * *Files identical despite different names*

### Comparing `mxops-2.1.0/tests/test_raise_tx_errors.py` & `mxops-2.2.0/tests/test_raise_tx_errors.py`

 * *Files identical despite different names*

### Comparing `mxops-2.1.0/tests/test_steps.py` & `mxops-2.2.0/tests/test_steps.py`

 * *Files identical despite different names*

### Comparing `mxops-2.1.0/tests/test_token_management.py` & `mxops-2.2.0/tests/test_token_management.py`

 * *Files identical despite different names*

### Comparing `mxops-2.1.0/tests/test_transfers_extraction.py` & `mxops-2.2.0/tests/test_transfers_extraction.py`

 * *Files identical despite different names*

### Comparing `mxops-2.1.0/tests/test_utils.py` & `mxops-2.2.0/tests/test_utils.py`

 * *Files identical despite different names*

