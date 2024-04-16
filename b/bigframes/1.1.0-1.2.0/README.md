# Comparing `tmp/bigframes-1.1.0.tar.gz` & `tmp/bigframes-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigframes-1.1.0.tar", last modified: Thu Apr  4 23:04:28 2024, max compression
+gzip compressed data, was "bigframes-1.2.0.tar", last modified: Tue Apr 16 17:11:39 2024, max compression
```

## Comparing `bigframes-1.1.0.tar` & `bigframes-1.2.0.tar`

### file list

```diff
@@ -1,377 +1,377 @@
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 23:04:28.092995 bigframes-1.1.0/
--rw-rw-r--   0 root         (0)     1003    11358 2024-04-04 23:02:01.000000 bigframes-1.1.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      914 2024-04-04 23:02:01.000000 bigframes-1.1.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4650 2024-04-04 23:04:28.092995 bigframes-1.1.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     2256 2024-04-04 23:02:01.000000 bigframes-1.1.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 23:04:28.020990 bigframes-1.1.0/bigframes/
--rw-rw-r--   0 root         (0)     1003     1111 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 23:04:28.020990 bigframes-1.1.0/bigframes/_config/
--rw-rw-r--   0 root         (0)     1003     2453 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/_config/__init__.py
--rw-rw-r--   0 root         (0)     1003     8228 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/_config/bigquery_options.py
--rw-rw-r--   0 root         (0)     1003     2139 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/_config/compute_options.py
--rw-rw-r--   0 root         (0)     1003     1661 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/_config/display_options.py
--rw-rw-r--   0 root         (0)     1003     1892 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/_config/sampling_options.py
--rw-rw-r--   0 root         (0)     1003     7152 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/clients.py
--rw-rw-r--   0 root         (0)     1003     1079 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/constants.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 23:04:28.028991 bigframes-1.1.0/bigframes/core/
--rw-rw-r--   0 root         (0)     1003    15360 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/core/__init__.py
--rw-rw-r--   0 root         (0)     1003    29614 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/core/block_transforms.py
--rw-rw-r--   0 root         (0)     1003    90329 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/core/blocks.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 23:04:28.028991 bigframes-1.1.0/bigframes/core/compile/
--rw-rw-r--   0 root         (0)     1003      832 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/core/compile/__init__.py
--rw-rw-r--   0 root         (0)     1003    17255 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/core/compile/aggregate_compiler.py
--rw-rw-r--   0 root         (0)     1003    62857 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/core/compile/compiled.py
--rw-rw-r--   0 root         (0)     1003     6694 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/core/compile/compiler.py
--rw-rw-r--   0 root         (0)     1003     3356 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/core/compile/concat.py
--rw-rw-r--   0 root         (0)     1003    47517 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/core/compile/scalar_op_compiler.py
--rw-rw-r--   0 root         (0)     1003     7057 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/core/compile/single_column.py
--rw-rw-r--   0 root         (0)     1003     1746 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/core/convert.py
--rw-rw-r--   0 root         (0)     1003     2495 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/core/eval.py
--rw-rw-r--   0 root         (0)     1003     6768 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/core/expression.py
--rw-rw-r--   0 root         (0)     1003     1846 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/core/global_session.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 23:04:28.028991 bigframes-1.1.0/bigframes/core/groupby/
--rw-rw-r--   0 root         (0)     1003    22543 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/core/groupby/__init__.py
--rw-rw-r--   0 root         (0)     1003      716 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/core/guid.py
--rw-rw-r--   0 root         (0)     1003    17649 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/core/indexers.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 23:04:28.028991 bigframes-1.1.0/bigframes/core/indexes/
--rw-rw-r--   0 root         (0)     1003      649 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/core/indexes/__init__.py
--rw-rw-r--   0 root         (0)     1003    16107 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/core/indexes/base.py
--rw-rw-r--   0 root         (0)     1003     1597 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/core/join_def.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 23:04:28.028991 bigframes-1.1.0/bigframes/core/joins/
--rw-rw-r--   0 root         (0)     1003      770 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/core/joins/__init__.py
--rw-rw-r--   0 root         (0)     1003     2132 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/core/joins/merge.py
--rw-rw-r--   0 root         (0)     1003     1883 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/core/joins/name_resolution.py
--rw-rw-r--   0 root         (0)     1003     2218 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/core/local_data.py
--rw-rw-r--   0 root         (0)     1003     2255 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/core/log_adapter.py
--rw-rw-r--   0 root         (0)     1003    21172 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/core/nodes.py
--rw-rw-r--   0 root         (0)     1003     9392 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/core/ordering.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 23:04:28.028991 bigframes-1.1.0/bigframes/core/reshape/
--rw-rw-r--   0 root         (0)     1003     5965 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/core/reshape/__init__.py
--rw-rw-r--   0 root         (0)     1003    10722 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/core/rewrite.py
--rw-rw-r--   0 root         (0)     1003      746 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/core/scalar.py
--rw-rw-r--   0 root         (0)     1003     2144 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/core/schema.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 23:04:28.032991 bigframes-1.1.0/bigframes/core/tools/
--rw-rw-r--   0 root         (0)     1003      664 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/core/tools/__init__.py
--rw-rw-r--   0 root         (0)     1003     2515 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/core/tools/datetimes.py
--rw-rw-r--   0 root         (0)     1003     3002 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/core/tree_properties.py
--rw-rw-r--   0 root         (0)     1003     5483 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/core/utils.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 23:04:28.032991 bigframes-1.1.0/bigframes/core/window/
--rw-rw-r--   0 root         (0)     1003     3075 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/core/window/__init__.py
--rw-rw-r--   0 root         (0)     1003     1286 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/core/window_spec.py
--rw-rw-r--   0 root         (0)     1003   125145 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/dataframe.py
--rw-rw-r--   0 root         (0)     1003    27294 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/dtypes.py
--rw-rw-r--   0 root         (0)     1003     1273 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/features.py
--rw-rw-r--   0 root         (0)     1003    11179 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/formatting_helpers.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 23:04:28.032991 bigframes-1.1.0/bigframes/functions/
--rw-rw-r--   0 root         (0)     1003      574 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/functions/__init__.py
--rw-rw-r--   0 root         (0)     1003    39370 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/functions/remote_function.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 23:04:28.036991 bigframes-1.1.0/bigframes/ml/
--rw-rw-r--   0 root         (0)     1003      877 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/ml/__init__.py
--rw-rw-r--   0 root         (0)     1003     8532 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/ml/base.py
--rw-rw-r--   0 root         (0)     1003     6649 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/ml/cluster.py
--rw-rw-r--   0 root         (0)     1003     7984 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/ml/compose.py
--rw-rw-r--   0 root         (0)     1003    15995 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/ml/core.py
--rw-rw-r--   0 root         (0)     1003     6797 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/ml/decomposition.py
--rw-rw-r--   0 root         (0)     1003    24706 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/ml/ensemble.py
--rw-rw-r--   0 root         (0)     1003    15988 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/ml/forecasting.py
--rw-rw-r--   0 root         (0)     1003     1141 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/ml/globals.py
--rw-rw-r--   0 root         (0)     1003    10861 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/ml/imported.py
--rw-rw-r--   0 root         (0)     1003    13798 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/ml/linear_model.py
--rw-rw-r--   0 root         (0)     1003    27142 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/ml/llm.py
--rw-rw-r--   0 root         (0)     1003     4899 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/ml/loader.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 23:04:28.036991 bigframes-1.1.0/bigframes/ml/metrics/
--rw-rw-r--   0 root         (0)     1003     1066 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/ml/metrics/__init__.py
--rw-rw-r--   0 root         (0)     1003    11096 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/ml/metrics/_metrics.py
--rw-rw-r--   0 root         (0)     1003     2373 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/ml/metrics/pairwise.py
--rw-rw-r--   0 root         (0)     1003     3747 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/ml/model_selection.py
--rw-rw-r--   0 root         (0)     1003     5067 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/ml/pipeline.py
--rw-rw-r--   0 root         (0)     1003    22667 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/ml/preprocessing.py
--rw-rw-r--   0 root         (0)     1003     5754 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/ml/remote.py
--rw-rw-r--   0 root         (0)     1003    13312 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/ml/sql.py
--rw-rw-r--   0 root         (0)     1003     2403 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/ml/utils.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 23:04:28.040992 bigframes-1.1.0/bigframes/operations/
--rw-rw-r--   0 root         (0)     1003    23014 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/operations/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 23:04:28.040992 bigframes-1.1.0/bigframes/operations/_matplotlib/
--rw-rw-r--   0 root         (0)     1003     1022 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/operations/_matplotlib/__init__.py
--rw-rw-r--   0 root         (0)     1003     4477 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/operations/_matplotlib/core.py
--rw-rw-r--   0 root         (0)     1003     5970 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/operations/_matplotlib/hist.py
--rw-rw-r--   0 root         (0)     1003    10425 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/operations/aggregations.py
--rw-rw-r--   0 root         (0)     1003     8273 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/operations/base.py
--rw-rw-r--   0 root         (0)     1003     3079 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/operations/datetimes.py
--rw-rw-r--   0 root         (0)     1003     2814 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/operations/plotting.py
--rw-rw-r--   0 root         (0)     1003     8493 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/operations/strings.py
--rw-rw-r--   0 root         (0)     1003     1679 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/operations/structs.py
--rw-rw-r--   0 root         (0)     1003     7613 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/operations/type.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 23:04:28.040992 bigframes-1.1.0/bigframes/pandas/
--rw-rw-r--   0 root         (0)     1003    23131 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/pandas/__init__.py
--rw-rw-r--   0 root         (0)     1003        0 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/py.typed
--rw-rw-r--   0 root         (0)     1003    60577 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/series.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 23:04:28.040992 bigframes-1.1.0/bigframes/session/
--rw-rw-r--   0 root         (0)     1003    80945 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/session/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 23:04:28.040992 bigframes-1.1.0/bigframes/session/_io/
--rw-rw-r--   0 root         (0)     1003      574 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/session/_io/__init__.py
--rw-rw-r--   0 root         (0)     1003     8040 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/session/_io/bigquery.py
--rw-rw-r--   0 root         (0)     1003     4345 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/session/_io/pandas.py
--rw-rw-r--   0 root         (0)     1003     8043 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/session/clients.py
--rw-rw-r--   0 root         (0)     1003        0 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/typing.py
--rw-rw-r--   0 root         (0)     1003      597 2024-04-04 23:02:01.000000 bigframes-1.1.0/bigframes/version.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 23:04:28.088995 bigframes-1.1.0/bigframes.egg-info/
--rw-r--r--   0 root         (0)     1003     4650 2024-04-04 23:04:27.000000 bigframes-1.1.0/bigframes.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003    12217 2024-04-04 23:04:27.000000 bigframes-1.1.0/bigframes.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2024-04-04 23:04:27.000000 bigframes-1.1.0/bigframes.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003        1 2024-04-04 23:04:27.000000 bigframes-1.1.0/bigframes.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      732 2024-04-04 23:04:27.000000 bigframes-1.1.0/bigframes.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003       29 2024-04-04 23:04:27.000000 bigframes-1.1.0/bigframes.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       81 2024-04-04 23:02:01.000000 bigframes-1.1.0/pyproject.toml
--rw-rw-r--   0 root         (0)     1003       67 2024-04-04 23:04:28.092995 bigframes-1.1.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     4428 2024-04-04 23:02:01.000000 bigframes-1.1.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 23:04:28.040992 bigframes-1.1.0/tests/
--rw-rw-r--   0 root         (0)     1003      574 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/__init__.py
--rw-rw-r--   0 root         (0)     1003     1785 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/config.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 23:04:28.044992 bigframes-1.1.0/tests/data/
--rw-rw-r--   0 root         (0)     1003      619 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/data/hockey_players.json
--rw-rw-r--   0 root         (0)     1003     1250 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/data/hockey_players.jsonl
--rw-rw-r--   0 root         (0)     1003      340 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/data/matrix_2by3.json
--rw-rw-r--   0 root         (0)     1003       80 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/data/matrix_2by3.jsonl
--rw-rw-r--   0 root         (0)     1003      421 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/data/matrix_3by4.json
--rw-rw-r--   0 root         (0)     1003      154 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/data/matrix_3by4.jsonl
--rw-rw-r--   0 root         (0)     1003    33350 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/data/nested.jsonl
--rw-rw-r--   0 root         (0)     1003      966 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/data/nested_schema.json
--rw-rw-r--   0 root         (0)     1003    58869 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/data/penguins.jsonl
--rw-rw-r--   0 root         (0)     1003      636 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/data/penguins_schema.json
--rw-rw-r--   0 root         (0)     1003     3909 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/data/scalars.jsonl
--rw-rw-r--   0 root         (0)     1003     1458 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/data/scalars_schema.json
--rw-rw-r--   0 root         (0)     1003    23424 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/data/time_series.jsonl
--rw-rw-r--   0 root         (0)     1003      192 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/data/time_series_schema.json
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 23:04:28.044992 bigframes-1.1.0/tests/system/
--rw-rw-r--   0 root         (0)     1003      574 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/system/__init__.py
--rw-rw-r--   0 root         (0)     1003    37000 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/system/conftest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 23:04:28.048992 bigframes-1.1.0/tests/system/large/
--rw-rw-r--   0 root         (0)     1003      574 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/system/large/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 23:04:28.048992 bigframes-1.1.0/tests/system/large/ml/
--rw-rw-r--   0 root         (0)     1003     5411 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/system/large/ml/test_cluster.py
--rw-rw-r--   0 root         (0)     1003     5391 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/system/large/ml/test_compose.py
--rw-rw-r--   0 root         (0)     1003     6401 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/system/large/ml/test_core.py
--rw-rw-r--   0 root         (0)     1003     6487 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/system/large/ml/test_decomposition.py
--rw-rw-r--   0 root         (0)     1003    14451 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/system/large/ml/test_ensemble.py
--rw-rw-r--   0 root         (0)     1003     4366 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/system/large/ml/test_forecasting.py
--rw-rw-r--   0 root         (0)     1003     8408 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/system/large/ml/test_linear_model.py
--rw-rw-r--   0 root         (0)     1003    30362 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/system/large/ml/test_pipeline.py
--rw-rw-r--   0 root         (0)     1003     3871 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/system/large/test_location.py
--rw-rw-r--   0 root         (0)     1003    49163 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/system/large/test_remote_function.py
--rw-rw-r--   0 root         (0)     1003     1908 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/system/large/test_session.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 23:04:28.048992 bigframes-1.1.0/tests/system/load/
--rw-rw-r--   0 root         (0)     1003     2664 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/system/load/test_large_tables.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 23:04:28.052992 bigframes-1.1.0/tests/system/small/
--rw-rw-r--   0 root         (0)     1003      574 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/system/small/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 23:04:28.056993 bigframes-1.1.0/tests/system/small/ml/
--rw-rw-r--   0 root         (0)     1003      574 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/system/small/ml/__init__.py
--rw-rw-r--   0 root         (0)     1003    11773 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/system/small/ml/conftest.py
--rw-rw-r--   0 root         (0)     1003     7074 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/system/small/ml/test_cluster.py
--rw-rw-r--   0 root         (0)     1003    13810 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/system/small/ml/test_core.py
--rw-rw-r--   0 root         (0)     1003     6764 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/system/small/ml/test_decomposition.py
--rw-rw-r--   0 root         (0)     1003    17015 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/system/small/ml/test_ensemble.py
--rw-rw-r--   0 root         (0)     1003     6859 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/system/small/ml/test_forecasting.py
--rw-rw-r--   0 root         (0)     1003     4983 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/system/small/ml/test_imported.py
--rw-rw-r--   0 root         (0)     1003     8788 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/system/small/ml/test_linear_model.py
--rw-rw-r--   0 root         (0)     1003    11541 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/system/small/ml/test_llm.py
--rw-rw-r--   0 root         (0)     1003    25138 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/system/small/ml/test_metrics.py
--rw-rw-r--   0 root         (0)     1003     2224 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/system/small/ml/test_metrics_pairwise.py
--rw-rw-r--   0 root         (0)     1003     6197 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/system/small/ml/test_model_selection.py
--rw-rw-r--   0 root         (0)     1003    27150 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/system/small/ml/test_preprocessing.py
--rw-rw-r--   0 root         (0)     1003     2570 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/system/small/ml/test_register.py
--rw-rw-r--   0 root         (0)     1003     1205 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/system/small/ml/test_remote.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 23:04:28.056993 bigframes-1.1.0/tests/system/small/operations/
--rw-rw-r--   0 root         (0)     1003      574 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/system/small/operations/__init__.py
--rw-rw-r--   0 root         (0)     1003    10399 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/system/small/operations/test_datetimes.py
--rw-rw-r--   0 root         (0)     1003    12557 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/system/small/operations/test_plotting.py
--rw-rw-r--   0 root         (0)     1003    15770 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/system/small/operations/test_strings.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 23:04:28.056993 bigframes-1.1.0/tests/system/small/regression/
--rw-rw-r--   0 root         (0)     1003     1999 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/system/small/regression/test_issue355_merge_after_filter.py
--rw-rw-r--   0 root         (0)     1003   138484 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/system/small/test_dataframe.py
--rw-rw-r--   0 root         (0)     1003    19620 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/system/small/test_dataframe_io.py
--rw-rw-r--   0 root         (0)     1003    10210 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/system/small/test_encryption.py
--rw-rw-r--   0 root         (0)     1003    12922 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/system/small/test_groupby.py
--rw-rw-r--   0 root         (0)     1003     1558 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/system/small/test_ibis.py
--rw-rw-r--   0 root         (0)     1003    13328 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/system/small/test_index.py
--rw-rw-r--   0 root         (0)     1003     1205 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/system/small/test_ipython.py
--rw-rw-r--   0 root         (0)     1003    41054 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/system/small/test_multiindex.py
--rw-rw-r--   0 root         (0)     1003     4190 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/system/small/test_numpy.py
--rw-rw-r--   0 root         (0)     1003    17980 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/system/small/test_pandas.py
--rw-rw-r--   0 root         (0)     1003     9533 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/system/small/test_pandas_options.py
--rw-rw-r--   0 root         (0)     1003     4562 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/system/small/test_progress_bar.py
--rw-rw-r--   0 root         (0)     1003    25513 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/system/small/test_remote_function.py
--rw-rw-r--   0 root         (0)     1003      913 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/system/small/test_scalar.py
--rw-rw-r--   0 root         (0)     1003   107376 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/system/small/test_series.py
--rw-rw-r--   0 root         (0)     1003    40409 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/system/small/test_session.py
--rw-rw-r--   0 root         (0)     1003     3343 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/system/small/test_window.py
--rw-rw-r--   0 root         (0)     1003    12113 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/system/utils.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 23:04:28.060993 bigframes-1.1.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      574 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 23:04:28.060993 bigframes-1.1.0/tests/unit/_config/
--rw-rw-r--   0 root         (0)     1003      574 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/unit/_config/__init__.py
--rw-rw-r--   0 root         (0)     1003     2733 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/unit/_config/test_bigquery_options.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 23:04:28.064993 bigframes-1.1.0/tests/unit/core/
--rw-rw-r--   0 root         (0)     1003      574 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/unit/core/__init__.py
--rw-rw-r--   0 root         (0)     1003     1619 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/unit/core/test_bf_utils.py
--rw-rw-r--   0 root         (0)     1003     2966 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/unit/core/test_blocks.py
--rw-rw-r--   0 root         (0)     1003     1553 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/unit/core/test_expression.py
--rw-rw-r--   0 root         (0)     1003     1813 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/unit/core/test_log_adapter.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 23:04:28.064993 bigframes-1.1.0/tests/unit/ml/
--rw-rw-r--   0 root         (0)     1003      574 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/unit/ml/__init__.py
--rw-rw-r--   0 root         (0)     1003     2323 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/unit/ml/test_api_primitives.py
--rw-rw-r--   0 root         (0)     1003     6555 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/unit/ml/test_compose.py
--rw-rw-r--   0 root         (0)     1003     7426 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/unit/ml/test_golden_sql.py
--rw-rw-r--   0 root         (0)     1003     4058 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/unit/ml/test_pipeline.py
--rw-rw-r--   0 root         (0)     1003    13063 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/unit/ml/test_sql.py
--rw-rw-r--   0 root         (0)     1003     4842 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/unit/resources.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 23:04:28.064993 bigframes-1.1.0/tests/unit/session/
--rw-rw-r--   0 root         (0)     1003      574 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/unit/session/__init__.py
--rw-rw-r--   0 root         (0)     1003     4347 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/unit/session/test_clients.py
--rw-rw-r--   0 root         (0)     1003     7809 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/unit/session/test_io_bigquery.py
--rw-rw-r--   0 root         (0)     1003    18664 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/unit/session/test_io_pandas.py
--rw-rw-r--   0 root         (0)     1003     6619 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/unit/session/test_session.py
--rw-rw-r--   0 root         (0)     1003     1744 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/unit/test_clients.py
--rw-rw-r--   0 root         (0)     1003     1056 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/unit/test_compute_options.py
--rw-rw-r--   0 root         (0)     1003     6648 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/unit/test_core.py
--rw-rw-r--   0 root         (0)     1003     2136 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/unit/test_dataframe.py
--rw-rw-r--   0 root         (0)     1003     8819 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/unit/test_dtypes.py
--rw-rw-r--   0 root         (0)     1003     1577 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/unit/test_features.py
--rw-rw-r--   0 root         (0)     1003      528 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/unit/test_formatting_helper.py
--rw-rw-r--   0 root         (0)     1003     1655 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/unit/test_formatting_helpers.py
--rw-rw-r--   0 root         (0)     1003     4055 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/unit/test_pandas.py
--rw-rw-r--   0 root         (0)     1003     1207 2024-04-04 23:02:01.000000 bigframes-1.1.0/tests/unit/test_remote_function.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 23:04:28.008990 bigframes-1.1.0/third_party/
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 23:04:28.064993 bigframes-1.1.0/third_party/bigframes_vendored/
--rw-rw-r--   0 root         (0)     1003        0 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 23:04:28.064993 bigframes-1.1.0/third_party/bigframes_vendored/cpython/
--rw-rw-r--   0 root         (0)     1003     2339 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/cpython/LICENSE
--rw-rw-r--   0 root         (0)     1003        0 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/cpython/__init__.py
--rw-rw-r--   0 root         (0)     1003    18853 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/cpython/_pprint.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 23:04:28.068993 bigframes-1.1.0/third_party/bigframes_vendored/google_cloud_bigquery/
--rw-rw-r--   0 root         (0)     1003    11358 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/google_cloud_bigquery/LICENSE
--rw-rw-r--   0 root         (0)     1003      574 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/google_cloud_bigquery/__init__.py
--rw-rw-r--   0 root         (0)     1003     5290 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/google_cloud_bigquery/_pandas_helpers.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 23:04:28.068993 bigframes-1.1.0/third_party/bigframes_vendored/google_cloud_bigquery/tests/
--rw-rw-r--   0 root         (0)     1003      574 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/google_cloud_bigquery/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 23:04:28.068993 bigframes-1.1.0/third_party/bigframes_vendored/google_cloud_bigquery/tests/unit/
--rw-rw-r--   0 root         (0)     1003      574 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/google_cloud_bigquery/tests/unit/__init__.py
--rw-rw-r--   0 root         (0)     1003    14045 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/google_cloud_bigquery/tests/unit/test_pandas_helpers.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 23:04:28.068993 bigframes-1.1.0/third_party/bigframes_vendored/ibis/
--rw-rw-r--   0 root         (0)     1003    11358 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/ibis/LICENSE.txt
--rw-rw-r--   0 root         (0)     1003    11663 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/ibis/README.md
--rw-rw-r--   0 root         (0)     1003        0 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/ibis/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 23:04:28.068993 bigframes-1.1.0/third_party/bigframes_vendored/ibis/backends/
--rw-rw-r--   0 root         (0)     1003        0 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/ibis/backends/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 23:04:28.068993 bigframes-1.1.0/third_party/bigframes_vendored/ibis/backends/bigquery/
--rw-rw-r--   0 root         (0)     1003      184 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/ibis/backends/bigquery/__init__.py
--rw-rw-r--   0 root         (0)     1003     2091 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/ibis/backends/bigquery/compiler.py
--rw-rw-r--   0 root         (0)     1003     6600 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/ibis/backends/bigquery/datatypes.py
--rw-rw-r--   0 root         (0)     1003     1582 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/ibis/backends/bigquery/registry.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 23:04:28.068993 bigframes-1.1.0/third_party/bigframes_vendored/ibis/expr/
--rw-rw-r--   0 root         (0)     1003        0 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/ibis/expr/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 23:04:28.072994 bigframes-1.1.0/third_party/bigframes_vendored/ibis/expr/operations/
--rw-rw-r--   0 root         (0)     1003      464 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/ibis/expr/operations/__init__.py
--rw-rw-r--   0 root         (0)     1003      536 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/ibis/expr/operations/analytic.py
--rw-rw-r--   0 root         (0)     1003      276 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/ibis/expr/operations/generic.py
--rw-rw-r--   0 root         (0)     1003      263 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/ibis/expr/operations/json.py
--rw-rw-r--   0 root         (0)     1003      690 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/ibis/expr/operations/reductions.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 23:04:28.072994 bigframes-1.1.0/third_party/bigframes_vendored/pandas/
--rw-rw-r--   0 root         (0)     1003     2284 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/pandas/AUTHORS.md
--rw-rw-r--   0 root         (0)     1003     1634 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/pandas/LICENSE
--rw-rw-r--   0 root         (0)     1003    10620 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/pandas/README.md
--rw-rw-r--   0 root         (0)     1003        0 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/pandas/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 23:04:28.072994 bigframes-1.1.0/third_party/bigframes_vendored/pandas/_config/
--rw-rw-r--   0 root         (0)     1003     1347 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/pandas/_config/config.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 23:04:28.072994 bigframes-1.1.0/third_party/bigframes_vendored/pandas/core/
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 23:04:28.076994 bigframes-1.1.0/third_party/bigframes_vendored/pandas/core/arrays/
--rw-rw-r--   0 root         (0)     1003        0 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/pandas/core/arrays/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 23:04:28.076994 bigframes-1.1.0/third_party/bigframes_vendored/pandas/core/arrays/arrow/
--rw-rw-r--   0 root         (0)     1003        0 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/pandas/core/arrays/arrow/__init__.py
--rw-rw-r--   0 root         (0)     1003     2824 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/pandas/core/arrays/arrow/accessors.py
--rw-rw-r--   0 root         (0)     1003     3672 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/pandas/core/arrays/datetimelike.py
--rw-rw-r--   0 root         (0)     1003     2086 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/pandas/core/common.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 23:04:28.076994 bigframes-1.1.0/third_party/bigframes_vendored/pandas/core/computation/
--rw-rw-r--   0 root         (0)     1003     6944 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/pandas/core/computation/align.py
--rw-rw-r--   0 root         (0)     1003     1543 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/pandas/core/computation/common.py
--rw-rw-r--   0 root         (0)     1003     2295 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/pandas/core/computation/engines.py
--rw-rw-r--   0 root         (0)     1003    12685 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/pandas/core/computation/eval.py
--rw-rw-r--   0 root         (0)     1003    25132 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/pandas/core/computation/expr.py
--rw-rw-r--   0 root         (0)     1003    16244 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/pandas/core/computation/ops.py
--rw-rw-r--   0 root         (0)     1003     6477 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/pandas/core/computation/parsing.py
--rw-rw-r--   0 root         (0)     1003    10303 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/pandas/core/computation/scope.py
--rw-rw-r--   0 root         (0)     1003     4386 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/pandas/core/config_init.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 23:04:28.076994 bigframes-1.1.0/third_party/bigframes_vendored/pandas/core/dtypes/
--rw-rw-r--   0 root         (0)     1003      707 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/pandas/core/dtypes/inference.py
--rw-rw-r--   0 root         (0)     1003   191651 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/pandas/core/frame.py
--rw-rw-r--   0 root         (0)     1003    38558 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/pandas/core/generic.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 23:04:28.076994 bigframes-1.1.0/third_party/bigframes_vendored/pandas/core/groupby/
--rw-rw-r--   0 root         (0)     1003    12987 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/pandas/core/groupby/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 23:04:28.076994 bigframes-1.1.0/third_party/bigframes_vendored/pandas/core/indexes/
--rw-rw-r--   0 root         (0)     1003        0 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/pandas/core/indexes/__init__.py
--rw-rw-r--   0 root         (0)     1003     3129 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/pandas/core/indexes/accessor.py
--rw-rw-r--   0 root         (0)     1003    11448 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/pandas/core/indexes/base.py
--rw-rw-r--   0 root         (0)     1003     2909 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/pandas/core/indexing.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 23:04:28.080994 bigframes-1.1.0/third_party/bigframes_vendored/pandas/core/reshape/
--rw-rw-r--   0 root         (0)     1003        0 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/pandas/core/reshape/__init__.py
--rw-rw-r--   0 root         (0)     1003     4372 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/pandas/core/reshape/concat.py
--rw-rw-r--   0 root         (0)     1003     3804 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/pandas/core/reshape/encoding.py
--rw-rw-r--   0 root         (0)     1003     3220 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/pandas/core/reshape/merge.py
--rw-rw-r--   0 root         (0)     1003     5276 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/pandas/core/reshape/tile.py
--rw-rw-r--   0 root         (0)     1003   109453 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/pandas/core/series.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 23:04:28.080994 bigframes-1.1.0/third_party/bigframes_vendored/pandas/core/strings/
--rw-rw-r--   0 root         (0)     1003    20170 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/pandas/core/strings/accessor.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 23:04:28.080994 bigframes-1.1.0/third_party/bigframes_vendored/pandas/core/tools/
--rw-rw-r--   0 root         (0)     1003        0 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/pandas/core/tools/__init__.py
--rw-rw-r--   0 root         (0)     1003     2858 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/pandas/core/tools/datetimes.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 23:04:28.080994 bigframes-1.1.0/third_party/bigframes_vendored/pandas/core/window/
--rw-rw-r--   0 root         (0)     1003        0 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/pandas/core/window/__init__.py
--rw-rw-r--   0 root         (0)     1003     1350 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/pandas/core/window/rolling.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 23:04:28.080994 bigframes-1.1.0/third_party/bigframes_vendored/pandas/io/
--rw-rw-r--   0 root         (0)     1003        0 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/pandas/io/__init__.py
--rw-rw-r--   0 root         (0)     1003     1269 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/pandas/io/common.py
--rw-rw-r--   0 root         (0)     1003     6612 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/pandas/io/gbq.py
--rw-rw-r--   0 root         (0)     1003     1428 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/pandas/io/parquet.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 23:04:28.084994 bigframes-1.1.0/third_party/bigframes_vendored/pandas/io/parsers/
--rw-rw-r--   0 root         (0)     1003        0 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/pandas/io/parsers/__init__.py
--rw-rw-r--   0 root         (0)     1003    10553 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/pandas/io/parsers/readers.py
--rw-rw-r--   0 root         (0)     1003     3130 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/pandas/io/pickle.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 23:04:28.084994 bigframes-1.1.0/third_party/bigframes_vendored/pandas/pandas/
--rw-rw-r--   0 root         (0)     1003    12353 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/pandas/pandas/_typing.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 23:04:28.084994 bigframes-1.1.0/third_party/bigframes_vendored/pandas/plotting/
--rw-rw-r--   0 root         (0)     1003    11128 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/pandas/plotting/_core.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 23:04:28.084994 bigframes-1.1.0/third_party/bigframes_vendored/pandas/util/
--rw-rw-r--   0 root         (0)     1003      765 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/pandas/util/_exceptions.py
--rw-rw-r--   0 root         (0)     1003     1573 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/pandas/util/_validators.py
--rw-rw-r--   0 root         (0)     1003        0 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 23:04:28.084994 bigframes-1.1.0/third_party/bigframes_vendored/sklearn/
--rw-rw-r--   0 root         (0)     1003     1532 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/sklearn/COPYING
--rw-rw-r--   0 root         (0)     1003        0 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/sklearn/__init__.py
--rw-rw-r--   0 root         (0)     1003     6210 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/sklearn/base.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 23:04:28.084994 bigframes-1.1.0/third_party/bigframes_vendored/sklearn/cluster/
--rw-rw-r--   0 root         (0)     1003     5924 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/sklearn/cluster/_kmeans.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 23:04:28.084994 bigframes-1.1.0/third_party/bigframes_vendored/sklearn/compose/
--rw-rw-r--   0 root         (0)     1003     2014 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/sklearn/compose/_column_transformer.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 23:04:28.084994 bigframes-1.1.0/third_party/bigframes_vendored/sklearn/decomposition/
--rw-rw-r--   0 root         (0)     1003     5387 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/sklearn/decomposition/_pca.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 23:04:28.084994 bigframes-1.1.0/third_party/bigframes_vendored/sklearn/ensemble/
--rw-rw-r--   0 root         (0)     1003        0 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/sklearn/ensemble/__init__.py
--rw-rw-r--   0 root         (0)     1003     8979 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/sklearn/ensemble/_forest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 23:04:28.084994 bigframes-1.1.0/third_party/bigframes_vendored/sklearn/linear_model/
--rw-rw-r--   0 root         (0)     1003     5417 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/sklearn/linear_model/_base.py
--rw-rw-r--   0 root         (0)     1003     4348 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/sklearn/linear_model/_logistic.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 23:04:28.088995 bigframes-1.1.0/third_party/bigframes_vendored/sklearn/metrics/
--rw-rw-r--   0 root         (0)     1003     9779 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/sklearn/metrics/_classification.py
--rw-rw-r--   0 root         (0)     1003     6347 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/sklearn/metrics/_ranking.py
--rw-rw-r--   0 root         (0)     1003     3550 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/sklearn/metrics/_regression.py
--rw-rw-r--   0 root         (0)     1003     2121 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/sklearn/metrics/pairwise.py
--rw-rw-r--   0 root         (0)     1003     2973 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/sklearn/pipeline.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 23:04:28.088995 bigframes-1.1.0/third_party/bigframes_vendored/sklearn/preprocessing/
--rw-rw-r--   0 root         (0)     1003     4980 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/sklearn/preprocessing/_data.py
--rw-rw-r--   0 root         (0)     1003     1523 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/sklearn/preprocessing/_discretization.py
--rw-rw-r--   0 root         (0)     1003     3753 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/sklearn/preprocessing/_encoder.py
--rw-rw-r--   0 root         (0)     1003     2085 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/sklearn/preprocessing/_label.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 23:04:28.088995 bigframes-1.1.0/third_party/bigframes_vendored/xgboost/
--rw-rw-r--   0 root         (0)     1003    11348 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/xgboost/LICENSE
--rw-rw-r--   0 root         (0)     1003        0 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/xgboost/__init__.py
--rw-rw-r--   0 root         (0)     1003     6921 2024-04-04 23:02:01.000000 bigframes-1.1.0/third_party/bigframes_vendored/xgboost/sklearn.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.986379 bigframes-1.2.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2024-04-16 17:09:14.000000 bigframes-1.2.0/LICENSE
+-rw-rw-r--   0 root         (0)     1003      914 2024-04-16 17:09:14.000000 bigframes-1.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4650 2024-04-16 17:11:39.986379 bigframes-1.2.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     2256 2024-04-16 17:09:14.000000 bigframes-1.2.0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.906391 bigframes-1.2.0/bigframes/
+-rw-rw-r--   0 root         (0)     1003     1111 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.906391 bigframes-1.2.0/bigframes/_config/
+-rw-rw-r--   0 root         (0)     1003     2453 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/_config/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8228 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/_config/bigquery_options.py
+-rw-rw-r--   0 root         (0)     1003     2141 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/_config/compute_options.py
+-rw-rw-r--   0 root         (0)     1003     1661 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/_config/display_options.py
+-rw-rw-r--   0 root         (0)     1003     1892 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/_config/sampling_options.py
+-rw-rw-r--   0 root         (0)     1003     7152 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/clients.py
+-rw-rw-r--   0 root         (0)     1003     2637 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/constants.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.914389 bigframes-1.2.0/bigframes/core/
+-rw-rw-r--   0 root         (0)     1003    15308 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/core/__init__.py
+-rw-rw-r--   0 root         (0)     1003    29614 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/core/block_transforms.py
+-rw-rw-r--   0 root         (0)     1003    91658 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/core/blocks.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.914389 bigframes-1.2.0/bigframes/core/compile/
+-rw-rw-r--   0 root         (0)     1003      832 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/core/compile/__init__.py
+-rw-rw-r--   0 root         (0)     1003    17255 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/core/compile/aggregate_compiler.py
+-rw-rw-r--   0 root         (0)     1003    62857 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/core/compile/compiled.py
+-rw-rw-r--   0 root         (0)     1003     6694 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/core/compile/compiler.py
+-rw-rw-r--   0 root         (0)     1003     3356 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/core/compile/concat.py
+-rw-rw-r--   0 root         (0)     1003    47483 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/core/compile/scalar_op_compiler.py
+-rw-rw-r--   0 root         (0)     1003     7121 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/core/compile/single_column.py
+-rw-rw-r--   0 root         (0)     1003     2369 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/core/convert.py
+-rw-rw-r--   0 root         (0)     1003     2495 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/core/eval.py
+-rw-rw-r--   0 root         (0)     1003     6768 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/core/expression.py
+-rw-rw-r--   0 root         (0)     1003     1846 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/core/global_session.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.914389 bigframes-1.2.0/bigframes/core/groupby/
+-rw-rw-r--   0 root         (0)     1003    22543 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/core/groupby/__init__.py
+-rw-rw-r--   0 root         (0)     1003      716 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/core/guid.py
+-rw-rw-r--   0 root         (0)     1003    18056 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/core/indexers.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.918389 bigframes-1.2.0/bigframes/core/indexes/
+-rw-rw-r--   0 root         (0)     1003      719 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/core/indexes/__init__.py
+-rw-rw-r--   0 root         (0)     1003    16223 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/core/indexes/base.py
+-rw-rw-r--   0 root         (0)     1003     1720 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/core/indexes/multi.py
+-rw-rw-r--   0 root         (0)     1003     1597 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/core/join_def.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.918389 bigframes-1.2.0/bigframes/core/joins/
+-rw-rw-r--   0 root         (0)     1003      691 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/core/joins/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2132 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/core/joins/merge.py
+-rw-rw-r--   0 root         (0)     1003     2218 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/core/local_data.py
+-rw-rw-r--   0 root         (0)     1003     2255 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/core/log_adapter.py
+-rw-rw-r--   0 root         (0)     1003    21172 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/core/nodes.py
+-rw-rw-r--   0 root         (0)     1003     9392 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/core/ordering.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.918389 bigframes-1.2.0/bigframes/core/reshape/
+-rw-rw-r--   0 root         (0)     1003     6872 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/core/reshape/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10722 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/core/rewrite.py
+-rw-rw-r--   0 root         (0)     1003      746 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/core/scalar.py
+-rw-rw-r--   0 root         (0)     1003     2144 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/core/schema.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.918389 bigframes-1.2.0/bigframes/core/tools/
+-rw-rw-r--   0 root         (0)     1003      664 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/core/tools/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2515 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/core/tools/datetimes.py
+-rw-rw-r--   0 root         (0)     1003     3002 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/core/tree_properties.py
+-rw-rw-r--   0 root         (0)     1003     5483 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/core/utils.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.918389 bigframes-1.2.0/bigframes/core/window/
+-rw-rw-r--   0 root         (0)     1003     3075 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/core/window/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1286 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/core/window_spec.py
+-rw-rw-r--   0 root         (0)     1003   130958 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/dataframe.py
+-rw-rw-r--   0 root         (0)     1003    27474 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/dtypes.py
+-rw-rw-r--   0 root         (0)     1003     1273 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/features.py
+-rw-rw-r--   0 root         (0)     1003    11179 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/formatting_helpers.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.918389 bigframes-1.2.0/bigframes/functions/
+-rw-rw-r--   0 root         (0)     1003      574 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/functions/__init__.py
+-rw-rw-r--   0 root         (0)     1003    39370 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/functions/remote_function.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.922388 bigframes-1.2.0/bigframes/ml/
+-rw-rw-r--   0 root         (0)     1003      877 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/ml/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8542 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/ml/base.py
+-rw-rw-r--   0 root         (0)     1003     6659 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/ml/cluster.py
+-rw-rw-r--   0 root         (0)     1003     7984 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/ml/compose.py
+-rw-rw-r--   0 root         (0)     1003    15995 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/ml/core.py
+-rw-rw-r--   0 root         (0)     1003     6807 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/ml/decomposition.py
+-rw-rw-r--   0 root         (0)     1003    24746 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/ml/ensemble.py
+-rw-rw-r--   0 root         (0)     1003    15998 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/ml/forecasting.py
+-rw-rw-r--   0 root         (0)     1003     1141 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/ml/globals.py
+-rw-rw-r--   0 root         (0)     1003    10844 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/ml/imported.py
+-rw-rw-r--   0 root         (0)     1003    13818 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/ml/linear_model.py
+-rw-rw-r--   0 root         (0)     1003    27172 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/ml/llm.py
+-rw-rw-r--   0 root         (0)     1003     4899 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/ml/loader.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.926388 bigframes-1.2.0/bigframes/ml/metrics/
+-rw-rw-r--   0 root         (0)     1003     1066 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/ml/metrics/__init__.py
+-rw-rw-r--   0 root         (0)     1003    11096 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/ml/metrics/_metrics.py
+-rw-rw-r--   0 root         (0)     1003     2373 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/ml/metrics/pairwise.py
+-rw-rw-r--   0 root         (0)     1003     3747 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/ml/model_selection.py
+-rw-rw-r--   0 root         (0)     1003     5067 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/ml/pipeline.py
+-rw-rw-r--   0 root         (0)     1003    22667 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/ml/preprocessing.py
+-rw-rw-r--   0 root         (0)     1003     5754 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/ml/remote.py
+-rw-rw-r--   0 root         (0)     1003    13312 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/ml/sql.py
+-rw-rw-r--   0 root         (0)     1003     2403 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/ml/utils.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.926388 bigframes-1.2.0/bigframes/operations/
+-rw-rw-r--   0 root         (0)     1003    23014 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/operations/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.926388 bigframes-1.2.0/bigframes/operations/_matplotlib/
+-rw-rw-r--   0 root         (0)     1003     1022 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/operations/_matplotlib/__init__.py
+-rw-rw-r--   0 root         (0)     1003     4477 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/operations/_matplotlib/core.py
+-rw-rw-r--   0 root         (0)     1003     5970 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/operations/_matplotlib/hist.py
+-rw-rw-r--   0 root         (0)     1003    12880 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/operations/aggregations.py
+-rw-rw-r--   0 root         (0)     1003     8273 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/operations/base.py
+-rw-rw-r--   0 root         (0)     1003     3079 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/operations/datetimes.py
+-rw-rw-r--   0 root         (0)     1003     2814 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/operations/plotting.py
+-rw-rw-r--   0 root         (0)     1003     9009 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/operations/strings.py
+-rw-rw-r--   0 root         (0)     1003     1679 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/operations/structs.py
+-rw-rw-r--   0 root         (0)     1003     7613 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/operations/type.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.926388 bigframes-1.2.0/bigframes/pandas/
+-rw-rw-r--   0 root         (0)     1003    23224 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/pandas/__init__.py
+-rw-rw-r--   0 root         (0)     1003        0 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/py.typed
+-rw-rw-r--   0 root         (0)     1003    64129 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/series.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.926388 bigframes-1.2.0/bigframes/session/
+-rw-rw-r--   0 root         (0)     1003    81282 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/session/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.930387 bigframes-1.2.0/bigframes/session/_io/
+-rw-rw-r--   0 root         (0)     1003      574 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/session/_io/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8040 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/session/_io/bigquery.py
+-rw-rw-r--   0 root         (0)     1003     4345 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/session/_io/pandas.py
+-rw-rw-r--   0 root         (0)     1003     8043 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/session/clients.py
+-rw-rw-r--   0 root         (0)     1003        0 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/typing.py
+-rw-rw-r--   0 root         (0)     1003      597 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/version.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.982380 bigframes-1.2.0/bigframes.egg-info/
+-rw-r--r--   0 root         (0)     1003     4650 2024-04-16 17:11:39.000000 bigframes-1.2.0/bigframes.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003    12253 2024-04-16 17:11:39.000000 bigframes-1.2.0/bigframes.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-04-16 17:11:39.000000 bigframes-1.2.0/bigframes.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-04-16 17:11:39.000000 bigframes-1.2.0/bigframes.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      732 2024-04-16 17:11:39.000000 bigframes-1.2.0/bigframes.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003       29 2024-04-16 17:11:39.000000 bigframes-1.2.0/bigframes.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       81 2024-04-16 17:09:14.000000 bigframes-1.2.0/pyproject.toml
+-rw-rw-r--   0 root         (0)     1003       67 2024-04-16 17:11:39.986379 bigframes-1.2.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     4428 2024-04-16 17:09:14.000000 bigframes-1.2.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.930387 bigframes-1.2.0/tests/
+-rw-rw-r--   0 root         (0)     1003      574 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.934387 bigframes-1.2.0/tests/data/
+-rw-rw-r--   0 root         (0)     1003      619 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/data/hockey_players.json
+-rw-rw-r--   0 root         (0)     1003     1250 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/data/hockey_players.jsonl
+-rw-rw-r--   0 root         (0)     1003      340 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/data/matrix_2by3.json
+-rw-rw-r--   0 root         (0)     1003       80 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/data/matrix_2by3.jsonl
+-rw-rw-r--   0 root         (0)     1003      421 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/data/matrix_3by4.json
+-rw-rw-r--   0 root         (0)     1003      154 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/data/matrix_3by4.jsonl
+-rw-rw-r--   0 root         (0)     1003    33350 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/data/nested.jsonl
+-rw-rw-r--   0 root         (0)     1003      966 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/data/nested_schema.json
+-rw-rw-r--   0 root         (0)     1003    58869 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/data/penguins.jsonl
+-rw-rw-r--   0 root         (0)     1003      636 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/data/penguins_schema.json
+-rw-rw-r--   0 root         (0)     1003     3909 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/data/scalars.jsonl
+-rw-rw-r--   0 root         (0)     1003     1458 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/data/scalars_schema.json
+-rw-rw-r--   0 root         (0)     1003    23424 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/data/time_series.jsonl
+-rw-rw-r--   0 root         (0)     1003      192 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/data/time_series_schema.json
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.934387 bigframes-1.2.0/tests/system/
+-rw-rw-r--   0 root         (0)     1003      574 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/__init__.py
+-rw-rw-r--   0 root         (0)     1003    37000 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/conftest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.934387 bigframes-1.2.0/tests/system/large/
+-rw-rw-r--   0 root         (0)     1003      574 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/large/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.938386 bigframes-1.2.0/tests/system/large/ml/
+-rw-rw-r--   0 root         (0)     1003     5411 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/large/ml/test_cluster.py
+-rw-rw-r--   0 root         (0)     1003     5391 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/large/ml/test_compose.py
+-rw-rw-r--   0 root         (0)     1003     6401 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/large/ml/test_core.py
+-rw-rw-r--   0 root         (0)     1003     6487 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/large/ml/test_decomposition.py
+-rw-rw-r--   0 root         (0)     1003    14451 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/large/ml/test_ensemble.py
+-rw-rw-r--   0 root         (0)     1003     4366 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/large/ml/test_forecasting.py
+-rw-rw-r--   0 root         (0)     1003     8408 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/large/ml/test_linear_model.py
+-rw-rw-r--   0 root         (0)     1003    30362 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/large/ml/test_pipeline.py
+-rw-rw-r--   0 root         (0)     1003     4079 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/large/test_location.py
+-rw-rw-r--   0 root         (0)     1003    49163 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/large/test_remote_function.py
+-rw-rw-r--   0 root         (0)     1003     1908 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/large/test_session.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.938386 bigframes-1.2.0/tests/system/load/
+-rw-rw-r--   0 root         (0)     1003     2664 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/load/test_large_tables.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.942386 bigframes-1.2.0/tests/system/small/
+-rw-rw-r--   0 root         (0)     1003      574 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/small/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.946385 bigframes-1.2.0/tests/system/small/ml/
+-rw-rw-r--   0 root         (0)     1003      574 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/small/ml/__init__.py
+-rw-rw-r--   0 root         (0)     1003    11773 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/small/ml/conftest.py
+-rw-rw-r--   0 root         (0)     1003     7074 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/small/ml/test_cluster.py
+-rw-rw-r--   0 root         (0)     1003    13810 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/small/ml/test_core.py
+-rw-rw-r--   0 root         (0)     1003     6764 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/small/ml/test_decomposition.py
+-rw-rw-r--   0 root         (0)     1003    17015 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/small/ml/test_ensemble.py
+-rw-rw-r--   0 root         (0)     1003     6859 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/small/ml/test_forecasting.py
+-rw-rw-r--   0 root         (0)     1003     4983 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/small/ml/test_imported.py
+-rw-rw-r--   0 root         (0)     1003     8788 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/small/ml/test_linear_model.py
+-rw-rw-r--   0 root         (0)     1003    11541 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/small/ml/test_llm.py
+-rw-rw-r--   0 root         (0)     1003    25138 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/small/ml/test_metrics.py
+-rw-rw-r--   0 root         (0)     1003     2224 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/small/ml/test_metrics_pairwise.py
+-rw-rw-r--   0 root         (0)     1003     6197 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/small/ml/test_model_selection.py
+-rw-rw-r--   0 root         (0)     1003    27150 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/small/ml/test_preprocessing.py
+-rw-rw-r--   0 root         (0)     1003     2570 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/small/ml/test_register.py
+-rw-rw-r--   0 root         (0)     1003     1205 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/small/ml/test_remote.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.946385 bigframes-1.2.0/tests/system/small/operations/
+-rw-rw-r--   0 root         (0)     1003      574 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/small/operations/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10399 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/small/operations/test_datetimes.py
+-rw-rw-r--   0 root         (0)     1003    12453 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/small/operations/test_plotting.py
+-rw-rw-r--   0 root         (0)     1003    15770 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/small/operations/test_strings.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.946385 bigframes-1.2.0/tests/system/small/regression/
+-rw-rw-r--   0 root         (0)     1003     1999 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/small/regression/test_issue355_merge_after_filter.py
+-rw-rw-r--   0 root         (0)     1003   139084 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/small/test_dataframe.py
+-rw-rw-r--   0 root         (0)     1003    18961 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/small/test_dataframe_io.py
+-rw-rw-r--   0 root         (0)     1003    10570 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/small/test_encryption.py
+-rw-rw-r--   0 root         (0)     1003    12922 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/small/test_groupby.py
+-rw-rw-r--   0 root         (0)     1003     1558 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/small/test_ibis.py
+-rw-rw-r--   0 root         (0)     1003    13328 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/small/test_index.py
+-rw-rw-r--   0 root         (0)     1003     1205 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/small/test_ipython.py
+-rw-rw-r--   0 root         (0)     1003    41010 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/small/test_multiindex.py
+-rw-rw-r--   0 root         (0)     1003     4190 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/small/test_numpy.py
+-rw-rw-r--   0 root         (0)     1003    19608 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/small/test_pandas.py
+-rw-rw-r--   0 root         (0)     1003     9533 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/small/test_pandas_options.py
+-rw-rw-r--   0 root         (0)     1003     4126 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/small/test_progress_bar.py
+-rw-rw-r--   0 root         (0)     1003    26485 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/small/test_remote_function.py
+-rw-rw-r--   0 root         (0)     1003      913 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/small/test_scalar.py
+-rw-rw-r--   0 root         (0)     1003   107873 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/small/test_series.py
+-rw-rw-r--   0 root         (0)     1003    40359 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/small/test_session.py
+-rw-rw-r--   0 root         (0)     1003     3343 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/small/test_window.py
+-rw-rw-r--   0 root         (0)     1003    12113 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/utils.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.950384 bigframes-1.2.0/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      574 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.950384 bigframes-1.2.0/tests/unit/_config/
+-rw-rw-r--   0 root         (0)     1003      574 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/unit/_config/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2733 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/unit/_config/test_bigquery_options.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.954384 bigframes-1.2.0/tests/unit/core/
+-rw-rw-r--   0 root         (0)     1003      574 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/unit/core/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1619 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/unit/core/test_bf_utils.py
+-rw-rw-r--   0 root         (0)     1003     2966 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/unit/core/test_blocks.py
+-rw-rw-r--   0 root         (0)     1003     1553 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/unit/core/test_expression.py
+-rw-rw-r--   0 root         (0)     1003     1813 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/unit/core/test_log_adapter.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.954384 bigframes-1.2.0/tests/unit/ml/
+-rw-rw-r--   0 root         (0)     1003      574 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/unit/ml/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2323 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/unit/ml/test_api_primitives.py
+-rw-rw-r--   0 root         (0)     1003     6555 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/unit/ml/test_compose.py
+-rw-rw-r--   0 root         (0)     1003     7426 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/unit/ml/test_golden_sql.py
+-rw-rw-r--   0 root         (0)     1003     4058 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/unit/ml/test_pipeline.py
+-rw-rw-r--   0 root         (0)     1003    13063 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/unit/ml/test_sql.py
+-rw-rw-r--   0 root         (0)     1003     4842 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/unit/resources.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.954384 bigframes-1.2.0/tests/unit/session/
+-rw-rw-r--   0 root         (0)     1003      574 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/unit/session/__init__.py
+-rw-rw-r--   0 root         (0)     1003     4347 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/unit/session/test_clients.py
+-rw-rw-r--   0 root         (0)     1003     7809 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/unit/session/test_io_bigquery.py
+-rw-rw-r--   0 root         (0)     1003    18664 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/unit/session/test_io_pandas.py
+-rw-rw-r--   0 root         (0)     1003     6619 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/unit/session/test_session.py
+-rw-rw-r--   0 root         (0)     1003     1744 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/unit/test_clients.py
+-rw-rw-r--   0 root         (0)     1003     1056 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/unit/test_compute_options.py
+-rw-rw-r--   0 root         (0)     1003     6648 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/unit/test_core.py
+-rw-rw-r--   0 root         (0)     1003     2136 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/unit/test_dataframe.py
+-rw-rw-r--   0 root         (0)     1003     8819 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/unit/test_dtypes.py
+-rw-rw-r--   0 root         (0)     1003     1577 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/unit/test_features.py
+-rw-rw-r--   0 root         (0)     1003      528 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/unit/test_formatting_helper.py
+-rw-rw-r--   0 root         (0)     1003     1655 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/unit/test_formatting_helpers.py
+-rw-rw-r--   0 root         (0)     1003     4055 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/unit/test_pandas.py
+-rw-rw-r--   0 root         (0)     1003     1207 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/unit/test_remote_function.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.894392 bigframes-1.2.0/third_party/
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.958383 bigframes-1.2.0/third_party/bigframes_vendored/
+-rw-rw-r--   0 root         (0)     1003        0 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.958383 bigframes-1.2.0/third_party/bigframes_vendored/cpython/
+-rw-rw-r--   0 root         (0)     1003     2339 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/cpython/LICENSE
+-rw-rw-r--   0 root         (0)     1003        0 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/cpython/__init__.py
+-rw-rw-r--   0 root         (0)     1003    18854 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/cpython/_pprint.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.958383 bigframes-1.2.0/third_party/bigframes_vendored/google_cloud_bigquery/
+-rw-rw-r--   0 root         (0)     1003    11358 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/google_cloud_bigquery/LICENSE
+-rw-rw-r--   0 root         (0)     1003      574 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/google_cloud_bigquery/__init__.py
+-rw-rw-r--   0 root         (0)     1003     5290 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/google_cloud_bigquery/_pandas_helpers.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.958383 bigframes-1.2.0/third_party/bigframes_vendored/google_cloud_bigquery/tests/
+-rw-rw-r--   0 root         (0)     1003      574 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/google_cloud_bigquery/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.958383 bigframes-1.2.0/third_party/bigframes_vendored/google_cloud_bigquery/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      574 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/google_cloud_bigquery/tests/unit/__init__.py
+-rw-rw-r--   0 root         (0)     1003    14045 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/google_cloud_bigquery/tests/unit/test_pandas_helpers.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.958383 bigframes-1.2.0/third_party/bigframes_vendored/ibis/
+-rw-rw-r--   0 root         (0)     1003    11358 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/ibis/LICENSE.txt
+-rw-rw-r--   0 root         (0)     1003    11663 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/ibis/README.md
+-rw-rw-r--   0 root         (0)     1003        0 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/ibis/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.958383 bigframes-1.2.0/third_party/bigframes_vendored/ibis/backends/
+-rw-rw-r--   0 root         (0)     1003        0 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/ibis/backends/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.962383 bigframes-1.2.0/third_party/bigframes_vendored/ibis/backends/bigquery/
+-rw-rw-r--   0 root         (0)     1003      184 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/ibis/backends/bigquery/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2091 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/ibis/backends/bigquery/compiler.py
+-rw-rw-r--   0 root         (0)     1003     6600 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/ibis/backends/bigquery/datatypes.py
+-rw-rw-r--   0 root         (0)     1003     1582 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/ibis/backends/bigquery/registry.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.962383 bigframes-1.2.0/third_party/bigframes_vendored/ibis/expr/
+-rw-rw-r--   0 root         (0)     1003        0 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/ibis/expr/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.962383 bigframes-1.2.0/third_party/bigframes_vendored/ibis/expr/operations/
+-rw-rw-r--   0 root         (0)     1003      464 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/ibis/expr/operations/__init__.py
+-rw-rw-r--   0 root         (0)     1003      536 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/ibis/expr/operations/analytic.py
+-rw-rw-r--   0 root         (0)     1003      276 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/ibis/expr/operations/generic.py
+-rw-rw-r--   0 root         (0)     1003      263 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/ibis/expr/operations/json.py
+-rw-rw-r--   0 root         (0)     1003      690 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/ibis/expr/operations/reductions.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.962383 bigframes-1.2.0/third_party/bigframes_vendored/pandas/
+-rw-rw-r--   0 root         (0)     1003     2284 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/AUTHORS.md
+-rw-rw-r--   0 root         (0)     1003     1634 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/LICENSE
+-rw-rw-r--   0 root         (0)     1003    10620 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/README.md
+-rw-rw-r--   0 root         (0)     1003        0 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.962383 bigframes-1.2.0/third_party/bigframes_vendored/pandas/_config/
+-rw-rw-r--   0 root         (0)     1003     1347 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/_config/config.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.966382 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.966382 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/arrays/
+-rw-rw-r--   0 root         (0)     1003        0 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/arrays/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.966382 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/arrays/arrow/
+-rw-rw-r--   0 root         (0)     1003        0 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/arrays/arrow/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2824 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/arrays/arrow/accessors.py
+-rw-rw-r--   0 root         (0)     1003     3689 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/arrays/datetimelike.py
+-rw-rw-r--   0 root         (0)     1003     2086 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/common.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.970382 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/computation/
+-rw-rw-r--   0 root         (0)     1003     6944 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/computation/align.py
+-rw-rw-r--   0 root         (0)     1003     1543 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/computation/common.py
+-rw-rw-r--   0 root         (0)     1003     2295 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/computation/engines.py
+-rw-rw-r--   0 root         (0)     1003    12685 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/computation/eval.py
+-rw-rw-r--   0 root         (0)     1003    25132 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/computation/expr.py
+-rw-rw-r--   0 root         (0)     1003    16244 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/computation/ops.py
+-rw-rw-r--   0 root         (0)     1003     6477 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/computation/parsing.py
+-rw-rw-r--   0 root         (0)     1003    10303 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/computation/scope.py
+-rw-rw-r--   0 root         (0)     1003     4394 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/config_init.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.970382 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/dtypes/
+-rw-rw-r--   0 root         (0)     1003      707 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/dtypes/inference.py
+-rw-rw-r--   0 root         (0)     1003   224405 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/frame.py
+-rw-rw-r--   0 root         (0)     1003    40214 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/generic.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.970382 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/groupby/
+-rw-rw-r--   0 root         (0)     1003    12988 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/groupby/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.970382 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/indexes/
+-rw-rw-r--   0 root         (0)     1003        0 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/indexes/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9588 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/indexes/accessor.py
+-rw-rw-r--   0 root         (0)     1003    11461 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/indexes/base.py
+-rw-rw-r--   0 root         (0)     1003     2941 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/indexes/multi.py
+-rw-rw-r--   0 root         (0)     1003     2909 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/indexing.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.970382 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/reshape/
+-rw-rw-r--   0 root         (0)     1003        0 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/reshape/__init__.py
+-rw-rw-r--   0 root         (0)     1003     4372 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/reshape/concat.py
+-rw-rw-r--   0 root         (0)     1003     3804 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/reshape/encoding.py
+-rw-rw-r--   0 root         (0)     1003     3220 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/reshape/merge.py
+-rw-rw-r--   0 root         (0)     1003     5844 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/reshape/tile.py
+-rw-rw-r--   0 root         (0)     1003   130169 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/series.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.970382 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/strings/
+-rw-rw-r--   0 root         (0)     1003    37771 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/strings/accessor.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.974381 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/tools/
+-rw-rw-r--   0 root         (0)     1003        0 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/tools/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2964 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/tools/datetimes.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.974381 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/window/
+-rw-rw-r--   0 root         (0)     1003        0 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/window/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1350 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/window/rolling.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.974381 bigframes-1.2.0/third_party/bigframes_vendored/pandas/io/
+-rw-rw-r--   0 root         (0)     1003        0 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/io/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1269 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/io/common.py
+-rw-rw-r--   0 root         (0)     1003     6612 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/io/gbq.py
+-rw-rw-r--   0 root         (0)     1003     1428 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/io/parquet.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.974381 bigframes-1.2.0/third_party/bigframes_vendored/pandas/io/parsers/
+-rw-rw-r--   0 root         (0)     1003        0 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/io/parsers/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10553 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/io/parsers/readers.py
+-rw-rw-r--   0 root         (0)     1003     3130 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/io/pickle.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.974381 bigframes-1.2.0/third_party/bigframes_vendored/pandas/pandas/
+-rw-rw-r--   0 root         (0)     1003    12353 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/pandas/_typing.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.974381 bigframes-1.2.0/third_party/bigframes_vendored/pandas/plotting/
+-rw-rw-r--   0 root         (0)     1003    11128 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/plotting/_core.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.974381 bigframes-1.2.0/third_party/bigframes_vendored/pandas/util/
+-rw-rw-r--   0 root         (0)     1003      765 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/util/_exceptions.py
+-rw-rw-r--   0 root         (0)     1003     1573 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/util/_validators.py
+-rw-rw-r--   0 root         (0)     1003        0 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.978381 bigframes-1.2.0/third_party/bigframes_vendored/sklearn/
+-rw-rw-r--   0 root         (0)     1003     1532 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/sklearn/COPYING
+-rw-rw-r--   0 root         (0)     1003        0 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/sklearn/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6211 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/sklearn/base.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.978381 bigframes-1.2.0/third_party/bigframes_vendored/sklearn/cluster/
+-rw-rw-r--   0 root         (0)     1003     5924 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/sklearn/cluster/_kmeans.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.978381 bigframes-1.2.0/third_party/bigframes_vendored/sklearn/compose/
+-rw-rw-r--   0 root         (0)     1003     2014 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/sklearn/compose/_column_transformer.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.978381 bigframes-1.2.0/third_party/bigframes_vendored/sklearn/decomposition/
+-rw-rw-r--   0 root         (0)     1003     5387 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/sklearn/decomposition/_pca.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.978381 bigframes-1.2.0/third_party/bigframes_vendored/sklearn/ensemble/
+-rw-rw-r--   0 root         (0)     1003        0 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/sklearn/ensemble/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8979 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/sklearn/ensemble/_forest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.978381 bigframes-1.2.0/third_party/bigframes_vendored/sklearn/linear_model/
+-rw-rw-r--   0 root         (0)     1003     5417 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/sklearn/linear_model/_base.py
+-rw-rw-r--   0 root         (0)     1003     4348 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/sklearn/linear_model/_logistic.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.978381 bigframes-1.2.0/third_party/bigframes_vendored/sklearn/metrics/
+-rw-rw-r--   0 root         (0)     1003     9779 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/sklearn/metrics/_classification.py
+-rw-rw-r--   0 root         (0)     1003     6347 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/sklearn/metrics/_ranking.py
+-rw-rw-r--   0 root         (0)     1003     3550 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/sklearn/metrics/_regression.py
+-rw-rw-r--   0 root         (0)     1003     2121 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/sklearn/metrics/pairwise.py
+-rw-rw-r--   0 root         (0)     1003     2973 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/sklearn/pipeline.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.982380 bigframes-1.2.0/third_party/bigframes_vendored/sklearn/preprocessing/
+-rw-rw-r--   0 root         (0)     1003     4980 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/sklearn/preprocessing/_data.py
+-rw-rw-r--   0 root         (0)     1003     1523 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/sklearn/preprocessing/_discretization.py
+-rw-rw-r--   0 root         (0)     1003     3753 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/sklearn/preprocessing/_encoder.py
+-rw-rw-r--   0 root         (0)     1003     2085 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/sklearn/preprocessing/_label.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.982380 bigframes-1.2.0/third_party/bigframes_vendored/xgboost/
+-rw-rw-r--   0 root         (0)     1003    11348 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/xgboost/LICENSE
+-rw-rw-r--   0 root         (0)     1003        0 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/xgboost/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6921 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/xgboost/sklearn.py
```

### Comparing `bigframes-1.1.0/LICENSE` & `bigframes-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/MANIFEST.in` & `bigframes-1.2.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/PKG-INFO` & `bigframes-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigframes
-Version: 1.1.0
+Version: 1.2.0
 Summary: BigQuery DataFrames -- scalable analytics and machine learning with BigQuery
 Home-page: https://github.com/googleapis/python-bigquery-dataframes
 Author: Google LLC
 Author-email: bigframes-feedback@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `bigframes-1.1.0/README.rst` & `bigframes-1.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/bigframes/__init__.py` & `bigframes-1.2.0/bigframes/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/bigframes/_config/__init__.py` & `bigframes-1.2.0/bigframes/_config/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/bigframes/_config/bigquery_options.py` & `bigframes-1.2.0/bigframes/_config/bigquery_options.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/bigframes/_config/compute_options.py` & `bigframes-1.2.0/bigframes/_config/compute_options.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import dataclasses
 from typing import Optional
 
 
 @dataclasses.dataclass
 class ComputeOptions:
     """
-    Encapsulates configuration for compute options.
+    Encapsulates the configuration for compute options.
 
     **Examples:**
 
         >>> import bigframes.pandas as bpd
         >>> df = bpd.read_gbq("bigquery-public-data.ml_datasets.penguins")
 
         >>> bpd.options.compute.maximum_bytes_billed = 500
@@ -35,15 +35,15 @@
         >>> bpd.options.compute.maximum_bytes_billed = None  # reset option
 
     Attributes:
         maximum_bytes_billed (int, Options):
             Limits the bytes billed for query jobs. Queries that will have
             bytes billed beyond this limit will fail (without incurring a
             charge). If unspecified, this will be set to your project default.
-            See `maximum_bytes_billed <https://cloud.google.com/python/docs/reference/bigquery/latest/google.cloud.bigquery.job.QueryJobConfig#google_cloud_bigquery_job_QueryJobConfig_maximum_bytes_billed>`_.
+            See `maximum_bytes_billed`: https://cloud.google.com/python/docs/reference/bigquery/latest/google.cloud.bigquery.job.QueryJobConfig#google_cloud_bigquery_job_QueryJobConfig_maximum_bytes_billed.
         enable_multi_query_execution (bool, Options):
             If enabled, large queries may be factored into multiple smaller queries
             in order to avoid generating queries that are too complex for the query
             engine to handle. However this comes at the cost of increase cost and latency.
     """
 
     maximum_bytes_billed: Optional[int] = None
```

### Comparing `bigframes-1.1.0/bigframes/_config/display_options.py` & `bigframes-1.2.0/bigframes/_config/display_options.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/bigframes/_config/sampling_options.py` & `bigframes-1.2.0/bigframes/_config/sampling_options.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/bigframes/clients.py` & `bigframes-1.2.0/bigframes/clients.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/bigframes/core/__init__.py` & `bigframes-1.2.0/bigframes/core/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,16 +102,15 @@
 
         return (
             required_session if (required_session is not None) else get_global_session()
         )
 
     @functools.cached_property
     def schema(self) -> schemata.ArraySchema:
-        # TODO: switch to use self.node.schema
-        return self._compiled_schema
+        return self.node.schema
 
     @functools.cached_property
     def _compiled_schema(self) -> schemata.ArraySchema:
         compiled = self._compile_unordered()
         items = tuple(
             schemata.SchemaItem(id, compiled.get_column_type(id))
             for id in compiled.column_ids
```

### Comparing `bigframes-1.1.0/bigframes/core/block_transforms.py` & `bigframes-1.2.0/bigframes/core/block_transforms.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/bigframes/core/blocks.py` & `bigframes-1.2.0/bigframes/core/blocks.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 """
 
 from __future__ import annotations
 
 import dataclasses
 import functools
 import itertools
+import os
 import random
 import typing
 from typing import Iterable, List, Literal, Mapping, Optional, Sequence, Tuple
 import warnings
 
 import google.cloud.bigquery as bigquery
 import pandas as pd
@@ -37,18 +38,20 @@
 import bigframes.constants as constants
 import bigframes.core as core
 import bigframes.core.expression as ex
 import bigframes.core.expression as scalars
 import bigframes.core.guid as guid
 import bigframes.core.join_def as join_defs
 import bigframes.core.ordering as ordering
+import bigframes.core.schema as bf_schema
 import bigframes.core.tree_properties as tree_properties
 import bigframes.core.utils
 import bigframes.core.utils as utils
 import bigframes.dtypes
+import bigframes.features
 import bigframes.operations as ops
 import bigframes.operations.aggregations as agg_ops
 import bigframes.session._io.pandas
 
 # Type constraint for wherever column labels are used
 Label = typing.Hashable
 
@@ -407,15 +410,40 @@
         level_names = [self.col_id_to_index_name[index_id] for index_id in ids]
         return Block(self.expr, ids, self.column_labels, level_names)
 
     def _to_dataframe(self, result) -> pd.DataFrame:
         """Convert BigQuery data to pandas DataFrame with specific dtypes."""
         dtypes = dict(zip(self.index_columns, self.index.dtypes))
         dtypes.update(zip(self.value_columns, self.dtypes))
-        return self.session._rows_to_dataframe(result, dtypes)
+        result_dataframe = self.session._rows_to_dataframe(result, dtypes)
+        # Runs strict validations to ensure internal type predictions and ibis are completely in sync
+        # Do not execute these validations outside of testing suite.
+        if "PYTEST_CURRENT_TEST" in os.environ:
+            self._validate_result_schema(result_dataframe)
+        return result_dataframe
+
+    def _validate_result_schema(self, result_df: pd.DataFrame):
+        ibis_schema = self.expr._compiled_schema
+        internal_schema = self.expr.node.schema
+        actual_schema = bf_schema.ArraySchema(
+            tuple(
+                bf_schema.SchemaItem(name, dtype)  # type: ignore
+                for name, dtype in result_df.dtypes.items()
+            )
+        )
+        if not bigframes.features.PANDAS_VERSIONS.is_arrow_list_dtype_usable:
+            return
+        if internal_schema != actual_schema:
+            raise ValueError(
+                f"This error should only occur while testing. BigFrames internal schema: {internal_schema} does not match actual schema: {actual_schema}"
+            )
+        if ibis_schema != actual_schema:
+            raise ValueError(
+                f"This error should only occur while testing. Ibis schema: {ibis_schema} does not match actual schema: {actual_schema}"
+            )
 
     def to_pandas(
         self,
         max_download_size: Optional[int] = None,
         sampling_method: Optional[str] = None,
         random_state: Optional[int] = None,
         *,
@@ -1200,15 +1228,15 @@
         Standard stats should be:
             - commonly used
             - efficiently computable.
         """
         # TODO: annotate aggregations themself with this information
         dtype = self.expr.get_column_type(column_id)
         stats: list[agg_ops.UnaryAggregateOp] = [agg_ops.count_op]
-        if dtype not in bigframes.dtypes.UNORDERED_DTYPES:
+        if bigframes.dtypes.is_orderable(dtype):
             stats += [agg_ops.min_op, agg_ops.max_op]
         if dtype in bigframes.dtypes.NUMERIC_BIGFRAMES_TYPES_PERMISSIVE:
             # Notable exclusions:
             # prod op tends to cause overflows
             # Also, var_op is redundant as can be derived from std
             stats += [
                 agg_ops.std_op,
```

### Comparing `bigframes-1.1.0/bigframes/core/compile/__init__.py` & `bigframes-1.2.0/bigframes/core/compile/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/bigframes/core/compile/aggregate_compiler.py` & `bigframes-1.2.0/bigframes/core/compile/aggregate_compiler.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/bigframes/core/compile/compiled.py` & `bigframes-1.2.0/bigframes/core/compile/compiled.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/bigframes/core/compile/compiler.py` & `bigframes-1.2.0/bigframes/core/compile/compiler.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/bigframes/core/compile/concat.py` & `bigframes-1.2.0/bigframes/core/compile/concat.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/bigframes/core/compile/scalar_op_compiler.py` & `bigframes-1.2.0/bigframes/core/compile/scalar_op_compiler.py`

 * *Files 0% similar despite different names*

```diff
@@ -393,15 +393,15 @@
 @scalar_op_compiler.register_unary_op(ops.expm1_op)
 def expm1_op_impl(x: ibis_types.Value):
     return exp_op_impl(x) - _ibis_num(1)
 
 
 @scalar_op_compiler.register_unary_op(ops.invert_op)
 def invert_op_impl(x: ibis_types.Value):
-    return typing.cast(ibis_types.NumericValue, x).negate()
+    return x.__invert__()
 
 
 ## String Operation
 @scalar_op_compiler.register_unary_op(ops.len_op)
 def len_op_impl(x: ibis_types.Value):
     return typing.cast(ibis_types.StringValue, x).length().cast(ibis_dtypes.int64)
```

### Comparing `bigframes-1.1.0/bigframes/core/compile/single_column.py` & `bigframes-1.2.0/bigframes/core/compile/single_column.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 from typing import Mapping
 
 import ibis
 import ibis.expr.datatypes as ibis_dtypes
 import ibis.expr.types as ibis_types
 
 import bigframes.core.compile.compiled as compiled
+import bigframes.core.guid as guids
 import bigframes.core.join_def as join_defs
-import bigframes.core.joins as joining
 import bigframes.core.ordering as orderings
 
 
 def join_by_column_ordered(
     left: compiled.OrderedIR,
     right: compiled.OrderedIR,
     join: join_defs.JoinDefinition,
@@ -46,17 +46,21 @@
             perform a true JOIN in generated SQL.
     Returns:
         The joined expression. The resulting columns will be, in order,
         first the coalesced join keys, then, all the left columns, and
         finally, all the right columns.
     """
 
-    l_hidden_mapping, r_hidden_mapping = joining.JoinNameRemapper(namespace="hidden")(
-        left._hidden_column_ids, right._hidden_column_ids
-    )
+    l_hidden_mapping = {
+        id: guids.generate_guid("hidden_") for id in left._hidden_column_ids
+    }
+    r_hidden_mapping = {
+        id: guids.generate_guid("hidden_") for id in right._hidden_column_ids
+    }
+
     l_mapping = {**join.get_left_mapping(), **l_hidden_mapping}
     r_mapping = {**join.get_right_mapping(), **r_hidden_mapping}
 
     left_table = left._to_ibis_expr(
         ordering_mode="unordered",
         expose_hidden_cols=True,
         col_id_overrides=l_mapping,
```

### Comparing `bigframes-1.1.0/bigframes/core/convert.py` & `bigframes-1.2.0/bigframes/core/convert.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,21 +9,35 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from __future__ import annotations
 
+from typing import Optional
+
 import pandas as pd
 
 import bigframes.core.indexes as index
 import bigframes.series as series
 
 
-def to_bf_series(obj, default_index: index.Index) -> series.Series:
+def to_bf_series(obj, default_index: Optional[index.Index]) -> series.Series:
+    """
+    Convert a an object to a bigframes series
+
+    Args:
+        obj (list-like or Series):
+            Object to convert to bigframes Series
+        default_index (list-like or Index or None):
+            Index to use if obj has no index
+
+    Returns
+        bigframes.pandas.Series
+    """
     if isinstance(obj, series.Series):
         return obj
     if isinstance(obj, pd.Series):
         return series.Series(obj)
     if isinstance(obj, index.Index):
         return series.Series(obj, default_index)
     if isinstance(obj, pd.Index):
@@ -31,14 +45,26 @@
     if pd.api.types.is_list_like(obj):
         return series.Series(obj, default_index)
     else:
         raise TypeError(f"Cannot interpret {obj} as series.")
 
 
 def to_pd_series(obj, default_index: pd.Index) -> pd.Series:
+    """
+    Convert a an object to a pandas series
+
+    Args:
+        obj (list-like or Series):
+            Object to convert to pandas Series
+        default_index (list-like or Index or None):
+            Index to use if obj has no index
+
+    Returns
+        pandas.Series
+    """
     if isinstance(obj, series.Series):
         return obj.to_pandas()
     if isinstance(obj, pd.Series):
         return obj
     if isinstance(obj, index.Index):
         return pd.Series(obj.to_pandas(), default_index)
     if isinstance(obj, pd.Index):
```

### Comparing `bigframes-1.1.0/bigframes/core/eval.py` & `bigframes-1.2.0/bigframes/core/eval.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/bigframes/core/expression.py` & `bigframes-1.2.0/bigframes/core/expression.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/bigframes/core/global_session.py` & `bigframes-1.2.0/bigframes/core/global_session.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/bigframes/core/groupby/__init__.py` & `bigframes-1.2.0/bigframes/core/groupby/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/bigframes/core/guid.py` & `bigframes-1.2.0/bigframes/core/guid.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/bigframes/core/indexers.py` & `bigframes-1.2.0/bigframes/core/indexers.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,15 +188,23 @@
             self._dataframe._set_block(df._get_block())
         elif (
             isinstance(key, tuple)
             and len(key) == 2
             and isinstance(key[0], bigframes.series.Series)
             and key[0].dtype == "boolean"
         ) and pd.api.types.is_scalar(value):
-            new_column = key[0].map({True: value, False: None})
+            # For integer scalar, if set value to a new column, the dtype would be default to float.
+            # But if set value to an existing Int64 column, the dtype would still be integer.
+            # So we need to use different NaN type to match this behavior.
+            new_column = key[0].map(
+                {
+                    True: value,
+                    False: pd.NA if key[1] in self._dataframe.columns else None,
+                }
+            )
             try:
                 original_column = self._dataframe[key[1]]
             except KeyError:
                 self._dataframe[key[1]] = new_column
                 return
             try:
                 self._dataframe[key[1]] = new_column.fillna(original_column)
```

### Comparing `bigframes-1.1.0/bigframes/core/indexes/__init__.py` & `bigframes-1.2.0/bigframes/functions/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,13 @@
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
-from bigframes.core.indexes.base import Index
-
-__all__ = [
-    "Index",
-]
```

### Comparing `bigframes-1.1.0/bigframes/core/indexes/base.py` & `bigframes-1.2.0/bigframes/core/indexes/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,17 +38,23 @@
 if typing.TYPE_CHECKING:
     import bigframes.dataframe
     import bigframes.series
 
 
 class Index(vendored_pandas_index.Index):
     __doc__ = vendored_pandas_index.Index.__doc__
-
-    def __init__(
-        self,
+    _query_job = None
+    _block: blocks.Block
+    _linked_frame: Union[
+        bigframes.dataframe.DataFrame, bigframes.series.Series, None
+    ] = None
+
+    # Overrided on __new__ to create subclasses like pandas does
+    def __new__(
+        cls,
         data=None,
         dtype=None,
         *,
         name=None,
         session=None,
     ):
         import bigframes.dataframe as df
@@ -69,26 +75,38 @@
             index = Index(data=block)
             name = data.name if name is None else name
             if name is not None:
                 index.name = name
             if dtype is not None:
                 index = index.astype(dtype)
             block = index._block
+        elif isinstance(data, pandas.Index):
+            pd_df = pandas.DataFrame(index=data)
+            block = df.DataFrame(pd_df, session=session)._block
         else:
             pd_index = pandas.Index(data=data, dtype=dtype, name=name)
             pd_df = pandas.DataFrame(index=pd_index)
             block = df.DataFrame(pd_df, session=session)._block
-        self._query_job = None
-        self._block: blocks.Block = block
+
+        # TODO: Support more index subtypes
+        from bigframes.core.indexes.multi import MultiIndex
+
+        klass = MultiIndex if len(block._index_columns) > 1 else cls
+        result = typing.cast(Index, object.__new__(klass))
+        result._query_job = None
+        result._block = block
+        return result
 
     @classmethod
     def from_frame(
         cls, frame: Union[bigframes.series.Series, bigframes.dataframe.DataFrame]
     ) -> Index:
-        return FrameIndex(frame)
+        index = Index(frame._block)
+        index._linked_frame = frame
+        return index
 
     @property
     def name(self) -> blocks.Label:
         names = self.names
         if len(names) == 1:
             return self.names[0]
         else:
@@ -103,14 +121,18 @@
     def names(self) -> typing.Sequence[blocks.Label]:
         """Returns the names of the Index."""
         return self._block._index_labels
 
     @names.setter
     def names(self, values: typing.Sequence[blocks.Label]):
         new_block = self._block.with_index_labels(values)
+        if self._linked_frame is not None:
+            self._linked_frame._set_block(
+                self._linked_frame._block.with_index_labels(values)
+            )
         self._block = new_block
 
     @property
     def nlevels(self) -> int:
         return len(self._block.index_columns)
 
     @property
@@ -448,30 +470,7 @@
     def to_numpy(self, dtype=None, **kwargs) -> np.ndarray:
         return self.to_pandas().to_numpy(dtype, **kwargs)
 
     __array__ = to_numpy
 
     def __len__(self):
         return self.shape[0]
-
-
-# Index that mutates the originating dataframe/series
-class FrameIndex(Index):
-    def __init__(
-        self,
-        series_or_dataframe: typing.Union[
-            bigframes.series.Series, bigframes.dataframe.DataFrame
-        ],
-    ):
-        super().__init__(series_or_dataframe._block)
-        self._whole_frame = series_or_dataframe
-
-    @property
-    def names(self) -> typing.Sequence[blocks.Label]:
-        """Returns the names of the Index."""
-        return self._block._index_labels
-
-    @names.setter
-    def names(self, values: typing.Sequence[blocks.Label]):
-        new_block = self._whole_frame._get_block().with_index_labels(values)
-        self._whole_frame._set_block(new_block)
-        self._block = new_block
```

### Comparing `bigframes-1.1.0/bigframes/core/join_def.py` & `bigframes-1.2.0/bigframes/core/join_def.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/bigframes/core/joins/__init__.py` & `bigframes-1.2.0/bigframes/core/indexes/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,13 +8,14 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Helpers to join ArrayValue objects."""
+from bigframes.core.indexes.base import Index
+from bigframes.core.indexes.multi import MultiIndex
 
-from bigframes.core.joins.merge import merge
-from bigframes.core.joins.name_resolution import JoinNameRemapper
-
-__all__ = ("merge", "JoinNameRemapper")
+__all__ = [
+    "Index",
+    "MultiIndex",
+]
```

### Comparing `bigframes-1.1.0/bigframes/core/joins/merge.py` & `bigframes-1.2.0/bigframes/core/joins/merge.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/bigframes/core/local_data.py` & `bigframes-1.2.0/bigframes/core/local_data.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/bigframes/core/log_adapter.py` & `bigframes-1.2.0/bigframes/core/log_adapter.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/bigframes/core/nodes.py` & `bigframes-1.2.0/bigframes/core/nodes.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/bigframes/core/ordering.py` & `bigframes-1.2.0/bigframes/core/ordering.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/bigframes/core/reshape/__init__.py` & `bigframes-1.2.0/bigframes/core/reshape/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from __future__ import annotations
 
 import typing
-from typing import Iterable, Literal, Optional, Tuple, Union
+from typing import Iterable, Literal, Optional, Union
 
 import pandas as pd
 
 import bigframes.constants as constants
 import bigframes.core as core
 import bigframes.core.expression as ex
 import bigframes.core.ordering as order
@@ -109,29 +109,49 @@
 
 
 def cut(
     x: bigframes.series.Series,
     bins: Union[
         int,
         pd.IntervalIndex,
-        Iterable[Tuple[Union[int, float], Union[int, float]]],
+        Iterable,
     ],
     *,
     labels: Optional[bool] = None,
 ) -> bigframes.series.Series:
     if isinstance(bins, int) and bins <= 0:
         raise ValueError("`bins` should be a positive integer.")
 
     if isinstance(bins, Iterable):
         if isinstance(bins, pd.IntervalIndex):
             as_index: pd.IntervalIndex = bins
             bins = tuple((bin.left.item(), bin.right.item()) for bin in bins)
-        else:
+        elif len(list(bins)) == 0:
+            raise ValueError("`bins` iterable should have at least one item")
+        elif isinstance(list(bins)[0], tuple):
             as_index = pd.IntervalIndex.from_tuples(list(bins))
             bins = tuple(bins)
+        elif pd.api.types.is_number(list(bins)[0]):
+            bins_list = list(bins)
+            if len(bins_list) < 2:
+                raise ValueError(
+                    "`bins` iterable of numeric breaks should have"
+                    " at least two items"
+                )
+            as_index = pd.IntervalIndex.from_breaks(bins_list)
+            single_type = all([isinstance(n, type(bins_list[0])) for n in bins_list])
+            numeric_type = type(bins_list[0]) if single_type else float
+            bins = tuple(
+                [
+                    (numeric_type(bins_list[i]), numeric_type(bins_list[i + 1]))
+                    for i in range(len(bins_list) - 1)
+                ]
+            )
+        else:
+            raise ValueError("`bins` iterable should contain tuples or numerics")
 
         if as_index.is_overlapping:
             raise ValueError("Overlapping IntervalIndex is not accepted.")
 
     if labels is not None and labels is not False:
         raise NotImplementedError(
             "The 'labels' parameter must be either False or None. "
```

### Comparing `bigframes-1.1.0/bigframes/core/rewrite.py` & `bigframes-1.2.0/bigframes/core/rewrite.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/bigframes/core/scalar.py` & `bigframes-1.2.0/bigframes/core/scalar.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/bigframes/core/schema.py` & `bigframes-1.2.0/bigframes/core/schema.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/bigframes/core/tools/__init__.py` & `bigframes-1.2.0/bigframes/core/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/bigframes/core/tools/datetimes.py` & `bigframes-1.2.0/bigframes/core/tools/datetimes.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/bigframes/core/tree_properties.py` & `bigframes-1.2.0/bigframes/core/tree_properties.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/bigframes/core/utils.py` & `bigframes-1.2.0/bigframes/core/utils.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/bigframes/core/window/__init__.py` & `bigframes-1.2.0/bigframes/core/window/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/bigframes/core/window_spec.py` & `bigframes-1.2.0/bigframes/core/window_spec.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/bigframes/dataframe.py` & `bigframes-1.2.0/bigframes/dataframe.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 
 """DataFrame is a two dimensional data structure."""
 
 from __future__ import annotations
 
 import datetime
-import os
+import inspect
 import re
 import sys
 import textwrap
 import typing
 from typing import (
     Callable,
     Dict,
@@ -171,19 +171,14 @@
             )
             if session:
                 self._block = session.read_pandas(pd_dataframe)._get_block()
             else:
                 self._block = bigframes.pandas.read_pandas(pd_dataframe)._get_block()
         self._query_job: Optional[bigquery.QueryJob] = None
 
-        # Runs strict validations to ensure internal type predictions and ibis are completely in sync
-        # Do not execute these validations outside of testing suite.
-        if "PYTEST_CURRENT_TEST" in os.environ:
-            self._block.expr.validate_schema()
-
     def __dir__(self):
         return dir(type(self)) + [
             label
             for label in self._block.column_labels
             if label and isinstance(label, str)
         ]
 
@@ -316,14 +311,16 @@
     def _session(self) -> bigframes.Session:
         return self._get_block().expr.session
 
     def __len__(self):
         rows, _ = self.shape
         return rows
 
+    __len__.__doc__ = inspect.getdoc(vendored_pandas_frame.DataFrame.__len__)
+
     def __iter__(self):
         return iter(self.columns)
 
     def astype(
         self,
         dtype: Union[bigframes.dtypes.DtypeString, bigframes.dtypes.Dtype],
     ) -> DataFrame:
@@ -468,15 +465,14 @@
             blocks.Label,
             Sequence[blocks.Label],
             # Index of column labels can be treated the same as a sequence of column labels.
             pandas.Index,
             bigframes.series.Series,
         ],
     ):  # No return type annotations (like pandas) as type cannot always be determined statically
-        """Gets the specified column(s) from the DataFrame."""
         # NOTE: This implements the operations described in
         # https://pandas.pydata.org/docs/getting_started/intro_tutorials/03_subset_data.html
 
         if isinstance(key, bigframes.series.Series):
             return self._getitem_bool_series(key)
 
         if isinstance(key, typing.Hashable):
@@ -500,14 +496,16 @@
         selected_ids: Tuple[str, ...] = ()
         for label in key:
             col_ids = self._block.label_to_col_id[label]
             selected_ids = (*selected_ids, *col_ids)
 
         return DataFrame(self._block.select_columns(selected_ids))
 
+    __getitem__.__doc__ = inspect.getdoc(vendored_pandas_frame.DataFrame.__getitem__)
+
     def _getitem_label(self, key: blocks.Label):
         col_ids = self._block.cols_matching_label(key)
         if len(col_ids) == 0:
             raise KeyError(key)
         block = self._block.select_columns(col_ids)
         if isinstance(self.columns, pandas.MultiIndex):
             # Multiindex should drop-level if not selecting entire
@@ -644,22 +642,19 @@
             # _repr_html_ stub is missing so mypy thinks it's a Series. Ignore mypy.
             html_string = pandas_df._repr_html_()  # type:ignore
 
         html_string += f"[{row_count} rows x {column_count} columns in total]"
         return html_string
 
     def __setitem__(self, key: str, value: SingleItemValue):
-        """Modify or insert a column into the DataFrame.
-
-        Note: This does **not** modify the original table the DataFrame was
-        derived from.
-        """
         df = self._assign_single_item(key, value)
         self._set_block(df._get_block())
 
+    __setitem__.__doc__ = inspect.getdoc(vendored_pandas_frame.DataFrame.__setitem__)
+
     def _apply_binop(
         self,
         other: float | int | bigframes.series.Series | DataFrame,
         op,
         axis: str | int = "columns",
         how: str = "outer",
         reverse: bool = False,
@@ -840,138 +835,229 @@
 
         block = block.select_columns(binop_result_ids).with_column_labels(columns)
         return DataFrame(block)
 
     def eq(self, other: typing.Any, axis: str | int = "columns") -> DataFrame:
         return self._apply_binop(other, ops.eq_op, axis=axis)
 
+    def __eq__(self, other) -> DataFrame:  # type: ignore
+        return self.eq(other)
+
+    __eq__.__doc__ = inspect.getdoc(vendored_pandas_frame.DataFrame.__eq__)
+
     def ne(self, other: typing.Any, axis: str | int = "columns") -> DataFrame:
         return self._apply_binop(other, ops.ne_op, axis=axis)
 
-    __eq__ = eq  # type: ignore
+    def __ne__(self, other) -> DataFrame:  # type: ignore
+        return self.ne(other)
 
-    __ne__ = ne  # type: ignore
+    __ne__.__doc__ = inspect.getdoc(vendored_pandas_frame.DataFrame.__ne__)
 
     def le(self, other: typing.Any, axis: str | int = "columns") -> DataFrame:
         return self._apply_binop(other, ops.le_op, axis=axis)
 
+    def __le__(self, other) -> DataFrame:
+        return self.le(other)
+
+    __le__.__doc__ = inspect.getdoc(vendored_pandas_frame.DataFrame.__le__)
+
     def lt(self, other: typing.Any, axis: str | int = "columns") -> DataFrame:
         return self._apply_binop(other, ops.lt_op, axis=axis)
 
+    def __lt__(self, other) -> DataFrame:
+        return self.lt(other)
+
+    __lt__.__doc__ = inspect.getdoc(vendored_pandas_frame.DataFrame.__lt__)
+
     def ge(self, other: typing.Any, axis: str | int = "columns") -> DataFrame:
         return self._apply_binop(other, ops.ge_op, axis=axis)
 
-    def gt(self, other: typing.Any, axis: str | int = "columns") -> DataFrame:
-        return self._apply_binop(other, ops.gt_op, axis=axis)
+    def __ge__(self, other) -> DataFrame:
+        return self.ge(other)
 
-    __lt__ = lt
+    __ge__.__doc__ = inspect.getdoc(vendored_pandas_frame.DataFrame.__ge__)
 
-    __le__ = le
+    def gt(self, other: typing.Any, axis: str | int = "columns") -> DataFrame:
+        return self._apply_binop(other, ops.gt_op, axis=axis)
 
-    __gt__ = gt
+    def __gt__(self, other) -> DataFrame:
+        return self.gt(other)
 
-    __ge__ = ge
+    __gt__.__doc__ = inspect.getdoc(vendored_pandas_frame.DataFrame.__gt__)
 
     def add(
         self,
         other: float | int | bigframes.series.Series | DataFrame,
         axis: str | int = "columns",
     ) -> DataFrame:
         # TODO(swast): Support fill_value parameter.
         # TODO(swast): Support level parameter with MultiIndex.
         return self._apply_binop(other, ops.add_op, axis=axis)
 
-    __radd__ = __add__ = radd = add
+    def radd(
+        self,
+        other: float | int | bigframes.series.Series | DataFrame,
+        axis: str | int = "columns",
+    ) -> DataFrame:
+        # TODO(swast): Support fill_value parameter.
+        # TODO(swast): Support level parameter with MultiIndex.
+        return self.add(other, axis=axis)
+
+    def __add__(self, other) -> DataFrame:
+        return self.add(other)
+
+    __add__.__doc__ = inspect.getdoc(vendored_pandas_frame.DataFrame.__add__)
+
+    __radd__ = __add__
 
     def sub(
         self,
         other: float | int | bigframes.series.Series | DataFrame,
         axis: str | int = "columns",
     ) -> DataFrame:
         return self._apply_binop(other, ops.sub_op, axis=axis)
 
-    __sub__ = subtract = sub
+    subtract = sub
+    subtract.__doc__ = inspect.getdoc(vendored_pandas_frame.DataFrame.sub)
+
+    def __sub__(self, other):
+        return self.sub(other)
+
+    __sub__.__doc__ = inspect.getdoc(vendored_pandas_frame.DataFrame.__sub__)
 
     def rsub(
         self,
         other: float | int | bigframes.series.Series | DataFrame,
         axis: str | int = "columns",
     ) -> DataFrame:
         return self._apply_binop(other, ops.sub_op, axis=axis, reverse=True)
 
-    __rsub__ = rsub
+    def __rsub__(self, other):
+        return self.rsub(other)
+
+    __rsub__.__doc__ = inspect.getdoc(vendored_pandas_frame.DataFrame.__rsub__)
 
     def mul(
         self,
         other: float | int | bigframes.series.Series | DataFrame,
         axis: str | int = "columns",
     ) -> DataFrame:
         return self._apply_binop(other, ops.mul_op, axis=axis)
 
-    __rmul__ = __mul__ = rmul = multiply = mul
+    multiply = mul
+    multiply.__doc__ = inspect.getdoc(vendored_pandas_frame.DataFrame.mul)
+
+    def __mul__(self, other):
+        return self.mul(other)
+
+    __mul__.__doc__ = inspect.getdoc(vendored_pandas_frame.DataFrame.__mul__)
+
+    def rmul(
+        self,
+        other: float | int | bigframes.series.Series | DataFrame,
+        axis: str | int = "columns",
+    ) -> DataFrame:
+        return self.mul(other, axis=axis)
+
+    def __rmul__(self, other):
+        return self.rmul(other)
+
+    __rmul__.__doc__ = inspect.getdoc(vendored_pandas_frame.DataFrame.__rmul__)
 
     def truediv(
         self,
         other: float | int | bigframes.series.Series | DataFrame,
         axis: str | int = "columns",
     ) -> DataFrame:
         return self._apply_binop(other, ops.div_op, axis=axis)
 
-    div = divide = __truediv__ = truediv
+    truediv.__doc__ = inspect.getdoc(vendored_pandas_frame.DataFrame.truediv)
+    div = divide = truediv
+
+    def __truediv__(self, other):
+        return self.truediv(other)
+
+    __truediv__.__doc__ = inspect.getdoc(vendored_pandas_frame.DataFrame.__truediv__)
 
     def rtruediv(
         self,
         other: float | int | bigframes.series.Series | DataFrame,
         axis: str | int = "columns",
     ) -> DataFrame:
         return self._apply_binop(other, ops.div_op, axis=axis, reverse=True)
 
-    __rtruediv__ = rdiv = rtruediv
+    rdiv = rtruediv
+    rdiv.__doc__ = inspect.getdoc(vendored_pandas_frame.DataFrame.rtruediv)
+
+    def __rtruediv__(self, other):
+        return self.rtruediv(other)
+
+    __rtruediv__.__doc__ = inspect.getdoc(vendored_pandas_frame.DataFrame.__rtruediv__)
 
     def floordiv(
         self,
         other: float | int | bigframes.series.Series | DataFrame,
         axis: str | int = "columns",
     ) -> DataFrame:
         return self._apply_binop(other, ops.floordiv_op, axis=axis)
 
-    __floordiv__ = floordiv
+    def __floordiv__(self, other):
+        return self.floordiv(other)
+
+    __floordiv__.__doc__ = inspect.getdoc(vendored_pandas_frame.DataFrame.__floordiv__)
 
     def rfloordiv(
         self,
         other: float | int | bigframes.series.Series | DataFrame,
         axis: str | int = "columns",
     ) -> DataFrame:
         return self._apply_binop(other, ops.floordiv_op, axis=axis, reverse=True)
 
-    __rfloordiv__ = rfloordiv
+    def __rfloordiv__(self, other):
+        return self.rfloordiv(other)
+
+    __rfloordiv__.__doc__ = inspect.getdoc(
+        vendored_pandas_frame.DataFrame.__rfloordiv__
+    )
 
     def mod(self, other: int | bigframes.series.Series | DataFrame, axis: str | int = "columns") -> DataFrame:  # type: ignore
         return self._apply_binop(other, ops.mod_op, axis=axis)
 
+    def __mod__(self, other):
+        return self.mod(other)
+
+    __mod__.__doc__ = inspect.getdoc(vendored_pandas_frame.DataFrame.__mod__)
+
     def rmod(self, other: int | bigframes.series.Series | DataFrame, axis: str | int = "columns") -> DataFrame:  # type: ignore
         return self._apply_binop(other, ops.mod_op, axis=axis, reverse=True)
 
-    __mod__ = mod
+    def __rmod__(self, other):
+        return self.rmod(other)
 
-    __rmod__ = rmod
+    __rmod__.__doc__ = inspect.getdoc(vendored_pandas_frame.DataFrame.__rmod__)
 
     def pow(
         self, other: int | bigframes.series.Series, axis: str | int = "columns"
     ) -> DataFrame:
         return self._apply_binop(other, ops.pow_op, axis=axis)
 
+    def __pow__(self, other):
+        return self.pow(other)
+
+    __pow__.__doc__ = inspect.getdoc(vendored_pandas_frame.DataFrame.__pow__)
+
     def rpow(
         self, other: int | bigframes.series.Series, axis: str | int = "columns"
     ) -> DataFrame:
         return self._apply_binop(other, ops.pow_op, axis=axis, reverse=True)
 
-    __pow__ = pow
+    def __rpow__(self, other):
+        return self.rpow(other)
 
-    __rpow__ = rpow
+    __rpow__.__doc__ = inspect.getdoc(vendored_pandas_frame.DataFrame.__rpow__)
 
     def align(
         self,
         other: typing.Union[DataFrame, bigframes.series.Series],
         join: str = "outer",
         axis: typing.Union[str, int, None] = None,
     ) -> typing.Tuple[
@@ -1973,14 +2059,15 @@
             frame = self._raise_on_non_numeric("prod")
         else:
             frame = self._drop_non_numeric()
         block = frame._block.aggregate_all_and_stack(agg_ops.product_op, axis=axis)
         return bigframes.series.Series(block.select_column("values"))
 
     product = prod
+    product.__doc__ = inspect.getdoc(vendored_pandas_frame.DataFrame.prod)
 
     def count(self, *, numeric_only: bool = False) -> bigframes.series.Series:
         if not numeric_only:
             frame = self
         else:
             frame = self._drop_non_numeric()
         block = frame._block.aggregate_all_and_stack(agg_ops.count_op)
@@ -2012,14 +2099,15 @@
             return bigframes.series.Series(
                 self._block.aggregate_all_and_stack(
                     agg_ops.lookup_agg_func(typing.cast(str, func))
                 )
             )
 
     aggregate = agg
+    aggregate.__doc__ = inspect.getdoc(vendored_pandas_frame.DataFrame.agg)
 
     def idxmin(self) -> bigframes.series.Series:
         return bigframes.series.Series(block_ops.idxmin(self._block))
 
     def idxmax(self) -> bigframes.series.Series:
         return bigframes.series.Series(block_ops.idxmax(self._block))
 
@@ -2085,14 +2173,15 @@
             frame = self._raise_on_non_numeric("kurt")
         else:
             frame = self._drop_non_numeric()
         result_block = block_ops.kurt(frame._block, frame._block.value_columns)
         return bigframes.series.Series(result_block)
 
     kurtosis = kurt
+    kurtosis.__doc__ = inspect.getdoc(vendored_pandas_frame.DataFrame.kurt)
 
     def _pivot(
         self,
         *,
         columns: typing.Union[blocks.Label, Sequence[blocks.Label]],
         columns_unique_values: typing.Optional[
             typing.Union[pandas.Index, Sequence[object]]
@@ -2134,14 +2223,74 @@
         ] = None,
         values: typing.Optional[
             typing.Union[blocks.Label, Sequence[blocks.Label]]
         ] = None,
     ) -> DataFrame:
         return self._pivot(columns=columns, index=index, values=values)
 
+    def pivot_table(
+        self,
+        values: typing.Optional[
+            typing.Union[blocks.Label, Sequence[blocks.Label]]
+        ] = None,
+        index: typing.Optional[
+            typing.Union[blocks.Label, Sequence[blocks.Label]]
+        ] = None,
+        columns: typing.Union[blocks.Label, Sequence[blocks.Label]] = None,
+        aggfunc: str = "mean",
+    ) -> DataFrame:
+        if isinstance(index, Iterable) and not (
+            isinstance(index, blocks.Label) and index in self.columns
+        ):
+            index = list(index)
+        else:
+            index = [index]
+
+        if isinstance(columns, Iterable) and not (
+            isinstance(columns, blocks.Label) and columns in self.columns
+        ):
+            columns = list(columns)
+        else:
+            columns = [columns]
+
+        if isinstance(values, Iterable) and not (
+            isinstance(values, blocks.Label) and values in self.columns
+        ):
+            values = list(values)
+        else:
+            values = [values]
+
+        # Unlike pivot, pivot_table has values always ordered.
+        values.sort()
+
+        keys = index + columns
+        agged = self.groupby(keys, dropna=True)[values].agg(aggfunc)
+
+        if isinstance(agged, bigframes.series.Series):
+            agged = agged.to_frame()
+
+        agged = agged.dropna(how="all")
+
+        if len(values) == 1:
+            agged = agged.rename(columns={agged.columns[0]: values[0]})
+
+        agged = agged.reset_index()
+
+        pivoted = agged.pivot(
+            columns=columns,
+            index=index,
+            values=values if len(values) > 1 else None,
+        ).sort_index()
+
+        # TODO: Remove the reordering step once the issue is resolved.
+        # The pivot_table method results in multi-index columns that are always ordered.
+        # However, the order of the pivoted result columns is not guaranteed to be sorted.
+        # Sort and reorder.
+        return pivoted[pivoted.columns.sort_values()]
+
     def stack(self, level: LevelsType = -1):
         if not isinstance(self.columns, pandas.MultiIndex):
             if level not in [0, -1, self.columns.name]:
                 raise IndexError(f"Invalid level {level} for single-level index")
             return self._stack_mono()
         return self._stack_multi(level)
 
@@ -2484,19 +2633,21 @@
     def abs(self) -> DataFrame:
         return self._apply_unary_op(ops.abs_op)
 
     def isna(self) -> DataFrame:
         return self._apply_unary_op(ops.isnull_op)
 
     isnull = isna
+    isnull.__doc__ = inspect.getdoc(vendored_pandas_frame.DataFrame.isna)
 
     def notna(self) -> DataFrame:
         return self._apply_unary_op(ops.notnull_op)
 
     notnull = notna
+    notnull.__doc__ = inspect.getdoc(vendored_pandas_frame.DataFrame.notna)
 
     def cumsum(self):
         is_numeric_types = [
             (dtype in bigframes.dtypes.NUMERIC_BIGFRAMES_TYPES_PERMISSIVE)
             for _, dtype in self.dtypes.items()
         ]
         if not all(is_numeric_types):
@@ -2802,15 +2953,18 @@
         return destination_table
 
     def to_numpy(
         self, dtype=None, copy=False, na_value=None, **kwargs
     ) -> numpy.ndarray:
         return self.to_pandas().to_numpy(dtype, copy, na_value, **kwargs)
 
-    __array__ = to_numpy
+    def __array__(self, dtype=None) -> numpy.ndarray:
+        return self.to_numpy(dtype=dtype)
+
+    __array__.__doc__ = inspect.getdoc(vendored_pandas_frame.DataFrame.__array__)
 
     def to_parquet(
         self,
         path: str,
         *,
         compression: Optional[Literal["snappy", "gzip"]] = "snappy",
         index: bool = True,
@@ -3169,14 +3323,15 @@
         df = self._drop_non_numeric() if numeric_only else self
         return DataFrame(block_ops.rank(df._block, method, na_option, ascending))
 
     def first_valid_index(self):
         return
 
     applymap = map
+    applymap.__doc__ = inspect.getdoc(vendored_pandas_frame.DataFrame.map)
 
     def _slice(
         self,
         start: typing.Optional[int] = None,
         stop: typing.Optional[int] = None,
         step: typing.Optional[int] = None,
     ) -> DataFrame:
@@ -3309,8 +3464,11 @@
 
         return result
 
     @property
     def plot(self):
         return plotting.PlotAccessor(self)
 
-    __matmul__ = dot
+    def __matmul__(self, other) -> DataFrame:
+        return self.dot(other)
+
+    __matmul__.__doc__ = inspect.getdoc(vendored_pandas_frame.DataFrame.__matmul__)
```

### Comparing `bigframes-1.1.0/bigframes/dtypes.py` & `bigframes-1.2.0/bigframes/dtypes.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,21 +53,19 @@
 BOOL_DTYPE = pd.BooleanDtype()
 STRING_DTYPE = pd.StringDtype(storage="pyarrow")
 BYTES_DTYPE = pd.ArrowDtype(pa.binary())
 DATE_DTYPE = pd.ArrowDtype(pa.date32())
 TIME_DTYPE = pd.ArrowDtype(pa.time64("us"))
 DATETIME_DTYPE = pd.ArrowDtype(pa.timestamp("us"))
 TIMESTAMP_DTYPE = pd.ArrowDtype(pa.timestamp("us", tz="UTC"))
+GEO_DTYPE = gpd.array.GeometryDtype()
 
 # Used when storing Null expressions
 DEFAULT_DTYPE = FLOAT_DTYPE
 
-# On BQ side, ARRAY, STRUCT, GEOGRAPHY, JSON are not orderable
-UNORDERED_DTYPES = [gpd.array.GeometryDtype()]
-
 # Type hints for dtype strings supported by BigQuery DataFrame
 DtypeString = Literal[
     "boolean",
     "Float64",
     "Int64",
     "int64[pyarrow]",
     "string",
@@ -130,35 +128,41 @@
 
 def is_array_like(type: ExpressionType) -> bool:
     return isinstance(type, pd.ArrowDtype) and isinstance(
         type.pyarrow_dtype, pa.ListType
     )
 
 
+def is_struct_like(type: ExpressionType) -> bool:
+    return isinstance(type, pd.ArrowDtype) and isinstance(
+        type.pyarrow_dtype, pa.StructType
+    )
+
+
 def is_numeric(type: ExpressionType) -> bool:
     return type in NUMERIC_BIGFRAMES_TYPES_PERMISSIVE
 
 
 def is_iterable(type: ExpressionType) -> bool:
     return type in (STRING_DTYPE, BYTES_DTYPE) or is_array_like(type)
 
 
 def is_comparable(type: ExpressionType) -> bool:
-    return (type is not None) and (type not in UNORDERED_DTYPES)
+    return (type is not None) and is_orderable(type)
 
 
-# Type hints for Ibis data types that can be read to Python objects by BigQuery DataFrame
-ReadOnlyIbisDtype = Union[
-    ibis_dtypes.Binary,
-    ibis_dtypes.JSON,
-    ibis_dtypes.Decimal,
-    ibis_dtypes.GeoSpatial,
-    ibis_dtypes.Array,
-    ibis_dtypes.Struct,
-]
+def is_orderable(type: ExpressionType) -> bool:
+    # On BQ side, ARRAY, STRUCT, GEOGRAPHY, JSON are not orderable
+    return not is_array_like(type) and not is_struct_like(type) and (type != GEO_DTYPE)
+
+
+def is_bool_coercable(type: ExpressionType) -> bool:
+    # TODO: Implement more bool coercions
+    return (type is None) or is_numeric(type) or is_string_like(type)
+
 
 BIDIRECTIONAL_MAPPINGS: Iterable[Tuple[IbisDtype, Dtype]] = (
     (ibis_dtypes.boolean, pd.BooleanDtype()),
     (ibis_dtypes.date, pd.ArrowDtype(pa.date32())),
     (ibis_dtypes.float64, pd.Float64Dtype()),
     (ibis_dtypes.int64, pd.Int64Dtype()),
     (ibis_dtypes.string, pd.StringDtype(storage="pyarrow")),
```

### Comparing `bigframes-1.1.0/bigframes/features.py` & `bigframes-1.2.0/bigframes/features.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/bigframes/formatting_helpers.py` & `bigframes-1.2.0/bigframes/formatting_helpers.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/bigframes/functions/__init__.py` & `bigframes-1.2.0/bigframes/version.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-# Copyright 2024 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
+__version__ = "1.2.0"
```

### Comparing `bigframes-1.1.0/bigframes/functions/remote_function.py` & `bigframes-1.2.0/bigframes/functions/remote_function.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/bigframes/ml/__init__.py` & `bigframes-1.2.0/bigframes/ml/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/bigframes/ml/base.py` & `bigframes-1.2.0/bigframes/ml/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,15 +189,15 @@
     def to_gbq(self: _T, model_name: str, replace: bool = False) -> _T:
         """Save the transformer as a BigQuery model.
 
         Args:
             model_name (str):
                 The name of the model.
             replace (bool, default False):
-                Whether to replace if the model already exists. Default to False.
+                Determine whether to replace if the model already exists. Default to False.
 
         Returns:
             Saved transformer."""
         if not self._bqml_model:
             raise RuntimeError("A transformer must be fitted before it can be saved")
 
         new_model = self._bqml_model.copy(model_name, replace)
```

### Comparing `bigframes-1.1.0/bigframes/ml/cluster.py` & `bigframes-1.2.0/bigframes/ml/cluster.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,15 +173,15 @@
     def to_gbq(self, model_name: str, replace: bool = False) -> KMeans:
         """Save the model to BigQuery.
 
         Args:
             model_name (str):
                 the name of the model.
             replace (bool, default False):
-                whether to replace if the model already exists. Default to False.
+                Determine whether to replace if the model already exists. Default to False.
 
         Returns:
             KMeans: saved model."""
         if not self._bqml_model:
             raise RuntimeError("A model must be fitted before it can be saved")
 
         new_model = self._bqml_model.copy(model_name, replace)
```

### Comparing `bigframes-1.1.0/bigframes/ml/compose.py` & `bigframes-1.2.0/bigframes/ml/compose.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/bigframes/ml/core.py` & `bigframes-1.2.0/bigframes/ml/core.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/bigframes/ml/decomposition.py` & `bigframes-1.2.0/bigframes/ml/decomposition.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,15 +167,15 @@
     def to_gbq(self, model_name: str, replace: bool = False) -> PCA:
         """Save the model to BigQuery.
 
         Args:
             model_name (str):
                 the name of the model.
             replace (bool, default False):
-                whether to replace if the model already exists. Default to False.
+                Determine whether to replace if the model already exists. Default to False.
 
         Returns:
             PCA: saved model."""
         if not self._bqml_model:
             raise RuntimeError("A model must be fitted before it can be saved")
 
         new_model = self._bqml_model.copy(model_name, replace)
```

### Comparing `bigframes-1.1.0/bigframes/ml/ensemble.py` & `bigframes-1.2.0/bigframes/ml/ensemble.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,17 +188,17 @@
     def to_gbq(self, model_name: str, replace: bool = False) -> XGBRegressor:
         """Save the model to BigQuery.
 
         Args:
             model_name (str):
                 The name of the model.
             replace (bool, default False):
-                Whether to replace if the model already exists. Default to False.
+                Determine whether to replace if the model already exists. Default to False.
 
-        Returns: saved model."""
+        Returns: Saved model."""
         if not self._bqml_model:
             raise RuntimeError("A model must be fitted before it can be saved")
 
         new_model = self._bqml_model.copy(model_name, replace)
         return new_model.session.read_gbq_model(model_name)
 
 
@@ -341,18 +341,18 @@
     def to_gbq(self, model_name: str, replace: bool = False) -> XGBClassifier:
         """Save the model to BigQuery.
 
         Args:
             model_name (str):
                 The name of the model.
             replace (bool, default False):
-                Whether to replace if the model already exists. Default to False.
+                Determine whether to replace if the model already exists. Default to False.
 
         Returns:
-            XGBClassifier: saved model."""
+            XGBClassifier: Saved model."""
         if not self._bqml_model:
             raise RuntimeError("A model must be fitted before it can be saved")
 
         new_model = self._bqml_model.copy(model_name, replace)
         return new_model.session.read_gbq_model(model_name)
 
 
@@ -504,18 +504,18 @@
     def to_gbq(self, model_name: str, replace: bool = False) -> RandomForestRegressor:
         """Save the model to BigQuery.
 
         Args:
             model_name (str):
                 The name of the model.
             replace (bool, default False):
-                Whether to replace if the model already exists. Default to False.
+                Determine whether to replace if the model already exists. Default to False.
 
         Returns:
-            RandomForestRegressor: saved model."""
+            RandomForestRegressor: Saved model."""
         if not self._bqml_model:
             raise RuntimeError("A model must be fitted before it can be saved")
 
         new_model = self._bqml_model.copy(model_name, replace)
         return new_model.session.read_gbq_model(model_name)
 
 
@@ -667,16 +667,16 @@
     def to_gbq(self, model_name: str, replace: bool = False) -> RandomForestClassifier:
         """Save the model to BigQuery.
 
         Args:
             model_name (str):
                 The name of the model.
             replace (bool, default False):
-                Whether to replace if the model already exists. Default to False.
+                Determine whether to replace if the model already exists. Default to False.
 
         Returns:
-            RandomForestClassifier: saved model."""
+            RandomForestClassifier: Saved model."""
         if not self._bqml_model:
             raise RuntimeError("A model must be fitted before it can be saved")
 
         new_model = self._bqml_model.copy(model_name, replace)
         return new_model.session.read_gbq_model(model_name)
```

### Comparing `bigframes-1.1.0/bigframes/ml/forecasting.py` & `bigframes-1.2.0/bigframes/ml/forecasting.py`

 * *Files 0% similar despite different names*

```diff
@@ -359,16 +359,16 @@
     def to_gbq(self, model_name: str, replace: bool = False) -> ARIMAPlus:
         """Save the model to BigQuery.
 
         Args:
             model_name (str):
                 the name of the model.
             replace (bool, default False):
-                whether to replace if the model already exists. Default to False.
+                Determine whether to replace if the model already exists. Default to False.
 
         Returns:
-            ARIMAPlus: saved model."""
+            ARIMAPlus: Saved model."""
         if not self._bqml_model:
             raise RuntimeError("A model must be fitted before it can be saved")
 
         new_model = self._bqml_model.copy(model_name, replace)
         return new_model.session.read_gbq_model(model_name)
```

### Comparing `bigframes-1.1.0/bigframes/ml/globals.py` & `bigframes-1.2.0/bigframes/ml/globals.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/bigframes/ml/imported.py` & `bigframes-1.2.0/bigframes/ml/imported.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 @log_adapter.class_logger
 class TensorFlowModel(base.Predictor):
     """Imported TensorFlow model.
 
     Args:
         model_path (str):
-            GCS path that holds the model files.
+            Cloud Storage path that holds the model files.
         session (BigQuery Session):
             BQ session to create the model.
     """
 
     def __init__(
         self,
         model_path: str,
@@ -65,18 +65,18 @@
         return tf_model
 
     def predict(self, X: Union[bpd.DataFrame, bpd.Series]) -> bpd.DataFrame:
         """Predict the result from input DataFrame.
 
         Args:
             X (bigframes.dataframe.DataFrame):
-                Input DataFrame, schema is defined by the model.
+                Input DataFrame. Schema is defined by the model.
 
         Returns:
-            bigframes.dataframe.DataFrame: Output DataFrame, schema is defined by the model."""
+            bigframes.dataframe.DataFrame: Output DataFrame. Schema is defined by the model."""
 
         if not self._bqml_model:
             if self.model_path is None:
                 raise ValueError("Model GCS path must be provided.")
             self._bqml_model = self._create_bqml_model()
         self._bqml_model = cast(core.BqmlModel, self._bqml_model)
 
@@ -87,18 +87,18 @@
     def to_gbq(self, model_name: str, replace: bool = False) -> TensorFlowModel:
         """Save the model to BigQuery.
 
         Args:
             model_name (str):
                 the name of the model.
             replace (bool, default False):
-                whether to replace if the model already exists. Default to False.
+                 Default to False.
 
         Returns:
-            TensorFlowModel: saved model."""
+            TensorFlowModel: Saved model."""
         if not self._bqml_model:
             if self.model_path is None:
                 raise ValueError("Model GCS path must be provided.")
             self._bqml_model = self._create_bqml_model()
         self._bqml_model = cast(core.BqmlModel, self._bqml_model)
 
         new_model = self._bqml_model.copy(model_name, replace)
@@ -142,15 +142,15 @@
         return onnx_model
 
     def predict(self, X: Union[bpd.DataFrame, bpd.Series]) -> bpd.DataFrame:
         """Predict the result from input DataFrame.
 
         Args:
             X (bigframes.dataframe.DataFrame or bigframes.series.Series):
-                Input DataFrame or Series, schema is defined by the model.
+                Input DataFrame or Series. Schema is defined by the model.
 
         Returns:
             bigframes.dataframe.DataFrame: Output DataFrame, schema is defined by the model."""
 
         if not self._bqml_model:
             if self.model_path is None:
                 raise ValueError("Model GCS path must be provided.")
@@ -164,18 +164,18 @@
     def to_gbq(self, model_name: str, replace: bool = False) -> ONNXModel:
         """Save the model to BigQuery.
 
         Args:
             model_name (str):
                 the name of the model.
             replace (bool, default False):
-                whether to replace if the model already exists. Default to False.
+                Determine whether to replace if the model already exists. Default to False.
 
         Returns:
-            ONNXModel: saved model."""
+            ONNXModel: Saved model."""
         if not self._bqml_model:
             if self.model_path is None:
                 raise ValueError("Model GCS path must be provided.")
             self._bqml_model = self._create_bqml_model()
         self._bqml_model = cast(core.BqmlModel, self._bqml_model)
 
         new_model = self._bqml_model.copy(model_name, replace)
@@ -258,18 +258,18 @@
         return xgboost_model
 
     def predict(self, X: Union[bpd.DataFrame, bpd.Series]) -> bpd.DataFrame:
         """Predict the result from input DataFrame.
 
         Args:
             X (bigframes.dataframe.DataFrame or bigframes.series.Series):
-                Input DataFrame or Series, schema is defined by the model.
+                Input DataFrame or Series. Schema is defined by the model.
 
         Returns:
-            bigframes.dataframe.DataFrame: Output DataFrame, schema is defined by the model."""
+            bigframes.dataframe.DataFrame: Output DataFrame. Schema is defined by the model."""
 
         if not self._bqml_model:
             if self.model_path is None:
                 raise ValueError("Model GCS path must be provided.")
             self._bqml_model = self._create_bqml_model()
         self._bqml_model = cast(core.BqmlModel, self._bqml_model)
 
@@ -280,18 +280,18 @@
     def to_gbq(self, model_name: str, replace: bool = False) -> XGBoostModel:
         """Save the model to BigQuery.
 
         Args:
             model_name (str):
                 the name of the model.
             replace (bool, default False):
-                whether to replace if the model already exists. Default to False.
+                Determine whether to replace if the model already exists. Default to False.
 
         Returns:
-            XGBoostModel: saved model."""
+            XGBoostModel: Saved model."""
         if not self._bqml_model:
             if self.model_path is None:
                 raise ValueError("Model GCS path must be provided.")
             self._bqml_model = self._create_bqml_model()
         self._bqml_model = cast(core.BqmlModel, self._bqml_model)
 
         new_model = self._bqml_model.copy(model_name, replace)
```

### Comparing `bigframes-1.1.0/bigframes/ml/linear_model.py` & `bigframes-1.2.0/bigframes/ml/linear_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,15 +180,15 @@
     def to_gbq(self, model_name: str, replace: bool = False) -> LinearRegression:
         """Save the model to BigQuery.
 
         Args:
             model_name (str):
                 the name of the model.
             replace (bool, default False):
-                whether to replace if the model already exists. Default to False.
+                Determine whether to replace if the model already exists. Default to False.
 
         Returns:
             LinearRegression: saved model."""
         if not self._bqml_model:
             raise RuntimeError("A model must be fitted before it can be saved")
 
         new_model = self._bqml_model.copy(model_name, replace)
@@ -345,15 +345,15 @@
     def to_gbq(self, model_name: str, replace: bool = False) -> LogisticRegression:
         """Save the model to BigQuery.
 
         Args:
             model_name (str):
                 the name of the model.
             replace (bool, default False):
-                whether to replace if the model already exists. Default to False.
+                Determine whether to replace if the model already exists. Default to False.
 
         Returns:
             LogisticRegression: saved model."""
         if not self._bqml_model:
             raise RuntimeError("A model must be fitted before it can be saved")
 
         # TODO(ashleyxu): support class_weight (struct array as dict in our API)
```

### Comparing `bigframes-1.1.0/bigframes/ml/llm.py` & `bigframes-1.2.0/bigframes/ml/llm.py`

 * *Files 0% similar despite different names*

```diff
@@ -244,15 +244,15 @@
     def to_gbq(self, model_name: str, replace: bool = False) -> PaLM2TextGenerator:
         """Save the model to BigQuery.
 
         Args:
             model_name (str):
                 the name of the model.
             replace (bool, default False):
-                whether to replace if the model already exists. Default to False.
+                Determine whether to replace if the model already exists. Default to False.
 
         Returns:
             PaLM2TextGenerator: saved model."""
 
         new_model = self._bqml_model.copy(model_name, replace)
         return new_model.session.read_gbq_model(model_name)
 
@@ -411,15 +411,15 @@
     ) -> PaLM2TextEmbeddingGenerator:
         """Save the model to BigQuery.
 
         Args:
             model_name (str):
                 the name of the model.
             replace (bool, default False):
-                whether to replace if the model already exists. Default to False.
+                Determine whether to replace if the model already exists. Default to False.
 
         Returns:
             PaLM2TextEmbeddingGenerator: saved model."""
 
         new_model = self._bqml_model.copy(model_name, replace)
         return new_model.session.read_gbq_model(model_name)
 
@@ -591,14 +591,14 @@
     def to_gbq(self, model_name: str, replace: bool = False) -> GeminiTextGenerator:
         """Save the model to BigQuery.
 
         Args:
             model_name (str):
                 the name of the model.
             replace (bool, default False):
-                whether to replace if the model already exists. Default to False.
+                Determine whether to replace if the model already exists. Default to False.
 
         Returns:
             GeminiTextGenerator: saved model."""
 
         new_model = self._bqml_model.copy(model_name, replace)
         return new_model.session.read_gbq_model(model_name)
```

### Comparing `bigframes-1.1.0/bigframes/ml/loader.py` & `bigframes-1.2.0/bigframes/ml/loader.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/bigframes/ml/metrics/__init__.py` & `bigframes-1.2.0/bigframes/ml/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/bigframes/ml/metrics/_metrics.py` & `bigframes-1.2.0/bigframes/ml/metrics/_metrics.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/bigframes/ml/metrics/pairwise.py` & `bigframes-1.2.0/bigframes/ml/metrics/pairwise.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/bigframes/ml/model_selection.py` & `bigframes-1.2.0/bigframes/ml/model_selection.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/bigframes/ml/pipeline.py` & `bigframes-1.2.0/bigframes/ml/pipeline.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/bigframes/ml/preprocessing.py` & `bigframes-1.2.0/bigframes/ml/preprocessing.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/bigframes/ml/remote.py` & `bigframes-1.2.0/bigframes/ml/remote.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/bigframes/ml/sql.py` & `bigframes-1.2.0/bigframes/ml/sql.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/bigframes/ml/utils.py` & `bigframes-1.2.0/bigframes/ml/utils.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/bigframes/operations/__init__.py` & `bigframes-1.2.0/bigframes/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/bigframes/operations/_matplotlib/__init__.py` & `bigframes-1.2.0/bigframes/operations/_matplotlib/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/bigframes/operations/_matplotlib/core.py` & `bigframes-1.2.0/bigframes/operations/_matplotlib/core.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/bigframes/operations/_matplotlib/hist.py` & `bigframes-1.2.0/bigframes/operations/_matplotlib/hist.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/bigframes/operations/base.py` & `bigframes-1.2.0/bigframes/operations/base.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/bigframes/operations/datetimes.py` & `bigframes-1.2.0/bigframes/operations/datetimes.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/bigframes/operations/plotting.py` & `bigframes-1.2.0/bigframes/operations/plotting.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/bigframes/operations/strings.py` & `bigframes-1.2.0/bigframes/operations/strings.py`

 * *Files 9% similar despite different names*

```diff
@@ -49,15 +49,33 @@
     def len(self) -> series.Series:
         return self._apply_unary_op(ops.len_op)
 
     def lower(self) -> series.Series:
         return self._apply_unary_op(ops.lower_op)
 
     def reverse(self) -> series.Series:
-        """Reverse strings in the Series."""
+        """Reverse strings in the Series.
+
+        **Examples:**
+
+            >>> import bigframes.pandas as bpd
+            >>> bpd.options.display.progress_bar = None
+
+            >>> s = bpd.Series(["apple", "banana", "", bpd.NA])
+            >>> s.str.reverse()
+            0     elppa
+            1    ananab
+            2
+            3      <NA>
+            dtype: string
+
+        Returns:
+            bigframes.series.Series: A Series of booleans indicating whether the given
+                pattern matches the start of each string element.
+        """
         # reverse method is in ibis, not pandas.
         return self._apply_unary_op(ops.reverse_op)
 
     def slice(
         self,
         start: Optional[int] = None,
         stop: Optional[int] = None,
```

### Comparing `bigframes-1.1.0/bigframes/operations/structs.py` & `bigframes-1.2.0/bigframes/operations/structs.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/bigframes/operations/type.py` & `bigframes-1.2.0/bigframes/operations/type.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/bigframes/pandas/__init__.py` & `bigframes-1.2.0/bigframes/pandas/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,14 +55,15 @@
 
 import bigframes._config as config
 import bigframes.constants as constants
 import bigframes.core.blocks
 import bigframes.core.expression as ex
 import bigframes.core.global_session as global_session
 import bigframes.core.indexes
+import bigframes.core.joins
 import bigframes.core.reshape
 import bigframes.core.tools
 import bigframes.dataframe
 import bigframes.operations as ops
 import bigframes.series
 import bigframes.session
 import bigframes.session.clients
@@ -703,14 +704,15 @@
 ArrowDtype = pandas.ArrowDtype
 
 # Class aliases
 # TODO(swast): Make these real classes so we can refer to these in type
 # checking and docstrings.
 DataFrame = bigframes.dataframe.DataFrame
 Index = bigframes.core.indexes.Index
+MultiIndex = bigframes.core.indexes.MultiIndex
 Series = bigframes.series.Series
 
 # Other public pandas attributes
 NamedAgg = namedtuple("NamedAgg", ["column", "aggfunc"])
 
 options = config.options
 """Global :class:`~bigframes._config.Options` to configure BigQuery DataFrames."""
@@ -756,14 +758,15 @@
     "Float64Dtype",
     "Int64Dtype",
     "StringDtype",
     "ArrowDtype"
     # Class aliases
     "DataFrame",
     "Index",
+    "MultiIndex",
     "Series",
     # Other public pandas attributes
     "NamedAgg",
     "options",
     "option_context",
     # Session management APIs
     "get_global_session",
```

### Comparing `bigframes-1.1.0/bigframes/series.py` & `bigframes-1.2.0/bigframes/series.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,20 +13,21 @@
 # limitations under the License.
 
 """Series is a 1 dimensional data structure."""
 
 from __future__ import annotations
 
 import functools
+import inspect
 import itertools
 import numbers
 import os
 import textwrap
 import typing
-from typing import Any, Literal, Mapping, Optional, Tuple, Union
+from typing import Any, Literal, Mapping, Optional, Sequence, Tuple, Union
 
 import bigframes_vendored.pandas.core.series as vendored_pandas_series
 import google.cloud.bigquery as bigquery
 import numpy
 import pandas
 import pandas.core.dtypes.common
 import typing_extensions
@@ -127,14 +128,19 @@
         return 1
 
     @property
     def empty(self) -> bool:
         return self.shape[0] == 0
 
     @property
+    def hasnans(self) -> bool:
+        # Note, hasnans is actually a null check, and NaNs don't count for nullable float
+        return self.isnull().any()
+
+    @property
     def values(self) -> numpy.ndarray:
         return self.to_numpy()
 
     @property
     def index(self) -> indexes.Index:
         return indexes.Index.from_frame(self)
 
@@ -171,14 +177,16 @@
 
     def _set_internal_query_job(self, query_job: bigquery.QueryJob):
         self._query_job = query_job
 
     def __len__(self):
         return self.shape[0]
 
+    __len__.__doc__ = inspect.getdoc(vendored_pandas_series.Series.__len__)
+
     def __iter__(self) -> typing.Iterator:
         self._optimize_query_complexity()
         return itertools.chain.from_iterable(
             map(lambda x: x.squeeze(axis=1), self._block.to_pandas_batches())
         )
 
     def copy(self) -> Series:
@@ -414,14 +422,15 @@
         )
 
     def ffill(self, *, limit: typing.Optional[int] = None) -> Series:
         window = bigframes.core.window_spec.WindowSpec(preceding=limit, following=0)
         return self._apply_window_op(agg_ops.LastNonNullOp(), window)
 
     pad = ffill
+    pad.__doc__ = inspect.getdoc(vendored_pandas_series.Series.ffill)
 
     def bfill(self, *, limit: typing.Optional[int] = None) -> Series:
         window = bigframes.core.window_spec.WindowSpec(preceding=0, following=limit)
         return self._apply_window_op(agg_ops.FirstNonNullOp(), window)
 
     def cummax(self) -> Series:
         return self._apply_window_op(
@@ -600,106 +609,138 @@
             ops.IsInOp(values=tuple(values), match_nulls=True)
         ).fillna(value=False)
 
     def isna(self) -> "Series":
         return self._apply_unary_op(ops.isnull_op)
 
     isnull = isna
+    isnull.__doc__ = inspect.getdoc(vendored_pandas_series.Series.isna)
 
     def notna(self) -> "Series":
         return self._apply_unary_op(ops.notnull_op)
 
     notnull = notna
+    notnull.__doc__ = inspect.getdoc(vendored_pandas_series.Series.notna)
 
     def __and__(self, other: bool | int | Series) -> Series:
         return self._apply_binary_op(other, ops.and_op)
 
+    __and__.__doc__ = inspect.getdoc(vendored_pandas_series.Series.__and__)
+
     __rand__ = __and__
 
     def __or__(self, other: bool | int | Series) -> Series:
         return self._apply_binary_op(other, ops.or_op)
 
+    __or__.__doc__ = inspect.getdoc(vendored_pandas_series.Series.__or__)
+
     __ror__ = __or__
 
     def __add__(self, other: float | int | Series) -> Series:
         return self.add(other)
 
+    __add__.__doc__ = inspect.getdoc(vendored_pandas_series.Series.__add__)
+
     def __radd__(self, other: float | int | Series) -> Series:
         return self.radd(other)
 
+    __radd__.__doc__ = inspect.getdoc(vendored_pandas_series.Series.__radd__)
+
     def add(self, other: float | int | Series) -> Series:
         return self._apply_binary_op(other, ops.add_op)
 
     def radd(self, other: float | int | Series) -> Series:
         return self._apply_binary_op(other, ops.add_op, reverse=True)
 
     def __sub__(self, other: float | int | Series) -> Series:
         return self.sub(other)
 
+    __sub__.__doc__ = inspect.getdoc(vendored_pandas_series.Series.__sub__)
+
     def __rsub__(self, other: float | int | Series) -> Series:
         return self.rsub(other)
 
+    __rsub__.__doc__ = inspect.getdoc(vendored_pandas_series.Series.__rsub__)
+
     def sub(self, other: float | int | Series) -> Series:
         return self._apply_binary_op(other, ops.sub_op)
 
     def rsub(self, other: float | int | Series) -> Series:
         return self._apply_binary_op(other, ops.sub_op, reverse=True)
 
     subtract = sub
+    subtract.__doc__ = inspect.getdoc(vendored_pandas_series.Series.sub)
 
     def __mul__(self, other: float | int | Series) -> Series:
         return self.mul(other)
 
+    __mul__.__doc__ = inspect.getdoc(vendored_pandas_series.Series.__mul__)
+
     def __rmul__(self, other: float | int | Series) -> Series:
         return self.rmul(other)
 
+    __rmul__.__doc__ = inspect.getdoc(vendored_pandas_series.Series.__rmul__)
+
     def mul(self, other: float | int | Series) -> Series:
         return self._apply_binary_op(other, ops.mul_op)
 
     def rmul(self, other: float | int | Series) -> Series:
         return self._apply_binary_op(other, ops.mul_op, reverse=True)
 
     multiply = mul
+    multiply.__doc__ = inspect.getdoc(vendored_pandas_series.Series.mul)
 
     def __truediv__(self, other: float | int | Series) -> Series:
         return self.truediv(other)
 
+    __truediv__.__doc__ = inspect.getdoc(vendored_pandas_series.Series.__truediv__)
+
     def __rtruediv__(self, other: float | int | Series) -> Series:
         return self.rtruediv(other)
 
+    __rtruediv__.__doc__ = inspect.getdoc(vendored_pandas_series.Series.__rtruediv__)
+
     def truediv(self, other: float | int | Series) -> Series:
         return self._apply_binary_op(other, ops.div_op)
 
     def rtruediv(self, other: float | int | Series) -> Series:
         return self._apply_binary_op(other, ops.div_op, reverse=True)
 
-    div = truediv
-
-    divide = truediv
+    truediv.__doc__ = inspect.getdoc(vendored_pandas_series.Series.truediv)
+    div = divide = truediv
 
     rdiv = rtruediv
+    rdiv.__doc__ = inspect.getdoc(vendored_pandas_series.Series.rtruediv)
 
     def __floordiv__(self, other: float | int | Series) -> Series:
         return self.floordiv(other)
 
+    __floordiv__.__doc__ = inspect.getdoc(vendored_pandas_series.Series.__floordiv__)
+
     def __rfloordiv__(self, other: float | int | Series) -> Series:
         return self.rfloordiv(other)
 
+    __rfloordiv__.__doc__ = inspect.getdoc(vendored_pandas_series.Series.__rfloordiv__)
+
     def floordiv(self, other: float | int | Series) -> Series:
         return self._apply_binary_op(other, ops.floordiv_op)
 
     def rfloordiv(self, other: float | int | Series) -> Series:
         return self._apply_binary_op(other, ops.floordiv_op, reverse=True)
 
     def __pow__(self, other: float | int | Series) -> Series:
         return self.pow(other)
 
+    __pow__.__doc__ = inspect.getdoc(vendored_pandas_series.Series.__pow__)
+
     def __rpow__(self, other: float | int | Series) -> Series:
         return self.rpow(other)
 
+    __rpow__.__doc__ = inspect.getdoc(vendored_pandas_series.Series.__rpow__)
+
     def pow(self, other: float | int | Series) -> Series:
         return self._apply_binary_op(other, ops.pow_op)
 
     def rpow(self, other: float | int | Series) -> Series:
         return self._apply_binary_op(other, ops.pow_op, reverse=True)
 
     def __lt__(self, other: float | int | Series) -> Series:  # type: ignore
@@ -725,17 +766,21 @@
 
     def ge(self, other) -> Series:
         return self._apply_binary_op(other, ops.ge_op)
 
     def __mod__(self, other) -> Series:  # type: ignore
         return self.mod(other)
 
+    __mod__.__doc__ = inspect.getdoc(vendored_pandas_series.Series.__mod__)
+
     def __rmod__(self, other) -> Series:  # type: ignore
         return self.rmod(other)
 
+    __rmod__.__doc__ = inspect.getdoc(vendored_pandas_series.Series.__rmod__)
+
     def mod(self, other) -> Series:  # type: ignore
         return self._apply_binary_op(other, ops.mod_op)
 
     def rmod(self, other) -> Series:  # type: ignore
         return self._apply_binary_op(other, ops.mod_op, reverse=True)
 
     def divmod(self, other) -> Tuple[Series, Series]:  # type: ignore
@@ -744,18 +789,40 @@
         return (self.floordiv(other), self.mod(other))
 
     def rdivmod(self, other) -> Tuple[Series, Series]:  # type: ignore
         # TODO(huanc): when self and other both has dtype int and self contains zeros,
         # the output should be dtype float, both floordiv and mod returns dtype int in this case.
         return (self.rfloordiv(other), self.rmod(other))
 
-    def __matmul__(self, other):
+    def dot(self, other):
         return (self * other).sum()
 
-    dot = __matmul__
+    def __matmul__(self, other):
+        return self.dot(other)
+
+    __matmul__.__doc__ = inspect.getdoc(vendored_pandas_series.Series.__matmul__)
+
+    def __rmatmul__(self, other):
+        return self.dot(other)
+
+    __rmatmul__.__doc__ = inspect.getdoc(vendored_pandas_series.Series.__rmatmul__)
+
+    def combine_first(self, other: Series) -> Series:
+        result = self._apply_binary_op(other, ops.coalesce_op)
+        result.name = self.name
+        return result
+
+    def update(self, other: Union[Series, Sequence, Mapping]) -> None:
+        import bigframes.core.convert
+
+        other = bigframes.core.convert.to_bf_series(other, default_index=None)
+        result = self._apply_binary_op(
+            other, ops.coalesce_op, reverse=True, alignment="left"
+        )
+        self._set_block(result._get_block())
 
     def abs(self) -> Series:
         return self._apply_unary_op(ops.abs_op)
 
     def round(self, decimals=0) -> "Series":
         return self._apply_binary_op(decimals, ops.round_op)
 
@@ -768,14 +835,17 @@
             )
         if min_periods:
             raise NotImplementedError(
                 f"min_periods not yet supported. {constants.FEEDBACK_LINK}"
             )
         return self._apply_binary_aggregation(other, agg_ops.CorrOp())
 
+    def autocorr(self, lag: int = 1) -> float:
+        return self.corr(self.shift(lag))
+
     def cov(self, other: Series) -> float:
         return self._apply_binary_aggregation(other, agg_ops.CovOp())
 
     def all(self) -> bool:
         return typing.cast(bool, self._apply_aggregation(agg_ops.all_op))
 
     def any(self) -> bool:
@@ -823,14 +893,15 @@
         else:
 
             return self._apply_aggregation(
                 agg_ops.lookup_agg_func(typing.cast(str, func))
             )
 
     aggregate = agg
+    aggregate.__doc__ = inspect.getdoc(vendored_pandas_series.Series.agg)
 
     def skew(self):
         count = self.count()
         if count < 3:
             return pandas.NA
 
         moment3 = self._central_moment(3)
@@ -857,14 +928,15 @@
         numerator = (count + 1) * (count - 1) * moment4
         denominator = (count - 2) * (count - 3) * moment2**2
         adjustment = 3 * (count - 1) ** 2 / ((count - 2) * (count - 3))
 
         return (numerator / denominator) - adjustment
 
     kurtosis = kurt
+    kurtosis.__doc__ = inspect.getdoc(vendored_pandas_series.Series.kurt)
 
     def mode(self) -> Series:
         block = self._block
         # Approach: Count each value, return each value for which count(x) == max(counts))
         block, agg_ids = block.aggregate(
             by_column_ids=[self._value_column],
             aggregations=((self._value_column, agg_ops.count_op),),
@@ -904,24 +976,27 @@
     def sum(self) -> float:
         return typing.cast(float, self._apply_aggregation(agg_ops.sum_op))
 
     def prod(self) -> float:
         return typing.cast(float, self._apply_aggregation(agg_ops.product_op))
 
     product = prod
+    product.__doc__ = inspect.getdoc(vendored_pandas_series.Series.prod)
 
     def __eq__(self, other: object) -> Series:  # type: ignore
         return self.eq(other)
 
     def __ne__(self, other: object) -> Series:  # type: ignore
         return self.ne(other)
 
     def __invert__(self) -> Series:
         return self._apply_unary_op(ops.invert_op)
 
+    __invert__.__doc__ = inspect.getdoc(vendored_pandas_series.Series.__invert__)
+
     def eq(self, other: object) -> Series:
         # TODO: enforce stricter alignment
         return self._apply_binary_op(other, ops.eq_op)
 
     def ne(self, other: object) -> Series:
         # TODO: enforce stricter alignment
         return self._apply_binary_op(other, ops.ne_op)
@@ -1048,14 +1123,16 @@
         if isinstance(indexer, Series):
             (left, right, block) = self._align(indexer, "left")
             block = block.filter_by_id(right)
             block = block.select_column(left)
             return Series(block)
         return self.loc[indexer]
 
+    __getitem__.__doc__ = inspect.getdoc(vendored_pandas_series.Series.__getitem__)
+
     def __getattr__(self, key: str):
         if hasattr(pandas.Series, key):
             raise AttributeError(
                 textwrap.dedent(
                     f"""
                     BigQuery DataFrames has not yet implemented an equivalent to
                     'pandas.Series.{key}'. {constants.FEEDBACK_LINK}
@@ -1435,14 +1512,15 @@
             buf, columns=columns, header=header, index=index, **kwargs
         )
 
     def tolist(self) -> list:
         return self.to_pandas().to_list()
 
     to_list = tolist
+    to_list.__doc__ = inspect.getdoc(vendored_pandas_series.Series.tolist)
 
     def to_markdown(
         self,
         buf: typing.IO[str] | None = None,
         mode: str = "wt",
         index: bool = True,
         **kwargs,
@@ -1450,15 +1528,18 @@
         return self.to_pandas().to_markdown(buf, mode=mode, index=index, **kwargs)  # type: ignore
 
     def to_numpy(
         self, dtype=None, copy=False, na_value=None, **kwargs
     ) -> numpy.ndarray:
         return self.to_pandas().to_numpy(dtype, copy, na_value, **kwargs)
 
-    __array__ = to_numpy
+    def __array__(self, dtype=None) -> numpy.ndarray:
+        return self.to_numpy(dtype=dtype)
+
+    __array__.__doc__ = inspect.getdoc(vendored_pandas_series.Series.__array__)
 
     def to_pickle(self, path, **kwargs) -> None:
         return self.to_pandas().to_pickle(path, **kwargs)
 
     def to_string(
         self,
         buf=None,
```

### Comparing `bigframes-1.1.0/bigframes/session/__init__.py` & `bigframes-1.2.0/bigframes/session/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2451,2610 +2451,2631 @@
 00009920: 696e 655f 6466 203d 2073 656c 662e 5f72  ine_df = self._r
 00009930: 6561 645f 7061 6e64 6173 5f69 6e6c 696e  ead_pandas_inlin
 00009940: 6528 7061 6e64 6173 5f64 6174 6166 7261  e(pandas_datafra
 00009950: 6d65 290a 2020 2020 2020 2020 6966 2069  me).        if i
 00009960: 6e6c 696e 655f 6466 2069 7320 6e6f 7420  nline_df is not 
 00009970: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
 00009980: 2020 7265 7475 726e 2069 6e6c 696e 655f    return inline_
-00009990: 6466 0a20 2020 2020 2020 2072 6574 7572  df.        retur
-000099a0: 6e20 7365 6c66 2e5f 7265 6164 5f70 616e  n self._read_pan
-000099b0: 6461 735f 6c6f 6164 5f6a 6f62 2870 616e  das_load_job(pan
-000099c0: 6461 735f 6461 7461 6672 616d 652c 2061  das_dataframe, a
-000099d0: 7069 5f6e 616d 6529 0a0a 2020 2020 6465  pi_name)..    de
-000099e0: 6620 5f72 6561 645f 7061 6e64 6173 5f69  f _read_pandas_i
-000099f0: 6e6c 696e 6528 0a20 2020 2020 2020 2073  nline(.        s
-00009a00: 656c 662c 2070 616e 6461 735f 6461 7461  elf, pandas_data
-00009a10: 6672 616d 653a 2070 616e 6461 732e 4461  frame: pandas.Da
-00009a20: 7461 4672 616d 650a 2020 2020 2920 2d3e  taFrame.    ) ->
-00009a30: 204f 7074 696f 6e61 6c5b 6461 7461 6672   Optional[datafr
-00009a40: 616d 652e 4461 7461 4672 616d 655d 3a0a  ame.DataFrame]:.
-00009a50: 2020 2020 2020 2020 696d 706f 7274 2062          import b
-00009a60: 6967 6672 616d 6573 2e64 6174 6166 7261  igframes.datafra
-00009a70: 6d65 2061 7320 6461 7461 6672 616d 650a  me as dataframe.
-00009a80: 0a20 2020 2020 2020 2069 6620 7061 6e64  .        if pand
-00009a90: 6173 5f64 6174 6166 7261 6d65 2e6d 656d  as_dataframe.mem
-00009aa0: 6f72 795f 7573 6167 6528 6465 6570 3d54  ory_usage(deep=T
-00009ab0: 7275 6529 2e73 756d 2829 203e 204d 4158  rue).sum() > MAX
-00009ac0: 5f49 4e4c 494e 455f 4446 5f42 5954 4553  _INLINE_DF_BYTES
-00009ad0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00009ae0: 7475 726e 204e 6f6e 650a 0a20 2020 2020  turn None..     
-00009af0: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
-00009b00: 2020 2020 696e 6c69 6e65 5f64 6620 3d20      inline_df = 
-00009b10: 6461 7461 6672 616d 652e 4461 7461 4672  dataframe.DataFr
-00009b20: 616d 6528 0a20 2020 2020 2020 2020 2020  ame(.           
-00009b30: 2020 2020 2062 6c6f 636b 732e 426c 6f63       blocks.Bloc
-00009b40: 6b2e 6672 6f6d 5f6c 6f63 616c 2870 616e  k.from_local(pan
-00009b50: 6461 735f 6461 7461 6672 616d 652c 2073  das_dataframe, s
-00009b60: 656c 6629 0a20 2020 2020 2020 2020 2020  elf).           
-00009b70: 2029 0a20 2020 2020 2020 2065 7863 6570   ).        excep
-00009b80: 7420 5661 6c75 6545 7272 6f72 3a20 2023  t ValueError:  #
-00009b90: 2054 6872 6f77 6e20 6279 2069 6269 7320   Thrown by ibis 
-00009ba0: 666f 7220 736f 6d65 2075 6e68 616e 646c  for some unhandl
-00009bb0: 6564 2074 7970 6573 0a20 2020 2020 2020  ed types.       
-00009bc0: 2020 2020 2072 6574 7572 6e20 4e6f 6e65       return None
-00009bd0: 0a20 2020 2020 2020 2065 7863 6570 7420  .        except 
-00009be0: 7061 2e41 7272 6f77 5479 7065 4572 726f  pa.ArrowTypeErro
-00009bf0: 723a 2020 2320 5468 726f 776e 2062 7920  r:  # Thrown by 
-00009c00: 6172 726f 7720 666f 7220 7479 7065 7320  arrow for types 
-00009c10: 7769 7468 6f75 7420 6d61 7070 696e 6720  without mapping 
-00009c20: 2867 656f 292e 0a20 2020 2020 2020 2020  (geo)..         
-00009c30: 2020 2072 6574 7572 6e20 4e6f 6e65 0a0a     return None..
-00009c40: 2020 2020 2020 2020 696e 6c69 6e65 5f74          inline_t
-00009c50: 7970 6573 203d 2069 6e6c 696e 655f 6466  ypes = inline_df
-00009c60: 2e5f 626c 6f63 6b2e 6578 7072 2e73 6368  ._block.expr.sch
-00009c70: 656d 612e 6474 7970 6573 0a20 2020 2020  ema.dtypes.     
-00009c80: 2020 2023 2049 6269 7320 6861 7320 7072     # Ibis has pr
-00009c90: 6f62 6c65 6d73 2065 7363 6170 696e 6720  oblems escaping 
-00009ca0: 6279 7465 7320 6c69 7465 7261 6c73 2c20  bytes literals, 
-00009cb0: 7768 6963 6820 7769 6c6c 2063 6175 7365  which will cause
-00009cc0: 2073 796e 7461 7820 6572 726f 7273 2073   syntax errors s
-00009cd0: 6572 7665 722d 7369 6465 2e0a 2020 2020  erver-side..    
-00009ce0: 2020 2020 6966 2061 6c6c 2864 7479 7065      if all(dtype
-00009cf0: 2069 6e20 494e 4c49 4e41 424c 455f 4454   in INLINABLE_DT
-00009d00: 5950 4553 2066 6f72 2064 7479 7065 2069  YPES for dtype i
-00009d10: 6e20 696e 6c69 6e65 5f74 7970 6573 293a  n inline_types):
-00009d20: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00009d30: 7572 6e20 696e 6c69 6e65 5f64 660a 2020  urn inline_df.  
-00009d40: 2020 2020 2020 7265 7475 726e 204e 6f6e        return Non
-00009d50: 650a 0a20 2020 2064 6566 205f 7265 6164  e..    def _read
-00009d60: 5f70 616e 6461 735f 6c6f 6164 5f6a 6f62  _pandas_load_job
-00009d70: 280a 2020 2020 2020 2020 7365 6c66 2c20  (.        self, 
-00009d80: 7061 6e64 6173 5f64 6174 6166 7261 6d65  pandas_dataframe
-00009d90: 3a20 7061 6e64 6173 2e44 6174 6146 7261  : pandas.DataFra
-00009da0: 6d65 2c20 6170 695f 6e61 6d65 3a20 7374  me, api_name: st
-00009db0: 720a 2020 2020 2920 2d3e 2064 6174 6166  r.    ) -> dataf
-00009dc0: 7261 6d65 2e44 6174 6146 7261 6d65 3a0a  rame.DataFrame:.
-00009dd0: 2020 2020 2020 2020 696d 706f 7274 2062          import b
-00009de0: 6967 6672 616d 6573 2e64 6174 6166 7261  igframes.datafra
-00009df0: 6d65 2061 7320 6461 7461 6672 616d 650a  me as dataframe.
-00009e00: 0a20 2020 2020 2020 2063 6f6c 5f69 6e64  .        col_ind
-00009e10: 6578 203d 2070 616e 6461 735f 6461 7461  ex = pandas_data
-00009e20: 6672 616d 652e 636f 6c75 6d6e 732e 636f  frame.columns.co
-00009e30: 7079 2829 0a20 2020 2020 2020 2063 6f6c  py().        col
-00009e40: 5f6c 6162 656c 732c 2069 6478 5f6c 6162  _labels, idx_lab
-00009e50: 656c 7320 3d20 280a 2020 2020 2020 2020  els = (.        
-00009e60: 2020 2020 636f 6c5f 696e 6465 782e 746f      col_index.to
-00009e70: 5f6c 6973 7428 292c 0a20 2020 2020 2020  _list(),.       
-00009e80: 2020 2020 2070 616e 6461 735f 6461 7461       pandas_data
-00009e90: 6672 616d 652e 696e 6465 782e 6e61 6d65  frame.index.name
-00009ea0: 732c 0a20 2020 2020 2020 2029 0a20 2020  s,.        ).   
-00009eb0: 2020 2020 206e 6577 5f63 6f6c 5f69 6473       new_col_ids
-00009ec0: 2c20 6e65 775f 6964 785f 6964 7320 3d20  , new_idx_ids = 
-00009ed0: 7574 696c 732e 6765 745f 7374 616e 6461  utils.get_standa
-00009ee0: 7264 697a 6564 5f69 6473 280a 2020 2020  rdized_ids(.    
-00009ef0: 2020 2020 2020 2020 636f 6c5f 6c61 6265          col_labe
-00009f00: 6c73 2c0a 2020 2020 2020 2020 2020 2020  ls,.            
-00009f10: 6964 785f 6c61 6265 6c73 2c0a 2020 2020  idx_labels,.    
-00009f20: 2020 2020 2020 2020 2320 4c6f 6164 696e          # Loadin
-00009f30: 6720 7061 7271 7565 7420 6669 6c65 7320  g parquet files 
-00009f40: 696e 746f 2042 6967 5175 6572 7920 7769  into BigQuery wi
-00009f50: 7468 2073 7065 6369 616c 2063 6f6c 756d  th special colum
-00009f60: 6e20 6e61 6d65 730a 2020 2020 2020 2020  n names.        
-00009f70: 2020 2020 2320 6973 206f 6e6c 7920 7375      # is only su
-00009f80: 7070 6f72 7465 6420 756e 6465 7220 616e  pported under an
-00009f90: 2061 6c6c 6f77 6c69 7374 2e0a 2020 2020   allowlist..    
-00009fa0: 2020 2020 2020 2020 7374 7269 6374 3d54          strict=T
-00009fb0: 7275 652c 0a20 2020 2020 2020 2029 0a0a  rue,.        )..
-00009fc0: 2020 2020 2020 2020 2320 4164 6420 6f72          # Add or
-00009fd0: 6465 7220 636f 6c75 6d6e 2074 6f20 7061  der column to pa
-00009fe0: 6e64 6173 2044 6174 6146 7261 6d65 2074  ndas DataFrame t
-00009ff0: 6f20 7072 6573 6572 7665 206f 7264 6572  o preserve order
-0000a000: 2069 6e20 4269 6751 7565 7279 0a20 2020   in BigQuery.   
-0000a010: 2020 2020 206f 7264 6572 696e 675f 636f       ordering_co
-0000a020: 6c20 3d20 2272 6f77 6964 220a 2020 2020  l = "rowid".    
-0000a030: 2020 2020 636f 6c75 6d6e 7320 3d20 6672      columns = fr
-0000a040: 6f7a 656e 7365 7428 636f 6c5f 6c61 6265  ozenset(col_labe
-0000a050: 6c73 202b 2069 6478 5f6c 6162 656c 7329  ls + idx_labels)
-0000a060: 0a20 2020 2020 2020 2073 7566 6669 7820  .        suffix 
-0000a070: 3d20 320a 2020 2020 2020 2020 7768 696c  = 2.        whil
-0000a080: 6520 6f72 6465 7269 6e67 5f63 6f6c 2069  e ordering_col i
-0000a090: 6e20 636f 6c75 6d6e 733a 0a20 2020 2020  n columns:.     
-0000a0a0: 2020 2020 2020 206f 7264 6572 696e 675f         ordering_
-0000a0b0: 636f 6c20 3d20 6622 726f 7769 645f 7b73  col = f"rowid_{s
-0000a0c0: 7566 6669 787d 220a 2020 2020 2020 2020  uffix}".        
-0000a0d0: 2020 2020 7375 6666 6978 202b 3d20 310a      suffix += 1.
-0000a0e0: 0a20 2020 2020 2020 2070 616e 6461 735f  .        pandas_
-0000a0f0: 6461 7461 6672 616d 655f 636f 7079 203d  dataframe_copy =
-0000a100: 2070 616e 6461 735f 6461 7461 6672 616d   pandas_datafram
-0000a110: 652e 636f 7079 2829 0a20 2020 2020 2020  e.copy().       
-0000a120: 2070 616e 6461 735f 6461 7461 6672 616d   pandas_datafram
-0000a130: 655f 636f 7079 2e69 6e64 6578 2e6e 616d  e_copy.index.nam
-0000a140: 6573 203d 206e 6577 5f69 6478 5f69 6473  es = new_idx_ids
-0000a150: 0a20 2020 2020 2020 2070 616e 6461 735f  .        pandas_
-0000a160: 6461 7461 6672 616d 655f 636f 7079 2e63  dataframe_copy.c
-0000a170: 6f6c 756d 6e73 203d 2070 616e 6461 732e  olumns = pandas.
-0000a180: 496e 6465 7828 6e65 775f 636f 6c5f 6964  Index(new_col_id
-0000a190: 7329 0a20 2020 2020 2020 2070 616e 6461  s).        panda
-0000a1a0: 735f 6461 7461 6672 616d 655f 636f 7079  s_dataframe_copy
-0000a1b0: 5b6f 7264 6572 696e 675f 636f 6c5d 203d  [ordering_col] =
-0000a1c0: 206e 702e 6172 616e 6765 2870 616e 6461   np.arange(panda
-0000a1d0: 735f 6461 7461 6672 616d 655f 636f 7079  s_dataframe_copy
-0000a1e0: 2e73 6861 7065 5b30 5d29 0a0a 2020 2020  .shape[0])..    
-0000a1f0: 2020 2020 6a6f 625f 636f 6e66 6967 203d      job_config =
-0000a200: 2073 656c 662e 5f70 7265 7061 7265 5f6c   self._prepare_l
-0000a210: 6f61 645f 6a6f 625f 636f 6e66 6967 2829  oad_job_config()
-0000a220: 0a0a 2020 2020 2020 2020 2320 5370 6563  ..        # Spec
-0000a230: 6966 7920 7468 6520 6461 7465 7469 6d65  ify the datetime
-0000a240: 2064 7479 7065 732c 2077 6869 6368 2069   dtypes, which i
-0000a250: 7320 6175 746f 2d64 6574 6563 7465 6420  s auto-detected 
-0000a260: 6173 2074 696d 6573 7461 6d70 2074 7970  as timestamp typ
-0000a270: 6573 2e0a 2020 2020 2020 2020 7363 6865  es..        sche
-0000a280: 6d61 3a20 6c69 7374 5b62 6967 7175 6572  ma: list[bigquer
-0000a290: 792e 5363 6865 6d61 4669 656c 645d 203d  y.SchemaField] =
-0000a2a0: 205b 5d0a 2020 2020 2020 2020 666f 7220   [].        for 
-0000a2b0: 636f 6c75 6d6e 2c20 6474 7970 6520 696e  column, dtype in
-0000a2c0: 207a 6970 286e 6577 5f63 6f6c 5f69 6473   zip(new_col_ids
-0000a2d0: 2c20 7061 6e64 6173 5f64 6174 6166 7261  , pandas_datafra
-0000a2e0: 6d65 2e64 7479 7065 7329 3a0a 2020 2020  me.dtypes):.    
-0000a2f0: 2020 2020 2020 2020 6966 2064 7479 7065          if dtype
-0000a300: 203d 3d20 2274 696d 6573 7461 6d70 5b75   == "timestamp[u
-0000a310: 735d 5b70 7961 7272 6f77 5d22 3a0a 2020  s][pyarrow]":.  
-0000a320: 2020 2020 2020 2020 2020 2020 2020 7363                sc
-0000a330: 6865 6d61 2e61 7070 656e 6428 0a20 2020  hema.append(.   
-0000a340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a350: 2062 6967 7175 6572 792e 5363 6865 6d61   bigquery.Schema
-0000a360: 4669 656c 6428 636f 6c75 6d6e 2c20 6269  Field(column, bi
-0000a370: 6771 7565 7279 2e65 6e75 6d73 2e53 716c  gquery.enums.Sql
-0000a380: 5479 7065 4e61 6d65 732e 4441 5445 5449  TypeNames.DATETI
-0000a390: 4d45 290a 2020 2020 2020 2020 2020 2020  ME).            
-0000a3a0: 2020 2020 290a 2020 2020 2020 2020 6a6f      ).        jo
-0000a3b0: 625f 636f 6e66 6967 2e73 6368 656d 6120  b_config.schema 
-0000a3c0: 3d20 7363 6865 6d61 0a0a 2020 2020 2020  = schema..      
-0000a3d0: 2020 2320 436c 7573 7465 7269 6e67 2070    # Clustering p
-0000a3e0: 726f 6261 626c 7920 6e6f 7420 6e65 6564  robably not need
-0000a3f0: 6564 2061 6e79 7761 7973 2061 7320 7061  ed anyways as pa
-0000a400: 6e64 6173 2074 6162 6c65 7320 6172 6520  ndas tables are 
-0000a410: 736d 616c 6c0a 2020 2020 2020 2020 636c  small.        cl
-0000a420: 7573 7465 725f 636f 6c73 203d 205b 6f72  uster_cols = [or
-0000a430: 6465 7269 6e67 5f63 6f6c 5d0a 2020 2020  dering_col].    
-0000a440: 2020 2020 6a6f 625f 636f 6e66 6967 2e63      job_config.c
-0000a450: 6c75 7374 6572 696e 675f 6669 656c 6473  lustering_fields
-0000a460: 203d 2063 6c75 7374 6572 5f63 6f6c 730a   = cluster_cols.
-0000a470: 0a20 2020 2020 2020 206a 6f62 5f63 6f6e  .        job_con
-0000a480: 6669 672e 6c61 6265 6c73 203d 207b 2262  fig.labels = {"b
-0000a490: 6967 6672 616d 6573 2d61 7069 223a 2061  igframes-api": a
-0000a4a0: 7069 5f6e 616d 657d 0a0a 2020 2020 2020  pi_name}..      
-0000a4b0: 2020 6c6f 6164 5f74 6162 6c65 5f64 6573    load_table_des
-0000a4c0: 7469 6e61 7469 6f6e 203d 2062 6967 6672  tination = bigfr
-0000a4d0: 616d 6573 5f69 6f2e 7261 6e64 6f6d 5f74  ames_io.random_t
-0000a4e0: 6162 6c65 2873 656c 662e 5f61 6e6f 6e79  able(self._anony
-0000a4f0: 6d6f 7573 5f64 6174 6173 6574 290a 2020  mous_dataset).  
-0000a500: 2020 2020 2020 6c6f 6164 5f6a 6f62 203d        load_job =
-0000a510: 2073 656c 662e 6271 636c 6965 6e74 2e6c   self.bqclient.l
-0000a520: 6f61 645f 7461 626c 655f 6672 6f6d 5f64  oad_table_from_d
-0000a530: 6174 6166 7261 6d65 280a 2020 2020 2020  ataframe(.      
-0000a540: 2020 2020 2020 7061 6e64 6173 5f64 6174        pandas_dat
-0000a550: 6166 7261 6d65 5f63 6f70 792c 0a20 2020  aframe_copy,.   
-0000a560: 2020 2020 2020 2020 206c 6f61 645f 7461           load_ta
-0000a570: 626c 655f 6465 7374 696e 6174 696f 6e2c  ble_destination,
-0000a580: 0a20 2020 2020 2020 2020 2020 206a 6f62  .            job
-0000a590: 5f63 6f6e 6669 673d 6a6f 625f 636f 6e66  _config=job_conf
-0000a5a0: 6967 2c0a 2020 2020 2020 2020 290a 2020  ig,.        ).  
-0000a5b0: 2020 2020 2020 7365 6c66 2e5f 7374 6172        self._star
-0000a5c0: 745f 6765 6e65 7269 635f 6a6f 6228 6c6f  t_generic_job(lo
-0000a5d0: 6164 5f6a 6f62 290a 0a20 2020 2020 2020  ad_job)..       
-0000a5e0: 206f 7264 6572 696e 6720 3d20 6f72 6465   ordering = orde
-0000a5f0: 722e 4578 7072 6573 7369 6f6e 4f72 6465  r.ExpressionOrde
-0000a600: 7269 6e67 280a 2020 2020 2020 2020 2020  ring(.          
-0000a610: 2020 6f72 6465 7269 6e67 5f76 616c 7565    ordering_value
-0000a620: 5f63 6f6c 756d 6e73 3d74 7570 6c65 285b  _columns=tuple([
-0000a630: 6f72 6465 722e 6173 6365 6e64 696e 675f  order.ascending_
-0000a640: 6f76 6572 286f 7264 6572 696e 675f 636f  over(ordering_co
-0000a650: 6c29 5d29 2c0a 2020 2020 2020 2020 2020  l)]),.          
-0000a660: 2020 746f 7461 6c5f 6f72 6465 7269 6e67    total_ordering
-0000a670: 5f63 6f6c 756d 6e73 3d66 726f 7a65 6e73  _columns=frozens
-0000a680: 6574 285b 6f72 6465 7269 6e67 5f63 6f6c  et([ordering_col
-0000a690: 5d29 2c0a 2020 2020 2020 2020 2020 2020  ]),.            
-0000a6a0: 696e 7465 6765 725f 656e 636f 6469 6e67  integer_encoding
-0000a6b0: 3d49 6e74 6567 6572 456e 636f 6469 6e67  =IntegerEncoding
-0000a6c0: 2854 7275 652c 2069 735f 7365 7175 656e  (True, is_sequen
-0000a6d0: 7469 616c 3d54 7275 6529 2c0a 2020 2020  tial=True),.    
-0000a6e0: 2020 2020 290a 2020 2020 2020 2020 7461      ).        ta
-0000a6f0: 626c 655f 6578 7072 6573 7369 6f6e 203d  ble_expression =
-0000a700: 2073 656c 662e 6962 6973 5f63 6c69 656e   self.ibis_clien
-0000a710: 742e 7461 626c 6528 2020 2320 7479 7065  t.table(  # type
-0000a720: 3a20 6967 6e6f 7265 0a20 2020 2020 2020  : ignore.       
-0000a730: 2020 2020 206c 6f61 645f 7461 626c 655f       load_table_
-0000a740: 6465 7374 696e 6174 696f 6e2e 7461 626c  destination.tabl
-0000a750: 655f 6964 2c0a 2020 2020 2020 2020 2020  e_id,.          
-0000a760: 2020 7363 6865 6d61 3d6c 6f61 645f 7461    schema=load_ta
-0000a770: 626c 655f 6465 7374 696e 6174 696f 6e2e  ble_destination.
-0000a780: 6461 7461 7365 745f 6964 2c0a 2020 2020  dataset_id,.    
-0000a790: 2020 2020 2020 2020 6461 7461 6261 7365          database
-0000a7a0: 3d6c 6f61 645f 7461 626c 655f 6465 7374  =load_table_dest
-0000a7b0: 696e 6174 696f 6e2e 7072 6f6a 6563 742c  ination.project,
-0000a7c0: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
-0000a7d0: 2020 2020 2320 622f 3239 3735 3930 3137      # b/29759017
-0000a7e0: 3820 506f 7465 6e74 6961 6c6c 7920 6120  8 Potentially a 
-0000a7f0: 6275 6720 696e 2062 7163 6c69 656e 742e  bug in bqclient.
-0000a800: 6c6f 6164 5f74 6162 6c65 5f66 726f 6d5f  load_table_from_
-0000a810: 6461 7461 6672 616d 6528 292c 2074 6861  dataframe(), tha
-0000a820: 7420 6f6e 6c79 2077 6865 6e20 7468 6520  t only when the 
-0000a830: 4446 2069 7320 656d 7074 792c 2074 6865  DF is empty, the
-0000a840: 2069 6e64 6578 2063 6f6c 756d 6e73 2064   index columns d
-0000a850: 6973 6170 7065 6172 2069 6e20 7461 626c  isappear in tabl
-0000a860: 655f 6578 7072 6573 7369 6f6e 2e0a 2020  e_expression..  
-0000a870: 2020 2020 2020 6966 2061 6e79 280a 2020        if any(.  
-0000a880: 2020 2020 2020 2020 2020 5b6e 6577 5f69            [new_i
-0000a890: 6478 5f69 6420 6e6f 7420 696e 2074 6162  dx_id not in tab
-0000a8a0: 6c65 5f65 7870 7265 7373 696f 6e2e 636f  le_expression.co
-0000a8b0: 6c75 6d6e 7320 666f 7220 6e65 775f 6964  lumns for new_id
-0000a8c0: 785f 6964 2069 6e20 6e65 775f 6964 785f  x_id in new_idx_
-0000a8d0: 6964 735d 0a20 2020 2020 2020 2029 3a0a  ids].        ):.
-0000a8e0: 2020 2020 2020 2020 2020 2020 6e65 775f              new_
-0000a8f0: 6964 785f 6964 732c 2069 6478 5f6c 6162  idx_ids, idx_lab
-0000a900: 656c 7320 3d20 5b5d 2c20 5b5d 0a0a 2020  els = [], []..  
-0000a910: 2020 2020 2020 636f 6c75 6d6e 5f76 616c        column_val
-0000a920: 7565 7320 3d20 5b0a 2020 2020 2020 2020  ues = [.        
-0000a930: 2020 2020 7461 626c 655f 6578 7072 6573      table_expres
-0000a940: 7369 6f6e 5b63 6f6c 5d0a 2020 2020 2020  sion[col].      
-0000a950: 2020 2020 2020 666f 7220 636f 6c20 696e        for col in
-0000a960: 2074 6162 6c65 5f65 7870 7265 7373 696f   table_expressio
-0000a970: 6e2e 636f 6c75 6d6e 730a 2020 2020 2020  n.columns.      
-0000a980: 2020 2020 2020 6966 2063 6f6c 2021 3d20        if col != 
-0000a990: 6f72 6465 7269 6e67 5f63 6f6c 0a20 2020  ordering_col.   
-0000a9a0: 2020 2020 205d 0a20 2020 2020 2020 2061       ].        a
-0000a9b0: 7272 6179 5f76 616c 7565 203d 2063 6f72  rray_value = cor
-0000a9c0: 652e 4172 7261 7956 616c 7565 2e66 726f  e.ArrayValue.fro
-0000a9d0: 6d5f 6962 6973 280a 2020 2020 2020 2020  m_ibis(.        
-0000a9e0: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
-0000a9f0: 2020 2020 2020 7461 626c 655f 6578 7072        table_expr
-0000aa00: 6573 7369 6f6e 2c0a 2020 2020 2020 2020  ession,.        
-0000aa10: 2020 2020 636f 6c75 6d6e 733d 636f 6c75      columns=colu
-0000aa20: 6d6e 5f76 616c 7565 732c 0a20 2020 2020  mn_values,.     
-0000aa30: 2020 2020 2020 2068 6964 6465 6e5f 6f72         hidden_or
-0000aa40: 6465 7269 6e67 5f63 6f6c 756d 6e73 3d5b  dering_columns=[
-0000aa50: 7461 626c 655f 6578 7072 6573 7369 6f6e  table_expression
-0000aa60: 5b6f 7264 6572 696e 675f 636f 6c5d 5d2c  [ordering_col]],
-0000aa70: 0a20 2020 2020 2020 2020 2020 206f 7264  .            ord
-0000aa80: 6572 696e 673d 6f72 6465 7269 6e67 2c0a  ering=ordering,.
-0000aa90: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
-0000aaa0: 2020 2062 6c6f 636b 203d 2062 6c6f 636b     block = block
-0000aab0: 732e 426c 6f63 6b28 0a20 2020 2020 2020  s.Block(.       
-0000aac0: 2020 2020 2061 7272 6179 5f76 616c 7565       array_value
-0000aad0: 2c0a 2020 2020 2020 2020 2020 2020 696e  ,.            in
-0000aae0: 6465 785f 636f 6c75 6d6e 733d 6e65 775f  dex_columns=new_
-0000aaf0: 6964 785f 6964 732c 0a20 2020 2020 2020  idx_ids,.       
-0000ab00: 2020 2020 2063 6f6c 756d 6e5f 6c61 6265       column_labe
-0000ab10: 6c73 3d63 6f6c 5f69 6e64 6578 2c0a 2020  ls=col_index,.  
-0000ab20: 2020 2020 2020 2020 2020 696e 6465 785f            index_
-0000ab30: 6c61 6265 6c73 3d69 6478 5f6c 6162 656c  labels=idx_label
-0000ab40: 732c 0a20 2020 2020 2020 2029 0a20 2020  s,.        ).   
-0000ab50: 2020 2020 2072 6574 7572 6e20 6461 7461       return data
-0000ab60: 6672 616d 652e 4461 7461 4672 616d 6528  frame.DataFrame(
-0000ab70: 626c 6f63 6b29 0a0a 2020 2020 6465 6620  block)..    def 
-0000ab80: 7265 6164 5f63 7376 280a 2020 2020 2020  read_csv(.      
-0000ab90: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-0000aba0: 6669 6c65 7061 7468 5f6f 725f 6275 6666  filepath_or_buff
-0000abb0: 6572 3a20 7374 7220 7c20 494f 5b22 6279  er: str | IO["by
-0000abc0: 7465 7322 5d2c 0a20 2020 2020 2020 202a  tes"],.        *
-0000abd0: 2c0a 2020 2020 2020 2020 7365 703a 204f  ,.        sep: O
-0000abe0: 7074 696f 6e61 6c5b 7374 725d 203d 2022  ptional[str] = "
-0000abf0: 2c22 2c0a 2020 2020 2020 2020 6865 6164  ,",.        head
-0000ac00: 6572 3a20 4f70 7469 6f6e 616c 5b69 6e74  er: Optional[int
-0000ac10: 5d20 3d20 302c 0a20 2020 2020 2020 206e  ] = 0,.        n
-0000ac20: 616d 6573 3a20 4f70 7469 6f6e 616c 5b0a  ames: Optional[.
-0000ac30: 2020 2020 2020 2020 2020 2020 556e 696f              Unio
-0000ac40: 6e5b 4d75 7461 626c 6553 6571 7565 6e63  n[MutableSequenc
-0000ac50: 655b 416e 795d 2c20 6e70 2e6e 6461 7272  e[Any], np.ndarr
-0000ac60: 6179 5b41 6e79 2c20 416e 795d 2c20 5475  ay[Any, Any], Tu
-0000ac70: 706c 655b 416e 792c 202e 2e2e 5d2c 2072  ple[Any, ...], r
-0000ac80: 616e 6765 5d0a 2020 2020 2020 2020 5d20  ange].        ] 
-0000ac90: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-0000aca0: 696e 6465 785f 636f 6c3a 204f 7074 696f  index_col: Optio
-0000acb0: 6e61 6c5b 0a20 2020 2020 2020 2020 2020  nal[.           
-0000acc0: 2055 6e69 6f6e 5b69 6e74 2c20 7374 722c   Union[int, str,
-0000acd0: 2053 6571 7565 6e63 655b 556e 696f 6e5b   Sequence[Union[
-0000ace0: 7374 722c 2069 6e74 5d5d 2c20 4c69 7465  str, int]], Lite
-0000acf0: 7261 6c5b 4661 6c73 655d 5d0a 2020 2020  ral[False]].    
-0000ad00: 2020 2020 5d20 3d20 4e6f 6e65 2c0a 2020      ] = None,.  
-0000ad10: 2020 2020 2020 7573 6563 6f6c 733a 204f        usecols: O
-0000ad20: 7074 696f 6e61 6c5b 0a20 2020 2020 2020  ptional[.       
-0000ad30: 2020 2020 2055 6e69 6f6e 5b0a 2020 2020       Union[.    
-0000ad40: 2020 2020 2020 2020 2020 2020 4d75 7461              Muta
-0000ad50: 626c 6553 6571 7565 6e63 655b 7374 725d  bleSequence[str]
-0000ad60: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000ad70: 2020 5475 706c 655b 7374 722c 202e 2e2e    Tuple[str, ...
-0000ad80: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
-0000ad90: 2020 2053 6571 7565 6e63 655b 696e 745d     Sequence[int]
-0000ada0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000adb0: 2020 7061 6e64 6173 2e53 6572 6965 732c    pandas.Series,
-0000adc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000add0: 2070 616e 6461 732e 496e 6465 782c 0a20   pandas.Index,. 
-0000ade0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-0000adf0: 702e 6e64 6172 7261 795b 416e 792c 2041  p.ndarray[Any, A
-0000ae00: 6e79 5d2c 0a20 2020 2020 2020 2020 2020  ny],.           
-0000ae10: 2020 2020 2043 616c 6c61 626c 655b 5b41       Callable[[A
-0000ae20: 6e79 5d2c 2062 6f6f 6c5d 2c0a 2020 2020  ny], bool],.    
-0000ae30: 2020 2020 2020 2020 5d0a 2020 2020 2020          ].      
-0000ae40: 2020 5d20 3d20 4e6f 6e65 2c0a 2020 2020    ] = None,.    
-0000ae50: 2020 2020 6474 7970 653a 204f 7074 696f      dtype: Optio
-0000ae60: 6e61 6c5b 4469 6374 5d20 3d20 4e6f 6e65  nal[Dict] = None
-0000ae70: 2c0a 2020 2020 2020 2020 656e 6769 6e65  ,.        engine
-0000ae80: 3a20 4f70 7469 6f6e 616c 5b0a 2020 2020  : Optional[.    
-0000ae90: 2020 2020 2020 2020 4c69 7465 7261 6c5b          Literal[
-0000aea0: 2263 222c 2022 7079 7468 6f6e 222c 2022  "c", "python", "
-0000aeb0: 7079 6172 726f 7722 2c20 2270 7974 686f  pyarrow", "pytho
-0000aec0: 6e2d 6677 6622 2c20 2262 6967 7175 6572  n-fwf", "bigquer
-0000aed0: 7922 5d0a 2020 2020 2020 2020 5d20 3d20  y"].        ] = 
-0000aee0: 4e6f 6e65 2c0a 2020 2020 2020 2020 656e  None,.        en
-0000aef0: 636f 6469 6e67 3a20 4f70 7469 6f6e 616c  coding: Optional
-0000af00: 5b73 7472 5d20 3d20 4e6f 6e65 2c0a 2020  [str] = None,.  
-0000af10: 2020 2020 2020 2a2a 6b77 6172 6773 2c0a        **kwargs,.
-0000af20: 2020 2020 2920 2d3e 2064 6174 6166 7261      ) -> datafra
-0000af30: 6d65 2e44 6174 6146 7261 6d65 3a0a 2020  me.DataFrame:.  
-0000af40: 2020 2020 2020 7461 626c 6520 3d20 6269        table = bi
-0000af50: 6766 7261 6d65 735f 696f 2e72 616e 646f  gframes_io.rando
-0000af60: 6d5f 7461 626c 6528 7365 6c66 2e5f 616e  m_table(self._an
-0000af70: 6f6e 796d 6f75 735f 6461 7461 7365 7429  onymous_dataset)
-0000af80: 0a0a 2020 2020 2020 2020 6966 2065 6e67  ..        if eng
-0000af90: 696e 6520 6973 206e 6f74 204e 6f6e 6520  ine is not None 
-0000afa0: 616e 6420 656e 6769 6e65 203d 3d20 2262  and engine == "b
-0000afb0: 6967 7175 6572 7922 3a0a 2020 2020 2020  igquery":.      
-0000afc0: 2020 2020 2020 6966 2061 6e79 2870 6172        if any(par
-0000afd0: 616d 2069 7320 6e6f 7420 4e6f 6e65 2066  am is not None f
-0000afe0: 6f72 2070 6172 616d 2069 6e20 2864 7479  or param in (dty
-0000aff0: 7065 2c20 6e61 6d65 7329 293a 0a20 2020  pe, names)):.   
-0000b000: 2020 2020 2020 2020 2020 2020 206e 6f74               not
-0000b010: 5f73 7570 706f 7274 6564 203d 2028 2264  _supported = ("d
-0000b020: 7479 7065 222c 2022 6e61 6d65 7322 290a  type", "names").
-0000b030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b040: 7261 6973 6520 4e6f 7449 6d70 6c65 6d65  raise NotImpleme
-0000b050: 6e74 6564 4572 726f 7228 0a20 2020 2020  ntedError(.     
-0000b060: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0000b070: 2242 6967 5175 6572 7920 656e 6769 6e65  "BigQuery engine
-0000b080: 2064 6f65 7320 6e6f 7420 7375 7070 6f72   does not suppor
-0000b090: 7420 7468 6573 6520 6172 6775 6d65 6e74  t these argument
-0000b0a0: 733a 207b 6e6f 745f 7375 7070 6f72 7465  s: {not_supporte
-0000b0b0: 647d 2e20 220a 2020 2020 2020 2020 2020  d}. ".          
-0000b0c0: 2020 2020 2020 2020 2020 6622 7b63 6f6e            f"{con
-0000b0d0: 7374 616e 7473 2e46 4545 4442 4143 4b5f  stants.FEEDBACK_
-0000b0e0: 4c49 4e4b 7d22 0a20 2020 2020 2020 2020  LINK}".         
-0000b0f0: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
-0000b100: 2020 2020 2020 6966 2069 6e64 6578 5f63        if index_c
-0000b110: 6f6c 2069 7320 6e6f 7420 4e6f 6e65 2061  ol is not None a
-0000b120: 6e64 2028 0a20 2020 2020 2020 2020 2020  nd (.           
-0000b130: 2020 2020 206e 6f74 2069 6e64 6578 5f63       not index_c
-0000b140: 6f6c 206f 7220 6e6f 7420 6973 696e 7374  ol or not isinst
-0000b150: 616e 6365 2869 6e64 6578 5f63 6f6c 2c20  ance(index_col, 
-0000b160: 7374 7229 0a20 2020 2020 2020 2020 2020  str).           
-0000b170: 2029 3a0a 2020 2020 2020 2020 2020 2020   ):.            
-0000b180: 2020 2020 7261 6973 6520 4e6f 7449 6d70      raise NotImp
-0000b190: 6c65 6d65 6e74 6564 4572 726f 7228 0a20  lementedError(. 
-0000b1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b1b0: 2020 2022 4269 6751 7565 7279 2065 6e67     "BigQuery eng
-0000b1c0: 696e 6520 6f6e 6c79 2073 7570 706f 7274  ine only support
-0000b1d0: 7320 6120 7369 6e67 6c65 2063 6f6c 756d  s a single colum
-0000b1e0: 6e20 6e61 6d65 2066 6f72 2060 696e 6465  n name for `inde
-0000b1f0: 785f 636f 6c60 2e20 220a 2020 2020 2020  x_col`. ".      
-0000b200: 2020 2020 2020 2020 2020 2020 2020 6622                f"
-0000b210: 7b63 6f6e 7374 616e 7473 2e46 4545 4442  {constants.FEEDB
-0000b220: 4143 4b5f 4c49 4e4b 7d22 0a20 2020 2020  ACK_LINK}".     
-0000b230: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
-0000b240: 2020 2020 2020 2020 2020 2320 4e6f 6e65            # None
-0000b250: 2076 616c 7565 2066 6f72 2069 6e64 6578   value for index
-0000b260: 5f63 6f6c 2063 616e 6e6f 7420 6265 2070  _col cannot be p
-0000b270: 6173 7365 6420 746f 2072 6561 645f 6762  assed to read_gb
-0000b280: 710a 2020 2020 2020 2020 2020 2020 6966  q.            if
-0000b290: 2069 6e64 6578 5f63 6f6c 2069 7320 4e6f   index_col is No
-0000b2a0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0000b2b0: 2020 2020 696e 6465 785f 636f 6c20 3d20      index_col = 
-0000b2c0: 2829 0a0a 2020 2020 2020 2020 2020 2020  ()..            
-0000b2d0: 2320 7573 6563 6f6c 7320 7368 6f75 6c64  # usecols should
-0000b2e0: 206f 6e6c 7920 6265 2061 6e20 6974 6572   only be an iter
-0000b2f0: 6162 6c65 206f 6620 7374 7269 6e67 7320  able of strings 
-0000b300: 2863 6f6c 756d 6e20 6e61 6d65 7329 2066  (column names) f
-0000b310: 6f72 2075 7365 2061 7320 636f 6c75 6d6e  or use as column
-0000b320: 7320 696e 2072 6561 645f 6762 712e 0a20  s in read_gbq.. 
-0000b330: 2020 2020 2020 2020 2020 2063 6f6c 756d             colum
-0000b340: 6e73 3a20 5475 706c 655b 416e 792c 202e  ns: Tuple[Any, .
-0000b350: 2e2e 5d20 3d20 7475 706c 6528 290a 2020  ..] = tuple().  
-0000b360: 2020 2020 2020 2020 2020 6966 2075 7365            if use
-0000b370: 636f 6c73 2069 7320 6e6f 7420 4e6f 6e65  cols is not None
-0000b380: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000b390: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
-0000b3a0: 7573 6563 6f6c 732c 2049 7465 7261 626c  usecols, Iterabl
-0000b3b0: 6529 2061 6e64 2061 6c6c 280a 2020 2020  e) and all(.    
-0000b3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b3d0: 6973 696e 7374 616e 6365 2863 6f6c 2c20  isinstance(col, 
-0000b3e0: 7374 7229 2066 6f72 2063 6f6c 2069 6e20  str) for col in 
-0000b3f0: 7573 6563 6f6c 730a 2020 2020 2020 2020  usecols.        
-0000b400: 2020 2020 2020 2020 293a 0a20 2020 2020          ):.     
-0000b410: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-0000b420: 6f6c 756d 6e73 203d 2074 7570 6c65 2863  olumns = tuple(c
-0000b430: 6f6c 2066 6f72 2063 6f6c 2069 6e20 7573  ol for col in us
-0000b440: 6563 6f6c 7329 0a20 2020 2020 2020 2020  ecols).         
-0000b450: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-0000b460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b470: 2072 6169 7365 204e 6f74 496d 706c 656d   raise NotImplem
-0000b480: 656e 7465 6445 7272 6f72 280a 2020 2020  entedError(.    
-0000b490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b4a0: 2020 2020 2242 6967 5175 6572 7920 656e      "BigQuery en
-0000b4b0: 6769 6e65 206f 6e6c 7920 7375 7070 6f72  gine only suppor
-0000b4c0: 7473 2061 6e20 6974 6572 6162 6c65 206f  ts an iterable o
-0000b4d0: 6620 7374 7269 6e67 7320 666f 7220 6075  f strings for `u
-0000b4e0: 7365 636f 6c73 602e 2022 0a20 2020 2020  secols`. ".     
-0000b4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b500: 2020 2066 227b 636f 6e73 7461 6e74 732e     f"{constants.
-0000b510: 4645 4544 4241 434b 5f4c 494e 4b7d 220a  FEEDBACK_LINK}".
-0000b520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b530: 2020 2020 290a 0a20 2020 2020 2020 2020      )..         
-0000b540: 2020 2069 6620 656e 636f 6469 6e67 2069     if encoding i
-0000b550: 7320 6e6f 7420 4e6f 6e65 2061 6e64 2065  s not None and e
-0000b560: 6e63 6f64 696e 6720 6e6f 7420 696e 205f  ncoding not in _
-0000b570: 5641 4c49 445f 454e 434f 4449 4e47 533a  VALID_ENCODINGS:
-0000b580: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b590: 2072 6169 7365 204e 6f74 496d 706c 656d   raise NotImplem
-0000b5a0: 656e 7465 6445 7272 6f72 280a 2020 2020  entedError(.    
+00009990: 6466 0a20 2020 2020 2020 2074 7279 3a0a  df.        try:.
+000099a0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+000099b0: 726e 2073 656c 662e 5f72 6561 645f 7061  rn self._read_pa
+000099c0: 6e64 6173 5f6c 6f61 645f 6a6f 6228 7061  ndas_load_job(pa
+000099d0: 6e64 6173 5f64 6174 6166 7261 6d65 2c20  ndas_dataframe, 
+000099e0: 6170 695f 6e61 6d65 290a 2020 2020 2020  api_name).      
+000099f0: 2020 6578 6365 7074 2070 612e 4172 726f    except pa.Arro
+00009a00: 7749 6e76 616c 6964 2061 7320 653a 0a20  wInvalid as e:. 
+00009a10: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+00009a20: 2070 612e 4172 726f 7749 6e76 616c 6964   pa.ArrowInvalid
+00009a30: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00009a40: 2020 6622 436f 756c 6420 6e6f 7420 636f    f"Could not co
+00009a50: 6e76 6572 7420 7769 7468 2061 2042 6967  nvert with a Big
+00009a60: 5175 6572 7920 7479 7065 3a20 607b 657d  Query type: `{e}
+00009a70: 602e 2022 0a20 2020 2020 2020 2020 2020  `. ".           
+00009a80: 2029 2066 726f 6d20 650a 0a20 2020 2064   ) from e..    d
+00009a90: 6566 205f 7265 6164 5f70 616e 6461 735f  ef _read_pandas_
+00009aa0: 696e 6c69 6e65 280a 2020 2020 2020 2020  inline(.        
+00009ab0: 7365 6c66 2c20 7061 6e64 6173 5f64 6174  self, pandas_dat
+00009ac0: 6166 7261 6d65 3a20 7061 6e64 6173 2e44  aframe: pandas.D
+00009ad0: 6174 6146 7261 6d65 0a20 2020 2029 202d  ataFrame.    ) -
+00009ae0: 3e20 4f70 7469 6f6e 616c 5b64 6174 6166  > Optional[dataf
+00009af0: 7261 6d65 2e44 6174 6146 7261 6d65 5d3a  rame.DataFrame]:
+00009b00: 0a20 2020 2020 2020 2069 6d70 6f72 7420  .        import 
+00009b10: 6269 6766 7261 6d65 732e 6461 7461 6672  bigframes.datafr
+00009b20: 616d 6520 6173 2064 6174 6166 7261 6d65  ame as dataframe
+00009b30: 0a0a 2020 2020 2020 2020 6966 2070 616e  ..        if pan
+00009b40: 6461 735f 6461 7461 6672 616d 652e 6d65  das_dataframe.me
+00009b50: 6d6f 7279 5f75 7361 6765 2864 6565 703d  mory_usage(deep=
+00009b60: 5472 7565 292e 7375 6d28 2920 3e20 4d41  True).sum() > MA
+00009b70: 585f 494e 4c49 4e45 5f44 465f 4259 5445  X_INLINE_DF_BYTE
+00009b80: 533a 0a20 2020 2020 2020 2020 2020 2072  S:.            r
+00009b90: 6574 7572 6e20 4e6f 6e65 0a0a 2020 2020  eturn None..    
+00009ba0: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
+00009bb0: 2020 2020 2069 6e6c 696e 655f 6466 203d       inline_df =
+00009bc0: 2064 6174 6166 7261 6d65 2e44 6174 6146   dataframe.DataF
+00009bd0: 7261 6d65 280a 2020 2020 2020 2020 2020  rame(.          
+00009be0: 2020 2020 2020 626c 6f63 6b73 2e42 6c6f        blocks.Blo
+00009bf0: 636b 2e66 726f 6d5f 6c6f 6361 6c28 7061  ck.from_local(pa
+00009c00: 6e64 6173 5f64 6174 6166 7261 6d65 2c20  ndas_dataframe, 
+00009c10: 7365 6c66 290a 2020 2020 2020 2020 2020  self).          
+00009c20: 2020 290a 2020 2020 2020 2020 6578 6365    ).        exce
+00009c30: 7074 2070 612e 4172 726f 7749 6e76 616c  pt pa.ArrowInval
+00009c40: 6964 2061 7320 653a 0a20 2020 2020 2020  id as e:.       
+00009c50: 2020 2020 2072 6169 7365 2070 612e 4172       raise pa.Ar
+00009c60: 726f 7749 6e76 616c 6964 280a 2020 2020  rowInvalid(.    
+00009c70: 2020 2020 2020 2020 2020 2020 6622 436f              f"Co
+00009c80: 756c 6420 6e6f 7420 636f 6e76 6572 7420  uld not convert 
+00009c90: 7769 7468 2061 2042 6967 5175 6572 7920  with a BigQuery 
+00009ca0: 7479 7065 3a20 607b 657d 602e 2022 0a20  type: `{e}`. ". 
+00009cb0: 2020 2020 2020 2020 2020 2029 2066 726f             ) fro
+00009cc0: 6d20 650a 2020 2020 2020 2020 6578 6365  m e.        exce
+00009cd0: 7074 2056 616c 7565 4572 726f 723a 2020  pt ValueError:  
+00009ce0: 2320 5468 726f 776e 2062 7920 6962 6973  # Thrown by ibis
+00009cf0: 2066 6f72 2073 6f6d 6520 756e 6861 6e64   for some unhand
+00009d00: 6c65 6420 7479 7065 730a 2020 2020 2020  led types.      
+00009d10: 2020 2020 2020 7265 7475 726e 204e 6f6e        return Non
+00009d20: 650a 2020 2020 2020 2020 6578 6365 7074  e.        except
+00009d30: 2070 612e 4172 726f 7754 7970 6545 7272   pa.ArrowTypeErr
+00009d40: 6f72 3a20 2023 2054 6872 6f77 6e20 6279  or:  # Thrown by
+00009d50: 2061 7272 6f77 2066 6f72 2074 7970 6573   arrow for types
+00009d60: 2077 6974 686f 7574 206d 6170 7069 6e67   without mapping
+00009d70: 2028 6765 6f29 2e0a 2020 2020 2020 2020   (geo)..        
+00009d80: 2020 2020 7265 7475 726e 204e 6f6e 650a      return None.
+00009d90: 0a20 2020 2020 2020 2069 6e6c 696e 655f  .        inline_
+00009da0: 7479 7065 7320 3d20 696e 6c69 6e65 5f64  types = inline_d
+00009db0: 662e 5f62 6c6f 636b 2e65 7870 722e 7363  f._block.expr.sc
+00009dc0: 6865 6d61 2e64 7479 7065 730a 2020 2020  hema.dtypes.    
+00009dd0: 2020 2020 2320 4962 6973 2068 6173 2070      # Ibis has p
+00009de0: 726f 626c 656d 7320 6573 6361 7069 6e67  roblems escaping
+00009df0: 2062 7974 6573 206c 6974 6572 616c 732c   bytes literals,
+00009e00: 2077 6869 6368 2077 696c 6c20 6361 7573   which will caus
+00009e10: 6520 7379 6e74 6178 2065 7272 6f72 7320  e syntax errors 
+00009e20: 7365 7276 6572 2d73 6964 652e 0a20 2020  server-side..   
+00009e30: 2020 2020 2069 6620 616c 6c28 6474 7970       if all(dtyp
+00009e40: 6520 696e 2049 4e4c 494e 4142 4c45 5f44  e in INLINABLE_D
+00009e50: 5459 5045 5320 666f 7220 6474 7970 6520  TYPES for dtype 
+00009e60: 696e 2069 6e6c 696e 655f 7479 7065 7329  in inline_types)
+00009e70: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00009e80: 7475 726e 2069 6e6c 696e 655f 6466 0a20  turn inline_df. 
+00009e90: 2020 2020 2020 2072 6574 7572 6e20 4e6f         return No
+00009ea0: 6e65 0a0a 2020 2020 6465 6620 5f72 6561  ne..    def _rea
+00009eb0: 645f 7061 6e64 6173 5f6c 6f61 645f 6a6f  d_pandas_load_jo
+00009ec0: 6228 0a20 2020 2020 2020 2073 656c 662c  b(.        self,
+00009ed0: 2070 616e 6461 735f 6461 7461 6672 616d   pandas_datafram
+00009ee0: 653a 2070 616e 6461 732e 4461 7461 4672  e: pandas.DataFr
+00009ef0: 616d 652c 2061 7069 5f6e 616d 653a 2073  ame, api_name: s
+00009f00: 7472 0a20 2020 2029 202d 3e20 6461 7461  tr.    ) -> data
+00009f10: 6672 616d 652e 4461 7461 4672 616d 653a  frame.DataFrame:
+00009f20: 0a20 2020 2020 2020 2069 6d70 6f72 7420  .        import 
+00009f30: 6269 6766 7261 6d65 732e 6461 7461 6672  bigframes.datafr
+00009f40: 616d 6520 6173 2064 6174 6166 7261 6d65  ame as dataframe
+00009f50: 0a0a 2020 2020 2020 2020 636f 6c5f 696e  ..        col_in
+00009f60: 6465 7820 3d20 7061 6e64 6173 5f64 6174  dex = pandas_dat
+00009f70: 6166 7261 6d65 2e63 6f6c 756d 6e73 2e63  aframe.columns.c
+00009f80: 6f70 7928 290a 2020 2020 2020 2020 636f  opy().        co
+00009f90: 6c5f 6c61 6265 6c73 2c20 6964 785f 6c61  l_labels, idx_la
+00009fa0: 6265 6c73 203d 2028 0a20 2020 2020 2020  bels = (.       
+00009fb0: 2020 2020 2063 6f6c 5f69 6e64 6578 2e74       col_index.t
+00009fc0: 6f5f 6c69 7374 2829 2c0a 2020 2020 2020  o_list(),.      
+00009fd0: 2020 2020 2020 7061 6e64 6173 5f64 6174        pandas_dat
+00009fe0: 6166 7261 6d65 2e69 6e64 6578 2e6e 616d  aframe.index.nam
+00009ff0: 6573 2c0a 2020 2020 2020 2020 290a 2020  es,.        ).  
+0000a000: 2020 2020 2020 6e65 775f 636f 6c5f 6964        new_col_id
+0000a010: 732c 206e 6577 5f69 6478 5f69 6473 203d  s, new_idx_ids =
+0000a020: 2075 7469 6c73 2e67 6574 5f73 7461 6e64   utils.get_stand
+0000a030: 6172 6469 7a65 645f 6964 7328 0a20 2020  ardized_ids(.   
+0000a040: 2020 2020 2020 2020 2063 6f6c 5f6c 6162           col_lab
+0000a050: 656c 732c 0a20 2020 2020 2020 2020 2020  els,.           
+0000a060: 2069 6478 5f6c 6162 656c 732c 0a20 2020   idx_labels,.   
+0000a070: 2020 2020 2020 2020 2023 204c 6f61 6469           # Loadi
+0000a080: 6e67 2070 6172 7175 6574 2066 696c 6573  ng parquet files
+0000a090: 2069 6e74 6f20 4269 6751 7565 7279 2077   into BigQuery w
+0000a0a0: 6974 6820 7370 6563 6961 6c20 636f 6c75  ith special colu
+0000a0b0: 6d6e 206e 616d 6573 0a20 2020 2020 2020  mn names.       
+0000a0c0: 2020 2020 2023 2069 7320 6f6e 6c79 2073       # is only s
+0000a0d0: 7570 706f 7274 6564 2075 6e64 6572 2061  upported under a
+0000a0e0: 6e20 616c 6c6f 776c 6973 742e 0a20 2020  n allowlist..   
+0000a0f0: 2020 2020 2020 2020 2073 7472 6963 743d           strict=
+0000a100: 5472 7565 2c0a 2020 2020 2020 2020 290a  True,.        ).
+0000a110: 0a20 2020 2020 2020 2023 2041 6464 206f  .        # Add o
+0000a120: 7264 6572 2063 6f6c 756d 6e20 746f 2070  rder column to p
+0000a130: 616e 6461 7320 4461 7461 4672 616d 6520  andas DataFrame 
+0000a140: 746f 2070 7265 7365 7276 6520 6f72 6465  to preserve orde
+0000a150: 7220 696e 2042 6967 5175 6572 790a 2020  r in BigQuery.  
+0000a160: 2020 2020 2020 6f72 6465 7269 6e67 5f63        ordering_c
+0000a170: 6f6c 203d 2022 726f 7769 6422 0a20 2020  ol = "rowid".   
+0000a180: 2020 2020 2063 6f6c 756d 6e73 203d 2066       columns = f
+0000a190: 726f 7a65 6e73 6574 2863 6f6c 5f6c 6162  rozenset(col_lab
+0000a1a0: 656c 7320 2b20 6964 785f 6c61 6265 6c73  els + idx_labels
+0000a1b0: 290a 2020 2020 2020 2020 7375 6666 6978  ).        suffix
+0000a1c0: 203d 2032 0a20 2020 2020 2020 2077 6869   = 2.        whi
+0000a1d0: 6c65 206f 7264 6572 696e 675f 636f 6c20  le ordering_col 
+0000a1e0: 696e 2063 6f6c 756d 6e73 3a0a 2020 2020  in columns:.    
+0000a1f0: 2020 2020 2020 2020 6f72 6465 7269 6e67          ordering
+0000a200: 5f63 6f6c 203d 2066 2272 6f77 6964 5f7b  _col = f"rowid_{
+0000a210: 7375 6666 6978 7d22 0a20 2020 2020 2020  suffix}".       
+0000a220: 2020 2020 2073 7566 6669 7820 2b3d 2031       suffix += 1
+0000a230: 0a0a 2020 2020 2020 2020 7061 6e64 6173  ..        pandas
+0000a240: 5f64 6174 6166 7261 6d65 5f63 6f70 7920  _dataframe_copy 
+0000a250: 3d20 7061 6e64 6173 5f64 6174 6166 7261  = pandas_datafra
+0000a260: 6d65 2e63 6f70 7928 290a 2020 2020 2020  me.copy().      
+0000a270: 2020 7061 6e64 6173 5f64 6174 6166 7261    pandas_datafra
+0000a280: 6d65 5f63 6f70 792e 696e 6465 782e 6e61  me_copy.index.na
+0000a290: 6d65 7320 3d20 6e65 775f 6964 785f 6964  mes = new_idx_id
+0000a2a0: 730a 2020 2020 2020 2020 7061 6e64 6173  s.        pandas
+0000a2b0: 5f64 6174 6166 7261 6d65 5f63 6f70 792e  _dataframe_copy.
+0000a2c0: 636f 6c75 6d6e 7320 3d20 7061 6e64 6173  columns = pandas
+0000a2d0: 2e49 6e64 6578 286e 6577 5f63 6f6c 5f69  .Index(new_col_i
+0000a2e0: 6473 290a 2020 2020 2020 2020 7061 6e64  ds).        pand
+0000a2f0: 6173 5f64 6174 6166 7261 6d65 5f63 6f70  as_dataframe_cop
+0000a300: 795b 6f72 6465 7269 6e67 5f63 6f6c 5d20  y[ordering_col] 
+0000a310: 3d20 6e70 2e61 7261 6e67 6528 7061 6e64  = np.arange(pand
+0000a320: 6173 5f64 6174 6166 7261 6d65 5f63 6f70  as_dataframe_cop
+0000a330: 792e 7368 6170 655b 305d 290a 0a20 2020  y.shape[0])..   
+0000a340: 2020 2020 206a 6f62 5f63 6f6e 6669 6720       job_config 
+0000a350: 3d20 7365 6c66 2e5f 7072 6570 6172 655f  = self._prepare_
+0000a360: 6c6f 6164 5f6a 6f62 5f63 6f6e 6669 6728  load_job_config(
+0000a370: 290a 0a20 2020 2020 2020 2023 2053 7065  )..        # Spe
+0000a380: 6369 6679 2074 6865 2064 6174 6574 696d  cify the datetim
+0000a390: 6520 6474 7970 6573 2c20 7768 6963 6820  e dtypes, which 
+0000a3a0: 6973 2061 7574 6f2d 6465 7465 6374 6564  is auto-detected
+0000a3b0: 2061 7320 7469 6d65 7374 616d 7020 7479   as timestamp ty
+0000a3c0: 7065 732e 0a20 2020 2020 2020 2073 6368  pes..        sch
+0000a3d0: 656d 613a 206c 6973 745b 6269 6771 7565  ema: list[bigque
+0000a3e0: 7279 2e53 6368 656d 6146 6965 6c64 5d20  ry.SchemaField] 
+0000a3f0: 3d20 5b5d 0a20 2020 2020 2020 2066 6f72  = [].        for
+0000a400: 2063 6f6c 756d 6e2c 2064 7479 7065 2069   column, dtype i
+0000a410: 6e20 7a69 7028 6e65 775f 636f 6c5f 6964  n zip(new_col_id
+0000a420: 732c 2070 616e 6461 735f 6461 7461 6672  s, pandas_datafr
+0000a430: 616d 652e 6474 7970 6573 293a 0a20 2020  ame.dtypes):.   
+0000a440: 2020 2020 2020 2020 2069 6620 6474 7970           if dtyp
+0000a450: 6520 3d3d 2022 7469 6d65 7374 616d 705b  e == "timestamp[
+0000a460: 7573 5d5b 7079 6172 726f 775d 223a 0a20  us][pyarrow]":. 
+0000a470: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000a480: 6368 656d 612e 6170 7065 6e64 280a 2020  chema.append(.  
+0000a490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a4a0: 2020 6269 6771 7565 7279 2e53 6368 656d    bigquery.Schem
+0000a4b0: 6146 6965 6c64 2863 6f6c 756d 6e2c 2062  aField(column, b
+0000a4c0: 6967 7175 6572 792e 656e 756d 732e 5371  igquery.enums.Sq
+0000a4d0: 6c54 7970 654e 616d 6573 2e44 4154 4554  lTypeNames.DATET
+0000a4e0: 494d 4529 0a20 2020 2020 2020 2020 2020  IME).           
+0000a4f0: 2020 2020 2029 0a20 2020 2020 2020 206a       ).        j
+0000a500: 6f62 5f63 6f6e 6669 672e 7363 6865 6d61  ob_config.schema
+0000a510: 203d 2073 6368 656d 610a 0a20 2020 2020   = schema..     
+0000a520: 2020 2023 2043 6c75 7374 6572 696e 6720     # Clustering 
+0000a530: 7072 6f62 6162 6c79 206e 6f74 206e 6565  probably not nee
+0000a540: 6465 6420 616e 7977 6179 7320 6173 2070  ded anyways as p
+0000a550: 616e 6461 7320 7461 626c 6573 2061 7265  andas tables are
+0000a560: 2073 6d61 6c6c 0a20 2020 2020 2020 2063   small.        c
+0000a570: 6c75 7374 6572 5f63 6f6c 7320 3d20 5b6f  luster_cols = [o
+0000a580: 7264 6572 696e 675f 636f 6c5d 0a20 2020  rdering_col].   
+0000a590: 2020 2020 206a 6f62 5f63 6f6e 6669 672e       job_config.
+0000a5a0: 636c 7573 7465 7269 6e67 5f66 6965 6c64  clustering_field
+0000a5b0: 7320 3d20 636c 7573 7465 725f 636f 6c73  s = cluster_cols
+0000a5c0: 0a0a 2020 2020 2020 2020 6a6f 625f 636f  ..        job_co
+0000a5d0: 6e66 6967 2e6c 6162 656c 7320 3d20 7b22  nfig.labels = {"
+0000a5e0: 6269 6766 7261 6d65 732d 6170 6922 3a20  bigframes-api": 
+0000a5f0: 6170 695f 6e61 6d65 7d0a 0a20 2020 2020  api_name}..     
+0000a600: 2020 206c 6f61 645f 7461 626c 655f 6465     load_table_de
+0000a610: 7374 696e 6174 696f 6e20 3d20 6269 6766  stination = bigf
+0000a620: 7261 6d65 735f 696f 2e72 616e 646f 6d5f  rames_io.random_
+0000a630: 7461 626c 6528 7365 6c66 2e5f 616e 6f6e  table(self._anon
+0000a640: 796d 6f75 735f 6461 7461 7365 7429 0a20  ymous_dataset). 
+0000a650: 2020 2020 2020 206c 6f61 645f 6a6f 6220         load_job 
+0000a660: 3d20 7365 6c66 2e62 7163 6c69 656e 742e  = self.bqclient.
+0000a670: 6c6f 6164 5f74 6162 6c65 5f66 726f 6d5f  load_table_from_
+0000a680: 6461 7461 6672 616d 6528 0a20 2020 2020  dataframe(.     
+0000a690: 2020 2020 2020 2070 616e 6461 735f 6461         pandas_da
+0000a6a0: 7461 6672 616d 655f 636f 7079 2c0a 2020  taframe_copy,.  
+0000a6b0: 2020 2020 2020 2020 2020 6c6f 6164 5f74            load_t
+0000a6c0: 6162 6c65 5f64 6573 7469 6e61 7469 6f6e  able_destination
+0000a6d0: 2c0a 2020 2020 2020 2020 2020 2020 6a6f  ,.            jo
+0000a6e0: 625f 636f 6e66 6967 3d6a 6f62 5f63 6f6e  b_config=job_con
+0000a6f0: 6669 672c 0a20 2020 2020 2020 2029 0a20  fig,.        ). 
+0000a700: 2020 2020 2020 2073 656c 662e 5f73 7461         self._sta
+0000a710: 7274 5f67 656e 6572 6963 5f6a 6f62 286c  rt_generic_job(l
+0000a720: 6f61 645f 6a6f 6229 0a0a 2020 2020 2020  oad_job)..      
+0000a730: 2020 6f72 6465 7269 6e67 203d 206f 7264    ordering = ord
+0000a740: 6572 2e45 7870 7265 7373 696f 6e4f 7264  er.ExpressionOrd
+0000a750: 6572 696e 6728 0a20 2020 2020 2020 2020  ering(.         
+0000a760: 2020 206f 7264 6572 696e 675f 7661 6c75     ordering_valu
+0000a770: 655f 636f 6c75 6d6e 733d 7475 706c 6528  e_columns=tuple(
+0000a780: 5b6f 7264 6572 2e61 7363 656e 6469 6e67  [order.ascending
+0000a790: 5f6f 7665 7228 6f72 6465 7269 6e67 5f63  _over(ordering_c
+0000a7a0: 6f6c 295d 292c 0a20 2020 2020 2020 2020  ol)]),.         
+0000a7b0: 2020 2074 6f74 616c 5f6f 7264 6572 696e     total_orderin
+0000a7c0: 675f 636f 6c75 6d6e 733d 6672 6f7a 656e  g_columns=frozen
+0000a7d0: 7365 7428 5b6f 7264 6572 696e 675f 636f  set([ordering_co
+0000a7e0: 6c5d 292c 0a20 2020 2020 2020 2020 2020  l]),.           
+0000a7f0: 2069 6e74 6567 6572 5f65 6e63 6f64 696e   integer_encodin
+0000a800: 673d 496e 7465 6765 7245 6e63 6f64 696e  g=IntegerEncodin
+0000a810: 6728 5472 7565 2c20 6973 5f73 6571 7565  g(True, is_seque
+0000a820: 6e74 6961 6c3d 5472 7565 292c 0a20 2020  ntial=True),.   
+0000a830: 2020 2020 2029 0a20 2020 2020 2020 2074       ).        t
+0000a840: 6162 6c65 5f65 7870 7265 7373 696f 6e20  able_expression 
+0000a850: 3d20 7365 6c66 2e69 6269 735f 636c 6965  = self.ibis_clie
+0000a860: 6e74 2e74 6162 6c65 2820 2023 2074 7970  nt.table(  # typ
+0000a870: 653a 2069 676e 6f72 650a 2020 2020 2020  e: ignore.      
+0000a880: 2020 2020 2020 6c6f 6164 5f74 6162 6c65        load_table
+0000a890: 5f64 6573 7469 6e61 7469 6f6e 2e74 6162  _destination.tab
+0000a8a0: 6c65 5f69 642c 0a20 2020 2020 2020 2020  le_id,.         
+0000a8b0: 2020 2073 6368 656d 613d 6c6f 6164 5f74     schema=load_t
+0000a8c0: 6162 6c65 5f64 6573 7469 6e61 7469 6f6e  able_destination
+0000a8d0: 2e64 6174 6173 6574 5f69 642c 0a20 2020  .dataset_id,.   
+0000a8e0: 2020 2020 2020 2020 2064 6174 6162 6173           databas
+0000a8f0: 653d 6c6f 6164 5f74 6162 6c65 5f64 6573  e=load_table_des
+0000a900: 7469 6e61 7469 6f6e 2e70 726f 6a65 6374  tination.project
+0000a910: 2c0a 2020 2020 2020 2020 290a 0a20 2020  ,.        )..   
+0000a920: 2020 2020 2023 2062 2f32 3937 3539 3031       # b/2975901
+0000a930: 3738 2050 6f74 656e 7469 616c 6c79 2061  78 Potentially a
+0000a940: 2062 7567 2069 6e20 6271 636c 6965 6e74   bug in bqclient
+0000a950: 2e6c 6f61 645f 7461 626c 655f 6672 6f6d  .load_table_from
+0000a960: 5f64 6174 6166 7261 6d65 2829 2c20 7468  _dataframe(), th
+0000a970: 6174 206f 6e6c 7920 7768 656e 2074 6865  at only when the
+0000a980: 2044 4620 6973 2065 6d70 7479 2c20 7468   DF is empty, th
+0000a990: 6520 696e 6465 7820 636f 6c75 6d6e 7320  e index columns 
+0000a9a0: 6469 7361 7070 6561 7220 696e 2074 6162  disappear in tab
+0000a9b0: 6c65 5f65 7870 7265 7373 696f 6e2e 0a20  le_expression.. 
+0000a9c0: 2020 2020 2020 2069 6620 616e 7928 0a20         if any(. 
+0000a9d0: 2020 2020 2020 2020 2020 205b 6e65 775f             [new_
+0000a9e0: 6964 785f 6964 206e 6f74 2069 6e20 7461  idx_id not in ta
+0000a9f0: 626c 655f 6578 7072 6573 7369 6f6e 2e63  ble_expression.c
+0000aa00: 6f6c 756d 6e73 2066 6f72 206e 6577 5f69  olumns for new_i
+0000aa10: 6478 5f69 6420 696e 206e 6577 5f69 6478  dx_id in new_idx
+0000aa20: 5f69 6473 5d0a 2020 2020 2020 2020 293a  _ids].        ):
+0000aa30: 0a20 2020 2020 2020 2020 2020 206e 6577  .            new
+0000aa40: 5f69 6478 5f69 6473 2c20 6964 785f 6c61  _idx_ids, idx_la
+0000aa50: 6265 6c73 203d 205b 5d2c 205b 5d0a 0a20  bels = [], [].. 
+0000aa60: 2020 2020 2020 2063 6f6c 756d 6e5f 7661         column_va
+0000aa70: 6c75 6573 203d 205b 0a20 2020 2020 2020  lues = [.       
+0000aa80: 2020 2020 2074 6162 6c65 5f65 7870 7265       table_expre
+0000aa90: 7373 696f 6e5b 636f 6c5d 0a20 2020 2020  ssion[col].     
+0000aaa0: 2020 2020 2020 2066 6f72 2063 6f6c 2069         for col i
+0000aab0: 6e20 7461 626c 655f 6578 7072 6573 7369  n table_expressi
+0000aac0: 6f6e 2e63 6f6c 756d 6e73 0a20 2020 2020  on.columns.     
+0000aad0: 2020 2020 2020 2069 6620 636f 6c20 213d         if col !=
+0000aae0: 206f 7264 6572 696e 675f 636f 6c0a 2020   ordering_col.  
+0000aaf0: 2020 2020 2020 5d0a 2020 2020 2020 2020        ].        
+0000ab00: 6172 7261 795f 7661 6c75 6520 3d20 636f  array_value = co
+0000ab10: 7265 2e41 7272 6179 5661 6c75 652e 6672  re.ArrayValue.fr
+0000ab20: 6f6d 5f69 6269 7328 0a20 2020 2020 2020  om_ibis(.       
+0000ab30: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+0000ab40: 2020 2020 2020 2074 6162 6c65 5f65 7870         table_exp
+0000ab50: 7265 7373 696f 6e2c 0a20 2020 2020 2020  ression,.       
+0000ab60: 2020 2020 2063 6f6c 756d 6e73 3d63 6f6c       columns=col
+0000ab70: 756d 6e5f 7661 6c75 6573 2c0a 2020 2020  umn_values,.    
+0000ab80: 2020 2020 2020 2020 6869 6464 656e 5f6f          hidden_o
+0000ab90: 7264 6572 696e 675f 636f 6c75 6d6e 733d  rdering_columns=
+0000aba0: 5b74 6162 6c65 5f65 7870 7265 7373 696f  [table_expressio
+0000abb0: 6e5b 6f72 6465 7269 6e67 5f63 6f6c 5d5d  n[ordering_col]]
+0000abc0: 2c0a 2020 2020 2020 2020 2020 2020 6f72  ,.            or
+0000abd0: 6465 7269 6e67 3d6f 7264 6572 696e 672c  dering=ordering,
+0000abe0: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
+0000abf0: 2020 2020 626c 6f63 6b20 3d20 626c 6f63      block = bloc
+0000ac00: 6b73 2e42 6c6f 636b 280a 2020 2020 2020  ks.Block(.      
+0000ac10: 2020 2020 2020 6172 7261 795f 7661 6c75        array_valu
+0000ac20: 652c 0a20 2020 2020 2020 2020 2020 2069  e,.            i
+0000ac30: 6e64 6578 5f63 6f6c 756d 6e73 3d6e 6577  ndex_columns=new
+0000ac40: 5f69 6478 5f69 6473 2c0a 2020 2020 2020  _idx_ids,.      
+0000ac50: 2020 2020 2020 636f 6c75 6d6e 5f6c 6162        column_lab
+0000ac60: 656c 733d 636f 6c5f 696e 6465 782c 0a20  els=col_index,. 
+0000ac70: 2020 2020 2020 2020 2020 2069 6e64 6578             index
+0000ac80: 5f6c 6162 656c 733d 6964 785f 6c61 6265  _labels=idx_labe
+0000ac90: 6c73 2c0a 2020 2020 2020 2020 290a 2020  ls,.        ).  
+0000aca0: 2020 2020 2020 7265 7475 726e 2064 6174        return dat
+0000acb0: 6166 7261 6d65 2e44 6174 6146 7261 6d65  aframe.DataFrame
+0000acc0: 2862 6c6f 636b 290a 0a20 2020 2064 6566  (block)..    def
+0000acd0: 2072 6561 645f 6373 7628 0a20 2020 2020   read_csv(.     
+0000ace0: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+0000acf0: 2066 696c 6570 6174 685f 6f72 5f62 7566   filepath_or_buf
+0000ad00: 6665 723a 2073 7472 207c 2049 4f5b 2262  fer: str | IO["b
+0000ad10: 7974 6573 225d 2c0a 2020 2020 2020 2020  ytes"],.        
+0000ad20: 2a2c 0a20 2020 2020 2020 2073 6570 3a20  *,.        sep: 
+0000ad30: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
+0000ad40: 222c 222c 0a20 2020 2020 2020 2068 6561  ",",.        hea
+0000ad50: 6465 723a 204f 7074 696f 6e61 6c5b 696e  der: Optional[in
+0000ad60: 745d 203d 2030 2c0a 2020 2020 2020 2020  t] = 0,.        
+0000ad70: 6e61 6d65 733a 204f 7074 696f 6e61 6c5b  names: Optional[
+0000ad80: 0a20 2020 2020 2020 2020 2020 2055 6e69  .            Uni
+0000ad90: 6f6e 5b4d 7574 6162 6c65 5365 7175 656e  on[MutableSequen
+0000ada0: 6365 5b41 6e79 5d2c 206e 702e 6e64 6172  ce[Any], np.ndar
+0000adb0: 7261 795b 416e 792c 2041 6e79 5d2c 2054  ray[Any, Any], T
+0000adc0: 7570 6c65 5b41 6e79 2c20 2e2e 2e5d 2c20  uple[Any, ...], 
+0000add0: 7261 6e67 655d 0a20 2020 2020 2020 205d  range].        ]
+0000ade0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+0000adf0: 2069 6e64 6578 5f63 6f6c 3a20 4f70 7469   index_col: Opti
+0000ae00: 6f6e 616c 5b0a 2020 2020 2020 2020 2020  onal[.          
+0000ae10: 2020 556e 696f 6e5b 696e 742c 2073 7472    Union[int, str
+0000ae20: 2c20 5365 7175 656e 6365 5b55 6e69 6f6e  , Sequence[Union
+0000ae30: 5b73 7472 2c20 696e 745d 5d2c 204c 6974  [str, int]], Lit
+0000ae40: 6572 616c 5b46 616c 7365 5d5d 0a20 2020  eral[False]].   
+0000ae50: 2020 2020 205d 203d 204e 6f6e 652c 0a20       ] = None,. 
+0000ae60: 2020 2020 2020 2075 7365 636f 6c73 3a20         usecols: 
+0000ae70: 4f70 7469 6f6e 616c 5b0a 2020 2020 2020  Optional[.      
+0000ae80: 2020 2020 2020 556e 696f 6e5b 0a20 2020        Union[.   
+0000ae90: 2020 2020 2020 2020 2020 2020 204d 7574               Mut
+0000aea0: 6162 6c65 5365 7175 656e 6365 5b73 7472  ableSequence[str
+0000aeb0: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
+0000aec0: 2020 2054 7570 6c65 5b73 7472 2c20 2e2e     Tuple[str, ..
+0000aed0: 2e5d 2c0a 2020 2020 2020 2020 2020 2020  .],.            
+0000aee0: 2020 2020 5365 7175 656e 6365 5b69 6e74      Sequence[int
+0000aef0: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
+0000af00: 2020 2070 616e 6461 732e 5365 7269 6573     pandas.Series
+0000af10: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000af20: 2020 7061 6e64 6173 2e49 6e64 6578 2c0a    pandas.Index,.
+0000af30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000af40: 6e70 2e6e 6461 7272 6179 5b41 6e79 2c20  np.ndarray[Any, 
+0000af50: 416e 795d 2c0a 2020 2020 2020 2020 2020  Any],.          
+0000af60: 2020 2020 2020 4361 6c6c 6162 6c65 5b5b        Callable[[
+0000af70: 416e 795d 2c20 626f 6f6c 5d2c 0a20 2020  Any], bool],.   
+0000af80: 2020 2020 2020 2020 205d 0a20 2020 2020           ].     
+0000af90: 2020 205d 203d 204e 6f6e 652c 0a20 2020     ] = None,.   
+0000afa0: 2020 2020 2064 7479 7065 3a20 4f70 7469       dtype: Opti
+0000afb0: 6f6e 616c 5b44 6963 745d 203d 204e 6f6e  onal[Dict] = Non
+0000afc0: 652c 0a20 2020 2020 2020 2065 6e67 696e  e,.        engin
+0000afd0: 653a 204f 7074 696f 6e61 6c5b 0a20 2020  e: Optional[.   
+0000afe0: 2020 2020 2020 2020 204c 6974 6572 616c           Literal
+0000aff0: 5b22 6322 2c20 2270 7974 686f 6e22 2c20  ["c", "python", 
+0000b000: 2270 7961 7272 6f77 222c 2022 7079 7468  "pyarrow", "pyth
+0000b010: 6f6e 2d66 7766 222c 2022 6269 6771 7565  on-fwf", "bigque
+0000b020: 7279 225d 0a20 2020 2020 2020 205d 203d  ry"].        ] =
+0000b030: 204e 6f6e 652c 0a20 2020 2020 2020 2065   None,.        e
+0000b040: 6e63 6f64 696e 673a 204f 7074 696f 6e61  ncoding: Optiona
+0000b050: 6c5b 7374 725d 203d 204e 6f6e 652c 0a20  l[str] = None,. 
+0000b060: 2020 2020 2020 202a 2a6b 7761 7267 732c         **kwargs,
+0000b070: 0a20 2020 2029 202d 3e20 6461 7461 6672  .    ) -> datafr
+0000b080: 616d 652e 4461 7461 4672 616d 653a 0a20  ame.DataFrame:. 
+0000b090: 2020 2020 2020 2074 6162 6c65 203d 2062         table = b
+0000b0a0: 6967 6672 616d 6573 5f69 6f2e 7261 6e64  igframes_io.rand
+0000b0b0: 6f6d 5f74 6162 6c65 2873 656c 662e 5f61  om_table(self._a
+0000b0c0: 6e6f 6e79 6d6f 7573 5f64 6174 6173 6574  nonymous_dataset
+0000b0d0: 290a 0a20 2020 2020 2020 2069 6620 656e  )..        if en
+0000b0e0: 6769 6e65 2069 7320 6e6f 7420 4e6f 6e65  gine is not None
+0000b0f0: 2061 6e64 2065 6e67 696e 6520 3d3d 2022   and engine == "
+0000b100: 6269 6771 7565 7279 223a 0a20 2020 2020  bigquery":.     
+0000b110: 2020 2020 2020 2069 6620 616e 7928 7061         if any(pa
+0000b120: 7261 6d20 6973 206e 6f74 204e 6f6e 6520  ram is not None 
+0000b130: 666f 7220 7061 7261 6d20 696e 2028 6474  for param in (dt
+0000b140: 7970 652c 206e 616d 6573 2929 3a0a 2020  ype, names)):.  
+0000b150: 2020 2020 2020 2020 2020 2020 2020 6e6f                no
+0000b160: 745f 7375 7070 6f72 7465 6420 3d20 2822  t_supported = ("
+0000b170: 6474 7970 6522 2c20 226e 616d 6573 2229  dtype", "names")
+0000b180: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b190: 2072 6169 7365 204e 6f74 496d 706c 656d   raise NotImplem
+0000b1a0: 656e 7465 6445 7272 6f72 280a 2020 2020  entedError(.    
+0000b1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b1c0: 6622 4269 6751 7565 7279 2065 6e67 696e  f"BigQuery engin
+0000b1d0: 6520 646f 6573 206e 6f74 2073 7570 706f  e does not suppo
+0000b1e0: 7274 2074 6865 7365 2061 7267 756d 656e  rt these argumen
+0000b1f0: 7473 3a20 7b6e 6f74 5f73 7570 706f 7274  ts: {not_support
+0000b200: 6564 7d2e 2022 0a20 2020 2020 2020 2020  ed}. ".         
+0000b210: 2020 2020 2020 2020 2020 2066 227b 636f             f"{co
+0000b220: 6e73 7461 6e74 732e 4645 4544 4241 434b  nstants.FEEDBACK
+0000b230: 5f4c 494e 4b7d 220a 2020 2020 2020 2020  _LINK}".        
+0000b240: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+0000b250: 2020 2020 2020 2069 6620 696e 6465 785f         if index_
+0000b260: 636f 6c20 6973 206e 6f74 204e 6f6e 6520  col is not None 
+0000b270: 616e 6420 280a 2020 2020 2020 2020 2020  and (.          
+0000b280: 2020 2020 2020 6e6f 7420 696e 6465 785f        not index_
+0000b290: 636f 6c20 6f72 206e 6f74 2069 7369 6e73  col or not isins
+0000b2a0: 7461 6e63 6528 696e 6465 785f 636f 6c2c  tance(index_col,
+0000b2b0: 2073 7472 290a 2020 2020 2020 2020 2020   str).          
+0000b2c0: 2020 293a 0a20 2020 2020 2020 2020 2020    ):.           
+0000b2d0: 2020 2020 2072 6169 7365 204e 6f74 496d       raise NotIm
+0000b2e0: 706c 656d 656e 7465 6445 7272 6f72 280a  plementedError(.
+0000b2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b300: 2020 2020 2242 6967 5175 6572 7920 656e      "BigQuery en
+0000b310: 6769 6e65 206f 6e6c 7920 7375 7070 6f72  gine only suppor
+0000b320: 7473 2061 2073 696e 676c 6520 636f 6c75  ts a single colu
+0000b330: 6d6e 206e 616d 6520 666f 7220 6069 6e64  mn name for `ind
+0000b340: 6578 5f63 6f6c 602e 2022 0a20 2020 2020  ex_col`. ".     
+0000b350: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0000b360: 227b 636f 6e73 7461 6e74 732e 4645 4544  "{constants.FEED
+0000b370: 4241 434b 5f4c 494e 4b7d 220a 2020 2020  BACK_LINK}".    
+0000b380: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
+0000b390: 2020 2020 2020 2020 2020 2023 204e 6f6e             # Non
+0000b3a0: 6520 7661 6c75 6520 666f 7220 696e 6465  e value for inde
+0000b3b0: 785f 636f 6c20 6361 6e6e 6f74 2062 6520  x_col cannot be 
+0000b3c0: 7061 7373 6564 2074 6f20 7265 6164 5f67  passed to read_g
+0000b3d0: 6271 0a20 2020 2020 2020 2020 2020 2069  bq.            i
+0000b3e0: 6620 696e 6465 785f 636f 6c20 6973 204e  f index_col is N
+0000b3f0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0000b400: 2020 2020 2069 6e64 6578 5f63 6f6c 203d       index_col =
+0000b410: 2028 290a 0a20 2020 2020 2020 2020 2020   ()..           
+0000b420: 2023 2075 7365 636f 6c73 2073 686f 756c   # usecols shoul
+0000b430: 6420 6f6e 6c79 2062 6520 616e 2069 7465  d only be an ite
+0000b440: 7261 626c 6520 6f66 2073 7472 696e 6773  rable of strings
+0000b450: 2028 636f 6c75 6d6e 206e 616d 6573 2920   (column names) 
+0000b460: 666f 7220 7573 6520 6173 2063 6f6c 756d  for use as colum
+0000b470: 6e73 2069 6e20 7265 6164 5f67 6271 2e0a  ns in read_gbq..
+0000b480: 2020 2020 2020 2020 2020 2020 636f 6c75              colu
+0000b490: 6d6e 733a 2054 7570 6c65 5b41 6e79 2c20  mns: Tuple[Any, 
+0000b4a0: 2e2e 2e5d 203d 2074 7570 6c65 2829 0a20  ...] = tuple(). 
+0000b4b0: 2020 2020 2020 2020 2020 2069 6620 7573             if us
+0000b4c0: 6563 6f6c 7320 6973 206e 6f74 204e 6f6e  ecols is not Non
+0000b4d0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+0000b4e0: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
+0000b4f0: 2875 7365 636f 6c73 2c20 4974 6572 6162  (usecols, Iterab
+0000b500: 6c65 2920 616e 6420 616c 6c28 0a20 2020  le) and all(.   
+0000b510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b520: 2069 7369 6e73 7461 6e63 6528 636f 6c2c   isinstance(col,
+0000b530: 2073 7472 2920 666f 7220 636f 6c20 696e   str) for col in
+0000b540: 2075 7365 636f 6c73 0a20 2020 2020 2020   usecols.       
+0000b550: 2020 2020 2020 2020 2029 3a0a 2020 2020           ):.    
+0000b560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b570: 636f 6c75 6d6e 7320 3d20 7475 706c 6528  columns = tuple(
+0000b580: 636f 6c20 666f 7220 636f 6c20 696e 2075  col for col in u
+0000b590: 7365 636f 6c73 290a 2020 2020 2020 2020  secols).        
+0000b5a0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
 0000b5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b5c0: 6622 4269 6751 7565 7279 2065 6e67 696e  f"BigQuery engin
-0000b5d0: 6520 6f6e 6c79 2073 7570 706f 7274 7320  e only supports 
-0000b5e0: 7468 6520 666f 6c6c 6f77 696e 6720 656e  the following en
-0000b5f0: 636f 6469 6e67 733a 207b 5f56 414c 4944  codings: {_VALID
-0000b600: 5f45 4e43 4f44 494e 4753 7d2e 2022 0a20  _ENCODINGS}. ". 
-0000b610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b620: 2020 2066 227b 636f 6e73 7461 6e74 732e     f"{constants.
-0000b630: 4645 4544 4241 434b 5f4c 494e 4b7d 220a  FEEDBACK_LINK}".
+0000b5c0: 2020 7261 6973 6520 4e6f 7449 6d70 6c65    raise NotImple
+0000b5d0: 6d65 6e74 6564 4572 726f 7228 0a20 2020  mentedError(.   
+0000b5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b5f0: 2020 2020 2022 4269 6751 7565 7279 2065       "BigQuery e
+0000b600: 6e67 696e 6520 6f6e 6c79 2073 7570 706f  ngine only suppo
+0000b610: 7274 7320 616e 2069 7465 7261 626c 6520  rts an iterable 
+0000b620: 6f66 2073 7472 696e 6773 2066 6f72 2060  of strings for `
+0000b630: 7573 6563 6f6c 7360 2e20 220a 2020 2020  usecols`. ".    
 0000b640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b650: 290a 0a20 2020 2020 2020 2020 2020 206a  )..            j
-0000b660: 6f62 5f63 6f6e 6669 6720 3d20 7365 6c66  ob_config = self
-0000b670: 2e5f 7072 6570 6172 655f 6c6f 6164 5f6a  ._prepare_load_j
-0000b680: 6f62 5f63 6f6e 6669 6728 290a 2020 2020  ob_config().    
-0000b690: 2020 2020 2020 2020 6a6f 625f 636f 6e66          job_conf
-0000b6a0: 6967 2e63 7265 6174 655f 6469 7370 6f73  ig.create_dispos
-0000b6b0: 6974 696f 6e20 3d20 6269 6771 7565 7279  ition = bigquery
-0000b6c0: 2e43 7265 6174 6544 6973 706f 7369 7469  .CreateDispositi
-0000b6d0: 6f6e 2e43 5245 4154 455f 4946 5f4e 4545  on.CREATE_IF_NEE
-0000b6e0: 4445 440a 2020 2020 2020 2020 2020 2020  DED.            
-0000b6f0: 6a6f 625f 636f 6e66 6967 2e73 6f75 7263  job_config.sourc
-0000b700: 655f 666f 726d 6174 203d 2062 6967 7175  e_format = bigqu
-0000b710: 6572 792e 536f 7572 6365 466f 726d 6174  ery.SourceFormat
-0000b720: 2e43 5356 0a20 2020 2020 2020 2020 2020  .CSV.           
-0000b730: 206a 6f62 5f63 6f6e 6669 672e 7772 6974   job_config.writ
-0000b740: 655f 6469 7370 6f73 6974 696f 6e20 3d20  e_disposition = 
-0000b750: 6269 6771 7565 7279 2e57 7269 7465 4469  bigquery.WriteDi
-0000b760: 7370 6f73 6974 696f 6e2e 5752 4954 455f  sposition.WRITE_
-0000b770: 454d 5054 590a 2020 2020 2020 2020 2020  EMPTY.          
-0000b780: 2020 6a6f 625f 636f 6e66 6967 2e61 7574    job_config.aut
-0000b790: 6f64 6574 6563 7420 3d20 5472 7565 0a20  odetect = True. 
-0000b7a0: 2020 2020 2020 2020 2020 206a 6f62 5f63             job_c
-0000b7b0: 6f6e 6669 672e 6669 656c 645f 6465 6c69  onfig.field_deli
-0000b7c0: 6d69 7465 7220 3d20 7365 700a 2020 2020  miter = sep.    
-0000b7d0: 2020 2020 2020 2020 6a6f 625f 636f 6e66          job_conf
-0000b7e0: 6967 2e65 6e63 6f64 696e 6720 3d20 656e  ig.encoding = en
-0000b7f0: 636f 6469 6e67 0a20 2020 2020 2020 2020  coding.         
-0000b800: 2020 206a 6f62 5f63 6f6e 6669 672e 6c61     job_config.la
-0000b810: 6265 6c73 203d 207b 2262 6967 6672 616d  bels = {"bigfram
-0000b820: 6573 2d61 7069 223a 2022 7265 6164 5f63  es-api": "read_c
-0000b830: 7376 227d 0a0a 2020 2020 2020 2020 2020  sv"}..          
-0000b840: 2020 2320 5765 2077 616e 7420 746f 206d    # We want to m
-0000b850: 6174 6368 2070 616e 6461 7320 6265 6861  atch pandas beha
-0000b860: 7669 6f72 2e20 4966 2068 6561 6465 7220  vior. If header 
-0000b870: 6973 2030 2c20 6e6f 2072 6f77 7320 7368  is 0, no rows sh
-0000b880: 6f75 6c64 2062 6520 736b 6970 7065 642c  ould be skipped,
-0000b890: 2073 6f20 7765 0a20 2020 2020 2020 2020   so we.         
-0000b8a0: 2020 2023 2064 6f20 6e6f 7420 6e65 6564     # do not need
-0000b8b0: 2074 6f20 7365 7420 6073 6b69 705f 6c65   to set `skip_le
-0000b8c0: 6164 696e 675f 726f 7773 602e 2049 6620  ading_rows`. If 
-0000b8d0: 6865 6164 6572 2069 7320 4e6f 6e65 2c20  header is None, 
-0000b8e0: 7468 656e 2074 6865 7265 2069 7320 6e6f  then there is no
-0000b8f0: 2068 6561 6465 722e 0a20 2020 2020 2020   header..       
-0000b900: 2020 2020 2023 2053 6574 7469 6e67 2073       # Setting s
-0000b910: 6b69 705f 6c65 6164 696e 675f 726f 7773  kip_leading_rows
-0000b920: 2074 6f20 3020 646f 6573 2074 6861 742e   to 0 does that.
-0000b930: 2049 6620 6865 6164 6572 3d4e 2061 6e64   If header=N and
-0000b940: 204e 3e30 2c20 7765 2077 616e 7420 746f   N>0, we want to
-0000b950: 2073 6b69 7020 4e20 726f 7773 2e0a 2020   skip N rows..  
-0000b960: 2020 2020 2020 2020 2020 6966 2068 6561            if hea
-0000b970: 6465 7220 6973 204e 6f6e 653a 0a20 2020  der is None:.   
-0000b980: 2020 2020 2020 2020 2020 2020 206a 6f62               job
-0000b990: 5f63 6f6e 6669 672e 736b 6970 5f6c 6561  _config.skip_lea
-0000b9a0: 6469 6e67 5f72 6f77 7320 3d20 300a 2020  ding_rows = 0.  
-0000b9b0: 2020 2020 2020 2020 2020 656c 6966 2068            elif h
-0000b9c0: 6561 6465 7220 3e20 303a 0a20 2020 2020  eader > 0:.     
-0000b9d0: 2020 2020 2020 2020 2020 206a 6f62 5f63             job_c
-0000b9e0: 6f6e 6669 672e 736b 6970 5f6c 6561 6469  onfig.skip_leadi
-0000b9f0: 6e67 5f72 6f77 7320 3d20 6865 6164 6572  ng_rows = header
-0000ba00: 0a0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-0000ba10: 7475 726e 2073 656c 662e 5f72 6561 645f  turn self._read_
-0000ba20: 6269 6771 7565 7279 5f6c 6f61 645f 6a6f  bigquery_load_jo
-0000ba30: 6228 0a20 2020 2020 2020 2020 2020 2020  b(.             
-0000ba40: 2020 2066 696c 6570 6174 685f 6f72 5f62     filepath_or_b
-0000ba50: 7566 6665 722c 0a20 2020 2020 2020 2020  uffer,.         
-0000ba60: 2020 2020 2020 2074 6162 6c65 2c0a 2020         table,.  
-0000ba70: 2020 2020 2020 2020 2020 2020 2020 6a6f                jo
-0000ba80: 625f 636f 6e66 6967 3d6a 6f62 5f63 6f6e  b_config=job_con
-0000ba90: 6669 672c 0a20 2020 2020 2020 2020 2020  fig,.           
-0000baa0: 2020 2020 2069 6e64 6578 5f63 6f6c 3d69       index_col=i
-0000bab0: 6e64 6578 5f63 6f6c 2c0a 2020 2020 2020  ndex_col,.      
-0000bac0: 2020 2020 2020 2020 2020 636f 6c75 6d6e            column
-0000bad0: 733d 636f 6c75 6d6e 732c 0a20 2020 2020  s=columns,.     
-0000bae0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0000baf0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-0000bb00: 2020 2069 6620 616e 7928 6172 6720 696e     if any(arg in
-0000bb10: 206b 7761 7267 7320 666f 7220 6172 6720   kwargs for arg 
-0000bb20: 696e 2028 2263 6875 6e6b 7369 7a65 222c  in ("chunksize",
-0000bb30: 2022 6974 6572 6174 6f72 2229 293a 0a20   "iterator")):. 
-0000bb40: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0000bb50: 6169 7365 204e 6f74 496d 706c 656d 656e  aise NotImplemen
-0000bb60: 7465 6445 7272 6f72 280a 2020 2020 2020  tedError(.      
-0000bb70: 2020 2020 2020 2020 2020 2020 2020 2227                "'
-0000bb80: 6368 756e 6b73 697a 6527 2061 6e64 2027  chunksize' and '
-0000bb90: 6974 6572 6174 6f72 2720 6172 6775 6d65  iterator' argume
-0000bba0: 6e74 7320 6172 6520 6e6f 7420 7375 7070  nts are not supp
-0000bbb0: 6f72 7465 642e 2022 0a20 2020 2020 2020  orted. ".       
-0000bbc0: 2020 2020 2020 2020 2020 2020 2066 227b               f"{
-0000bbd0: 636f 6e73 7461 6e74 732e 4645 4544 4241  constants.FEEDBA
-0000bbe0: 434b 5f4c 494e 4b7d 220a 2020 2020 2020  CK_LINK}".      
-0000bbf0: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
-0000bc00: 2020 2020 2020 2020 2069 6620 6973 696e           if isin
-0000bc10: 7374 616e 6365 2866 696c 6570 6174 685f  stance(filepath_
-0000bc20: 6f72 5f62 7566 6665 722c 2073 7472 293a  or_buffer, str):
-0000bc30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000bc40: 2073 656c 662e 5f63 6865 636b 5f66 696c   self._check_fil
-0000bc50: 655f 7369 7a65 2866 696c 6570 6174 685f  e_size(filepath_
-0000bc60: 6f72 5f62 7566 6665 7229 0a20 2020 2020  or_buffer).     
-0000bc70: 2020 2020 2020 2070 616e 6461 735f 6466         pandas_df
-0000bc80: 203d 2070 616e 6461 732e 7265 6164 5f63   = pandas.read_c
-0000bc90: 7376 280a 2020 2020 2020 2020 2020 2020  sv(.            
-0000bca0: 2020 2020 6669 6c65 7061 7468 5f6f 725f      filepath_or_
-0000bcb0: 6275 6666 6572 2c0a 2020 2020 2020 2020  buffer,.        
-0000bcc0: 2020 2020 2020 2020 7365 703d 7365 702c          sep=sep,
-0000bcd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000bce0: 2068 6561 6465 723d 6865 6164 6572 2c0a   header=header,.
-0000bcf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bd00: 6e61 6d65 733d 6e61 6d65 732c 0a20 2020  names=names,.   
-0000bd10: 2020 2020 2020 2020 2020 2020 2069 6e64               ind
-0000bd20: 6578 5f63 6f6c 3d69 6e64 6578 5f63 6f6c  ex_col=index_col
-0000bd30: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000bd40: 2020 7573 6563 6f6c 733d 7573 6563 6f6c    usecols=usecol
-0000bd50: 732c 2020 2320 7479 7065 3a20 6967 6e6f  s,  # type: igno
-0000bd60: 7265 0a20 2020 2020 2020 2020 2020 2020  re.             
-0000bd70: 2020 2064 7479 7065 3d64 7479 7065 2c0a     dtype=dtype,.
-0000bd80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bd90: 656e 6769 6e65 3d65 6e67 696e 652c 0a20  engine=engine,. 
-0000bda0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-0000bdb0: 6e63 6f64 696e 673d 656e 636f 6469 6e67  ncoding=encoding
-0000bdc0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000bdd0: 2020 2a2a 6b77 6172 6773 2c0a 2020 2020    **kwargs,.    
-0000bde0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-0000bdf0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-0000be00: 662e 5f72 6561 645f 7061 6e64 6173 2870  f._read_pandas(p
-0000be10: 616e 6461 735f 6466 2c20 2272 6561 645f  andas_df, "read_
-0000be20: 6373 7622 2920 2023 2074 7970 653a 2069  csv")  # type: i
-0000be30: 676e 6f72 650a 0a20 2020 2064 6566 2072  gnore..    def r
-0000be40: 6561 645f 7069 636b 6c65 280a 2020 2020  ead_pickle(.    
-0000be50: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
-0000be60: 2020 6669 6c65 7061 7468 5f6f 725f 6275    filepath_or_bu
-0000be70: 6666 6572 3a20 4669 6c65 5061 7468 207c  ffer: FilePath |
-0000be80: 2052 6561 6450 6963 6b6c 6542 7566 6665   ReadPickleBuffe
-0000be90: 722c 0a20 2020 2020 2020 2063 6f6d 7072  r,.        compr
-0000bea0: 6573 7369 6f6e 3a20 436f 6d70 7265 7373  ession: Compress
-0000beb0: 696f 6e4f 7074 696f 6e73 203d 2022 696e  ionOptions = "in
-0000bec0: 6665 7222 2c0a 2020 2020 2020 2020 7374  fer",.        st
-0000bed0: 6f72 6167 655f 6f70 7469 6f6e 733a 2053  orage_options: S
-0000bee0: 746f 7261 6765 4f70 7469 6f6e 7320 3d20  torageOptions = 
-0000bef0: 4e6f 6e65 2c0a 2020 2020 293a 0a20 2020  None,.    ):.   
-0000bf00: 2020 2020 2070 616e 6461 735f 6f62 6a20       pandas_obj 
-0000bf10: 3d20 7061 6e64 6173 2e72 6561 645f 7069  = pandas.read_pi
-0000bf20: 636b 6c65 280a 2020 2020 2020 2020 2020  ckle(.          
-0000bf30: 2020 6669 6c65 7061 7468 5f6f 725f 6275    filepath_or_bu
-0000bf40: 6666 6572 2c0a 2020 2020 2020 2020 2020  ffer,.          
-0000bf50: 2020 636f 6d70 7265 7373 696f 6e3d 636f    compression=co
-0000bf60: 6d70 7265 7373 696f 6e2c 0a20 2020 2020  mpression,.     
-0000bf70: 2020 2020 2020 2073 746f 7261 6765 5f6f         storage_o
-0000bf80: 7074 696f 6e73 3d73 746f 7261 6765 5f6f  ptions=storage_o
-0000bf90: 7074 696f 6e73 2c0a 2020 2020 2020 2020  ptions,.        
-0000bfa0: 290a 0a20 2020 2020 2020 2069 6620 6973  )..        if is
-0000bfb0: 696e 7374 616e 6365 2870 616e 6461 735f  instance(pandas_
-0000bfc0: 6f62 6a2c 2070 616e 6461 732e 5365 7269  obj, pandas.Seri
-0000bfd0: 6573 293a 0a20 2020 2020 2020 2020 2020  es):.           
-0000bfe0: 2069 6620 7061 6e64 6173 5f6f 626a 2e6e   if pandas_obj.n
-0000bff0: 616d 6520 6973 204e 6f6e 653a 0a20 2020  ame is None:.   
-0000c000: 2020 2020 2020 2020 2020 2020 2070 616e               pan
-0000c010: 6461 735f 6f62 6a2e 6e61 6d65 203d 2022  das_obj.name = "
-0000c020: 3022 0a20 2020 2020 2020 2020 2020 2062  0".            b
-0000c030: 6967 6672 616d 6573 5f64 6620 3d20 7365  igframes_df = se
-0000c040: 6c66 2e5f 7265 6164 5f70 616e 6461 7328  lf._read_pandas(
-0000c050: 7061 6e64 6173 5f6f 626a 2e74 6f5f 6672  pandas_obj.to_fr
-0000c060: 616d 6528 292c 2022 7265 6164 5f70 6963  ame(), "read_pic
-0000c070: 6b6c 6522 290a 2020 2020 2020 2020 2020  kle").          
-0000c080: 2020 7265 7475 726e 2062 6967 6672 616d    return bigfram
-0000c090: 6573 5f64 665b 6269 6766 7261 6d65 735f  es_df[bigframes_
-0000c0a0: 6466 2e63 6f6c 756d 6e73 5b30 5d5d 0a20  df.columns[0]]. 
-0000c0b0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-0000c0c0: 6c66 2e5f 7265 6164 5f70 616e 6461 7328  lf._read_pandas(
-0000c0d0: 7061 6e64 6173 5f6f 626a 2c20 2272 6561  pandas_obj, "rea
-0000c0e0: 645f 7069 636b 6c65 2229 0a0a 2020 2020  d_pickle")..    
-0000c0f0: 6465 6620 7265 6164 5f70 6172 7175 6574  def read_parquet
-0000c100: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
-0000c110: 2020 2020 2020 2020 7061 7468 3a20 7374          path: st
-0000c120: 7220 7c20 494f 5b22 6279 7465 7322 5d2c  r | IO["bytes"],
-0000c130: 0a20 2020 2020 2020 202a 2c0a 2020 2020  .        *,.    
-0000c140: 2020 2020 656e 6769 6e65 3a20 7374 7220      engine: str 
-0000c150: 3d20 2261 7574 6f22 2c0a 2020 2020 2920  = "auto",.    ) 
-0000c160: 2d3e 2064 6174 6166 7261 6d65 2e44 6174  -> dataframe.Dat
-0000c170: 6146 7261 6d65 3a0a 2020 2020 2020 2020  aFrame:.        
-0000c180: 7461 626c 6520 3d20 6269 6766 7261 6d65  table = bigframe
-0000c190: 735f 696f 2e72 616e 646f 6d5f 7461 626c  s_io.random_tabl
-0000c1a0: 6528 7365 6c66 2e5f 616e 6f6e 796d 6f75  e(self._anonymou
-0000c1b0: 735f 6461 7461 7365 7429 0a0a 2020 2020  s_dataset)..    
-0000c1c0: 2020 2020 6966 2065 6e67 696e 6520 3d3d      if engine ==
-0000c1d0: 2022 6269 6771 7565 7279 223a 0a20 2020   "bigquery":.   
-0000c1e0: 2020 2020 2020 2020 206a 6f62 5f63 6f6e           job_con
-0000c1f0: 6669 6720 3d20 7365 6c66 2e5f 7072 6570  fig = self._prep
-0000c200: 6172 655f 6c6f 6164 5f6a 6f62 5f63 6f6e  are_load_job_con
-0000c210: 6669 6728 290a 2020 2020 2020 2020 2020  fig().          
-0000c220: 2020 6a6f 625f 636f 6e66 6967 2e63 7265    job_config.cre
-0000c230: 6174 655f 6469 7370 6f73 6974 696f 6e20  ate_disposition 
-0000c240: 3d20 6269 6771 7565 7279 2e43 7265 6174  = bigquery.Creat
-0000c250: 6544 6973 706f 7369 7469 6f6e 2e43 5245  eDisposition.CRE
-0000c260: 4154 455f 4946 5f4e 4545 4445 440a 2020  ATE_IF_NEEDED.  
-0000c270: 2020 2020 2020 2020 2020 6a6f 625f 636f            job_co
-0000c280: 6e66 6967 2e73 6f75 7263 655f 666f 726d  nfig.source_form
-0000c290: 6174 203d 2062 6967 7175 6572 792e 536f  at = bigquery.So
-0000c2a0: 7572 6365 466f 726d 6174 2e50 4152 5155  urceFormat.PARQU
-0000c2b0: 4554 0a20 2020 2020 2020 2020 2020 206a  ET.            j
-0000c2c0: 6f62 5f63 6f6e 6669 672e 7772 6974 655f  ob_config.write_
-0000c2d0: 6469 7370 6f73 6974 696f 6e20 3d20 6269  disposition = bi
-0000c2e0: 6771 7565 7279 2e57 7269 7465 4469 7370  gquery.WriteDisp
-0000c2f0: 6f73 6974 696f 6e2e 5752 4954 455f 454d  osition.WRITE_EM
-0000c300: 5054 590a 2020 2020 2020 2020 2020 2020  PTY.            
-0000c310: 6a6f 625f 636f 6e66 6967 2e6c 6162 656c  job_config.label
-0000c320: 7320 3d20 7b22 6269 6766 7261 6d65 732d  s = {"bigframes-
-0000c330: 6170 6922 3a20 2272 6561 645f 7061 7271  api": "read_parq
-0000c340: 7565 7422 7d0a 0a20 2020 2020 2020 2020  uet"}..         
-0000c350: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
-0000c360: 7265 6164 5f62 6967 7175 6572 795f 6c6f  read_bigquery_lo
-0000c370: 6164 5f6a 6f62 2870 6174 682c 2074 6162  ad_job(path, tab
-0000c380: 6c65 2c20 6a6f 625f 636f 6e66 6967 3d6a  le, job_config=j
-0000c390: 6f62 5f63 6f6e 6669 6729 0a20 2020 2020  ob_config).     
-0000c3a0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-0000c3b0: 2020 2020 2072 6561 645f 7061 7271 7565       read_parque
-0000c3c0: 745f 6b77 6172 6773 3a20 4469 6374 5b73  t_kwargs: Dict[s
-0000c3d0: 7472 2c20 416e 795d 203d 207b 7d0a 2020  tr, Any] = {}.  
-0000c3e0: 2020 2020 2020 2020 2020 6966 2070 616e            if pan
-0000c3f0: 6461 732e 5f5f 7665 7273 696f 6e5f 5f2e  das.__version__.
-0000c400: 7374 6172 7473 7769 7468 2822 312e 2229  startswith("1.")
-0000c410: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000c420: 2020 7265 6164 5f70 6172 7175 6574 5f6b    read_parquet_k
-0000c430: 7761 7267 735b 2275 7365 5f6e 756c 6c61  wargs["use_nulla
-0000c440: 626c 655f 6474 7970 6573 225d 203d 2054  ble_dtypes"] = T
-0000c450: 7275 650a 2020 2020 2020 2020 2020 2020  rue.            
-0000c460: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-0000c470: 2020 2020 2020 7265 6164 5f70 6172 7175        read_parqu
-0000c480: 6574 5f6b 7761 7267 735b 2264 7479 7065  et_kwargs["dtype
-0000c490: 5f62 6163 6b65 6e64 225d 203d 2022 7079  _backend"] = "py
-0000c4a0: 6172 726f 7722 0a0a 2020 2020 2020 2020  arrow"..        
-0000c4b0: 2020 2020 7061 6e64 6173 5f6f 626a 203d      pandas_obj =
-0000c4c0: 2070 616e 6461 732e 7265 6164 5f70 6172   pandas.read_par
-0000c4d0: 7175 6574 280a 2020 2020 2020 2020 2020  quet(.          
-0000c4e0: 2020 2020 2020 7061 7468 2c0a 2020 2020        path,.    
-0000c4f0: 2020 2020 2020 2020 2020 2020 656e 6769              engi
-0000c500: 6e65 3d65 6e67 696e 652c 2020 2320 7479  ne=engine,  # ty
-0000c510: 7065 3a20 6967 6e6f 7265 0a20 2020 2020  pe: ignore.     
-0000c520: 2020 2020 2020 2020 2020 202a 2a72 6561             **rea
-0000c530: 645f 7061 7271 7565 745f 6b77 6172 6773  d_parquet_kwargs
-0000c540: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
-0000c550: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000c560: 726e 2073 656c 662e 5f72 6561 645f 7061  rn self._read_pa
-0000c570: 6e64 6173 2870 616e 6461 735f 6f62 6a2c  ndas(pandas_obj,
-0000c580: 2022 7265 6164 5f70 6172 7175 6574 2229   "read_parquet")
-0000c590: 0a0a 2020 2020 6465 6620 7265 6164 5f6a  ..    def read_j
-0000c5a0: 736f 6e28 0a20 2020 2020 2020 2073 656c  son(.        sel
-0000c5b0: 662c 0a20 2020 2020 2020 2070 6174 685f  f,.        path_
-0000c5c0: 6f72 5f62 7566 3a20 7374 7220 7c20 494f  or_buf: str | IO
-0000c5d0: 5b22 6279 7465 7322 5d2c 0a20 2020 2020  ["bytes"],.     
-0000c5e0: 2020 202a 2c0a 2020 2020 2020 2020 6f72     *,.        or
-0000c5f0: 6965 6e74 3a20 4c69 7465 7261 6c5b 0a20  ient: Literal[. 
-0000c600: 2020 2020 2020 2020 2020 2022 7370 6c69             "spli
-0000c610: 7422 2c20 2272 6563 6f72 6473 222c 2022  t", "records", "
-0000c620: 696e 6465 7822 2c20 2263 6f6c 756d 6e73  index", "columns
-0000c630: 222c 2022 7661 6c75 6573 222c 2022 7461  ", "values", "ta
-0000c640: 626c 6522 0a20 2020 2020 2020 205d 203d  ble".        ] =
-0000c650: 2022 636f 6c75 6d6e 7322 2c0a 2020 2020   "columns",.    
-0000c660: 2020 2020 6474 7970 653a 204f 7074 696f      dtype: Optio
-0000c670: 6e61 6c5b 4469 6374 5d20 3d20 4e6f 6e65  nal[Dict] = None
-0000c680: 2c0a 2020 2020 2020 2020 656e 636f 6469  ,.        encodi
-0000c690: 6e67 3a20 4f70 7469 6f6e 616c 5b73 7472  ng: Optional[str
-0000c6a0: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
-0000c6b0: 2020 6c69 6e65 733a 2062 6f6f 6c20 3d20    lines: bool = 
-0000c6c0: 4661 6c73 652c 0a20 2020 2020 2020 2065  False,.        e
-0000c6d0: 6e67 696e 653a 204c 6974 6572 616c 5b22  ngine: Literal["
-0000c6e0: 756a 736f 6e22 2c20 2270 7961 7272 6f77  ujson", "pyarrow
-0000c6f0: 222c 2022 6269 6771 7565 7279 225d 203d  ", "bigquery"] =
-0000c700: 2022 756a 736f 6e22 2c0a 2020 2020 2020   "ujson",.      
-0000c710: 2020 2a2a 6b77 6172 6773 2c0a 2020 2020    **kwargs,.    
-0000c720: 2920 2d3e 2064 6174 6166 7261 6d65 2e44  ) -> dataframe.D
-0000c730: 6174 6146 7261 6d65 3a0a 2020 2020 2020  ataFrame:.      
-0000c740: 2020 7461 626c 6520 3d20 6269 6766 7261    table = bigfra
-0000c750: 6d65 735f 696f 2e72 616e 646f 6d5f 7461  mes_io.random_ta
-0000c760: 626c 6528 7365 6c66 2e5f 616e 6f6e 796d  ble(self._anonym
-0000c770: 6f75 735f 6461 7461 7365 7429 0a0a 2020  ous_dataset)..  
-0000c780: 2020 2020 2020 6966 2065 6e67 696e 6520        if engine 
-0000c790: 3d3d 2022 6269 6771 7565 7279 223a 0a0a  == "bigquery":..
-0000c7a0: 2020 2020 2020 2020 2020 2020 6966 2064              if d
-0000c7b0: 7479 7065 2069 7320 6e6f 7420 4e6f 6e65  type is not None
-0000c7c0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000c7d0: 2020 7261 6973 6520 4e6f 7449 6d70 6c65    raise NotImple
-0000c7e0: 6d65 6e74 6564 4572 726f 7228 0a20 2020  mentedError(.   
-0000c7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c800: 2022 4269 6751 7565 7279 2065 6e67 696e   "BigQuery engin
-0000c810: 6520 646f 6573 206e 6f74 2073 7570 706f  e does not suppo
-0000c820: 7274 2074 6865 2064 7479 7065 2061 7267  rt the dtype arg
-0000c830: 756d 656e 7473 2e22 0a20 2020 2020 2020  uments.".       
-0000c840: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
-0000c850: 2020 2020 2020 2020 6966 206e 6f74 206c          if not l
-0000c860: 696e 6573 3a0a 2020 2020 2020 2020 2020  ines:.          
-0000c870: 2020 2020 2020 7261 6973 6520 4e6f 7449        raise NotI
-0000c880: 6d70 6c65 6d65 6e74 6564 4572 726f 7228  mplementedError(
-0000c890: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c8a0: 2020 2020 2022 4f6e 6c79 206e 6577 6c69       "Only newli
-0000c8b0: 6e65 2064 656c 696d 6974 6564 204a 534f  ne delimited JSO
-0000c8c0: 4e20 666f 726d 6174 2069 7320 7375 7070  N format is supp
-0000c8d0: 6f72 7465 642e 220a 2020 2020 2020 2020  orted.".        
-0000c8e0: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
-0000c8f0: 2020 2020 2020 2069 6620 656e 636f 6469         if encodi
-0000c900: 6e67 2069 7320 6e6f 7420 4e6f 6e65 2061  ng is not None a
-0000c910: 6e64 2065 6e63 6f64 696e 6720 6e6f 7420  nd encoding not 
-0000c920: 696e 205f 5641 4c49 445f 454e 434f 4449  in _VALID_ENCODI
-0000c930: 4e47 533a 0a20 2020 2020 2020 2020 2020  NGS:.           
-0000c940: 2020 2020 2072 6169 7365 204e 6f74 496d       raise NotIm
-0000c950: 706c 656d 656e 7465 6445 7272 6f72 280a  plementedError(.
-0000c960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c970: 2020 2020 6622 4269 6751 7565 7279 2065      f"BigQuery e
-0000c980: 6e67 696e 6520 6f6e 6c79 2073 7570 706f  ngine only suppo
-0000c990: 7274 7320 7468 6520 666f 6c6c 6f77 696e  rts the followin
-0000c9a0: 6720 656e 636f 6469 6e67 733a 207b 5f56  g encodings: {_V
-0000c9b0: 414c 4944 5f45 4e43 4f44 494e 4753 7d22  ALID_ENCODINGS}"
-0000c9c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c9d0: 2029 0a0a 2020 2020 2020 2020 2020 2020   )..            
-0000c9e0: 6966 206c 696e 6573 2061 6e64 206f 7269  if lines and ori
-0000c9f0: 656e 7420 213d 2022 7265 636f 7264 7322  ent != "records"
-0000ca00: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000ca10: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
-0000ca20: 6f72 280a 2020 2020 2020 2020 2020 2020  or(.            
-0000ca30: 2020 2020 2020 2020 2227 6c69 6e65 7327          "'lines'
-0000ca40: 206b 6579 776f 7264 2069 7320 6f6e 6c79   keyword is only
-0000ca50: 2076 616c 6964 2077 6865 6e20 276f 7269   valid when 'ori
-0000ca60: 656e 7427 2069 7320 2772 6563 6f72 6473  ent' is 'records
-0000ca70: 272e 220a 2020 2020 2020 2020 2020 2020  '.".            
-0000ca80: 2020 2020 290a 0a20 2020 2020 2020 2020      )..         
-0000ca90: 2020 206a 6f62 5f63 6f6e 6669 6720 3d20     job_config = 
-0000caa0: 7365 6c66 2e5f 7072 6570 6172 655f 6c6f  self._prepare_lo
-0000cab0: 6164 5f6a 6f62 5f63 6f6e 6669 6728 290a  ad_job_config().
-0000cac0: 2020 2020 2020 2020 2020 2020 6a6f 625f              job_
-0000cad0: 636f 6e66 6967 2e63 7265 6174 655f 6469  config.create_di
-0000cae0: 7370 6f73 6974 696f 6e20 3d20 6269 6771  sposition = bigq
-0000caf0: 7565 7279 2e43 7265 6174 6544 6973 706f  uery.CreateDispo
-0000cb00: 7369 7469 6f6e 2e43 5245 4154 455f 4946  sition.CREATE_IF
-0000cb10: 5f4e 4545 4445 440a 2020 2020 2020 2020  _NEEDED.        
-0000cb20: 2020 2020 6a6f 625f 636f 6e66 6967 2e73      job_config.s
-0000cb30: 6f75 7263 655f 666f 726d 6174 203d 2062  ource_format = b
-0000cb40: 6967 7175 6572 792e 536f 7572 6365 466f  igquery.SourceFo
-0000cb50: 726d 6174 2e4e 4557 4c49 4e45 5f44 454c  rmat.NEWLINE_DEL
-0000cb60: 494d 4954 4544 5f4a 534f 4e0a 2020 2020  IMITED_JSON.    
-0000cb70: 2020 2020 2020 2020 6a6f 625f 636f 6e66          job_conf
-0000cb80: 6967 2e77 7269 7465 5f64 6973 706f 7369  ig.write_disposi
-0000cb90: 7469 6f6e 203d 2062 6967 7175 6572 792e  tion = bigquery.
-0000cba0: 5772 6974 6544 6973 706f 7369 7469 6f6e  WriteDisposition
-0000cbb0: 2e57 5249 5445 5f45 4d50 5459 0a20 2020  .WRITE_EMPTY.   
-0000cbc0: 2020 2020 2020 2020 206a 6f62 5f63 6f6e           job_con
-0000cbd0: 6669 672e 6175 746f 6465 7465 6374 203d  fig.autodetect =
-0000cbe0: 2054 7275 650a 2020 2020 2020 2020 2020   True.          
-0000cbf0: 2020 6a6f 625f 636f 6e66 6967 2e65 6e63    job_config.enc
-0000cc00: 6f64 696e 6720 3d20 656e 636f 6469 6e67  oding = encoding
+0000b650: 2020 2020 6622 7b63 6f6e 7374 616e 7473      f"{constants
+0000b660: 2e46 4545 4442 4143 4b5f 4c49 4e4b 7d22  .FEEDBACK_LINK}"
+0000b670: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b680: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+0000b690: 2020 2020 6966 2065 6e63 6f64 696e 6720      if encoding 
+0000b6a0: 6973 206e 6f74 204e 6f6e 6520 616e 6420  is not None and 
+0000b6b0: 656e 636f 6469 6e67 206e 6f74 2069 6e20  encoding not in 
+0000b6c0: 5f56 414c 4944 5f45 4e43 4f44 494e 4753  _VALID_ENCODINGS
+0000b6d0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000b6e0: 2020 7261 6973 6520 4e6f 7449 6d70 6c65    raise NotImple
+0000b6f0: 6d65 6e74 6564 4572 726f 7228 0a20 2020  mentedError(.   
+0000b700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b710: 2066 2242 6967 5175 6572 7920 656e 6769   f"BigQuery engi
+0000b720: 6e65 206f 6e6c 7920 7375 7070 6f72 7473  ne only supports
+0000b730: 2074 6865 2066 6f6c 6c6f 7769 6e67 2065   the following e
+0000b740: 6e63 6f64 696e 6773 3a20 7b5f 5641 4c49  ncodings: {_VALI
+0000b750: 445f 454e 434f 4449 4e47 537d 2e20 220a  D_ENCODINGS}. ".
+0000b760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b770: 2020 2020 6622 7b63 6f6e 7374 616e 7473      f"{constants
+0000b780: 2e46 4545 4442 4143 4b5f 4c49 4e4b 7d22  .FEEDBACK_LINK}"
+0000b790: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b7a0: 2029 0a0a 2020 2020 2020 2020 2020 2020   )..            
+0000b7b0: 6a6f 625f 636f 6e66 6967 203d 2073 656c  job_config = sel
+0000b7c0: 662e 5f70 7265 7061 7265 5f6c 6f61 645f  f._prepare_load_
+0000b7d0: 6a6f 625f 636f 6e66 6967 2829 0a20 2020  job_config().   
+0000b7e0: 2020 2020 2020 2020 206a 6f62 5f63 6f6e           job_con
+0000b7f0: 6669 672e 6372 6561 7465 5f64 6973 706f  fig.create_dispo
+0000b800: 7369 7469 6f6e 203d 2062 6967 7175 6572  sition = bigquer
+0000b810: 792e 4372 6561 7465 4469 7370 6f73 6974  y.CreateDisposit
+0000b820: 696f 6e2e 4352 4541 5445 5f49 465f 4e45  ion.CREATE_IF_NE
+0000b830: 4544 4544 0a20 2020 2020 2020 2020 2020  EDED.           
+0000b840: 206a 6f62 5f63 6f6e 6669 672e 736f 7572   job_config.sour
+0000b850: 6365 5f66 6f72 6d61 7420 3d20 6269 6771  ce_format = bigq
+0000b860: 7565 7279 2e53 6f75 7263 6546 6f72 6d61  uery.SourceForma
+0000b870: 742e 4353 560a 2020 2020 2020 2020 2020  t.CSV.          
+0000b880: 2020 6a6f 625f 636f 6e66 6967 2e77 7269    job_config.wri
+0000b890: 7465 5f64 6973 706f 7369 7469 6f6e 203d  te_disposition =
+0000b8a0: 2062 6967 7175 6572 792e 5772 6974 6544   bigquery.WriteD
+0000b8b0: 6973 706f 7369 7469 6f6e 2e57 5249 5445  isposition.WRITE
+0000b8c0: 5f45 4d50 5459 0a20 2020 2020 2020 2020  _EMPTY.         
+0000b8d0: 2020 206a 6f62 5f63 6f6e 6669 672e 6175     job_config.au
+0000b8e0: 746f 6465 7465 6374 203d 2054 7275 650a  todetect = True.
+0000b8f0: 2020 2020 2020 2020 2020 2020 6a6f 625f              job_
+0000b900: 636f 6e66 6967 2e66 6965 6c64 5f64 656c  config.field_del
+0000b910: 696d 6974 6572 203d 2073 6570 0a20 2020  imiter = sep.   
+0000b920: 2020 2020 2020 2020 206a 6f62 5f63 6f6e           job_con
+0000b930: 6669 672e 656e 636f 6469 6e67 203d 2065  fig.encoding = e
+0000b940: 6e63 6f64 696e 670a 2020 2020 2020 2020  ncoding.        
+0000b950: 2020 2020 6a6f 625f 636f 6e66 6967 2e6c      job_config.l
+0000b960: 6162 656c 7320 3d20 7b22 6269 6766 7261  abels = {"bigfra
+0000b970: 6d65 732d 6170 6922 3a20 2272 6561 645f  mes-api": "read_
+0000b980: 6373 7622 7d0a 0a20 2020 2020 2020 2020  csv"}..         
+0000b990: 2020 2023 2057 6520 7761 6e74 2074 6f20     # We want to 
+0000b9a0: 6d61 7463 6820 7061 6e64 6173 2062 6568  match pandas beh
+0000b9b0: 6176 696f 722e 2049 6620 6865 6164 6572  avior. If header
+0000b9c0: 2069 7320 302c 206e 6f20 726f 7773 2073   is 0, no rows s
+0000b9d0: 686f 756c 6420 6265 2073 6b69 7070 6564  hould be skipped
+0000b9e0: 2c20 736f 2077 650a 2020 2020 2020 2020  , so we.        
+0000b9f0: 2020 2020 2320 646f 206e 6f74 206e 6565      # do not nee
+0000ba00: 6420 746f 2073 6574 2060 736b 6970 5f6c  d to set `skip_l
+0000ba10: 6561 6469 6e67 5f72 6f77 7360 2e20 4966  eading_rows`. If
+0000ba20: 2068 6561 6465 7220 6973 204e 6f6e 652c   header is None,
+0000ba30: 2074 6865 6e20 7468 6572 6520 6973 206e   then there is n
+0000ba40: 6f20 6865 6164 6572 2e0a 2020 2020 2020  o header..      
+0000ba50: 2020 2020 2020 2320 5365 7474 696e 6720        # Setting 
+0000ba60: 736b 6970 5f6c 6561 6469 6e67 5f72 6f77  skip_leading_row
+0000ba70: 7320 746f 2030 2064 6f65 7320 7468 6174  s to 0 does that
+0000ba80: 2e20 4966 2068 6561 6465 723d 4e20 616e  . If header=N an
+0000ba90: 6420 4e3e 302c 2077 6520 7761 6e74 2074  d N>0, we want t
+0000baa0: 6f20 736b 6970 204e 2072 6f77 732e 0a20  o skip N rows.. 
+0000bab0: 2020 2020 2020 2020 2020 2069 6620 6865             if he
+0000bac0: 6164 6572 2069 7320 4e6f 6e65 3a0a 2020  ader is None:.  
+0000bad0: 2020 2020 2020 2020 2020 2020 2020 6a6f                jo
+0000bae0: 625f 636f 6e66 6967 2e73 6b69 705f 6c65  b_config.skip_le
+0000baf0: 6164 696e 675f 726f 7773 203d 2030 0a20  ading_rows = 0. 
+0000bb00: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+0000bb10: 6865 6164 6572 203e 2030 3a0a 2020 2020  header > 0:.    
+0000bb20: 2020 2020 2020 2020 2020 2020 6a6f 625f              job_
+0000bb30: 636f 6e66 6967 2e73 6b69 705f 6c65 6164  config.skip_lead
+0000bb40: 696e 675f 726f 7773 203d 2068 6561 6465  ing_rows = heade
+0000bb50: 720a 0a20 2020 2020 2020 2020 2020 2072  r..            r
+0000bb60: 6574 7572 6e20 7365 6c66 2e5f 7265 6164  eturn self._read
+0000bb70: 5f62 6967 7175 6572 795f 6c6f 6164 5f6a  _bigquery_load_j
+0000bb80: 6f62 280a 2020 2020 2020 2020 2020 2020  ob(.            
+0000bb90: 2020 2020 6669 6c65 7061 7468 5f6f 725f      filepath_or_
+0000bba0: 6275 6666 6572 2c0a 2020 2020 2020 2020  buffer,.        
+0000bbb0: 2020 2020 2020 2020 7461 626c 652c 0a20          table,. 
+0000bbc0: 2020 2020 2020 2020 2020 2020 2020 206a                 j
+0000bbd0: 6f62 5f63 6f6e 6669 673d 6a6f 625f 636f  ob_config=job_co
+0000bbe0: 6e66 6967 2c0a 2020 2020 2020 2020 2020  nfig,.          
+0000bbf0: 2020 2020 2020 696e 6465 785f 636f 6c3d        index_col=
+0000bc00: 696e 6465 785f 636f 6c2c 0a20 2020 2020  index_col,.     
+0000bc10: 2020 2020 2020 2020 2020 2063 6f6c 756d             colum
+0000bc20: 6e73 3d63 6f6c 756d 6e73 2c0a 2020 2020  ns=columns,.    
+0000bc30: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+0000bc40: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0000bc50: 2020 2020 6966 2061 6e79 2861 7267 2069      if any(arg i
+0000bc60: 6e20 6b77 6172 6773 2066 6f72 2061 7267  n kwargs for arg
+0000bc70: 2069 6e20 2822 6368 756e 6b73 697a 6522   in ("chunksize"
+0000bc80: 2c20 2269 7465 7261 746f 7222 2929 3a0a  , "iterator")):.
+0000bc90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bca0: 7261 6973 6520 4e6f 7449 6d70 6c65 6d65  raise NotImpleme
+0000bcb0: 6e74 6564 4572 726f 7228 0a20 2020 2020  ntedError(.     
+0000bcc0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+0000bcd0: 2763 6875 6e6b 7369 7a65 2720 616e 6420  'chunksize' and 
+0000bce0: 2769 7465 7261 746f 7227 2061 7267 756d  'iterator' argum
+0000bcf0: 656e 7473 2061 7265 206e 6f74 2073 7570  ents are not sup
+0000bd00: 706f 7274 6564 2e20 220a 2020 2020 2020  ported. ".      
+0000bd10: 2020 2020 2020 2020 2020 2020 2020 6622                f"
+0000bd20: 7b63 6f6e 7374 616e 7473 2e46 4545 4442  {constants.FEEDB
+0000bd30: 4143 4b5f 4c49 4e4b 7d22 0a20 2020 2020  ACK_LINK}".     
+0000bd40: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
+0000bd50: 2020 2020 2020 2020 2020 6966 2069 7369            if isi
+0000bd60: 6e73 7461 6e63 6528 6669 6c65 7061 7468  nstance(filepath
+0000bd70: 5f6f 725f 6275 6666 6572 2c20 7374 7229  _or_buffer, str)
+0000bd80: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000bd90: 2020 7365 6c66 2e5f 6368 6563 6b5f 6669    self._check_fi
+0000bda0: 6c65 5f73 697a 6528 6669 6c65 7061 7468  le_size(filepath
+0000bdb0: 5f6f 725f 6275 6666 6572 290a 2020 2020  _or_buffer).    
+0000bdc0: 2020 2020 2020 2020 7061 6e64 6173 5f64          pandas_d
+0000bdd0: 6620 3d20 7061 6e64 6173 2e72 6561 645f  f = pandas.read_
+0000bde0: 6373 7628 0a20 2020 2020 2020 2020 2020  csv(.           
+0000bdf0: 2020 2020 2066 696c 6570 6174 685f 6f72       filepath_or
+0000be00: 5f62 7566 6665 722c 0a20 2020 2020 2020  _buffer,.       
+0000be10: 2020 2020 2020 2020 2073 6570 3d73 6570           sep=sep
+0000be20: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000be30: 2020 6865 6164 6572 3d68 6561 6465 722c    header=header,
+0000be40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000be50: 206e 616d 6573 3d6e 616d 6573 2c0a 2020   names=names,.  
+0000be60: 2020 2020 2020 2020 2020 2020 2020 696e                in
+0000be70: 6465 785f 636f 6c3d 696e 6465 785f 636f  dex_col=index_co
+0000be80: 6c2c 0a20 2020 2020 2020 2020 2020 2020  l,.             
+0000be90: 2020 2075 7365 636f 6c73 3d75 7365 636f     usecols=useco
+0000bea0: 6c73 2c20 2023 2074 7970 653a 2069 676e  ls,  # type: ign
+0000beb0: 6f72 650a 2020 2020 2020 2020 2020 2020  ore.            
+0000bec0: 2020 2020 6474 7970 653d 6474 7970 652c      dtype=dtype,
+0000bed0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000bee0: 2065 6e67 696e 653d 656e 6769 6e65 2c0a   engine=engine,.
+0000bef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bf00: 656e 636f 6469 6e67 3d65 6e63 6f64 696e  encoding=encodin
+0000bf10: 672c 0a20 2020 2020 2020 2020 2020 2020  g,.             
+0000bf20: 2020 202a 2a6b 7761 7267 732c 0a20 2020     **kwargs,.   
+0000bf30: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+0000bf40: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+0000bf50: 6c66 2e5f 7265 6164 5f70 616e 6461 7328  lf._read_pandas(
+0000bf60: 7061 6e64 6173 5f64 662c 2022 7265 6164  pandas_df, "read
+0000bf70: 5f63 7376 2229 2020 2320 7479 7065 3a20  _csv")  # type: 
+0000bf80: 6967 6e6f 7265 0a0a 2020 2020 6465 6620  ignore..    def 
+0000bf90: 7265 6164 5f70 6963 6b6c 6528 0a20 2020  read_pickle(.   
+0000bfa0: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+0000bfb0: 2020 2066 696c 6570 6174 685f 6f72 5f62     filepath_or_b
+0000bfc0: 7566 6665 723a 2046 696c 6550 6174 6820  uffer: FilePath 
+0000bfd0: 7c20 5265 6164 5069 636b 6c65 4275 6666  | ReadPickleBuff
+0000bfe0: 6572 2c0a 2020 2020 2020 2020 636f 6d70  er,.        comp
+0000bff0: 7265 7373 696f 6e3a 2043 6f6d 7072 6573  ression: Compres
+0000c000: 7369 6f6e 4f70 7469 6f6e 7320 3d20 2269  sionOptions = "i
+0000c010: 6e66 6572 222c 0a20 2020 2020 2020 2073  nfer",.        s
+0000c020: 746f 7261 6765 5f6f 7074 696f 6e73 3a20  torage_options: 
+0000c030: 5374 6f72 6167 654f 7074 696f 6e73 203d  StorageOptions =
+0000c040: 204e 6f6e 652c 0a20 2020 2029 3a0a 2020   None,.    ):.  
+0000c050: 2020 2020 2020 7061 6e64 6173 5f6f 626a        pandas_obj
+0000c060: 203d 2070 616e 6461 732e 7265 6164 5f70   = pandas.read_p
+0000c070: 6963 6b6c 6528 0a20 2020 2020 2020 2020  ickle(.         
+0000c080: 2020 2066 696c 6570 6174 685f 6f72 5f62     filepath_or_b
+0000c090: 7566 6665 722c 0a20 2020 2020 2020 2020  uffer,.         
+0000c0a0: 2020 2063 6f6d 7072 6573 7369 6f6e 3d63     compression=c
+0000c0b0: 6f6d 7072 6573 7369 6f6e 2c0a 2020 2020  ompression,.    
+0000c0c0: 2020 2020 2020 2020 7374 6f72 6167 655f          storage_
+0000c0d0: 6f70 7469 6f6e 733d 7374 6f72 6167 655f  options=storage_
+0000c0e0: 6f70 7469 6f6e 732c 0a20 2020 2020 2020  options,.       
+0000c0f0: 2029 0a0a 2020 2020 2020 2020 6966 2069   )..        if i
+0000c100: 7369 6e73 7461 6e63 6528 7061 6e64 6173  sinstance(pandas
+0000c110: 5f6f 626a 2c20 7061 6e64 6173 2e53 6572  _obj, pandas.Ser
+0000c120: 6965 7329 3a0a 2020 2020 2020 2020 2020  ies):.          
+0000c130: 2020 6966 2070 616e 6461 735f 6f62 6a2e    if pandas_obj.
+0000c140: 6e61 6d65 2069 7320 4e6f 6e65 3a0a 2020  name is None:.  
+0000c150: 2020 2020 2020 2020 2020 2020 2020 7061                pa
+0000c160: 6e64 6173 5f6f 626a 2e6e 616d 6520 3d20  ndas_obj.name = 
+0000c170: 2230 220a 2020 2020 2020 2020 2020 2020  "0".            
+0000c180: 6269 6766 7261 6d65 735f 6466 203d 2073  bigframes_df = s
+0000c190: 656c 662e 5f72 6561 645f 7061 6e64 6173  elf._read_pandas
+0000c1a0: 2870 616e 6461 735f 6f62 6a2e 746f 5f66  (pandas_obj.to_f
+0000c1b0: 7261 6d65 2829 2c20 2272 6561 645f 7069  rame(), "read_pi
+0000c1c0: 636b 6c65 2229 0a20 2020 2020 2020 2020  ckle").         
+0000c1d0: 2020 2072 6574 7572 6e20 6269 6766 7261     return bigfra
+0000c1e0: 6d65 735f 6466 5b62 6967 6672 616d 6573  mes_df[bigframes
+0000c1f0: 5f64 662e 636f 6c75 6d6e 735b 305d 5d0a  _df.columns[0]].
+0000c200: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+0000c210: 656c 662e 5f72 6561 645f 7061 6e64 6173  elf._read_pandas
+0000c220: 2870 616e 6461 735f 6f62 6a2c 2022 7265  (pandas_obj, "re
+0000c230: 6164 5f70 6963 6b6c 6522 290a 0a20 2020  ad_pickle")..   
+0000c240: 2064 6566 2072 6561 645f 7061 7271 7565   def read_parque
+0000c250: 7428 0a20 2020 2020 2020 2073 656c 662c  t(.        self,
+0000c260: 0a20 2020 2020 2020 2070 6174 683a 2073  .        path: s
+0000c270: 7472 207c 2049 4f5b 2262 7974 6573 225d  tr | IO["bytes"]
+0000c280: 2c0a 2020 2020 2020 2020 2a2c 0a20 2020  ,.        *,.   
+0000c290: 2020 2020 2065 6e67 696e 653a 2073 7472       engine: str
+0000c2a0: 203d 2022 6175 746f 222c 0a20 2020 2029   = "auto",.    )
+0000c2b0: 202d 3e20 6461 7461 6672 616d 652e 4461   -> dataframe.Da
+0000c2c0: 7461 4672 616d 653a 0a20 2020 2020 2020  taFrame:.       
+0000c2d0: 2074 6162 6c65 203d 2062 6967 6672 616d   table = bigfram
+0000c2e0: 6573 5f69 6f2e 7261 6e64 6f6d 5f74 6162  es_io.random_tab
+0000c2f0: 6c65 2873 656c 662e 5f61 6e6f 6e79 6d6f  le(self._anonymo
+0000c300: 7573 5f64 6174 6173 6574 290a 0a20 2020  us_dataset)..   
+0000c310: 2020 2020 2069 6620 656e 6769 6e65 203d       if engine =
+0000c320: 3d20 2262 6967 7175 6572 7922 3a0a 2020  = "bigquery":.  
+0000c330: 2020 2020 2020 2020 2020 6a6f 625f 636f            job_co
+0000c340: 6e66 6967 203d 2073 656c 662e 5f70 7265  nfig = self._pre
+0000c350: 7061 7265 5f6c 6f61 645f 6a6f 625f 636f  pare_load_job_co
+0000c360: 6e66 6967 2829 0a20 2020 2020 2020 2020  nfig().         
+0000c370: 2020 206a 6f62 5f63 6f6e 6669 672e 6372     job_config.cr
+0000c380: 6561 7465 5f64 6973 706f 7369 7469 6f6e  eate_disposition
+0000c390: 203d 2062 6967 7175 6572 792e 4372 6561   = bigquery.Crea
+0000c3a0: 7465 4469 7370 6f73 6974 696f 6e2e 4352  teDisposition.CR
+0000c3b0: 4541 5445 5f49 465f 4e45 4544 4544 0a20  EATE_IF_NEEDED. 
+0000c3c0: 2020 2020 2020 2020 2020 206a 6f62 5f63             job_c
+0000c3d0: 6f6e 6669 672e 736f 7572 6365 5f66 6f72  onfig.source_for
+0000c3e0: 6d61 7420 3d20 6269 6771 7565 7279 2e53  mat = bigquery.S
+0000c3f0: 6f75 7263 6546 6f72 6d61 742e 5041 5251  ourceFormat.PARQ
+0000c400: 5545 540a 2020 2020 2020 2020 2020 2020  UET.            
+0000c410: 6a6f 625f 636f 6e66 6967 2e77 7269 7465  job_config.write
+0000c420: 5f64 6973 706f 7369 7469 6f6e 203d 2062  _disposition = b
+0000c430: 6967 7175 6572 792e 5772 6974 6544 6973  igquery.WriteDis
+0000c440: 706f 7369 7469 6f6e 2e57 5249 5445 5f45  position.WRITE_E
+0000c450: 4d50 5459 0a20 2020 2020 2020 2020 2020  MPTY.           
+0000c460: 206a 6f62 5f63 6f6e 6669 672e 6c61 6265   job_config.labe
+0000c470: 6c73 203d 207b 2262 6967 6672 616d 6573  ls = {"bigframes
+0000c480: 2d61 7069 223a 2022 7265 6164 5f70 6172  -api": "read_par
+0000c490: 7175 6574 227d 0a0a 2020 2020 2020 2020  quet"}..        
+0000c4a0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+0000c4b0: 5f72 6561 645f 6269 6771 7565 7279 5f6c  _read_bigquery_l
+0000c4c0: 6f61 645f 6a6f 6228 7061 7468 2c20 7461  oad_job(path, ta
+0000c4d0: 626c 652c 206a 6f62 5f63 6f6e 6669 673d  ble, job_config=
+0000c4e0: 6a6f 625f 636f 6e66 6967 290a 2020 2020  job_config).    
+0000c4f0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0000c500: 2020 2020 2020 7265 6164 5f70 6172 7175        read_parqu
+0000c510: 6574 5f6b 7761 7267 733a 2044 6963 745b  et_kwargs: Dict[
+0000c520: 7374 722c 2041 6e79 5d20 3d20 7b7d 0a20  str, Any] = {}. 
+0000c530: 2020 2020 2020 2020 2020 2069 6620 7061             if pa
+0000c540: 6e64 6173 2e5f 5f76 6572 7369 6f6e 5f5f  ndas.__version__
+0000c550: 2e73 7461 7274 7377 6974 6828 2231 2e22  .startswith("1."
+0000c560: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0000c570: 2020 2072 6561 645f 7061 7271 7565 745f     read_parquet_
+0000c580: 6b77 6172 6773 5b22 7573 655f 6e75 6c6c  kwargs["use_null
+0000c590: 6162 6c65 5f64 7479 7065 7322 5d20 3d20  able_dtypes"] = 
+0000c5a0: 5472 7565 0a20 2020 2020 2020 2020 2020  True.           
+0000c5b0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+0000c5c0: 2020 2020 2020 2072 6561 645f 7061 7271         read_parq
+0000c5d0: 7565 745f 6b77 6172 6773 5b22 6474 7970  uet_kwargs["dtyp
+0000c5e0: 655f 6261 636b 656e 6422 5d20 3d20 2270  e_backend"] = "p
+0000c5f0: 7961 7272 6f77 220a 0a20 2020 2020 2020  yarrow"..       
+0000c600: 2020 2020 2070 616e 6461 735f 6f62 6a20       pandas_obj 
+0000c610: 3d20 7061 6e64 6173 2e72 6561 645f 7061  = pandas.read_pa
+0000c620: 7271 7565 7428 0a20 2020 2020 2020 2020  rquet(.         
+0000c630: 2020 2020 2020 2070 6174 682c 0a20 2020         path,.   
+0000c640: 2020 2020 2020 2020 2020 2020 2065 6e67               eng
+0000c650: 696e 653d 656e 6769 6e65 2c20 2023 2074  ine=engine,  # t
+0000c660: 7970 653a 2069 676e 6f72 650a 2020 2020  ype: ignore.    
+0000c670: 2020 2020 2020 2020 2020 2020 2a2a 7265              **re
+0000c680: 6164 5f70 6172 7175 6574 5f6b 7761 7267  ad_parquet_kwarg
+0000c690: 732c 0a20 2020 2020 2020 2020 2020 2029  s,.            )
+0000c6a0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+0000c6b0: 7572 6e20 7365 6c66 2e5f 7265 6164 5f70  urn self._read_p
+0000c6c0: 616e 6461 7328 7061 6e64 6173 5f6f 626a  andas(pandas_obj
+0000c6d0: 2c20 2272 6561 645f 7061 7271 7565 7422  , "read_parquet"
+0000c6e0: 290a 0a20 2020 2064 6566 2072 6561 645f  )..    def read_
+0000c6f0: 6a73 6f6e 280a 2020 2020 2020 2020 7365  json(.        se
+0000c700: 6c66 2c0a 2020 2020 2020 2020 7061 7468  lf,.        path
+0000c710: 5f6f 725f 6275 663a 2073 7472 207c 2049  _or_buf: str | I
+0000c720: 4f5b 2262 7974 6573 225d 2c0a 2020 2020  O["bytes"],.    
+0000c730: 2020 2020 2a2c 0a20 2020 2020 2020 206f      *,.        o
+0000c740: 7269 656e 743a 204c 6974 6572 616c 5b0a  rient: Literal[.
+0000c750: 2020 2020 2020 2020 2020 2020 2273 706c              "spl
+0000c760: 6974 222c 2022 7265 636f 7264 7322 2c20  it", "records", 
+0000c770: 2269 6e64 6578 222c 2022 636f 6c75 6d6e  "index", "column
+0000c780: 7322 2c20 2276 616c 7565 7322 2c20 2274  s", "values", "t
+0000c790: 6162 6c65 220a 2020 2020 2020 2020 5d20  able".        ] 
+0000c7a0: 3d20 2263 6f6c 756d 6e73 222c 0a20 2020  = "columns",.   
+0000c7b0: 2020 2020 2064 7479 7065 3a20 4f70 7469       dtype: Opti
+0000c7c0: 6f6e 616c 5b44 6963 745d 203d 204e 6f6e  onal[Dict] = Non
+0000c7d0: 652c 0a20 2020 2020 2020 2065 6e63 6f64  e,.        encod
+0000c7e0: 696e 673a 204f 7074 696f 6e61 6c5b 7374  ing: Optional[st
+0000c7f0: 725d 203d 204e 6f6e 652c 0a20 2020 2020  r] = None,.     
+0000c800: 2020 206c 696e 6573 3a20 626f 6f6c 203d     lines: bool =
+0000c810: 2046 616c 7365 2c0a 2020 2020 2020 2020   False,.        
+0000c820: 656e 6769 6e65 3a20 4c69 7465 7261 6c5b  engine: Literal[
+0000c830: 2275 6a73 6f6e 222c 2022 7079 6172 726f  "ujson", "pyarro
+0000c840: 7722 2c20 2262 6967 7175 6572 7922 5d20  w", "bigquery"] 
+0000c850: 3d20 2275 6a73 6f6e 222c 0a20 2020 2020  = "ujson",.     
+0000c860: 2020 202a 2a6b 7761 7267 732c 0a20 2020     **kwargs,.   
+0000c870: 2029 202d 3e20 6461 7461 6672 616d 652e   ) -> dataframe.
+0000c880: 4461 7461 4672 616d 653a 0a20 2020 2020  DataFrame:.     
+0000c890: 2020 2074 6162 6c65 203d 2062 6967 6672     table = bigfr
+0000c8a0: 616d 6573 5f69 6f2e 7261 6e64 6f6d 5f74  ames_io.random_t
+0000c8b0: 6162 6c65 2873 656c 662e 5f61 6e6f 6e79  able(self._anony
+0000c8c0: 6d6f 7573 5f64 6174 6173 6574 290a 0a20  mous_dataset).. 
+0000c8d0: 2020 2020 2020 2069 6620 656e 6769 6e65         if engine
+0000c8e0: 203d 3d20 2262 6967 7175 6572 7922 3a0a   == "bigquery":.
+0000c8f0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0000c900: 6474 7970 6520 6973 206e 6f74 204e 6f6e  dtype is not Non
+0000c910: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+0000c920: 2020 2072 6169 7365 204e 6f74 496d 706c     raise NotImpl
+0000c930: 656d 656e 7465 6445 7272 6f72 280a 2020  ementedError(.  
+0000c940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c950: 2020 2242 6967 5175 6572 7920 656e 6769    "BigQuery engi
+0000c960: 6e65 2064 6f65 7320 6e6f 7420 7375 7070  ne does not supp
+0000c970: 6f72 7420 7468 6520 6474 7970 6520 6172  ort the dtype ar
+0000c980: 6775 6d65 6e74 732e 220a 2020 2020 2020  guments.".      
+0000c990: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
+0000c9a0: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
+0000c9b0: 6c69 6e65 733a 0a20 2020 2020 2020 2020  lines:.         
+0000c9c0: 2020 2020 2020 2072 6169 7365 204e 6f74         raise Not
+0000c9d0: 496d 706c 656d 656e 7465 6445 7272 6f72  ImplementedError
+0000c9e0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+0000c9f0: 2020 2020 2020 224f 6e6c 7920 6e65 776c        "Only newl
+0000ca00: 696e 6520 6465 6c69 6d69 7465 6420 4a53  ine delimited JS
+0000ca10: 4f4e 2066 6f72 6d61 7420 6973 2073 7570  ON format is sup
+0000ca20: 706f 7274 6564 2e22 0a20 2020 2020 2020  ported.".       
+0000ca30: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
+0000ca40: 2020 2020 2020 2020 6966 2065 6e63 6f64          if encod
+0000ca50: 696e 6720 6973 206e 6f74 204e 6f6e 6520  ing is not None 
+0000ca60: 616e 6420 656e 636f 6469 6e67 206e 6f74  and encoding not
+0000ca70: 2069 6e20 5f56 414c 4944 5f45 4e43 4f44   in _VALID_ENCOD
+0000ca80: 494e 4753 3a0a 2020 2020 2020 2020 2020  INGS:.          
+0000ca90: 2020 2020 2020 7261 6973 6520 4e6f 7449        raise NotI
+0000caa0: 6d70 6c65 6d65 6e74 6564 4572 726f 7228  mplementedError(
+0000cab0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000cac0: 2020 2020 2066 2242 6967 5175 6572 7920       f"BigQuery 
+0000cad0: 656e 6769 6e65 206f 6e6c 7920 7375 7070  engine only supp
+0000cae0: 6f72 7473 2074 6865 2066 6f6c 6c6f 7769  orts the followi
+0000caf0: 6e67 2065 6e63 6f64 696e 6773 3a20 7b5f  ng encodings: {_
+0000cb00: 5641 4c49 445f 454e 434f 4449 4e47 537d  VALID_ENCODINGS}
+0000cb10: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+0000cb20: 2020 290a 0a20 2020 2020 2020 2020 2020    )..           
+0000cb30: 2069 6620 6c69 6e65 7320 616e 6420 6f72   if lines and or
+0000cb40: 6965 6e74 2021 3d20 2272 6563 6f72 6473  ient != "records
+0000cb50: 223a 0a20 2020 2020 2020 2020 2020 2020  ":.             
+0000cb60: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
+0000cb70: 726f 7228 0a20 2020 2020 2020 2020 2020  ror(.           
+0000cb80: 2020 2020 2020 2020 2022 276c 696e 6573           "'lines
+0000cb90: 2720 6b65 7977 6f72 6420 6973 206f 6e6c  ' keyword is onl
+0000cba0: 7920 7661 6c69 6420 7768 656e 2027 6f72  y valid when 'or
+0000cbb0: 6965 6e74 2720 6973 2027 7265 636f 7264  ient' is 'record
+0000cbc0: 7327 2e22 0a20 2020 2020 2020 2020 2020  s'.".           
+0000cbd0: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+0000cbe0: 2020 2020 6a6f 625f 636f 6e66 6967 203d      job_config =
+0000cbf0: 2073 656c 662e 5f70 7265 7061 7265 5f6c   self._prepare_l
+0000cc00: 6f61 645f 6a6f 625f 636f 6e66 6967 2829  oad_job_config()
 0000cc10: 0a20 2020 2020 2020 2020 2020 206a 6f62  .            job
-0000cc20: 5f63 6f6e 6669 672e 6c61 6265 6c73 203d  _config.labels =
-0000cc30: 207b 2262 6967 6672 616d 6573 2d61 7069   {"bigframes-api
-0000cc40: 223a 2022 7265 6164 5f6a 736f 6e22 7d0a  ": "read_json"}.
-0000cc50: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-0000cc60: 7572 6e20 7365 6c66 2e5f 7265 6164 5f62  urn self._read_b
-0000cc70: 6967 7175 6572 795f 6c6f 6164 5f6a 6f62  igquery_load_job
-0000cc80: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0000cc90: 2020 7061 7468 5f6f 725f 6275 662c 0a20    path_or_buf,. 
-0000cca0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0000ccb0: 6162 6c65 2c0a 2020 2020 2020 2020 2020  able,.          
-0000ccc0: 2020 2020 2020 6a6f 625f 636f 6e66 6967        job_config
-0000ccd0: 3d6a 6f62 5f63 6f6e 6669 672c 0a20 2020  =job_config,.   
-0000cce0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-0000ccf0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-0000cd00: 2020 2020 2069 6620 616e 7928 6172 6720       if any(arg 
-0000cd10: 696e 206b 7761 7267 7320 666f 7220 6172  in kwargs for ar
-0000cd20: 6720 696e 2028 2263 6875 6e6b 7369 7a65  g in ("chunksize
-0000cd30: 222c 2022 6974 6572 6174 6f72 2229 293a  ", "iterator")):
-0000cd40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000cd50: 2072 6169 7365 204e 6f74 496d 706c 656d   raise NotImplem
-0000cd60: 656e 7465 6445 7272 6f72 280a 2020 2020  entedError(.    
-0000cd70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cd80: 2227 6368 756e 6b73 697a 6527 2061 6e64  "'chunksize' and
-0000cd90: 2027 6974 6572 6174 6f72 2720 6172 6775   'iterator' argu
-0000cda0: 6d65 6e74 7320 6172 6520 6e6f 7420 7375  ments are not su
-0000cdb0: 7070 6f72 7465 642e 220a 2020 2020 2020  pported.".      
-0000cdc0: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
-0000cdd0: 2020 2020 2020 2020 2069 6620 6973 696e           if isin
-0000cde0: 7374 616e 6365 2870 6174 685f 6f72 5f62  stance(path_or_b
-0000cdf0: 7566 2c20 7374 7229 3a0a 2020 2020 2020  uf, str):.      
-0000ce00: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-0000ce10: 6368 6563 6b5f 6669 6c65 5f73 697a 6528  check_file_size(
-0000ce20: 7061 7468 5f6f 725f 6275 6629 0a0a 2020  path_or_buf)..  
-0000ce30: 2020 2020 2020 2020 2020 6966 2065 6e67            if eng
-0000ce40: 696e 6520 3d3d 2022 756a 736f 6e22 3a0a  ine == "ujson":.
-0000ce50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ce60: 7061 6e64 6173 5f64 6620 3d20 7061 6e64  pandas_df = pand
-0000ce70: 6173 2e72 6561 645f 6a73 6f6e 2820 2023  as.read_json(  #
-0000ce80: 2074 7970 653a 2069 676e 6f72 650a 2020   type: ignore.  
-0000ce90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cea0: 2020 7061 7468 5f6f 725f 6275 662c 0a20    path_or_buf,. 
-0000ceb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cec0: 2020 206f 7269 656e 743d 6f72 6965 6e74     orient=orient
-0000ced0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000cee0: 2020 2020 2020 6474 7970 653d 6474 7970        dtype=dtyp
-0000cef0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-0000cf00: 2020 2020 2020 2065 6e63 6f64 696e 673d         encoding=
-0000cf10: 656e 636f 6469 6e67 2c0a 2020 2020 2020  encoding,.      
-0000cf20: 2020 2020 2020 2020 2020 2020 2020 6c69                li
-0000cf30: 6e65 733d 6c69 6e65 732c 0a20 2020 2020  nes=lines,.     
-0000cf40: 2020 2020 2020 2020 2020 2020 2020 202a                 *
-0000cf50: 2a6b 7761 7267 732c 0a20 2020 2020 2020  *kwargs,.       
-0000cf60: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
-0000cf70: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-0000cf80: 2020 2020 2020 2020 2020 2020 2020 7061                pa
-0000cf90: 6e64 6173 5f64 6620 3d20 7061 6e64 6173  ndas_df = pandas
-0000cfa0: 2e72 6561 645f 6a73 6f6e 2820 2023 2074  .read_json(  # t
-0000cfb0: 7970 653a 2069 676e 6f72 650a 2020 2020  ype: ignore.    
-0000cfc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cfd0: 7061 7468 5f6f 725f 6275 662c 0a20 2020  path_or_buf,.   
+0000cc20: 5f63 6f6e 6669 672e 6372 6561 7465 5f64  _config.create_d
+0000cc30: 6973 706f 7369 7469 6f6e 203d 2062 6967  isposition = big
+0000cc40: 7175 6572 792e 4372 6561 7465 4469 7370  query.CreateDisp
+0000cc50: 6f73 6974 696f 6e2e 4352 4541 5445 5f49  osition.CREATE_I
+0000cc60: 465f 4e45 4544 4544 0a20 2020 2020 2020  F_NEEDED.       
+0000cc70: 2020 2020 206a 6f62 5f63 6f6e 6669 672e       job_config.
+0000cc80: 736f 7572 6365 5f66 6f72 6d61 7420 3d20  source_format = 
+0000cc90: 6269 6771 7565 7279 2e53 6f75 7263 6546  bigquery.SourceF
+0000cca0: 6f72 6d61 742e 4e45 574c 494e 455f 4445  ormat.NEWLINE_DE
+0000ccb0: 4c49 4d49 5445 445f 4a53 4f4e 0a20 2020  LIMITED_JSON.   
+0000ccc0: 2020 2020 2020 2020 206a 6f62 5f63 6f6e           job_con
+0000ccd0: 6669 672e 7772 6974 655f 6469 7370 6f73  fig.write_dispos
+0000cce0: 6974 696f 6e20 3d20 6269 6771 7565 7279  ition = bigquery
+0000ccf0: 2e57 7269 7465 4469 7370 6f73 6974 696f  .WriteDispositio
+0000cd00: 6e2e 5752 4954 455f 454d 5054 590a 2020  n.WRITE_EMPTY.  
+0000cd10: 2020 2020 2020 2020 2020 6a6f 625f 636f            job_co
+0000cd20: 6e66 6967 2e61 7574 6f64 6574 6563 7420  nfig.autodetect 
+0000cd30: 3d20 5472 7565 0a20 2020 2020 2020 2020  = True.         
+0000cd40: 2020 206a 6f62 5f63 6f6e 6669 672e 656e     job_config.en
+0000cd50: 636f 6469 6e67 203d 2065 6e63 6f64 696e  coding = encodin
+0000cd60: 670a 2020 2020 2020 2020 2020 2020 6a6f  g.            jo
+0000cd70: 625f 636f 6e66 6967 2e6c 6162 656c 7320  b_config.labels 
+0000cd80: 3d20 7b22 6269 6766 7261 6d65 732d 6170  = {"bigframes-ap
+0000cd90: 6922 3a20 2272 6561 645f 6a73 6f6e 227d  i": "read_json"}
+0000cda0: 0a0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+0000cdb0: 7475 726e 2073 656c 662e 5f72 6561 645f  turn self._read_
+0000cdc0: 6269 6771 7565 7279 5f6c 6f61 645f 6a6f  bigquery_load_jo
+0000cdd0: 6228 0a20 2020 2020 2020 2020 2020 2020  b(.             
+0000cde0: 2020 2070 6174 685f 6f72 5f62 7566 2c0a     path_or_buf,.
+0000cdf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ce00: 7461 626c 652c 0a20 2020 2020 2020 2020  table,.         
+0000ce10: 2020 2020 2020 206a 6f62 5f63 6f6e 6669         job_confi
+0000ce20: 673d 6a6f 625f 636f 6e66 6967 2c0a 2020  g=job_config,.  
+0000ce30: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+0000ce40: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0000ce50: 2020 2020 2020 6966 2061 6e79 2861 7267        if any(arg
+0000ce60: 2069 6e20 6b77 6172 6773 2066 6f72 2061   in kwargs for a
+0000ce70: 7267 2069 6e20 2822 6368 756e 6b73 697a  rg in ("chunksiz
+0000ce80: 6522 2c20 2269 7465 7261 746f 7222 2929  e", "iterator"))
+0000ce90: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000cea0: 2020 7261 6973 6520 4e6f 7449 6d70 6c65    raise NotImple
+0000ceb0: 6d65 6e74 6564 4572 726f 7228 0a20 2020  mentedError(.   
+0000cec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ced0: 2022 2763 6875 6e6b 7369 7a65 2720 616e   "'chunksize' an
+0000cee0: 6420 2769 7465 7261 746f 7227 2061 7267  d 'iterator' arg
+0000cef0: 756d 656e 7473 2061 7265 206e 6f74 2073  uments are not s
+0000cf00: 7570 706f 7274 6564 2e22 0a20 2020 2020  upported.".     
+0000cf10: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
+0000cf20: 2020 2020 2020 2020 2020 6966 2069 7369            if isi
+0000cf30: 6e73 7461 6e63 6528 7061 7468 5f6f 725f  nstance(path_or_
+0000cf40: 6275 662c 2073 7472 293a 0a20 2020 2020  buf, str):.     
+0000cf50: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000cf60: 5f63 6865 636b 5f66 696c 655f 7369 7a65  _check_file_size
+0000cf70: 2870 6174 685f 6f72 5f62 7566 290a 0a20  (path_or_buf).. 
+0000cf80: 2020 2020 2020 2020 2020 2069 6620 656e             if en
+0000cf90: 6769 6e65 203d 3d20 2275 6a73 6f6e 223a  gine == "ujson":
+0000cfa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000cfb0: 2070 616e 6461 735f 6466 203d 2070 616e   pandas_df = pan
+0000cfc0: 6461 732e 7265 6164 5f6a 736f 6e28 2020  das.read_json(  
+0000cfd0: 2320 7479 7065 3a20 6967 6e6f 7265 0a20  # type: ignore. 
 0000cfe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cff0: 206f 7269 656e 743d 6f72 6965 6e74 2c0a   orient=orient,.
+0000cff0: 2020 2070 6174 685f 6f72 5f62 7566 2c0a     path_or_buf,.
 0000d000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d010: 2020 2020 6474 7970 653d 6474 7970 652c      dtype=dtype,
-0000d020: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d030: 2020 2020 2065 6e63 6f64 696e 673d 656e       encoding=en
-0000d040: 636f 6469 6e67 2c0a 2020 2020 2020 2020  coding,.        
-0000d050: 2020 2020 2020 2020 2020 2020 6c69 6e65              line
-0000d060: 733d 6c69 6e65 732c 0a20 2020 2020 2020  s=lines,.       
-0000d070: 2020 2020 2020 2020 2020 2020 2065 6e67               eng
-0000d080: 696e 653d 656e 6769 6e65 2c0a 2020 2020  ine=engine,.    
+0000d010: 2020 2020 6f72 6965 6e74 3d6f 7269 656e      orient=orien
+0000d020: 742c 0a20 2020 2020 2020 2020 2020 2020  t,.             
+0000d030: 2020 2020 2020 2064 7479 7065 3d64 7479         dtype=dty
+0000d040: 7065 2c0a 2020 2020 2020 2020 2020 2020  pe,.            
+0000d050: 2020 2020 2020 2020 656e 636f 6469 6e67          encoding
+0000d060: 3d65 6e63 6f64 696e 672c 0a20 2020 2020  =encoding,.     
+0000d070: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+0000d080: 696e 6573 3d6c 696e 6573 2c0a 2020 2020  ines=lines,.    
 0000d090: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000d0a0: 2a2a 6b77 6172 6773 2c0a 2020 2020 2020  **kwargs,.      
-0000d0b0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-0000d0c0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-0000d0d0: 656c 662e 5f72 6561 645f 7061 6e64 6173  elf._read_pandas
-0000d0e0: 2870 616e 6461 735f 6466 2c20 2272 6561  (pandas_df, "rea
-0000d0f0: 645f 6a73 6f6e 2229 0a0a 2020 2020 6465  d_json")..    de
-0000d100: 6620 5f63 6865 636b 5f66 696c 655f 7369  f _check_file_si
-0000d110: 7a65 2873 656c 662c 2066 696c 6570 6174  ze(self, filepat
-0000d120: 683a 2073 7472 293a 0a20 2020 2020 2020  h: str):.       
-0000d130: 206d 6178 5f73 697a 6520 3d20 3130 3234   max_size = 1024
-0000d140: 202a 2031 3032 3420 2a20 3130 3234 2020   * 1024 * 1024  
-0000d150: 2320 3120 4742 2069 6e20 6279 7465 730a  # 1 GB in bytes.
-0000d160: 2020 2020 2020 2020 6966 2066 696c 6570          if filep
-0000d170: 6174 682e 7374 6172 7473 7769 7468 2822  ath.startswith("
-0000d180: 6773 3a2f 2f22 293a 2020 2320 4743 5320  gs://"):  # GCS 
-0000d190: 6669 6c65 2070 6174 680a 2020 2020 2020  file path.      
-0000d1a0: 2020 2020 2020 636c 6965 6e74 203d 2073        client = s
-0000d1b0: 746f 7261 6765 2e43 6c69 656e 7428 290a  torage.Client().
-0000d1c0: 2020 2020 2020 2020 2020 2020 6275 636b              buck
-0000d1d0: 6574 5f6e 616d 652c 2062 6c6f 625f 6e61  et_name, blob_na
-0000d1e0: 6d65 203d 2066 696c 6570 6174 682e 7370  me = filepath.sp
-0000d1f0: 6c69 7428 222f 222c 2033 295b 323a 5d0a  lit("/", 3)[2:].
-0000d200: 2020 2020 2020 2020 2020 2020 6275 636b              buck
-0000d210: 6574 203d 2063 6c69 656e 742e 6275 636b  et = client.buck
-0000d220: 6574 2862 7563 6b65 745f 6e61 6d65 290a  et(bucket_name).
-0000d230: 2020 2020 2020 2020 2020 2020 626c 6f62              blob
-0000d240: 203d 2062 7563 6b65 742e 626c 6f62 2862   = bucket.blob(b
-0000d250: 6c6f 625f 6e61 6d65 290a 2020 2020 2020  lob_name).      
-0000d260: 2020 2020 2020 626c 6f62 2e72 656c 6f61        blob.reloa
-0000d270: 6428 290a 2020 2020 2020 2020 2020 2020  d().            
-0000d280: 6669 6c65 5f73 697a 6520 3d20 626c 6f62  file_size = blob
-0000d290: 2e73 697a 650a 2020 2020 2020 2020 656c  .size.        el
-0000d2a0: 7365 3a20 2023 206c 6f63 616c 2066 696c  se:  # local fil
-0000d2b0: 6520 7061 7468 0a20 2020 2020 2020 2020  e path.         
-0000d2c0: 2020 2066 696c 655f 7369 7a65 203d 206f     file_size = o
-0000d2d0: 732e 7061 7468 2e67 6574 7369 7a65 2866  s.path.getsize(f
-0000d2e0: 696c 6570 6174 6829 0a0a 2020 2020 2020  ilepath)..      
-0000d2f0: 2020 6966 2066 696c 655f 7369 7a65 203e    if file_size >
-0000d300: 206d 6178 5f73 697a 653a 0a20 2020 2020   max_size:.     
-0000d310: 2020 2020 2020 2023 2043 6f6e 7665 7274         # Convert
-0000d320: 2074 6f20 4742 0a20 2020 2020 2020 2020   to GB.         
-0000d330: 2020 2066 696c 655f 7369 7a65 203d 2072     file_size = r
-0000d340: 6f75 6e64 2866 696c 655f 7369 7a65 202f  ound(file_size /
-0000d350: 2028 3130 3234 2a2a 3329 2c20 3129 0a20   (1024**3), 1). 
-0000d360: 2020 2020 2020 2020 2020 206d 6178 5f73             max_s
-0000d370: 697a 6520 3d20 696e 7428 6d61 785f 7369  ize = int(max_si
-0000d380: 7a65 202f 2031 3032 342a 2a33 290a 2020  ze / 1024**3).  
-0000d390: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
-0000d3a0: 2e77 6172 6e69 6e67 280a 2020 2020 2020  .warning(.      
-0000d3b0: 2020 2020 2020 2020 2020 6622 4669 6c65            f"File
-0000d3c0: 2073 697a 6520 7b66 696c 655f 7369 7a65   size {file_size
-0000d3d0: 7d47 4220 6578 6365 6564 7320 7b6d 6178  }GB exceeds {max
-0000d3e0: 5f73 697a 657d 4742 2e20 220a 2020 2020  _size}GB. ".    
-0000d3f0: 2020 2020 2020 2020 2020 2020 2249 7420              "It 
-0000d400: 6973 2072 6563 6f6d 6d65 6e64 6564 2074  is recommended t
-0000d410: 6f20 7573 6520 656e 6769 6e65 3d27 6269  o use engine='bi
-0000d420: 6771 7565 7279 2720 220a 2020 2020 2020  gquery' ".      
-0000d430: 2020 2020 2020 2020 2020 2266 6f72 206c            "for l
-0000d440: 6172 6765 2066 696c 6573 2074 6f20 6176  arge files to av
-0000d450: 6f69 6420 6c6f 6164 696e 6720 7468 6520  oid loading the 
-0000d460: 6669 6c65 2069 6e74 6f20 6c6f 6361 6c20  file into local 
-0000d470: 6d65 6d6f 7279 2e22 0a20 2020 2020 2020  memory.".       
-0000d480: 2020 2020 2029 0a0a 2020 2020 6465 6620       )..    def 
-0000d490: 5f63 7265 6174 655f 656d 7074 795f 7465  _create_empty_te
-0000d4a0: 6d70 5f74 6162 6c65 280a 2020 2020 2020  mp_table(.      
-0000d4b0: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-0000d4c0: 7363 6865 6d61 3a20 4974 6572 6162 6c65  schema: Iterable
-0000d4d0: 5b62 6967 7175 6572 792e 5363 6865 6d61  [bigquery.Schema
-0000d4e0: 4669 656c 645d 2c0a 2020 2020 2020 2020  Field],.        
-0000d4f0: 636c 7573 7465 725f 636f 6c73 3a20 4c69  cluster_cols: Li
-0000d500: 7374 5b73 7472 5d2c 0a20 2020 2029 202d  st[str],.    ) -
-0000d510: 3e20 6269 6771 7565 7279 2e54 6162 6c65  > bigquery.Table
-0000d520: 5265 6665 7265 6e63 653a 0a20 2020 2020  Reference:.     
-0000d530: 2020 2023 2043 616e 2774 2073 6574 2061     # Can't set a
-0000d540: 2074 6162 6c65 2069 6e20 5f53 4553 5349   table in _SESSI
-0000d550: 4f4e 2061 7320 6465 7374 696e 6174 696f  ON as destinatio
-0000d560: 6e20 7669 6120 7175 6572 7920 6a6f 6220  n via query job 
-0000d570: 4150 492c 2073 6f20 7765 0a20 2020 2020  API, so we.     
-0000d580: 2020 2023 2072 756e 2044 444c 2c20 696e     # run DDL, in
-0000d590: 7374 6561 642e 0a20 2020 2020 2020 2064  stead..        d
-0000d5a0: 6174 6173 6574 203d 2073 656c 662e 5f61  ataset = self._a
-0000d5b0: 6e6f 6e79 6d6f 7573 5f64 6174 6173 6574  nonymous_dataset
-0000d5c0: 0a20 2020 2020 2020 2065 7870 6972 6174  .        expirat
-0000d5d0: 696f 6e20 3d20 280a 2020 2020 2020 2020  ion = (.        
-0000d5e0: 2020 2020 6461 7465 7469 6d65 2e64 6174      datetime.dat
-0000d5f0: 6574 696d 652e 6e6f 7728 6461 7465 7469  etime.now(dateti
-0000d600: 6d65 2e74 696d 657a 6f6e 652e 7574 6329  me.timezone.utc)
-0000d610: 202b 2063 6f6e 7374 616e 7473 2e44 4546   + constants.DEF
-0000d620: 4155 4c54 5f45 5850 4952 4154 494f 4e0a  AULT_EXPIRATION.
-0000d630: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
-0000d640: 2020 2074 6162 6c65 203d 2062 6967 6672     table = bigfr
-0000d650: 616d 6573 5f69 6f2e 6372 6561 7465 5f74  ames_io.create_t
-0000d660: 656d 705f 7461 626c 6528 0a20 2020 2020  emp_table(.     
-0000d670: 2020 2020 2020 2073 656c 662e 6271 636c         self.bqcl
-0000d680: 6965 6e74 2c0a 2020 2020 2020 2020 2020  ient,.          
-0000d690: 2020 6461 7461 7365 742c 0a20 2020 2020    dataset,.     
-0000d6a0: 2020 2020 2020 2065 7870 6972 6174 696f         expiratio
-0000d6b0: 6e2c 0a20 2020 2020 2020 2020 2020 2073  n,.            s
-0000d6c0: 6368 656d 613d 7363 6865 6d61 2c0a 2020  chema=schema,.  
-0000d6d0: 2020 2020 2020 2020 2020 636c 7573 7465            cluste
-0000d6e0: 725f 636f 6c75 6d6e 733d 636c 7573 7465  r_columns=cluste
-0000d6f0: 725f 636f 6c73 2c0a 2020 2020 2020 2020  r_cols,.        
-0000d700: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-0000d710: 2062 6967 7175 6572 792e 5461 626c 6552   bigquery.TableR
-0000d720: 6566 6572 656e 6365 2e66 726f 6d5f 7374  eference.from_st
-0000d730: 7269 6e67 2874 6162 6c65 290a 0a20 2020  ring(table)..   
-0000d740: 2064 6566 205f 6372 6561 7465 5f74 6f74   def _create_tot
-0000d750: 616c 5f6f 7264 6572 696e 6728 0a20 2020  al_ordering(.   
-0000d760: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-0000d770: 2020 2074 6162 6c65 3a20 6962 6973 5f74     table: ibis_t
-0000d780: 7970 6573 2e54 6162 6c65 2c0a 2020 2020  ypes.Table,.    
-0000d790: 2920 2d3e 2063 6f72 652e 4172 7261 7956  ) -> core.ArrayV
-0000d7a0: 616c 7565 3a0a 2020 2020 2020 2020 2320  alue:.        # 
-0000d7b0: 5369 6e63 6520 7468 6973 206d 6967 6874  Since this might
-0000d7c0: 2061 6c73 6f20 6265 2075 7365 6420 6173   also be used as
-0000d7d0: 2074 6865 2069 6e64 6578 2c20 646f 6e27   the index, don'
-0000d7e0: 7420 7573 6520 7468 6520 6465 6661 756c  t use the defaul
-0000d7f0: 740a 2020 2020 2020 2020 2320 226f 7264  t.        # "ord
-0000d800: 6572 696e 6720 4944 2220 6e61 6d65 2e0a  ering ID" name..
-0000d810: 2020 2020 2020 2020 6f72 6465 7269 6e67          ordering
-0000d820: 5f68 6173 685f 7061 7274 203d 2067 7569  _hash_part = gui
-0000d830: 642e 6765 6e65 7261 7465 5f67 7569 6428  d.generate_guid(
-0000d840: 2262 6967 6672 616d 6573 5f6f 7264 6572  "bigframes_order
-0000d850: 696e 675f 2229 0a20 2020 2020 2020 206f  ing_").        o
-0000d860: 7264 6572 696e 675f 7261 6e64 5f70 6172  rdering_rand_par
-0000d870: 7420 3d20 6775 6964 2e67 656e 6572 6174  t = guid.generat
-0000d880: 655f 6775 6964 2822 6269 6766 7261 6d65  e_guid("bigframe
-0000d890: 735f 6f72 6465 7269 6e67 5f22 290a 0a20  s_ordering_").. 
-0000d8a0: 2020 2020 2020 2023 2041 6c6c 2069 6e70         # All inp
-0000d8b0: 7574 7320 696e 746f 2068 6173 6820 6d75  uts into hash mu
-0000d8c0: 7374 2062 6520 6e6f 6e2d 6e75 6c6c 206f  st be non-null o
-0000d8d0: 7220 7265 7375 6c74 696e 6720 6861 7368  r resulting hash
-0000d8e0: 2077 696c 6c20 6265 206e 756c 6c0a 2020   will be null.  
-0000d8f0: 2020 2020 2020 7374 725f 7661 6c75 6573        str_values
-0000d900: 203d 206c 6973 7428 0a20 2020 2020 2020   = list(.       
-0000d910: 2020 2020 206d 6170 286c 616d 6264 6120       map(lambda 
-0000d920: 636f 6c3a 205f 636f 6e76 6572 745f 746f  col: _convert_to
-0000d930: 5f6e 6f6e 6e75 6c6c 5f73 7472 696e 6728  _nonnull_string(
-0000d940: 7461 626c 655b 636f 6c5d 292c 2074 6162  table[col]), tab
-0000d950: 6c65 2e63 6f6c 756d 6e73 290a 2020 2020  le.columns).    
-0000d960: 2020 2020 290a 2020 2020 2020 2020 6675      ).        fu
-0000d970: 6c6c 5f72 6f77 5f73 7472 203d 2028 0a20  ll_row_str = (. 
-0000d980: 2020 2020 2020 2020 2020 2073 7472 5f76             str_v
-0000d990: 616c 7565 735b 305d 2e63 6f6e 6361 7428  alues[0].concat(
-0000d9a0: 2a73 7472 5f76 616c 7565 735b 313a 5d29  *str_values[1:])
-0000d9b0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000d9c0: 6c65 6e28 7374 725f 7661 6c75 6573 2920  len(str_values) 
-0000d9d0: 3e20 310a 2020 2020 2020 2020 2020 2020  > 1.            
-0000d9e0: 656c 7365 2073 7472 5f76 616c 7565 735b  else str_values[
-0000d9f0: 305d 0a20 2020 2020 2020 2029 0a20 2020  0].        ).   
-0000da00: 2020 2020 2066 756c 6c5f 726f 775f 6861       full_row_ha
-0000da10: 7368 203d 2066 756c 6c5f 726f 775f 7374  sh = full_row_st
-0000da20: 722e 6861 7368 2829 2e6e 616d 6528 6f72  r.hash().name(or
-0000da30: 6465 7269 6e67 5f68 6173 685f 7061 7274  dering_hash_part
-0000da40: 290a 2020 2020 2020 2020 2320 5573 6564  ).        # Used
-0000da50: 2074 6f20 6469 7361 6d62 6967 7561 7465   to disambiguate
-0000da60: 2062 6574 7765 656e 2069 6465 6e74 6963   between identic
-0000da70: 616c 2072 6f77 7320 2877 6869 6368 2077  al rows (which w
-0000da80: 696c 6c20 6861 7665 2069 6465 6e74 6963  ill have identic
-0000da90: 616c 2068 6173 6829 0a20 2020 2020 2020  al hash).       
-0000daa0: 2072 616e 646f 6d5f 7661 6c75 6520 3d20   random_value = 
-0000dab0: 6962 6973 2e72 616e 646f 6d28 292e 6e61  ibis.random().na
-0000dac0: 6d65 286f 7264 6572 696e 675f 7261 6e64  me(ordering_rand
-0000dad0: 5f70 6172 7429 0a0a 2020 2020 2020 2020  _part)..        
-0000dae0: 6f72 6967 696e 616c 5f63 6f6c 756d 6e5f  original_column_
-0000daf0: 6964 7320 3d20 7461 626c 652e 636f 6c75  ids = table.colu
-0000db00: 6d6e 730a 2020 2020 2020 2020 7461 626c  mns.        tabl
-0000db10: 655f 7769 7468 5f6f 7264 6572 696e 6720  e_with_ordering 
-0000db20: 3d20 7461 626c 652e 7365 6c65 6374 280a  = table.select(.
-0000db30: 2020 2020 2020 2020 2020 2020 6974 6572              iter
-0000db40: 746f 6f6c 732e 6368 6169 6e28 6f72 6967  tools.chain(orig
-0000db50: 696e 616c 5f63 6f6c 756d 6e5f 6964 732c  inal_column_ids,
-0000db60: 205b 6675 6c6c 5f72 6f77 5f68 6173 682c   [full_row_hash,
-0000db70: 2072 616e 646f 6d5f 7661 6c75 655d 290a   random_value]).
-0000db80: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
-0000db90: 2020 206f 7264 6572 696e 675f 7265 6631     ordering_ref1
-0000dba0: 203d 206f 7264 6572 2e61 7363 656e 6469   = order.ascendi
-0000dbb0: 6e67 5f6f 7665 7228 6f72 6465 7269 6e67  ng_over(ordering
-0000dbc0: 5f68 6173 685f 7061 7274 290a 2020 2020  _hash_part).    
-0000dbd0: 2020 2020 6f72 6465 7269 6e67 5f72 6566      ordering_ref
-0000dbe0: 3220 3d20 6f72 6465 722e 6173 6365 6e64  2 = order.ascend
-0000dbf0: 696e 675f 6f76 6572 286f 7264 6572 696e  ing_over(orderin
-0000dc00: 675f 7261 6e64 5f70 6172 7429 0a20 2020  g_rand_part).   
-0000dc10: 2020 2020 206f 7264 6572 696e 6720 3d20       ordering = 
-0000dc20: 6f72 6465 722e 4578 7072 6573 7369 6f6e  order.Expression
-0000dc30: 4f72 6465 7269 6e67 280a 2020 2020 2020  Ordering(.      
-0000dc40: 2020 2020 2020 6f72 6465 7269 6e67 5f76        ordering_v
-0000dc50: 616c 7565 5f63 6f6c 756d 6e73 3d28 6f72  alue_columns=(or
-0000dc60: 6465 7269 6e67 5f72 6566 312c 206f 7264  dering_ref1, ord
-0000dc70: 6572 696e 675f 7265 6632 292c 0a20 2020  ering_ref2),.   
-0000dc80: 2020 2020 2020 2020 2074 6f74 616c 5f6f           total_o
-0000dc90: 7264 6572 696e 675f 636f 6c75 6d6e 733d  rdering_columns=
-0000dca0: 6672 6f7a 656e 7365 7428 5b6f 7264 6572  frozenset([order
-0000dcb0: 696e 675f 6861 7368 5f70 6172 742c 206f  ing_hash_part, o
-0000dcc0: 7264 6572 696e 675f 7261 6e64 5f70 6172  rdering_rand_par
-0000dcd0: 745d 292c 0a20 2020 2020 2020 2029 0a20  t]),.        ). 
-0000dce0: 2020 2020 2020 2063 6f6c 756d 6e73 203d         columns =
-0000dcf0: 205b 7461 626c 655f 7769 7468 5f6f 7264   [table_with_ord
-0000dd00: 6572 696e 675b 636f 6c5d 2066 6f72 2063  ering[col] for c
-0000dd10: 6f6c 2069 6e20 6f72 6967 696e 616c 5f63  ol in original_c
-0000dd20: 6f6c 756d 6e5f 6964 735d 0a20 2020 2020  olumn_ids].     
-0000dd30: 2020 2068 6964 6465 6e5f 636f 6c75 6d6e     hidden_column
-0000dd40: 7320 3d20 5b0a 2020 2020 2020 2020 2020  s = [.          
-0000dd50: 2020 7461 626c 655f 7769 7468 5f6f 7264    table_with_ord
-0000dd60: 6572 696e 675b 6f72 6465 7269 6e67 5f68  ering[ordering_h
-0000dd70: 6173 685f 7061 7274 5d2c 0a20 2020 2020  ash_part],.     
-0000dd80: 2020 2020 2020 2074 6162 6c65 5f77 6974         table_wit
-0000dd90: 685f 6f72 6465 7269 6e67 5b6f 7264 6572  h_ordering[order
-0000dda0: 696e 675f 7261 6e64 5f70 6172 745d 2c0a  ing_rand_part],.
-0000ddb0: 2020 2020 2020 2020 5d0a 2020 2020 2020          ].      
-0000ddc0: 2020 7265 7475 726e 2063 6f72 652e 4172    return core.Ar
-0000ddd0: 7261 7956 616c 7565 2e66 726f 6d5f 6962  rayValue.from_ib
-0000dde0: 6973 280a 2020 2020 2020 2020 2020 2020  is(.            
-0000ddf0: 7365 6c66 2c0a 2020 2020 2020 2020 2020  self,.          
-0000de00: 2020 7461 626c 655f 7769 7468 5f6f 7264    table_with_ord
-0000de10: 6572 696e 672c 0a20 2020 2020 2020 2020  ering,.         
-0000de20: 2020 2063 6f6c 756d 6e73 2c0a 2020 2020     columns,.    
-0000de30: 2020 2020 2020 2020 6869 6464 656e 5f6f          hidden_o
-0000de40: 7264 6572 696e 675f 636f 6c75 6d6e 733d  rdering_columns=
-0000de50: 6869 6464 656e 5f63 6f6c 756d 6e73 2c0a  hidden_columns,.
-0000de60: 2020 2020 2020 2020 2020 2020 6f72 6465              orde
-0000de70: 7269 6e67 3d6f 7264 6572 696e 672c 0a20  ring=ordering,. 
-0000de80: 2020 2020 2020 2029 0a0a 2020 2020 6465         )..    de
-0000de90: 6620 5f69 6269 735f 746f 5f74 656d 705f  f _ibis_to_temp_
-0000dea0: 7461 626c 6528 0a20 2020 2020 2020 2073  table(.        s
-0000deb0: 656c 662c 0a20 2020 2020 2020 2074 6162  elf,.        tab
-0000dec0: 6c65 3a20 6962 6973 5f74 7970 6573 2e54  le: ibis_types.T
-0000ded0: 6162 6c65 2c0a 2020 2020 2020 2020 636c  able,.        cl
-0000dee0: 7573 7465 725f 636f 6c73 3a20 4974 6572  uster_cols: Iter
-0000def0: 6162 6c65 5b73 7472 5d2c 0a20 2020 2020  able[str],.     
-0000df00: 2020 2061 7069 5f6e 616d 653a 2073 7472     api_name: str
-0000df10: 2c0a 2020 2020 2920 2d3e 2062 6967 7175  ,.    ) -> bigqu
-0000df20: 6572 792e 5461 626c 6552 6566 6572 656e  ery.TableReferen
-0000df30: 6365 3a0a 2020 2020 2020 2020 6465 7374  ce:.        dest
-0000df40: 696e 6174 696f 6e2c 205f 203d 2073 656c  ination, _ = sel
-0000df50: 662e 5f71 7565 7279 5f74 6f5f 6465 7374  f._query_to_dest
-0000df60: 696e 6174 696f 6e28 0a20 2020 2020 2020  ination(.       
-0000df70: 2020 2020 2073 656c 662e 6962 6973 5f63       self.ibis_c
-0000df80: 6c69 656e 742e 636f 6d70 696c 6528 7461  lient.compile(ta
-0000df90: 626c 6529 2c0a 2020 2020 2020 2020 2020  ble),.          
-0000dfa0: 2020 696e 6465 785f 636f 6c73 3d6c 6973    index_cols=lis
-0000dfb0: 7428 636c 7573 7465 725f 636f 6c73 292c  t(cluster_cols),
-0000dfc0: 0a20 2020 2020 2020 2020 2020 2061 7069  .            api
-0000dfd0: 5f6e 616d 653d 6170 695f 6e61 6d65 2c0a  _name=api_name,.
-0000dfe0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-0000dff0: 2020 2320 5468 6572 6520 7368 6f75 6c64    # There should
-0000e000: 2061 6c77 6179 7320 6265 2061 2064 6573   always be a des
-0000e010: 7469 6e61 7469 6f6e 2074 6162 6c65 2066  tination table f
-0000e020: 6f72 2074 6869 7320 7175 6572 7920 7479  or this query ty
-0000e030: 7065 2e0a 2020 2020 2020 2020 7265 7475  pe..        retu
-0000e040: 726e 2074 7970 696e 672e 6361 7374 2862  rn typing.cast(b
-0000e050: 6967 7175 6572 792e 5461 626c 6552 6566  igquery.TableRef
-0000e060: 6572 656e 6365 2c20 6465 7374 696e 6174  erence, destinat
-0000e070: 696f 6e29 0a0a 2020 2020 6465 6620 7265  ion)..    def re
-0000e080: 6d6f 7465 5f66 756e 6374 696f 6e28 0a20  mote_function(. 
-0000e090: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-0000e0a0: 2020 2020 2069 6e70 7574 5f74 7970 6573       input_types
-0000e0b0: 3a20 4c69 7374 5b74 7970 655d 2c0a 2020  : List[type],.  
-0000e0c0: 2020 2020 2020 6f75 7470 7574 5f74 7970        output_typ
-0000e0d0: 653a 2074 7970 652c 0a20 2020 2020 2020  e: type,.       
-0000e0e0: 2064 6174 6173 6574 3a20 4f70 7469 6f6e   dataset: Option
-0000e0f0: 616c 5b73 7472 5d20 3d20 4e6f 6e65 2c0a  al[str] = None,.
-0000e100: 2020 2020 2020 2020 6269 6771 7565 7279          bigquery
-0000e110: 5f63 6f6e 6e65 6374 696f 6e3a 204f 7074  _connection: Opt
-0000e120: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
-0000e130: 652c 0a20 2020 2020 2020 2072 6575 7365  e,.        reuse
-0000e140: 3a20 626f 6f6c 203d 2054 7275 652c 0a20  : bool = True,. 
-0000e150: 2020 2020 2020 206e 616d 653a 204f 7074         name: Opt
-0000e160: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
-0000e170: 652c 0a20 2020 2020 2020 2070 6163 6b61  e,.        packa
-0000e180: 6765 733a 204f 7074 696f 6e61 6c5b 5365  ges: Optional[Se
-0000e190: 7175 656e 6365 5b73 7472 5d5d 203d 204e  quence[str]] = N
-0000e1a0: 6f6e 652c 0a20 2020 2020 2020 2063 6c6f  one,.        clo
-0000e1b0: 7564 5f66 756e 6374 696f 6e5f 7365 7276  ud_function_serv
-0000e1c0: 6963 655f 6163 636f 756e 743a 204f 7074  ice_account: Opt
-0000e1d0: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
-0000e1e0: 652c 0a20 2020 2020 2020 2063 6c6f 7564  e,.        cloud
-0000e1f0: 5f66 756e 6374 696f 6e5f 6b6d 735f 6b65  _function_kms_ke
-0000e200: 795f 6e61 6d65 3a20 4f70 7469 6f6e 616c  y_name: Optional
-0000e210: 5b73 7472 5d20 3d20 4e6f 6e65 2c0a 2020  [str] = None,.  
-0000e220: 2020 2020 2020 636c 6f75 645f 6675 6e63        cloud_func
-0000e230: 7469 6f6e 5f64 6f63 6b65 725f 7265 706f  tion_docker_repo
-0000e240: 7369 746f 7279 3a20 4f70 7469 6f6e 616c  sitory: Optional
-0000e250: 5b73 7472 5d20 3d20 4e6f 6e65 2c0a 2020  [str] = None,.  
-0000e260: 2020 293a 0a20 2020 2020 2020 2022 2222    ):.        """
-0000e270: 4465 636f 7261 746f 7220 746f 2074 7572  Decorator to tur
-0000e280: 6e20 6120 7573 6572 2064 6566 696e 6564  n a user defined
-0000e290: 2066 756e 6374 696f 6e20 696e 746f 2061   function into a
-0000e2a0: 2042 6967 5175 6572 7920 7265 6d6f 7465   BigQuery remote
-0000e2b0: 2066 756e 6374 696f 6e2e 2043 6865 636b   function. Check
-0000e2c0: 206f 7574 0a20 2020 2020 2020 2074 6865   out.        the
-0000e2d0: 2063 6f64 6520 7361 6d70 6c65 7320 6174   code samples at
-0000e2e0: 3a20 6874 7470 733a 2f2f 636c 6f75 642e  : https://cloud.
-0000e2f0: 676f 6f67 6c65 2e63 6f6d 2f62 6967 7175  google.com/bigqu
-0000e300: 6572 792f 646f 6373 2f72 656d 6f74 652d  ery/docs/remote-
-0000e310: 6675 6e63 7469 6f6e 7323 6269 6771 7565  functions#bigque
-0000e320: 7279 2d64 6174 6166 7261 6d65 732e 0a0a  ry-dataframes...
-0000e330: 2020 2020 2020 2020 2e2e 206e 6f74 653a          .. note:
-0000e340: 3a0a 2020 2020 2020 2020 2020 2020 506c  :.            Pl
-0000e350: 6561 7365 206d 616b 6520 7375 7265 2066  ease make sure f
-0000e360: 6f6c 6c6f 7769 6e67 2069 7320 7365 7475  ollowing is setu
-0000e370: 7020 6265 666f 7265 2075 7369 6e67 2074  p before using t
-0000e380: 6869 7320 4150 493a 0a0a 2020 2020 2020  his API:..      
-0000e390: 2020 312e 2048 6176 6520 7468 6520 6265    1. Have the be
-0000e3a0: 6c6f 7720 4150 4973 2065 6e61 626c 6564  low APIs enabled
-0000e3b0: 2066 6f72 2079 6f75 7220 7072 6f6a 6563   for your projec
-0000e3c0: 743a 0a0a 2020 2020 2020 2020 2020 2020  t:..            
-0000e3d0: 2a20 4269 6751 7565 7279 2043 6f6e 6e65  * BigQuery Conne
-0000e3e0: 6374 696f 6e20 4150 490a 2020 2020 2020  ction API.      
-0000e3f0: 2020 2020 2020 2a20 436c 6f75 6420 4675        * Cloud Fu
-0000e400: 6e63 7469 6f6e 7320 4150 490a 2020 2020  nctions API.    
-0000e410: 2020 2020 2020 2020 2a20 436c 6f75 6420          * Cloud 
-0000e420: 5275 6e20 4150 490a 2020 2020 2020 2020  Run API.        
-0000e430: 2020 2020 2a20 436c 6f75 6420 4275 696c      * Cloud Buil
-0000e440: 6420 4150 490a 2020 2020 2020 2020 2020  d API.          
-0000e450: 2020 2a20 4172 7469 6661 6374 2052 6567    * Artifact Reg
-0000e460: 6973 7472 7920 4150 490a 2020 2020 2020  istry API.      
-0000e470: 2020 2020 2020 2a20 436c 6f75 6420 5265        * Cloud Re
-0000e480: 736f 7572 6365 204d 616e 6167 6572 2041  source Manager A
-0000e490: 5049 0a0a 2020 2020 2020 2020 2020 2054  PI..           T
-0000e4a0: 6869 7320 6361 6e20 6265 2064 6f6e 6520  his can be done 
-0000e4b0: 6672 6f6d 2074 6865 2063 6c6f 7564 2063  from the cloud c
-0000e4c0: 6f6e 736f 6c65 2028 6368 616e 6765 2060  onsole (change `
-0000e4d0: 5052 4f4a 4543 545f 4944 6020 746f 2079  PROJECT_ID` to y
-0000e4e0: 6f75 7273 293a 0a20 2020 2020 2020 2020  ours):.         
-0000e4f0: 2020 6874 7470 733a 2f2f 636f 6e73 6f6c    https://consol
-0000e500: 652e 636c 6f75 642e 676f 6f67 6c65 2e63  e.cloud.google.c
-0000e510: 6f6d 2f61 7069 732f 656e 6162 6c65 666c  om/apis/enablefl
-0000e520: 6f77 3f61 7069 6964 3d62 6967 7175 6572  ow?apiid=bigquer
-0000e530: 7963 6f6e 6e65 6374 696f 6e2e 676f 6f67  yconnection.goog
-0000e540: 6c65 6170 6973 2e63 6f6d 2c63 6c6f 7564  leapis.com,cloud
-0000e550: 6675 6e63 7469 6f6e 732e 676f 6f67 6c65  functions.google
-0000e560: 6170 6973 2e63 6f6d 2c72 756e 2e67 6f6f  apis.com,run.goo
-0000e570: 676c 6561 7069 732e 636f 6d2c 636c 6f75  gleapis.com,clou
-0000e580: 6462 7569 6c64 2e67 6f6f 676c 6561 7069  dbuild.googleapi
-0000e590: 732e 636f 6d2c 6172 7469 6661 6374 7265  s.com,artifactre
-0000e5a0: 6769 7374 7279 2e67 6f6f 676c 6561 7069  gistry.googleapi
-0000e5b0: 732e 636f 6d2c 636c 6f75 6472 6573 6f75  s.com,cloudresou
-0000e5c0: 7263 656d 616e 6167 6572 2e67 6f6f 676c  rcemanager.googl
-0000e5d0: 6561 7069 732e 636f 6d26 7072 6f6a 6563  eapis.com&projec
-0000e5e0: 743d 5052 4f4a 4543 545f 4944 0a0a 2020  t=PROJECT_ID..  
-0000e5f0: 2020 2020 2020 2020 204f 7220 6672 6f6d           Or from
-0000e600: 2074 6865 2067 636c 6f75 6420 434c 493a   the gcloud CLI:
-0000e610: 0a0a 2020 2020 2020 2020 2020 2060 2420  ..           `$ 
-0000e620: 6763 6c6f 7564 2073 6572 7669 6365 7320  gcloud services 
-0000e630: 656e 6162 6c65 2062 6967 7175 6572 7963  enable bigqueryc
-0000e640: 6f6e 6e65 6374 696f 6e2e 676f 6f67 6c65  onnection.google
-0000e650: 6170 6973 2e63 6f6d 2063 6c6f 7564 6675  apis.com cloudfu
-0000e660: 6e63 7469 6f6e 732e 676f 6f67 6c65 6170  nctions.googleap
-0000e670: 6973 2e63 6f6d 2072 756e 2e67 6f6f 676c  is.com run.googl
-0000e680: 6561 7069 732e 636f 6d20 636c 6f75 6462  eapis.com cloudb
-0000e690: 7569 6c64 2e67 6f6f 676c 6561 7069 732e  uild.googleapis.
-0000e6a0: 636f 6d20 6172 7469 6661 6374 7265 6769  com artifactregi
-0000e6b0: 7374 7279 2e67 6f6f 676c 6561 7069 732e  stry.googleapis.
-0000e6c0: 636f 6d20 636c 6f75 6472 6573 6f75 7263  com cloudresourc
-0000e6d0: 656d 616e 6167 6572 2e67 6f6f 676c 6561  emanager.googlea
-0000e6e0: 7069 732e 636f 6d60 0a0a 2020 2020 2020  pis.com`..      
-0000e6f0: 2020 322e 2048 6176 6520 666f 6c6c 6f77    2. Have follow
-0000e700: 696e 6720 4941 4d20 726f 6c65 7320 656e  ing IAM roles en
-0000e710: 6162 6c65 6420 666f 7220 796f 753a 0a0a  abled for you:..
-0000e720: 2020 2020 2020 2020 2020 2020 2a20 4269              * Bi
-0000e730: 6751 7565 7279 2044 6174 6120 4564 6974  gQuery Data Edit
-0000e740: 6f72 2028 726f 6c65 732f 6269 6771 7565  or (roles/bigque
-0000e750: 7279 2e64 6174 6145 6469 746f 7229 0a20  ry.dataEditor). 
-0000e760: 2020 2020 2020 2020 2020 202a 2042 6967             * Big
-0000e770: 5175 6572 7920 436f 6e6e 6563 7469 6f6e  Query Connection
-0000e780: 2041 646d 696e 2028 726f 6c65 732f 6269   Admin (roles/bi
-0000e790: 6771 7565 7279 2e63 6f6e 6e65 6374 696f  gquery.connectio
-0000e7a0: 6e41 646d 696e 290a 2020 2020 2020 2020  nAdmin).        
-0000e7b0: 2020 2020 2a20 436c 6f75 6420 4675 6e63      * Cloud Func
-0000e7c0: 7469 6f6e 7320 4465 7665 6c6f 7065 7220  tions Developer 
-0000e7d0: 2872 6f6c 6573 2f63 6c6f 7564 6675 6e63  (roles/cloudfunc
-0000e7e0: 7469 6f6e 732e 6465 7665 6c6f 7065 7229  tions.developer)
-0000e7f0: 0a20 2020 2020 2020 2020 2020 202a 2053  .            * S
-0000e800: 6572 7669 6365 2041 6363 6f75 6e74 2055  ervice Account U
-0000e810: 7365 7220 2872 6f6c 6573 2f69 616d 2e73  ser (roles/iam.s
-0000e820: 6572 7669 6365 4163 636f 756e 7455 7365  erviceAccountUse
-0000e830: 7229 206f 6e20 7468 6520 7365 7276 6963  r) on the servic
-0000e840: 6520 6163 636f 756e 7420 6050 524f 4a45  e account `PROJE
-0000e850: 4354 5f4e 554d 4245 522d 636f 6d70 7574  CT_NUMBER-comput
-0000e860: 6540 6465 7665 6c6f 7065 722e 6773 6572  e@developer.gser
-0000e870: 7669 6365 6163 636f 756e 742e 636f 6d60  viceaccount.com`
-0000e880: 0a20 2020 2020 2020 2020 2020 202a 2053  .            * S
-0000e890: 746f 7261 6765 204f 626a 6563 7420 5669  torage Object Vi
-0000e8a0: 6577 6572 2028 726f 6c65 732f 7374 6f72  ewer (roles/stor
-0000e8b0: 6167 652e 6f62 6a65 6374 5669 6577 6572  age.objectViewer
-0000e8c0: 290a 2020 2020 2020 2020 2020 2020 2a20  ).            * 
-0000e8d0: 5072 6f6a 6563 7420 4941 4d20 4164 6d69  Project IAM Admi
-0000e8e0: 6e20 2872 6f6c 6573 2f72 6573 6f75 7263  n (roles/resourc
-0000e8f0: 656d 616e 6167 6572 2e70 726f 6a65 6374  emanager.project
-0000e900: 4961 6d41 646d 696e 2920 284f 6e6c 7920  IamAdmin) (Only 
-0000e910: 7265 7175 6972 6564 2069 6620 7468 6520  required if the 
-0000e920: 6269 6771 7565 7279 2063 6f6e 6e65 6374  bigquery connect
-0000e930: 696f 6e20 6265 696e 6720 7573 6564 2069  ion being used i
-0000e940: 7320 6e6f 7420 7072 652d 6372 6561 7465  s not pre-create
-0000e950: 6420 616e 6420 6973 2063 7265 6174 6564  d and is created
-0000e960: 2064 796e 616d 6963 616c 6c79 2077 6974   dynamically wit
-0000e970: 6820 7573 6572 2063 7265 6465 6e74 6961  h user credentia
-0000e980: 6c73 2e29 0a0a 2020 2020 2020 2020 332e  ls.)..        3.
-0000e990: 2045 6974 6865 7220 7468 6520 7573 6572   Either the user
-0000e9a0: 2068 6173 2073 6574 4961 6d50 6f6c 6963   has setIamPolic
-0000e9b0: 7920 7072 6976 696c 6567 6520 6f6e 2074  y privilege on t
-0000e9c0: 6865 2070 726f 6a65 6374 2c20 6f72 2061  he project, or a
-0000e9d0: 2042 6967 5175 6572 7920 636f 6e6e 6563   BigQuery connec
-0000e9e0: 7469 6f6e 2069 7320 7072 652d 6372 6561  tion is pre-crea
-0000e9f0: 7465 6420 7769 7468 206e 6563 6573 7361  ted with necessa
-0000ea00: 7279 2049 414d 2072 6f6c 6520 7365 743a  ry IAM role set:
-0000ea10: 0a0a 2020 2020 2020 2020 2020 2020 312e  ..            1.
-0000ea20: 2054 6f20 6372 6561 7465 2061 2063 6f6e   To create a con
-0000ea30: 6e65 6374 696f 6e2c 2066 6f6c 6c6f 7720  nection, follow 
-0000ea40: 6874 7470 733a 2f2f 636c 6f75 642e 676f  https://cloud.go
-0000ea50: 6f67 6c65 2e63 6f6d 2f62 6967 7175 6572  ogle.com/bigquer
-0000ea60: 792f 646f 6373 2f72 6566 6572 656e 6365  y/docs/reference
-0000ea70: 2f73 7461 6e64 6172 642d 7371 6c2f 7265  /standard-sql/re
-0000ea80: 6d6f 7465 2d66 756e 6374 696f 6e73 2363  mote-functions#c
-0000ea90: 7265 6174 655f 615f 636f 6e6e 6563 7469  reate_a_connecti
-0000eaa0: 6f6e 0a20 2020 2020 2020 2020 2020 2032  on.            2
-0000eab0: 2e20 546f 2073 6574 2075 7020 4941 4d2c  . To set up IAM,
-0000eac0: 2066 6f6c 6c6f 7720 6874 7470 733a 2f2f   follow https://
-0000ead0: 636c 6f75 642e 676f 6f67 6c65 2e63 6f6d  cloud.google.com
-0000eae0: 2f62 6967 7175 6572 792f 646f 6373 2f72  /bigquery/docs/r
-0000eaf0: 6566 6572 656e 6365 2f73 7461 6e64 6172  eference/standar
-0000eb00: 642d 7371 6c2f 7265 6d6f 7465 2d66 756e  d-sql/remote-fun
-0000eb10: 6374 696f 6e73 2367 7261 6e74 5f70 6572  ctions#grant_per
-0000eb20: 6d69 7373 696f 6e5f 6f6e 5f66 756e 6374  mission_on_funct
-0000eb30: 696f 6e0a 0a20 2020 2020 2020 2020 2020  ion..           
-0000eb40: 2020 2020 416c 7465 726e 6174 6976 656c      Alternativel
-0000eb50: 792c 2074 6865 2049 414d 2063 6f75 6c64  y, the IAM could
-0000eb60: 2061 6c73 6f20 6265 2073 6574 7570 2076   also be setup v
-0000eb70: 6961 2074 6865 2067 636c 6f75 6420 434c  ia the gcloud CL
-0000eb80: 493a 0a0a 2020 2020 2020 2020 2020 2020  I:..            
-0000eb90: 2020 2060 2420 6763 6c6f 7564 2070 726f     `$ gcloud pro
-0000eba0: 6a65 6374 7320 6164 642d 6961 6d2d 706f  jects add-iam-po
-0000ebb0: 6c69 6379 2d62 696e 6469 6e67 2050 524f  licy-binding PRO
-0000ebc0: 4a45 4354 5f49 4420 2d2d 6d65 6d62 6572  JECT_ID --member
-0000ebd0: 3d22 7365 7276 6963 6541 6363 6f75 6e74  ="serviceAccount
-0000ebe0: 3a43 4f4e 4e45 4354 494f 4e5f 5345 5256  :CONNECTION_SERV
-0000ebf0: 4943 455f 4143 434f 554e 545f 4944 2220  ICE_ACCOUNT_ID" 
-0000ec00: 2d2d 726f 6c65 3d22 726f 6c65 732f 7275  --role="roles/ru
-0000ec10: 6e2e 696e 766f 6b65 7222 602e 0a0a 2020  n.invoker"`...  
-0000ec20: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
-0000ec30: 2020 2020 2020 2020 696e 7075 745f 7479          input_ty
-0000ec40: 7065 7320 286c 6973 7428 7479 7065 2929  pes (list(type))
-0000ec50: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000ec60: 2020 4c69 7374 206f 6620 696e 7075 7420    List of input 
-0000ec70: 6461 7461 2074 7970 6573 2069 6e20 7468  data types in th
-0000ec80: 6520 7573 6572 2064 6566 696e 6564 2066  e user defined f
-0000ec90: 756e 6374 696f 6e2e 0a20 2020 2020 2020  unction..       
-0000eca0: 2020 2020 206f 7574 7075 745f 7479 7065       output_type
-0000ecb0: 2028 7479 7065 293a 0a20 2020 2020 2020   (type):.       
-0000ecc0: 2020 2020 2020 2020 2044 6174 6120 7479           Data ty
-0000ecd0: 7065 206f 6620 7468 6520 6f75 7470 7574  pe of the output
-0000ece0: 2069 6e20 7468 6520 7573 6572 2064 6566   in the user def
-0000ecf0: 696e 6564 2066 756e 6374 696f 6e2e 0a20  ined function.. 
-0000ed00: 2020 2020 2020 2020 2020 2064 6174 6173             datas
-0000ed10: 6574 2028 7374 722c 204f 7074 696f 6e61  et (str, Optiona
-0000ed20: 6c29 3a0a 2020 2020 2020 2020 2020 2020  l):.            
-0000ed30: 2020 2020 4461 7461 7365 7420 696e 2077      Dataset in w
-0000ed40: 6869 6368 2074 6f20 6372 6561 7465 2061  hich to create a
-0000ed50: 2042 6967 5175 6572 7920 7265 6d6f 7465   BigQuery remote
-0000ed60: 2066 756e 6374 696f 6e2e 2049 7420 7368   function. It sh
-0000ed70: 6f75 6c64 2062 6520 696e 0a20 2020 2020  ould be in.     
-0000ed80: 2020 2020 2020 2020 2020 2060 3c70 726f             `<pro
-0000ed90: 6a65 6374 5f69 643e 2e3c 6461 7461 7365  ject_id>.<datase
-0000eda0: 745f 6e61 6d65 3e60 206f 7220 603c 6461  t_name>` or `<da
-0000edb0: 7461 7365 745f 6e61 6d65 3e60 2066 6f72  taset_name>` for
-0000edc0: 6d61 742e 2049 6620 7468 6973 0a20 2020  mat. If this.   
-0000edd0: 2020 2020 2020 2020 2020 2020 2070 6172               par
-0000ede0: 616d 6574 6572 2069 7320 6e6f 7420 7072  ameter is not pr
-0000edf0: 6f76 6964 6564 2074 6865 6e20 7365 7373  ovided then sess
-0000ee00: 696f 6e20 6461 7461 7365 7420 6964 2069  ion dataset id i
-0000ee10: 7320 7573 6564 2e0a 2020 2020 2020 2020  s used..        
-0000ee20: 2020 2020 6269 6771 7565 7279 5f63 6f6e      bigquery_con
-0000ee30: 6e65 6374 696f 6e20 2873 7472 2c20 4f70  nection (str, Op
-0000ee40: 7469 6f6e 616c 293a 0a20 2020 2020 2020  tional):.       
-0000ee50: 2020 2020 2020 2020 204e 616d 6520 6f66           Name of
-0000ee60: 2074 6865 2042 6967 5175 6572 7920 636f   the BigQuery co
-0000ee70: 6e6e 6563 7469 6f6e 2e20 596f 7520 7368  nnection. You sh
-0000ee80: 6f75 6c64 2065 6974 6865 7220 6861 7665  ould either have
-0000ee90: 2074 6865 0a20 2020 2020 2020 2020 2020   the.           
-0000eea0: 2020 2020 2063 6f6e 6e65 6374 696f 6e20       connection 
-0000eeb0: 616c 7265 6164 7920 6372 6561 7465 6420  already created 
-0000eec0: 696e 2074 6865 2060 6c6f 6361 7469 6f6e  in the `location
-0000eed0: 6020 796f 7520 6861 7665 2063 686f 7365  ` you have chose
-0000eee0: 6e2c 206f 720a 2020 2020 2020 2020 2020  n, or.          
-0000eef0: 2020 2020 2020 796f 7520 7368 6f75 6c64        you should
-0000ef00: 2068 6176 6520 7468 6520 5072 6f6a 6563   have the Projec
-0000ef10: 7420 4941 4d20 4164 6d69 6e20 726f 6c65  t IAM Admin role
-0000ef20: 2074 6f20 656e 6162 6c65 2074 6865 2073   to enable the s
-0000ef30: 6572 7669 6365 0a20 2020 2020 2020 2020  ervice.         
-0000ef40: 2020 2020 2020 2074 6f20 6372 6561 7465         to create
-0000ef50: 2074 6865 2063 6f6e 6e65 6374 696f 6e20   the connection 
-0000ef60: 666f 7220 796f 7520 6966 2079 6f75 206e  for you if you n
-0000ef70: 6565 6420 6974 2e20 4966 2074 6869 7320  eed it. If this 
-0000ef80: 7061 7261 6d65 7465 7220 6973 0a20 2020  parameter is.   
-0000ef90: 2020 2020 2020 2020 2020 2020 206e 6f74               not
-0000efa0: 2070 726f 7669 6465 6420 7468 656e 2074   provided then t
-0000efb0: 6865 2042 6967 5175 6572 7920 636f 6e6e  he BigQuery conn
-0000efc0: 6563 7469 6f6e 2066 726f 6d20 7468 6520  ection from the 
-0000efd0: 7365 7373 696f 6e20 6973 2075 7365 642e  session is used.
-0000efe0: 0a20 2020 2020 2020 2020 2020 2072 6575  .            reu
-0000eff0: 7365 2028 626f 6f6c 2c20 4f70 7469 6f6e  se (bool, Option
-0000f000: 616c 293a 0a20 2020 2020 2020 2020 2020  al):.           
-0000f010: 2020 2020 2052 6575 7365 2074 6865 2072       Reuse the r
-0000f020: 656d 6f74 6520 6675 6e63 7469 6f6e 2069  emote function i
-0000f030: 6620 616c 7265 6164 7920 6578 6973 7473  f already exists
-0000f040: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000f050: 2020 6054 7275 6560 2062 7920 6465 6661    `True` by defa
-0000f060: 756c 742c 2077 6869 6368 2077 696c 6c20  ult, which will 
-0000f070: 7265 7375 6c74 2069 6e20 7265 7573 696e  result in reusin
-0000f080: 6720 616e 2065 7869 7374 696e 6720 7265  g an existing re
-0000f090: 6d6f 7465 0a20 2020 2020 2020 2020 2020  mote.           
-0000f0a0: 2020 2020 2066 756e 6374 696f 6e20 616e       function an
-0000f0b0: 6420 636f 7272 6573 706f 6e64 696e 6720  d corresponding 
-0000f0c0: 636c 6f75 6420 6675 6e63 7469 6f6e 2028  cloud function (
-0000f0d0: 6966 2061 6e79 2920 7468 6174 2077 6173  if any) that was
-0000f0e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f0f0: 2070 7265 7669 6f75 736c 7920 6372 6561   previously crea
-0000f100: 7465 6420 666f 7220 7468 6520 7361 6d65  ted for the same
-0000f110: 2075 6466 2e0a 2020 2020 2020 2020 2020   udf..          
-0000f120: 2020 2020 2020 5365 7474 696e 6720 6974        Setting it
-0000f130: 2074 6f20 6046 616c 7365 6020 776f 756c   to `False` woul
-0000f140: 6420 666f 7263 6520 6372 6561 7469 6e67  d force creating
-0000f150: 2061 2075 6e69 7175 6520 7265 6d6f 7465   a unique remote
-0000f160: 2066 756e 6374 696f 6e2e 0a20 2020 2020   function..     
-0000f170: 2020 2020 2020 2020 2020 2049 6620 7468             If th
-0000f180: 6520 7265 7175 6972 6564 2072 656d 6f74  e required remot
-0000f190: 6520 6675 6e63 7469 6f6e 2064 6f65 7320  e function does 
-0000f1a0: 6e6f 7420 6578 6973 7420 7468 656e 2069  not exist then i
-0000f1b0: 7420 776f 756c 6420 6265 0a20 2020 2020  t would be.     
-0000f1c0: 2020 2020 2020 2020 2020 2063 7265 6174             creat
-0000f1d0: 6564 2069 7272 6573 7065 6374 6976 6520  ed irrespective 
-0000f1e0: 6f66 2074 6869 7320 7061 7261 6d2e 0a20  of this param.. 
-0000f1f0: 2020 2020 2020 2020 2020 206e 616d 6520             name 
-0000f200: 2873 7472 2c20 4f70 7469 6f6e 616c 293a  (str, Optional):
-0000f210: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f220: 2045 7870 6c69 6369 7420 6e61 6d65 206f   Explicit name o
-0000f230: 6620 7468 6520 7065 7273 6973 7465 6420  f the persisted 
-0000f240: 4269 6751 7565 7279 2072 656d 6f74 6520  BigQuery remote 
-0000f250: 6675 6e63 7469 6f6e 2e20 5573 6520 6974  function. Use it
-0000f260: 2077 6974 680a 2020 2020 2020 2020 2020   with.          
-0000f270: 2020 2020 2020 6361 7574 696f 6e2c 2062        caution, b
-0000f280: 6563 6175 7365 2074 776f 2075 7365 7273  ecause two users
-0000f290: 2077 6f72 6b69 6e67 2069 6e20 7468 6520   working in the 
-0000f2a0: 7361 6d65 2070 726f 6a65 6374 2061 6e64  same project and
-0000f2b0: 2064 6174 6173 6574 0a20 2020 2020 2020   dataset.       
-0000f2c0: 2020 2020 2020 2020 2063 6f75 6c64 206f           could o
-0000f2d0: 7665 7277 7269 7465 2065 6163 6820 6f74  verwrite each ot
-0000f2e0: 6865 7227 7320 7265 6d6f 7465 2066 756e  her's remote fun
-0000f2f0: 6374 696f 6e73 2069 6620 7468 6579 2075  ctions if they u
-0000f300: 7365 2074 6865 2073 616d 650a 2020 2020  se the same.    
-0000f310: 2020 2020 2020 2020 2020 2020 7065 7273              pers
-0000f320: 6973 7465 6e74 206e 616d 652e 0a20 2020  istent name..   
-0000f330: 2020 2020 2020 2020 2070 6163 6b61 6765           package
-0000f340: 7320 2873 7472 5b5d 2c20 4f70 7469 6f6e  s (str[], Option
-0000f350: 616c 293a 0a20 2020 2020 2020 2020 2020  al):.           
-0000f360: 2020 2020 2045 7870 6c69 6369 7420 6e61       Explicit na
-0000f370: 6d65 206f 6620 7468 6520 6578 7465 726e  me of the extern
-0000f380: 616c 2070 6163 6b61 6765 2064 6570 656e  al package depen
-0000f390: 6465 6e63 6965 732e 2045 6163 6820 6465  dencies. Each de
-0000f3a0: 7065 6e64 656e 6379 0a20 2020 2020 2020  pendency.       
-0000f3b0: 2020 2020 2020 2020 2069 7320 6164 6465           is adde
-0000f3c0: 6420 746f 2074 6865 2060 7265 7175 6972  d to the `requir
-0000f3d0: 656d 656e 7473 2e74 7874 6020 6173 2069  ements.txt` as i
-0000f3e0: 732c 2061 6e64 2063 616e 2062 6520 6f66  s, and can be of
-0000f3f0: 2074 6865 2066 6f72 6d0a 2020 2020 2020   the form.      
-0000f400: 2020 2020 2020 2020 2020 7375 7070 6f72            suppor
-0000f410: 7465 6420 696e 2068 7474 7073 3a2f 2f70  ted in https://p
-0000f420: 6970 2e70 7970 612e 696f 2f65 6e2f 7374  ip.pypa.io/en/st
-0000f430: 6162 6c65 2f72 6566 6572 656e 6365 2f72  able/reference/r
-0000f440: 6571 7569 7265 6d65 6e74 732d 6669 6c65  equirements-file
-0000f450: 2d66 6f72 6d61 742f 2e0a 2020 2020 2020  -format/..      
-0000f460: 2020 2020 2020 636c 6f75 645f 6675 6e63        cloud_func
-0000f470: 7469 6f6e 5f73 6572 7669 6365 5f61 6363  tion_service_acc
-0000f480: 6f75 6e74 2028 7374 722c 204f 7074 696f  ount (str, Optio
-0000f490: 6e61 6c29 3a0a 2020 2020 2020 2020 2020  nal):.          
-0000f4a0: 2020 2020 2020 5365 7276 6963 6520 6163        Service ac
-0000f4b0: 636f 756e 7420 746f 2075 7365 2066 6f72  count to use for
-0000f4c0: 2074 6865 2063 6c6f 7564 2066 756e 6374   the cloud funct
-0000f4d0: 696f 6e73 2e20 4966 206e 6f74 2070 726f  ions. If not pro
-0000f4e0: 7669 6465 640a 2020 2020 2020 2020 2020  vided.          
-0000f4f0: 2020 2020 2020 7468 656e 2074 6865 2064        then the d
-0000f500: 6566 6175 6c74 2073 6572 7669 6365 2061  efault service a
-0000f510: 6363 6f75 6e74 2077 6f75 6c64 2062 6520  ccount would be 
-0000f520: 7573 6564 2e20 5365 650a 2020 2020 2020  used. See.      
-0000f530: 2020 2020 2020 2020 2020 6874 7470 733a            https:
-0000f540: 2f2f 636c 6f75 642e 676f 6f67 6c65 2e63  //cloud.google.c
-0000f550: 6f6d 2f66 756e 6374 696f 6e73 2f64 6f63  om/functions/doc
-0000f560: 732f 7365 6375 7269 6e67 2f66 756e 6374  s/securing/funct
-0000f570: 696f 6e2d 6964 656e 7469 7479 0a20 2020  ion-identity.   
-0000f580: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-0000f590: 206d 6f72 6520 6465 7461 696c 732e 2050   more details. P
-0000f5a0: 6c65 6173 6520 6d61 6b65 2073 7572 6520  lease make sure 
-0000f5b0: 7468 6520 7365 7276 6963 6520 6163 636f  the service acco
-0000f5c0: 756e 7420 6861 7320 7468 650a 2020 2020  unt has the.    
-0000f5d0: 2020 2020 2020 2020 2020 2020 6e65 6365              nece
-0000f5e0: 7373 6172 7920 4941 4d20 7065 726d 6973  ssary IAM permis
-0000f5f0: 7369 6f6e 7320 636f 6e66 6967 7572 6564  sions configured
-0000f600: 2061 7320 6465 7363 7269 6265 6420 696e   as described in
-0000f610: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f620: 2068 7474 7073 3a2f 2f63 6c6f 7564 2e67   https://cloud.g
-0000f630: 6f6f 676c 652e 636f 6d2f 6675 6e63 7469  oogle.com/functi
-0000f640: 6f6e 732f 646f 6373 2f72 6566 6572 656e  ons/docs/referen
-0000f650: 6365 2f69 616d 2f72 6f6c 6573 2361 6464  ce/iam/roles#add
-0000f660: 6974 696f 6e61 6c2d 636f 6e66 6967 7572  itional-configur
-0000f670: 6174 696f 6e2e 0a20 2020 2020 2020 2020  ation..         
-0000f680: 2020 2063 6c6f 7564 5f66 756e 6374 696f     cloud_functio
-0000f690: 6e5f 6b6d 735f 6b65 795f 6e61 6d65 2028  n_kms_key_name (
-0000f6a0: 7374 722c 204f 7074 696f 6e61 6c29 3a0a  str, Optional):.
-0000f6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f6c0: 4375 7374 6f6d 6572 206d 616e 6167 6564  Customer managed
-0000f6d0: 2065 6e63 7279 7074 696f 6e20 6b65 7920   encryption key 
-0000f6e0: 746f 2070 726f 7465 6374 2063 6c6f 7564  to protect cloud
-0000f6f0: 2066 756e 6374 696f 6e73 2061 6e64 0a20   functions and. 
-0000f700: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0000f710: 656c 6174 6564 2064 6174 6120 6174 2072  elated data at r
-0000f720: 6573 742e 2054 6869 7320 6973 206f 6620  est. This is of 
-0000f730: 7468 6520 666f 726d 6174 0a20 2020 2020  the format.     
-0000f740: 2020 2020 2020 2020 2020 2070 726f 6a65             proje
-0000f750: 6374 732f 5052 4f4a 4543 545f 4944 2f6c  cts/PROJECT_ID/l
-0000f760: 6f63 6174 696f 6e73 2f4c 4f43 4154 494f  ocations/LOCATIO
-0000f770: 4e2f 6b65 7952 696e 6773 2f4b 4559 5249  N/keyRings/KEYRI
-0000f780: 4e47 2f63 7279 7074 6f4b 6579 732f 4b45  NG/cryptoKeys/KE
-0000f790: 592e 0a20 2020 2020 2020 2020 2020 2020  Y..             
-0000f7a0: 2020 2052 6561 6420 6874 7470 733a 2f2f     Read https://
-0000f7b0: 636c 6f75 642e 676f 6f67 6c65 2e63 6f6d  cloud.google.com
-0000f7c0: 2f66 756e 6374 696f 6e73 2f64 6f63 732f  /functions/docs/
-0000f7d0: 7365 6375 7269 6e67 2f63 6d65 6b20 666f  securing/cmek fo
-0000f7e0: 720a 2020 2020 2020 2020 2020 2020 2020  r.              
-0000f7f0: 2020 6d6f 7265 2064 6574 6169 6c73 2069    more details i
-0000f800: 6e63 6c75 6469 6e67 2067 7261 6e74 696e  ncluding grantin
-0000f810: 6720 6e65 6365 7373 6172 7920 7365 7276  g necessary serv
-0000f820: 6963 6520 6163 636f 756e 7473 0a20 2020  ice accounts.   
-0000f830: 2020 2020 2020 2020 2020 2020 2061 6363               acc
-0000f840: 6573 7320 746f 2074 6865 206b 6579 2e0a  ess to the key..
-0000f850: 2020 2020 2020 2020 2020 2020 636c 6f75              clou
-0000f860: 645f 6675 6e63 7469 6f6e 5f64 6f63 6b65  d_function_docke
-0000f870: 725f 7265 706f 7369 746f 7279 2028 7374  r_repository (st
-0000f880: 722c 204f 7074 696f 6e61 6c29 3a0a 2020  r, Optional):.  
-0000f890: 2020 2020 2020 2020 2020 2020 2020 446f                Do
-0000f8a0: 636b 6572 2072 6570 6f73 6974 6f72 7920  cker repository 
-0000f8b0: 6372 6561 7465 6420 7769 7468 2074 6865  created with the
-0000f8c0: 2073 616d 6520 656e 6372 7970 7469 6f6e   same encryption
-0000f8d0: 206b 6579 2061 730a 2020 2020 2020 2020   key as.        
-0000f8e0: 2020 2020 2020 2020 6063 6c6f 7564 5f66          `cloud_f
-0000f8f0: 756e 6374 696f 6e5f 6b6d 735f 6b65 795f  unction_kms_key_
-0000f900: 6e61 6d65 6020 746f 2073 746f 7265 2065  name` to store e
-0000f910: 6e63 7279 7074 6564 2061 7274 6966 6163  ncrypted artifac
-0000f920: 7473 0a20 2020 2020 2020 2020 2020 2020  ts.             
-0000f930: 2020 2063 7265 6174 6564 2074 6f20 7375     created to su
-0000f940: 7070 6f72 7420 7468 6520 636c 6f75 6420  pport the cloud 
-0000f950: 6675 6e63 7469 6f6e 2e20 5468 6973 2069  function. This i
-0000f960: 7320 6f66 2074 6865 2066 6f72 6d61 740a  s of the format.
-0000f970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f980: 7072 6f6a 6563 7473 2f50 524f 4a45 4354  projects/PROJECT
-0000f990: 5f49 442f 6c6f 6361 7469 6f6e 732f 4c4f  _ID/locations/LO
-0000f9a0: 4341 5449 4f4e 2f72 6570 6f73 6974 6f72  CATION/repositor
-0000f9b0: 6965 732f 5245 504f 5349 544f 5259 5f4e  ies/REPOSITORY_N
-0000f9c0: 414d 452e 0a20 2020 2020 2020 2020 2020  AME..           
-0000f9d0: 2020 2020 2046 6f72 206d 6f72 6520 6465       For more de
-0000f9e0: 7461 696c 7320 7365 650a 2020 2020 2020  tails see.      
-0000f9f0: 2020 2020 2020 2020 2020 6874 7470 733a            https:
-0000fa00: 2f2f 636c 6f75 642e 676f 6f67 6c65 2e63  //cloud.google.c
-0000fa10: 6f6d 2f66 756e 6374 696f 6e73 2f64 6f63  om/functions/doc
-0000fa20: 732f 7365 6375 7269 6e67 2f63 6d65 6b23  s/securing/cmek#
-0000fa30: 6265 666f 7265 5f79 6f75 5f62 6567 696e  before_you_begin
-0000fa40: 2e0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-0000fa50: 733a 0a20 2020 2020 2020 2020 2020 2063  s:.            c
-0000fa60: 616c 6c61 626c 653a 2041 2072 656d 6f74  allable: A remot
-0000fa70: 6520 6675 6e63 7469 6f6e 206f 626a 6563  e function objec
-0000fa80: 7420 706f 696e 7469 6e67 2074 6f20 7468  t pointing to th
-0000fa90: 6520 636c 6f75 6420 6173 7365 7473 2063  e cloud assets c
-0000faa0: 7265 6174 6564 0a20 2020 2020 2020 2020  reated.         
-0000fab0: 2020 2069 6e20 7468 6520 6261 636b 6772     in the backgr
-0000fac0: 6f75 6e64 2074 6f20 7375 7070 6f72 7420  ound to support 
-0000fad0: 7468 6520 7265 6d6f 7465 2065 7865 6375  the remote execu
-0000fae0: 7469 6f6e 2e20 5468 6520 636c 6f75 6420  tion. The cloud 
-0000faf0: 6173 7365 7473 2063 616e 2062 650a 2020  assets can be.  
-0000fb00: 2020 2020 2020 2020 2020 6c6f 6361 7465            locate
-0000fb10: 6420 7468 726f 7567 6820 7468 6520 666f  d through the fo
-0000fb20: 6c6c 6f77 696e 6720 7072 6f70 6572 7469  llowing properti
-0000fb30: 6573 2073 6574 2069 6e20 7468 6520 6f62  es set in the ob
-0000fb40: 6a65 6374 3a0a 0a20 2020 2020 2020 2020  ject:..         
-0000fb50: 2020 2060 6269 6766 7261 6d65 735f 636c     `bigframes_cl
-0000fb60: 6f75 645f 6675 6e63 7469 6f6e 6020 2d20  oud_function` - 
-0000fb70: 5468 6520 676f 6f67 6c65 2063 6c6f 7564  The google cloud
-0000fb80: 2066 756e 6374 696f 6e20 6465 706c 6f79   function deploy
-0000fb90: 6564 2066 6f72 2074 6865 2075 7365 7220  ed for the user 
-0000fba0: 6465 6669 6e65 6420 636f 6465 2e0a 0a20  defined code... 
-0000fbb0: 2020 2020 2020 2020 2020 2060 6269 6766             `bigf
-0000fbc0: 7261 6d65 735f 7265 6d6f 7465 5f66 756e  rames_remote_fun
-0000fbd0: 6374 696f 6e60 202d 2054 6865 2062 6967  ction` - The big
-0000fbe0: 7175 6572 7920 7265 6d6f 7465 2066 756e  query remote fun
-0000fbf0: 6374 696f 6e20 6361 7061 626c 6520 6f66  ction capable of
-0000fc00: 2063 616c 6c69 6e67 2069 6e74 6f20 6062   calling into `b
-0000fc10: 6967 6672 616d 6573 5f63 6c6f 7564 5f66  igframes_cloud_f
-0000fc20: 756e 6374 696f 6e60 2e0a 2020 2020 2020  unction`..      
-0000fc30: 2020 2222 220a 2020 2020 2020 2020 7265    """.        re
-0000fc40: 7475 726e 2062 6967 6672 616d 6573 5f72  turn bigframes_r
-0000fc50: 6628 0a20 2020 2020 2020 2020 2020 2069  f(.            i
-0000fc60: 6e70 7574 5f74 7970 6573 2c0a 2020 2020  nput_types,.    
-0000fc70: 2020 2020 2020 2020 6f75 7470 7574 5f74          output_t
-0000fc80: 7970 652c 0a20 2020 2020 2020 2020 2020  ype,.           
-0000fc90: 2073 6573 7369 6f6e 3d73 656c 662c 0a20   session=self,. 
-0000fca0: 2020 2020 2020 2020 2020 2064 6174 6173             datas
-0000fcb0: 6574 3d64 6174 6173 6574 2c0a 2020 2020  et=dataset,.    
-0000fcc0: 2020 2020 2020 2020 6269 6771 7565 7279          bigquery
-0000fcd0: 5f63 6f6e 6e65 6374 696f 6e3d 6269 6771  _connection=bigq
-0000fce0: 7565 7279 5f63 6f6e 6e65 6374 696f 6e2c  uery_connection,
-0000fcf0: 0a20 2020 2020 2020 2020 2020 2072 6575  .            reu
-0000fd00: 7365 3d72 6575 7365 2c0a 2020 2020 2020  se=reuse,.      
-0000fd10: 2020 2020 2020 6e61 6d65 3d6e 616d 652c        name=name,
-0000fd20: 0a20 2020 2020 2020 2020 2020 2070 6163  .            pac
-0000fd30: 6b61 6765 733d 7061 636b 6167 6573 2c0a  kages=packages,.
-0000fd40: 2020 2020 2020 2020 2020 2020 636c 6f75              clou
-0000fd50: 645f 6675 6e63 7469 6f6e 5f73 6572 7669  d_function_servi
-0000fd60: 6365 5f61 6363 6f75 6e74 3d63 6c6f 7564  ce_account=cloud
-0000fd70: 5f66 756e 6374 696f 6e5f 7365 7276 6963  _function_servic
-0000fd80: 655f 6163 636f 756e 742c 0a20 2020 2020  e_account,.     
-0000fd90: 2020 2020 2020 2063 6c6f 7564 5f66 756e         cloud_fun
-0000fda0: 6374 696f 6e5f 6b6d 735f 6b65 795f 6e61  ction_kms_key_na
-0000fdb0: 6d65 3d63 6c6f 7564 5f66 756e 6374 696f  me=cloud_functio
-0000fdc0: 6e5f 6b6d 735f 6b65 795f 6e61 6d65 2c0a  n_kms_key_name,.
-0000fdd0: 2020 2020 2020 2020 2020 2020 636c 6f75              clou
-0000fde0: 645f 6675 6e63 7469 6f6e 5f64 6f63 6b65  d_function_docke
-0000fdf0: 725f 7265 706f 7369 746f 7279 3d63 6c6f  r_repository=clo
-0000fe00: 7564 5f66 756e 6374 696f 6e5f 646f 636b  ud_function_dock
-0000fe10: 6572 5f72 6570 6f73 6974 6f72 792c 0a20  er_repository,. 
-0000fe20: 2020 2020 2020 2029 0a0a 2020 2020 6465         )..    de
-0000fe30: 6620 7265 6164 5f67 6271 5f66 756e 6374  f read_gbq_funct
-0000fe40: 696f 6e28 0a20 2020 2020 2020 2073 656c  ion(.        sel
-0000fe50: 662c 0a20 2020 2020 2020 2066 756e 6374  f,.        funct
-0000fe60: 696f 6e5f 6e61 6d65 3a20 7374 722c 0a20  ion_name: str,. 
-0000fe70: 2020 2029 3a0a 2020 2020 2020 2020 2222     ):.        ""
-0000fe80: 224c 6f61 6473 2061 2042 6967 5175 6572  "Loads a BigQuer
-0000fe90: 7920 6675 6e63 7469 6f6e 2066 726f 6d20  y function from 
-0000fea0: 4269 6751 7565 7279 2e0a 0a20 2020 2020  BigQuery...     
-0000feb0: 2020 2054 6865 6e20 6974 2063 616e 2062     Then it can b
-0000fec0: 6520 6170 706c 6965 6420 746f 2061 2044  e applied to a D
-0000fed0: 6174 6146 7261 6d65 206f 7220 5365 7269  ataFrame or Seri
-0000fee0: 6573 2e0a 0a20 2020 2020 2020 202e 2e20  es...        .. 
-0000fef0: 6e6f 7465 3a3a 0a20 2020 2020 2020 2020  note::.         
-0000ff00: 2020 2054 6865 2072 6574 7572 6e20 7479     The return ty
-0000ff10: 7065 206f 6620 7468 6520 6675 6e63 7469  pe of the functi
-0000ff20: 6f6e 206d 7573 7420 6265 2065 7870 6c69  on must be expli
-0000ff30: 6369 746c 7920 7370 6563 6966 6965 6420  citly specified 
-0000ff40: 696e 2074 6865 0a20 2020 2020 2020 2020  in the.         
-0000ff50: 2020 2066 756e 6374 696f 6e27 7320 6f72     function's or
-0000ff60: 6967 696e 616c 2064 6566 696e 6974 696f  iginal definitio
-0000ff70: 6e20 6576 656e 2069 6620 6e6f 7420 6f74  n even if not ot
-0000ff80: 6865 7277 6973 6520 7265 7175 6972 6564  herwise required
-0000ff90: 2e0a 0a20 2020 2020 2020 2042 6967 5175  ...        BigQu
-0000ffa0: 6572 7920 5574 696c 7320 7072 6f76 6964  ery Utils provid
-0000ffb0: 6573 206d 616e 7920 7075 626c 6963 2066  es many public f
-0000ffc0: 756e 6374 696f 6e73 2075 6e64 6572 2074  unctions under t
-0000ffd0: 6865 2060 6062 7175 7469 6c60 6020 7072  he ``bqutil`` pr
-0000ffe0: 6f6a 6563 7420 6f6e 2047 6f6f 676c 6520  oject on Google 
-0000fff0: 436c 6f75 6420 506c 6174 666f 726d 2070  Cloud Platform p
-00010000: 726f 6a65 6374 0a20 2020 2020 2020 2028  roject.        (
-00010010: 5365 653a 2068 7474 7073 3a2f 2f67 6974  See: https://git
-00010020: 6875 622e 636f 6d2f 476f 6f67 6c65 436c  hub.com/GoogleCl
-00010030: 6f75 6450 6c61 7466 6f72 6d2f 6269 6771  oudPlatform/bigq
-00010040: 7565 7279 2d75 7469 6c73 2f74 7265 652f  uery-utils/tree/
-00010050: 6d61 7374 6572 2f75 6466 7323 7573 696e  master/udfs#usin
-00010060: 672d 7468 652d 7564 6673 292e 0a20 2020  g-the-udfs)..   
-00010070: 2020 2020 2059 6f75 2063 616e 2063 6865       You can che
-00010080: 636b 6f75 7420 436f 6d6d 756e 6974 7920  ckout Community 
-00010090: 5544 4673 2074 6f20 7573 6520 636f 6d6d  UDFs to use comm
-000100a0: 756e 6974 792d 636f 6e74 7269 6275 7465  unity-contribute
-000100b0: 6420 6675 6e63 7469 6f6e 732e 0a20 2020  d functions..   
-000100c0: 2020 2020 2028 5365 653a 2068 7474 7073       (See: https
-000100d0: 3a2f 2f67 6974 6875 622e 636f 6d2f 476f  ://github.com/Go
-000100e0: 6f67 6c65 436c 6f75 6450 6c61 7466 6f72  ogleCloudPlatfor
-000100f0: 6d2f 6269 6771 7565 7279 2d75 7469 6c73  m/bigquery-utils
-00010100: 2f74 7265 652f 6d61 7374 6572 2f75 6466  /tree/master/udf
-00010110: 732f 636f 6d6d 756e 6974 7923 636f 6d6d  s/community#comm
-00010120: 756e 6974 792d 7564 6673 292e 0a0a 2020  unity-udfs)...  
-00010130: 2020 2020 2020 2a2a 4578 616d 706c 6573        **Examples
-00010140: 3a2a 2a0a 0a20 2020 2020 2020 2055 7365  :**..        Use
-00010150: 2074 6865 2060 6063 775f 6c6f 7765 725f   the ``cw_lower_
-00010160: 6361 7365 5f61 7363 6969 5f6f 6e6c 7960  case_ascii_only`
-00010170: 6020 6675 6e63 7469 6f6e 2066 726f 6d20  ` function from 
-00010180: 436f 6d6d 756e 6974 7920 5544 4673 2e0a  Community UDFs..
-00010190: 2020 2020 2020 2020 2868 7474 7073 3a2f          (https:/
-000101a0: 2f67 6974 6875 622e 636f 6d2f 476f 6f67  /github.com/Goog
-000101b0: 6c65 436c 6f75 6450 6c61 7466 6f72 6d2f  leCloudPlatform/
-000101c0: 6269 6771 7565 7279 2d75 7469 6c73 2f62  bigquery-utils/b
-000101d0: 6c6f 622f 6d61 7374 6572 2f75 6466 732f  lob/master/udfs/
-000101e0: 636f 6d6d 756e 6974 792f 6377 5f6c 6f77  community/cw_low
-000101f0: 6572 5f63 6173 655f 6173 6369 695f 6f6e  er_case_ascii_on
-00010200: 6c79 2e73 716c 7829 0a0a 2020 2020 2020  ly.sqlx)..      
-00010210: 2020 2020 2020 3e3e 3e20 696d 706f 7274        >>> import
-00010220: 2062 6967 6672 616d 6573 2e70 616e 6461   bigframes.panda
-00010230: 7320 6173 2062 7064 0a20 2020 2020 2020  s as bpd.       
-00010240: 2020 2020 203e 3e3e 2062 7064 2e6f 7074       >>> bpd.opt
-00010250: 696f 6e73 2e64 6973 706c 6179 2e70 726f  ions.display.pro
-00010260: 6772 6573 735f 6261 7220 3d20 4e6f 6e65  gress_bar = None
-00010270: 0a0a 2020 2020 2020 2020 2020 2020 3e3e  ..            >>
-00010280: 3e20 6466 203d 2062 7064 2e44 6174 6146  > df = bpd.DataF
-00010290: 7261 6d65 287b 2769 6427 3a20 5b31 2c20  rame({'id': [1, 
-000102a0: 322c 2033 5d2c 2027 6e61 6d65 273a 205b  2, 3], 'name': [
-000102b0: 2741 5552 c389 4c49 4527 2c20 2743 c389  'AUR..LIE', 'C..
-000102c0: 4c45 5354 494e 4527 2c20 2744 4150 484e  LESTINE', 'DAPHN
-000102d0: c389 275d 7d29 0a20 2020 2020 2020 2020  ..']}).         
-000102e0: 2020 203e 3e3e 2064 660a 2020 2020 2020     >>> df.      
-000102f0: 2020 2020 2020 2020 2069 6420 2020 2020           id     
-00010300: 2020 6e61 6d65 0a20 2020 2020 2020 2020    name.         
-00010310: 2020 2030 2020 2031 2020 2020 4155 52c3     0   1    AUR.
-00010320: 894c 4945 0a20 2020 2020 2020 2020 2020  .LIE.           
-00010330: 2031 2020 2032 2020 43c3 894c 4553 5449   1   2  C..LESTI
-00010340: 4e45 0a20 2020 2020 2020 2020 2020 2032  NE.            2
-00010350: 2020 2033 2020 2020 2044 4150 484e c389     3     DAPHN..
-00010360: 0a20 2020 2020 2020 2020 2020 203c 424c  .            <BL
-00010370: 414e 4b4c 494e 453e 0a20 2020 2020 2020  ANKLINE>.       
-00010380: 2020 2020 205b 3320 726f 7773 2078 2032       [3 rows x 2
-00010390: 2063 6f6c 756d 6e73 5d0a 0a20 2020 2020   columns]..     
-000103a0: 2020 2020 2020 203e 3e3e 2066 756e 6320         >>> func 
-000103b0: 3d20 6270 642e 7265 6164 5f67 6271 5f66  = bpd.read_gbq_f
-000103c0: 756e 6374 696f 6e28 2262 7175 7469 6c2e  unction("bqutil.
-000103d0: 666e 2e63 775f 6c6f 7765 725f 6361 7365  fn.cw_lower_case
-000103e0: 5f61 7363 6969 5f6f 6e6c 7922 290a 2020  _ascii_only").  
-000103f0: 2020 2020 2020 2020 2020 3e3e 3e20 6466            >>> df
-00010400: 3120 3d20 6466 2e61 7373 6967 6e28 6e65  1 = df.assign(ne
-00010410: 775f 6e61 6d65 3d64 665b 276e 616d 6527  w_name=df['name'
-00010420: 5d2e 6170 706c 7928 6675 6e63 2929 0a20  ].apply(func)). 
-00010430: 2020 2020 2020 2020 2020 203e 3e3e 2064             >>> d
-00010440: 6631 0a20 2020 2020 2020 2020 2020 2020  f1.             
-00010450: 2020 6964 2020 2020 2020 206e 616d 6520    id       name 
-00010460: 2020 6e65 775f 6e61 6d65 0a20 2020 2020    new_name.     
-00010470: 2020 2020 2020 2030 2020 2031 2020 2020         0   1    
-00010480: 4155 52c3 894c 4945 2020 2020 6175 72c3  AUR..LIE    aur.
-00010490: 896c 6965 0a20 2020 2020 2020 2020 2020  .lie.           
-000104a0: 2031 2020 2032 2020 43c3 894c 4553 5449   1   2  C..LESTI
-000104b0: 4e45 2020 63c3 896c 6573 7469 6e65 0a20  NE  c..lestine. 
-000104c0: 2020 2020 2020 2020 2020 2032 2020 2033             2   3
-000104d0: 2020 2020 2044 4150 484e c389 2020 2020       DAPHN..    
-000104e0: 2064 6170 686e c389 0a20 2020 2020 2020   daphn...       
-000104f0: 2020 2020 203c 424c 414e 4b4c 494e 453e       <BLANKLINE>
-00010500: 0a20 2020 2020 2020 2020 2020 205b 3320  .            [3 
-00010510: 726f 7773 2078 2033 2063 6f6c 756d 6e73  rows x 3 columns
-00010520: 5d0a 0a20 2020 2020 2020 2041 7267 733a  ]..        Args:
-00010530: 0a20 2020 2020 2020 2020 2020 2066 756e  .            fun
-00010540: 6374 696f 6e5f 6e61 6d65 2028 7374 7229  ction_name (str)
-00010550: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00010560: 2020 7468 6520 6675 6e63 7469 6f6e 2773    the function's
-00010570: 206e 616d 6520 696e 2042 6967 5175 6572   name in BigQuer
-00010580: 7920 696e 2074 6865 2066 6f72 6d61 740a  y in the format.
-00010590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000105a0: 6070 726f 6a65 6374 5f69 642e 6461 7461  `project_id.data
-000105b0: 7365 745f 6964 2e66 756e 6374 696f 6e5f  set_id.function_
-000105c0: 6e61 6d65 602c 206f 720a 2020 2020 2020  name`, or.      
-000105d0: 2020 2020 2020 2020 2020 6064 6174 6173            `datas
-000105e0: 6574 5f69 642e 6675 6e63 7469 6f6e 5f6e  et_id.function_n
-000105f0: 616d 6560 2074 6f20 6c6f 6164 2066 726f  ame` to load fro
-00010600: 6d20 7468 6520 6465 6661 756c 7420 7072  m the default pr
-00010610: 6f6a 6563 742c 206f 720a 2020 2020 2020  oject, or.      
-00010620: 2020 2020 2020 2020 2020 6066 756e 6374            `funct
-00010630: 696f 6e5f 6e61 6d65 6020 746f 206c 6f61  ion_name` to loa
-00010640: 6420 6672 6f6d 2074 6865 2064 6566 6175  d from the defau
-00010650: 6c74 2070 726f 6a65 6374 2061 6e64 2074  lt project and t
-00010660: 6865 2064 6174 6173 6574 0a20 2020 2020  he dataset.     
-00010670: 2020 2020 2020 2020 2020 2061 7373 6f63             assoc
-00010680: 6961 7465 6420 7769 7468 2074 6865 2063  iated with the c
-00010690: 7572 7265 6e74 2073 6573 7369 6f6e 2e0a  urrent session..
-000106a0: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
-000106b0: 3a0a 2020 2020 2020 2020 2020 2020 6361  :.            ca
-000106c0: 6c6c 6162 6c65 3a20 4120 6675 6e63 7469  llable: A functi
-000106d0: 6f6e 206f 626a 6563 7420 706f 696e 7469  on object pointi
-000106e0: 6e67 2074 6f20 7468 6520 4269 6751 7565  ng to the BigQue
-000106f0: 7279 2066 756e 6374 696f 6e20 7265 6164  ry function read
-00010700: 0a20 2020 2020 2020 2020 2020 2066 726f  .            fro
-00010710: 6d20 4269 6751 7565 7279 2e0a 0a20 2020  m BigQuery...   
-00010720: 2020 2020 2020 2020 2054 6865 206f 626a           The obj
-00010730: 6563 7420 6973 2073 696d 696c 6172 2074  ect is similar t
-00010740: 6f20 7468 6520 6f6e 6520 6372 6561 7465  o the one create
-00010750: 6420 6279 2074 6865 2060 7265 6d6f 7465  d by the `remote
-00010760: 5f66 756e 6374 696f 6e60 0a20 2020 2020  _function`.     
-00010770: 2020 2020 2020 2064 6563 6f72 6174 6f72         decorator
-00010780: 2c20 696e 636c 7564 696e 6720 7468 6520  , including the 
-00010790: 6062 6967 6672 616d 6573 5f72 656d 6f74  `bigframes_remot
-000107a0: 655f 6675 6e63 7469 6f6e 6020 7072 6f70  e_function` prop
-000107b0: 6572 7479 2c20 6275 740a 2020 2020 2020  erty, but.      
-000107c0: 2020 2020 2020 6e6f 7420 696e 636c 7564        not includ
-000107d0: 696e 6720 7468 6520 6062 6967 6672 616d  ing the `bigfram
-000107e0: 6573 5f63 6c6f 7564 5f66 756e 6374 696f  es_cloud_functio
-000107f0: 6e60 2070 726f 7065 7274 792e 0a20 2020  n` property..   
-00010800: 2020 2020 2022 2222 0a0a 2020 2020 2020       """..      
-00010810: 2020 7265 7475 726e 2062 6967 6672 616d    return bigfram
-00010820: 6573 5f72 6766 280a 2020 2020 2020 2020  es_rgf(.        
-00010830: 2020 2020 6675 6e63 7469 6f6e 5f6e 616d      function_nam
-00010840: 653d 6675 6e63 7469 6f6e 5f6e 616d 652c  e=function_name,
-00010850: 0a20 2020 2020 2020 2020 2020 2073 6573  .            ses
-00010860: 7369 6f6e 3d73 656c 662c 0a20 2020 2020  sion=self,.     
-00010870: 2020 2029 0a0a 2020 2020 6465 6620 5f70     )..    def _p
-00010880: 7265 7061 7265 5f71 7565 7279 5f6a 6f62  repare_query_job
-00010890: 5f63 6f6e 6669 6728 0a20 2020 2020 2020  _config(.       
-000108a0: 2073 656c 662c 0a20 2020 2020 2020 206a   self,.        j
-000108b0: 6f62 5f63 6f6e 6669 673a 204f 7074 696f  ob_config: Optio
-000108c0: 6e61 6c5b 6269 6771 7565 7279 2e51 7565  nal[bigquery.Que
-000108d0: 7279 4a6f 6243 6f6e 6669 675d 203d 204e  ryJobConfig] = N
-000108e0: 6f6e 652c 0a20 2020 2029 202d 3e20 6269  one,.    ) -> bi
-000108f0: 6771 7565 7279 2e51 7565 7279 4a6f 6243  gquery.QueryJobC
-00010900: 6f6e 6669 673a 0a20 2020 2020 2020 2069  onfig:.        i
-00010910: 6620 6a6f 625f 636f 6e66 6967 2069 7320  f job_config is 
-00010920: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00010930: 2020 6a6f 625f 636f 6e66 6967 203d 2062    job_config = b
-00010940: 6967 7175 6572 792e 5175 6572 794a 6f62  igquery.QueryJob
-00010950: 436f 6e66 6967 2829 0a20 2020 2020 2020  Config().       
-00010960: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00010970: 2020 2023 2043 7265 6174 6520 6120 636f     # Create a co
-00010980: 7079 2073 6f20 7468 6174 2077 6520 646f  py so that we do
-00010990: 6e27 7420 6d75 7461 7465 2074 6865 206f  n't mutate the o
-000109a0: 7269 6769 6e61 6c20 636f 6e66 6967 2070  riginal config p
-000109b0: 6173 7365 640a 2020 2020 2020 2020 2020  assed.          
-000109c0: 2020 6a6f 625f 636f 6e66 6967 203d 2074    job_config = t
-000109d0: 7970 696e 672e 6361 7374 280a 2020 2020  yping.cast(.    
-000109e0: 2020 2020 2020 2020 2020 2020 6269 6771              bigq
-000109f0: 7565 7279 2e51 7565 7279 4a6f 6243 6f6e  uery.QueryJobCon
-00010a00: 6669 672c 0a20 2020 2020 2020 2020 2020  fig,.           
-00010a10: 2020 2020 2062 6967 7175 6572 792e 5175       bigquery.Qu
-00010a20: 6572 794a 6f62 436f 6e66 6967 2e66 726f  eryJobConfig.fro
-00010a30: 6d5f 6170 695f 7265 7072 286a 6f62 5f63  m_api_repr(job_c
-00010a40: 6f6e 6669 672e 746f 5f61 7069 5f72 6570  onfig.to_api_rep
-00010a50: 7228 2929 2c0a 2020 2020 2020 2020 2020  r()),.          
-00010a60: 2020 290a 0a20 2020 2020 2020 2069 6620    )..        if 
-00010a70: 6269 6766 7261 6d65 732e 6f70 7469 6f6e  bigframes.option
-00010a80: 732e 636f 6d70 7574 652e 6d61 7869 6d75  s.compute.maximu
-00010a90: 6d5f 6279 7465 735f 6269 6c6c 6564 2069  m_bytes_billed i
-00010aa0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00010ab0: 2020 2020 2020 2020 6a6f 625f 636f 6e66          job_conf
-00010ac0: 6967 2e6d 6178 696d 756d 5f62 7974 6573  ig.maximum_bytes
-00010ad0: 5f62 696c 6c65 6420 3d20 280a 2020 2020  _billed = (.    
-00010ae0: 2020 2020 2020 2020 2020 2020 6269 6766              bigf
-00010af0: 7261 6d65 732e 6f70 7469 6f6e 732e 636f  rames.options.co
-00010b00: 6d70 7574 652e 6d61 7869 6d75 6d5f 6279  mpute.maximum_by
-00010b10: 7465 735f 6269 6c6c 6564 0a20 2020 2020  tes_billed.     
-00010b20: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
-00010b30: 2020 6966 2073 656c 662e 5f62 715f 6b6d    if self._bq_km
-00010b40: 735f 6b65 795f 6e61 6d65 3a0a 2020 2020  s_key_name:.    
-00010b50: 2020 2020 2020 2020 6a6f 625f 636f 6e66          job_conf
-00010b60: 6967 2e64 6573 7469 6e61 7469 6f6e 5f65  ig.destination_e
-00010b70: 6e63 7279 7074 696f 6e5f 636f 6e66 6967  ncryption_config
-00010b80: 7572 6174 696f 6e20 3d20 280a 2020 2020  uration = (.    
-00010b90: 2020 2020 2020 2020 2020 2020 6269 6771              bigq
-00010ba0: 7565 7279 2e45 6e63 7279 7074 696f 6e43  uery.EncryptionC
-00010bb0: 6f6e 6669 6775 7261 7469 6f6e 286b 6d73  onfiguration(kms
-00010bc0: 5f6b 6579 5f6e 616d 653d 7365 6c66 2e5f  _key_name=self._
-00010bd0: 6271 5f6b 6d73 5f6b 6579 5f6e 616d 6529  bq_kms_key_name)
-00010be0: 0a20 2020 2020 2020 2020 2020 2029 0a0a  .            )..
-00010bf0: 2020 2020 2020 2020 7265 7475 726e 206a          return j
-00010c00: 6f62 5f63 6f6e 6669 670a 0a20 2020 2064  ob_config..    d
-00010c10: 6566 205f 7072 6570 6172 655f 6c6f 6164  ef _prepare_load
-00010c20: 5f6a 6f62 5f63 6f6e 6669 6728 7365 6c66  _job_config(self
-00010c30: 2920 2d3e 2062 6967 7175 6572 792e 4c6f  ) -> bigquery.Lo
-00010c40: 6164 4a6f 6243 6f6e 6669 673a 0a20 2020  adJobConfig:.   
-00010c50: 2020 2020 2023 2043 7265 6174 6520 6120       # Create a 
-00010c60: 636f 7079 2073 6f20 7468 6174 2077 6520  copy so that we 
-00010c70: 646f 6e27 7420 6d75 7461 7465 2074 6865  don't mutate the
-00010c80: 206f 7269 6769 6e61 6c20 636f 6e66 6967   original config
-00010c90: 2070 6173 7365 640a 2020 2020 2020 2020   passed.        
-00010ca0: 6a6f 625f 636f 6e66 6967 203d 2062 6967  job_config = big
-00010cb0: 7175 6572 792e 4c6f 6164 4a6f 6243 6f6e  query.LoadJobCon
-00010cc0: 6669 6728 290a 0a20 2020 2020 2020 2069  fig()..        i
-00010cd0: 6620 7365 6c66 2e5f 6271 5f6b 6d73 5f6b  f self._bq_kms_k
-00010ce0: 6579 5f6e 616d 653a 0a20 2020 2020 2020  ey_name:.       
-00010cf0: 2020 2020 206a 6f62 5f63 6f6e 6669 672e       job_config.
-00010d00: 6465 7374 696e 6174 696f 6e5f 656e 6372  destination_encr
-00010d10: 7970 7469 6f6e 5f63 6f6e 6669 6775 7261  yption_configura
-00010d20: 7469 6f6e 203d 2028 0a20 2020 2020 2020  tion = (.       
-00010d30: 2020 2020 2020 2020 2062 6967 7175 6572           bigquer
-00010d40: 792e 456e 6372 7970 7469 6f6e 436f 6e66  y.EncryptionConf
-00010d50: 6967 7572 6174 696f 6e28 6b6d 735f 6b65  iguration(kms_ke
-00010d60: 795f 6e61 6d65 3d73 656c 662e 5f62 715f  y_name=self._bq_
-00010d70: 6b6d 735f 6b65 795f 6e61 6d65 290a 2020  kms_key_name).  
-00010d80: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
-00010d90: 2020 2020 2072 6574 7572 6e20 6a6f 625f       return job_
-00010da0: 636f 6e66 6967 0a0a 2020 2020 6465 6620  config..    def 
-00010db0: 5f70 7265 7061 7265 5f63 6f70 795f 6a6f  _prepare_copy_jo
-00010dc0: 625f 636f 6e66 6967 2873 656c 6629 202d  b_config(self) -
-00010dd0: 3e20 6269 6771 7565 7279 2e43 6f70 794a  > bigquery.CopyJ
-00010de0: 6f62 436f 6e66 6967 3a0a 2020 2020 2020  obConfig:.      
-00010df0: 2020 2320 4372 6561 7465 2061 2063 6f70    # Create a cop
-00010e00: 7920 736f 2074 6861 7420 7765 2064 6f6e  y so that we don
-00010e10: 2774 206d 7574 6174 6520 7468 6520 6f72  't mutate the or
-00010e20: 6967 696e 616c 2063 6f6e 6669 6720 7061  iginal config pa
-00010e30: 7373 6564 0a20 2020 2020 2020 206a 6f62  ssed.        job
-00010e40: 5f63 6f6e 6669 6720 3d20 6269 6771 7565  _config = bigque
-00010e50: 7279 2e43 6f70 794a 6f62 436f 6e66 6967  ry.CopyJobConfig
-00010e60: 2829 0a0a 2020 2020 2020 2020 6966 2073  ()..        if s
-00010e70: 656c 662e 5f62 715f 6b6d 735f 6b65 795f  elf._bq_kms_key_
-00010e80: 6e61 6d65 3a0a 2020 2020 2020 2020 2020  name:.          
-00010e90: 2020 6a6f 625f 636f 6e66 6967 2e64 6573    job_config.des
-00010ea0: 7469 6e61 7469 6f6e 5f65 6e63 7279 7074  tination_encrypt
-00010eb0: 696f 6e5f 636f 6e66 6967 7572 6174 696f  ion_configuratio
-00010ec0: 6e20 3d20 280a 2020 2020 2020 2020 2020  n = (.          
-00010ed0: 2020 2020 2020 6269 6771 7565 7279 2e45        bigquery.E
-00010ee0: 6e63 7279 7074 696f 6e43 6f6e 6669 6775  ncryptionConfigu
-00010ef0: 7261 7469 6f6e 286b 6d73 5f6b 6579 5f6e  ration(kms_key_n
-00010f00: 616d 653d 7365 6c66 2e5f 6271 5f6b 6d73  ame=self._bq_kms
-00010f10: 5f6b 6579 5f6e 616d 6529 0a20 2020 2020  _key_name).     
-00010f20: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
-00010f30: 2020 7265 7475 726e 206a 6f62 5f63 6f6e    return job_con
-00010f40: 6669 670a 0a20 2020 2064 6566 205f 7374  fig..    def _st
-00010f50: 6172 745f 7175 6572 7928 0a20 2020 2020  art_query(.     
-00010f60: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-00010f70: 2073 716c 3a20 7374 722c 0a20 2020 2020   sql: str,.     
-00010f80: 2020 206a 6f62 5f63 6f6e 6669 673a 204f     job_config: O
-00010f90: 7074 696f 6e61 6c5b 6269 6771 7565 7279  ptional[bigquery
-00010fa0: 2e6a 6f62 2e51 7565 7279 4a6f 6243 6f6e  .job.QueryJobCon
-00010fb0: 6669 675d 203d 204e 6f6e 652c 0a20 2020  fig] = None,.   
-00010fc0: 2020 2020 206d 6178 5f72 6573 756c 7473       max_results
-00010fd0: 3a20 4f70 7469 6f6e 616c 5b69 6e74 5d20  : Optional[int] 
-00010fe0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-00010ff0: 7469 6d65 6f75 743a 204f 7074 696f 6e61  timeout: Optiona
-00011000: 6c5b 666c 6f61 745d 203d 204e 6f6e 652c  l[float] = None,
-00011010: 0a20 2020 2029 202d 3e20 5475 706c 655b  .    ) -> Tuple[
-00011020: 6269 6771 7565 7279 2e74 6162 6c65 2e52  bigquery.table.R
-00011030: 6f77 4974 6572 6174 6f72 2c20 6269 6771  owIterator, bigq
-00011040: 7565 7279 2e51 7565 7279 4a6f 625d 3a0a  uery.QueryJob]:.
-00011050: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00011060: 2020 2020 5374 6172 7473 2042 6967 5175      Starts BigQu
-00011070: 6572 7920 7175 6572 7920 6a6f 6220 616e  ery query job an
-00011080: 6420 7761 6974 7320 666f 7220 7265 7375  d waits for resu
-00011090: 6c74 732e 0a20 2020 2020 2020 2022 2222  lts..        """
-000110a0: 0a20 2020 2020 2020 206a 6f62 5f63 6f6e  .        job_con
-000110b0: 6669 6720 3d20 7365 6c66 2e5f 7072 6570  fig = self._prep
-000110c0: 6172 655f 7175 6572 795f 6a6f 625f 636f  are_query_job_co
-000110d0: 6e66 6967 286a 6f62 5f63 6f6e 6669 6729  nfig(job_config)
-000110e0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000110f0: 6269 6766 7261 6d65 732e 7365 7373 696f  bigframes.sessio
-00011100: 6e2e 5f69 6f2e 6269 6771 7565 7279 2e73  n._io.bigquery.s
-00011110: 7461 7274 5f71 7565 7279 5f77 6974 685f  tart_query_with_
-00011120: 636c 6965 6e74 280a 2020 2020 2020 2020  client(.        
-00011130: 2020 2020 7365 6c66 2e62 7163 6c69 656e      self.bqclien
-00011140: 742c 2073 716c 2c20 6a6f 625f 636f 6e66  t, sql, job_conf
-00011150: 6967 2c20 6d61 785f 7265 7375 6c74 732c  ig, max_results,
-00011160: 2074 696d 656f 7574 0a20 2020 2020 2020   timeout.       
-00011170: 2029 0a0a 2020 2020 6465 6620 5f73 7461   )..    def _sta
-00011180: 7274 5f71 7565 7279 5f6d 6c5f 6464 6c28  rt_query_ml_ddl(
-00011190: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
-000111a0: 2020 2020 2020 2073 716c 3a20 7374 722c         sql: str,
-000111b0: 0a20 2020 2029 202d 3e20 5475 706c 655b  .    ) -> Tuple[
-000111c0: 6269 6771 7565 7279 2e74 6162 6c65 2e52  bigquery.table.R
-000111d0: 6f77 4974 6572 6174 6f72 2c20 6269 6771  owIterator, bigq
-000111e0: 7565 7279 2e51 7565 7279 4a6f 625d 3a0a  uery.QueryJob]:.
-000111f0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00011200: 2020 2020 5374 6172 7473 2042 6967 5175      Starts BigQu
-00011210: 6572 7920 4d4c 2044 444c 2071 7565 7279  ery ML DDL query
-00011220: 206a 6f62 2028 4352 4541 5445 204d 4f44   job (CREATE MOD
-00011230: 454c 2f41 4c54 4552 204d 4f44 454c 2f2e  EL/ALTER MODEL/.
-00011240: 2e2e 2920 616e 640a 2020 2020 2020 2020  ..) and.        
-00011250: 7761 6974 7320 666f 7220 7265 7375 6c74  waits for result
-00011260: 732e 0a20 2020 2020 2020 2022 2222 0a20  s..        """. 
-00011270: 2020 2020 2020 206a 6f62 5f63 6f6e 6669         job_confi
-00011280: 6720 3d20 7365 6c66 2e5f 7072 6570 6172  g = self._prepar
-00011290: 655f 7175 6572 795f 6a6f 625f 636f 6e66  e_query_job_conf
-000112a0: 6967 2829 0a0a 2020 2020 2020 2020 2320  ig()..        # 
-000112b0: 4251 4d4c 2065 7870 6563 7473 206b 6d73  BQML expects kms
-000112c0: 5f6b 6579 5f6e 616d 6520 7468 726f 7567  _key_name throug
-000112d0: 6820 4f50 5449 4f4e 5320 616e 6420 6e6f  h OPTIONS and no
-000112e0: 7420 7468 726f 7567 6820 6a6f 6220 636f  t through job co
-000112f0: 6e66 6967 2c0a 2020 2020 2020 2020 2320  nfig,.        # 
-00011300: 736f 2077 6520 6d75 7374 2072 6573 6574  so we must reset
-00011310: 2061 6e79 2065 6e63 7279 7074 696f 6e20   any encryption 
-00011320: 7365 7420 696e 2074 6865 206a 6f62 2063  set in the job c
-00011330: 6f6e 6669 670a 2020 2020 2020 2020 2320  onfig.        # 
-00011340: 6874 7470 733a 2f2f 636c 6f75 642e 676f  https://cloud.go
-00011350: 6f67 6c65 2e63 6f6d 2f62 6967 7175 6572  ogle.com/bigquer
-00011360: 792f 646f 6373 2f63 7573 746f 6d65 722d  y/docs/customer-
-00011370: 6d61 6e61 6765 642d 656e 6372 7970 7469  managed-encrypti
-00011380: 6f6e 2365 6e63 7279 7074 2d6d 6f64 656c  on#encrypt-model
-00011390: 0a20 2020 2020 2020 206a 6f62 5f63 6f6e  .        job_con
-000113a0: 6669 672e 6465 7374 696e 6174 696f 6e5f  fig.destination_
-000113b0: 656e 6372 7970 7469 6f6e 5f63 6f6e 6669  encryption_confi
-000113c0: 6775 7261 7469 6f6e 203d 204e 6f6e 650a  guration = None.
-000113d0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000113e0: 6269 6766 7261 6d65 732e 7365 7373 696f  bigframes.sessio
-000113f0: 6e2e 5f69 6f2e 6269 6771 7565 7279 2e73  n._io.bigquery.s
-00011400: 7461 7274 5f71 7565 7279 5f77 6974 685f  tart_query_with_
-00011410: 636c 6965 6e74 280a 2020 2020 2020 2020  client(.        
-00011420: 2020 2020 7365 6c66 2e62 7163 6c69 656e      self.bqclien
-00011430: 742c 2073 716c 2c20 6a6f 625f 636f 6e66  t, sql, job_conf
-00011440: 6967 0a20 2020 2020 2020 2029 0a0a 2020  ig.        )..  
-00011450: 2020 6465 6620 5f63 6163 6865 5f77 6974    def _cache_wit
-00011460: 685f 636c 7573 7465 725f 636f 6c73 280a  h_cluster_cols(.
-00011470: 2020 2020 2020 2020 7365 6c66 2c20 6172          self, ar
-00011480: 7261 795f 7661 6c75 653a 2063 6f72 652e  ray_value: core.
-00011490: 4172 7261 7956 616c 7565 2c20 636c 7573  ArrayValue, clus
-000114a0: 7465 725f 636f 6c73 3a20 7479 7069 6e67  ter_cols: typing
-000114b0: 2e53 6571 7565 6e63 655b 7374 725d 0a20  .Sequence[str]. 
-000114c0: 2020 2029 202d 3e20 636f 7265 2e41 7272     ) -> core.Arr
-000114d0: 6179 5661 6c75 653a 0a20 2020 2020 2020  ayValue:.       
-000114e0: 2022 2222 4578 6563 7574 6573 2074 6865   """Executes the
-000114f0: 2071 7565 7279 2061 6e64 2075 7365 7320   query and uses 
-00011500: 7468 6520 7265 7375 6c74 696e 6720 7461  the resulting ta
-00011510: 626c 6520 746f 2072 6577 7269 7465 2066  ble to rewrite f
-00011520: 7574 7572 6520 6578 6563 7574 696f 6e73  uture executions
-00011530: 2e22 2222 0a20 2020 2020 2020 2023 2054  .""".        # T
-00011540: 4f44 4f3a 2055 7365 2074 6869 7320 666f  ODO: Use this fo
-00011550: 7220 616c 6c20 6578 6563 7574 696f 6e73  r all executions
-00011560: 3f20 5072 6f62 6c65 6d20 6973 2074 6861  ? Problem is tha
-00011570: 7420 6361 6368 696e 6720 6d61 7465 7269  t caching materi
-00011580: 616c 697a 6573 2065 7874 7261 0a20 2020  alizes extra.   
-00011590: 2020 2020 2023 206f 7264 6572 696e 6720       # ordering 
-000115a0: 636f 6c75 6d6e 730a 2020 2020 2020 2020  columns.        
-000115b0: 636f 6d70 696c 6564 5f76 616c 7565 203d  compiled_value =
-000115c0: 2073 656c 662e 5f63 6f6d 7069 6c65 5f6f   self._compile_o
-000115d0: 7264 6572 6564 2861 7272 6179 5f76 616c  rdered(array_val
-000115e0: 7565 290a 0a20 2020 2020 2020 2069 6269  ue)..        ibi
-000115f0: 735f 6578 7072 203d 2063 6f6d 7069 6c65  s_expr = compile
-00011600: 645f 7661 6c75 652e 5f74 6f5f 6962 6973  d_value._to_ibis
-00011610: 5f65 7870 7228 0a20 2020 2020 2020 2020  _expr(.         
-00011620: 2020 206f 7264 6572 696e 675f 6d6f 6465     ordering_mode
-00011630: 3d22 756e 6f72 6465 7265 6422 2c20 6578  ="unordered", ex
-00011640: 706f 7365 5f68 6964 6465 6e5f 636f 6c73  pose_hidden_cols
-00011650: 3d54 7275 650a 2020 2020 2020 2020 290a  =True.        ).
-00011660: 2020 2020 2020 2020 746d 705f 7461 626c          tmp_tabl
-00011670: 6520 3d20 7365 6c66 2e5f 6962 6973 5f74  e = self._ibis_t
-00011680: 6f5f 7465 6d70 5f74 6162 6c65 280a 2020  o_temp_table(.  
-00011690: 2020 2020 2020 2020 2020 6962 6973 5f65            ibis_e
-000116a0: 7870 722c 2063 6c75 7374 6572 5f63 6f6c  xpr, cluster_col
-000116b0: 733d 636c 7573 7465 725f 636f 6c73 2c20  s=cluster_cols, 
-000116c0: 6170 695f 6e61 6d65 3d22 6361 6368 6564  api_name="cached
-000116d0: 220a 2020 2020 2020 2020 290a 2020 2020  ".        ).    
-000116e0: 2020 2020 7461 626c 655f 6578 7072 6573      table_expres
-000116f0: 7369 6f6e 203d 2073 656c 662e 6962 6973  sion = self.ibis
-00011700: 5f63 6c69 656e 742e 7461 626c 6528 0a20  _client.table(. 
-00011710: 2020 2020 2020 2020 2020 2074 6d70 5f74             tmp_t
-00011720: 6162 6c65 2e74 6162 6c65 5f69 642c 0a20  able.table_id,. 
-00011730: 2020 2020 2020 2020 2020 2073 6368 656d             schem
-00011740: 613d 746d 705f 7461 626c 652e 6461 7461  a=tmp_table.data
-00011750: 7365 745f 6964 2c0a 2020 2020 2020 2020  set_id,.        
-00011760: 2020 2020 6461 7461 6261 7365 3d74 6d70      database=tmp
-00011770: 5f74 6162 6c65 2e70 726f 6a65 6374 2c0a  _table.project,.
-00011780: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00011790: 2020 6e65 775f 636f 6c75 6d6e 7320 3d20    new_columns = 
-000117a0: 5b74 6162 6c65 5f65 7870 7265 7373 696f  [table_expressio
-000117b0: 6e5b 636f 6c75 6d6e 5d20 666f 7220 636f  n[column] for co
-000117c0: 6c75 6d6e 2069 6e20 636f 6d70 696c 6564  lumn in compiled
-000117d0: 5f76 616c 7565 2e63 6f6c 756d 6e5f 6964  _value.column_id
-000117e0: 735d 0a20 2020 2020 2020 206e 6577 5f68  s].        new_h
-000117f0: 6964 6465 6e5f 636f 6c75 6d6e 7320 3d20  idden_columns = 
-00011800: 5b0a 2020 2020 2020 2020 2020 2020 7461  [.            ta
-00011810: 626c 655f 6578 7072 6573 7369 6f6e 5b63  ble_expression[c
-00011820: 6f6c 756d 6e5d 0a20 2020 2020 2020 2020  olumn].         
-00011830: 2020 2066 6f72 2063 6f6c 756d 6e20 696e     for column in
-00011840: 2063 6f6d 7069 6c65 645f 7661 6c75 652e   compiled_value.
-00011850: 5f68 6964 6465 6e5f 6f72 6465 7269 6e67  _hidden_ordering
-00011860: 5f63 6f6c 756d 6e5f 6e61 6d65 730a 2020  _column_names.  
-00011870: 2020 2020 2020 5d0a 2020 2020 2020 2020        ].        
-00011880: 2320 544f 444f 3a20 496e 7374 6561 642c  # TODO: Instead,
-00011890: 206b 6565 7020 7365 7373 696f 6e2d 7769   keep session-wi
-000118a0: 6465 206d 6170 206f 6620 6361 6368 6564  de map of cached
-000118b0: 2072 6573 756c 7473 2061 6e64 2061 7574   results and aut
-000118c0: 6f6d 6174 6963 616c 6c79 2072 6575 7365  omatically reuse
-000118d0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000118e0: 636f 7265 2e41 7272 6179 5661 6c75 652e  core.ArrayValue.
-000118f0: 6672 6f6d 5f69 6269 7328 0a20 2020 2020  from_ibis(.     
-00011900: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-00011910: 2020 2020 2020 2020 2074 6162 6c65 5f65           table_e
-00011920: 7870 7265 7373 696f 6e2c 0a20 2020 2020  xpression,.     
-00011930: 2020 2020 2020 2063 6f6c 756d 6e73 3d6e         columns=n
-00011940: 6577 5f63 6f6c 756d 6e73 2c0a 2020 2020  ew_columns,.    
-00011950: 2020 2020 2020 2020 6869 6464 656e 5f6f          hidden_o
-00011960: 7264 6572 696e 675f 636f 6c75 6d6e 733d  rdering_columns=
-00011970: 6e65 775f 6869 6464 656e 5f63 6f6c 756d  new_hidden_colum
-00011980: 6e73 2c0a 2020 2020 2020 2020 2020 2020  ns,.            
-00011990: 6f72 6465 7269 6e67 3d63 6f6d 7069 6c65  ordering=compile
-000119a0: 645f 7661 6c75 652e 5f6f 7264 6572 696e  d_value._orderin
-000119b0: 672c 0a20 2020 2020 2020 2029 0a0a 2020  g,.        )..  
-000119c0: 2020 6465 6620 5f63 6163 6865 5f77 6974    def _cache_wit
-000119d0: 685f 6f66 6673 6574 7328 7365 6c66 2c20  h_offsets(self, 
-000119e0: 6172 7261 795f 7661 6c75 653a 2063 6f72  array_value: cor
-000119f0: 652e 4172 7261 7956 616c 7565 2920 2d3e  e.ArrayValue) ->
-00011a00: 2063 6f72 652e 4172 7261 7956 616c 7565   core.ArrayValue
-00011a10: 3a0a 2020 2020 2020 2020 2222 2245 7865  :.        """Exe
-00011a20: 6375 7465 7320 7468 6520 7175 6572 7920  cutes the query 
-00011a30: 616e 6420 7573 6573 2074 6865 2072 6573  and uses the res
-00011a40: 756c 7469 6e67 2074 6162 6c65 2074 6f20  ulting table to 
-00011a50: 7265 7772 6974 6520 6675 7475 7265 2065  rewrite future e
-00011a60: 7865 6375 7469 6f6e 732e 2222 220a 2020  xecutions.""".  
-00011a70: 2020 2020 2020 2320 544f 444f 3a20 5573        # TODO: Us
-00011a80: 6520 7468 6973 2066 6f72 2061 6c6c 2065  e this for all e
-00011a90: 7865 6375 7469 6f6e 733f 2050 726f 626c  xecutions? Probl
-00011aa0: 656d 2069 7320 7468 6174 2063 6163 6869  em is that cachi
-00011ab0: 6e67 206d 6174 6572 6961 6c69 7a65 7320  ng materializes 
-00011ac0: 6578 7472 610a 2020 2020 2020 2020 2320  extra.        # 
-00011ad0: 6f72 6465 7269 6e67 2063 6f6c 756d 6e73  ordering columns
-00011ae0: 0a20 2020 2020 2020 2063 6f6d 7069 6c65  .        compile
-00011af0: 645f 7661 6c75 6520 3d20 7365 6c66 2e5f  d_value = self._
-00011b00: 636f 6d70 696c 655f 6f72 6465 7265 6428  compile_ordered(
-00011b10: 6172 7261 795f 7661 6c75 6529 0a0a 2020  array_value)..  
-00011b20: 2020 2020 2020 6962 6973 5f65 7870 7220        ibis_expr 
-00011b30: 3d20 636f 6d70 696c 6564 5f76 616c 7565  = compiled_value
-00011b40: 2e5f 746f 5f69 6269 735f 6578 7072 280a  ._to_ibis_expr(.
-00011b50: 2020 2020 2020 2020 2020 2020 6f72 6465              orde
-00011b60: 7269 6e67 5f6d 6f64 653d 226f 6666 7365  ring_mode="offse
-00011b70: 745f 636f 6c22 2c20 6f72 6465 725f 636f  t_col", order_co
-00011b80: 6c5f 6e61 6d65 3d22 6269 6766 7261 6d65  l_name="bigframe
-00011b90: 735f 6f66 6673 6574 7322 0a20 2020 2020  s_offsets".     
-00011ba0: 2020 2029 0a20 2020 2020 2020 2074 6d70     ).        tmp
-00011bb0: 5f74 6162 6c65 203d 2073 656c 662e 5f69  _table = self._i
-00011bc0: 6269 735f 746f 5f74 656d 705f 7461 626c  bis_to_temp_tabl
-00011bd0: 6528 0a20 2020 2020 2020 2020 2020 2069  e(.            i
-00011be0: 6269 735f 6578 7072 2c20 636c 7573 7465  bis_expr, cluste
-00011bf0: 725f 636f 6c73 3d5b 2262 6967 6672 616d  r_cols=["bigfram
-00011c00: 6573 5f6f 6666 7365 7473 225d 2c20 6170  es_offsets"], ap
-00011c10: 695f 6e61 6d65 3d22 6361 6368 6564 220a  i_name="cached".
-00011c20: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00011c30: 2020 7461 626c 655f 6578 7072 6573 7369    table_expressi
-00011c40: 6f6e 203d 2073 656c 662e 6962 6973 5f63  on = self.ibis_c
-00011c50: 6c69 656e 742e 7461 626c 6528 0a20 2020  lient.table(.   
-00011c60: 2020 2020 2020 2020 2074 6d70 5f74 6162           tmp_tab
-00011c70: 6c65 2e74 6162 6c65 5f69 642c 0a20 2020  le.table_id,.   
-00011c80: 2020 2020 2020 2020 2073 6368 656d 613d           schema=
-00011c90: 746d 705f 7461 626c 652e 6461 7461 7365  tmp_table.datase
-00011ca0: 745f 6964 2c0a 2020 2020 2020 2020 2020  t_id,.          
-00011cb0: 2020 6461 7461 6261 7365 3d74 6d70 5f74    database=tmp_t
-00011cc0: 6162 6c65 2e70 726f 6a65 6374 2c0a 2020  able.project,.  
-00011cd0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00011ce0: 6e65 775f 636f 6c75 6d6e 7320 3d20 5b74  new_columns = [t
-00011cf0: 6162 6c65 5f65 7870 7265 7373 696f 6e5b  able_expression[
-00011d00: 636f 6c75 6d6e 5d20 666f 7220 636f 6c75  column] for colu
-00011d10: 6d6e 2069 6e20 636f 6d70 696c 6564 5f76  mn in compiled_v
-00011d20: 616c 7565 2e63 6f6c 756d 6e5f 6964 735d  alue.column_ids]
-00011d30: 0a20 2020 2020 2020 206e 6577 5f68 6964  .        new_hid
-00011d40: 6465 6e5f 636f 6c75 6d6e 7320 3d20 5b74  den_columns = [t
-00011d50: 6162 6c65 5f65 7870 7265 7373 696f 6e5b  able_expression[
-00011d60: 2262 6967 6672 616d 6573 5f6f 6666 7365  "bigframes_offse
-00011d70: 7473 225d 5d0a 2020 2020 2020 2020 2320  ts"]].        # 
-00011d80: 544f 444f 3a20 496e 7374 6561 642c 206b  TODO: Instead, k
-00011d90: 6565 7020 7365 7373 696f 6e2d 7769 6465  eep session-wide
-00011da0: 206d 6170 206f 6620 6361 6368 6564 2072   map of cached r
-00011db0: 6573 756c 7473 2061 6e64 2061 7574 6f6d  esults and autom
-00011dc0: 6174 6963 616c 6c79 2072 6575 7365 0a20  atically reuse. 
-00011dd0: 2020 2020 2020 2072 6574 7572 6e20 636f         return co
-00011de0: 7265 2e41 7272 6179 5661 6c75 652e 6672  re.ArrayValue.fr
-00011df0: 6f6d 5f69 6269 7328 0a20 2020 2020 2020  om_ibis(.       
-00011e00: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-00011e10: 2020 2020 2020 2074 6162 6c65 5f65 7870         table_exp
-00011e20: 7265 7373 696f 6e2c 0a20 2020 2020 2020  ression,.       
-00011e30: 2020 2020 2063 6f6c 756d 6e73 3d6e 6577       columns=new
-00011e40: 5f63 6f6c 756d 6e73 2c0a 2020 2020 2020  _columns,.      
-00011e50: 2020 2020 2020 6869 6464 656e 5f6f 7264        hidden_ord
-00011e60: 6572 696e 675f 636f 6c75 6d6e 733d 6e65  ering_columns=ne
-00011e70: 775f 6869 6464 656e 5f63 6f6c 756d 6e73  w_hidden_columns
-00011e80: 2c0a 2020 2020 2020 2020 2020 2020 6f72  ,.            or
-00011e90: 6465 7269 6e67 3d6f 7264 6572 2e45 7870  dering=order.Exp
-00011ea0: 7265 7373 696f 6e4f 7264 6572 696e 672e  ressionOrdering.
-00011eb0: 6672 6f6d 5f6f 6666 7365 745f 636f 6c28  from_offset_col(
-00011ec0: 2262 6967 6672 616d 6573 5f6f 6666 7365  "bigframes_offse
-00011ed0: 7473 2229 2c0a 2020 2020 2020 2020 290a  ts"),.        ).
-00011ee0: 0a20 2020 2064 6566 205f 7369 6d70 6c69  .    def _simpli
-00011ef0: 6679 5f77 6974 685f 6361 6368 696e 6728  fy_with_caching(
-00011f00: 7365 6c66 2c20 6172 7261 795f 7661 6c75  self, array_valu
-00011f10: 653a 2063 6f72 652e 4172 7261 7956 616c  e: core.ArrayVal
-00011f20: 7565 2920 2d3e 2063 6f72 652e 4172 7261  ue) -> core.Arra
-00011f30: 7956 616c 7565 3a0a 2020 2020 2020 2020  yValue:.        
-00011f40: 2222 2241 7474 656d 7074 7320 746f 2068  """Attempts to h
-00011f50: 616e 646c 6520 7468 6520 636f 6d70 6c65  andle the comple
-00011f60: 7869 7479 2062 7920 6361 6368 696e 6720  xity by caching 
-00011f70: 6475 706c 6963 6174 6564 2073 7562 7472  duplicated subtr
-00011f80: 6565 7320 616e 6420 6272 6561 6b69 6e67  ees and breaking
-00011f90: 2074 6865 2071 7565 7279 2069 6e74 6f20   the query into 
-00011fa0: 7069 6563 6573 2e22 2222 0a20 2020 2020  pieces.""".     
-00011fb0: 2020 2069 6620 6e6f 7420 6269 6766 7261     if not bigfra
-00011fc0: 6d65 732e 6f70 7469 6f6e 732e 636f 6d70  mes.options.comp
-00011fd0: 7574 652e 656e 6162 6c65 5f6d 756c 7469  ute.enable_multi
-00011fe0: 5f71 7565 7279 5f65 7865 6375 7469 6f6e  _query_execution
-00011ff0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00012000: 7475 726e 2061 7272 6179 5f76 616c 7565  turn array_value
-00012010: 0a20 2020 2020 2020 206e 6f64 6520 3d20  .        node = 
-00012020: 6172 7261 795f 7661 6c75 652e 6e6f 6465  array_value.node
-00012030: 0a20 2020 2020 2020 2069 6620 6e6f 6465  .        if node
-00012040: 2e70 6c61 6e6e 696e 675f 636f 6d70 6c65  .planning_comple
-00012050: 7869 7479 203c 2051 5545 5259 5f43 4f4d  xity < QUERY_COM
-00012060: 504c 4558 4954 595f 4c49 4d49 543a 0a20  PLEXITY_LIMIT:. 
-00012070: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00012080: 6e20 6172 7261 795f 7661 6c75 650a 0a20  n array_value.. 
-00012090: 2020 2020 2020 2066 6f72 205f 2069 6e20         for _ in 
-000120a0: 7261 6e67 6528 4d41 585f 5355 4254 5245  range(MAX_SUBTRE
-000120b0: 455f 4641 4354 4f52 494e 4753 293a 0a20  E_FACTORINGS):. 
-000120c0: 2020 2020 2020 2020 2020 2075 7064 6174             updat
-000120d0: 6564 203d 2073 656c 662e 5f63 6163 6865  ed = self._cache
-000120e0: 5f6d 6f73 745f 636f 6d70 6c65 785f 7375  _most_complex_su
-000120f0: 6274 7265 6528 6e6f 6465 290a 2020 2020  btree(node).    
-00012100: 2020 2020 2020 2020 6966 2075 7064 6174          if updat
-00012110: 6564 2069 7320 4e6f 6e65 3a0a 2020 2020  ed is None:.    
-00012120: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00012130: 726e 2063 6f72 652e 4172 7261 7956 616c  rn core.ArrayVal
-00012140: 7565 286e 6f64 6529 0a20 2020 2020 2020  ue(node).       
-00012150: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00012160: 2020 2020 2020 2020 2020 206e 6f64 6520             node 
-00012170: 3d20 7570 6461 7465 640a 0a20 2020 2020  = updated..     
-00012180: 2020 2072 6574 7572 6e20 636f 7265 2e41     return core.A
-00012190: 7272 6179 5661 6c75 6528 6e6f 6465 290a  rrayValue(node).
-000121a0: 0a20 2020 2064 6566 205f 6361 6368 655f  .    def _cache_
-000121b0: 6d6f 7374 5f63 6f6d 706c 6578 5f73 7562  most_complex_sub
-000121c0: 7472 6565 280a 2020 2020 2020 2020 7365  tree(.        se
-000121d0: 6c66 2c20 6e6f 6465 3a20 6e6f 6465 732e  lf, node: nodes.
-000121e0: 4269 6746 7261 6d65 4e6f 6465 0a20 2020  BigFrameNode.   
-000121f0: 2029 202d 3e20 4f70 7469 6f6e 616c 5b6e   ) -> Optional[n
-00012200: 6f64 6573 2e42 6967 4672 616d 654e 6f64  odes.BigFrameNod
-00012210: 655d 3a0a 2020 2020 2020 2020 2320 544f  e]:.        # TO
-00012220: 444f 3a20 4966 2071 7565 7279 2066 6169  DO: If query fai
-00012230: 6c73 2c20 7265 7472 7920 7769 7468 206c  ls, retry with l
-00012240: 6f77 6572 2063 6f6d 706c 6578 6974 7920  ower complexity 
-00012250: 6c69 6d69 740a 2020 2020 2020 2020 7661  limit.        va
-00012260: 6c69 645f 6361 6e64 6964 6174 6573 203d  lid_candidates =
-00012270: 2074 7261 7665 7273 616c 732e 636f 756e   traversals.coun
-00012280: 745f 636f 6d70 6c65 785f 6e6f 6465 7328  t_complex_nodes(
-00012290: 0a20 2020 2020 2020 2020 2020 206e 6f64  .            nod
-000122a0: 652c 0a20 2020 2020 2020 2020 2020 206d  e,.            m
-000122b0: 696e 5f63 6f6d 706c 6578 6974 793d 2851  in_complexity=(Q
-000122c0: 5545 5259 5f43 4f4d 504c 4558 4954 595f  UERY_COMPLEXITY_
-000122d0: 4c49 4d49 5420 2f20 3530 3029 2c0a 2020  LIMIT / 500),.  
-000122e0: 2020 2020 2020 2020 2020 6d61 785f 636f            max_co
-000122f0: 6d70 6c65 7869 7479 3d51 5545 5259 5f43  mplexity=QUERY_C
-00012300: 4f4d 504c 4558 4954 595f 4c49 4d49 542c  OMPLEXITY_LIMIT,
-00012310: 0a20 2020 2020 2020 2029 2e69 7465 6d73  .        ).items
-00012320: 2829 0a20 2020 2020 2020 2023 2048 6575  ().        # Heu
-00012330: 7269 7374 6963 3a20 7375 6274 7265 655f  ristic: subtree_
-00012340: 636f 6d70 6c65 6978 7479 202a 2028 636f  compleixty * (co
-00012350: 7069 6573 206f 6620 7375 6274 7265 6529  pies of subtree)
-00012360: 5e32 0a20 2020 2020 2020 2062 6573 745f  ^2.        best_
-00012370: 6361 6e64 6964 6174 6520 3d20 6d61 7828  candidate = max(
-00012380: 0a20 2020 2020 2020 2020 2020 2076 616c  .            val
-00012390: 6964 5f63 616e 6469 6461 7465 732c 0a20  id_candidates,. 
-000123a0: 2020 2020 2020 2020 2020 206b 6579 3d6c             key=l
-000123b0: 616d 6264 6120 693a 2069 5b30 5d2e 706c  ambda i: i[0].pl
-000123c0: 616e 6e69 6e67 5f63 6f6d 706c 6578 6974  anning_complexit
-000123d0: 7920 2b20 2869 5b31 5d20 2a2a 2032 292c  y + (i[1] ** 2),
-000123e0: 0a20 2020 2020 2020 2020 2020 2064 6566  .            def
-000123f0: 6175 6c74 3d4e 6f6e 652c 0a20 2020 2020  ault=None,.     
-00012400: 2020 2029 0a0a 2020 2020 2020 2020 6966     )..        if
-00012410: 2062 6573 745f 6361 6e64 6964 6174 6520   best_candidate 
-00012420: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-00012430: 2020 2020 2023 204e 6f20 676f 6f64 2073       # No good s
-00012440: 7562 7472 6565 7320 746f 2063 6163 6865  ubtrees to cache
-00012450: 2c20 6a75 7374 2072 6574 7572 6e20 6f72  , just return or
-00012460: 6967 696e 616c 2074 7265 650a 2020 2020  iginal tree.    
-00012470: 2020 2020 2020 2020 7265 7475 726e 204e          return N
-00012480: 6f6e 650a 0a20 2020 2020 2020 2023 2054  one..        # T
-00012490: 4f44 4f3a 2041 6464 2063 6c75 7374 6572  ODO: Add cluster
-000124a0: 696e 6720 636f 6c75 6d6e 7320 6261 7365  ing columns base
-000124b0: 6420 6f6e 2061 6363 6573 7320 7061 7474  d on access patt
-000124c0: 6572 6e73 0a20 2020 2020 2020 206d 6174  erns.        mat
-000124d0: 6572 6961 6c69 7a65 6420 3d20 7365 6c66  erialized = self
-000124e0: 2e5f 6361 6368 655f 7769 7468 5f63 6c75  ._cache_with_clu
-000124f0: 7374 6572 5f63 6f6c 7328 0a20 2020 2020  ster_cols(.     
-00012500: 2020 2020 2020 2063 6f72 652e 4172 7261         core.Arra
-00012510: 7956 616c 7565 2862 6573 745f 6361 6e64  yValue(best_cand
-00012520: 6964 6174 655b 305d 292c 205b 5d0a 2020  idate[0]), [].  
-00012530: 2020 2020 2020 292e 6e6f 6465 0a0a 2020        ).node..  
-00012540: 2020 2020 2020 7265 7475 726e 2074 7261        return tra
-00012550: 7665 7273 616c 732e 7265 706c 6163 655f  versals.replace_
-00012560: 6e6f 6465 7328 0a20 2020 2020 2020 2020  nodes(.         
-00012570: 2020 206e 6f64 652c 2074 6f5f 7265 706c     node, to_repl
-00012580: 6163 653d 6265 7374 5f63 616e 6469 6461  ace=best_candida
-00012590: 7465 5b30 5d2c 2072 6570 6c61 6365 6d65  te[0], replaceme
-000125a0: 6e65 743d 6d61 7465 7269 616c 697a 6564  net=materialized
-000125b0: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
-000125c0: 6465 6620 5f69 735f 7472 6976 6961 6c6c  def _is_triviall
-000125d0: 795f 6578 6563 7574 6162 6c65 2873 656c  y_executable(sel
-000125e0: 662c 2061 7272 6179 5f76 616c 7565 3a20  f, array_value: 
-000125f0: 636f 7265 2e41 7272 6179 5661 6c75 6529  core.ArrayValue)
-00012600: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-00012610: 2020 2020 2020 4361 6e20 7468 6520 626c        Can the bl
-00012620: 6f63 6b20 6265 2065 7661 6c75 6174 6564  ock be evaluated
-00012630: 2076 6572 7920 6368 6561 706c 793f 0a20   very cheaply?. 
-00012640: 2020 2020 2020 2049 6620 5472 7565 2c20         If True, 
-00012650: 7468 6520 6172 7261 795f 7661 6c75 6520  the array_value 
-00012660: 7072 6f62 6162 6c79 2069 7320 6e6f 7420  probably is not 
-00012670: 776f 7274 6820 6361 6368 696e 672e 0a20  worth caching.. 
-00012680: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00012690: 2020 2023 204f 6e63 6520 7265 7772 6974     # Once rewrit
-000126a0: 696e 6720 6973 2061 7661 696c 6162 6c65  ing is available
-000126b0: 2c20 7769 6c6c 2077 616e 7420 746f 2072  , will want to r
-000126c0: 6577 7269 7465 2062 6566 6f72 650a 2020  ewrite before.  
-000126d0: 2020 2020 2020 2320 6576 616c 7561 7469        # evaluati
-000126e0: 6e67 2065 7865 6375 7469 6f6e 2063 6f73  ng execution cos
-000126f0: 742e 0a20 2020 2020 2020 2072 6574 7572  t..        retur
-00012700: 6e20 7472 6176 6572 7361 6c73 2e69 735f  n traversals.is_
-00012710: 7472 6976 6961 6c6c 795f 6578 6563 7574  trivially_execut
-00012720: 6162 6c65 2861 7272 6179 5f76 616c 7565  able(array_value
-00012730: 2e6e 6f64 6529 0a0a 2020 2020 6465 6620  .node)..    def 
-00012740: 5f65 7865 6375 7465 280a 2020 2020 2020  _execute(.      
-00012750: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-00012760: 6172 7261 795f 7661 6c75 653a 2063 6f72  array_value: cor
-00012770: 652e 4172 7261 7956 616c 7565 2c0a 2020  e.ArrayValue,.  
-00012780: 2020 2020 2020 6a6f 625f 636f 6e66 6967        job_config
-00012790: 3a20 4f70 7469 6f6e 616c 5b62 6967 7175  : Optional[bigqu
-000127a0: 6572 792e 6a6f 622e 5175 6572 794a 6f62  ery.job.QueryJob
-000127b0: 436f 6e66 6967 5d20 3d20 4e6f 6e65 2c0a  Config] = None,.
-000127c0: 2020 2020 2020 2020 2a2c 0a20 2020 2020          *,.     
-000127d0: 2020 2073 6f72 7465 643a 2062 6f6f 6c20     sorted: bool 
-000127e0: 3d20 5472 7565 2c0a 2020 2020 2020 2020  = True,.        
-000127f0: 6472 795f 7275 6e3d 4661 6c73 652c 0a20  dry_run=False,. 
-00012800: 2020 2020 2020 2063 6f6c 5f69 645f 6f76         col_id_ov
-00012810: 6572 7269 6465 733a 204d 6170 7069 6e67  errides: Mapping
-00012820: 5b73 7472 2c20 7374 725d 203d 207b 7d2c  [str, str] = {},
-00012830: 0a20 2020 2029 202d 3e20 7475 706c 655b  .    ) -> tuple[
-00012840: 6269 6771 7565 7279 2e74 6162 6c65 2e52  bigquery.table.R
-00012850: 6f77 4974 6572 6174 6f72 2c20 6269 6771  owIterator, bigq
-00012860: 7565 7279 2e51 7565 7279 4a6f 625d 3a0a  uery.QueryJob]:.
-00012870: 2020 2020 2020 2020 7371 6c20 3d20 7365          sql = se
-00012880: 6c66 2e5f 746f 5f73 716c 280a 2020 2020  lf._to_sql(.    
-00012890: 2020 2020 2020 2020 6172 7261 795f 7661          array_va
-000128a0: 6c75 652c 2073 6f72 7465 643d 736f 7274  lue, sorted=sort
-000128b0: 6564 2c20 636f 6c5f 6964 5f6f 7665 7272  ed, col_id_overr
-000128c0: 6964 6573 3d63 6f6c 5f69 645f 6f76 6572  ides=col_id_over
-000128d0: 7269 6465 730a 2020 2020 2020 2020 2920  rides.        ) 
-000128e0: 2023 2074 7970 653a 6967 6e6f 7265 0a20   # type:ignore. 
-000128f0: 2020 2020 2020 2069 6620 6a6f 625f 636f         if job_co
-00012900: 6e66 6967 2069 7320 4e6f 6e65 3a0a 2020  nfig is None:.  
-00012910: 2020 2020 2020 2020 2020 6a6f 625f 636f            job_co
-00012920: 6e66 6967 203d 2062 6967 7175 6572 792e  nfig = bigquery.
-00012930: 5175 6572 794a 6f62 436f 6e66 6967 2864  QueryJobConfig(d
-00012940: 7279 5f72 756e 3d64 7279 5f72 756e 290a  ry_run=dry_run).
-00012950: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00012960: 2020 2020 2020 2020 2020 6a6f 625f 636f            job_co
-00012970: 6e66 6967 2e64 7279 5f72 756e 203d 2064  nfig.dry_run = d
-00012980: 7279 5f72 756e 0a20 2020 2020 2020 2072  ry_run.        r
-00012990: 6574 7572 6e20 7365 6c66 2e5f 7374 6172  eturn self._star
-000129a0: 745f 7175 6572 7928 0a20 2020 2020 2020  t_query(.       
-000129b0: 2020 2020 2073 716c 3d73 716c 2c0a 2020       sql=sql,.  
-000129c0: 2020 2020 2020 2020 2020 6a6f 625f 636f            job_co
-000129d0: 6e66 6967 3d6a 6f62 5f63 6f6e 6669 672c  nfig=job_config,
-000129e0: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
-000129f0: 6465 6620 5f70 6565 6b28 0a20 2020 2020  def _peek(.     
-00012a00: 2020 2073 656c 662c 2061 7272 6179 5f76     self, array_v
-00012a10: 616c 7565 3a20 636f 7265 2e41 7272 6179  alue: core.Array
-00012a20: 5661 6c75 652c 206e 5f72 6f77 733a 2069  Value, n_rows: i
-00012a30: 6e74 0a20 2020 2029 202d 3e20 7475 706c  nt.    ) -> tupl
-00012a40: 655b 6269 6771 7565 7279 2e74 6162 6c65  e[bigquery.table
-00012a50: 2e52 6f77 4974 6572 6174 6f72 2c20 6269  .RowIterator, bi
-00012a60: 6771 7565 7279 2e51 7565 7279 4a6f 625d  gquery.QueryJob]
-00012a70: 3a0a 2020 2020 2020 2020 2222 2241 2027  :.        """A '
-00012a80: 7065 656b 2720 6566 6669 6369 656e 746c  peek' efficientl
-00012a90: 7920 6163 6365 7373 6573 2061 2073 6d61  y accesses a sma
-00012aa0: 6c6c 206e 756d 6265 7220 6f66 2072 6f77  ll number of row
-00012ab0: 7320 696e 2074 6865 2064 6174 6166 7261  s in the datafra
-00012ac0: 6d65 2e22 2222 0a20 2020 2020 2020 2069  me.""".        i
-00012ad0: 6620 6e6f 7420 7472 6565 5f70 726f 7065  f not tree_prope
-00012ae0: 7274 6965 732e 7065 656b 6162 6c65 2861  rties.peekable(a
-00012af0: 7272 6179 5f76 616c 7565 2e6e 6f64 6529  rray_value.node)
-00012b00: 3a0a 2020 2020 2020 2020 2020 2020 7761  :.            wa
-00012b10: 726e 696e 6773 2e77 6172 6e28 2250 6565  rnings.warn("Pee
-00012b20: 6b69 6e67 2074 6869 7320 7661 6c75 6520  king this value 
-00012b30: 6361 6e6e 6f74 2062 6520 646f 6e65 2065  cannot be done e
-00012b40: 6666 6963 6965 6e74 6c79 2e22 290a 2020  fficiently.").  
-00012b50: 2020 2020 2020 7371 6c20 3d20 7365 6c66        sql = self
-00012b60: 2e5f 636f 6d70 696c 655f 756e 6f72 6465  ._compile_unorde
-00012b70: 7265 6428 6172 7261 795f 7661 6c75 6529  red(array_value)
-00012b80: 2e70 6565 6b5f 7371 6c28 6e5f 726f 7773  .peek_sql(n_rows
-00012b90: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-00012ba0: 2073 656c 662e 5f73 7461 7274 5f71 7565   self._start_que
-00012bb0: 7279 280a 2020 2020 2020 2020 2020 2020  ry(.            
-00012bc0: 7371 6c3d 7371 6c2c 0a20 2020 2020 2020  sql=sql,.       
-00012bd0: 2029 0a0a 2020 2020 6465 6620 5f74 6f5f   )..    def _to_
-00012be0: 7371 6c28 0a20 2020 2020 2020 2073 656c  sql(.        sel
-00012bf0: 662c 0a20 2020 2020 2020 2061 7272 6179  f,.        array
-00012c00: 5f76 616c 7565 3a20 636f 7265 2e41 7272  _value: core.Arr
-00012c10: 6179 5661 6c75 652c 0a20 2020 2020 2020  ayValue,.       
-00012c20: 206f 6666 7365 745f 636f 6c75 6d6e 3a20   offset_column: 
-00012c30: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
-00012c40: 7374 725d 203d 204e 6f6e 652c 0a20 2020  str] = None,.   
-00012c50: 2020 2020 2063 6f6c 5f69 645f 6f76 6572       col_id_over
-00012c60: 7269 6465 733a 2074 7970 696e 672e 4d61  rides: typing.Ma
-00012c70: 7070 696e 675b 7374 722c 2073 7472 5d20  pping[str, str] 
-00012c80: 3d20 7b7d 2c0a 2020 2020 2020 2020 736f  = {},.        so
-00012c90: 7274 6564 3a20 626f 6f6c 203d 2046 616c  rted: bool = Fal
-00012ca0: 7365 2c0a 2020 2020 2920 2d3e 2073 7472  se,.    ) -> str
-00012cb0: 3a0a 2020 2020 2020 2020 6966 206f 6666  :.        if off
-00012cc0: 7365 745f 636f 6c75 6d6e 3a0a 2020 2020  set_column:.    
-00012cd0: 2020 2020 2020 2020 6172 7261 795f 7661          array_va
-00012ce0: 6c75 6520 3d20 6172 7261 795f 7661 6c75  lue = array_valu
-00012cf0: 652e 7072 6f6d 6f74 655f 6f66 6673 6574  e.promote_offset
-00012d00: 7328 6f66 6673 6574 5f63 6f6c 756d 6e29  s(offset_column)
-00012d10: 0a20 2020 2020 2020 2069 6620 736f 7274  .        if sort
-00012d20: 6564 3a0a 2020 2020 2020 2020 2020 2020  ed:.            
-00012d30: 7265 7475 726e 2073 656c 662e 5f63 6f6d  return self._com
-00012d40: 7069 6c65 5f6f 7264 6572 6564 2861 7272  pile_ordered(arr
-00012d50: 6179 5f76 616c 7565 292e 746f 5f73 716c  ay_value).to_sql
-00012d60: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00012d70: 2020 636f 6c5f 6964 5f6f 7665 7272 6964    col_id_overrid
-00012d80: 6573 3d63 6f6c 5f69 645f 6f76 6572 7269  es=col_id_overri
-00012d90: 6465 732c 2073 6f72 7465 643d 5472 7565  des, sorted=True
-00012da0: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-00012db0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00012dc0: 6c66 2e5f 636f 6d70 696c 655f 756e 6f72  lf._compile_unor
-00012dd0: 6465 7265 6428 6172 7261 795f 7661 6c75  dered(array_valu
-00012de0: 6529 2e74 6f5f 7371 6c28 0a20 2020 2020  e).to_sql(.     
-00012df0: 2020 2020 2020 2063 6f6c 5f69 645f 6f76         col_id_ov
-00012e00: 6572 7269 6465 733d 636f 6c5f 6964 5f6f  errides=col_id_o
-00012e10: 7665 7272 6964 6573 0a20 2020 2020 2020  verrides.       
-00012e20: 2029 0a0a 2020 2020 6465 6620 5f63 6f6d   )..    def _com
-00012e30: 7069 6c65 5f6f 7264 6572 6564 280a 2020  pile_ordered(.  
-00012e40: 2020 2020 2020 7365 6c66 2c20 6172 7261        self, arra
-00012e50: 795f 7661 6c75 653a 2063 6f72 652e 4172  y_value: core.Ar
-00012e60: 7261 7956 616c 7565 0a20 2020 2029 202d  rayValue.    ) -
-00012e70: 3e20 6269 6766 7261 6d65 732e 636f 7265  > bigframes.core
-00012e80: 2e63 6f6d 7069 6c65 2e4f 7264 6572 6564  .compile.Ordered
-00012e90: 4952 3a0a 2020 2020 2020 2020 7265 7475  IR:.        retu
-00012ea0: 726e 2062 6967 6672 616d 6573 2e63 6f72  rn bigframes.cor
-00012eb0: 652e 636f 6d70 696c 652e 636f 6d70 696c  e.compile.compil
-00012ec0: 655f 6f72 6465 7265 645f 6972 2861 7272  e_ordered_ir(arr
-00012ed0: 6179 5f76 616c 7565 2e6e 6f64 6529 0a0a  ay_value.node)..
-00012ee0: 2020 2020 6465 6620 5f63 6f6d 7069 6c65      def _compile
-00012ef0: 5f75 6e6f 7264 6572 6564 280a 2020 2020  _unordered(.    
-00012f00: 2020 2020 7365 6c66 2c20 6172 7261 795f      self, array_
-00012f10: 7661 6c75 653a 2063 6f72 652e 4172 7261  value: core.Arra
-00012f20: 7956 616c 7565 0a20 2020 2029 202d 3e20  yValue.    ) -> 
-00012f30: 6269 6766 7261 6d65 732e 636f 7265 2e63  bigframes.core.c
-00012f40: 6f6d 7069 6c65 2e55 6e6f 7264 6572 6564  ompile.Unordered
-00012f50: 4952 3a0a 2020 2020 2020 2020 7265 7475  IR:.        retu
-00012f60: 726e 2062 6967 6672 616d 6573 2e63 6f72  rn bigframes.cor
-00012f70: 652e 636f 6d70 696c 652e 636f 6d70 696c  e.compile.compil
-00012f80: 655f 756e 6f72 6465 7265 645f 6972 2861  e_unordered_ir(a
-00012f90: 7272 6179 5f76 616c 7565 2e6e 6f64 6529  rray_value.node)
-00012fa0: 0a0a 2020 2020 6465 6620 5f67 6574 5f74  ..    def _get_t
-00012fb0: 6162 6c65 5f73 697a 6528 7365 6c66 2c20  able_size(self, 
-00012fc0: 6465 7374 696e 6174 696f 6e5f 7461 626c  destination_tabl
-00012fd0: 6529 3a0a 2020 2020 2020 2020 7461 626c  e):.        tabl
-00012fe0: 6520 3d20 7365 6c66 2e62 7163 6c69 656e  e = self.bqclien
-00012ff0: 742e 6765 745f 7461 626c 6528 6465 7374  t.get_table(dest
-00013000: 696e 6174 696f 6e5f 7461 626c 6529 0a20  ination_table). 
-00013010: 2020 2020 2020 2072 6574 7572 6e20 7461         return ta
-00013020: 626c 652e 6e75 6d5f 6279 7465 730a 0a20  ble.num_bytes.. 
-00013030: 2020 2064 6566 205f 726f 7773 5f74 6f5f     def _rows_to_
-00013040: 6461 7461 6672 616d 6528 0a20 2020 2020  dataframe(.     
-00013050: 2020 2073 656c 662c 2072 6f77 5f69 7465     self, row_ite
-00013060: 7261 746f 723a 2062 6967 7175 6572 792e  rator: bigquery.
-00013070: 7461 626c 652e 526f 7749 7465 7261 746f  table.RowIterato
-00013080: 722c 2064 7479 7065 733a 2044 6963 740a  r, dtypes: Dict.
-00013090: 2020 2020 2920 2d3e 2070 616e 6461 732e      ) -> pandas.
-000130a0: 4461 7461 4672 616d 653a 0a20 2020 2020  DataFrame:.     
-000130b0: 2020 2023 2043 616e 2069 676e 6f72 6520     # Can ignore 
-000130c0: 696e 6665 7272 6564 2064 6174 6174 7970  inferred datatyp
-000130d0: 6520 756e 7469 6c20 6474 7970 6520 656d  e until dtype em
-000130e0: 756c 6174 696f 6e20 6272 6561 6b73 2031  ulation breaks 1
-000130f0: 3a31 206d 6170 7069 6e67 2062 6574 7765  :1 mapping betwe
-00013100: 656e 2042 5120 7479 7065 7320 616e 6420  en BQ types and 
-00013110: 6269 6766 7261 6d65 7320 7479 7065 730a  bigframes types.
-00013120: 2020 2020 2020 2020 6474 7970 6573 5f66          dtypes_f
-00013130: 726f 6d5f 6271 203d 2062 6967 6672 616d  rom_bq = bigfram
-00013140: 6573 2e64 7479 7065 732e 6266 5f74 7970  es.dtypes.bf_typ
-00013150: 655f 6672 6f6d 5f74 7970 655f 6b69 6e64  e_from_type_kind
-00013160: 2872 6f77 5f69 7465 7261 746f 722e 7363  (row_iterator.sc
-00013170: 6865 6d61 290a 2020 2020 2020 2020 6172  hema).        ar
-00013180: 726f 775f 7461 626c 6520 3d20 726f 775f  row_table = row_
-00013190: 6974 6572 6174 6f72 2e74 6f5f 6172 726f  iterator.to_arro
-000131a0: 7728 290a 2020 2020 2020 2020 7265 7475  w().        retu
-000131b0: 726e 2062 6967 6672 616d 6573 2e73 6573  rn bigframes.ses
-000131c0: 7369 6f6e 2e5f 696f 2e70 616e 6461 732e  sion._io.pandas.
-000131d0: 6172 726f 775f 746f 5f70 616e 6461 7328  arrow_to_pandas(
-000131e0: 6172 726f 775f 7461 626c 652c 2064 7479  arrow_table, dty
-000131f0: 7065 735f 6672 6f6d 5f62 7129 0a0a 2020  pes_from_bq)..  
-00013200: 2020 6465 6620 5f73 7461 7274 5f67 656e    def _start_gen
-00013210: 6572 6963 5f6a 6f62 2873 656c 662c 206a  eric_job(self, j
-00013220: 6f62 3a20 666f 726d 6174 7469 6e67 5f68  ob: formatting_h
-00013230: 656c 7065 7273 2e47 656e 6572 6963 4a6f  elpers.GenericJo
-00013240: 6229 3a0a 2020 2020 2020 2020 6966 2062  b):.        if b
-00013250: 6967 6672 616d 6573 2e6f 7074 696f 6e73  igframes.options
-00013260: 2e64 6973 706c 6179 2e70 726f 6772 6573  .display.progres
-00013270: 735f 6261 7220 6973 206e 6f74 204e 6f6e  s_bar is not Non
-00013280: 653a 0a20 2020 2020 2020 2020 2020 2066  e:.            f
-00013290: 6f72 6d61 7474 696e 675f 6865 6c70 6572  ormatting_helper
-000132a0: 732e 7761 6974 5f66 6f72 5f6a 6f62 280a  s.wait_for_job(.
-000132b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000132c0: 6a6f 622c 2062 6967 6672 616d 6573 2e6f  job, bigframes.o
-000132d0: 7074 696f 6e73 2e64 6973 706c 6179 2e70  ptions.display.p
-000132e0: 726f 6772 6573 735f 6261 720a 2020 2020  rogress_bar.    
-000132f0: 2020 2020 2020 2020 2920 2023 2057 6169          )  # Wai
-00013300: 7420 666f 7220 7468 6520 6a6f 6220 746f  t for the job to
-00013310: 2063 6f6d 706c 6574 650a 2020 2020 2020   complete.      
-00013320: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00013330: 2020 2020 6a6f 622e 7265 7375 6c74 2829      job.result()
-00013340: 0a0a 0a64 6566 2063 6f6e 6e65 6374 2863  ...def connect(c
-00013350: 6f6e 7465 7874 3a20 4f70 7469 6f6e 616c  ontext: Optional
-00013360: 5b62 6967 7175 6572 795f 6f70 7469 6f6e  [bigquery_option
-00013370: 732e 4269 6751 7565 7279 4f70 7469 6f6e  s.BigQueryOption
-00013380: 735d 203d 204e 6f6e 6529 202d 3e20 5365  s] = None) -> Se
-00013390: 7373 696f 6e3a 0a20 2020 2072 6574 7572  ssion:.    retur
-000133a0: 6e20 5365 7373 696f 6e28 636f 6e74 6578  n Session(contex
-000133b0: 7429 0a0a 0a64 6566 205f 6361 6e5f 636c  t)...def _can_cl
-000133c0: 7573 7465 725f 6271 2866 6965 6c64 3a20  uster_bq(field: 
-000133d0: 6269 6771 7565 7279 2e53 6368 656d 6146  bigquery.SchemaF
-000133e0: 6965 6c64 293a 0a20 2020 2023 2068 7474  ield):.    # htt
-000133f0: 7073 3a2f 2f63 6c6f 7564 2e67 6f6f 676c  ps://cloud.googl
-00013400: 652e 636f 6d2f 6269 6771 7565 7279 2f64  e.com/bigquery/d
-00013410: 6f63 732f 636c 7573 7465 7265 642d 7461  ocs/clustered-ta
-00013420: 626c 6573 0a20 2020 2023 204e 6f74 6162  bles.    # Notab
-00013430: 6c79 2c20 666c 6f61 7420 6973 2065 7863  ly, float is exc
-00013440: 6c75 6465 640a 2020 2020 7479 7065 5f20  luded.    type_ 
-00013450: 3d20 6669 656c 642e 6669 656c 645f 7479  = field.field_ty
-00013460: 7065 0a20 2020 2072 6574 7572 6e20 7479  pe.    return ty
-00013470: 7065 5f20 696e 2028 0a20 2020 2020 2020  pe_ in (.       
-00013480: 2022 494e 5445 4745 5222 2c0a 2020 2020   "INTEGER",.    
-00013490: 2020 2020 2249 4e54 3634 222c 0a20 2020      "INT64",.   
-000134a0: 2020 2020 2022 5354 5249 4e47 222c 0a20       "STRING",. 
-000134b0: 2020 2020 2020 2022 4e55 4d45 5249 4322         "NUMERIC"
-000134c0: 2c0a 2020 2020 2020 2020 2244 4543 494d  ,.        "DECIM
-000134d0: 414c 222c 0a20 2020 2020 2020 2022 4249  AL",.        "BI
-000134e0: 474e 554d 4552 4943 222c 0a20 2020 2020  GNUMERIC",.     
-000134f0: 2020 2022 4249 4744 4543 494d 414c 222c     "BIGDECIMAL",
-00013500: 0a20 2020 2020 2020 2022 4441 5445 222c  .        "DATE",
-00013510: 0a20 2020 2020 2020 2022 4441 5445 5449  .        "DATETI
-00013520: 4d45 222c 0a20 2020 2020 2020 2022 5449  ME",.        "TI
-00013530: 4d45 5354 414d 5022 2c0a 2020 2020 2020  MESTAMP",.      
-00013540: 2020 2242 4f4f 4c22 2c0a 2020 2020 2020    "BOOL",.      
-00013550: 2020 2242 4f4f 4c45 414e 222c 0a20 2020    "BOOLEAN",.   
-00013560: 2029 0a0a 0a64 6566 205f 636f 6e76 6572   )...def _conver
-00013570: 745f 746f 5f6e 6f6e 6e75 6c6c 5f73 7472  t_to_nonnull_str
-00013580: 696e 6728 636f 6c75 6d6e 3a20 6962 6973  ing(column: ibis
-00013590: 5f74 7970 6573 2e43 6f6c 756d 6e29 202d  _types.Column) -
-000135a0: 3e20 6962 6973 5f74 7970 6573 2e53 7472  > ibis_types.Str
-000135b0: 696e 6756 616c 7565 3a0a 2020 2020 636f  ingValue:.    co
-000135c0: 6c5f 7479 7065 203d 2063 6f6c 756d 6e2e  l_type = column.
-000135d0: 7479 7065 2829 0a20 2020 2069 6620 280a  type().    if (.
-000135e0: 2020 2020 2020 2020 636f 6c5f 7479 7065          col_type
-000135f0: 2e69 735f 6e75 6d65 7269 6328 290a 2020  .is_numeric().  
-00013600: 2020 2020 2020 6f72 2063 6f6c 5f74 7970        or col_typ
-00013610: 652e 6973 5f62 6f6f 6c65 616e 2829 0a20  e.is_boolean(). 
-00013620: 2020 2020 2020 206f 7220 636f 6c5f 7479         or col_ty
-00013630: 7065 2e69 735f 6269 6e61 7279 2829 0a20  pe.is_binary(). 
-00013640: 2020 2020 2020 206f 7220 636f 6c5f 7479         or col_ty
-00013650: 7065 2e69 735f 7465 6d70 6f72 616c 2829  pe.is_temporal()
-00013660: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
-00013670: 7265 7375 6c74 203d 2063 6f6c 756d 6e2e  result = column.
-00013680: 6361 7374 2869 6269 735f 6474 7970 6573  cast(ibis_dtypes
-00013690: 2e53 7472 696e 6728 6e75 6c6c 6162 6c65  .String(nullable
-000136a0: 3d54 7275 6529 290a 2020 2020 656c 6966  =True)).    elif
-000136b0: 2063 6f6c 5f74 7970 652e 6973 5f67 656f   col_type.is_geo
-000136c0: 7370 6174 6961 6c28 293a 0a20 2020 2020  spatial():.     
-000136d0: 2020 2072 6573 756c 7420 3d20 7479 7069     result = typi
-000136e0: 6e67 2e63 6173 7428 6962 6973 5f74 7970  ng.cast(ibis_typ
-000136f0: 6573 2e47 656f 5370 6174 6961 6c43 6f6c  es.GeoSpatialCol
-00013700: 756d 6e2c 2063 6f6c 756d 6e29 2e61 735f  umn, column).as_
-00013710: 7465 7874 2829 0a20 2020 2065 6c69 6620  text().    elif 
-00013720: 636f 6c5f 7479 7065 2e69 735f 7374 7269  col_type.is_stri
-00013730: 6e67 2829 3a0a 2020 2020 2020 2020 7265  ng():.        re
-00013740: 7375 6c74 203d 2063 6f6c 756d 6e0a 2020  sult = column.  
-00013750: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00013760: 2320 544f 5f4a 534f 4e5f 5354 5249 4e47  # TO_JSON_STRING
-00013770: 2077 6f72 6b73 2077 6974 6820 616c 6c20   works with all 
-00013780: 6461 7461 2074 7970 6573 2c20 6275 7420  data types, but 
-00013790: 6973 6e27 7420 7468 6520 6d6f 7374 2065  isn't the most e
-000137a0: 6666 6963 6965 6e74 0a20 2020 2020 2020  fficient.       
-000137b0: 2023 204e 6565 6465 6420 666f 7220 4a53   # Needed for JS
-000137c0: 4f4e 2c20 5354 5255 4354 2061 6e64 2041  ON, STRUCT and A
-000137d0: 5252 4159 2064 6174 6174 7970 6573 0a20  RRAY datatypes. 
-000137e0: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
-000137f0: 7665 6e64 6f72 6564 5f69 6269 735f 6f70  vendored_ibis_op
-00013800: 732e 546f 4a73 6f6e 5374 7269 6e67 2863  s.ToJsonString(c
-00013810: 6f6c 756d 6e29 2e74 6f5f 6578 7072 2829  olumn).to_expr()
-00013820: 2020 2320 7479 7065 3a20 6967 6e6f 7265    # type: ignore
-00013830: 0a20 2020 2023 2045 7363 6170 6520 6261  .    # Escape ba
-00013840: 636b 736c 6173 6865 7320 616e 6420 7573  ckslashes and us
-00013850: 6520 6261 636b 736c 6173 6820 6173 2064  e backslash as d
-00013860: 656c 696e 6561 746f 720a 2020 2020 6573  elineator.    es
-00013870: 6361 7065 6420 3d20 7479 7069 6e67 2e63  caped = typing.c
-00013880: 6173 7428 6962 6973 5f74 7970 6573 2e53  ast(ibis_types.S
-00013890: 7472 696e 6743 6f6c 756d 6e2c 2072 6573  tringColumn, res
-000138a0: 756c 742e 6669 6c6c 6e61 2822 2229 292e  ult.fillna("")).
-000138b0: 7265 706c 6163 6528 225c 5c22 2c20 225c  replace("\\", "\
-000138c0: 5c5c 5c22 2920 2023 2074 7970 653a 2069  \\\")  # type: i
-000138d0: 676e 6f72 650a 2020 2020 7265 7475 726e  gnore.    return
-000138e0: 2074 7970 696e 672e 6361 7374 2869 6269   typing.cast(ibi
-000138f0: 735f 7479 7065 732e 5374 7269 6e67 436f  s_types.StringCo
-00013900: 6c75 6d6e 2c20 6962 6973 2e6c 6974 6572  lumn, ibis.liter
-00013910: 616c 2822 5c5c 2229 292e 636f 6e63 6174  al("\\")).concat
-00013920: 2865 7363 6170 6564 290a 0a0a 6465 6620  (escaped)...def 
-00013930: 5f74 7261 6e73 666f 726d 5f72 6561 645f  _transform_read_
-00013940: 6762 715f 636f 6e66 6967 7572 6174 696f  gbq_configuratio
-00013950: 6e28 636f 6e66 6967 7572 6174 696f 6e3a  n(configuration:
-00013960: 204f 7074 696f 6e61 6c5b 6469 6374 5d29   Optional[dict])
-00013970: 202d 3e20 6469 6374 3a0a 2020 2020 2222   -> dict:.    ""
-00013980: 220a 2020 2020 466f 7220 6261 636b 7761  ".    For backwa
-00013990: 7264 732d 636f 6d70 6174 6962 696c 6974  rds-compatibilit
-000139a0: 792c 2063 6f6e 7665 7274 2061 6e79 2070  y, convert any p
-000139b0: 7265 7669 6f75 736c 7920 636c 6965 6e74  reviously client
-000139c0: 2d73 6964 6520 6f6e 6c79 0a20 2020 2070  -side only.    p
-000139d0: 6172 616d 6574 6572 7320 7375 6368 2061  arameters such a
-000139e0: 7320 7469 6d65 6f75 744d 7320 746f 2074  s timeoutMs to t
-000139f0: 6865 2070 726f 7065 7274 7920 6e61 6d65  he property name
-00013a00: 2065 7870 6563 7465 6420 6279 2074 6865   expected by the
-00013a10: 2052 4553 5420 4150 492e 0a0a 2020 2020   REST API...    
-00013a20: 4d61 6b65 7320 6120 636f 7079 206f 6620  Makes a copy of 
-00013a30: 636f 6e66 6967 7572 6174 696f 6e20 6966  configuration if
-00013a40: 2063 6861 6e67 6573 2061 7265 206e 6565   changes are nee
-00013a50: 6465 642e 0a20 2020 2022 2222 0a0a 2020  ded..    """..  
-00013a60: 2020 6966 2063 6f6e 6669 6775 7261 7469    if configurati
-00013a70: 6f6e 2069 7320 4e6f 6e65 3a0a 2020 2020  on is None:.    
-00013a80: 2020 2020 7265 7475 726e 207b 7d0a 0a20      return {}.. 
-00013a90: 2020 2074 696d 656f 7574 5f6d 7320 3d20     timeout_ms = 
-00013aa0: 636f 6e66 6967 7572 6174 696f 6e2e 6765  configuration.ge
-00013ab0: 7428 2271 7565 7279 222c 207b 7d29 2e67  t("query", {}).g
-00013ac0: 6574 2822 7469 6d65 6f75 744d 7322 290a  et("timeoutMs").
-00013ad0: 2020 2020 6966 2074 696d 656f 7574 5f6d      if timeout_m
-00013ae0: 7320 6973 206e 6f74 204e 6f6e 653a 0a20  s is not None:. 
-00013af0: 2020 2020 2020 2023 2054 7261 6e73 666f         # Transfo
-00013b00: 726d 2074 696d 656f 7574 4d73 2074 6f20  rm timeoutMs to 
-00013b10: 616e 2061 6374 7561 6c20 7365 7276 6572  an actual server
-00013b20: 2d73 6964 6520 636f 6e66 6967 7572 6174  -side configurat
-00013b30: 696f 6e2e 0a20 2020 2020 2020 2023 2068  ion..        # h
-00013b40: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00013b50: 6d2f 676f 6f67 6c65 6170 6973 2f70 7974  m/googleapis/pyt
-00013b60: 686f 6e2d 6269 6771 7565 7279 2d70 616e  hon-bigquery-pan
-00013b70: 6461 732f 6973 7375 6573 2f34 3739 0a20  das/issues/479. 
-00013b80: 2020 2020 2020 2063 6f6e 6669 6775 7261         configura
-00013b90: 7469 6f6e 203d 2063 6f70 792e 6465 6570  tion = copy.deep
-00013ba0: 636f 7079 2863 6f6e 6669 6775 7261 7469  copy(configurati
-00013bb0: 6f6e 290a 2020 2020 2020 2020 6465 6c20  on).        del 
-00013bc0: 636f 6e66 6967 7572 6174 696f 6e5b 2271  configuration["q
-00013bd0: 7565 7279 225d 5b22 7469 6d65 6f75 744d  uery"]["timeoutM
-00013be0: 7322 5d0a 2020 2020 2020 2020 636f 6e66  s"].        conf
-00013bf0: 6967 7572 6174 696f 6e5b 226a 6f62 5469  iguration["jobTi
-00013c00: 6d65 6f75 744d 7322 5d20 3d20 7469 6d65  meoutMs"] = time
-00013c10: 6f75 745f 6d73 0a0a 2020 2020 7265 7475  out_ms..    retu
-00013c20: 726e 2063 6f6e 6669 6775 7261 7469 6f6e  rn configuration
-00013c30: 0a                                       .
+0000d0b0: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
+0000d0c0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+0000d0d0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+0000d0e0: 616e 6461 735f 6466 203d 2070 616e 6461  andas_df = panda
+0000d0f0: 732e 7265 6164 5f6a 736f 6e28 2020 2320  s.read_json(  # 
+0000d100: 7479 7065 3a20 6967 6e6f 7265 0a20 2020  type: ignore.   
+0000d110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d120: 2070 6174 685f 6f72 5f62 7566 2c0a 2020   path_or_buf,.  
+0000d130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d140: 2020 6f72 6965 6e74 3d6f 7269 656e 742c    orient=orient,
+0000d150: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d160: 2020 2020 2064 7479 7065 3d64 7479 7065       dtype=dtype
+0000d170: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000d180: 2020 2020 2020 656e 636f 6469 6e67 3d65        encoding=e
+0000d190: 6e63 6f64 696e 672c 0a20 2020 2020 2020  ncoding,.       
+0000d1a0: 2020 2020 2020 2020 2020 2020 206c 696e               lin
+0000d1b0: 6573 3d6c 696e 6573 2c0a 2020 2020 2020  es=lines,.      
+0000d1c0: 2020 2020 2020 2020 2020 2020 2020 656e                en
+0000d1d0: 6769 6e65 3d65 6e67 696e 652c 0a20 2020  gine=engine,.   
+0000d1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d1f0: 202a 2a6b 7761 7267 732c 0a20 2020 2020   **kwargs,.     
+0000d200: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+0000d210: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0000d220: 7365 6c66 2e5f 7265 6164 5f70 616e 6461  self._read_panda
+0000d230: 7328 7061 6e64 6173 5f64 662c 2022 7265  s(pandas_df, "re
+0000d240: 6164 5f6a 736f 6e22 290a 0a20 2020 2064  ad_json")..    d
+0000d250: 6566 205f 6368 6563 6b5f 6669 6c65 5f73  ef _check_file_s
+0000d260: 697a 6528 7365 6c66 2c20 6669 6c65 7061  ize(self, filepa
+0000d270: 7468 3a20 7374 7229 3a0a 2020 2020 2020  th: str):.      
+0000d280: 2020 6d61 785f 7369 7a65 203d 2031 3032    max_size = 102
+0000d290: 3420 2a20 3130 3234 202a 2031 3032 3420  4 * 1024 * 1024 
+0000d2a0: 2023 2031 2047 4220 696e 2062 7974 6573   # 1 GB in bytes
+0000d2b0: 0a20 2020 2020 2020 2069 6620 6669 6c65  .        if file
+0000d2c0: 7061 7468 2e73 7461 7274 7377 6974 6828  path.startswith(
+0000d2d0: 2267 733a 2f2f 2229 3a20 2023 2047 4353  "gs://"):  # GCS
+0000d2e0: 2066 696c 6520 7061 7468 0a20 2020 2020   file path.     
+0000d2f0: 2020 2020 2020 2063 6c69 656e 7420 3d20         client = 
+0000d300: 7374 6f72 6167 652e 436c 6965 6e74 2829  storage.Client()
+0000d310: 0a20 2020 2020 2020 2020 2020 2062 7563  .            buc
+0000d320: 6b65 745f 6e61 6d65 2c20 626c 6f62 5f6e  ket_name, blob_n
+0000d330: 616d 6520 3d20 6669 6c65 7061 7468 2e73  ame = filepath.s
+0000d340: 706c 6974 2822 2f22 2c20 3329 5b32 3a5d  plit("/", 3)[2:]
+0000d350: 0a20 2020 2020 2020 2020 2020 2062 7563  .            buc
+0000d360: 6b65 7420 3d20 636c 6965 6e74 2e62 7563  ket = client.buc
+0000d370: 6b65 7428 6275 636b 6574 5f6e 616d 6529  ket(bucket_name)
+0000d380: 0a20 2020 2020 2020 2020 2020 2062 6c6f  .            blo
+0000d390: 6220 3d20 6275 636b 6574 2e62 6c6f 6228  b = bucket.blob(
+0000d3a0: 626c 6f62 5f6e 616d 6529 0a20 2020 2020  blob_name).     
+0000d3b0: 2020 2020 2020 2062 6c6f 622e 7265 6c6f         blob.relo
+0000d3c0: 6164 2829 0a20 2020 2020 2020 2020 2020  ad().           
+0000d3d0: 2066 696c 655f 7369 7a65 203d 2062 6c6f   file_size = blo
+0000d3e0: 622e 7369 7a65 0a20 2020 2020 2020 2065  b.size.        e
+0000d3f0: 6c73 653a 2020 2320 6c6f 6361 6c20 6669  lse:  # local fi
+0000d400: 6c65 2070 6174 680a 2020 2020 2020 2020  le path.        
+0000d410: 2020 2020 6669 6c65 5f73 697a 6520 3d20      file_size = 
+0000d420: 6f73 2e70 6174 682e 6765 7473 697a 6528  os.path.getsize(
+0000d430: 6669 6c65 7061 7468 290a 0a20 2020 2020  filepath)..     
+0000d440: 2020 2069 6620 6669 6c65 5f73 697a 6520     if file_size 
+0000d450: 3e20 6d61 785f 7369 7a65 3a0a 2020 2020  > max_size:.    
+0000d460: 2020 2020 2020 2020 2320 436f 6e76 6572          # Conver
+0000d470: 7420 746f 2047 420a 2020 2020 2020 2020  t to GB.        
+0000d480: 2020 2020 6669 6c65 5f73 697a 6520 3d20      file_size = 
+0000d490: 726f 756e 6428 6669 6c65 5f73 697a 6520  round(file_size 
+0000d4a0: 2f20 2831 3032 342a 2a33 292c 2031 290a  / (1024**3), 1).
+0000d4b0: 2020 2020 2020 2020 2020 2020 6d61 785f              max_
+0000d4c0: 7369 7a65 203d 2069 6e74 286d 6178 5f73  size = int(max_s
+0000d4d0: 697a 6520 2f20 3130 3234 2a2a 3329 0a20  ize / 1024**3). 
+0000d4e0: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
+0000d4f0: 722e 7761 726e 696e 6728 0a20 2020 2020  r.warning(.     
+0000d500: 2020 2020 2020 2020 2020 2066 2246 696c             f"Fil
+0000d510: 6520 7369 7a65 207b 6669 6c65 5f73 697a  e size {file_siz
+0000d520: 657d 4742 2065 7863 6565 6473 207b 6d61  e}GB exceeds {ma
+0000d530: 785f 7369 7a65 7d47 422e 2022 0a20 2020  x_size}GB. ".   
+0000d540: 2020 2020 2020 2020 2020 2020 2022 4974               "It
+0000d550: 2069 7320 7265 636f 6d6d 656e 6465 6420   is recommended 
+0000d560: 746f 2075 7365 2065 6e67 696e 653d 2762  to use engine='b
+0000d570: 6967 7175 6572 7927 2022 0a20 2020 2020  igquery' ".     
+0000d580: 2020 2020 2020 2020 2020 2022 666f 7220             "for 
+0000d590: 6c61 7267 6520 6669 6c65 7320 746f 2061  large files to a
+0000d5a0: 766f 6964 206c 6f61 6469 6e67 2074 6865  void loading the
+0000d5b0: 2066 696c 6520 696e 746f 206c 6f63 616c   file into local
+0000d5c0: 206d 656d 6f72 792e 220a 2020 2020 2020   memory.".      
+0000d5d0: 2020 2020 2020 290a 0a20 2020 2064 6566        )..    def
+0000d5e0: 205f 6372 6561 7465 5f65 6d70 7479 5f74   _create_empty_t
+0000d5f0: 656d 705f 7461 626c 6528 0a20 2020 2020  emp_table(.     
+0000d600: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+0000d610: 2073 6368 656d 613a 2049 7465 7261 626c   schema: Iterabl
+0000d620: 655b 6269 6771 7565 7279 2e53 6368 656d  e[bigquery.Schem
+0000d630: 6146 6965 6c64 5d2c 0a20 2020 2020 2020  aField],.       
+0000d640: 2063 6c75 7374 6572 5f63 6f6c 733a 204c   cluster_cols: L
+0000d650: 6973 745b 7374 725d 2c0a 2020 2020 2920  ist[str],.    ) 
+0000d660: 2d3e 2062 6967 7175 6572 792e 5461 626c  -> bigquery.Tabl
+0000d670: 6552 6566 6572 656e 6365 3a0a 2020 2020  eReference:.    
+0000d680: 2020 2020 2320 4361 6e27 7420 7365 7420      # Can't set 
+0000d690: 6120 7461 626c 6520 696e 205f 5345 5353  a table in _SESS
+0000d6a0: 494f 4e20 6173 2064 6573 7469 6e61 7469  ION as destinati
+0000d6b0: 6f6e 2076 6961 2071 7565 7279 206a 6f62  on via query job
+0000d6c0: 2041 5049 2c20 736f 2077 650a 2020 2020   API, so we.    
+0000d6d0: 2020 2020 2320 7275 6e20 4444 4c2c 2069      # run DDL, i
+0000d6e0: 6e73 7465 6164 2e0a 2020 2020 2020 2020  nstead..        
+0000d6f0: 6461 7461 7365 7420 3d20 7365 6c66 2e5f  dataset = self._
+0000d700: 616e 6f6e 796d 6f75 735f 6461 7461 7365  anonymous_datase
+0000d710: 740a 2020 2020 2020 2020 6578 7069 7261  t.        expira
+0000d720: 7469 6f6e 203d 2028 0a20 2020 2020 2020  tion = (.       
+0000d730: 2020 2020 2064 6174 6574 696d 652e 6461       datetime.da
+0000d740: 7465 7469 6d65 2e6e 6f77 2864 6174 6574  tetime.now(datet
+0000d750: 696d 652e 7469 6d65 7a6f 6e65 2e75 7463  ime.timezone.utc
+0000d760: 2920 2b20 636f 6e73 7461 6e74 732e 4445  ) + constants.DE
+0000d770: 4641 554c 545f 4558 5049 5241 5449 4f4e  FAULT_EXPIRATION
+0000d780: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
+0000d790: 2020 2020 7461 626c 6520 3d20 6269 6766      table = bigf
+0000d7a0: 7261 6d65 735f 696f 2e63 7265 6174 655f  rames_io.create_
+0000d7b0: 7465 6d70 5f74 6162 6c65 280a 2020 2020  temp_table(.    
+0000d7c0: 2020 2020 2020 2020 7365 6c66 2e62 7163          self.bqc
+0000d7d0: 6c69 656e 742c 0a20 2020 2020 2020 2020  lient,.         
+0000d7e0: 2020 2064 6174 6173 6574 2c0a 2020 2020     dataset,.    
+0000d7f0: 2020 2020 2020 2020 6578 7069 7261 7469          expirati
+0000d800: 6f6e 2c0a 2020 2020 2020 2020 2020 2020  on,.            
+0000d810: 7363 6865 6d61 3d73 6368 656d 612c 0a20  schema=schema,. 
+0000d820: 2020 2020 2020 2020 2020 2063 6c75 7374             clust
+0000d830: 6572 5f63 6f6c 756d 6e73 3d63 6c75 7374  er_columns=clust
+0000d840: 6572 5f63 6f6c 732c 0a20 2020 2020 2020  er_cols,.       
+0000d850: 2029 0a20 2020 2020 2020 2072 6574 7572   ).        retur
+0000d860: 6e20 6269 6771 7565 7279 2e54 6162 6c65  n bigquery.Table
+0000d870: 5265 6665 7265 6e63 652e 6672 6f6d 5f73  Reference.from_s
+0000d880: 7472 696e 6728 7461 626c 6529 0a0a 2020  tring(table)..  
+0000d890: 2020 6465 6620 5f63 7265 6174 655f 746f    def _create_to
+0000d8a0: 7461 6c5f 6f72 6465 7269 6e67 280a 2020  tal_ordering(.  
+0000d8b0: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+0000d8c0: 2020 2020 7461 626c 653a 2069 6269 735f      table: ibis_
+0000d8d0: 7479 7065 732e 5461 626c 652c 0a20 2020  types.Table,.   
+0000d8e0: 2029 202d 3e20 636f 7265 2e41 7272 6179   ) -> core.Array
+0000d8f0: 5661 6c75 653a 0a20 2020 2020 2020 2023  Value:.        #
+0000d900: 2053 696e 6365 2074 6869 7320 6d69 6768   Since this migh
+0000d910: 7420 616c 736f 2062 6520 7573 6564 2061  t also be used a
+0000d920: 7320 7468 6520 696e 6465 782c 2064 6f6e  s the index, don
+0000d930: 2774 2075 7365 2074 6865 2064 6566 6175  't use the defau
+0000d940: 6c74 0a20 2020 2020 2020 2023 2022 6f72  lt.        # "or
+0000d950: 6465 7269 6e67 2049 4422 206e 616d 652e  dering ID" name.
+0000d960: 0a20 2020 2020 2020 206f 7264 6572 696e  .        orderin
+0000d970: 675f 6861 7368 5f70 6172 7420 3d20 6775  g_hash_part = gu
+0000d980: 6964 2e67 656e 6572 6174 655f 6775 6964  id.generate_guid
+0000d990: 2822 6269 6766 7261 6d65 735f 6f72 6465  ("bigframes_orde
+0000d9a0: 7269 6e67 5f22 290a 2020 2020 2020 2020  ring_").        
+0000d9b0: 6f72 6465 7269 6e67 5f72 616e 645f 7061  ordering_rand_pa
+0000d9c0: 7274 203d 2067 7569 642e 6765 6e65 7261  rt = guid.genera
+0000d9d0: 7465 5f67 7569 6428 2262 6967 6672 616d  te_guid("bigfram
+0000d9e0: 6573 5f6f 7264 6572 696e 675f 2229 0a0a  es_ordering_")..
+0000d9f0: 2020 2020 2020 2020 2320 416c 6c20 696e          # All in
+0000da00: 7075 7473 2069 6e74 6f20 6861 7368 206d  puts into hash m
+0000da10: 7573 7420 6265 206e 6f6e 2d6e 756c 6c20  ust be non-null 
+0000da20: 6f72 2072 6573 756c 7469 6e67 2068 6173  or resulting has
+0000da30: 6820 7769 6c6c 2062 6520 6e75 6c6c 0a20  h will be null. 
+0000da40: 2020 2020 2020 2073 7472 5f76 616c 7565         str_value
+0000da50: 7320 3d20 6c69 7374 280a 2020 2020 2020  s = list(.      
+0000da60: 2020 2020 2020 6d61 7028 6c61 6d62 6461        map(lambda
+0000da70: 2063 6f6c 3a20 5f63 6f6e 7665 7274 5f74   col: _convert_t
+0000da80: 6f5f 6e6f 6e6e 756c 6c5f 7374 7269 6e67  o_nonnull_string
+0000da90: 2874 6162 6c65 5b63 6f6c 5d29 2c20 7461  (table[col]), ta
+0000daa0: 626c 652e 636f 6c75 6d6e 7329 0a20 2020  ble.columns).   
+0000dab0: 2020 2020 2029 0a20 2020 2020 2020 2066       ).        f
+0000dac0: 756c 6c5f 726f 775f 7374 7220 3d20 280a  ull_row_str = (.
+0000dad0: 2020 2020 2020 2020 2020 2020 7374 725f              str_
+0000dae0: 7661 6c75 6573 5b30 5d2e 636f 6e63 6174  values[0].concat
+0000daf0: 282a 7374 725f 7661 6c75 6573 5b31 3a5d  (*str_values[1:]
+0000db00: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+0000db10: 206c 656e 2873 7472 5f76 616c 7565 7329   len(str_values)
+0000db20: 203e 2031 0a20 2020 2020 2020 2020 2020   > 1.           
+0000db30: 2065 6c73 6520 7374 725f 7661 6c75 6573   else str_values
+0000db40: 5b30 5d0a 2020 2020 2020 2020 290a 2020  [0].        ).  
+0000db50: 2020 2020 2020 6675 6c6c 5f72 6f77 5f68        full_row_h
+0000db60: 6173 6820 3d20 6675 6c6c 5f72 6f77 5f73  ash = full_row_s
+0000db70: 7472 2e68 6173 6828 292e 6e61 6d65 286f  tr.hash().name(o
+0000db80: 7264 6572 696e 675f 6861 7368 5f70 6172  rdering_hash_par
+0000db90: 7429 0a20 2020 2020 2020 2023 2055 7365  t).        # Use
+0000dba0: 6420 746f 2064 6973 616d 6269 6775 6174  d to disambiguat
+0000dbb0: 6520 6265 7477 6565 6e20 6964 656e 7469  e between identi
+0000dbc0: 6361 6c20 726f 7773 2028 7768 6963 6820  cal rows (which 
+0000dbd0: 7769 6c6c 2068 6176 6520 6964 656e 7469  will have identi
+0000dbe0: 6361 6c20 6861 7368 290a 2020 2020 2020  cal hash).      
+0000dbf0: 2020 7261 6e64 6f6d 5f76 616c 7565 203d    random_value =
+0000dc00: 2069 6269 732e 7261 6e64 6f6d 2829 2e6e   ibis.random().n
+0000dc10: 616d 6528 6f72 6465 7269 6e67 5f72 616e  ame(ordering_ran
+0000dc20: 645f 7061 7274 290a 0a20 2020 2020 2020  d_part)..       
+0000dc30: 206f 7269 6769 6e61 6c5f 636f 6c75 6d6e   original_column
+0000dc40: 5f69 6473 203d 2074 6162 6c65 2e63 6f6c  _ids = table.col
+0000dc50: 756d 6e73 0a20 2020 2020 2020 2074 6162  umns.        tab
+0000dc60: 6c65 5f77 6974 685f 6f72 6465 7269 6e67  le_with_ordering
+0000dc70: 203d 2074 6162 6c65 2e73 656c 6563 7428   = table.select(
+0000dc80: 0a20 2020 2020 2020 2020 2020 2069 7465  .            ite
+0000dc90: 7274 6f6f 6c73 2e63 6861 696e 286f 7269  rtools.chain(ori
+0000dca0: 6769 6e61 6c5f 636f 6c75 6d6e 5f69 6473  ginal_column_ids
+0000dcb0: 2c20 5b66 756c 6c5f 726f 775f 6861 7368  , [full_row_hash
+0000dcc0: 2c20 7261 6e64 6f6d 5f76 616c 7565 5d29  , random_value])
+0000dcd0: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
+0000dce0: 2020 2020 6f72 6465 7269 6e67 5f72 6566      ordering_ref
+0000dcf0: 3120 3d20 6f72 6465 722e 6173 6365 6e64  1 = order.ascend
+0000dd00: 696e 675f 6f76 6572 286f 7264 6572 696e  ing_over(orderin
+0000dd10: 675f 6861 7368 5f70 6172 7429 0a20 2020  g_hash_part).   
+0000dd20: 2020 2020 206f 7264 6572 696e 675f 7265       ordering_re
+0000dd30: 6632 203d 206f 7264 6572 2e61 7363 656e  f2 = order.ascen
+0000dd40: 6469 6e67 5f6f 7665 7228 6f72 6465 7269  ding_over(orderi
+0000dd50: 6e67 5f72 616e 645f 7061 7274 290a 2020  ng_rand_part).  
+0000dd60: 2020 2020 2020 6f72 6465 7269 6e67 203d        ordering =
+0000dd70: 206f 7264 6572 2e45 7870 7265 7373 696f   order.Expressio
+0000dd80: 6e4f 7264 6572 696e 6728 0a20 2020 2020  nOrdering(.     
+0000dd90: 2020 2020 2020 206f 7264 6572 696e 675f         ordering_
+0000dda0: 7661 6c75 655f 636f 6c75 6d6e 733d 286f  value_columns=(o
+0000ddb0: 7264 6572 696e 675f 7265 6631 2c20 6f72  rdering_ref1, or
+0000ddc0: 6465 7269 6e67 5f72 6566 3229 2c0a 2020  dering_ref2),.  
+0000ddd0: 2020 2020 2020 2020 2020 746f 7461 6c5f            total_
+0000dde0: 6f72 6465 7269 6e67 5f63 6f6c 756d 6e73  ordering_columns
+0000ddf0: 3d66 726f 7a65 6e73 6574 285b 6f72 6465  =frozenset([orde
+0000de00: 7269 6e67 5f68 6173 685f 7061 7274 2c20  ring_hash_part, 
+0000de10: 6f72 6465 7269 6e67 5f72 616e 645f 7061  ordering_rand_pa
+0000de20: 7274 5d29 2c0a 2020 2020 2020 2020 290a  rt]),.        ).
+0000de30: 2020 2020 2020 2020 636f 6c75 6d6e 7320          columns 
+0000de40: 3d20 5b74 6162 6c65 5f77 6974 685f 6f72  = [table_with_or
+0000de50: 6465 7269 6e67 5b63 6f6c 5d20 666f 7220  dering[col] for 
+0000de60: 636f 6c20 696e 206f 7269 6769 6e61 6c5f  col in original_
+0000de70: 636f 6c75 6d6e 5f69 6473 5d0a 2020 2020  column_ids].    
+0000de80: 2020 2020 6869 6464 656e 5f63 6f6c 756d      hidden_colum
+0000de90: 6e73 203d 205b 0a20 2020 2020 2020 2020  ns = [.         
+0000dea0: 2020 2074 6162 6c65 5f77 6974 685f 6f72     table_with_or
+0000deb0: 6465 7269 6e67 5b6f 7264 6572 696e 675f  dering[ordering_
+0000dec0: 6861 7368 5f70 6172 745d 2c0a 2020 2020  hash_part],.    
+0000ded0: 2020 2020 2020 2020 7461 626c 655f 7769          table_wi
+0000dee0: 7468 5f6f 7264 6572 696e 675b 6f72 6465  th_ordering[orde
+0000def0: 7269 6e67 5f72 616e 645f 7061 7274 5d2c  ring_rand_part],
+0000df00: 0a20 2020 2020 2020 205d 0a20 2020 2020  .        ].     
+0000df10: 2020 2072 6574 7572 6e20 636f 7265 2e41     return core.A
+0000df20: 7272 6179 5661 6c75 652e 6672 6f6d 5f69  rrayValue.from_i
+0000df30: 6269 7328 0a20 2020 2020 2020 2020 2020  bis(.           
+0000df40: 2073 656c 662c 0a20 2020 2020 2020 2020   self,.         
+0000df50: 2020 2074 6162 6c65 5f77 6974 685f 6f72     table_with_or
+0000df60: 6465 7269 6e67 2c0a 2020 2020 2020 2020  dering,.        
+0000df70: 2020 2020 636f 6c75 6d6e 732c 0a20 2020      columns,.   
+0000df80: 2020 2020 2020 2020 2068 6964 6465 6e5f           hidden_
+0000df90: 6f72 6465 7269 6e67 5f63 6f6c 756d 6e73  ordering_columns
+0000dfa0: 3d68 6964 6465 6e5f 636f 6c75 6d6e 732c  =hidden_columns,
+0000dfb0: 0a20 2020 2020 2020 2020 2020 206f 7264  .            ord
+0000dfc0: 6572 696e 673d 6f72 6465 7269 6e67 2c0a  ering=ordering,.
+0000dfd0: 2020 2020 2020 2020 290a 0a20 2020 2064          )..    d
+0000dfe0: 6566 205f 6962 6973 5f74 6f5f 7465 6d70  ef _ibis_to_temp
+0000dff0: 5f74 6162 6c65 280a 2020 2020 2020 2020  _table(.        
+0000e000: 7365 6c66 2c0a 2020 2020 2020 2020 7461  self,.        ta
+0000e010: 626c 653a 2069 6269 735f 7479 7065 732e  ble: ibis_types.
+0000e020: 5461 626c 652c 0a20 2020 2020 2020 2063  Table,.        c
+0000e030: 6c75 7374 6572 5f63 6f6c 733a 2049 7465  luster_cols: Ite
+0000e040: 7261 626c 655b 7374 725d 2c0a 2020 2020  rable[str],.    
+0000e050: 2020 2020 6170 695f 6e61 6d65 3a20 7374      api_name: st
+0000e060: 722c 0a20 2020 2029 202d 3e20 6269 6771  r,.    ) -> bigq
+0000e070: 7565 7279 2e54 6162 6c65 5265 6665 7265  uery.TableRefere
+0000e080: 6e63 653a 0a20 2020 2020 2020 2064 6573  nce:.        des
+0000e090: 7469 6e61 7469 6f6e 2c20 5f20 3d20 7365  tination, _ = se
+0000e0a0: 6c66 2e5f 7175 6572 795f 746f 5f64 6573  lf._query_to_des
+0000e0b0: 7469 6e61 7469 6f6e 280a 2020 2020 2020  tination(.      
+0000e0c0: 2020 2020 2020 7365 6c66 2e69 6269 735f        self.ibis_
+0000e0d0: 636c 6965 6e74 2e63 6f6d 7069 6c65 2874  client.compile(t
+0000e0e0: 6162 6c65 292c 0a20 2020 2020 2020 2020  able),.         
+0000e0f0: 2020 2069 6e64 6578 5f63 6f6c 733d 6c69     index_cols=li
+0000e100: 7374 2863 6c75 7374 6572 5f63 6f6c 7329  st(cluster_cols)
+0000e110: 2c0a 2020 2020 2020 2020 2020 2020 6170  ,.            ap
+0000e120: 695f 6e61 6d65 3d61 7069 5f6e 616d 652c  i_name=api_name,
+0000e130: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+0000e140: 2020 2023 2054 6865 7265 2073 686f 756c     # There shoul
+0000e150: 6420 616c 7761 7973 2062 6520 6120 6465  d always be a de
+0000e160: 7374 696e 6174 696f 6e20 7461 626c 6520  stination table 
+0000e170: 666f 7220 7468 6973 2071 7565 7279 2074  for this query t
+0000e180: 7970 652e 0a20 2020 2020 2020 2072 6574  ype..        ret
+0000e190: 7572 6e20 7479 7069 6e67 2e63 6173 7428  urn typing.cast(
+0000e1a0: 6269 6771 7565 7279 2e54 6162 6c65 5265  bigquery.TableRe
+0000e1b0: 6665 7265 6e63 652c 2064 6573 7469 6e61  ference, destina
+0000e1c0: 7469 6f6e 290a 0a20 2020 2064 6566 2072  tion)..    def r
+0000e1d0: 656d 6f74 655f 6675 6e63 7469 6f6e 280a  emote_function(.
+0000e1e0: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+0000e1f0: 2020 2020 2020 696e 7075 745f 7479 7065        input_type
+0000e200: 733a 204c 6973 745b 7479 7065 5d2c 0a20  s: List[type],. 
+0000e210: 2020 2020 2020 206f 7574 7075 745f 7479         output_ty
+0000e220: 7065 3a20 7479 7065 2c0a 2020 2020 2020  pe: type,.      
+0000e230: 2020 6461 7461 7365 743a 204f 7074 696f    dataset: Optio
+0000e240: 6e61 6c5b 7374 725d 203d 204e 6f6e 652c  nal[str] = None,
+0000e250: 0a20 2020 2020 2020 2062 6967 7175 6572  .        bigquer
+0000e260: 795f 636f 6e6e 6563 7469 6f6e 3a20 4f70  y_connection: Op
+0000e270: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
+0000e280: 6e65 2c0a 2020 2020 2020 2020 7265 7573  ne,.        reus
+0000e290: 653a 2062 6f6f 6c20 3d20 5472 7565 2c0a  e: bool = True,.
+0000e2a0: 2020 2020 2020 2020 6e61 6d65 3a20 4f70          name: Op
+0000e2b0: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
+0000e2c0: 6e65 2c0a 2020 2020 2020 2020 7061 636b  ne,.        pack
+0000e2d0: 6167 6573 3a20 4f70 7469 6f6e 616c 5b53  ages: Optional[S
+0000e2e0: 6571 7565 6e63 655b 7374 725d 5d20 3d20  equence[str]] = 
+0000e2f0: 4e6f 6e65 2c0a 2020 2020 2020 2020 636c  None,.        cl
+0000e300: 6f75 645f 6675 6e63 7469 6f6e 5f73 6572  oud_function_ser
+0000e310: 7669 6365 5f61 6363 6f75 6e74 3a20 4f70  vice_account: Op
+0000e320: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
+0000e330: 6e65 2c0a 2020 2020 2020 2020 636c 6f75  ne,.        clou
+0000e340: 645f 6675 6e63 7469 6f6e 5f6b 6d73 5f6b  d_function_kms_k
+0000e350: 6579 5f6e 616d 653a 204f 7074 696f 6e61  ey_name: Optiona
+0000e360: 6c5b 7374 725d 203d 204e 6f6e 652c 0a20  l[str] = None,. 
+0000e370: 2020 2020 2020 2063 6c6f 7564 5f66 756e         cloud_fun
+0000e380: 6374 696f 6e5f 646f 636b 6572 5f72 6570  ction_docker_rep
+0000e390: 6f73 6974 6f72 793a 204f 7074 696f 6e61  ository: Optiona
+0000e3a0: 6c5b 7374 725d 203d 204e 6f6e 652c 0a20  l[str] = None,. 
+0000e3b0: 2020 2029 3a0a 2020 2020 2020 2020 2222     ):.        ""
+0000e3c0: 2244 6563 6f72 6174 6f72 2074 6f20 7475  "Decorator to tu
+0000e3d0: 726e 2061 2075 7365 7220 6465 6669 6e65  rn a user define
+0000e3e0: 6420 6675 6e63 7469 6f6e 2069 6e74 6f20  d function into 
+0000e3f0: 6120 4269 6751 7565 7279 2072 656d 6f74  a BigQuery remot
+0000e400: 6520 6675 6e63 7469 6f6e 2e20 4368 6563  e function. Chec
+0000e410: 6b20 6f75 740a 2020 2020 2020 2020 7468  k out.        th
+0000e420: 6520 636f 6465 2073 616d 706c 6573 2061  e code samples a
+0000e430: 743a 2068 7474 7073 3a2f 2f63 6c6f 7564  t: https://cloud
+0000e440: 2e67 6f6f 676c 652e 636f 6d2f 6269 6771  .google.com/bigq
+0000e450: 7565 7279 2f64 6f63 732f 7265 6d6f 7465  uery/docs/remote
+0000e460: 2d66 756e 6374 696f 6e73 2362 6967 7175  -functions#bigqu
+0000e470: 6572 792d 6461 7461 6672 616d 6573 2e0a  ery-dataframes..
+0000e480: 0a20 2020 2020 2020 202e 2e20 6e6f 7465  .        .. note
+0000e490: 3a3a 0a20 2020 2020 2020 2020 2020 2050  ::.            P
+0000e4a0: 6c65 6173 6520 6d61 6b65 2073 7572 6520  lease make sure 
+0000e4b0: 666f 6c6c 6f77 696e 6720 6973 2073 6574  following is set
+0000e4c0: 7570 2062 6566 6f72 6520 7573 696e 6720  up before using 
+0000e4d0: 7468 6973 2041 5049 3a0a 0a20 2020 2020  this API:..     
+0000e4e0: 2020 2031 2e20 4861 7665 2074 6865 2062     1. Have the b
+0000e4f0: 656c 6f77 2041 5049 7320 656e 6162 6c65  elow APIs enable
+0000e500: 6420 666f 7220 796f 7572 2070 726f 6a65  d for your proje
+0000e510: 6374 3a0a 0a20 2020 2020 2020 2020 2020  ct:..           
+0000e520: 202a 2042 6967 5175 6572 7920 436f 6e6e   * BigQuery Conn
+0000e530: 6563 7469 6f6e 2041 5049 0a20 2020 2020  ection API.     
+0000e540: 2020 2020 2020 202a 2043 6c6f 7564 2046         * Cloud F
+0000e550: 756e 6374 696f 6e73 2041 5049 0a20 2020  unctions API.   
+0000e560: 2020 2020 2020 2020 202a 2043 6c6f 7564           * Cloud
+0000e570: 2052 756e 2041 5049 0a20 2020 2020 2020   Run API.       
+0000e580: 2020 2020 202a 2043 6c6f 7564 2042 7569       * Cloud Bui
+0000e590: 6c64 2041 5049 0a20 2020 2020 2020 2020  ld API.         
+0000e5a0: 2020 202a 2041 7274 6966 6163 7420 5265     * Artifact Re
+0000e5b0: 6769 7374 7279 2041 5049 0a20 2020 2020  gistry API.     
+0000e5c0: 2020 2020 2020 202a 2043 6c6f 7564 2052         * Cloud R
+0000e5d0: 6573 6f75 7263 6520 4d61 6e61 6765 7220  esource Manager 
+0000e5e0: 4150 490a 0a20 2020 2020 2020 2020 2020  API..           
+0000e5f0: 5468 6973 2063 616e 2062 6520 646f 6e65  This can be done
+0000e600: 2066 726f 6d20 7468 6520 636c 6f75 6420   from the cloud 
+0000e610: 636f 6e73 6f6c 6520 2863 6861 6e67 6520  console (change 
+0000e620: 6050 524f 4a45 4354 5f49 4460 2074 6f20  `PROJECT_ID` to 
+0000e630: 796f 7572 7329 3a0a 2020 2020 2020 2020  yours):.        
+0000e640: 2020 2068 7474 7073 3a2f 2f63 6f6e 736f     https://conso
+0000e650: 6c65 2e63 6c6f 7564 2e67 6f6f 676c 652e  le.cloud.google.
+0000e660: 636f 6d2f 6170 6973 2f65 6e61 626c 6566  com/apis/enablef
+0000e670: 6c6f 773f 6170 6969 643d 6269 6771 7565  low?apiid=bigque
+0000e680: 7279 636f 6e6e 6563 7469 6f6e 2e67 6f6f  ryconnection.goo
+0000e690: 676c 6561 7069 732e 636f 6d2c 636c 6f75  gleapis.com,clou
+0000e6a0: 6466 756e 6374 696f 6e73 2e67 6f6f 676c  dfunctions.googl
+0000e6b0: 6561 7069 732e 636f 6d2c 7275 6e2e 676f  eapis.com,run.go
+0000e6c0: 6f67 6c65 6170 6973 2e63 6f6d 2c63 6c6f  ogleapis.com,clo
+0000e6d0: 7564 6275 696c 642e 676f 6f67 6c65 6170  udbuild.googleap
+0000e6e0: 6973 2e63 6f6d 2c61 7274 6966 6163 7472  is.com,artifactr
+0000e6f0: 6567 6973 7472 792e 676f 6f67 6c65 6170  egistry.googleap
+0000e700: 6973 2e63 6f6d 2c63 6c6f 7564 7265 736f  is.com,cloudreso
+0000e710: 7572 6365 6d61 6e61 6765 722e 676f 6f67  urcemanager.goog
+0000e720: 6c65 6170 6973 2e63 6f6d 2670 726f 6a65  leapis.com&proje
+0000e730: 6374 3d50 524f 4a45 4354 5f49 440a 0a20  ct=PROJECT_ID.. 
+0000e740: 2020 2020 2020 2020 2020 4f72 2066 726f            Or fro
+0000e750: 6d20 7468 6520 6763 6c6f 7564 2043 4c49  m the gcloud CLI
+0000e760: 3a0a 0a20 2020 2020 2020 2020 2020 6024  :..           `$
+0000e770: 2067 636c 6f75 6420 7365 7276 6963 6573   gcloud services
+0000e780: 2065 6e61 626c 6520 6269 6771 7565 7279   enable bigquery
+0000e790: 636f 6e6e 6563 7469 6f6e 2e67 6f6f 676c  connection.googl
+0000e7a0: 6561 7069 732e 636f 6d20 636c 6f75 6466  eapis.com cloudf
+0000e7b0: 756e 6374 696f 6e73 2e67 6f6f 676c 6561  unctions.googlea
+0000e7c0: 7069 732e 636f 6d20 7275 6e2e 676f 6f67  pis.com run.goog
+0000e7d0: 6c65 6170 6973 2e63 6f6d 2063 6c6f 7564  leapis.com cloud
+0000e7e0: 6275 696c 642e 676f 6f67 6c65 6170 6973  build.googleapis
+0000e7f0: 2e63 6f6d 2061 7274 6966 6163 7472 6567  .com artifactreg
+0000e800: 6973 7472 792e 676f 6f67 6c65 6170 6973  istry.googleapis
+0000e810: 2e63 6f6d 2063 6c6f 7564 7265 736f 7572  .com cloudresour
+0000e820: 6365 6d61 6e61 6765 722e 676f 6f67 6c65  cemanager.google
+0000e830: 6170 6973 2e63 6f6d 600a 0a20 2020 2020  apis.com`..     
+0000e840: 2020 2032 2e20 4861 7665 2066 6f6c 6c6f     2. Have follo
+0000e850: 7769 6e67 2049 414d 2072 6f6c 6573 2065  wing IAM roles e
+0000e860: 6e61 626c 6564 2066 6f72 2079 6f75 3a0a  nabled for you:.
+0000e870: 0a20 2020 2020 2020 2020 2020 202a 2042  .            * B
+0000e880: 6967 5175 6572 7920 4461 7461 2045 6469  igQuery Data Edi
+0000e890: 746f 7220 2872 6f6c 6573 2f62 6967 7175  tor (roles/bigqu
+0000e8a0: 6572 792e 6461 7461 4564 6974 6f72 290a  ery.dataEditor).
+0000e8b0: 2020 2020 2020 2020 2020 2020 2a20 4269              * Bi
+0000e8c0: 6751 7565 7279 2043 6f6e 6e65 6374 696f  gQuery Connectio
+0000e8d0: 6e20 4164 6d69 6e20 2872 6f6c 6573 2f62  n Admin (roles/b
+0000e8e0: 6967 7175 6572 792e 636f 6e6e 6563 7469  igquery.connecti
+0000e8f0: 6f6e 4164 6d69 6e29 0a20 2020 2020 2020  onAdmin).       
+0000e900: 2020 2020 202a 2043 6c6f 7564 2046 756e       * Cloud Fun
+0000e910: 6374 696f 6e73 2044 6576 656c 6f70 6572  ctions Developer
+0000e920: 2028 726f 6c65 732f 636c 6f75 6466 756e   (roles/cloudfun
+0000e930: 6374 696f 6e73 2e64 6576 656c 6f70 6572  ctions.developer
+0000e940: 290a 2020 2020 2020 2020 2020 2020 2a20  ).            * 
+0000e950: 5365 7276 6963 6520 4163 636f 756e 7420  Service Account 
+0000e960: 5573 6572 2028 726f 6c65 732f 6961 6d2e  User (roles/iam.
+0000e970: 7365 7276 6963 6541 6363 6f75 6e74 5573  serviceAccountUs
+0000e980: 6572 2920 6f6e 2074 6865 2073 6572 7669  er) on the servi
+0000e990: 6365 2061 6363 6f75 6e74 2060 5052 4f4a  ce account `PROJ
+0000e9a0: 4543 545f 4e55 4d42 4552 2d63 6f6d 7075  ECT_NUMBER-compu
+0000e9b0: 7465 4064 6576 656c 6f70 6572 2e67 7365  te@developer.gse
+0000e9c0: 7276 6963 6561 6363 6f75 6e74 2e63 6f6d  rviceaccount.com
+0000e9d0: 600a 2020 2020 2020 2020 2020 2020 2a20  `.            * 
+0000e9e0: 5374 6f72 6167 6520 4f62 6a65 6374 2056  Storage Object V
+0000e9f0: 6965 7765 7220 2872 6f6c 6573 2f73 746f  iewer (roles/sto
+0000ea00: 7261 6765 2e6f 626a 6563 7456 6965 7765  rage.objectViewe
+0000ea10: 7229 0a20 2020 2020 2020 2020 2020 202a  r).            *
+0000ea20: 2050 726f 6a65 6374 2049 414d 2041 646d   Project IAM Adm
+0000ea30: 696e 2028 726f 6c65 732f 7265 736f 7572  in (roles/resour
+0000ea40: 6365 6d61 6e61 6765 722e 7072 6f6a 6563  cemanager.projec
+0000ea50: 7449 616d 4164 6d69 6e29 2028 4f6e 6c79  tIamAdmin) (Only
+0000ea60: 2072 6571 7569 7265 6420 6966 2074 6865   required if the
+0000ea70: 2062 6967 7175 6572 7920 636f 6e6e 6563   bigquery connec
+0000ea80: 7469 6f6e 2062 6569 6e67 2075 7365 6420  tion being used 
+0000ea90: 6973 206e 6f74 2070 7265 2d63 7265 6174  is not pre-creat
+0000eaa0: 6564 2061 6e64 2069 7320 6372 6561 7465  ed and is create
+0000eab0: 6420 6479 6e61 6d69 6361 6c6c 7920 7769  d dynamically wi
+0000eac0: 7468 2075 7365 7220 6372 6564 656e 7469  th user credenti
+0000ead0: 616c 732e 290a 0a20 2020 2020 2020 2033  als.)..        3
+0000eae0: 2e20 4569 7468 6572 2074 6865 2075 7365  . Either the use
+0000eaf0: 7220 6861 7320 7365 7449 616d 506f 6c69  r has setIamPoli
+0000eb00: 6379 2070 7269 7669 6c65 6765 206f 6e20  cy privilege on 
+0000eb10: 7468 6520 7072 6f6a 6563 742c 206f 7220  the project, or 
+0000eb20: 6120 4269 6751 7565 7279 2063 6f6e 6e65  a BigQuery conne
+0000eb30: 6374 696f 6e20 6973 2070 7265 2d63 7265  ction is pre-cre
+0000eb40: 6174 6564 2077 6974 6820 6e65 6365 7373  ated with necess
+0000eb50: 6172 7920 4941 4d20 726f 6c65 2073 6574  ary IAM role set
+0000eb60: 3a0a 0a20 2020 2020 2020 2020 2020 2031  :..            1
+0000eb70: 2e20 546f 2063 7265 6174 6520 6120 636f  . To create a co
+0000eb80: 6e6e 6563 7469 6f6e 2c20 666f 6c6c 6f77  nnection, follow
+0000eb90: 2068 7474 7073 3a2f 2f63 6c6f 7564 2e67   https://cloud.g
+0000eba0: 6f6f 676c 652e 636f 6d2f 6269 6771 7565  oogle.com/bigque
+0000ebb0: 7279 2f64 6f63 732f 7265 6665 7265 6e63  ry/docs/referenc
+0000ebc0: 652f 7374 616e 6461 7264 2d73 716c 2f72  e/standard-sql/r
+0000ebd0: 656d 6f74 652d 6675 6e63 7469 6f6e 7323  emote-functions#
+0000ebe0: 6372 6561 7465 5f61 5f63 6f6e 6e65 6374  create_a_connect
+0000ebf0: 696f 6e0a 2020 2020 2020 2020 2020 2020  ion.            
+0000ec00: 322e 2054 6f20 7365 7420 7570 2049 414d  2. To set up IAM
+0000ec10: 2c20 666f 6c6c 6f77 2068 7474 7073 3a2f  , follow https:/
+0000ec20: 2f63 6c6f 7564 2e67 6f6f 676c 652e 636f  /cloud.google.co
+0000ec30: 6d2f 6269 6771 7565 7279 2f64 6f63 732f  m/bigquery/docs/
+0000ec40: 7265 6665 7265 6e63 652f 7374 616e 6461  reference/standa
+0000ec50: 7264 2d73 716c 2f72 656d 6f74 652d 6675  rd-sql/remote-fu
+0000ec60: 6e63 7469 6f6e 7323 6772 616e 745f 7065  nctions#grant_pe
+0000ec70: 726d 6973 7369 6f6e 5f6f 6e5f 6675 6e63  rmission_on_func
+0000ec80: 7469 6f6e 0a0a 2020 2020 2020 2020 2020  tion..          
+0000ec90: 2020 2020 2041 6c74 6572 6e61 7469 7665       Alternative
+0000eca0: 6c79 2c20 7468 6520 4941 4d20 636f 756c  ly, the IAM coul
+0000ecb0: 6420 616c 736f 2062 6520 7365 7475 7020  d also be setup 
+0000ecc0: 7669 6120 7468 6520 6763 6c6f 7564 2043  via the gcloud C
+0000ecd0: 4c49 3a0a 0a20 2020 2020 2020 2020 2020  LI:..           
+0000ece0: 2020 2020 6024 2067 636c 6f75 6420 7072      `$ gcloud pr
+0000ecf0: 6f6a 6563 7473 2061 6464 2d69 616d 2d70  ojects add-iam-p
+0000ed00: 6f6c 6963 792d 6269 6e64 696e 6720 5052  olicy-binding PR
+0000ed10: 4f4a 4543 545f 4944 202d 2d6d 656d 6265  OJECT_ID --membe
+0000ed20: 723d 2273 6572 7669 6365 4163 636f 756e  r="serviceAccoun
+0000ed30: 743a 434f 4e4e 4543 5449 4f4e 5f53 4552  t:CONNECTION_SER
+0000ed40: 5649 4345 5f41 4343 4f55 4e54 5f49 4422  VICE_ACCOUNT_ID"
+0000ed50: 202d 2d72 6f6c 653d 2272 6f6c 6573 2f72   --role="roles/r
+0000ed60: 756e 2e69 6e76 6f6b 6572 2260 2e0a 0a20  un.invoker"`... 
+0000ed70: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
+0000ed80: 2020 2020 2020 2020 2069 6e70 7574 5f74           input_t
+0000ed90: 7970 6573 2028 6c69 7374 2874 7970 6529  ypes (list(type)
+0000eda0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0000edb0: 2020 204c 6973 7420 6f66 2069 6e70 7574     List of input
+0000edc0: 2064 6174 6120 7479 7065 7320 696e 2074   data types in t
+0000edd0: 6865 2075 7365 7220 6465 6669 6e65 6420  he user defined 
+0000ede0: 6675 6e63 7469 6f6e 2e0a 2020 2020 2020  function..      
+0000edf0: 2020 2020 2020 6f75 7470 7574 5f74 7970        output_typ
+0000ee00: 6520 2874 7970 6529 3a0a 2020 2020 2020  e (type):.      
+0000ee10: 2020 2020 2020 2020 2020 4461 7461 2074            Data t
+0000ee20: 7970 6520 6f66 2074 6865 206f 7574 7075  ype of the outpu
+0000ee30: 7420 696e 2074 6865 2075 7365 7220 6465  t in the user de
+0000ee40: 6669 6e65 6420 6675 6e63 7469 6f6e 2e0a  fined function..
+0000ee50: 2020 2020 2020 2020 2020 2020 6461 7461              data
+0000ee60: 7365 7420 2873 7472 2c20 4f70 7469 6f6e  set (str, Option
+0000ee70: 616c 293a 0a20 2020 2020 2020 2020 2020  al):.           
+0000ee80: 2020 2020 2044 6174 6173 6574 2069 6e20       Dataset in 
+0000ee90: 7768 6963 6820 746f 2063 7265 6174 6520  which to create 
+0000eea0: 6120 4269 6751 7565 7279 2072 656d 6f74  a BigQuery remot
+0000eeb0: 6520 6675 6e63 7469 6f6e 2e20 4974 2073  e function. It s
+0000eec0: 686f 756c 6420 6265 2069 6e0a 2020 2020  hould be in.    
+0000eed0: 2020 2020 2020 2020 2020 2020 603c 7072              `<pr
+0000eee0: 6f6a 6563 745f 6964 3e2e 3c64 6174 6173  oject_id>.<datas
+0000eef0: 6574 5f6e 616d 653e 6020 6f72 2060 3c64  et_name>` or `<d
+0000ef00: 6174 6173 6574 5f6e 616d 653e 6020 666f  ataset_name>` fo
+0000ef10: 726d 6174 2e20 4966 2074 6869 730a 2020  rmat. If this.  
+0000ef20: 2020 2020 2020 2020 2020 2020 2020 7061                pa
+0000ef30: 7261 6d65 7465 7220 6973 206e 6f74 2070  rameter is not p
+0000ef40: 726f 7669 6465 6420 7468 656e 2073 6573  rovided then ses
+0000ef50: 7369 6f6e 2064 6174 6173 6574 2069 6420  sion dataset id 
+0000ef60: 6973 2075 7365 642e 0a20 2020 2020 2020  is used..       
+0000ef70: 2020 2020 2062 6967 7175 6572 795f 636f       bigquery_co
+0000ef80: 6e6e 6563 7469 6f6e 2028 7374 722c 204f  nnection (str, O
+0000ef90: 7074 696f 6e61 6c29 3a0a 2020 2020 2020  ptional):.      
+0000efa0: 2020 2020 2020 2020 2020 4e61 6d65 206f            Name o
+0000efb0: 6620 7468 6520 4269 6751 7565 7279 2063  f the BigQuery c
+0000efc0: 6f6e 6e65 6374 696f 6e2e 2059 6f75 2073  onnection. You s
+0000efd0: 686f 756c 6420 6569 7468 6572 2068 6176  hould either hav
+0000efe0: 6520 7468 650a 2020 2020 2020 2020 2020  e the.          
+0000eff0: 2020 2020 2020 636f 6e6e 6563 7469 6f6e        connection
+0000f000: 2061 6c72 6561 6479 2063 7265 6174 6564   already created
+0000f010: 2069 6e20 7468 6520 606c 6f63 6174 696f   in the `locatio
+0000f020: 6e60 2079 6f75 2068 6176 6520 6368 6f73  n` you have chos
+0000f030: 656e 2c20 6f72 0a20 2020 2020 2020 2020  en, or.         
+0000f040: 2020 2020 2020 2079 6f75 2073 686f 756c         you shoul
+0000f050: 6420 6861 7665 2074 6865 2050 726f 6a65  d have the Proje
+0000f060: 6374 2049 414d 2041 646d 696e 2072 6f6c  ct IAM Admin rol
+0000f070: 6520 746f 2065 6e61 626c 6520 7468 6520  e to enable the 
+0000f080: 7365 7276 6963 650a 2020 2020 2020 2020  service.        
+0000f090: 2020 2020 2020 2020 746f 2063 7265 6174          to creat
+0000f0a0: 6520 7468 6520 636f 6e6e 6563 7469 6f6e  e the connection
+0000f0b0: 2066 6f72 2079 6f75 2069 6620 796f 7520   for you if you 
+0000f0c0: 6e65 6564 2069 742e 2049 6620 7468 6973  need it. If this
+0000f0d0: 2070 6172 616d 6574 6572 2069 730a 2020   parameter is.  
+0000f0e0: 2020 2020 2020 2020 2020 2020 2020 6e6f                no
+0000f0f0: 7420 7072 6f76 6964 6564 2074 6865 6e20  t provided then 
+0000f100: 7468 6520 4269 6751 7565 7279 2063 6f6e  the BigQuery con
+0000f110: 6e65 6374 696f 6e20 6672 6f6d 2074 6865  nection from the
+0000f120: 2073 6573 7369 6f6e 2069 7320 7573 6564   session is used
+0000f130: 2e0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+0000f140: 7573 6520 2862 6f6f 6c2c 204f 7074 696f  use (bool, Optio
+0000f150: 6e61 6c29 3a0a 2020 2020 2020 2020 2020  nal):.          
+0000f160: 2020 2020 2020 5265 7573 6520 7468 6520        Reuse the 
+0000f170: 7265 6d6f 7465 2066 756e 6374 696f 6e20  remote function 
+0000f180: 6966 2061 6c72 6561 6479 2065 7869 7374  if already exist
+0000f190: 732e 0a20 2020 2020 2020 2020 2020 2020  s..             
+0000f1a0: 2020 2060 5472 7565 6020 6279 2064 6566     `True` by def
+0000f1b0: 6175 6c74 2c20 7768 6963 6820 7769 6c6c  ault, which will
+0000f1c0: 2072 6573 756c 7420 696e 2072 6575 7369   result in reusi
+0000f1d0: 6e67 2061 6e20 6578 6973 7469 6e67 2072  ng an existing r
+0000f1e0: 656d 6f74 650a 2020 2020 2020 2020 2020  emote.          
+0000f1f0: 2020 2020 2020 6675 6e63 7469 6f6e 2061        function a
+0000f200: 6e64 2063 6f72 7265 7370 6f6e 6469 6e67  nd corresponding
+0000f210: 2063 6c6f 7564 2066 756e 6374 696f 6e20   cloud function 
+0000f220: 2869 6620 616e 7929 2074 6861 7420 7761  (if any) that wa
+0000f230: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
+0000f240: 2020 7072 6576 696f 7573 6c79 2063 7265    previously cre
+0000f250: 6174 6564 2066 6f72 2074 6865 2073 616d  ated for the sam
+0000f260: 6520 7564 662e 0a20 2020 2020 2020 2020  e udf..         
+0000f270: 2020 2020 2020 2053 6574 7469 6e67 2069         Setting i
+0000f280: 7420 746f 2060 4661 6c73 6560 2077 6f75  t to `False` wou
+0000f290: 6c64 2066 6f72 6365 2063 7265 6174 696e  ld force creatin
+0000f2a0: 6720 6120 756e 6971 7565 2072 656d 6f74  g a unique remot
+0000f2b0: 6520 6675 6e63 7469 6f6e 2e0a 2020 2020  e function..    
+0000f2c0: 2020 2020 2020 2020 2020 2020 4966 2074              If t
+0000f2d0: 6865 2072 6571 7569 7265 6420 7265 6d6f  he required remo
+0000f2e0: 7465 2066 756e 6374 696f 6e20 646f 6573  te function does
+0000f2f0: 206e 6f74 2065 7869 7374 2074 6865 6e20   not exist then 
+0000f300: 6974 2077 6f75 6c64 2062 650a 2020 2020  it would be.    
+0000f310: 2020 2020 2020 2020 2020 2020 6372 6561              crea
+0000f320: 7465 6420 6972 7265 7370 6563 7469 7665  ted irrespective
+0000f330: 206f 6620 7468 6973 2070 6172 616d 2e0a   of this param..
+0000f340: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
+0000f350: 2028 7374 722c 204f 7074 696f 6e61 6c29   (str, Optional)
+0000f360: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000f370: 2020 4578 706c 6963 6974 206e 616d 6520    Explicit name 
+0000f380: 6f66 2074 6865 2070 6572 7369 7374 6564  of the persisted
+0000f390: 2042 6967 5175 6572 7920 7265 6d6f 7465   BigQuery remote
+0000f3a0: 2066 756e 6374 696f 6e2e 2055 7365 2069   function. Use i
+0000f3b0: 7420 7769 7468 0a20 2020 2020 2020 2020  t with.         
+0000f3c0: 2020 2020 2020 2063 6175 7469 6f6e 2c20         caution, 
+0000f3d0: 6265 6361 7573 6520 7477 6f20 7573 6572  because two user
+0000f3e0: 7320 776f 726b 696e 6720 696e 2074 6865  s working in the
+0000f3f0: 2073 616d 6520 7072 6f6a 6563 7420 616e   same project an
+0000f400: 6420 6461 7461 7365 740a 2020 2020 2020  d dataset.      
+0000f410: 2020 2020 2020 2020 2020 636f 756c 6420            could 
+0000f420: 6f76 6572 7772 6974 6520 6561 6368 206f  overwrite each o
+0000f430: 7468 6572 2773 2072 656d 6f74 6520 6675  ther's remote fu
+0000f440: 6e63 7469 6f6e 7320 6966 2074 6865 7920  nctions if they 
+0000f450: 7573 6520 7468 6520 7361 6d65 0a20 2020  use the same.   
+0000f460: 2020 2020 2020 2020 2020 2020 2070 6572               per
+0000f470: 7369 7374 656e 7420 6e61 6d65 2e0a 2020  sistent name..  
+0000f480: 2020 2020 2020 2020 2020 7061 636b 6167            packag
+0000f490: 6573 2028 7374 725b 5d2c 204f 7074 696f  es (str[], Optio
+0000f4a0: 6e61 6c29 3a0a 2020 2020 2020 2020 2020  nal):.          
+0000f4b0: 2020 2020 2020 4578 706c 6963 6974 206e        Explicit n
+0000f4c0: 616d 6520 6f66 2074 6865 2065 7874 6572  ame of the exter
+0000f4d0: 6e61 6c20 7061 636b 6167 6520 6465 7065  nal package depe
+0000f4e0: 6e64 656e 6369 6573 2e20 4561 6368 2064  ndencies. Each d
+0000f4f0: 6570 656e 6465 6e63 790a 2020 2020 2020  ependency.      
+0000f500: 2020 2020 2020 2020 2020 6973 2061 6464            is add
+0000f510: 6564 2074 6f20 7468 6520 6072 6571 7569  ed to the `requi
+0000f520: 7265 6d65 6e74 732e 7478 7460 2061 7320  rements.txt` as 
+0000f530: 6973 2c20 616e 6420 6361 6e20 6265 206f  is, and can be o
+0000f540: 6620 7468 6520 666f 726d 0a20 2020 2020  f the form.     
+0000f550: 2020 2020 2020 2020 2020 2073 7570 706f             suppo
+0000f560: 7274 6564 2069 6e20 6874 7470 733a 2f2f  rted in https://
+0000f570: 7069 702e 7079 7061 2e69 6f2f 656e 2f73  pip.pypa.io/en/s
+0000f580: 7461 626c 652f 7265 6665 7265 6e63 652f  table/reference/
+0000f590: 7265 7175 6972 656d 656e 7473 2d66 696c  requirements-fil
+0000f5a0: 652d 666f 726d 6174 2f2e 0a20 2020 2020  e-format/..     
+0000f5b0: 2020 2020 2020 2063 6c6f 7564 5f66 756e         cloud_fun
+0000f5c0: 6374 696f 6e5f 7365 7276 6963 655f 6163  ction_service_ac
+0000f5d0: 636f 756e 7420 2873 7472 2c20 4f70 7469  count (str, Opti
+0000f5e0: 6f6e 616c 293a 0a20 2020 2020 2020 2020  onal):.         
+0000f5f0: 2020 2020 2020 2053 6572 7669 6365 2061         Service a
+0000f600: 6363 6f75 6e74 2074 6f20 7573 6520 666f  ccount to use fo
+0000f610: 7220 7468 6520 636c 6f75 6420 6675 6e63  r the cloud func
+0000f620: 7469 6f6e 732e 2049 6620 6e6f 7420 7072  tions. If not pr
+0000f630: 6f76 6964 6564 0a20 2020 2020 2020 2020  ovided.         
+0000f640: 2020 2020 2020 2074 6865 6e20 7468 6520         then the 
+0000f650: 6465 6661 756c 7420 7365 7276 6963 6520  default service 
+0000f660: 6163 636f 756e 7420 776f 756c 6420 6265  account would be
+0000f670: 2075 7365 642e 2053 6565 0a20 2020 2020   used. See.     
+0000f680: 2020 2020 2020 2020 2020 2068 7474 7073             https
+0000f690: 3a2f 2f63 6c6f 7564 2e67 6f6f 676c 652e  ://cloud.google.
+0000f6a0: 636f 6d2f 6675 6e63 7469 6f6e 732f 646f  com/functions/do
+0000f6b0: 6373 2f73 6563 7572 696e 672f 6675 6e63  cs/securing/func
+0000f6c0: 7469 6f6e 2d69 6465 6e74 6974 790a 2020  tion-identity.  
+0000f6d0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+0000f6e0: 7220 6d6f 7265 2064 6574 6169 6c73 2e20  r more details. 
+0000f6f0: 506c 6561 7365 206d 616b 6520 7375 7265  Please make sure
+0000f700: 2074 6865 2073 6572 7669 6365 2061 6363   the service acc
+0000f710: 6f75 6e74 2068 6173 2074 6865 0a20 2020  ount has the.   
+0000f720: 2020 2020 2020 2020 2020 2020 206e 6563               nec
+0000f730: 6573 7361 7279 2049 414d 2070 6572 6d69  essary IAM permi
+0000f740: 7373 696f 6e73 2063 6f6e 6669 6775 7265  ssions configure
+0000f750: 6420 6173 2064 6573 6372 6962 6564 2069  d as described i
+0000f760: 6e0a 2020 2020 2020 2020 2020 2020 2020  n.              
+0000f770: 2020 6874 7470 733a 2f2f 636c 6f75 642e    https://cloud.
+0000f780: 676f 6f67 6c65 2e63 6f6d 2f66 756e 6374  google.com/funct
+0000f790: 696f 6e73 2f64 6f63 732f 7265 6665 7265  ions/docs/refere
+0000f7a0: 6e63 652f 6961 6d2f 726f 6c65 7323 6164  nce/iam/roles#ad
+0000f7b0: 6469 7469 6f6e 616c 2d63 6f6e 6669 6775  ditional-configu
+0000f7c0: 7261 7469 6f6e 2e0a 2020 2020 2020 2020  ration..        
+0000f7d0: 2020 2020 636c 6f75 645f 6675 6e63 7469      cloud_functi
+0000f7e0: 6f6e 5f6b 6d73 5f6b 6579 5f6e 616d 6520  on_kms_key_name 
+0000f7f0: 2873 7472 2c20 4f70 7469 6f6e 616c 293a  (str, Optional):
+0000f800: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f810: 2043 7573 746f 6d65 7220 6d61 6e61 6765   Customer manage
+0000f820: 6420 656e 6372 7970 7469 6f6e 206b 6579  d encryption key
+0000f830: 2074 6f20 7072 6f74 6563 7420 636c 6f75   to protect clou
+0000f840: 6420 6675 6e63 7469 6f6e 7320 616e 640a  d functions and.
+0000f850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f860: 7265 6c61 7465 6420 6461 7461 2061 7420  related data at 
+0000f870: 7265 7374 2e20 5468 6973 2069 7320 6f66  rest. This is of
+0000f880: 2074 6865 2066 6f72 6d61 740a 2020 2020   the format.    
+0000f890: 2020 2020 2020 2020 2020 2020 7072 6f6a              proj
+0000f8a0: 6563 7473 2f50 524f 4a45 4354 5f49 442f  ects/PROJECT_ID/
+0000f8b0: 6c6f 6361 7469 6f6e 732f 4c4f 4341 5449  locations/LOCATI
+0000f8c0: 4f4e 2f6b 6579 5269 6e67 732f 4b45 5952  ON/keyRings/KEYR
+0000f8d0: 494e 472f 6372 7970 746f 4b65 7973 2f4b  ING/cryptoKeys/K
+0000f8e0: 4559 2e0a 2020 2020 2020 2020 2020 2020  EY..            
+0000f8f0: 2020 2020 5265 6164 2068 7474 7073 3a2f      Read https:/
+0000f900: 2f63 6c6f 7564 2e67 6f6f 676c 652e 636f  /cloud.google.co
+0000f910: 6d2f 6675 6e63 7469 6f6e 732f 646f 6373  m/functions/docs
+0000f920: 2f73 6563 7572 696e 672f 636d 656b 2066  /securing/cmek f
+0000f930: 6f72 0a20 2020 2020 2020 2020 2020 2020  or.             
+0000f940: 2020 206d 6f72 6520 6465 7461 696c 7320     more details 
+0000f950: 696e 636c 7564 696e 6720 6772 616e 7469  including granti
+0000f960: 6e67 206e 6563 6573 7361 7279 2073 6572  ng necessary ser
+0000f970: 7669 6365 2061 6363 6f75 6e74 730a 2020  vice accounts.  
+0000f980: 2020 2020 2020 2020 2020 2020 2020 6163                ac
+0000f990: 6365 7373 2074 6f20 7468 6520 6b65 792e  cess to the key.
+0000f9a0: 0a20 2020 2020 2020 2020 2020 2063 6c6f  .            clo
+0000f9b0: 7564 5f66 756e 6374 696f 6e5f 646f 636b  ud_function_dock
+0000f9c0: 6572 5f72 6570 6f73 6974 6f72 7920 2873  er_repository (s
+0000f9d0: 7472 2c20 4f70 7469 6f6e 616c 293a 0a20  tr, Optional):. 
+0000f9e0: 2020 2020 2020 2020 2020 2020 2020 2044                 D
+0000f9f0: 6f63 6b65 7220 7265 706f 7369 746f 7279  ocker repository
+0000fa00: 2063 7265 6174 6564 2077 6974 6820 7468   created with th
+0000fa10: 6520 7361 6d65 2065 6e63 7279 7074 696f  e same encryptio
+0000fa20: 6e20 6b65 7920 6173 0a20 2020 2020 2020  n key as.       
+0000fa30: 2020 2020 2020 2020 2060 636c 6f75 645f           `cloud_
+0000fa40: 6675 6e63 7469 6f6e 5f6b 6d73 5f6b 6579  function_kms_key
+0000fa50: 5f6e 616d 6560 2074 6f20 7374 6f72 6520  _name` to store 
+0000fa60: 656e 6372 7970 7465 6420 6172 7469 6661  encrypted artifa
+0000fa70: 6374 730a 2020 2020 2020 2020 2020 2020  cts.            
+0000fa80: 2020 2020 6372 6561 7465 6420 746f 2073      created to s
+0000fa90: 7570 706f 7274 2074 6865 2063 6c6f 7564  upport the cloud
+0000faa0: 2066 756e 6374 696f 6e2e 2054 6869 7320   function. This 
+0000fab0: 6973 206f 6620 7468 6520 666f 726d 6174  is of the format
+0000fac0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000fad0: 2070 726f 6a65 6374 732f 5052 4f4a 4543   projects/PROJEC
+0000fae0: 545f 4944 2f6c 6f63 6174 696f 6e73 2f4c  T_ID/locations/L
+0000faf0: 4f43 4154 494f 4e2f 7265 706f 7369 746f  OCATION/reposito
+0000fb00: 7269 6573 2f52 4550 4f53 4954 4f52 595f  ries/REPOSITORY_
+0000fb10: 4e41 4d45 2e0a 2020 2020 2020 2020 2020  NAME..          
+0000fb20: 2020 2020 2020 466f 7220 6d6f 7265 2064        For more d
+0000fb30: 6574 6169 6c73 2073 6565 0a20 2020 2020  etails see.     
+0000fb40: 2020 2020 2020 2020 2020 2068 7474 7073             https
+0000fb50: 3a2f 2f63 6c6f 7564 2e67 6f6f 676c 652e  ://cloud.google.
+0000fb60: 636f 6d2f 6675 6e63 7469 6f6e 732f 646f  com/functions/do
+0000fb70: 6373 2f73 6563 7572 696e 672f 636d 656b  cs/securing/cmek
+0000fb80: 2362 6566 6f72 655f 796f 755f 6265 6769  #before_you_begi
+0000fb90: 6e2e 0a20 2020 2020 2020 2052 6574 7572  n..        Retur
+0000fba0: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
+0000fbb0: 6361 6c6c 6162 6c65 3a20 4120 7265 6d6f  callable: A remo
+0000fbc0: 7465 2066 756e 6374 696f 6e20 6f62 6a65  te function obje
+0000fbd0: 6374 2070 6f69 6e74 696e 6720 746f 2074  ct pointing to t
+0000fbe0: 6865 2063 6c6f 7564 2061 7373 6574 7320  he cloud assets 
+0000fbf0: 6372 6561 7465 640a 2020 2020 2020 2020  created.        
+0000fc00: 2020 2020 696e 2074 6865 2062 6163 6b67      in the backg
+0000fc10: 726f 756e 6420 746f 2073 7570 706f 7274  round to support
+0000fc20: 2074 6865 2072 656d 6f74 6520 6578 6563   the remote exec
+0000fc30: 7574 696f 6e2e 2054 6865 2063 6c6f 7564  ution. The cloud
+0000fc40: 2061 7373 6574 7320 6361 6e20 6265 0a20   assets can be. 
+0000fc50: 2020 2020 2020 2020 2020 206c 6f63 6174             locat
+0000fc60: 6564 2074 6872 6f75 6768 2074 6865 2066  ed through the f
+0000fc70: 6f6c 6c6f 7769 6e67 2070 726f 7065 7274  ollowing propert
+0000fc80: 6965 7320 7365 7420 696e 2074 6865 206f  ies set in the o
+0000fc90: 626a 6563 743a 0a0a 2020 2020 2020 2020  bject:..        
+0000fca0: 2020 2020 6062 6967 6672 616d 6573 5f63      `bigframes_c
+0000fcb0: 6c6f 7564 5f66 756e 6374 696f 6e60 202d  loud_function` -
+0000fcc0: 2054 6865 2067 6f6f 676c 6520 636c 6f75   The google clou
+0000fcd0: 6420 6675 6e63 7469 6f6e 2064 6570 6c6f  d function deplo
+0000fce0: 7965 6420 666f 7220 7468 6520 7573 6572  yed for the user
+0000fcf0: 2064 6566 696e 6564 2063 6f64 652e 0a0a   defined code...
+0000fd00: 2020 2020 2020 2020 2020 2020 6062 6967              `big
+0000fd10: 6672 616d 6573 5f72 656d 6f74 655f 6675  frames_remote_fu
+0000fd20: 6e63 7469 6f6e 6020 2d20 5468 6520 6269  nction` - The bi
+0000fd30: 6771 7565 7279 2072 656d 6f74 6520 6675  gquery remote fu
+0000fd40: 6e63 7469 6f6e 2063 6170 6162 6c65 206f  nction capable o
+0000fd50: 6620 6361 6c6c 696e 6720 696e 746f 2060  f calling into `
+0000fd60: 6269 6766 7261 6d65 735f 636c 6f75 645f  bigframes_cloud_
+0000fd70: 6675 6e63 7469 6f6e 602e 0a20 2020 2020  function`..     
+0000fd80: 2020 2022 2222 0a20 2020 2020 2020 2072     """.        r
+0000fd90: 6574 7572 6e20 6269 6766 7261 6d65 735f  eturn bigframes_
+0000fda0: 7266 280a 2020 2020 2020 2020 2020 2020  rf(.            
+0000fdb0: 696e 7075 745f 7479 7065 732c 0a20 2020  input_types,.   
+0000fdc0: 2020 2020 2020 2020 206f 7574 7075 745f           output_
+0000fdd0: 7479 7065 2c0a 2020 2020 2020 2020 2020  type,.          
+0000fde0: 2020 7365 7373 696f 6e3d 7365 6c66 2c0a    session=self,.
+0000fdf0: 2020 2020 2020 2020 2020 2020 6461 7461              data
+0000fe00: 7365 743d 6461 7461 7365 742c 0a20 2020  set=dataset,.   
+0000fe10: 2020 2020 2020 2020 2062 6967 7175 6572           bigquer
+0000fe20: 795f 636f 6e6e 6563 7469 6f6e 3d62 6967  y_connection=big
+0000fe30: 7175 6572 795f 636f 6e6e 6563 7469 6f6e  query_connection
+0000fe40: 2c0a 2020 2020 2020 2020 2020 2020 7265  ,.            re
+0000fe50: 7573 653d 7265 7573 652c 0a20 2020 2020  use=reuse,.     
+0000fe60: 2020 2020 2020 206e 616d 653d 6e61 6d65         name=name
+0000fe70: 2c0a 2020 2020 2020 2020 2020 2020 7061  ,.            pa
+0000fe80: 636b 6167 6573 3d70 6163 6b61 6765 732c  ckages=packages,
+0000fe90: 0a20 2020 2020 2020 2020 2020 2063 6c6f  .            clo
+0000fea0: 7564 5f66 756e 6374 696f 6e5f 7365 7276  ud_function_serv
+0000feb0: 6963 655f 6163 636f 756e 743d 636c 6f75  ice_account=clou
+0000fec0: 645f 6675 6e63 7469 6f6e 5f73 6572 7669  d_function_servi
+0000fed0: 6365 5f61 6363 6f75 6e74 2c0a 2020 2020  ce_account,.    
+0000fee0: 2020 2020 2020 2020 636c 6f75 645f 6675          cloud_fu
+0000fef0: 6e63 7469 6f6e 5f6b 6d73 5f6b 6579 5f6e  nction_kms_key_n
+0000ff00: 616d 653d 636c 6f75 645f 6675 6e63 7469  ame=cloud_functi
+0000ff10: 6f6e 5f6b 6d73 5f6b 6579 5f6e 616d 652c  on_kms_key_name,
+0000ff20: 0a20 2020 2020 2020 2020 2020 2063 6c6f  .            clo
+0000ff30: 7564 5f66 756e 6374 696f 6e5f 646f 636b  ud_function_dock
+0000ff40: 6572 5f72 6570 6f73 6974 6f72 793d 636c  er_repository=cl
+0000ff50: 6f75 645f 6675 6e63 7469 6f6e 5f64 6f63  oud_function_doc
+0000ff60: 6b65 725f 7265 706f 7369 746f 7279 2c0a  ker_repository,.
+0000ff70: 2020 2020 2020 2020 290a 0a20 2020 2064          )..    d
+0000ff80: 6566 2072 6561 645f 6762 715f 6675 6e63  ef read_gbq_func
+0000ff90: 7469 6f6e 280a 2020 2020 2020 2020 7365  tion(.        se
+0000ffa0: 6c66 2c0a 2020 2020 2020 2020 6675 6e63  lf,.        func
+0000ffb0: 7469 6f6e 5f6e 616d 653a 2073 7472 2c0a  tion_name: str,.
+0000ffc0: 2020 2020 293a 0a20 2020 2020 2020 2022      ):.        "
+0000ffd0: 2222 4c6f 6164 7320 6120 4269 6751 7565  ""Loads a BigQue
+0000ffe0: 7279 2066 756e 6374 696f 6e20 6672 6f6d  ry function from
+0000fff0: 2042 6967 5175 6572 792e 0a0a 2020 2020   BigQuery...    
+00010000: 2020 2020 5468 656e 2069 7420 6361 6e20      Then it can 
+00010010: 6265 2061 7070 6c69 6564 2074 6f20 6120  be applied to a 
+00010020: 4461 7461 4672 616d 6520 6f72 2053 6572  DataFrame or Ser
+00010030: 6965 732e 0a0a 2020 2020 2020 2020 2e2e  ies...        ..
+00010040: 206e 6f74 653a 3a0a 2020 2020 2020 2020   note::.        
+00010050: 2020 2020 5468 6520 7265 7475 726e 2074      The return t
+00010060: 7970 6520 6f66 2074 6865 2066 756e 6374  ype of the funct
+00010070: 696f 6e20 6d75 7374 2062 6520 6578 706c  ion must be expl
+00010080: 6963 6974 6c79 2073 7065 6369 6669 6564  icitly specified
+00010090: 2069 6e20 7468 650a 2020 2020 2020 2020   in the.        
+000100a0: 2020 2020 6675 6e63 7469 6f6e 2773 206f      function's o
+000100b0: 7269 6769 6e61 6c20 6465 6669 6e69 7469  riginal definiti
+000100c0: 6f6e 2065 7665 6e20 6966 206e 6f74 206f  on even if not o
+000100d0: 7468 6572 7769 7365 2072 6571 7569 7265  therwise require
+000100e0: 642e 0a0a 2020 2020 2020 2020 4269 6751  d...        BigQ
+000100f0: 7565 7279 2055 7469 6c73 2070 726f 7669  uery Utils provi
+00010100: 6465 7320 6d61 6e79 2070 7562 6c69 6320  des many public 
+00010110: 6675 6e63 7469 6f6e 7320 756e 6465 7220  functions under 
+00010120: 7468 6520 6060 6271 7574 696c 6060 2070  the ``bqutil`` p
+00010130: 726f 6a65 6374 206f 6e20 476f 6f67 6c65  roject on Google
+00010140: 2043 6c6f 7564 2050 6c61 7466 6f72 6d20   Cloud Platform 
+00010150: 7072 6f6a 6563 740a 2020 2020 2020 2020  project.        
+00010160: 2853 6565 3a20 6874 7470 733a 2f2f 6769  (See: https://gi
+00010170: 7468 7562 2e63 6f6d 2f47 6f6f 676c 6543  thub.com/GoogleC
+00010180: 6c6f 7564 506c 6174 666f 726d 2f62 6967  loudPlatform/big
+00010190: 7175 6572 792d 7574 696c 732f 7472 6565  query-utils/tree
+000101a0: 2f6d 6173 7465 722f 7564 6673 2375 7369  /master/udfs#usi
+000101b0: 6e67 2d74 6865 2d75 6466 7329 2e0a 2020  ng-the-udfs)..  
+000101c0: 2020 2020 2020 596f 7520 6361 6e20 6368        You can ch
+000101d0: 6563 6b6f 7574 2043 6f6d 6d75 6e69 7479  eckout Community
+000101e0: 2055 4446 7320 746f 2075 7365 2063 6f6d   UDFs to use com
+000101f0: 6d75 6e69 7479 2d63 6f6e 7472 6962 7574  munity-contribut
+00010200: 6564 2066 756e 6374 696f 6e73 2e0a 2020  ed functions..  
+00010210: 2020 2020 2020 2853 6565 3a20 6874 7470        (See: http
+00010220: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f47  s://github.com/G
+00010230: 6f6f 676c 6543 6c6f 7564 506c 6174 666f  oogleCloudPlatfo
+00010240: 726d 2f62 6967 7175 6572 792d 7574 696c  rm/bigquery-util
+00010250: 732f 7472 6565 2f6d 6173 7465 722f 7564  s/tree/master/ud
+00010260: 6673 2f63 6f6d 6d75 6e69 7479 2363 6f6d  fs/community#com
+00010270: 6d75 6e69 7479 2d75 6466 7329 2e0a 0a20  munity-udfs)... 
+00010280: 2020 2020 2020 202a 2a45 7861 6d70 6c65         **Example
+00010290: 733a 2a2a 0a0a 2020 2020 2020 2020 5573  s:**..        Us
+000102a0: 6520 7468 6520 6060 6377 5f6c 6f77 6572  e the ``cw_lower
+000102b0: 5f63 6173 655f 6173 6369 695f 6f6e 6c79  _case_ascii_only
+000102c0: 6060 2066 756e 6374 696f 6e20 6672 6f6d  `` function from
+000102d0: 2043 6f6d 6d75 6e69 7479 2055 4446 732e   Community UDFs.
+000102e0: 0a20 2020 2020 2020 2028 6874 7470 733a  .        (https:
+000102f0: 2f2f 6769 7468 7562 2e63 6f6d 2f47 6f6f  //github.com/Goo
+00010300: 676c 6543 6c6f 7564 506c 6174 666f 726d  gleCloudPlatform
+00010310: 2f62 6967 7175 6572 792d 7574 696c 732f  /bigquery-utils/
+00010320: 626c 6f62 2f6d 6173 7465 722f 7564 6673  blob/master/udfs
+00010330: 2f63 6f6d 6d75 6e69 7479 2f63 775f 6c6f  /community/cw_lo
+00010340: 7765 725f 6361 7365 5f61 7363 6969 5f6f  wer_case_ascii_o
+00010350: 6e6c 792e 7371 6c78 290a 0a20 2020 2020  nly.sqlx)..     
+00010360: 2020 2020 2020 203e 3e3e 2069 6d70 6f72         >>> impor
+00010370: 7420 6269 6766 7261 6d65 732e 7061 6e64  t bigframes.pand
+00010380: 6173 2061 7320 6270 640a 2020 2020 2020  as as bpd.      
+00010390: 2020 2020 2020 3e3e 3e20 6270 642e 6f70        >>> bpd.op
+000103a0: 7469 6f6e 732e 6469 7370 6c61 792e 7072  tions.display.pr
+000103b0: 6f67 7265 7373 5f62 6172 203d 204e 6f6e  ogress_bar = Non
+000103c0: 650a 0a20 2020 2020 2020 2020 2020 203e  e..            >
+000103d0: 3e3e 2064 6620 3d20 6270 642e 4461 7461  >> df = bpd.Data
+000103e0: 4672 616d 6528 7b27 6964 273a 205b 312c  Frame({'id': [1,
+000103f0: 2032 2c20 335d 2c20 276e 616d 6527 3a20   2, 3], 'name': 
+00010400: 5b27 4155 52c3 894c 4945 272c 2027 43c3  ['AUR..LIE', 'C.
+00010410: 894c 4553 5449 4e45 272c 2027 4441 5048  .LESTINE', 'DAPH
+00010420: 4ec3 8927 5d7d 290a 2020 2020 2020 2020  N..']}).        
+00010430: 2020 2020 3e3e 3e20 6466 0a20 2020 2020      >>> df.     
+00010440: 2020 2020 2020 2020 2020 6964 2020 2020            id    
+00010450: 2020 206e 616d 650a 2020 2020 2020 2020     name.        
+00010460: 2020 2020 3020 2020 3120 2020 2041 5552      0   1    AUR
+00010470: c389 4c49 450a 2020 2020 2020 2020 2020  ..LIE.          
+00010480: 2020 3120 2020 3220 2043 c389 4c45 5354    1   2  C..LEST
+00010490: 494e 450a 2020 2020 2020 2020 2020 2020  INE.            
+000104a0: 3220 2020 3320 2020 2020 4441 5048 4ec3  2   3     DAPHN.
+000104b0: 890a 2020 2020 2020 2020 2020 2020 3c42  ..            <B
+000104c0: 4c41 4e4b 4c49 4e45 3e0a 2020 2020 2020  LANKLINE>.      
+000104d0: 2020 2020 2020 5b33 2072 6f77 7320 7820        [3 rows x 
+000104e0: 3220 636f 6c75 6d6e 735d 0a0a 2020 2020  2 columns]..    
+000104f0: 2020 2020 2020 2020 3e3e 3e20 6675 6e63          >>> func
+00010500: 203d 2062 7064 2e72 6561 645f 6762 715f   = bpd.read_gbq_
+00010510: 6675 6e63 7469 6f6e 2822 6271 7574 696c  function("bqutil
+00010520: 2e66 6e2e 6377 5f6c 6f77 6572 5f63 6173  .fn.cw_lower_cas
+00010530: 655f 6173 6369 695f 6f6e 6c79 2229 0a20  e_ascii_only"). 
+00010540: 2020 2020 2020 2020 2020 203e 3e3e 2064             >>> d
+00010550: 6631 203d 2064 662e 6173 7369 676e 286e  f1 = df.assign(n
+00010560: 6577 5f6e 616d 653d 6466 5b27 6e61 6d65  ew_name=df['name
+00010570: 275d 2e61 7070 6c79 2866 756e 6329 290a  '].apply(func)).
+00010580: 2020 2020 2020 2020 2020 2020 3e3e 3e20              >>> 
+00010590: 6466 310a 2020 2020 2020 2020 2020 2020  df1.            
+000105a0: 2020 2069 6420 2020 2020 2020 6e61 6d65     id       name
+000105b0: 2020 206e 6577 5f6e 616d 650a 2020 2020     new_name.    
+000105c0: 2020 2020 2020 2020 3020 2020 3120 2020          0   1   
+000105d0: 2041 5552 c389 4c49 4520 2020 2061 7572   AUR..LIE    aur
+000105e0: c389 6c69 650a 2020 2020 2020 2020 2020  ..lie.          
+000105f0: 2020 3120 2020 3220 2043 c389 4c45 5354    1   2  C..LEST
+00010600: 494e 4520 2063 c389 6c65 7374 696e 650a  INE  c..lestine.
+00010610: 2020 2020 2020 2020 2020 2020 3220 2020              2   
+00010620: 3320 2020 2020 4441 5048 4ec3 8920 2020  3     DAPHN..   
+00010630: 2020 6461 7068 6ec3 890a 2020 2020 2020    daphn...      
+00010640: 2020 2020 2020 3c42 4c41 4e4b 4c49 4e45        <BLANKLINE
+00010650: 3e0a 2020 2020 2020 2020 2020 2020 5b33  >.            [3
+00010660: 2072 6f77 7320 7820 3320 636f 6c75 6d6e   rows x 3 column
+00010670: 735d 0a0a 2020 2020 2020 2020 4172 6773  s]..        Args
+00010680: 3a0a 2020 2020 2020 2020 2020 2020 6675  :.            fu
+00010690: 6e63 7469 6f6e 5f6e 616d 6520 2873 7472  nction_name (str
+000106a0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+000106b0: 2020 2074 6865 2066 756e 6374 696f 6e27     the function'
+000106c0: 7320 6e61 6d65 2069 6e20 4269 6751 7565  s name in BigQue
+000106d0: 7279 2069 6e20 7468 6520 666f 726d 6174  ry in the format
+000106e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000106f0: 2060 7072 6f6a 6563 745f 6964 2e64 6174   `project_id.dat
+00010700: 6173 6574 5f69 642e 6675 6e63 7469 6f6e  aset_id.function
+00010710: 5f6e 616d 6560 2c20 6f72 0a20 2020 2020  _name`, or.     
+00010720: 2020 2020 2020 2020 2020 2060 6461 7461             `data
+00010730: 7365 745f 6964 2e66 756e 6374 696f 6e5f  set_id.function_
+00010740: 6e61 6d65 6020 746f 206c 6f61 6420 6672  name` to load fr
+00010750: 6f6d 2074 6865 2064 6566 6175 6c74 2070  om the default p
+00010760: 726f 6a65 6374 2c20 6f72 0a20 2020 2020  roject, or.     
+00010770: 2020 2020 2020 2020 2020 2060 6675 6e63             `func
+00010780: 7469 6f6e 5f6e 616d 6560 2074 6f20 6c6f  tion_name` to lo
+00010790: 6164 2066 726f 6d20 7468 6520 6465 6661  ad from the defa
+000107a0: 756c 7420 7072 6f6a 6563 7420 616e 6420  ult project and 
+000107b0: 7468 6520 6461 7461 7365 740a 2020 2020  the dataset.    
+000107c0: 2020 2020 2020 2020 2020 2020 6173 736f              asso
+000107d0: 6369 6174 6564 2077 6974 6820 7468 6520  ciated with the 
+000107e0: 6375 7272 656e 7420 7365 7373 696f 6e2e  current session.
+000107f0: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+00010800: 733a 0a20 2020 2020 2020 2020 2020 2063  s:.            c
+00010810: 616c 6c61 626c 653a 2041 2066 756e 6374  allable: A funct
+00010820: 696f 6e20 6f62 6a65 6374 2070 6f69 6e74  ion object point
+00010830: 696e 6720 746f 2074 6865 2042 6967 5175  ing to the BigQu
+00010840: 6572 7920 6675 6e63 7469 6f6e 2072 6561  ery function rea
+00010850: 640a 2020 2020 2020 2020 2020 2020 6672  d.            fr
+00010860: 6f6d 2042 6967 5175 6572 792e 0a0a 2020  om BigQuery...  
+00010870: 2020 2020 2020 2020 2020 5468 6520 6f62            The ob
+00010880: 6a65 6374 2069 7320 7369 6d69 6c61 7220  ject is similar 
+00010890: 746f 2074 6865 206f 6e65 2063 7265 6174  to the one creat
+000108a0: 6564 2062 7920 7468 6520 6072 656d 6f74  ed by the `remot
+000108b0: 655f 6675 6e63 7469 6f6e 600a 2020 2020  e_function`.    
+000108c0: 2020 2020 2020 2020 6465 636f 7261 746f          decorato
+000108d0: 722c 2069 6e63 6c75 6469 6e67 2074 6865  r, including the
+000108e0: 2060 6269 6766 7261 6d65 735f 7265 6d6f   `bigframes_remo
+000108f0: 7465 5f66 756e 6374 696f 6e60 2070 726f  te_function` pro
+00010900: 7065 7274 792c 2062 7574 0a20 2020 2020  perty, but.     
+00010910: 2020 2020 2020 206e 6f74 2069 6e63 6c75         not inclu
+00010920: 6469 6e67 2074 6865 2060 6269 6766 7261  ding the `bigfra
+00010930: 6d65 735f 636c 6f75 645f 6675 6e63 7469  mes_cloud_functi
+00010940: 6f6e 6020 7072 6f70 6572 7479 2e0a 2020  on` property..  
+00010950: 2020 2020 2020 2222 220a 0a20 2020 2020        """..     
+00010960: 2020 2072 6574 7572 6e20 6269 6766 7261     return bigfra
+00010970: 6d65 735f 7267 6628 0a20 2020 2020 2020  mes_rgf(.       
+00010980: 2020 2020 2066 756e 6374 696f 6e5f 6e61       function_na
+00010990: 6d65 3d66 756e 6374 696f 6e5f 6e61 6d65  me=function_name
+000109a0: 2c0a 2020 2020 2020 2020 2020 2020 7365  ,.            se
+000109b0: 7373 696f 6e3d 7365 6c66 2c0a 2020 2020  ssion=self,.    
+000109c0: 2020 2020 290a 0a20 2020 2064 6566 205f      )..    def _
+000109d0: 7072 6570 6172 655f 7175 6572 795f 6a6f  prepare_query_jo
+000109e0: 625f 636f 6e66 6967 280a 2020 2020 2020  b_config(.      
+000109f0: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
+00010a00: 6a6f 625f 636f 6e66 6967 3a20 4f70 7469  job_config: Opti
+00010a10: 6f6e 616c 5b62 6967 7175 6572 792e 5175  onal[bigquery.Qu
+00010a20: 6572 794a 6f62 436f 6e66 6967 5d20 3d20  eryJobConfig] = 
+00010a30: 4e6f 6e65 2c0a 2020 2020 2920 2d3e 2062  None,.    ) -> b
+00010a40: 6967 7175 6572 792e 5175 6572 794a 6f62  igquery.QueryJob
+00010a50: 436f 6e66 6967 3a0a 2020 2020 2020 2020  Config:.        
+00010a60: 6966 206a 6f62 5f63 6f6e 6669 6720 6973  if job_config is
+00010a70: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00010a80: 2020 206a 6f62 5f63 6f6e 6669 6720 3d20     job_config = 
+00010a90: 6269 6771 7565 7279 2e51 7565 7279 4a6f  bigquery.QueryJo
+00010aa0: 6243 6f6e 6669 6728 290a 2020 2020 2020  bConfig().      
+00010ab0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00010ac0: 2020 2020 2320 4372 6561 7465 2061 2063      # Create a c
+00010ad0: 6f70 7920 736f 2074 6861 7420 7765 2064  opy so that we d
+00010ae0: 6f6e 2774 206d 7574 6174 6520 7468 6520  on't mutate the 
+00010af0: 6f72 6967 696e 616c 2063 6f6e 6669 6720  original config 
+00010b00: 7061 7373 6564 0a20 2020 2020 2020 2020  passed.         
+00010b10: 2020 206a 6f62 5f63 6f6e 6669 6720 3d20     job_config = 
+00010b20: 7479 7069 6e67 2e63 6173 7428 0a20 2020  typing.cast(.   
+00010b30: 2020 2020 2020 2020 2020 2020 2062 6967               big
+00010b40: 7175 6572 792e 5175 6572 794a 6f62 436f  query.QueryJobCo
+00010b50: 6e66 6967 2c0a 2020 2020 2020 2020 2020  nfig,.          
+00010b60: 2020 2020 2020 6269 6771 7565 7279 2e51        bigquery.Q
+00010b70: 7565 7279 4a6f 6243 6f6e 6669 672e 6672  ueryJobConfig.fr
+00010b80: 6f6d 5f61 7069 5f72 6570 7228 6a6f 625f  om_api_repr(job_
+00010b90: 636f 6e66 6967 2e74 6f5f 6170 695f 7265  config.to_api_re
+00010ba0: 7072 2829 292c 0a20 2020 2020 2020 2020  pr()),.         
+00010bb0: 2020 2029 0a0a 2020 2020 2020 2020 6966     )..        if
+00010bc0: 2062 6967 6672 616d 6573 2e6f 7074 696f   bigframes.optio
+00010bd0: 6e73 2e63 6f6d 7075 7465 2e6d 6178 696d  ns.compute.maxim
+00010be0: 756d 5f62 7974 6573 5f62 696c 6c65 6420  um_bytes_billed 
+00010bf0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00010c00: 2020 2020 2020 2020 206a 6f62 5f63 6f6e           job_con
+00010c10: 6669 672e 6d61 7869 6d75 6d5f 6279 7465  fig.maximum_byte
+00010c20: 735f 6269 6c6c 6564 203d 2028 0a20 2020  s_billed = (.   
+00010c30: 2020 2020 2020 2020 2020 2020 2062 6967               big
+00010c40: 6672 616d 6573 2e6f 7074 696f 6e73 2e63  frames.options.c
+00010c50: 6f6d 7075 7465 2e6d 6178 696d 756d 5f62  ompute.maximum_b
+00010c60: 7974 6573 5f62 696c 6c65 640a 2020 2020  ytes_billed.    
+00010c70: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+00010c80: 2020 2069 6620 7365 6c66 2e5f 6271 5f6b     if self._bq_k
+00010c90: 6d73 5f6b 6579 5f6e 616d 653a 0a20 2020  ms_key_name:.   
+00010ca0: 2020 2020 2020 2020 206a 6f62 5f63 6f6e           job_con
+00010cb0: 6669 672e 6465 7374 696e 6174 696f 6e5f  fig.destination_
+00010cc0: 656e 6372 7970 7469 6f6e 5f63 6f6e 6669  encryption_confi
+00010cd0: 6775 7261 7469 6f6e 203d 2028 0a20 2020  guration = (.   
+00010ce0: 2020 2020 2020 2020 2020 2020 2062 6967               big
+00010cf0: 7175 6572 792e 456e 6372 7970 7469 6f6e  query.Encryption
+00010d00: 436f 6e66 6967 7572 6174 696f 6e28 6b6d  Configuration(km
+00010d10: 735f 6b65 795f 6e61 6d65 3d73 656c 662e  s_key_name=self.
+00010d20: 5f62 715f 6b6d 735f 6b65 795f 6e61 6d65  _bq_kms_key_name
+00010d30: 290a 2020 2020 2020 2020 2020 2020 290a  ).            ).
+00010d40: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00010d50: 6a6f 625f 636f 6e66 6967 0a0a 2020 2020  job_config..    
+00010d60: 6465 6620 5f70 7265 7061 7265 5f6c 6f61  def _prepare_loa
+00010d70: 645f 6a6f 625f 636f 6e66 6967 2873 656c  d_job_config(sel
+00010d80: 6629 202d 3e20 6269 6771 7565 7279 2e4c  f) -> bigquery.L
+00010d90: 6f61 644a 6f62 436f 6e66 6967 3a0a 2020  oadJobConfig:.  
+00010da0: 2020 2020 2020 2320 4372 6561 7465 2061        # Create a
+00010db0: 2063 6f70 7920 736f 2074 6861 7420 7765   copy so that we
+00010dc0: 2064 6f6e 2774 206d 7574 6174 6520 7468   don't mutate th
+00010dd0: 6520 6f72 6967 696e 616c 2063 6f6e 6669  e original confi
+00010de0: 6720 7061 7373 6564 0a20 2020 2020 2020  g passed.       
+00010df0: 206a 6f62 5f63 6f6e 6669 6720 3d20 6269   job_config = bi
+00010e00: 6771 7565 7279 2e4c 6f61 644a 6f62 436f  gquery.LoadJobCo
+00010e10: 6e66 6967 2829 0a0a 2020 2020 2020 2020  nfig()..        
+00010e20: 6966 2073 656c 662e 5f62 715f 6b6d 735f  if self._bq_kms_
+00010e30: 6b65 795f 6e61 6d65 3a0a 2020 2020 2020  key_name:.      
+00010e40: 2020 2020 2020 6a6f 625f 636f 6e66 6967        job_config
+00010e50: 2e64 6573 7469 6e61 7469 6f6e 5f65 6e63  .destination_enc
+00010e60: 7279 7074 696f 6e5f 636f 6e66 6967 7572  ryption_configur
+00010e70: 6174 696f 6e20 3d20 280a 2020 2020 2020  ation = (.      
+00010e80: 2020 2020 2020 2020 2020 6269 6771 7565            bigque
+00010e90: 7279 2e45 6e63 7279 7074 696f 6e43 6f6e  ry.EncryptionCon
+00010ea0: 6669 6775 7261 7469 6f6e 286b 6d73 5f6b  figuration(kms_k
+00010eb0: 6579 5f6e 616d 653d 7365 6c66 2e5f 6271  ey_name=self._bq
+00010ec0: 5f6b 6d73 5f6b 6579 5f6e 616d 6529 0a20  _kms_key_name). 
+00010ed0: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
+00010ee0: 2020 2020 2020 7265 7475 726e 206a 6f62        return job
+00010ef0: 5f63 6f6e 6669 670a 0a20 2020 2064 6566  _config..    def
+00010f00: 205f 7072 6570 6172 655f 636f 7079 5f6a   _prepare_copy_j
+00010f10: 6f62 5f63 6f6e 6669 6728 7365 6c66 2920  ob_config(self) 
+00010f20: 2d3e 2062 6967 7175 6572 792e 436f 7079  -> bigquery.Copy
+00010f30: 4a6f 6243 6f6e 6669 673a 0a20 2020 2020  JobConfig:.     
+00010f40: 2020 2023 2043 7265 6174 6520 6120 636f     # Create a co
+00010f50: 7079 2073 6f20 7468 6174 2077 6520 646f  py so that we do
+00010f60: 6e27 7420 6d75 7461 7465 2074 6865 206f  n't mutate the o
+00010f70: 7269 6769 6e61 6c20 636f 6e66 6967 2070  riginal config p
+00010f80: 6173 7365 640a 2020 2020 2020 2020 6a6f  assed.        jo
+00010f90: 625f 636f 6e66 6967 203d 2062 6967 7175  b_config = bigqu
+00010fa0: 6572 792e 436f 7079 4a6f 6243 6f6e 6669  ery.CopyJobConfi
+00010fb0: 6728 290a 0a20 2020 2020 2020 2069 6620  g()..        if 
+00010fc0: 7365 6c66 2e5f 6271 5f6b 6d73 5f6b 6579  self._bq_kms_key
+00010fd0: 5f6e 616d 653a 0a20 2020 2020 2020 2020  _name:.         
+00010fe0: 2020 206a 6f62 5f63 6f6e 6669 672e 6465     job_config.de
+00010ff0: 7374 696e 6174 696f 6e5f 656e 6372 7970  stination_encryp
+00011000: 7469 6f6e 5f63 6f6e 6669 6775 7261 7469  tion_configurati
+00011010: 6f6e 203d 2028 0a20 2020 2020 2020 2020  on = (.         
+00011020: 2020 2020 2020 2062 6967 7175 6572 792e         bigquery.
+00011030: 456e 6372 7970 7469 6f6e 436f 6e66 6967  EncryptionConfig
+00011040: 7572 6174 696f 6e28 6b6d 735f 6b65 795f  uration(kms_key_
+00011050: 6e61 6d65 3d73 656c 662e 5f62 715f 6b6d  name=self._bq_km
+00011060: 735f 6b65 795f 6e61 6d65 290a 2020 2020  s_key_name).    
+00011070: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+00011080: 2020 2072 6574 7572 6e20 6a6f 625f 636f     return job_co
+00011090: 6e66 6967 0a0a 2020 2020 6465 6620 5f73  nfig..    def _s
+000110a0: 7461 7274 5f71 7565 7279 280a 2020 2020  tart_query(.    
+000110b0: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+000110c0: 2020 7371 6c3a 2073 7472 2c0a 2020 2020    sql: str,.    
+000110d0: 2020 2020 6a6f 625f 636f 6e66 6967 3a20      job_config: 
+000110e0: 4f70 7469 6f6e 616c 5b62 6967 7175 6572  Optional[bigquer
+000110f0: 792e 6a6f 622e 5175 6572 794a 6f62 436f  y.job.QueryJobCo
+00011100: 6e66 6967 5d20 3d20 4e6f 6e65 2c0a 2020  nfig] = None,.  
+00011110: 2020 2020 2020 6d61 785f 7265 7375 6c74        max_result
+00011120: 733a 204f 7074 696f 6e61 6c5b 696e 745d  s: Optional[int]
+00011130: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+00011140: 2074 696d 656f 7574 3a20 4f70 7469 6f6e   timeout: Option
+00011150: 616c 5b66 6c6f 6174 5d20 3d20 4e6f 6e65  al[float] = None
+00011160: 2c0a 2020 2020 2920 2d3e 2054 7570 6c65  ,.    ) -> Tuple
+00011170: 5b62 6967 7175 6572 792e 7461 626c 652e  [bigquery.table.
+00011180: 526f 7749 7465 7261 746f 722c 2062 6967  RowIterator, big
+00011190: 7175 6572 792e 5175 6572 794a 6f62 5d3a  query.QueryJob]:
+000111a0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+000111b0: 2020 2020 2053 7461 7274 7320 4269 6751       Starts BigQ
+000111c0: 7565 7279 2071 7565 7279 206a 6f62 2061  uery query job a
+000111d0: 6e64 2077 6169 7473 2066 6f72 2072 6573  nd waits for res
+000111e0: 756c 7473 2e0a 2020 2020 2020 2020 2222  ults..        ""
+000111f0: 220a 2020 2020 2020 2020 6a6f 625f 636f  ".        job_co
+00011200: 6e66 6967 203d 2073 656c 662e 5f70 7265  nfig = self._pre
+00011210: 7061 7265 5f71 7565 7279 5f6a 6f62 5f63  pare_query_job_c
+00011220: 6f6e 6669 6728 6a6f 625f 636f 6e66 6967  onfig(job_config
+00011230: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00011240: 2062 6967 6672 616d 6573 2e73 6573 7369   bigframes.sessi
+00011250: 6f6e 2e5f 696f 2e62 6967 7175 6572 792e  on._io.bigquery.
+00011260: 7374 6172 745f 7175 6572 795f 7769 7468  start_query_with
+00011270: 5f63 6c69 656e 7428 0a20 2020 2020 2020  _client(.       
+00011280: 2020 2020 2073 656c 662e 6271 636c 6965       self.bqclie
+00011290: 6e74 2c20 7371 6c2c 206a 6f62 5f63 6f6e  nt, sql, job_con
+000112a0: 6669 672c 206d 6178 5f72 6573 756c 7473  fig, max_results
+000112b0: 2c20 7469 6d65 6f75 740a 2020 2020 2020  , timeout.      
+000112c0: 2020 290a 0a20 2020 2064 6566 205f 7374    )..    def _st
+000112d0: 6172 745f 7175 6572 795f 6d6c 5f64 646c  art_query_ml_ddl
+000112e0: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+000112f0: 2020 2020 2020 2020 7371 6c3a 2073 7472          sql: str
+00011300: 2c0a 2020 2020 2920 2d3e 2054 7570 6c65  ,.    ) -> Tuple
+00011310: 5b62 6967 7175 6572 792e 7461 626c 652e  [bigquery.table.
+00011320: 526f 7749 7465 7261 746f 722c 2062 6967  RowIterator, big
+00011330: 7175 6572 792e 5175 6572 794a 6f62 5d3a  query.QueryJob]:
+00011340: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00011350: 2020 2020 2053 7461 7274 7320 4269 6751       Starts BigQ
+00011360: 7565 7279 204d 4c20 4444 4c20 7175 6572  uery ML DDL quer
+00011370: 7920 6a6f 6220 2843 5245 4154 4520 4d4f  y job (CREATE MO
+00011380: 4445 4c2f 414c 5445 5220 4d4f 4445 4c2f  DEL/ALTER MODEL/
+00011390: 2e2e 2e29 2061 6e64 0a20 2020 2020 2020  ...) and.       
+000113a0: 2077 6169 7473 2066 6f72 2072 6573 756c   waits for resul
+000113b0: 7473 2e0a 2020 2020 2020 2020 2222 220a  ts..        """.
+000113c0: 2020 2020 2020 2020 6a6f 625f 636f 6e66          job_conf
+000113d0: 6967 203d 2073 656c 662e 5f70 7265 7061  ig = self._prepa
+000113e0: 7265 5f71 7565 7279 5f6a 6f62 5f63 6f6e  re_query_job_con
+000113f0: 6669 6728 290a 0a20 2020 2020 2020 2023  fig()..        #
+00011400: 2042 514d 4c20 6578 7065 6374 7320 6b6d   BQML expects km
+00011410: 735f 6b65 795f 6e61 6d65 2074 6872 6f75  s_key_name throu
+00011420: 6768 204f 5054 494f 4e53 2061 6e64 206e  gh OPTIONS and n
+00011430: 6f74 2074 6872 6f75 6768 206a 6f62 2063  ot through job c
+00011440: 6f6e 6669 672c 0a20 2020 2020 2020 2023  onfig,.        #
+00011450: 2073 6f20 7765 206d 7573 7420 7265 7365   so we must rese
+00011460: 7420 616e 7920 656e 6372 7970 7469 6f6e  t any encryption
+00011470: 2073 6574 2069 6e20 7468 6520 6a6f 6220   set in the job 
+00011480: 636f 6e66 6967 0a20 2020 2020 2020 2023  config.        #
+00011490: 2068 7474 7073 3a2f 2f63 6c6f 7564 2e67   https://cloud.g
+000114a0: 6f6f 676c 652e 636f 6d2f 6269 6771 7565  oogle.com/bigque
+000114b0: 7279 2f64 6f63 732f 6375 7374 6f6d 6572  ry/docs/customer
+000114c0: 2d6d 616e 6167 6564 2d65 6e63 7279 7074  -managed-encrypt
+000114d0: 696f 6e23 656e 6372 7970 742d 6d6f 6465  ion#encrypt-mode
+000114e0: 6c0a 2020 2020 2020 2020 6a6f 625f 636f  l.        job_co
+000114f0: 6e66 6967 2e64 6573 7469 6e61 7469 6f6e  nfig.destination
+00011500: 5f65 6e63 7279 7074 696f 6e5f 636f 6e66  _encryption_conf
+00011510: 6967 7572 6174 696f 6e20 3d20 4e6f 6e65  iguration = None
+00011520: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00011530: 2062 6967 6672 616d 6573 2e73 6573 7369   bigframes.sessi
+00011540: 6f6e 2e5f 696f 2e62 6967 7175 6572 792e  on._io.bigquery.
+00011550: 7374 6172 745f 7175 6572 795f 7769 7468  start_query_with
+00011560: 5f63 6c69 656e 7428 0a20 2020 2020 2020  _client(.       
+00011570: 2020 2020 2073 656c 662e 6271 636c 6965       self.bqclie
+00011580: 6e74 2c20 7371 6c2c 206a 6f62 5f63 6f6e  nt, sql, job_con
+00011590: 6669 670a 2020 2020 2020 2020 290a 0a20  fig.        ).. 
+000115a0: 2020 2064 6566 205f 6361 6368 655f 7769     def _cache_wi
+000115b0: 7468 5f63 6c75 7374 6572 5f63 6f6c 7328  th_cluster_cols(
+000115c0: 0a20 2020 2020 2020 2073 656c 662c 2061  .        self, a
+000115d0: 7272 6179 5f76 616c 7565 3a20 636f 7265  rray_value: core
+000115e0: 2e41 7272 6179 5661 6c75 652c 2063 6c75  .ArrayValue, clu
+000115f0: 7374 6572 5f63 6f6c 733a 2074 7970 696e  ster_cols: typin
+00011600: 672e 5365 7175 656e 6365 5b73 7472 5d0a  g.Sequence[str].
+00011610: 2020 2020 2920 2d3e 2063 6f72 652e 4172      ) -> core.Ar
+00011620: 7261 7956 616c 7565 3a0a 2020 2020 2020  rayValue:.      
+00011630: 2020 2222 2245 7865 6375 7465 7320 7468    """Executes th
+00011640: 6520 7175 6572 7920 616e 6420 7573 6573  e query and uses
+00011650: 2074 6865 2072 6573 756c 7469 6e67 2074   the resulting t
+00011660: 6162 6c65 2074 6f20 7265 7772 6974 6520  able to rewrite 
+00011670: 6675 7475 7265 2065 7865 6375 7469 6f6e  future execution
+00011680: 732e 2222 220a 2020 2020 2020 2020 2320  s.""".        # 
+00011690: 544f 444f 3a20 5573 6520 7468 6973 2066  TODO: Use this f
+000116a0: 6f72 2061 6c6c 2065 7865 6375 7469 6f6e  or all execution
+000116b0: 733f 2050 726f 626c 656d 2069 7320 7468  s? Problem is th
+000116c0: 6174 2063 6163 6869 6e67 206d 6174 6572  at caching mater
+000116d0: 6961 6c69 7a65 7320 6578 7472 610a 2020  ializes extra.  
+000116e0: 2020 2020 2020 2320 6f72 6465 7269 6e67        # ordering
+000116f0: 2063 6f6c 756d 6e73 0a20 2020 2020 2020   columns.       
+00011700: 2063 6f6d 7069 6c65 645f 7661 6c75 6520   compiled_value 
+00011710: 3d20 7365 6c66 2e5f 636f 6d70 696c 655f  = self._compile_
+00011720: 6f72 6465 7265 6428 6172 7261 795f 7661  ordered(array_va
+00011730: 6c75 6529 0a0a 2020 2020 2020 2020 6962  lue)..        ib
+00011740: 6973 5f65 7870 7220 3d20 636f 6d70 696c  is_expr = compil
+00011750: 6564 5f76 616c 7565 2e5f 746f 5f69 6269  ed_value._to_ibi
+00011760: 735f 6578 7072 280a 2020 2020 2020 2020  s_expr(.        
+00011770: 2020 2020 6f72 6465 7269 6e67 5f6d 6f64      ordering_mod
+00011780: 653d 2275 6e6f 7264 6572 6564 222c 2065  e="unordered", e
+00011790: 7870 6f73 655f 6869 6464 656e 5f63 6f6c  xpose_hidden_col
+000117a0: 733d 5472 7565 0a20 2020 2020 2020 2029  s=True.        )
+000117b0: 0a20 2020 2020 2020 2074 6d70 5f74 6162  .        tmp_tab
+000117c0: 6c65 203d 2073 656c 662e 5f69 6269 735f  le = self._ibis_
+000117d0: 746f 5f74 656d 705f 7461 626c 6528 0a20  to_temp_table(. 
+000117e0: 2020 2020 2020 2020 2020 2069 6269 735f             ibis_
+000117f0: 6578 7072 2c20 636c 7573 7465 725f 636f  expr, cluster_co
+00011800: 6c73 3d63 6c75 7374 6572 5f63 6f6c 732c  ls=cluster_cols,
+00011810: 2061 7069 5f6e 616d 653d 2263 6163 6865   api_name="cache
+00011820: 6422 0a20 2020 2020 2020 2029 0a20 2020  d".        ).   
+00011830: 2020 2020 2074 6162 6c65 5f65 7870 7265       table_expre
+00011840: 7373 696f 6e20 3d20 7365 6c66 2e69 6269  ssion = self.ibi
+00011850: 735f 636c 6965 6e74 2e74 6162 6c65 280a  s_client.table(.
+00011860: 2020 2020 2020 2020 2020 2020 746d 705f              tmp_
+00011870: 7461 626c 652e 7461 626c 655f 6964 2c0a  table.table_id,.
+00011880: 2020 2020 2020 2020 2020 2020 7363 6865              sche
+00011890: 6d61 3d74 6d70 5f74 6162 6c65 2e64 6174  ma=tmp_table.dat
+000118a0: 6173 6574 5f69 642c 0a20 2020 2020 2020  aset_id,.       
+000118b0: 2020 2020 2064 6174 6162 6173 653d 746d       database=tm
+000118c0: 705f 7461 626c 652e 7072 6f6a 6563 742c  p_table.project,
+000118d0: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+000118e0: 2020 206e 6577 5f63 6f6c 756d 6e73 203d     new_columns =
+000118f0: 205b 7461 626c 655f 6578 7072 6573 7369   [table_expressi
+00011900: 6f6e 5b63 6f6c 756d 6e5d 2066 6f72 2063  on[column] for c
+00011910: 6f6c 756d 6e20 696e 2063 6f6d 7069 6c65  olumn in compile
+00011920: 645f 7661 6c75 652e 636f 6c75 6d6e 5f69  d_value.column_i
+00011930: 6473 5d0a 2020 2020 2020 2020 6e65 775f  ds].        new_
+00011940: 6869 6464 656e 5f63 6f6c 756d 6e73 203d  hidden_columns =
+00011950: 205b 0a20 2020 2020 2020 2020 2020 2074   [.            t
+00011960: 6162 6c65 5f65 7870 7265 7373 696f 6e5b  able_expression[
+00011970: 636f 6c75 6d6e 5d0a 2020 2020 2020 2020  column].        
+00011980: 2020 2020 666f 7220 636f 6c75 6d6e 2069      for column i
+00011990: 6e20 636f 6d70 696c 6564 5f76 616c 7565  n compiled_value
+000119a0: 2e5f 6869 6464 656e 5f6f 7264 6572 696e  ._hidden_orderin
+000119b0: 675f 636f 6c75 6d6e 5f6e 616d 6573 0a20  g_column_names. 
+000119c0: 2020 2020 2020 205d 0a20 2020 2020 2020         ].       
+000119d0: 2023 2054 4f44 4f3a 2049 6e73 7465 6164   # TODO: Instead
+000119e0: 2c20 6b65 6570 2073 6573 7369 6f6e 2d77  , keep session-w
+000119f0: 6964 6520 6d61 7020 6f66 2063 6163 6865  ide map of cache
+00011a00: 6420 7265 7375 6c74 7320 616e 6420 6175  d results and au
+00011a10: 746f 6d61 7469 6361 6c6c 7920 7265 7573  tomatically reus
+00011a20: 650a 2020 2020 2020 2020 7265 7475 726e  e.        return
+00011a30: 2063 6f72 652e 4172 7261 7956 616c 7565   core.ArrayValue
+00011a40: 2e66 726f 6d5f 6962 6973 280a 2020 2020  .from_ibis(.    
+00011a50: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+00011a60: 2020 2020 2020 2020 2020 7461 626c 655f            table_
+00011a70: 6578 7072 6573 7369 6f6e 2c0a 2020 2020  expression,.    
+00011a80: 2020 2020 2020 2020 636f 6c75 6d6e 733d          columns=
+00011a90: 6e65 775f 636f 6c75 6d6e 732c 0a20 2020  new_columns,.   
+00011aa0: 2020 2020 2020 2020 2068 6964 6465 6e5f           hidden_
+00011ab0: 6f72 6465 7269 6e67 5f63 6f6c 756d 6e73  ordering_columns
+00011ac0: 3d6e 6577 5f68 6964 6465 6e5f 636f 6c75  =new_hidden_colu
+00011ad0: 6d6e 732c 0a20 2020 2020 2020 2020 2020  mns,.           
+00011ae0: 206f 7264 6572 696e 673d 636f 6d70 696c   ordering=compil
+00011af0: 6564 5f76 616c 7565 2e5f 6f72 6465 7269  ed_value._orderi
+00011b00: 6e67 2c0a 2020 2020 2020 2020 290a 0a20  ng,.        ).. 
+00011b10: 2020 2064 6566 205f 6361 6368 655f 7769     def _cache_wi
+00011b20: 7468 5f6f 6666 7365 7473 2873 656c 662c  th_offsets(self,
+00011b30: 2061 7272 6179 5f76 616c 7565 3a20 636f   array_value: co
+00011b40: 7265 2e41 7272 6179 5661 6c75 6529 202d  re.ArrayValue) -
+00011b50: 3e20 636f 7265 2e41 7272 6179 5661 6c75  > core.ArrayValu
+00011b60: 653a 0a20 2020 2020 2020 2022 2222 4578  e:.        """Ex
+00011b70: 6563 7574 6573 2074 6865 2071 7565 7279  ecutes the query
+00011b80: 2061 6e64 2075 7365 7320 7468 6520 7265   and uses the re
+00011b90: 7375 6c74 696e 6720 7461 626c 6520 746f  sulting table to
+00011ba0: 2072 6577 7269 7465 2066 7574 7572 6520   rewrite future 
+00011bb0: 6578 6563 7574 696f 6e73 2e22 2222 0a20  executions.""". 
+00011bc0: 2020 2020 2020 2023 2054 4f44 4f3a 2055         # TODO: U
+00011bd0: 7365 2074 6869 7320 666f 7220 616c 6c20  se this for all 
+00011be0: 6578 6563 7574 696f 6e73 3f20 5072 6f62  executions? Prob
+00011bf0: 6c65 6d20 6973 2074 6861 7420 6361 6368  lem is that cach
+00011c00: 696e 6720 6d61 7465 7269 616c 697a 6573  ing materializes
+00011c10: 2065 7874 7261 0a20 2020 2020 2020 2023   extra.        #
+00011c20: 206f 7264 6572 696e 6720 636f 6c75 6d6e   ordering column
+00011c30: 730a 2020 2020 2020 2020 636f 6d70 696c  s.        compil
+00011c40: 6564 5f76 616c 7565 203d 2073 656c 662e  ed_value = self.
+00011c50: 5f63 6f6d 7069 6c65 5f6f 7264 6572 6564  _compile_ordered
+00011c60: 2861 7272 6179 5f76 616c 7565 290a 0a20  (array_value).. 
+00011c70: 2020 2020 2020 2069 6269 735f 6578 7072         ibis_expr
+00011c80: 203d 2063 6f6d 7069 6c65 645f 7661 6c75   = compiled_valu
+00011c90: 652e 5f74 6f5f 6962 6973 5f65 7870 7228  e._to_ibis_expr(
+00011ca0: 0a20 2020 2020 2020 2020 2020 206f 7264  .            ord
+00011cb0: 6572 696e 675f 6d6f 6465 3d22 6f66 6673  ering_mode="offs
+00011cc0: 6574 5f63 6f6c 222c 206f 7264 6572 5f63  et_col", order_c
+00011cd0: 6f6c 5f6e 616d 653d 2262 6967 6672 616d  ol_name="bigfram
+00011ce0: 6573 5f6f 6666 7365 7473 220a 2020 2020  es_offsets".    
+00011cf0: 2020 2020 290a 2020 2020 2020 2020 746d      ).        tm
+00011d00: 705f 7461 626c 6520 3d20 7365 6c66 2e5f  p_table = self._
+00011d10: 6962 6973 5f74 6f5f 7465 6d70 5f74 6162  ibis_to_temp_tab
+00011d20: 6c65 280a 2020 2020 2020 2020 2020 2020  le(.            
+00011d30: 6962 6973 5f65 7870 722c 2063 6c75 7374  ibis_expr, clust
+00011d40: 6572 5f63 6f6c 733d 5b22 6269 6766 7261  er_cols=["bigfra
+00011d50: 6d65 735f 6f66 6673 6574 7322 5d2c 2061  mes_offsets"], a
+00011d60: 7069 5f6e 616d 653d 2263 6163 6865 6422  pi_name="cached"
+00011d70: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+00011d80: 2020 2074 6162 6c65 5f65 7870 7265 7373     table_express
+00011d90: 696f 6e20 3d20 7365 6c66 2e69 6269 735f  ion = self.ibis_
+00011da0: 636c 6965 6e74 2e74 6162 6c65 280a 2020  client.table(.  
+00011db0: 2020 2020 2020 2020 2020 746d 705f 7461            tmp_ta
+00011dc0: 626c 652e 7461 626c 655f 6964 2c0a 2020  ble.table_id,.  
+00011dd0: 2020 2020 2020 2020 2020 7363 6865 6d61            schema
+00011de0: 3d74 6d70 5f74 6162 6c65 2e64 6174 6173  =tmp_table.datas
+00011df0: 6574 5f69 642c 0a20 2020 2020 2020 2020  et_id,.         
+00011e00: 2020 2064 6174 6162 6173 653d 746d 705f     database=tmp_
+00011e10: 7461 626c 652e 7072 6f6a 6563 742c 0a20  table.project,. 
+00011e20: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00011e30: 206e 6577 5f63 6f6c 756d 6e73 203d 205b   new_columns = [
+00011e40: 7461 626c 655f 6578 7072 6573 7369 6f6e  table_expression
+00011e50: 5b63 6f6c 756d 6e5d 2066 6f72 2063 6f6c  [column] for col
+00011e60: 756d 6e20 696e 2063 6f6d 7069 6c65 645f  umn in compiled_
+00011e70: 7661 6c75 652e 636f 6c75 6d6e 5f69 6473  value.column_ids
+00011e80: 5d0a 2020 2020 2020 2020 6e65 775f 6869  ].        new_hi
+00011e90: 6464 656e 5f63 6f6c 756d 6e73 203d 205b  dden_columns = [
+00011ea0: 7461 626c 655f 6578 7072 6573 7369 6f6e  table_expression
+00011eb0: 5b22 6269 6766 7261 6d65 735f 6f66 6673  ["bigframes_offs
+00011ec0: 6574 7322 5d5d 0a20 2020 2020 2020 2023  ets"]].        #
+00011ed0: 2054 4f44 4f3a 2049 6e73 7465 6164 2c20   TODO: Instead, 
+00011ee0: 6b65 6570 2073 6573 7369 6f6e 2d77 6964  keep session-wid
+00011ef0: 6520 6d61 7020 6f66 2063 6163 6865 6420  e map of cached 
+00011f00: 7265 7375 6c74 7320 616e 6420 6175 746f  results and auto
+00011f10: 6d61 7469 6361 6c6c 7920 7265 7573 650a  matically reuse.
+00011f20: 2020 2020 2020 2020 7265 7475 726e 2063          return c
+00011f30: 6f72 652e 4172 7261 7956 616c 7565 2e66  ore.ArrayValue.f
+00011f40: 726f 6d5f 6962 6973 280a 2020 2020 2020  rom_ibis(.      
+00011f50: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+00011f60: 2020 2020 2020 2020 7461 626c 655f 6578          table_ex
+00011f70: 7072 6573 7369 6f6e 2c0a 2020 2020 2020  pression,.      
+00011f80: 2020 2020 2020 636f 6c75 6d6e 733d 6e65        columns=ne
+00011f90: 775f 636f 6c75 6d6e 732c 0a20 2020 2020  w_columns,.     
+00011fa0: 2020 2020 2020 2068 6964 6465 6e5f 6f72         hidden_or
+00011fb0: 6465 7269 6e67 5f63 6f6c 756d 6e73 3d6e  dering_columns=n
+00011fc0: 6577 5f68 6964 6465 6e5f 636f 6c75 6d6e  ew_hidden_column
+00011fd0: 732c 0a20 2020 2020 2020 2020 2020 206f  s,.            o
+00011fe0: 7264 6572 696e 673d 6f72 6465 722e 4578  rdering=order.Ex
+00011ff0: 7072 6573 7369 6f6e 4f72 6465 7269 6e67  pressionOrdering
+00012000: 2e66 726f 6d5f 6f66 6673 6574 5f63 6f6c  .from_offset_col
+00012010: 2822 6269 6766 7261 6d65 735f 6f66 6673  ("bigframes_offs
+00012020: 6574 7322 292c 0a20 2020 2020 2020 2029  ets"),.        )
+00012030: 0a0a 2020 2020 6465 6620 5f73 696d 706c  ..    def _simpl
+00012040: 6966 795f 7769 7468 5f63 6163 6869 6e67  ify_with_caching
+00012050: 2873 656c 662c 2061 7272 6179 5f76 616c  (self, array_val
+00012060: 7565 3a20 636f 7265 2e41 7272 6179 5661  ue: core.ArrayVa
+00012070: 6c75 6529 202d 3e20 636f 7265 2e41 7272  lue) -> core.Arr
+00012080: 6179 5661 6c75 653a 0a20 2020 2020 2020  ayValue:.       
+00012090: 2022 2222 4174 7465 6d70 7473 2074 6f20   """Attempts to 
+000120a0: 6861 6e64 6c65 2074 6865 2063 6f6d 706c  handle the compl
+000120b0: 6578 6974 7920 6279 2063 6163 6869 6e67  exity by caching
+000120c0: 2064 7570 6c69 6361 7465 6420 7375 6274   duplicated subt
+000120d0: 7265 6573 2061 6e64 2062 7265 616b 696e  rees and breakin
+000120e0: 6720 7468 6520 7175 6572 7920 696e 746f  g the query into
+000120f0: 2070 6965 6365 732e 2222 220a 2020 2020   pieces.""".    
+00012100: 2020 2020 6966 206e 6f74 2062 6967 6672      if not bigfr
+00012110: 616d 6573 2e6f 7074 696f 6e73 2e63 6f6d  ames.options.com
+00012120: 7075 7465 2e65 6e61 626c 655f 6d75 6c74  pute.enable_mult
+00012130: 695f 7175 6572 795f 6578 6563 7574 696f  i_query_executio
+00012140: 6e3a 0a20 2020 2020 2020 2020 2020 2072  n:.            r
+00012150: 6574 7572 6e20 6172 7261 795f 7661 6c75  eturn array_valu
+00012160: 650a 2020 2020 2020 2020 6e6f 6465 203d  e.        node =
+00012170: 2061 7272 6179 5f76 616c 7565 2e6e 6f64   array_value.nod
+00012180: 650a 2020 2020 2020 2020 6966 206e 6f64  e.        if nod
+00012190: 652e 706c 616e 6e69 6e67 5f63 6f6d 706c  e.planning_compl
+000121a0: 6578 6974 7920 3c20 5155 4552 595f 434f  exity < QUERY_CO
+000121b0: 4d50 4c45 5849 5459 5f4c 494d 4954 3a0a  MPLEXITY_LIMIT:.
+000121c0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+000121d0: 726e 2061 7272 6179 5f76 616c 7565 0a0a  rn array_value..
+000121e0: 2020 2020 2020 2020 666f 7220 5f20 696e          for _ in
+000121f0: 2072 616e 6765 284d 4158 5f53 5542 5452   range(MAX_SUBTR
+00012200: 4545 5f46 4143 544f 5249 4e47 5329 3a0a  EE_FACTORINGS):.
+00012210: 2020 2020 2020 2020 2020 2020 7570 6461              upda
+00012220: 7465 6420 3d20 7365 6c66 2e5f 6361 6368  ted = self._cach
+00012230: 655f 6d6f 7374 5f63 6f6d 706c 6578 5f73  e_most_complex_s
+00012240: 7562 7472 6565 286e 6f64 6529 0a20 2020  ubtree(node).   
+00012250: 2020 2020 2020 2020 2069 6620 7570 6461           if upda
+00012260: 7465 6420 6973 204e 6f6e 653a 0a20 2020  ted is None:.   
+00012270: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00012280: 7572 6e20 636f 7265 2e41 7272 6179 5661  urn core.ArrayVa
+00012290: 6c75 6528 6e6f 6465 290a 2020 2020 2020  lue(node).      
+000122a0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+000122b0: 2020 2020 2020 2020 2020 2020 6e6f 6465              node
+000122c0: 203d 2075 7064 6174 6564 0a0a 2020 2020   = updated..    
+000122d0: 2020 2020 7265 7475 726e 2063 6f72 652e      return core.
+000122e0: 4172 7261 7956 616c 7565 286e 6f64 6529  ArrayValue(node)
+000122f0: 0a0a 2020 2020 6465 6620 5f63 6163 6865  ..    def _cache
+00012300: 5f6d 6f73 745f 636f 6d70 6c65 785f 7375  _most_complex_su
+00012310: 6274 7265 6528 0a20 2020 2020 2020 2073  btree(.        s
+00012320: 656c 662c 206e 6f64 653a 206e 6f64 6573  elf, node: nodes
+00012330: 2e42 6967 4672 616d 654e 6f64 650a 2020  .BigFrameNode.  
+00012340: 2020 2920 2d3e 204f 7074 696f 6e61 6c5b    ) -> Optional[
+00012350: 6e6f 6465 732e 4269 6746 7261 6d65 4e6f  nodes.BigFrameNo
+00012360: 6465 5d3a 0a20 2020 2020 2020 2023 2054  de]:.        # T
+00012370: 4f44 4f3a 2049 6620 7175 6572 7920 6661  ODO: If query fa
+00012380: 696c 732c 2072 6574 7279 2077 6974 6820  ils, retry with 
+00012390: 6c6f 7765 7220 636f 6d70 6c65 7869 7479  lower complexity
+000123a0: 206c 696d 6974 0a20 2020 2020 2020 2076   limit.        v
+000123b0: 616c 6964 5f63 616e 6469 6461 7465 7320  alid_candidates 
+000123c0: 3d20 7472 6176 6572 7361 6c73 2e63 6f75  = traversals.cou
+000123d0: 6e74 5f63 6f6d 706c 6578 5f6e 6f64 6573  nt_complex_nodes
+000123e0: 280a 2020 2020 2020 2020 2020 2020 6e6f  (.            no
+000123f0: 6465 2c0a 2020 2020 2020 2020 2020 2020  de,.            
+00012400: 6d69 6e5f 636f 6d70 6c65 7869 7479 3d28  min_complexity=(
+00012410: 5155 4552 595f 434f 4d50 4c45 5849 5459  QUERY_COMPLEXITY
+00012420: 5f4c 494d 4954 202f 2035 3030 292c 0a20  _LIMIT / 500),. 
+00012430: 2020 2020 2020 2020 2020 206d 6178 5f63             max_c
+00012440: 6f6d 706c 6578 6974 793d 5155 4552 595f  omplexity=QUERY_
+00012450: 434f 4d50 4c45 5849 5459 5f4c 494d 4954  COMPLEXITY_LIMIT
+00012460: 2c0a 2020 2020 2020 2020 292e 6974 656d  ,.        ).item
+00012470: 7328 290a 2020 2020 2020 2020 2320 4865  s().        # He
+00012480: 7572 6973 7469 633a 2073 7562 7472 6565  uristic: subtree
+00012490: 5f63 6f6d 706c 6569 7874 7920 2a20 2863  _compleixty * (c
+000124a0: 6f70 6965 7320 6f66 2073 7562 7472 6565  opies of subtree
+000124b0: 295e 320a 2020 2020 2020 2020 6265 7374  )^2.        best
+000124c0: 5f63 616e 6469 6461 7465 203d 206d 6178  _candidate = max
+000124d0: 280a 2020 2020 2020 2020 2020 2020 7661  (.            va
+000124e0: 6c69 645f 6361 6e64 6964 6174 6573 2c0a  lid_candidates,.
+000124f0: 2020 2020 2020 2020 2020 2020 6b65 793d              key=
+00012500: 6c61 6d62 6461 2069 3a20 695b 305d 2e70  lambda i: i[0].p
+00012510: 6c61 6e6e 696e 675f 636f 6d70 6c65 7869  lanning_complexi
+00012520: 7479 202b 2028 695b 315d 202a 2a20 3229  ty + (i[1] ** 2)
+00012530: 2c0a 2020 2020 2020 2020 2020 2020 6465  ,.            de
+00012540: 6661 756c 743d 4e6f 6e65 2c0a 2020 2020  fault=None,.    
+00012550: 2020 2020 290a 0a20 2020 2020 2020 2069      )..        i
+00012560: 6620 6265 7374 5f63 616e 6469 6461 7465  f best_candidate
+00012570: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+00012580: 2020 2020 2020 2320 4e6f 2067 6f6f 6420        # No good 
+00012590: 7375 6274 7265 6573 2074 6f20 6361 6368  subtrees to cach
+000125a0: 652c 206a 7573 7420 7265 7475 726e 206f  e, just return o
+000125b0: 7269 6769 6e61 6c20 7472 6565 0a20 2020  riginal tree.   
+000125c0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+000125d0: 4e6f 6e65 0a0a 2020 2020 2020 2020 2320  None..        # 
+000125e0: 544f 444f 3a20 4164 6420 636c 7573 7465  TODO: Add cluste
+000125f0: 7269 6e67 2063 6f6c 756d 6e73 2062 6173  ring columns bas
+00012600: 6564 206f 6e20 6163 6365 7373 2070 6174  ed on access pat
+00012610: 7465 726e 730a 2020 2020 2020 2020 6d61  terns.        ma
+00012620: 7465 7269 616c 697a 6564 203d 2073 656c  terialized = sel
+00012630: 662e 5f63 6163 6865 5f77 6974 685f 636c  f._cache_with_cl
+00012640: 7573 7465 725f 636f 6c73 280a 2020 2020  uster_cols(.    
+00012650: 2020 2020 2020 2020 636f 7265 2e41 7272          core.Arr
+00012660: 6179 5661 6c75 6528 6265 7374 5f63 616e  ayValue(best_can
+00012670: 6469 6461 7465 5b30 5d29 2c20 5b5d 0a20  didate[0]), []. 
+00012680: 2020 2020 2020 2029 2e6e 6f64 650a 0a20         ).node.. 
+00012690: 2020 2020 2020 2072 6574 7572 6e20 7472         return tr
+000126a0: 6176 6572 7361 6c73 2e72 6570 6c61 6365  aversals.replace
+000126b0: 5f6e 6f64 6573 280a 2020 2020 2020 2020  _nodes(.        
+000126c0: 2020 2020 6e6f 6465 2c20 746f 5f72 6570      node, to_rep
+000126d0: 6c61 6365 3d62 6573 745f 6361 6e64 6964  lace=best_candid
+000126e0: 6174 655b 305d 2c20 7265 706c 6163 656d  ate[0], replacem
+000126f0: 656e 6574 3d6d 6174 6572 6961 6c69 7a65  enet=materialize
+00012700: 640a 2020 2020 2020 2020 290a 0a20 2020  d.        )..   
+00012710: 2064 6566 205f 6973 5f74 7269 7669 616c   def _is_trivial
+00012720: 6c79 5f65 7865 6375 7461 626c 6528 7365  ly_executable(se
+00012730: 6c66 2c20 6172 7261 795f 7661 6c75 653a  lf, array_value:
+00012740: 2063 6f72 652e 4172 7261 7956 616c 7565   core.ArrayValue
+00012750: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
+00012760: 2020 2020 2020 2043 616e 2074 6865 2062         Can the b
+00012770: 6c6f 636b 2062 6520 6576 616c 7561 7465  lock be evaluate
+00012780: 6420 7665 7279 2063 6865 6170 6c79 3f0a  d very cheaply?.
+00012790: 2020 2020 2020 2020 4966 2054 7275 652c          If True,
+000127a0: 2074 6865 2061 7272 6179 5f76 616c 7565   the array_value
+000127b0: 2070 726f 6261 626c 7920 6973 206e 6f74   probably is not
+000127c0: 2077 6f72 7468 2063 6163 6869 6e67 2e0a   worth caching..
+000127d0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+000127e0: 2020 2020 2320 4f6e 6365 2072 6577 7269      # Once rewri
+000127f0: 7469 6e67 2069 7320 6176 6169 6c61 626c  ting is availabl
+00012800: 652c 2077 696c 6c20 7761 6e74 2074 6f20  e, will want to 
+00012810: 7265 7772 6974 6520 6265 666f 7265 0a20  rewrite before. 
+00012820: 2020 2020 2020 2023 2065 7661 6c75 6174         # evaluat
+00012830: 696e 6720 6578 6563 7574 696f 6e20 636f  ing execution co
+00012840: 7374 2e0a 2020 2020 2020 2020 7265 7475  st..        retu
+00012850: 726e 2074 7261 7665 7273 616c 732e 6973  rn traversals.is
+00012860: 5f74 7269 7669 616c 6c79 5f65 7865 6375  _trivially_execu
+00012870: 7461 626c 6528 6172 7261 795f 7661 6c75  table(array_valu
+00012880: 652e 6e6f 6465 290a 0a20 2020 2064 6566  e.node)..    def
+00012890: 205f 6578 6563 7574 6528 0a20 2020 2020   _execute(.     
+000128a0: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+000128b0: 2061 7272 6179 5f76 616c 7565 3a20 636f   array_value: co
+000128c0: 7265 2e41 7272 6179 5661 6c75 652c 0a20  re.ArrayValue,. 
+000128d0: 2020 2020 2020 206a 6f62 5f63 6f6e 6669         job_confi
+000128e0: 673a 204f 7074 696f 6e61 6c5b 6269 6771  g: Optional[bigq
+000128f0: 7565 7279 2e6a 6f62 2e51 7565 7279 4a6f  uery.job.QueryJo
+00012900: 6243 6f6e 6669 675d 203d 204e 6f6e 652c  bConfig] = None,
+00012910: 0a20 2020 2020 2020 202a 2c0a 2020 2020  .        *,.    
+00012920: 2020 2020 736f 7274 6564 3a20 626f 6f6c      sorted: bool
+00012930: 203d 2054 7275 652c 0a20 2020 2020 2020   = True,.       
+00012940: 2064 7279 5f72 756e 3d46 616c 7365 2c0a   dry_run=False,.
+00012950: 2020 2020 2020 2020 636f 6c5f 6964 5f6f          col_id_o
+00012960: 7665 7272 6964 6573 3a20 4d61 7070 696e  verrides: Mappin
+00012970: 675b 7374 722c 2073 7472 5d20 3d20 7b7d  g[str, str] = {}
+00012980: 2c0a 2020 2020 2920 2d3e 2074 7570 6c65  ,.    ) -> tuple
+00012990: 5b62 6967 7175 6572 792e 7461 626c 652e  [bigquery.table.
+000129a0: 526f 7749 7465 7261 746f 722c 2062 6967  RowIterator, big
+000129b0: 7175 6572 792e 5175 6572 794a 6f62 5d3a  query.QueryJob]:
+000129c0: 0a20 2020 2020 2020 2073 716c 203d 2073  .        sql = s
+000129d0: 656c 662e 5f74 6f5f 7371 6c28 0a20 2020  elf._to_sql(.   
+000129e0: 2020 2020 2020 2020 2061 7272 6179 5f76           array_v
+000129f0: 616c 7565 2c20 736f 7274 6564 3d73 6f72  alue, sorted=sor
+00012a00: 7465 642c 2063 6f6c 5f69 645f 6f76 6572  ted, col_id_over
+00012a10: 7269 6465 733d 636f 6c5f 6964 5f6f 7665  rides=col_id_ove
+00012a20: 7272 6964 6573 0a20 2020 2020 2020 2029  rrides.        )
+00012a30: 2020 2320 7479 7065 3a69 676e 6f72 650a    # type:ignore.
+00012a40: 2020 2020 2020 2020 6966 206a 6f62 5f63          if job_c
+00012a50: 6f6e 6669 6720 6973 204e 6f6e 653a 0a20  onfig is None:. 
+00012a60: 2020 2020 2020 2020 2020 206a 6f62 5f63             job_c
+00012a70: 6f6e 6669 6720 3d20 6269 6771 7565 7279  onfig = bigquery
+00012a80: 2e51 7565 7279 4a6f 6243 6f6e 6669 6728  .QueryJobConfig(
+00012a90: 6472 795f 7275 6e3d 6472 795f 7275 6e29  dry_run=dry_run)
+00012aa0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+00012ab0: 2020 2020 2020 2020 2020 206a 6f62 5f63             job_c
+00012ac0: 6f6e 6669 672e 6472 795f 7275 6e20 3d20  onfig.dry_run = 
+00012ad0: 6472 795f 7275 6e0a 2020 2020 2020 2020  dry_run.        
+00012ae0: 7265 7475 726e 2073 656c 662e 5f73 7461  return self._sta
+00012af0: 7274 5f71 7565 7279 280a 2020 2020 2020  rt_query(.      
+00012b00: 2020 2020 2020 7371 6c3d 7371 6c2c 0a20        sql=sql,. 
+00012b10: 2020 2020 2020 2020 2020 206a 6f62 5f63             job_c
+00012b20: 6f6e 6669 673d 6a6f 625f 636f 6e66 6967  onfig=job_config
+00012b30: 2c0a 2020 2020 2020 2020 290a 0a20 2020  ,.        )..   
+00012b40: 2064 6566 205f 7065 656b 280a 2020 2020   def _peek(.    
+00012b50: 2020 2020 7365 6c66 2c20 6172 7261 795f      self, array_
+00012b60: 7661 6c75 653a 2063 6f72 652e 4172 7261  value: core.Arra
+00012b70: 7956 616c 7565 2c20 6e5f 726f 7773 3a20  yValue, n_rows: 
+00012b80: 696e 740a 2020 2020 2920 2d3e 2074 7570  int.    ) -> tup
+00012b90: 6c65 5b62 6967 7175 6572 792e 7461 626c  le[bigquery.tabl
+00012ba0: 652e 526f 7749 7465 7261 746f 722c 2062  e.RowIterator, b
+00012bb0: 6967 7175 6572 792e 5175 6572 794a 6f62  igquery.QueryJob
+00012bc0: 5d3a 0a20 2020 2020 2020 2022 2222 4120  ]:.        """A 
+00012bd0: 2770 6565 6b27 2065 6666 6963 6965 6e74  'peek' efficient
+00012be0: 6c79 2061 6363 6573 7365 7320 6120 736d  ly accesses a sm
+00012bf0: 616c 6c20 6e75 6d62 6572 206f 6620 726f  all number of ro
+00012c00: 7773 2069 6e20 7468 6520 6461 7461 6672  ws in the datafr
+00012c10: 616d 652e 2222 220a 2020 2020 2020 2020  ame.""".        
+00012c20: 6966 206e 6f74 2074 7265 655f 7072 6f70  if not tree_prop
+00012c30: 6572 7469 6573 2e70 6565 6b61 626c 6528  erties.peekable(
+00012c40: 6172 7261 795f 7661 6c75 652e 6e6f 6465  array_value.node
+00012c50: 293a 0a20 2020 2020 2020 2020 2020 2077  ):.            w
+00012c60: 6172 6e69 6e67 732e 7761 726e 2822 5065  arnings.warn("Pe
+00012c70: 656b 696e 6720 7468 6973 2076 616c 7565  eking this value
+00012c80: 2063 616e 6e6f 7420 6265 2064 6f6e 6520   cannot be done 
+00012c90: 6566 6669 6369 656e 746c 792e 2229 0a20  efficiently."). 
+00012ca0: 2020 2020 2020 2073 716c 203d 2073 656c         sql = sel
+00012cb0: 662e 5f63 6f6d 7069 6c65 5f75 6e6f 7264  f._compile_unord
+00012cc0: 6572 6564 2861 7272 6179 5f76 616c 7565  ered(array_value
+00012cd0: 292e 7065 656b 5f73 716c 286e 5f72 6f77  ).peek_sql(n_row
+00012ce0: 7329 0a20 2020 2020 2020 2072 6574 7572  s).        retur
+00012cf0: 6e20 7365 6c66 2e5f 7374 6172 745f 7175  n self._start_qu
+00012d00: 6572 7928 0a20 2020 2020 2020 2020 2020  ery(.           
+00012d10: 2073 716c 3d73 716c 2c0a 2020 2020 2020   sql=sql,.      
+00012d20: 2020 290a 0a20 2020 2064 6566 205f 746f    )..    def _to
+00012d30: 5f73 716c 280a 2020 2020 2020 2020 7365  _sql(.        se
+00012d40: 6c66 2c0a 2020 2020 2020 2020 6172 7261  lf,.        arra
+00012d50: 795f 7661 6c75 653a 2063 6f72 652e 4172  y_value: core.Ar
+00012d60: 7261 7956 616c 7565 2c0a 2020 2020 2020  rayValue,.      
+00012d70: 2020 6f66 6673 6574 5f63 6f6c 756d 6e3a    offset_column:
+00012d80: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
+00012d90: 5b73 7472 5d20 3d20 4e6f 6e65 2c0a 2020  [str] = None,.  
+00012da0: 2020 2020 2020 636f 6c5f 6964 5f6f 7665        col_id_ove
+00012db0: 7272 6964 6573 3a20 7479 7069 6e67 2e4d  rrides: typing.M
+00012dc0: 6170 7069 6e67 5b73 7472 2c20 7374 725d  apping[str, str]
+00012dd0: 203d 207b 7d2c 0a20 2020 2020 2020 2073   = {},.        s
+00012de0: 6f72 7465 643a 2062 6f6f 6c20 3d20 4661  orted: bool = Fa
+00012df0: 6c73 652c 0a20 2020 2029 202d 3e20 7374  lse,.    ) -> st
+00012e00: 723a 0a20 2020 2020 2020 2069 6620 6f66  r:.        if of
+00012e10: 6673 6574 5f63 6f6c 756d 6e3a 0a20 2020  fset_column:.   
+00012e20: 2020 2020 2020 2020 2061 7272 6179 5f76           array_v
+00012e30: 616c 7565 203d 2061 7272 6179 5f76 616c  alue = array_val
+00012e40: 7565 2e70 726f 6d6f 7465 5f6f 6666 7365  ue.promote_offse
+00012e50: 7473 286f 6666 7365 745f 636f 6c75 6d6e  ts(offset_column
+00012e60: 290a 2020 2020 2020 2020 6966 2073 6f72  ).        if sor
+00012e70: 7465 643a 0a20 2020 2020 2020 2020 2020  ted:.           
+00012e80: 2072 6574 7572 6e20 7365 6c66 2e5f 636f   return self._co
+00012e90: 6d70 696c 655f 6f72 6465 7265 6428 6172  mpile_ordered(ar
+00012ea0: 7261 795f 7661 6c75 6529 2e74 6f5f 7371  ray_value).to_sq
+00012eb0: 6c28 0a20 2020 2020 2020 2020 2020 2020  l(.             
+00012ec0: 2020 2063 6f6c 5f69 645f 6f76 6572 7269     col_id_overri
+00012ed0: 6465 733d 636f 6c5f 6964 5f6f 7665 7272  des=col_id_overr
+00012ee0: 6964 6573 2c20 736f 7274 6564 3d54 7275  ides, sorted=Tru
+00012ef0: 650a 2020 2020 2020 2020 2020 2020 290a  e.            ).
+00012f00: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00012f10: 656c 662e 5f63 6f6d 7069 6c65 5f75 6e6f  elf._compile_uno
+00012f20: 7264 6572 6564 2861 7272 6179 5f76 616c  rdered(array_val
+00012f30: 7565 292e 746f 5f73 716c 280a 2020 2020  ue).to_sql(.    
+00012f40: 2020 2020 2020 2020 636f 6c5f 6964 5f6f          col_id_o
+00012f50: 7665 7272 6964 6573 3d63 6f6c 5f69 645f  verrides=col_id_
+00012f60: 6f76 6572 7269 6465 730a 2020 2020 2020  overrides.      
+00012f70: 2020 290a 0a20 2020 2064 6566 205f 636f    )..    def _co
+00012f80: 6d70 696c 655f 6f72 6465 7265 6428 0a20  mpile_ordered(. 
+00012f90: 2020 2020 2020 2073 656c 662c 2061 7272         self, arr
+00012fa0: 6179 5f76 616c 7565 3a20 636f 7265 2e41  ay_value: core.A
+00012fb0: 7272 6179 5661 6c75 650a 2020 2020 2920  rrayValue.    ) 
+00012fc0: 2d3e 2062 6967 6672 616d 6573 2e63 6f72  -> bigframes.cor
+00012fd0: 652e 636f 6d70 696c 652e 4f72 6465 7265  e.compile.Ordere
+00012fe0: 6449 523a 0a20 2020 2020 2020 2072 6574  dIR:.        ret
+00012ff0: 7572 6e20 6269 6766 7261 6d65 732e 636f  urn bigframes.co
+00013000: 7265 2e63 6f6d 7069 6c65 2e63 6f6d 7069  re.compile.compi
+00013010: 6c65 5f6f 7264 6572 6564 5f69 7228 6172  le_ordered_ir(ar
+00013020: 7261 795f 7661 6c75 652e 6e6f 6465 290a  ray_value.node).
+00013030: 0a20 2020 2064 6566 205f 636f 6d70 696c  .    def _compil
+00013040: 655f 756e 6f72 6465 7265 6428 0a20 2020  e_unordered(.   
+00013050: 2020 2020 2073 656c 662c 2061 7272 6179       self, array
+00013060: 5f76 616c 7565 3a20 636f 7265 2e41 7272  _value: core.Arr
+00013070: 6179 5661 6c75 650a 2020 2020 2920 2d3e  ayValue.    ) ->
+00013080: 2062 6967 6672 616d 6573 2e63 6f72 652e   bigframes.core.
+00013090: 636f 6d70 696c 652e 556e 6f72 6465 7265  compile.Unordere
+000130a0: 6449 523a 0a20 2020 2020 2020 2072 6574  dIR:.        ret
+000130b0: 7572 6e20 6269 6766 7261 6d65 732e 636f  urn bigframes.co
+000130c0: 7265 2e63 6f6d 7069 6c65 2e63 6f6d 7069  re.compile.compi
+000130d0: 6c65 5f75 6e6f 7264 6572 6564 5f69 7228  le_unordered_ir(
+000130e0: 6172 7261 795f 7661 6c75 652e 6e6f 6465  array_value.node
+000130f0: 290a 0a20 2020 2064 6566 205f 6765 745f  )..    def _get_
+00013100: 7461 626c 655f 7369 7a65 2873 656c 662c  table_size(self,
+00013110: 2064 6573 7469 6e61 7469 6f6e 5f74 6162   destination_tab
+00013120: 6c65 293a 0a20 2020 2020 2020 2074 6162  le):.        tab
+00013130: 6c65 203d 2073 656c 662e 6271 636c 6965  le = self.bqclie
+00013140: 6e74 2e67 6574 5f74 6162 6c65 2864 6573  nt.get_table(des
+00013150: 7469 6e61 7469 6f6e 5f74 6162 6c65 290a  tination_table).
+00013160: 2020 2020 2020 2020 7265 7475 726e 2074          return t
+00013170: 6162 6c65 2e6e 756d 5f62 7974 6573 0a0a  able.num_bytes..
+00013180: 2020 2020 6465 6620 5f72 6f77 735f 746f      def _rows_to
+00013190: 5f64 6174 6166 7261 6d65 280a 2020 2020  _dataframe(.    
+000131a0: 2020 2020 7365 6c66 2c20 726f 775f 6974      self, row_it
+000131b0: 6572 6174 6f72 3a20 6269 6771 7565 7279  erator: bigquery
+000131c0: 2e74 6162 6c65 2e52 6f77 4974 6572 6174  .table.RowIterat
+000131d0: 6f72 2c20 6474 7970 6573 3a20 4469 6374  or, dtypes: Dict
+000131e0: 0a20 2020 2029 202d 3e20 7061 6e64 6173  .    ) -> pandas
+000131f0: 2e44 6174 6146 7261 6d65 3a0a 2020 2020  .DataFrame:.    
+00013200: 2020 2020 2320 4361 6e20 6967 6e6f 7265      # Can ignore
+00013210: 2069 6e66 6572 7265 6420 6461 7461 7479   inferred dataty
+00013220: 7065 2075 6e74 696c 2064 7479 7065 2065  pe until dtype e
+00013230: 6d75 6c61 7469 6f6e 2062 7265 616b 7320  mulation breaks 
+00013240: 313a 3120 6d61 7070 696e 6720 6265 7477  1:1 mapping betw
+00013250: 6565 6e20 4251 2074 7970 6573 2061 6e64  een BQ types and
+00013260: 2062 6967 6672 616d 6573 2074 7970 6573   bigframes types
+00013270: 0a20 2020 2020 2020 2064 7479 7065 735f  .        dtypes_
+00013280: 6672 6f6d 5f62 7120 3d20 6269 6766 7261  from_bq = bigfra
+00013290: 6d65 732e 6474 7970 6573 2e62 665f 7479  mes.dtypes.bf_ty
+000132a0: 7065 5f66 726f 6d5f 7479 7065 5f6b 696e  pe_from_type_kin
+000132b0: 6428 726f 775f 6974 6572 6174 6f72 2e73  d(row_iterator.s
+000132c0: 6368 656d 6129 0a20 2020 2020 2020 2061  chema).        a
+000132d0: 7272 6f77 5f74 6162 6c65 203d 2072 6f77  rrow_table = row
+000132e0: 5f69 7465 7261 746f 722e 746f 5f61 7272  _iterator.to_arr
+000132f0: 6f77 2829 0a20 2020 2020 2020 2072 6574  ow().        ret
+00013300: 7572 6e20 6269 6766 7261 6d65 732e 7365  urn bigframes.se
+00013310: 7373 696f 6e2e 5f69 6f2e 7061 6e64 6173  ssion._io.pandas
+00013320: 2e61 7272 6f77 5f74 6f5f 7061 6e64 6173  .arrow_to_pandas
+00013330: 2861 7272 6f77 5f74 6162 6c65 2c20 6474  (arrow_table, dt
+00013340: 7970 6573 5f66 726f 6d5f 6271 290a 0a20  ypes_from_bq).. 
+00013350: 2020 2064 6566 205f 7374 6172 745f 6765     def _start_ge
+00013360: 6e65 7269 635f 6a6f 6228 7365 6c66 2c20  neric_job(self, 
+00013370: 6a6f 623a 2066 6f72 6d61 7474 696e 675f  job: formatting_
+00013380: 6865 6c70 6572 732e 4765 6e65 7269 634a  helpers.GenericJ
+00013390: 6f62 293a 0a20 2020 2020 2020 2069 6620  ob):.        if 
+000133a0: 6269 6766 7261 6d65 732e 6f70 7469 6f6e  bigframes.option
+000133b0: 732e 6469 7370 6c61 792e 7072 6f67 7265  s.display.progre
+000133c0: 7373 5f62 6172 2069 7320 6e6f 7420 4e6f  ss_bar is not No
+000133d0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000133e0: 666f 726d 6174 7469 6e67 5f68 656c 7065  formatting_helpe
+000133f0: 7273 2e77 6169 745f 666f 725f 6a6f 6228  rs.wait_for_job(
+00013400: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013410: 206a 6f62 2c20 6269 6766 7261 6d65 732e   job, bigframes.
+00013420: 6f70 7469 6f6e 732e 6469 7370 6c61 792e  options.display.
+00013430: 7072 6f67 7265 7373 5f62 6172 0a20 2020  progress_bar.   
+00013440: 2020 2020 2020 2020 2029 2020 2320 5761           )  # Wa
+00013450: 6974 2066 6f72 2074 6865 206a 6f62 2074  it for the job t
+00013460: 6f20 636f 6d70 6c65 7465 0a20 2020 2020  o complete.     
+00013470: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00013480: 2020 2020 206a 6f62 2e72 6573 756c 7428       job.result(
+00013490: 290a 0a0a 6465 6620 636f 6e6e 6563 7428  )...def connect(
+000134a0: 636f 6e74 6578 743a 204f 7074 696f 6e61  context: Optiona
+000134b0: 6c5b 6269 6771 7565 7279 5f6f 7074 696f  l[bigquery_optio
+000134c0: 6e73 2e42 6967 5175 6572 794f 7074 696f  ns.BigQueryOptio
+000134d0: 6e73 5d20 3d20 4e6f 6e65 2920 2d3e 2053  ns] = None) -> S
+000134e0: 6573 7369 6f6e 3a0a 2020 2020 7265 7475  ession:.    retu
+000134f0: 726e 2053 6573 7369 6f6e 2863 6f6e 7465  rn Session(conte
+00013500: 7874 290a 0a0a 6465 6620 5f63 616e 5f63  xt)...def _can_c
+00013510: 6c75 7374 6572 5f62 7128 6669 656c 643a  luster_bq(field:
+00013520: 2062 6967 7175 6572 792e 5363 6865 6d61   bigquery.Schema
+00013530: 4669 656c 6429 3a0a 2020 2020 2320 6874  Field):.    # ht
+00013540: 7470 733a 2f2f 636c 6f75 642e 676f 6f67  tps://cloud.goog
+00013550: 6c65 2e63 6f6d 2f62 6967 7175 6572 792f  le.com/bigquery/
+00013560: 646f 6373 2f63 6c75 7374 6572 6564 2d74  docs/clustered-t
+00013570: 6162 6c65 730a 2020 2020 2320 4e6f 7461  ables.    # Nota
+00013580: 626c 792c 2066 6c6f 6174 2069 7320 6578  bly, float is ex
+00013590: 636c 7564 6564 0a20 2020 2074 7970 655f  cluded.    type_
+000135a0: 203d 2066 6965 6c64 2e66 6965 6c64 5f74   = field.field_t
+000135b0: 7970 650a 2020 2020 7265 7475 726e 2074  ype.    return t
+000135c0: 7970 655f 2069 6e20 280a 2020 2020 2020  ype_ in (.      
+000135d0: 2020 2249 4e54 4547 4552 222c 0a20 2020    "INTEGER",.   
+000135e0: 2020 2020 2022 494e 5436 3422 2c0a 2020       "INT64",.  
+000135f0: 2020 2020 2020 2253 5452 494e 4722 2c0a        "STRING",.
+00013600: 2020 2020 2020 2020 224e 554d 4552 4943          "NUMERIC
+00013610: 222c 0a20 2020 2020 2020 2022 4445 4349  ",.        "DECI
+00013620: 4d41 4c22 2c0a 2020 2020 2020 2020 2242  MAL",.        "B
+00013630: 4947 4e55 4d45 5249 4322 2c0a 2020 2020  IGNUMERIC",.    
+00013640: 2020 2020 2242 4947 4445 4349 4d41 4c22      "BIGDECIMAL"
+00013650: 2c0a 2020 2020 2020 2020 2244 4154 4522  ,.        "DATE"
+00013660: 2c0a 2020 2020 2020 2020 2244 4154 4554  ,.        "DATET
+00013670: 494d 4522 2c0a 2020 2020 2020 2020 2254  IME",.        "T
+00013680: 494d 4553 5441 4d50 222c 0a20 2020 2020  IMESTAMP",.     
+00013690: 2020 2022 424f 4f4c 222c 0a20 2020 2020     "BOOL",.     
+000136a0: 2020 2022 424f 4f4c 4541 4e22 2c0a 2020     "BOOLEAN",.  
+000136b0: 2020 290a 0a0a 6465 6620 5f63 6f6e 7665    )...def _conve
+000136c0: 7274 5f74 6f5f 6e6f 6e6e 756c 6c5f 7374  rt_to_nonnull_st
+000136d0: 7269 6e67 2863 6f6c 756d 6e3a 2069 6269  ring(column: ibi
+000136e0: 735f 7479 7065 732e 436f 6c75 6d6e 2920  s_types.Column) 
+000136f0: 2d3e 2069 6269 735f 7479 7065 732e 5374  -> ibis_types.St
+00013700: 7269 6e67 5661 6c75 653a 0a20 2020 2063  ringValue:.    c
+00013710: 6f6c 5f74 7970 6520 3d20 636f 6c75 6d6e  ol_type = column
+00013720: 2e74 7970 6528 290a 2020 2020 6966 2028  .type().    if (
+00013730: 0a20 2020 2020 2020 2063 6f6c 5f74 7970  .        col_typ
+00013740: 652e 6973 5f6e 756d 6572 6963 2829 0a20  e.is_numeric(). 
+00013750: 2020 2020 2020 206f 7220 636f 6c5f 7479         or col_ty
+00013760: 7065 2e69 735f 626f 6f6c 6561 6e28 290a  pe.is_boolean().
+00013770: 2020 2020 2020 2020 6f72 2063 6f6c 5f74          or col_t
+00013780: 7970 652e 6973 5f62 696e 6172 7928 290a  ype.is_binary().
+00013790: 2020 2020 2020 2020 6f72 2063 6f6c 5f74          or col_t
+000137a0: 7970 652e 6973 5f74 656d 706f 7261 6c28  ype.is_temporal(
+000137b0: 290a 2020 2020 293a 0a20 2020 2020 2020  ).    ):.       
+000137c0: 2072 6573 756c 7420 3d20 636f 6c75 6d6e   result = column
+000137d0: 2e63 6173 7428 6962 6973 5f64 7479 7065  .cast(ibis_dtype
+000137e0: 732e 5374 7269 6e67 286e 756c 6c61 626c  s.String(nullabl
+000137f0: 653d 5472 7565 2929 0a20 2020 2065 6c69  e=True)).    eli
+00013800: 6620 636f 6c5f 7479 7065 2e69 735f 6765  f col_type.is_ge
+00013810: 6f73 7061 7469 616c 2829 3a0a 2020 2020  ospatial():.    
+00013820: 2020 2020 7265 7375 6c74 203d 2074 7970      result = typ
+00013830: 696e 672e 6361 7374 2869 6269 735f 7479  ing.cast(ibis_ty
+00013840: 7065 732e 4765 6f53 7061 7469 616c 436f  pes.GeoSpatialCo
+00013850: 6c75 6d6e 2c20 636f 6c75 6d6e 292e 6173  lumn, column).as
+00013860: 5f74 6578 7428 290a 2020 2020 656c 6966  _text().    elif
+00013870: 2063 6f6c 5f74 7970 652e 6973 5f73 7472   col_type.is_str
+00013880: 696e 6728 293a 0a20 2020 2020 2020 2072  ing():.        r
+00013890: 6573 756c 7420 3d20 636f 6c75 6d6e 0a20  esult = column. 
+000138a0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+000138b0: 2023 2054 4f5f 4a53 4f4e 5f53 5452 494e   # TO_JSON_STRIN
+000138c0: 4720 776f 726b 7320 7769 7468 2061 6c6c  G works with all
+000138d0: 2064 6174 6120 7479 7065 732c 2062 7574   data types, but
+000138e0: 2069 736e 2774 2074 6865 206d 6f73 7420   isn't the most 
+000138f0: 6566 6669 6369 656e 740a 2020 2020 2020  efficient.      
+00013900: 2020 2320 4e65 6564 6564 2066 6f72 204a    # Needed for J
+00013910: 534f 4e2c 2053 5452 5543 5420 616e 6420  SON, STRUCT and 
+00013920: 4152 5241 5920 6461 7461 7479 7065 730a  ARRAY datatypes.
+00013930: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
+00013940: 2076 656e 646f 7265 645f 6962 6973 5f6f   vendored_ibis_o
+00013950: 7073 2e54 6f4a 736f 6e53 7472 696e 6728  ps.ToJsonString(
+00013960: 636f 6c75 6d6e 292e 746f 5f65 7870 7228  column).to_expr(
+00013970: 2920 2023 2074 7970 653a 2069 676e 6f72  )  # type: ignor
+00013980: 650a 2020 2020 2320 4573 6361 7065 2062  e.    # Escape b
+00013990: 6163 6b73 6c61 7368 6573 2061 6e64 2075  ackslashes and u
+000139a0: 7365 2062 6163 6b73 6c61 7368 2061 7320  se backslash as 
+000139b0: 6465 6c69 6e65 6174 6f72 0a20 2020 2065  delineator.    e
+000139c0: 7363 6170 6564 203d 2074 7970 696e 672e  scaped = typing.
+000139d0: 6361 7374 2869 6269 735f 7479 7065 732e  cast(ibis_types.
+000139e0: 5374 7269 6e67 436f 6c75 6d6e 2c20 7265  StringColumn, re
+000139f0: 7375 6c74 2e66 696c 6c6e 6128 2222 2929  sult.fillna(""))
+00013a00: 2e72 6570 6c61 6365 2822 5c5c 222c 2022  .replace("\\", "
+00013a10: 5c5c 5c5c 2229 2020 2320 7479 7065 3a20  \\\\")  # type: 
+00013a20: 6967 6e6f 7265 0a20 2020 2072 6574 7572  ignore.    retur
+00013a30: 6e20 7479 7069 6e67 2e63 6173 7428 6962  n typing.cast(ib
+00013a40: 6973 5f74 7970 6573 2e53 7472 696e 6743  is_types.StringC
+00013a50: 6f6c 756d 6e2c 2069 6269 732e 6c69 7465  olumn, ibis.lite
+00013a60: 7261 6c28 225c 5c22 2929 2e63 6f6e 6361  ral("\\")).conca
+00013a70: 7428 6573 6361 7065 6429 0a0a 0a64 6566  t(escaped)...def
+00013a80: 205f 7472 616e 7366 6f72 6d5f 7265 6164   _transform_read
+00013a90: 5f67 6271 5f63 6f6e 6669 6775 7261 7469  _gbq_configurati
+00013aa0: 6f6e 2863 6f6e 6669 6775 7261 7469 6f6e  on(configuration
+00013ab0: 3a20 4f70 7469 6f6e 616c 5b64 6963 745d  : Optional[dict]
+00013ac0: 2920 2d3e 2064 6963 743a 0a20 2020 2022  ) -> dict:.    "
+00013ad0: 2222 0a20 2020 2046 6f72 2062 6163 6b77  "".    For backw
+00013ae0: 6172 6473 2d63 6f6d 7061 7469 6269 6c69  ards-compatibili
+00013af0: 7479 2c20 636f 6e76 6572 7420 616e 7920  ty, convert any 
+00013b00: 7072 6576 696f 7573 6c79 2063 6c69 656e  previously clien
+00013b10: 742d 7369 6465 206f 6e6c 790a 2020 2020  t-side only.    
+00013b20: 7061 7261 6d65 7465 7273 2073 7563 6820  parameters such 
+00013b30: 6173 2074 696d 656f 7574 4d73 2074 6f20  as timeoutMs to 
+00013b40: 7468 6520 7072 6f70 6572 7479 206e 616d  the property nam
+00013b50: 6520 6578 7065 6374 6564 2062 7920 7468  e expected by th
+00013b60: 6520 5245 5354 2041 5049 2e0a 0a20 2020  e REST API...   
+00013b70: 204d 616b 6573 2061 2063 6f70 7920 6f66   Makes a copy of
+00013b80: 2063 6f6e 6669 6775 7261 7469 6f6e 2069   configuration i
+00013b90: 6620 6368 616e 6765 7320 6172 6520 6e65  f changes are ne
+00013ba0: 6564 6564 2e0a 2020 2020 2222 220a 0a20  eded..    """.. 
+00013bb0: 2020 2069 6620 636f 6e66 6967 7572 6174     if configurat
+00013bc0: 696f 6e20 6973 204e 6f6e 653a 0a20 2020  ion is None:.   
+00013bd0: 2020 2020 2072 6574 7572 6e20 7b7d 0a0a       return {}..
+00013be0: 2020 2020 7469 6d65 6f75 745f 6d73 203d      timeout_ms =
+00013bf0: 2063 6f6e 6669 6775 7261 7469 6f6e 2e67   configuration.g
+00013c00: 6574 2822 7175 6572 7922 2c20 7b7d 292e  et("query", {}).
+00013c10: 6765 7428 2274 696d 656f 7574 4d73 2229  get("timeoutMs")
+00013c20: 0a20 2020 2069 6620 7469 6d65 6f75 745f  .    if timeout_
+00013c30: 6d73 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ms is not None:.
+00013c40: 2020 2020 2020 2020 2320 5472 616e 7366          # Transf
+00013c50: 6f72 6d20 7469 6d65 6f75 744d 7320 746f  orm timeoutMs to
+00013c60: 2061 6e20 6163 7475 616c 2073 6572 7665   an actual serve
+00013c70: 722d 7369 6465 2063 6f6e 6669 6775 7261  r-side configura
+00013c80: 7469 6f6e 2e0a 2020 2020 2020 2020 2320  tion..        # 
+00013c90: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00013ca0: 6f6d 2f67 6f6f 676c 6561 7069 732f 7079  om/googleapis/py
+00013cb0: 7468 6f6e 2d62 6967 7175 6572 792d 7061  thon-bigquery-pa
+00013cc0: 6e64 6173 2f69 7373 7565 732f 3437 390a  ndas/issues/479.
+00013cd0: 2020 2020 2020 2020 636f 6e66 6967 7572          configur
+00013ce0: 6174 696f 6e20 3d20 636f 7079 2e64 6565  ation = copy.dee
+00013cf0: 7063 6f70 7928 636f 6e66 6967 7572 6174  pcopy(configurat
+00013d00: 696f 6e29 0a20 2020 2020 2020 2064 656c  ion).        del
+00013d10: 2063 6f6e 6669 6775 7261 7469 6f6e 5b22   configuration["
+00013d20: 7175 6572 7922 5d5b 2274 696d 656f 7574  query"]["timeout
+00013d30: 4d73 225d 0a20 2020 2020 2020 2063 6f6e  Ms"].        con
+00013d40: 6669 6775 7261 7469 6f6e 5b22 6a6f 6254  figuration["jobT
+00013d50: 696d 656f 7574 4d73 225d 203d 2074 696d  imeoutMs"] = tim
+00013d60: 656f 7574 5f6d 730a 0a20 2020 2072 6574  eout_ms..    ret
+00013d70: 7572 6e20 636f 6e66 6967 7572 6174 696f  urn configuratio
+00013d80: 6e0a                                     n.
```

### Comparing `bigframes-1.1.0/bigframes/session/_io/__init__.py` & `bigframes-1.2.0/bigframes/session/_io/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/bigframes/session/_io/bigquery.py` & `bigframes-1.2.0/bigframes/session/_io/bigquery.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/bigframes/session/_io/pandas.py` & `bigframes-1.2.0/bigframes/session/_io/pandas.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/bigframes/session/clients.py` & `bigframes-1.2.0/bigframes/session/clients.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/bigframes/version.py` & `bigframes-1.2.0/tests/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
-__version__ = "1.1.0"
```

### Comparing `bigframes-1.1.0/bigframes.egg-info/PKG-INFO` & `bigframes-1.2.0/bigframes.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigframes
-Version: 1.1.0
+Version: 1.2.0
 Summary: BigQuery DataFrames -- scalable analytics and machine learning with BigQuery
 Home-page: https://github.com/googleapis/python-bigquery-dataframes
 Author: Google LLC
 Author-email: bigframes-feedback@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `bigframes-1.1.0/bigframes.egg-info/SOURCES.txt` & `bigframes-1.2.0/bigframes.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -52,17 +52,17 @@
 bigframes/core/compile/compiler.py
 bigframes/core/compile/concat.py
 bigframes/core/compile/scalar_op_compiler.py
 bigframes/core/compile/single_column.py
 bigframes/core/groupby/__init__.py
 bigframes/core/indexes/__init__.py
 bigframes/core/indexes/base.py
+bigframes/core/indexes/multi.py
 bigframes/core/joins/__init__.py
 bigframes/core/joins/merge.py
-bigframes/core/joins/name_resolution.py
 bigframes/core/reshape/__init__.py
 bigframes/core/tools/__init__.py
 bigframes/core/tools/datetimes.py
 bigframes/core/window/__init__.py
 bigframes/functions/__init__.py
 bigframes/functions/remote_function.py
 bigframes/ml/__init__.py
@@ -101,15 +101,14 @@
 bigframes/pandas/__init__.py
 bigframes/session/__init__.py
 bigframes/session/clients.py
 bigframes/session/_io/__init__.py
 bigframes/session/_io/bigquery.py
 bigframes/session/_io/pandas.py
 tests/__init__.py
-tests/config.py
 tests/data/hockey_players.json
 tests/data/hockey_players.jsonl
 tests/data/matrix_2by3.json
 tests/data/matrix_2by3.jsonl
 tests/data/matrix_3by4.json
 tests/data/matrix_3by4.jsonl
 tests/data/nested.jsonl
@@ -254,14 +253,15 @@
 third_party/bigframes_vendored/pandas/core/computation/parsing.py
 third_party/bigframes_vendored/pandas/core/computation/scope.py
 third_party/bigframes_vendored/pandas/core/dtypes/inference.py
 third_party/bigframes_vendored/pandas/core/groupby/__init__.py
 third_party/bigframes_vendored/pandas/core/indexes/__init__.py
 third_party/bigframes_vendored/pandas/core/indexes/accessor.py
 third_party/bigframes_vendored/pandas/core/indexes/base.py
+third_party/bigframes_vendored/pandas/core/indexes/multi.py
 third_party/bigframes_vendored/pandas/core/reshape/__init__.py
 third_party/bigframes_vendored/pandas/core/reshape/concat.py
 third_party/bigframes_vendored/pandas/core/reshape/encoding.py
 third_party/bigframes_vendored/pandas/core/reshape/merge.py
 third_party/bigframes_vendored/pandas/core/reshape/tile.py
 third_party/bigframes_vendored/pandas/core/strings/accessor.py
 third_party/bigframes_vendored/pandas/core/tools/__init__.py
```

### Comparing `bigframes-1.1.0/bigframes.egg-info/requires.txt` & `bigframes-1.2.0/bigframes.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/setup.py` & `bigframes-1.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/__init__.py` & `bigframes-1.2.0/tests/system/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/data/hockey_players.json` & `bigframes-1.2.0/tests/data/hockey_players.json`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/data/hockey_players.jsonl` & `bigframes-1.2.0/tests/data/hockey_players.jsonl`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/data/nested.jsonl` & `bigframes-1.2.0/tests/data/nested.jsonl`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/data/nested_schema.json` & `bigframes-1.2.0/tests/data/nested_schema.json`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/data/penguins.jsonl` & `bigframes-1.2.0/tests/data/penguins.jsonl`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/data/penguins_schema.json` & `bigframes-1.2.0/tests/data/penguins_schema.json`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/data/scalars.jsonl` & `bigframes-1.2.0/tests/data/scalars.jsonl`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/data/scalars_schema.json` & `bigframes-1.2.0/tests/data/scalars_schema.json`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/data/time_series.jsonl` & `bigframes-1.2.0/tests/data/time_series.jsonl`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/system/__init__.py` & `bigframes-1.2.0/tests/system/large/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/system/conftest.py` & `bigframes-1.2.0/tests/system/conftest.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/system/large/__init__.py` & `bigframes-1.2.0/tests/system/small/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/system/large/ml/test_cluster.py` & `bigframes-1.2.0/tests/system/large/ml/test_cluster.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/system/large/ml/test_compose.py` & `bigframes-1.2.0/tests/system/large/ml/test_compose.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/system/large/ml/test_core.py` & `bigframes-1.2.0/tests/system/large/ml/test_core.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/system/large/ml/test_decomposition.py` & `bigframes-1.2.0/tests/system/large/ml/test_decomposition.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/system/large/ml/test_ensemble.py` & `bigframes-1.2.0/tests/system/large/ml/test_ensemble.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/system/large/ml/test_forecasting.py` & `bigframes-1.2.0/tests/system/large/ml/test_forecasting.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/system/large/ml/test_linear_model.py` & `bigframes-1.2.0/tests/system/large/ml/test_linear_model.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/system/large/ml/test_pipeline.py` & `bigframes-1.2.0/tests/system/large/ml/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/system/large/test_location.py` & `bigframes-1.2.0/tests/system/large/test_location.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 
 import typing
 
 from google.cloud import bigquery
 import pytest
 
 import bigframes
+import bigframes.constants
 import bigframes.session.clients
-from tests import config
 
 
 def _assert_bq_execution_location(session: bigframes.Session):
     df = session.read_gbq(
         """
         SELECT "aaa" as name, 111 as number
         UNION ALL
@@ -62,15 +62,19 @@
         session.bqclient._connection.API_BASE_URL == "https://bigquery.googleapis.com"
     )
 
     # assert that bigframes session honors the location
     _assert_bq_execution_location(session)
 
 
-@pytest.mark.parametrize("bigquery_location", config.ALL_BIGQUERY_LOCATIONS)
+@pytest.mark.parametrize(
+    "bigquery_location",
+    # Sort the set to avoid nondeterminism.
+    sorted(bigframes.constants.ALL_BIGQUERY_LOCATIONS),
+)
 def test_bq_location(bigquery_location):
     session = bigframes.Session(
         context=bigframes.BigQueryOptions(location=bigquery_location)
     )
 
     assert session.bqclient.location == bigquery_location
 
@@ -81,15 +85,16 @@
 
     # assert that bigframes session honors the location
     _assert_bq_execution_location(session)
 
 
 @pytest.mark.parametrize(
     "bigquery_location",
-    config.REP_ENABLED_BIGQUERY_LOCATIONS,
+    # Sort the set to avoid nondeterminism.
+    sorted(bigframes.constants.REP_ENABLED_BIGQUERY_LOCATIONS),
 )
 def test_bq_rep_endpoints(bigquery_location):
     session = bigframes.Session(
         context=bigframes.BigQueryOptions(
             location=bigquery_location, use_regional_endpoints=True
         )
     )
@@ -104,15 +109,16 @@
 
     # assert that bigframes session honors the location
     _assert_bq_execution_location(session)
 
 
 @pytest.mark.parametrize(
     "bigquery_location",
-    config.LEP_ENABLED_BIGQUERY_LOCATIONS,
+    # Sort the set to avoid nondeterminism.
+    sorted(bigframes.constants.LEP_ENABLED_BIGQUERY_LOCATIONS),
 )
 def test_bq_lep_endpoints(bigquery_location):
     # We are not testing BigFrames Session for LEP endpoints because it involves
     # query execution using the endpoint, which requires the project to be
     # allowlisted for LEP access. We could hardcode one project which is
     # allowlisted but then not every open source developer will have access to
     # that. Let's rely on just creating the clients for LEP.
```

### Comparing `bigframes-1.1.0/tests/system/large/test_remote_function.py` & `bigframes-1.2.0/tests/system/large/test_remote_function.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/system/large/test_session.py` & `bigframes-1.2.0/tests/system/large/test_session.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/system/load/test_large_tables.py` & `bigframes-1.2.0/tests/system/load/test_large_tables.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/system/small/__init__.py` & `bigframes-1.2.0/tests/system/small/ml/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/system/small/ml/__init__.py` & `bigframes-1.2.0/tests/system/small/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/system/small/ml/conftest.py` & `bigframes-1.2.0/tests/system/small/ml/conftest.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/system/small/ml/test_cluster.py` & `bigframes-1.2.0/tests/system/small/ml/test_cluster.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/system/small/ml/test_core.py` & `bigframes-1.2.0/tests/system/small/ml/test_core.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/system/small/ml/test_decomposition.py` & `bigframes-1.2.0/tests/system/small/ml/test_decomposition.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/system/small/ml/test_ensemble.py` & `bigframes-1.2.0/tests/system/small/ml/test_ensemble.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/system/small/ml/test_forecasting.py` & `bigframes-1.2.0/tests/system/small/ml/test_forecasting.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/system/small/ml/test_imported.py` & `bigframes-1.2.0/tests/system/small/ml/test_imported.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/system/small/ml/test_linear_model.py` & `bigframes-1.2.0/tests/system/small/ml/test_linear_model.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/system/small/ml/test_llm.py` & `bigframes-1.2.0/tests/system/small/ml/test_llm.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/system/small/ml/test_metrics.py` & `bigframes-1.2.0/tests/system/small/ml/test_metrics.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/system/small/ml/test_metrics_pairwise.py` & `bigframes-1.2.0/tests/system/small/ml/test_metrics_pairwise.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/system/small/ml/test_model_selection.py` & `bigframes-1.2.0/tests/system/small/ml/test_model_selection.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/system/small/ml/test_preprocessing.py` & `bigframes-1.2.0/tests/system/small/ml/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/system/small/ml/test_register.py` & `bigframes-1.2.0/tests/system/small/ml/test_register.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/system/small/ml/test_remote.py` & `bigframes-1.2.0/tests/system/small/ml/test_remote.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/system/small/operations/__init__.py` & `bigframes-1.2.0/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/system/small/operations/test_datetimes.py` & `bigframes-1.2.0/tests/system/small/operations/test_datetimes.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/system/small/operations/test_plotting.py` & `bigframes-1.2.0/tests/system/small/operations/test_plotting.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,21 +23,18 @@
 
 def _check_legend_labels(ax, labels):
     """
     Check the ax has expected legend label
     """
     assert ax.get_legend() is not None
     texts = ax.get_legend().get_texts()
-    if not isinstance(texts, list):
-        assert texts.get_text() == labels
-    else:
-        actual_labels = [t.get_text() for t in texts]
-        assert len(actual_labels) == len(labels)
-        for label, e in zip(actual_labels, labels):
-            assert label == e
+    actual_labels = [t.get_text() for t in texts]
+    assert len(actual_labels) == len(labels)
+    for label, e in zip(actual_labels, labels):
+        assert label == e
 
 
 def test_series_hist_bins(scalars_dfs):
     scalars_df, scalars_pandas_df = scalars_dfs
     bins = 5
     ax = scalars_df["int64_col"].plot.hist(bins=bins)
     pd_ax = scalars_pandas_df["int64_col"].plot.hist(bins=bins)
```

### Comparing `bigframes-1.1.0/tests/system/small/operations/test_strings.py` & `bigframes-1.2.0/tests/system/small/operations/test_strings.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/system/small/regression/test_issue355_merge_after_filter.py` & `bigframes-1.2.0/tests/system/small/regression/test_issue355_merge_after_filter.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/system/small/test_dataframe.py` & `bigframes-1.2.0/tests/system/small/test_dataframe.py`

 * *Files 0% similar despite different names*

```diff
@@ -520,21 +520,14 @@
 
     # Remove columns with flaky formatting, like NUMERIC columns (which use the
     # object dtype). Also makes a copy so that mutating the index name doesn't
     # break other tests.
     scalars_df = scalars_df.drop(columns=["numeric_col"])
     scalars_pandas_df = scalars_pandas_df.drop(columns=["numeric_col"])
 
-    if scalars_pandas_df.index.name is None:
-        # Note: Not quite the same as no index / default index, but hopefully
-        # simulates it well enough while being consistent enough for string
-        # comparison to work.
-        scalars_df = scalars_df.set_index("rowindex", drop=False).sort_index()
-        scalars_df.index.name = None
-
     # When there are 10 or fewer rows, the outputs should be identical.
     actual = repr(scalars_df.head(10))
 
     with display_options.pandas_repr(bigframes.options.display):
         expected = repr(scalars_pandas_df.head(10))
 
     assert actual == expected
@@ -2609,14 +2602,42 @@
         values=values, index=index, columns=columns
     )
 
     # Pandas produces NaN, where bq dataframes produces pd.NA
     pd.testing.assert_frame_equal(bf_result, pd_result, check_dtype=False)
 
 
+@pytest.mark.parametrize(
+    ("values", "index", "columns", "aggfunc"),
+    [
+        (("culmen_length_mm", "body_mass_g"), "species", "sex", "std"),
+        (["body_mass_g", "culmen_length_mm"], ("species", "island"), "sex", "sum"),
+        ("body_mass_g", "sex", ["island", "species"], "mean"),
+        ("culmen_depth_mm", "island", "species", "max"),
+    ],
+)
+def test_df_pivot_table(
+    penguins_df_default_index,
+    penguins_pandas_df_default_index,
+    values,
+    index,
+    columns,
+    aggfunc,
+):
+    bf_result = penguins_df_default_index.pivot_table(
+        values=values, index=index, columns=columns, aggfunc=aggfunc
+    ).to_pandas()
+    pd_result = penguins_pandas_df_default_index.pivot_table(
+        values=values, index=index, columns=columns, aggfunc=aggfunc
+    )
+    pd.testing.assert_frame_equal(
+        bf_result, pd_result, check_dtype=False, check_column_type=False
+    )
+
+
 def test_ipython_key_completions_with_drop(scalars_dfs):
     scalars_df, scalars_pandas_df = scalars_dfs
     col_names = "string_col"
     bf_dataframe = scalars_df.drop(columns=col_names)
     pd_dataframe = scalars_pandas_df.drop(columns=col_names)
     expected = pd_dataframe.columns.tolist()
 
@@ -2893,23 +2914,31 @@
 
     pd.testing.assert_frame_equal(
         bf_df.to_pandas(),
         pd_df,
     )
 
 
-def test_loc_setitem_bool_series_scalar_existing_col(scalars_dfs):
+@pytest.mark.parametrize(
+    ("col", "value"),
+    [
+        ("string_col", "hello"),
+        ("int64_col", 3),
+        ("float64_col", 3.5),
+    ],
+)
+def test_loc_setitem_bool_series_scalar_existing_col(scalars_dfs, col, value):
     if pd.__version__.startswith("1."):
         pytest.skip("this loc overload not supported in pandas 1.x.")
 
     scalars_df, scalars_pandas_df = scalars_dfs
     bf_df = scalars_df.copy()
     pd_df = scalars_pandas_df.copy()
-    bf_df.loc[bf_df["int64_too"] == 1, "string_col"] = "hello"
-    pd_df.loc[pd_df["int64_too"] == 1, "string_col"] = "hello"
+    bf_df.loc[bf_df["int64_too"] == 1, col] = value
+    pd_df.loc[pd_df["int64_too"] == 1, col] = value
 
     pd.testing.assert_frame_equal(
         bf_df.to_pandas(),
         pd_df,
     )
 
 
@@ -3952,17 +3981,14 @@
         ("keep", "average", True, True),
         ("top", "min", False, False),
         ("bottom", "max", False, False),
         ("top", "first", False, False),
         ("bottom", "dense", False, False),
     ],
 )
-@pytest.mark.skipif(
-    True, reason="Blocked by possible pandas rank() regression (b/283278923)"
-)
 def test_df_rank_with_nulls(
     scalars_df_index,
     scalars_pandas_df_index,
     na_option,
     method,
     ascending,
     numeric_only,
```

### Comparing `bigframes-1.1.0/tests/system/small/test_dataframe_io.py` & `bigframes-1.2.0/tests/system/small/test_dataframe_io.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 import pyarrow as pa
 import pytest
 
 from tests.system import utils
 
 try:
     import pandas_gbq  # type: ignore
-except ImportError:
+except ImportError:  # pragma: NO COVER
+    # TODO(b/332758806): Run system tests without "extras"
     pandas_gbq = None
 
 import typing
 
 import bigframes
 import bigframes.dataframe
 import bigframes.features
@@ -125,20 +126,17 @@
     index: bool,
 ):
     if pd.__version__.startswith("1."):
         pytest.skip("date_format parameter not supported in pandas 1.x.")
     """Test the `to_csv` API with the `index` parameter."""
     scalars_df, scalars_pandas_df = scalars_dfs
     index_col = None
-    if scalars_df.index.name is not None:
-        path = gcs_folder + f"test_index_df_to_csv_index_{index}*.csv"
-        if index:
-            index_col = typing.cast(str, scalars_df.index.name)
-    else:
-        path = gcs_folder + f"test_default_index_df_to_csv_index_{index}*.csv"
+    path = gcs_folder + f"test_index_df_to_csv_index_{index}*.csv"
+    if index:
+        index_col = typing.cast(str, scalars_df.index.name)
 
     # TODO(swast): Support "date_format" parameter and make sure our
     # DATETIME/TIMESTAMP column export is the same format as pandas by default.
     scalars_df.to_csv(path, index=index)
 
     # Pandas dataframes dtypes from read_csv are not fully compatible with
     # BigQuery-backed dataframes, so manually convert the dtypes specifically
@@ -382,58 +380,51 @@
     [True, False],
 )
 def test_to_json_index_invalid_orient(
     scalars_dfs: Tuple[bigframes.dataframe.DataFrame, pd.DataFrame],
     gcs_folder: str,
     index: bool,
 ):
-    scalars_df, scalars_pandas_df = scalars_dfs
-    if scalars_df.index.name is not None:
-        path = gcs_folder + f"test_index_df_to_json_index_{index}*.jsonl"
-    else:
-        path = gcs_folder + f"test_default_index_df_to_json_index_{index}*.jsonl"
+    scalars_df, _ = scalars_dfs
+    path = gcs_folder + f"test_index_df_to_json_index_{index}*.jsonl"
     with pytest.raises(ValueError):
         scalars_df.to_json(path, index=index, lines=True)
 
 
 @pytest.mark.parametrize(
     ("index"),
     [True, False],
 )
 def test_to_json_index_invalid_lines(
     scalars_dfs: Tuple[bigframes.dataframe.DataFrame, pd.DataFrame],
     gcs_folder: str,
     index: bool,
 ):
-    scalars_df, scalars_pandas_df = scalars_dfs
-    if scalars_df.index.name is not None:
-        path = gcs_folder + f"test_index_df_to_json_index_{index}.jsonl"
-    else:
-        path = gcs_folder + f"test_default_index_df_to_json_index_{index}.jsonl"
+    scalars_df, _ = scalars_dfs
+    path = gcs_folder + f"test_index_df_to_json_index_{index}.jsonl"
     with pytest.raises(NotImplementedError):
         scalars_df.to_json(path, index=index)
 
 
 @pytest.mark.parametrize(
     ("index"),
     [True, False],
 )
 def test_to_json_index_records_orient(
     scalars_dfs: Tuple[bigframes.dataframe.DataFrame, pd.DataFrame],
     gcs_folder: str,
     index: bool,
 ):
-    """Test the `to_json` API with the `index` parameter."""
+    """Test the `to_json` API with the `index` parameter.
+
+    Uses the scalable options orient='records' and lines=True.
+    """
     scalars_df, scalars_pandas_df = scalars_dfs
-    if scalars_df.index.name is not None:
-        path = gcs_folder + f"test_index_df_to_json_index_{index}*.jsonl"
-    else:
-        path = gcs_folder + f"test_default_index_df_to_json_index_{index}*.jsonl"
+    path = gcs_folder + f"test_index_df_to_json_index_{index}*.jsonl"
 
-    """ Test the `to_json` API with `orient` is `records` and `lines` is True"""
     scalars_df.to_json(path, index=index, orient="records", lines=True)
 
     gcs_df = pd.read_json(
         utils.get_first_file_from_wildcard(path),
         lines=True,
         convert_dates=["datetime_col"],
     )
@@ -456,19 +447,15 @@
     ("index"),
     [True, False],
 )
 def test_to_parquet_index(scalars_dfs, gcs_folder, index):
     """Test the `to_parquet` API with the `index` parameter."""
     scalars_df, scalars_pandas_df = scalars_dfs
     scalars_pandas_df = scalars_pandas_df.copy()
-
-    if scalars_df.index.name is not None:
-        path = gcs_folder + f"test_index_df_to_parquet_{index}*.parquet"
-    else:
-        path = gcs_folder + f"test_default_index_df_to_parquet_{index}*.parquet"
+    path = gcs_folder + f"test_index_df_to_parquet_{index}*.parquet"
 
     # TODO(b/268693993): Type GEOGRAPHY is not currently supported for parquet.
     scalars_df = scalars_df.drop(columns="geography_col")
     scalars_pandas_df = scalars_pandas_df.drop(columns="geography_col")
 
     # TODO(swast): Do a bit more processing on the input DataFrame to ensure
     # the exported results are from the generated query, not just the source
```

### Comparing `bigframes-1.1.0/tests/system/small/test_encryption.py` & `bigframes-1.2.0/tests/system/small/test_encryption.py`

 * *Files 10% similar despite different names*

```diff
@@ -60,16 +60,16 @@
 
     # The result table should exist with the intended encryption
     table = session.bqclient.get_table(df.query_job.destination)
     assert table.encryption_configuration.kms_key_name == cmek
 
 
 def test_session_query_job(bq_cmek, session_with_bq_cmek):
-    if not bq_cmek:
-        pytest.skip("no cmek set for testing")
+    if not bq_cmek:  # pragma: NO COVER
+        pytest.skip("no cmek set for testing")  # pragma: NO COVER
 
     _, query_job = session_with_bq_cmek._start_query(
         "SELECT 123", job_config=bigquery.QueryJobConfig(use_query_cache=False)
     )
     query_job.result()
 
     assert query_job.destination_encryption_configuration.kms_key_name.startswith(
@@ -78,16 +78,16 @@
 
     # The result table should exist with the intended encryption
     table = session_with_bq_cmek.bqclient.get_table(query_job.destination)
     assert table.encryption_configuration.kms_key_name == bq_cmek
 
 
 def test_session_load_job(bq_cmek, session_with_bq_cmek):
-    if not bq_cmek:
-        pytest.skip("no cmek set for testing")
+    if not bq_cmek:  # pragma: NO COVER
+        pytest.skip("no cmek set for testing")  # pragma: NO COVER
 
     # Session should have cmek set in the default query and load job configs
     load_table = bigframes.session._io.bigquery.random_table(
         session_with_bq_cmek._anonymous_dataset
     )
 
     df = pandas.DataFrame({"col0": [1, 2, 3]})
@@ -110,27 +110,27 @@
 
     # The load destination table should be created with the intended encryption
     table = session_with_bq_cmek.bqclient.get_table(load_job.destination)
     assert table.encryption_configuration.kms_key_name == bq_cmek
 
 
 def test_read_gbq(bq_cmek, session_with_bq_cmek, scalars_table_id):
-    if not bq_cmek:
-        pytest.skip("no cmek set for testing")
+    if not bq_cmek:  # pragma: NO COVER
+        pytest.skip("no cmek set for testing")  # pragma: NO COVER
 
     # Read the BQ table
     df = session_with_bq_cmek.read_gbq(scalars_table_id)
 
     # Assert encryption
     _assert_bq_table_is_encrypted(df, bq_cmek, session_with_bq_cmek)
 
 
 def test_df_apis(bq_cmek, session_with_bq_cmek, scalars_table_id):
-    if not bq_cmek:
-        pytest.skip("no cmek set for testing")
+    if not bq_cmek:  # pragma: NO COVER
+        pytest.skip("no cmek set for testing")  # pragma: NO COVER
 
     # Read a BQ table and assert encryption
     df = session_with_bq_cmek.read_gbq(scalars_table_id)
 
     # Perform a few dataframe operations and assert encryption
     df1 = df.dropna()
     _assert_bq_table_is_encrypted(df1, bq_cmek, session_with_bq_cmek)
@@ -148,16 +148,16 @@
             id="default_engine",
         ),
     ],
 )
 def test_read_csv_gcs(
     bq_cmek, session_with_bq_cmek, scalars_df_index, gcs_folder, engine
 ):
-    if not bq_cmek:
-        pytest.skip("no cmek set for testing")
+    if not bq_cmek:  # pragma: NO COVER
+        pytest.skip("no cmek set for testing")  # pragma: NO COVER
 
     # Create a csv in gcs
     write_path = gcs_folder + "test_read_csv_gcs_bigquery_engine*.csv"
     read_path = (
         utils.get_first_file_from_wildcard(write_path) if engine is None else write_path
     )
     scalars_df_index.to_csv(write_path)
@@ -166,16 +166,16 @@
     df = session_with_bq_cmek.read_csv(read_path, engine=engine)
 
     # Assert encryption
     _assert_bq_table_is_encrypted(df, bq_cmek, session_with_bq_cmek)
 
 
 def test_to_gbq(bq_cmek, session_with_bq_cmek, scalars_table_id):
-    if not bq_cmek:
-        pytest.skip("no cmek set for testing")
+    if not bq_cmek:  # pragma: NO COVER
+        pytest.skip("no cmek set for testing")  # pragma: NO COVER
 
     # Read a BQ table and assert encryption
     df = session_with_bq_cmek.read_gbq(scalars_table_id)
     _assert_bq_table_is_encrypted(df, bq_cmek, session_with_bq_cmek)
 
     # Modify the dataframe and assert encryption
     df = df.dropna().head()
@@ -201,38 +201,38 @@
     output_table_dataset = session_with_bq_cmek.bqclient.get_dataset(
         output_table.dataset_id
     )
     assert output_table_dataset.default_encryption_configuration is None
 
 
 def test_read_pandas(bq_cmek, session_with_bq_cmek):
-    if not bq_cmek:
-        pytest.skip("no cmek set for testing")
+    if not bq_cmek:  # pragma: NO COVER
+        pytest.skip("no cmek set for testing")  # pragma: NO COVER
 
     # Read a pandas dataframe
     df = session_with_bq_cmek.read_pandas(pandas.DataFrame([1]))
 
     # Assert encryption
     _assert_bq_table_is_encrypted(df, bq_cmek, session_with_bq_cmek)
 
 
 def test_read_pandas_large(bq_cmek, session_with_bq_cmek):
-    if not bq_cmek:
-        pytest.skip("no cmek set for testing")
+    if not bq_cmek:  # pragma: NO COVER
+        pytest.skip("no cmek set for testing")  # pragma: NO COVER
 
     # Read a pandas dataframe large enough to trigger a BQ load job
     df = session_with_bq_cmek.read_pandas(pandas.DataFrame(range(10_000)))
 
     # Assert encryption
     _assert_bq_table_is_encrypted(df, bq_cmek, session_with_bq_cmek)
 
 
 def test_bqml(bq_cmek, session_with_bq_cmek, penguins_table_id):
-    if not bq_cmek:
-        pytest.skip("no cmek set for testing")
+    if not bq_cmek:  # pragma: NO COVER
+        pytest.skip("no cmek set for testing")  # pragma: NO COVER
 
     model = bigframes.ml.linear_model.LinearRegression()
     df = session_with_bq_cmek.read_gbq(penguins_table_id).dropna()
     X_train = df[
         [
             "species",
             "island",
```

### Comparing `bigframes-1.1.0/tests/system/small/test_groupby.py` & `bigframes-1.2.0/tests/system/small/test_groupby.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/system/small/test_ibis.py` & `bigframes-1.2.0/tests/system/small/test_ibis.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/system/small/test_index.py` & `bigframes-1.2.0/tests/system/small/test_index.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/system/small/test_ipython.py` & `bigframes-1.2.0/tests/system/small/test_ipython.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/system/small/test_multiindex.py` & `bigframes-1.2.0/tests/system/small/test_multiindex.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,39 @@
 import pandas
 import pytest
 
 import bigframes.pandas as bpd
 from tests.system.utils import assert_pandas_df_equal, skip_legacy_pandas
 
 
+def test_multi_index_from_arrays():
+    bf_idx = bpd.MultiIndex.from_arrays(
+        [
+            pandas.Index([4, 99], dtype=pandas.Int64Dtype()),
+            pandas.Index(
+                [" Hello, World!", "_some_new_string"],
+                dtype=pandas.StringDtype(storage="pyarrow"),
+            ),
+        ],
+        names=[" 1index 1", "_1index 2"],
+    )
+    pd_idx = pandas.MultiIndex.from_arrays(
+        [
+            pandas.Index([4, 99], dtype=pandas.Int64Dtype()),
+            pandas.Index(
+                [" Hello, World!", "_some_new_string"],
+                dtype=pandas.StringDtype(storage="pyarrow"),
+            ),
+        ],
+        names=[" 1index 1", "_1index 2"],
+    )
+    assert bf_idx.names == pd_idx.names
+    pandas.testing.assert_index_equal(bf_idx.to_pandas(), pd_idx)
+
+
 @skip_legacy_pandas
 def test_read_pandas_multi_index_axes():
     index = pandas.MultiIndex.from_arrays(
         [
             pandas.Index([4, 99], dtype=pandas.Int64Dtype()),
             pandas.Index(
                 [" Hello, World!", "_some_new_string"],
@@ -878,33 +903,14 @@
     pd_result = pd_df.unstack()
 
     # Pandas produces NaN, where bq dataframes produces pd.NA
     # Column ordering seems to depend on pandas version
     pandas.testing.assert_series_equal(bf_result, pd_result, check_dtype=False)
 
 
-@pytest.mark.skip(reason="Pandas fails in newer versions.")
-def test_column_multi_index_w_na_stack(scalars_df_index, scalars_pandas_df_index):
-    columns = ["int64_too", "int64_col", "rowindex_2"]
-    level1 = pandas.Index(["b", pandas.NA, pandas.NA])
-    # Need resulting column to be pyarrow string rather than object dtype
-    level2 = pandas.Index([pandas.NA, "b", "b"], dtype="string[pyarrow]")
-    multi_columns = pandas.MultiIndex.from_arrays([level1, level2])
-    bf_df = scalars_df_index[columns].copy()
-    bf_df.columns = multi_columns
-    pd_df = scalars_pandas_df_index[columns].copy()
-    pd_df.columns = multi_columns
-
-    bf_result = bf_df.stack().to_pandas()
-    pd_result = pd_df.stack()
-
-    # Pandas produces NaN, where bq dataframes produces pd.NA
-    pandas.testing.assert_frame_equal(bf_result, pd_result, check_dtype=False)
-
-
 def test_corr_w_multi_index(scalars_df_index, scalars_pandas_df_index):
     columns = ["int64_too", "float64_col", "int64_col"]
     multi_columns = pandas.MultiIndex.from_tuples(zip(["a", "b", "b"], [1, 2, 2]))
 
     bf = scalars_df_index[columns].copy()
     bf.columns = multi_columns
```

### Comparing `bigframes-1.1.0/tests/system/small/test_numpy.py` & `bigframes-1.2.0/tests/system/small/test_numpy.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/system/small/test_pandas.py` & `bigframes-1.2.0/tests/system/small/test_pandas.py`

 * *Files 4% similar despite different names*

```diff
@@ -132,15 +132,15 @@
 
     bf_result = bpd.get_dummies(bf_series, dtype=bool)
     pd_result = pd.get_dummies(pd_series, dtype=bool)
     # dtype argument above is needed for pandas v1 only
 
     # adjust for expected dtype differences
     for (column_name, type_name) in zip(pd_result.columns, pd_result.dtypes):
-        if type_name == "bool":
+        if type_name == "bool":  # pragma: NO COVER
             pd_result[column_name] = pd_result[column_name].astype("boolean")
     pd_result.columns = pd_result.columns.astype(object)
 
     pd.testing.assert_frame_equal(
         bf_result.to_pandas(),
         pd_result,
     )
@@ -153,15 +153,15 @@
 
     bf_result = bpd.get_dummies(bf_series, dtype=bool)
     pd_result = pd.get_dummies(pd_series, dtype=bool)
     # dtype argument above is needed for pandas v1 only
 
     # adjust for expected dtype differences
     for (column_name, type_name) in zip(pd_result.columns, pd_result.dtypes):
-        if type_name == "bool":
+        if type_name == "bool":  # pragma: NO COVER
             pd_result[column_name] = pd_result[column_name].astype("boolean")
     pd_result.columns = pd_result.columns.astype(object)
 
     pd.testing.assert_frame_equal(
         bf_result.to_pandas(),
         pd_result,
     )
@@ -421,14 +421,66 @@
 
     pd.testing.assert_series_equal(
         bf_result, pd_result_converted, check_index=False, check_dtype=False
     )
 
 
 @pytest.mark.parametrize(
+    ("breaks",),
+    [
+        ([0, 5, 10, 15, 20, 100, 1000],),  # ints
+        ([0.5, 10.5, 15.5, 20.5, 100.5, 1000.5],),  # floats
+        ([0, 5, 10.5, 15.5, 20, 100, 1000.5],),  # mixed
+    ],
+)
+def test_cut_numeric_breaks(scalars_dfs, breaks):
+    scalars_df, scalars_pandas_df = scalars_dfs
+
+    pd_result = pd.cut(scalars_pandas_df["float64_col"], breaks)
+    bf_result = bpd.cut(scalars_df["float64_col"], breaks).to_pandas()
+
+    # Convert to match data format
+    pd_result_converted = pd.Series(
+        [
+            {"left_exclusive": interval.left, "right_inclusive": interval.right}
+            if pd.notna(val)
+            else pd.NA
+            for val, interval in zip(
+                pd_result, pd_result.cat.categories[pd_result.cat.codes]
+            )
+        ],
+        name=pd_result.name,
+    )
+
+    pd.testing.assert_series_equal(
+        bf_result, pd_result_converted, check_index=False, check_dtype=False
+    )
+
+
+@pytest.mark.parametrize(
+    ("bins",),
+    [
+        (-1,),  # negative integer bins argument
+        ([],),  # empty iterable of bins
+        (["notabreak"],),  # iterable of wrong type
+        ([1],),  # numeric breaks with only one numeric
+        # this is supported by pandas but not by
+        # the bigquery operation and a bigframes workaround
+        # is not yet available. Should return column
+        # of structs with all NaN values.
+    ],
+)
+def test_cut_errors(scalars_dfs, bins):
+    scalars_df, _ = scalars_dfs
+
+    with pytest.raises(ValueError):
+        bpd.cut(scalars_df["float64_col"], bins)
+
+
+@pytest.mark.parametrize(
     ("bins",),
     [
         ([(-5, 2), (2, 3), (-3000, -10)],),
         (pd.IntervalIndex.from_tuples([(1, 2), (2, 3), (4, 5)]),),
     ],
 )
 def test_cut_with_interval(scalars_dfs, bins):
```

### Comparing `bigframes-1.1.0/tests/system/small/test_pandas_options.py` & `bigframes-1.2.0/tests/system/small/test_pandas_options.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/system/small/test_progress_bar.py` & `bigframes-1.2.0/tests/system/small/test_progress_bar.py`

 * *Files 5% similar despite different names*

```diff
@@ -122,17 +122,7 @@
         "Destination Table",
         "Slot Time",
         "Bytes Processed",
         "Cache hit",
     ]
     for string in string_checks:
         assert string in query_job_repr
-
-
-def test_query_job_dry_run(penguins_df_default_index: bf.dataframe.DataFrame, capsys):
-    with bf.option_context("display.repr_mode", "deferred"):
-        repr(penguins_df_default_index)
-        repr(penguins_df_default_index["body_mass_g"])
-        lines = capsys.readouterr().out.split("\n")
-        lines = filter(None, lines)
-        for line in lines:
-            assert "Computation deferred. Computation will process" in line
```

### Comparing `bigframes-1.1.0/tests/system/small/test_remote_function.py` & `bigframes-1.2.0/tests/system/small/test_remote_function.py`

 * *Files 7% similar despite different names*

```diff
@@ -101,15 +101,16 @@
         resource_manager_client=resourcemanager_client,
         dataset=dataset_id_permanent,
         bigquery_connection=bq_cf_connection,
         # See e2e tests for tests that actually deploy the Cloud Function.
         reuse=True,
     )
     def square(x):
-        return x * x
+        # This executes on a remote function, where coverage isn't tracked.
+        return x * x  # pragma: NO COVER
 
     assert square.bigframes_remote_function
     assert square.bigframes_cloud_function
 
     scalars_df, scalars_pandas_df = scalars_dfs
 
     bf_int64_col = scalars_df["int64_col"]
@@ -153,15 +154,16 @@
         resource_manager_client=resourcemanager_client,
         dataset=dataset_id_permanent,
         bigquery_connection=bq_cf_connection_location,
         # See e2e tests for tests that actually deploy the Cloud Function.
         reuse=True,
     )
     def square(x):
-        return x * x
+        # This executes on a remote function, where coverage isn't tracked.
+        return x * x  # pragma: NO COVER
 
     scalars_df, scalars_pandas_df = scalars_dfs
 
     bf_int64_col = scalars_df["int64_col"]
     bf_int64_col_filter = bf_int64_col.notnull()
     bf_int64_col_filtered = bf_int64_col[bf_int64_col_filter]
     bf_result_col = bf_int64_col_filtered.apply(square)
@@ -203,15 +205,16 @@
             resource_manager_client=resourcemanager_client,
             dataset=dataset_id_permanent,
             bigquery_connection=bq_cf_connection_location_mismatched,
             # See e2e tests for tests that actually deploy the Cloud Function.
             reuse=True,
         )
         def square(x):
-            return x * x
+            # This executes on a remote function, where coverage isn't tracked.
+            return x * x  # pragma: NO COVER
 
 
 @pytest.mark.flaky(retries=2, delay=120)
 def test_remote_function_direct_no_session_param_location_project_specified(
     bigquery_client,
     bigqueryconnection_client,
     cloudfunctions_client,
@@ -229,15 +232,16 @@
         resource_manager_client=resourcemanager_client,
         dataset=dataset_id_permanent,
         bigquery_connection=bq_cf_connection_location_project,
         # See e2e tests for tests that actually deploy the Cloud Function.
         reuse=True,
     )
     def square(x):
-        return x * x
+        # This executes on a remote function, where coverage isn't tracked.
+        return x * x  # pragma: NO COVER
 
     scalars_df, scalars_pandas_df = scalars_dfs
 
     bf_int64_col = scalars_df["int64_col"]
     bf_int64_col_filter = bf_int64_col.notnull()
     bf_int64_col_filtered = bf_int64_col[bf_int64_col_filter]
     bf_result_col = bf_int64_col_filtered.apply(square)
@@ -279,26 +283,28 @@
             resource_manager_client=resourcemanager_client,
             dataset=dataset_id_permanent,
             bigquery_connection=bq_cf_connection_location_project_mismatched,
             # See e2e tests for tests that actually deploy the Cloud Function.
             reuse=True,
         )
         def square(x):
-            return x * x
+            # This executes on a remote function, where coverage isn't tracked.
+            return x * x  # pragma: NO COVER
 
 
 @pytest.mark.flaky(retries=2, delay=120)
 def test_remote_function_direct_session_param(session_with_bq_connection, scalars_dfs):
     @rf.remote_function(
         [int],
         int,
         session=session_with_bq_connection,
     )
     def square(x):
-        return x * x
+        # This executes on a remote function, where coverage isn't tracked.
+        return x * x  # pragma: NO COVER
 
     scalars_df, scalars_pandas_df = scalars_dfs
 
     bf_int64_col = scalars_df["int64_col"]
     bf_int64_col_filter = bf_int64_col.notnull()
     bf_int64_col_filtered = bf_int64_col[bf_int64_col_filter]
     bf_result_col = bf_int64_col_filtered.apply(square)
@@ -327,15 +333,16 @@
     # Without an explicit bigquery connection, the one present in Session set
     # through the explicit BigQueryOptions would be used. Without an explicit `reuse`
     # the default behavior of reuse=True will take effect. Please note that the
     # udf is same as the one used in other tests in this file so the underlying
     # cloud function would be common and quickly reused.
     @session_with_bq_connection.remote_function([int], int)
     def square(x):
-        return x * x
+        # This executes on a remote function, where coverage isn't tracked.
+        return x * x  # pragma: NO COVER
 
     scalars_df, scalars_pandas_df = scalars_dfs
 
     bf_int64_col = scalars_df["int64_col"]
     bf_int64_col_filter = bf_int64_col.notnull()
     bf_int64_col_filtered = bf_int64_col[bf_int64_col_filter]
     bf_result_col = bf_int64_col_filtered.apply(square)
@@ -366,15 +373,16 @@
         int,
         dataset_id_permanent,
         bq_cf_connection,
         # See e2e tests for tests that actually deploy the Cloud Function.
         reuse=True,
     )
     def square(x):
-        return x * x
+        # This executes on a remote function, where coverage isn't tracked.
+        return x * x  # pragma: NO COVER
 
     scalars_df, scalars_pandas_df = scalars_dfs
 
     bf_int64_col = scalars_df["int64_col"]
     bf_int64_col_filter = bf_int64_col.notnull()
     bf_int64_col_filtered = bf_int64_col[bf_int64_col_filter]
     bf_result_col = bf_int64_col_filtered.apply(square)
@@ -493,15 +501,16 @@
     with pytest.raises(
         google.api_core.exceptions.NotFound,
         match=f"Not found: Connection {connection_name}",
     ):
 
         @session.remote_function([int], int, dataset=dataset_id_permanent)
         def add_one(x):
-            return x + 1
+            # This executes on a remote function, where coverage isn't tracked.
+            return x + 1  # pragma: NO COVER
 
 
 @pytest.mark.flaky(retries=2, delay=120)
 def test_read_gbq_function_detects_invalid_function(bigquery_client, dataset_id):
     dataset_ref = bigquery.DatasetReference.from_string(dataset_id)
     with pytest.raises(ValueError) as e:
         rf.read_gbq_function(
@@ -530,15 +539,16 @@
         dataset=dataset_id_permanent,
         cloud_functions_client=cloudfunctions_client,
         resource_manager_client=resourcemanager_client,
         bigquery_connection=bq_cf_connection,
         reuse=True,
     )
     def square1(x):
-        return x * x
+        # This executes on a remote function, where coverage isn't tracked.
+        return x * x  # pragma: NO COVER
 
     square2 = rf.read_gbq_function(
         function_name=square1.bigframes_remote_function,
         bigquery_client=bigquery_client,
     )
 
     # The newly-created function (square1) should have a remote function AND a
```

### Comparing `bigframes-1.1.0/tests/system/small/test_scalar.py` & `bigframes-1.2.0/tests/system/small/test_scalar.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/system/small/test_series.py` & `bigframes-1.2.0/tests/system/small/test_series.py`

 * *Files 2% similar despite different names*

```diff
@@ -280,14 +280,29 @@
     scalars_df, scalars_pandas_df = scalars_dfs
     bf_result = scalars_df[col_name].abs().to_pandas()
     pd_result = scalars_pandas_df[col_name].abs()
 
     assert_series_equal(pd_result, bf_result)
 
 
+@pytest.mark.parametrize(
+    ("col_name",),
+    (
+        ("bool_col",),
+        ("int64_col",),
+    ),
+)
+def test_series_invert(scalars_dfs, col_name):
+    scalars_df, scalars_pandas_df = scalars_dfs
+    bf_result = (~scalars_df[col_name]).to_pandas()
+    pd_result = ~scalars_pandas_df[col_name]
+
+    assert_series_equal(pd_result, bf_result)
+
+
 def test_fillna(scalars_dfs):
     scalars_df, scalars_pandas_df = scalars_dfs
     col_name = "string_col"
     bf_result = scalars_df[col_name].fillna("Missing").to_pandas()
     pd_result = scalars_pandas_df[col_name].fillna("Missing")
     assert_series_equal(
         pd_result,
@@ -699,14 +714,22 @@
         scalars_pandas_df["int64_too"]
         .astype("int64")
         .corr(scalars_pandas_df["int64_too"].astype("int64"))
     )
     assert math.isclose(pd_result, bf_result)
 
 
+@skip_legacy_pandas
+def test_series_autocorr(scalars_dfs):
+    scalars_df, scalars_pandas_df = scalars_dfs
+    bf_result = scalars_df["float64_col"].autocorr(2)
+    pd_result = scalars_pandas_df["float64_col"].autocorr(2)
+    assert math.isclose(pd_result, bf_result)
+
+
 def test_series_cov(scalars_dfs):
     scalars_df, scalars_pandas_df = scalars_dfs
     bf_result = scalars_df["int64_too"].cov(scalars_df["int64_too"])
     pd_result = (
         scalars_pandas_df["int64_too"]
         .astype("int64")
         .cov(scalars_pandas_df["int64_too"].astype("int64"))
@@ -1242,14 +1265,47 @@
 
     assert_series_equal(
         bf_result,
         pd_result,
     )
 
 
+@skip_legacy_pandas
+def test_series_combine_first(scalars_dfs):
+    scalars_df, scalars_pandas_df = scalars_dfs
+    int64_col = scalars_df["int64_col"].head(7)
+    float64_col = scalars_df["float64_col"].tail(7)
+    bf_result = int64_col.combine_first(float64_col).to_pandas()
+
+    pd_int64_col = scalars_pandas_df["int64_col"].head(7)
+    pd_float64_col = scalars_pandas_df["float64_col"].tail(7)
+    pd_result = pd_int64_col.combine_first(pd_float64_col)
+
+    assert_series_equal(
+        bf_result,
+        pd_result,
+    )
+
+
+def test_series_update(scalars_dfs):
+    scalars_df, scalars_pandas_df = scalars_dfs
+    int64_col = scalars_df["int64_col"].head(7)
+    float64_col = scalars_df["float64_col"].tail(7).copy()
+    float64_col.update(int64_col)
+
+    pd_int64_col = scalars_pandas_df["int64_col"].head(7)
+    pd_float64_col = scalars_pandas_df["float64_col"].tail(7).copy()
+    pd_float64_col.update(pd_int64_col)
+
+    assert_series_equal(
+        float64_col.to_pandas(),
+        pd_float64_col,
+    )
+
+
 def test_mean(scalars_dfs):
     scalars_df, scalars_pandas_df = scalars_dfs
     col_name = "int64_col"
     bf_result = scalars_df[col_name].mean()
     pd_result = scalars_pandas_df[col_name].mean()
     assert math.isclose(pd_result, bf_result)
 
@@ -1272,16 +1328,14 @@
     assert bf_result.size == scalars_df[col_name].size
     # TODO(b/323387826): The precision increased by 1 unexpectedly.
     # assert bf_result.dtype == pd.ArrowDtype(pa.decimal128(38, 9))
 
 
 def test_repr(scalars_dfs):
     scalars_df, scalars_pandas_df = scalars_dfs
-    if scalars_pandas_df.index.name != "rowindex":
-        pytest.skip("Require index & ordering for consistent repr.")
 
     col_name = "int64_col"
     bf_series = scalars_df[col_name]
     pd_series = scalars_pandas_df[col_name]
     assert repr(bf_series) == repr(pd_series)
 
 
@@ -1401,32 +1455,28 @@
     )
 
 
 def test_groupby_level_sum(scalars_dfs):
     # TODO(tbergeron): Use a non-unique index once that becomes possible in tests
     scalars_df, scalars_pandas_df = scalars_dfs
     col_name = "int64_too"
-    if scalars_pandas_df.index.name != "rowindex":
-        pytest.skip("Require index for groupby level.")
 
     bf_series = scalars_df[col_name].groupby(level=0).sum()
     pd_series = scalars_pandas_df[col_name].groupby(level=0).sum()
     # TODO(swast): Update groupby to use index based on group by key(s).
     pd.testing.assert_series_equal(
         pd_series.sort_index(),
         bf_series.to_pandas().sort_index(),
     )
 
 
 def test_groupby_level_list_sum(scalars_dfs):
     # TODO(tbergeron): Use a non-unique index once that becomes possible in tests
     scalars_df, scalars_pandas_df = scalars_dfs
     col_name = "int64_too"
-    if scalars_pandas_df.index.name != "rowindex":
-        pytest.skip("Require index for groupby level.")
 
     bf_series = scalars_df[col_name].groupby(level=["rowindex"]).sum()
     pd_series = scalars_pandas_df[col_name].groupby(level=["rowindex"]).sum()
     # TODO(swast): Update groupby to use index based on group by key(s).
     pd.testing.assert_series_equal(
         pd_series.sort_index(),
         bf_series.to_pandas().sort_index(),
@@ -1636,14 +1686,32 @@
 
     bf_result = scalars_df["string_col"].size
     pd_result = scalars_pandas_df["string_col"].size
 
     assert pd_result == bf_result
 
 
+def test_series_hasnans_true(scalars_dfs):
+    scalars_df, scalars_pandas_df = scalars_dfs
+
+    bf_result = scalars_df["string_col"].hasnans
+    pd_result = scalars_pandas_df["string_col"].hasnans
+
+    assert pd_result == bf_result
+
+
+def test_series_hasnans_false(scalars_dfs):
+    scalars_df, scalars_pandas_df = scalars_dfs
+
+    bf_result = scalars_df["string_col"].dropna().hasnans
+    pd_result = scalars_pandas_df["string_col"].dropna().hasnans
+
+    assert pd_result == bf_result
+
+
 def test_empty_false(scalars_dfs):
     scalars_df, scalars_pandas_df = scalars_dfs
 
     bf_result = scalars_df["string_col"].empty
     pd_result = scalars_pandas_df["string_col"].empty
 
     assert pd_result == bf_result
@@ -1706,62 +1774,50 @@
 
     assert pd_result == bf_result
 
 
 def test_head(scalars_dfs):
     scalars_df, scalars_pandas_df = scalars_dfs
 
-    if scalars_df.index.name is None:
-        pytest.skip("Require explicit index for offset ops.")
-
     bf_result = scalars_df["string_col"].head(2).to_pandas()
     pd_result = scalars_pandas_df["string_col"].head(2)
 
     assert_series_equal(
         pd_result,
         bf_result,
     )
 
 
 def test_tail(scalars_dfs):
     scalars_df, scalars_pandas_df = scalars_dfs
 
-    if scalars_df.index.name is None:
-        pytest.skip("Require explicit index for offset ops.")
-
     bf_result = scalars_df["string_col"].tail(2).to_pandas()
     pd_result = scalars_pandas_df["string_col"].tail(2)
 
     assert_series_equal(
         pd_result,
         bf_result,
     )
 
 
 def test_head_then_scalar_operation(scalars_dfs):
     scalars_df, scalars_pandas_df = scalars_dfs
 
-    if scalars_df.index.name is None:
-        pytest.skip("Require explicit index for offset ops.")
-
     bf_result = (scalars_df["float64_col"].head(1) + 4).to_pandas()
     pd_result = scalars_pandas_df["float64_col"].head(1) + 4
 
     pd.testing.assert_series_equal(
         bf_result,
         pd_result,
     )
 
 
 def test_head_then_series_operation(scalars_dfs):
     scalars_df, scalars_pandas_df = scalars_dfs
 
-    if scalars_df.index.name is None:
-        pytest.skip("Require explicit index for offset ops.")
-
     bf_result = (
         scalars_df["float64_col"].head(4) + scalars_df["float64_col"].head(2)
     ).to_pandas()
     pd_result = scalars_pandas_df["float64_col"].head(4) + scalars_pandas_df[
         "float64_col"
     ].head(2)
 
@@ -1838,52 +1894,14 @@
     pd.testing.assert_series_equal(
         bf_result,
         pd_result,
     )
 
 
 @pytest.mark.parametrize(
-    ("na_option",),
-    [
-        ("keep",),
-        ("top",),
-        ("bottom",),
-    ],
-)
-@pytest.mark.parametrize(
-    ("method",),
-    [
-        ("average",),
-        ("min",),
-        ("max",),
-        ("first",),
-        ("dense",),
-    ],
-)
-@pytest.mark.skipif(
-    True, reason="Blocked by possible pandas rank() regression (b/283278923)"
-)
-def test_rank_with_nulls(scalars_df_index, scalars_pandas_df_index, na_option, method):
-    col_name = "bool_col"
-    bf_result = (
-        scalars_df_index[col_name].rank(na_option=na_option, method=method).to_pandas()
-    )
-    pd_result = (
-        scalars_pandas_df_index[col_name]
-        .rank(na_option=na_option, method=method)
-        .astype(pd.Float64Dtype())
-    )
-
-    pd.testing.assert_series_equal(
-        bf_result,
-        pd_result,
-    )
-
-
-@pytest.mark.parametrize(
     ("keep",),
     [
         ("first",),
         ("last",),
         ("all",),
     ],
 )
@@ -3441,17 +3459,16 @@
                 numpy.nan,
             ],
             id="struct_array",
         ),
     ],
 )
 def test_series_explode(data):
-    data = [[1, 2, 3], [], numpy.nan, [3, 4]]
     s = bigframes.pandas.Series(data)
-    pd_s = pd.Series(data)
+    pd_s = s.to_pandas()
     pd.testing.assert_series_equal(
         s.explode().to_pandas(),
         pd_s.explode(),
         check_index_type=False,
         check_dtype=False,
     )
```

### Comparing `bigframes-1.1.0/tests/system/small/test_session.py` & `bigframes-1.2.0/tests/system/small/test_session.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 import typing
 from typing import List
 
 import google
 import google.cloud.bigquery as bigquery
 import numpy as np
 import pandas as pd
+import pyarrow as pa
 import pytest
 
 import bigframes
 import bigframes.core.indexes.base
 import bigframes.dataframe
 import bigframes.dtypes
 import bigframes.ml.linear_model
@@ -432,14 +433,19 @@
 def test_read_pandas_index(session):
     pd_idx = pd.Index([2, 7, 1, 2, 8], dtype=pd.Int64Dtype())
     bf_idx = session.read_pandas(pd_idx)
 
     pd.testing.assert_index_equal(bf_idx.to_pandas(), pd_idx)
 
 
+def test_read_pandas_w_unsupported_mixed_dtype(session):
+    with pytest.raises(pa.ArrowInvalid, match="Could not convert"):
+        session.read_pandas(pd.DataFrame({"a": [1, "hello"]}))
+
+
 def test_read_pandas_inline_respects_location():
     options = bigframes.BigQueryOptions(location="europe-west1")
     session = bigframes.Session(options)
 
     df = session.read_pandas(pd.DataFrame([[1, 2, 3], [4, 5, 6]]))
     repr(df)
 
@@ -489,18 +495,15 @@
 
     pd.testing.assert_frame_equal(result, expected)
 
 
 @utils.skip_legacy_pandas
 def test_read_csv_gcs_default_engine(session, scalars_dfs, gcs_folder):
     scalars_df, _ = scalars_dfs
-    if scalars_df.index.name is not None:
-        path = gcs_folder + "test_read_csv_gcs_default_engine_w_index*.csv"
-    else:
-        path = gcs_folder + "test_read_csv_gcs_default_engine_wo_index*.csv"
+    path = gcs_folder + "test_read_csv_gcs_default_engine_w_index*.csv"
     read_path = utils.get_first_file_from_wildcard(path)
     scalars_df.to_csv(path, index=False)
     dtype = scalars_df.dtypes.to_dict()
     dtype.pop("geography_col")
     df = session.read_csv(
         read_path,
         # Convert default pandas dtypes to match BigQuery DataFrames dtypes.
@@ -516,18 +519,15 @@
     scalars_df = scalars_df.drop(columns=["bytes_col", "numeric_col", "geography_col"])
     assert df.shape[0] == scalars_df.shape[0]
     pd.testing.assert_series_equal(df.dtypes, scalars_df.dtypes)
 
 
 def test_read_csv_gcs_bq_engine(session, scalars_dfs, gcs_folder):
     scalars_df, _ = scalars_dfs
-    if scalars_df.index.name is not None:
-        path = gcs_folder + "test_read_csv_gcs_bq_engine_w_index*.csv"
-    else:
-        path = gcs_folder + "test_read_csv_gcs_bq_engine_wo_index*.csv"
+    path = gcs_folder + "test_read_csv_gcs_bq_engine_w_index*.csv"
     scalars_df.to_csv(path, index=False)
     df = session.read_csv(path, engine="bigquery")
 
     # TODO(chelsealin): If we serialize the index, can more easily compare values.
     pd.testing.assert_index_equal(df.columns, scalars_df.columns)
 
     # The auto detects of BigQuery load job have restrictions to detect the bytes,
```

### Comparing `bigframes-1.1.0/tests/system/small/test_window.py` & `bigframes-1.2.0/tests/system/small/test_window.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/system/utils.py` & `bigframes-1.2.0/tests/system/utils.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/unit/__init__.py` & `bigframes-1.2.0/tests/unit/_config/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/unit/_config/__init__.py` & `bigframes-1.2.0/tests/unit/core/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/unit/_config/test_bigquery_options.py` & `bigframes-1.2.0/tests/unit/_config/test_bigquery_options.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/unit/core/__init__.py` & `bigframes-1.2.0/tests/unit/ml/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/unit/core/test_bf_utils.py` & `bigframes-1.2.0/tests/unit/core/test_bf_utils.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/unit/core/test_blocks.py` & `bigframes-1.2.0/tests/unit/core/test_blocks.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/unit/core/test_expression.py` & `bigframes-1.2.0/tests/unit/core/test_expression.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/unit/core/test_log_adapter.py` & `bigframes-1.2.0/tests/unit/core/test_log_adapter.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/unit/ml/__init__.py` & `bigframes-1.2.0/tests/unit/session/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/unit/ml/test_api_primitives.py` & `bigframes-1.2.0/tests/unit/ml/test_api_primitives.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/unit/ml/test_compose.py` & `bigframes-1.2.0/tests/unit/ml/test_compose.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/unit/ml/test_golden_sql.py` & `bigframes-1.2.0/tests/unit/ml/test_golden_sql.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/unit/ml/test_pipeline.py` & `bigframes-1.2.0/tests/unit/ml/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/unit/ml/test_sql.py` & `bigframes-1.2.0/tests/unit/ml/test_sql.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/unit/resources.py` & `bigframes-1.2.0/tests/unit/resources.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/unit/session/__init__.py` & `bigframes-1.2.0/third_party/bigframes_vendored/google_cloud_bigquery/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/unit/session/test_clients.py` & `bigframes-1.2.0/tests/unit/session/test_clients.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/unit/session/test_io_bigquery.py` & `bigframes-1.2.0/tests/unit/session/test_io_bigquery.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/unit/session/test_io_pandas.py` & `bigframes-1.2.0/tests/unit/session/test_io_pandas.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/unit/session/test_session.py` & `bigframes-1.2.0/tests/unit/session/test_session.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/unit/test_clients.py` & `bigframes-1.2.0/tests/unit/test_clients.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/unit/test_compute_options.py` & `bigframes-1.2.0/tests/unit/test_compute_options.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/unit/test_core.py` & `bigframes-1.2.0/tests/unit/test_core.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/unit/test_dataframe.py` & `bigframes-1.2.0/tests/unit/test_dataframe.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/unit/test_dtypes.py` & `bigframes-1.2.0/tests/unit/test_dtypes.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/unit/test_features.py` & `bigframes-1.2.0/tests/unit/test_features.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/unit/test_formatting_helper.py` & `bigframes-1.2.0/tests/unit/test_formatting_helper.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/unit/test_formatting_helpers.py` & `bigframes-1.2.0/tests/unit/test_formatting_helpers.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/unit/test_pandas.py` & `bigframes-1.2.0/tests/unit/test_pandas.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/tests/unit/test_remote_function.py` & `bigframes-1.2.0/tests/unit/test_remote_function.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/third_party/bigframes_vendored/cpython/LICENSE` & `bigframes-1.2.0/third_party/bigframes_vendored/cpython/LICENSE`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/third_party/bigframes_vendored/cpython/_pprint.py` & `bigframes-1.2.0/third_party/bigframes_vendored/cpython/_pprint.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,14 +106,15 @@
         if k not in init_params:  # happens if k is part of a **kwargs
             return True
         if init_params[k] == inspect._empty:  # k has no default value
             return True
         # try to avoid calling repr on nested estimators
         if isinstance(v, BaseEstimator) and v.__class__ != init_params[k].__class__:
             return True
+
         # Use repr as a last resort. It may be expensive.
         def is_scalar_nan(x):
             return isinstance(x, numbers.Real) and math.isnan(x)
 
         if repr(v) != repr(init_params[k]) and not (
             is_scalar_nan(init_params[k]) and is_scalar_nan(v)
         ):
```

### Comparing `bigframes-1.1.0/third_party/bigframes_vendored/google_cloud_bigquery/LICENSE` & `bigframes-1.2.0/third_party/bigframes_vendored/google_cloud_bigquery/LICENSE`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/third_party/bigframes_vendored/google_cloud_bigquery/__init__.py` & `bigframes-1.2.0/third_party/bigframes_vendored/google_cloud_bigquery/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/third_party/bigframes_vendored/google_cloud_bigquery/_pandas_helpers.py` & `bigframes-1.2.0/third_party/bigframes_vendored/google_cloud_bigquery/_pandas_helpers.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/third_party/bigframes_vendored/google_cloud_bigquery/tests/__init__.py` & `bigframes-1.2.0/third_party/bigframes_vendored/google_cloud_bigquery/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/third_party/bigframes_vendored/google_cloud_bigquery/tests/unit/__init__.py` & `bigframes-1.2.0/bigframes/core/joins/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,7 +7,15 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
+"""Helpers to join ArrayValue objects."""
+
+from bigframes.core.joins.merge import merge
+
+__all__ = [
+    "merge",
+]
```

### Comparing `bigframes-1.1.0/third_party/bigframes_vendored/google_cloud_bigquery/tests/unit/test_pandas_helpers.py` & `bigframes-1.2.0/third_party/bigframes_vendored/google_cloud_bigquery/tests/unit/test_pandas_helpers.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/third_party/bigframes_vendored/ibis/LICENSE.txt` & `bigframes-1.2.0/third_party/bigframes_vendored/ibis/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/third_party/bigframes_vendored/ibis/README.md` & `bigframes-1.2.0/third_party/bigframes_vendored/ibis/README.md`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/third_party/bigframes_vendored/ibis/backends/bigquery/compiler.py` & `bigframes-1.2.0/third_party/bigframes_vendored/ibis/backends/bigquery/compiler.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/third_party/bigframes_vendored/ibis/backends/bigquery/datatypes.py` & `bigframes-1.2.0/third_party/bigframes_vendored/ibis/backends/bigquery/datatypes.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/third_party/bigframes_vendored/ibis/backends/bigquery/registry.py` & `bigframes-1.2.0/third_party/bigframes_vendored/ibis/backends/bigquery/registry.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/third_party/bigframes_vendored/ibis/expr/operations/analytic.py` & `bigframes-1.2.0/third_party/bigframes_vendored/ibis/expr/operations/analytic.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/third_party/bigframes_vendored/ibis/expr/operations/reductions.py` & `bigframes-1.2.0/third_party/bigframes_vendored/ibis/expr/operations/reductions.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/third_party/bigframes_vendored/pandas/AUTHORS.md` & `bigframes-1.2.0/third_party/bigframes_vendored/pandas/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/third_party/bigframes_vendored/pandas/LICENSE` & `bigframes-1.2.0/third_party/bigframes_vendored/pandas/LICENSE`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/third_party/bigframes_vendored/pandas/README.md` & `bigframes-1.2.0/third_party/bigframes_vendored/pandas/README.md`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/third_party/bigframes_vendored/pandas/_config/config.py` & `bigframes-1.2.0/third_party/bigframes_vendored/pandas/_config/config.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/third_party/bigframes_vendored/pandas/core/arrays/arrow/accessors.py` & `bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/arrays/arrow/accessors.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/third_party/bigframes_vendored/pandas/core/arrays/datetimelike.py` & `bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/arrays/datetimelike.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 
 class DatelikeOps:
     def strftime(self, date_format: str):
         """
         Convert to string Series using specified date_format.
 
         Return a Series of formatted strings specified by date_format. Details
-        of the string format can be found in `BigQuery format elements doc
-        <%(https://cloud.google.com/bigquery/docs/reference/standard-sql/format-elements)s>`__.
+        of the string format can be found in BigQuery format elements doc:
+        https://cloud.google.com/bigquery/docs/reference/standard-sql/format-elements#format_elements_date_time.
 
         **Examples:**
 
             >>> import bigframes.pandas as bpd
             >>> bpd.options.display.progress_bar = None
 
             >>> s = bpd.to_datetime(
```

### Comparing `bigframes-1.1.0/third_party/bigframes_vendored/pandas/core/common.py` & `bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/common.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/third_party/bigframes_vendored/pandas/core/computation/align.py` & `bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/computation/align.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/third_party/bigframes_vendored/pandas/core/computation/common.py` & `bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/computation/common.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/third_party/bigframes_vendored/pandas/core/computation/engines.py` & `bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/computation/engines.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/third_party/bigframes_vendored/pandas/core/computation/eval.py` & `bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/computation/eval.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/third_party/bigframes_vendored/pandas/core/computation/expr.py` & `bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/computation/expr.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/third_party/bigframes_vendored/pandas/core/computation/ops.py` & `bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/computation/ops.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/third_party/bigframes_vendored/pandas/core/computation/parsing.py` & `bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/computation/parsing.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/third_party/bigframes_vendored/pandas/core/computation/scope.py` & `bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/computation/scope.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/third_party/bigframes_vendored/pandas/core/config_init.py` & `bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/config_init.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 If you need to make sure options are available even before a certain
 module is imported, register them here rather than in the module.
 
 """
 from __future__ import annotations
 
 display_options_doc = """
-Encapsulates configuration for displaying objects.
+Encapsulates the configuration for displaying objects.
 
 **Examples:**
 
 Define Repr mode to "deferred" will prevent job execution in repr.
     >>> import bigframes.pandas as bpd
     >>> df = bpd.read_gbq("bigquery-public-data.ml_datasets.penguins")
 
@@ -75,15 +75,15 @@
         specified.
     memory_usage (bool):
         This specifies if the memory usage of a DataFrame should be displayed when
         df.info() is called. Valid values True,False,
 """
 
 sampling_options_doc = """
-Encapsulates configuration for data sampling.
+Encapsulates the configuration for data sampling.
 
 Attributes:
     max_download_size (int, default 500):
         Download size threshold in MB. If value set to None, the download size
         won't be checked.
     enable_downsampling (bool, default False):
         Whether to enable downsampling, If max_download_size is exceeded when
```

### Comparing `bigframes-1.1.0/third_party/bigframes_vendored/pandas/core/dtypes/inference.py` & `bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/dtypes/inference.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/third_party/bigframes_vendored/pandas/core/frame.py` & `bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/frame.py`

 * *Files 4% similar despite different names*

```diff
@@ -335,14 +335,15 @@
             ordering_id
             0               1     3
             1               2     4
             <BLANKLINE>
             [2 rows x 2 columns]
 
         Write a DataFrame to a BigQuery table with clustering columns:
+
             >>> df = bpd.DataFrame({'col1': [1, 2], 'col2': [3, 4], 'col3': [5, 6]})
             >>> clustering_cols = ['col1', 'col3']
             >>> df.to_gbq(
             ...             "bigframes-dev.birds.test-clusters",
             ...             if_exists="replace",
             ...             clustering_columns=clustering_cols,
             ...           )
@@ -906,36 +907,14 @@
                 a bytes object is returned.
         """
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
 
     # ----------------------------------------------------------------------
     # Unsorted
 
-    def equals(self, other) -> bool:
-        """
-        Test whether two objects contain the same elements.
-
-        This function allows two Series or DataFrames to be compared against
-        each other to see if they have the same shape and elements. NaNs in
-        the same location are considered equal.
-
-        The row/column index do not need to have the same type, as long
-        as the values are considered equal. Corresponding columns must be of
-        the same dtype.
-
-        Args:
-            other (Series or DataFrame):
-                The other Series or DataFrame to be compared with the first.
-
-        Returns:
-            bool: True if all elements are the same in both objects, False
-            otherwise.
-        """
-        raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
-
     def assign(self, **kwargs) -> DataFrame:
         r"""
         Assign new columns to a DataFrame.
 
         Returns a new object with all original columns in addition to new ones.
         Existing columns that are re-assigned will be overwritten.
 
@@ -1204,15 +1183,14 @@
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
 
     def rename_axis(self, mapper: Optional[str], **kwargs) -> DataFrame:
         """
         Set the name of the axis for the index.
 
         .. note::
-
             Currently only accepts a single string parameter (the new name of the index).
 
         Args:
             mapper str:
                 Value to set the axis name attribute.
 
         Returns:
@@ -1858,15 +1836,15 @@
 
         Returns:
             DataFrame: The original DataFrame sorted by the labels.
         """
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
 
     # ----------------------------------------------------------------------
-    # Arithmetic Methods
+    # Arithmetic and Logical Methods
 
     def eq(self, other, axis: str | int = "columns") -> DataFrame:
         """
         Get equal to of DataFrame and other, element-wise (binary operator `eq`).
 
         Among flexible wrappers (`eq`, `ne`, `le`, `lt`, `ge`, `gt`) to comparison
         operators.
@@ -1886,15 +1864,16 @@
             ...       index=['circle', 'triangle', 'rectangle'])
             >>> df["degrees"].eq(360)
             circle        True
             triangle     False
             rectangle     True
             Name: degrees, dtype: boolean
 
-        You can also use arithmetic operator ``==``:
+        You can also use logical operator `==`:
+
             >>> df["degrees"] == 360
             circle        True
             triangle     False
             rectangle     True
             Name: degrees, dtype: boolean
 
         Args:
@@ -1905,14 +1884,47 @@
                 (1 or 'columns').
 
         Returns:
             DataFrame: Result of the comparison.
         """
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
 
+    def __eq__(self, other):
+        """
+        Check equality of DataFrame and other, element-wise, using logical
+        operator `==`.
+
+        Equivalent to `DataFrame.eq(other)`.
+
+        **Examples:**
+
+            >>> import bigframes.pandas as bpd
+            >>> bpd.options.display.progress_bar = None
+
+            >>> df = bpd.DataFrame({
+            ...         'a': [0, 3, 4],
+            ...         'b': [360, 0, 180]
+            ...      })
+            >>> df == 0
+                   a      b
+            0   True  False
+            1  False   True
+            2  False  False
+            <BLANKLINE>
+            [3 rows x 2 columns]
+
+        Args:
+            other (scalar or DataFrame):
+                Object to be compared to the DataFrame for equality.
+
+        Returns:
+            DataFrame: The result of comparing `other` to DataFrame.
+        """
+        raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
+
     def ne(self, other, axis: str | int = "columns") -> DataFrame:
         """
         Get not equal to of DataFrame and other, element-wise (binary operator `ne`).
 
         Among flexible wrappers (`eq`, `ne`, `le`, `lt`, `ge`, `gt`) to comparison
         operators.
 
@@ -1950,14 +1962,47 @@
                 Whether to compare by the index (0 or 'index') or columns
                 (1 or 'columns').
         Returns:
             DataFrame: Result of the comparison.
         """
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
 
+    def __ne__(self, other):
+        """
+        Check inequality of DataFrame and other, element-wise, using logical
+        operator `!=`.
+
+        Equivalent to `DataFrame.ne(other)`.
+
+        **Examples:**
+
+            >>> import bigframes.pandas as bpd
+            >>> bpd.options.display.progress_bar = None
+
+            >>> df = bpd.DataFrame({
+            ...         'a': [0, 3, 4],
+            ...         'b': [360, 0, 180]
+            ...      })
+            >>> df != 0
+                   a      b
+            0  False   True
+            1   True  False
+            2   True   True
+            <BLANKLINE>
+            [3 rows x 2 columns]
+
+        Args:
+            other (scalar or DataFrame):
+                Object to be compared to the DataFrame for inequality.
+
+        Returns:
+            DataFrame: The result of comparing `other` to DataFrame.
+        """
+        raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
+
     def le(self, other, axis: str | int = "columns") -> DataFrame:
         """Get 'less than or equal to' of dataframe and other, element-wise (binary operator `<=`).
 
         Among flexible wrappers (`eq`, `ne`, `le`, `lt`, `ge`, `gt`) to comparison
         operators.
 
         Equivalent to `==`, `!=`, `<=`, `<`, `>=`, `>` with support to choose axis
@@ -2000,14 +2045,47 @@
                 (1 or 'columns').
 
         Returns:
             DataFrame: DataFrame of bool. The result of the comparison.
         """
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
 
+    def __le__(self, other):
+        """
+        Check whether DataFrame is less than or equal to other, element-wise,
+        using logical operator `<=`.
+
+        Equivalent to `DataFrame.le(other)`.
+
+        **Examples:**
+
+            >>> import bigframes.pandas as bpd
+            >>> bpd.options.display.progress_bar = None
+
+            >>> df = bpd.DataFrame({
+            ...         'a': [0, -1, 1],
+            ...         'b': [1, 0, -1]
+            ...      })
+            >>> df <= 0
+                   a      b
+            0   True  False
+            1   True   True
+            2  False   True
+            <BLANKLINE>
+            [3 rows x 2 columns]
+
+        Args:
+            other (scalar or DataFrame):
+                Object to be compared to the DataFrame.
+
+        Returns:
+            DataFrame: The result of comparing `other` to DataFrame.
+        """
+        raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
+
     def lt(self, other, axis: str | int = "columns") -> DataFrame:
         """Get 'less than' of DataFrame and other, element-wise (binary operator `<`).
 
         Among flexible wrappers (`eq`, `ne`, `le`, `lt`, `ge`, `gt`) to comparison
         operators.
 
         Equivalent to `==`, `!=`, `<=`, `<`, `>=`, `>` with support to choose axis
@@ -2050,14 +2128,47 @@
                 (1 or 'columns').
 
         Returns:
             DataFrame: DataFrame of bool. The result of the comparison.
         """
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
 
+    def __lt__(self, other):
+        """
+        Check whether DataFrame is less than other, element-wise, using logical
+        operator `<`.
+
+        Equivalent to `DataFrame.lt(other)`.
+
+        **Examples:**
+
+            >>> import bigframes.pandas as bpd
+            >>> bpd.options.display.progress_bar = None
+
+            >>> df = bpd.DataFrame({
+            ...         'a': [0, -1, 1],
+            ...         'b': [1, 0, -1]
+            ...      })
+            >>> df < 0
+                   a      b
+            0  False  False
+            1   True  False
+            2  False   True
+            <BLANKLINE>
+            [3 rows x 2 columns]
+
+        Args:
+            other (scalar or DataFrame):
+                Object to be compared to the DataFrame.
+
+        Returns:
+            DataFrame: The result of comparing `other` to DataFrame.
+        """
+        raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
+
     def ge(self, other, axis: str | int = "columns") -> DataFrame:
         """Get 'greater than or equal to' of DataFrame and other, element-wise (binary operator `>=`).
 
         Among flexible wrappers (`eq`, `ne`, `le`, `lt`, `ge`, `gt`) to comparison
         operators.
 
         Equivalent to `==`, `!=`, `<=`, `<`, `>=`, `>` with support to choose axis
@@ -2100,14 +2211,47 @@
                 (1 or 'columns').
 
         Returns:
             DataFrame: DataFrame of bool. The result of the comparison.
         """
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
 
+    def __ge__(self, other):
+        """
+        Check whether DataFrame is greater than or equal to other, element-wise,
+        using logical operator `>=`.
+
+        Equivalent to `DataFrame.ge(other)`.
+
+        **Examples:**
+
+            >>> import bigframes.pandas as bpd
+            >>> bpd.options.display.progress_bar = None
+
+            >>> df = bpd.DataFrame({
+            ...         'a': [0, -1, 1],
+            ...         'b': [1, 0, -1]
+            ...      })
+            >>> df >= 0
+                   a      b
+            0   True   True
+            1  False   True
+            2   True  False
+            <BLANKLINE>
+            [3 rows x 2 columns]
+
+        Args:
+            other (scalar or DataFrame):
+                Object to be compared to the DataFrame.
+
+        Returns:
+            DataFrame: The result of comparing `other` to DataFrame.
+        """
+        raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
+
     def gt(self, other, axis: str | int = "columns") -> DataFrame:
         """Get 'greater than' of DataFrame and other, element-wise (binary operator `>`).
 
         Among flexible wrappers (`eq`, `ne`, `le`, `lt`, `ge`, `gt`) to comparison
         operators.
 
         Equivalent to `==`, `!=`, `<=`, `<`, `>=`, `>` with support to choose axis
@@ -2148,14 +2292,47 @@
                 (1 or 'columns').
 
         Returns:
             DataFrame: DataFrame of bool: The result of the comparison.
         """
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
 
+    def __gt__(self, other):
+        """
+        Check whether DataFrame is greater than other, element-wise, using logical
+        operator `>`.
+
+        Equivalent to `DataFrame.gt(other)`.
+
+        **Examples:**
+
+            >>> import bigframes.pandas as bpd
+            >>> bpd.options.display.progress_bar = None
+
+            >>> df = bpd.DataFrame({
+            ...         'a': [0, -1, 1],
+            ...         'b': [1, 0, -1]
+            ...      })
+            >>> df > 0
+                   a      b
+            0  False   True
+            1  False  False
+            2   True  False
+            <BLANKLINE>
+            [3 rows x 2 columns]
+
+        Args:
+            other (scalar or DataFrame):
+                Object to be compared to the DataFrame.
+
+        Returns:
+            DataFrame: The result of comparing `other` to DataFrame.
+        """
+        raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
+
     def add(self, other, axis: str | int = "columns") -> DataFrame:
         """Get addition of DataFrame and other, element-wise (binary operator `+`).
 
         Equivalent to ``dataframe + other``. With reverse version, `radd`.
 
         Among flexible wrappers (`add`, `sub`, `mul`, `div`, `mod`, `pow`) to
         arithmetic operators: `+`, `-`, `*`, `/`, `//`, `%`, `**`.
@@ -2179,15 +2356,134 @@
             0    5
             1    7
             2    9
             dtype: Int64
 
         You can also use arithmetic operator ``+``:
 
-            >>> df['A'] + (df['B'])
+            >>> df['A'] + df['B']
+            0    5
+            1    7
+            2    9
+            dtype: Int64
+
+        Args:
+            other (float, int, or Series):
+                Any single or multiple element data structure, or list-like object.
+            axis ({0 or 'index', 1 or 'columns'}):
+                Whether to compare by the index (0 or 'index') or columns.
+                (1 or 'columns'). For Series input, axis to match Series index on.
+
+        Returns:
+            DataFrame: DataFrame result of the arithmetic operation.
+        """
+        raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
+
+    def __add__(self, other) -> DataFrame:
+        """Get addition of DataFrame and other, column-wise, using arithmatic
+        operator `+`.
+
+        Equivalent to ``DataFrame.add(other)``.
+
+        **Examples:**
+
+            >>> import bigframes.pandas as bpd
+            >>> bpd.options.display.progress_bar = None
+
+            >>> df = bpd.DataFrame({
+            ...         'height': [1.5, 2.6],
+            ...         'weight': [500, 800]
+            ...     },
+            ...     index=['elk', 'moose'])
+            >>> df
+                   height  weight
+            elk       1.5     500
+            moose     2.6     800
+            <BLANKLINE>
+            [2 rows x 2 columns]
+
+        Adding a scalar affects all rows and columns.
+
+            >>> df + 1.5
+                   height  weight
+            elk       3.0   501.5
+            moose     4.1   801.5
+            <BLANKLINE>
+            [2 rows x 2 columns]
+
+        You can add another DataFrame with index and columns aligned.
+
+            >>> delta = bpd.DataFrame({
+            ...         'height': [0.5, 0.9],
+            ...         'weight': [50, 80]
+            ...     },
+            ...     index=['elk', 'moose'])
+            >>> df + delta
+                   height  weight
+            elk       2.0     550
+            moose     3.5     880
+            <BLANKLINE>
+            [2 rows x 2 columns]
+
+        Adding any mis-aligned index and columns will result in invalid values.
+
+            >>> delta = bpd.DataFrame({
+            ...         'depth': [0.5, 0.9, 1.0],
+            ...         'weight': [50, 80, 100]
+            ...     },
+            ...     index=['elk', 'moose', 'bison'])
+            >>> df + delta
+                   depth  height  weight
+            elk     <NA>    <NA>     550
+            moose   <NA>    <NA>     880
+            bison   <NA>    <NA>    <NA>
+            <BLANKLINE>
+            [3 rows x 3 columns]
+
+        Args:
+            other (scalar or DataFrame):
+                Object to be added to the DataFrame.
+
+        Returns:
+            DataFrame: The result of adding `other` to DataFrame.
+        """
+        raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
+
+    def radd(self, other, axis: str | int = "columns") -> DataFrame:
+        """Get addition of DataFrame and other, element-wise (binary operator `+`).
+
+        Equivalent to ``other + dataframe``. With reverse version, `add`.
+
+        Among flexible wrappers (`add`, `sub`, `mul`, `div`, `mod`, `pow`) to
+        arithmetic operators: `+`, `-`, `*`, `/`, `//`, `%`, `**`.
+
+        .. note::
+            Mismatched indices will be unioned together.
+
+        **Examples:**
+
+            >>> import bigframes.pandas as bpd
+            >>> bpd.options.display.progress_bar = None
+
+            >>> df = bpd.DataFrame({
+            ...     'A': [1, 2, 3],
+            ...     'B': [4, 5, 6],
+            ...     })
+
+        You can use method name:
+
+            >>> df['A'].radd(df['B'])
+            0    5
+            1    7
+            2    9
+            dtype: Int64
+
+        You can also use arithmetic operator ``+``:
+
+            >>> df['A'] + df['B']
             0    5
             1    7
             2    9
             dtype: Int64
 
         Args:
             other (float, int, or Series):
@@ -2246,14 +2542,57 @@
                 (1 or 'columns'). For Series input, axis to match Series index on.
 
         Returns:
             DataFrame: DataFrame result of the arithmetic operation.
         """
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
 
+    def __sub__(self, other):
+        """
+        Get subtraction of other from DataFrame, element-wise, using operator `-`.
+
+        Equivalent to `DataFrame.sub(other)`.
+
+        **Examples:**
+
+            >>> import bigframes.pandas as bpd
+            >>> bpd.options.display.progress_bar = None
+
+        You can subtract a scalar:
+
+            >>> df = bpd.DataFrame({"a": [1, 2, 3], "b": [4, 5, 6]})
+            >>> df - 2
+                a  b
+            0  -1  2
+            1   0  3
+            2   1  4
+            <BLANKLINE>
+            [3 rows x 2 columns]
+
+        You can also subtract another DataFrame with index and column labels
+        aligned:
+
+            >>> df1 = bpd.DataFrame({"a": [2, 2, 2], "b": [3, 3, 3]})
+            >>> df - df1
+                a  b
+            0  -1  1
+            1   0  2
+            2   1  3
+            <BLANKLINE>
+            [3 rows x 2 columns]
+
+        Args:
+            other (scalar or DataFrame):
+                Object to subtract from the DataFrame.
+
+        Returns:
+            DataFrame: The result of the subtraction.
+        """
+        raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
+
     def rsub(self, other, axis: str | int = "columns") -> DataFrame:
         """Get subtraction of DataFrame and other, element-wise (binary operator `-`).
 
         Equivalent to ``other - dataframe``. With reverse version, `sub`.
 
         Among flexible wrappers (`add`, `sub`, `mul`, `div`, `mod`, `pow`) to
         arithmetic operators: `+`, `-`, `*`, `/`, `//`, `%`, `**`.
@@ -2292,14 +2631,29 @@
                 (1 or 'columns'). For Series input, axis to match Series index on.
 
         Returns:
             DataFrame: DataFrame result of the arithmetic operation.
         """
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
 
+    def __rsub__(self, other):
+        """
+        Get subtraction of DataFrame from other, element-wise, using operator `-`.
+
+        Equivalent to `DataFrame.rsub(other)`.
+
+        Args:
+            other (scalar or DataFrame):
+                Object to subtract the DataFrame from.
+
+        Returns:
+            DataFrame: The result of the subtraction.
+        """
+        raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
+
     def mul(self, other, axis: str | int = "columns") -> DataFrame:
         """Get multiplication of DataFrame and other, element-wise (binary operator `*`).
 
         Equivalent to ``dataframe * other``. With reverse version, `rmul`.
 
         Among flexible wrappers (`add`, `sub`, `mul`, `div`, `mod`, `pow`) to
         arithmetic operators: `+`, `-`, `*`, `/`, `//`, `%`, `**`.
@@ -2341,14 +2695,149 @@
                 (1 or 'columns'). For Series input, axis to match Series index on.
 
         Returns:
             DataFrame: DataFrame result of the arithmetic operation.
         """
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
 
+    def __mul__(self, other):
+        """
+        Get multiplication of DataFrame with other, element-wise, using operator `*`.
+
+        Equivalent to `DataFrame.mul(other)`.
+
+        **Examples:**
+
+            >>> import bigframes.pandas as bpd
+            >>> bpd.options.display.progress_bar = None
+
+        You can multiply with a scalar:
+
+            >>> df = bpd.DataFrame({"a": [1, 2, 3], "b": [4, 5, 6]})
+            >>> df * 3
+               a   b
+            0  3  12
+            1  6  15
+            2  9  18
+            <BLANKLINE>
+            [3 rows x 2 columns]
+
+        You can also multiply with another DataFrame with index and column labels
+        aligned:
+
+            >>> df1 = bpd.DataFrame({"a": [2, 2, 2], "b": [3, 3, 3]})
+            >>> df * df1
+               a   b
+            0  2  12
+            1  4  15
+            2  6  18
+            <BLANKLINE>
+            [3 rows x 2 columns]
+
+        Args:
+            other (scalar or DataFrame):
+                Object to multiply with the DataFrame.
+
+        Returns:
+            DataFrame: The result of the multiplication.
+        """
+        raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
+
+    def rmul(self, other, axis: str | int = "columns") -> DataFrame:
+        """Get multiplication of DataFrame and other, element-wise (binary operator `*`).
+
+        Equivalent to ``other * dataframe``. With reverse version, `mul`.
+
+        Among flexible wrappers (`add`, `sub`, `mul`, `div`, `mod`, `pow`) to
+        arithmetic operators: `+`, `-`, `*`, `/`, `//`, `%`, `**`.
+
+        .. note::
+            Mismatched indices will be unioned together.
+
+        **Examples:**
+
+            >>> import bigframes.pandas as bpd
+            >>> bpd.options.display.progress_bar = None
+
+            >>> df = bpd.DataFrame({
+            ...     'A': [1, 2, 3],
+            ...     'B': [4, 5, 6],
+            ...     })
+
+        You can use method name:
+
+            >>> df['A'].rmul(df['B'])
+            0     4
+            1    10
+            2    18
+            dtype: Int64
+
+        You can also use arithmetic operator ``*``:
+
+            >>> df['A'] * (df['B'])
+            0     4
+            1    10
+            2    18
+            dtype: Int64
+
+        Args:
+            other (float, int, or Series):
+                Any single or multiple element data structure, or list-like object.
+            axis ({0 or 'index', 1 or 'columns'}):
+                Whether to compare by the index (0 or 'index') or columns.
+                (1 or 'columns'). For Series input, axis to match Series index on.
+
+        Returns:
+            DataFrame: DataFrame result of the arithmetic operation.
+        """
+        raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
+
+    def __rmul__(self, other):
+        """
+        Get multiplication of DataFrame with other, element-wise, using operator `*`.
+
+        Equivalent to `DataFrame.rmul(other)`.
+
+        **Examples:**
+
+            >>> import bigframes.pandas as bpd
+            >>> bpd.options.display.progress_bar = None
+
+        You can multiply with a scalar:
+
+            >>> df = bpd.DataFrame({"a": [1, 2, 3], "b": [4, 5, 6]})
+            >>> df * 3
+               a   b
+            0  3  12
+            1  6  15
+            2  9  18
+            <BLANKLINE>
+            [3 rows x 2 columns]
+
+        You can also multiply with another DataFrame with index and column labels
+        aligned:
+
+            >>> df1 = bpd.DataFrame({"a": [2, 2, 2], "b": [3, 3, 3]})
+            >>> df * df1
+               a   b
+            0  2  12
+            1  4  15
+            2  6  18
+            <BLANKLINE>
+            [3 rows x 2 columns]
+
+        Args:
+            other (scalar or DataFrame):
+                Object to multiply the DataFrame with.
+
+        Returns:
+            DataFrame: The result of the multiplication.
+        """
+        raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
+
     def truediv(self, other, axis: str | int = "columns") -> DataFrame:
         """Get floating division of DataFrame and other, element-wise (binary operator `/`).
 
         Equivalent to ``dataframe / other``. With reverse version, `rtruediv`.
 
         Among flexible wrappers (`add`, `sub`, `mul`, `div`, `mod`, `pow`) to
         arithmetic operators: `+`, `-`, `*`, `/`, `//`, `%`, `**`.
@@ -2390,14 +2879,57 @@
                 (1 or 'columns'). For Series input, axis to match Series index on.
 
         Returns:
             DataFrame: DataFrame result of the arithmetic operation.
         """
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
 
+    def __truediv__(self, other):
+        """
+        Get division of DataFrame by other, element-wise, using operator `/`.
+
+        Equivalent to `DataFrame.truediv(other)`.
+
+        **Examples:**
+
+            >>> import bigframes.pandas as bpd
+            >>> bpd.options.display.progress_bar = None
+
+        You can multiply with a scalar:
+
+            >>> df = bpd.DataFrame({"a": [1, 2, 3], "b": [4, 5, 6]})
+            >>> df / 2
+                 a    b
+            0  0.5  2.0
+            1  1.0  2.5
+            2  1.5  3.0
+            <BLANKLINE>
+            [3 rows x 2 columns]
+
+        You can also multiply with another DataFrame with index and column labels
+        aligned:
+
+            >>> denominator = bpd.DataFrame({"a": [2, 2, 2], "b": [3, 3, 3]})
+            >>> df / denominator
+                a         b
+            0  0.5  1.333333
+            1  1.0  1.666667
+            2  1.5       2.0
+            <BLANKLINE>
+            [3 rows x 2 columns]
+
+        Args:
+            other (scalar or DataFrame):
+                Object to divide the DataFrame by.
+
+        Returns:
+            DataFrame: The result of the division.
+        """
+        raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
+
     def rtruediv(self, other, axis: str | int = "columns") -> DataFrame:
         """Get floating division of DataFrame and other, element-wise (binary operator `/`).
 
         Equivalent to ``other / dataframe``. With reverse version, `truediv`.
 
         Among flexible wrappers (`add`, `sub`, `mul`, `div`, `mod`, `pow`) to
         arithmetic operators: `+`, `-`, `*`, `/`, `//`, `%`, `**`.
@@ -2436,14 +2968,29 @@
                 (1 or 'columns'). For Series input, axis to match Series index on.
 
         Returns:
             DataFrame: DataFrame result of the arithmetic operation.
         """
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
 
+    def __rtruediv__(self, other):
+        """
+        Get division of other by DataFrame, element-wise, using operator `/`.
+
+        Equivalent to `DataFrame.rtruediv(other)`.
+
+        Args:
+            other (scalar or DataFrame):
+                Object to divide by the DataFrame.
+
+        Returns:
+            DataFrame: The result of the division.
+        """
+        raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
+
     def floordiv(self, other, axis: str | int = "columns") -> DataFrame:
         """Get integer division of DataFrame and other, element-wise (binary operator `//`).
 
         Equivalent to ``dataframe // other``. With reverse version, `rfloordiv`.
 
         Among flexible wrappers (`add`, `sub`, `mul`, `div`, `mod`, `pow`) to
         arithmetic operators: `+`, `-`, `*`, `/`, `//`, `%`, `**`.
@@ -2485,14 +3032,57 @@
                 (1 or 'columns'). For Series input, axis to match Series index on.
 
         Returns:
             DataFrame: DataFrame result of the arithmetic operation.
         """
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
 
+    def __floordiv__(self, other):
+        """
+        Get integer divison of DataFrame by other, using arithmatic operator `//`.
+
+        Equivalent to `DataFrame.floordiv(other)`.
+
+        **Examples:**
+
+            >>> import bigframes.pandas as bpd
+            >>> bpd.options.display.progress_bar = None
+
+        You can divide by a scalar:
+
+            >>> df = bpd.DataFrame({"a": [15, 15, 15], "b": [30, 30, 30]})
+            >>> df // 2
+               a   b
+            0  7  15
+            1  7  15
+            2  7  15
+            <BLANKLINE>
+            [3 rows x 2 columns]
+
+        You can also divide by another DataFrame with index and column labels
+        aligned:
+
+            >>> divisor = bpd.DataFrame({"a": [2, 3, 4], "b": [5, 6, 7]})
+            >>> df // divisor
+               a  b
+            0  7  6
+            1  5  5
+            2  3  4
+            <BLANKLINE>
+            [3 rows x 2 columns]
+
+        Args:
+            other (scalar or DataFrame):
+                Object to divide the DataFrame by.
+
+        Returns:
+            DataFrame: The result of the integer divison.
+        """
+        raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
+
     def rfloordiv(self, other, axis: str | int = "columns") -> DataFrame:
         """Get integer division of DataFrame and other, element-wise (binary operator `//`).
 
         Equivalent to ``other // dataframe``. With reverse version, `rfloordiv`.
 
         Among flexible wrappers (`add`, `sub`, `mul`, `div`, `mod`, `pow`) to
         arithmetic operators: `+`, `-`, `*`, `/`, `//`, `%`, `**`.
@@ -2531,14 +3121,29 @@
                 (1 or 'columns'). For Series input, axis to match Series index on.
 
         Returns:
             DataFrame: DataFrame result of the arithmetic operation.
         """
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
 
+    def __rfloordiv__(self, other):
+        """
+        Get integer divison of other by DataFrame.
+
+        Equivalent to `DataFrame.rfloordiv(other)`.
+
+        Args:
+            other (scalar or DataFrame):
+                Object to divide by the DataFrame.
+
+        Returns:
+            DataFrame: The result of the integer divison.
+        """
+        raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
+
     def mod(self, other, axis: str | int = "columns") -> DataFrame:
         """Get modulo of DataFrame and other, element-wise (binary operator `%`).
 
         Equivalent to ``dataframe % other``. With reverse version, `rmod`.
 
         Among flexible wrappers (`add`, `sub`, `mul`, `div`, `mod`, `pow`) to
         arithmetic operators: `+`, `-`, `*`, `/`, `//`, `%`, `**`.
@@ -2580,14 +3185,57 @@
                 (1 or 'columns'). For Series input, axis to match Series index on.
 
         Returns:
             DataFrame: DataFrame result of the arithmetic operation.
         """
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
 
+    def __mod__(self, other):
+        """
+        Get modulo of DataFrame with other, element-wise, using operator `%`.
+
+        Equivalent to `DataFrame.mod(other)`.
+
+        **Examples:**
+
+            >>> import bigframes.pandas as bpd
+            >>> bpd.options.display.progress_bar = None
+
+        You can modulo with a scalar:
+
+            >>> df = bpd.DataFrame({"a": [1, 2, 3], "b": [4, 5, 6]})
+            >>> df % 3
+               a  b
+            0  1  1
+            1  2  2
+            2  0  0
+            <BLANKLINE>
+            [3 rows x 2 columns]
+
+        You can also modulo with another DataFrame with index and column labels
+        aligned:
+
+            >>> modulo = bpd.DataFrame({"a": [2, 2, 2], "b": [3, 3, 3]})
+            >>> df % modulo
+               a  b
+            0  1  1
+            1  0  2
+            2  1  0
+            <BLANKLINE>
+            [3 rows x 2 columns]
+
+        Args:
+            other (scalar or DataFrame):
+                Object to modulo the DataFrame by.
+
+        Returns:
+            DataFrame: The result of the modulo.
+        """
+        raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
+
     def rmod(self, other, axis: str | int = "columns") -> DataFrame:
         """Get modulo of DataFrame and other, element-wise (binary operator `%`).
 
         Equivalent to ``other % dataframe``. With reverse version, `mod`.
 
         Among flexible wrappers (`add`, `sub`, `mul`, `div`, `mod`, `pow`) to
         arithmetic operators: `+`, `-`, `*`, `/`, `//`, `%`, `**`.
@@ -2626,14 +3274,29 @@
                 (1 or 'columns'). For Series input, axis to match Series index on.
 
         Returns:
             DataFrame: DataFrame result of the arithmetic operation.
         """
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
 
+    def __rmod__(self, other):
+        """
+        Get integer divison of other by DataFrame.
+
+        Equivalent to `DataFrame.rmod(other)`.
+
+        Args:
+            other (scalar or DataFrame):
+                Object to modulo by the DataFrame.
+
+        Returns:
+            DataFrame: The result of the modulo.
+        """
+        raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
+
     def pow(self, other, axis: str | int = "columns") -> DataFrame:
         """Get Exponential power of dataframe and other, element-wise (binary operator `**`).
 
         Equivalent to ``dataframe ** other``, but with support to substitute a fill_value
         for missing data in one of the inputs. With reverse version, `rpow`.
 
         Among flexible wrappers (`add`, `sub`, `mul`, `div`, `mod`, `pow`) to
@@ -2676,14 +3339,58 @@
                 (1 or 'columns'). For Series input, axis to match Series index on.
 
         Returns:
             DataFrame: DataFrame result of the arithmetic operation.
         """
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
 
+    def __pow__(self, other):
+        """
+        Get exponentiation of DataFrame with other, element-wise, using operator
+        `**`.
+
+        Equivalent to `DataFrame.pow(other)`.
+
+        **Examples:**
+
+            >>> import bigframes.pandas as bpd
+            >>> bpd.options.display.progress_bar = None
+
+        You can exponentiate with a scalar:
+
+            >>> df = bpd.DataFrame({"a": [1, 2, 3], "b": [4, 5, 6]})
+            >>> df ** 2
+               a   b
+            0  1  16
+            1  4  25
+            2  9  36
+            <BLANKLINE>
+            [3 rows x 2 columns]
+
+        You can also exponentiate with another DataFrame with index and column
+        labels aligned:
+
+            >>> exponent = bpd.DataFrame({"a": [2, 2, 2], "b": [3, 3, 3]})
+            >>> df ** exponent
+               a    b
+            0  1   64
+            1  4  125
+            2  9  216
+            <BLANKLINE>
+            [3 rows x 2 columns]
+
+        Args:
+            other (scalar or DataFrame):
+                Object to exponentiate the DataFrame with.
+
+        Returns:
+            DataFrame: The result of the exponentiation.
+        """
+        raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
+
     def rpow(self, other, axis: str | int = "columns") -> DataFrame:
         """Get Exponential power of dataframe and other, element-wise (binary operator `rpow`).
 
         Equivalent to ``other ** dataframe``, but with support to substitute a fill_value
         for missing data in one of the inputs. With reverse version, `pow`.
 
         Among flexible wrappers (`add`, `sub`, `mul`, `div`, `mod`, `pow`) to
@@ -2723,14 +3430,30 @@
                 (1 or 'columns'). For Series input, axis to match Series index on.
 
         Returns:
             DataFrame: DataFrame result of the arithmetic operation.
         """
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
 
+    def __rpow__(self, other):
+        """
+        Get exponentiation of other with DataFrame, element-wise, using operator
+        `**`.
+
+        Equivalent to `DataFrame.rpow(other)`.
+
+        Args:
+            other (scalar or DataFrame):
+                Object to exponentiate with the DataFrame.
+
+        Returns:
+            DataFrame: The result of the exponentiation.
+        """
+        raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
+
     def combine(
         self, other, func, fill_value=None, overwrite: bool = True
     ) -> DataFrame:
         """Perform column-wise combine with another DataFrame.
 
         Combines a DataFrame with `other` DataFrame using `func`
         to element-wise combine columns. The row and column indexes of the
@@ -4098,15 +4821,14 @@
         well, but not used for ordering.
 
         This method is equivalent to
         ``df.sort_values(columns, ascending=True).head(n)``, but more
         performant.
 
         .. note::
-
             This function cannot be used with all column types. For example, when
             specifying columns with `object` or `category` dtypes, ``TypeError`` is
             raised.
 
         **Examples:**
 
             >>> import bigframes.pandas as bpd
@@ -4707,14 +5429,96 @@
                 have hierarchically indexed columns.
 
         Returns:
             DataFrame: Returns reshaped DataFrame.
         """
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
 
+    def pivot_table(self, values=None, index=None, columns=None, aggfunc="mean"):
+        """
+        Create a spreadsheet-style pivot table as a DataFrame.
+
+        The levels in the pivot table will be stored in MultiIndex objects (hierarchical indexes)
+        on the index and columns of the result DataFrame.
+
+        **Examples:**
+
+            >>> import bigframes.pandas as bpd
+            >>> bpd.options.display.progress_bar = None
+
+            >>> df = bpd.DataFrame({
+            ...     'Product': ['Product A', 'Product B', 'Product A', 'Product B', 'Product A', 'Product B'],
+            ...     'Region': ['East', 'West', 'East', 'West', 'West', 'East'],
+            ...     'Sales': [100, 200, 150, 100, 200, 150],
+            ...     'Rating': [3, 5, 4, 3, 3, 5]
+            ... })
+            >>> df
+                 Product Region  Sales  Rating
+            0  Product A   East    100       3
+            1  Product B   West    200       5
+            2  Product A   East    150       4
+            3  Product B   West    100       3
+            4  Product A   West    200       3
+            5  Product B   East    150       5
+            <BLANKLINE>
+            [6 rows x 4 columns]
+
+        Using `pivot_table` with default aggfunc "mean":
+
+            >>> pivot_table = df.pivot_table(
+            ...     values=['Sales', 'Rating'],
+            ...     index='Product',
+            ...     columns='Region'
+            ... )
+            >>> pivot_table
+                      Rating       Sales
+            Region      East West   East   West
+            Product
+            Product A    3.5  3.0  125.0  200.0
+            Product B    5.0  4.0  150.0  150.0
+            <BLANKLINE>
+            [2 rows x 4 columns]
+
+        Using `pivot_table` with specified aggfunc "max":
+
+            >>> pivot_table = df.pivot_table(
+            ...     values=['Sales', 'Rating'],
+            ...     index='Product',
+            ...     columns='Region',
+            ...     aggfunc="max"
+            ... )
+            >>> pivot_table
+                      Rating      Sales
+            Region      East West  East West
+            Product
+            Product A      4    3   150  200
+            Product B      5    5   150  200
+            <BLANKLINE>
+            [2 rows x 4 columns]
+
+        Args:
+            values (str, object or a list of the previous, optional):
+                Column(s) to use for populating new frame's values. If not
+                specified, all remaining columns will be used and the result will
+                have hierarchically indexed columns.
+
+            index (str or object or a list of str, optional):
+                Column to use to make new frame's index. If not given, uses existing index.
+
+            columns (str or object or a list of str):
+                Column to use to make new frame's columns.
+
+            aggfunc (str, default "mean"):
+                Aggregation function name to compute summary statistics (e.g., 'sum', 'mean').
+
+        Returns:
+            DataFrame: An Excel style pivot table.
+        """
+        raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
+
     def stack(self, level=-1):
         """
         Stack the prescribed level(s) from columns to index.
 
         Return a reshaped DataFrame or Series having a multi-level
         index with one or more new inner-most levels compared to the current
         DataFrame. The new inner-most levels are created by pivoting the
@@ -4988,14 +5792,15 @@
         Evaluate a string describing operations on DataFrame columns.
 
         Operates on columns only, not specific rows or elements.  This allows
         `eval` to run arbitrary code, which can make you vulnerable to code
         injection if you pass user input to this function.
 
         **Examples:**
+
             >>> import bigframes.pandas as bpd
             >>> bpd.options.display.progress_bar = None
 
             >>> df = bpd.DataFrame({'A': range(1, 6), 'B': range(10, 0, -2)})
             >>> df
             A   B
             0  1  10
@@ -5009,45 +5814,45 @@
             0    11
             1    10
             2     9
             3     8
             4     7
             dtype: Int64
 
-            Assignment is allowed though by default the original DataFrame is not
-            modified.
+        Assignment is allowed though by default the original DataFrame is not
+        modified.
 
             >>> df.eval('C = A + B')
-            A   B   C
+               A   B   C
             0  1  10  11
             1  2   8  10
             2  3   6   9
             3  4   4   8
             4  5   2   7
             <BLANKLINE>
             [5 rows x 3 columns]
             >>> df
-            A   B
+               A   B
             0  1  10
             1  2   8
             2  3   6
             3  4   4
             4  5   2
             <BLANKLINE>
             [5 rows x 2 columns]
 
-            Multiple columns can be assigned to using multi-line expressions:
+        Multiple columns can be assigned to using multi-line expressions:
 
             >>> df.eval(
             ...     '''
             ... C = A + B
             ... D = A - B
             ... '''
             ... )
-            A   B   C  D
+               A   B   C  D
             0  1  10  11 -9
             1  2   8  10 -6
             2  3   6   9 -3
             3  4   4   8  0
             4  5   2   7  3
             <BLANKLINE>
             [5 rows x 4 columns]
@@ -5063,14 +5868,15 @@
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
 
     def query(self, expr: str) -> DataFrame | None:
         """
         Query the columns of a DataFrame with a boolean expression.
 
         **Examples:**
+
             >>> import bigframes.pandas as bpd
             >>> bpd.options.display.progress_bar = None
 
             >>> df = bpd.DataFrame({'A': range(1, 6),
             ...                    'B': range(10, 0, -2),
             ...                    'C C': range(10, 5, -1)})
             >>> df
@@ -5358,23 +6164,71 @@
         """
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
 
     @property
     def iat(self):
         """Access a single value for a row/column pair by integer position.
 
+        **Examples:**
+
+            >>> import bigframes.pandas as bpd
+            >>> df = bpd.DataFrame([[0, 2, 3], [0, 4, 1], [10, 20, 30]],
+            ...                    columns=['A', 'B', 'C'])
+            >>> bpd.options.display.progress_bar = None
+            >>> df
+                A       B       C
+            0   0       2       3
+            1   0       4       1
+            2   10      20      30
+            <BLANKLINE>
+            [3 rows x 3 columns]
+
+        Get value at specified row/column pair
+
+            >>> df.iat[1, 2]
+            1
+
+        Get value within a series
+
+            >>> df.loc[0].iat[1]
+            2
+
         Returns:
             bigframes.core.indexers.IatDataFrameIndexer: Indexers object.
         """
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
 
     @property
     def at(self):
         """Access a single value for a row/column label pair.
 
+        **Examples:**
+
+            >>> import bigframes.pandas as bpd
+            >>> df = bpd.DataFrame([[0, 2, 3], [0, 4, 1], [10, 20, 30]],
+            ...   index=[4, 5, 6], columns=['A', 'B', 'C'])
+            >>> bpd.options.display.progress_bar = None
+            >>> df
+                A   B   C
+            4   0   2   3
+            5   0   4   1
+            6  10  20  30
+            <BLANKLINE>
+            [3 rows x 3 columns]
+
+        Get value at specified row/column pair
+
+            >>> df.at[4, 'B']
+            2
+
+        Get value within a series
+
+            >>> df.loc[5].at['B']
+            4
+
         Returns:
             bigframes.core.indexers.AtDataFrameIndexer: Indexers object.
         """
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
 
     def dot(self, other):
         """
@@ -5387,14 +6241,15 @@
 
         .. note::
             The dimensions of DataFrame and other must be compatible in order to
             compute the matrix multiplication. In addition, the column names of
             DataFrame and the index of other must contain the same values, as they
             will be aligned prior to the multiplication.
 
+        .. note::
             The dot method for Series computes the inner product, instead of the
             matrix product here.
 
         **Examples:**
 
             >>> import bigframes.pandas as bpd
             >>> bpd.options.display.progress_bar = None
@@ -5473,17 +6328,264 @@
             Series or DataFrame:
                 If `other` is a Series, return the matrix product between self and
                 other as a Series. If other is a DataFrame, return
                 the matrix product of self and other in a DataFrame.
         """
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
 
+    def __matmul__(self, other):
+        """
+        Compute the matrix multiplication between the DataFrame and other, using
+        operator `@`.
+
+        Equivalent to `DataFrame.dot(other)`.
+
+        **Examples:**
+
+            >>> import bigframes.pandas as bpd
+            >>> bpd.options.display.progress_bar = None
+
+            >>> left = bpd.DataFrame([[0, 1, -2, -1], [1, 1, 1, 1]])
+            >>> left
+               0  1   2   3
+            0  0  1  -2  -1
+            1  1  1   1   1
+            <BLANKLINE>
+            [2 rows x 4 columns]
+            >>> right = bpd.DataFrame([[0, 1], [1, 2], [-1, -1], [2, 0]])
+            >>> right
+                0   1
+            0   0   1
+            1   1   2
+            2  -1  -1
+            3   2   0
+            <BLANKLINE>
+            [4 rows x 2 columns]
+            >>> left @ right
+               0  1
+            0  1  4
+            1  2  2
+            <BLANKLINE>
+            [2 rows x 2 columns]
+
+        The operand can be a Series, in which case the result will also be a
+        Series:
+
+            >>> right = bpd.Series([1, 2, -1,0])
+            >>> left @ right
+            0    4
+            1    2
+            dtype: Int64
+
+        Args:
+            other (DataFrame or Series):
+                Object to be matrix multiplied with the DataFrame.
+
+        Returns:
+            DataFrame or Series: The result of the matrix multiplication.
+        """
+        raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
+
     @property
     def plot(self):
         """
         Make plots of Dataframes.
 
         Returns:
             bigframes.operations.plotting.PlotAccessor:
                 An accessor making plots.
         """
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
+
+    def __len__(self):
+        """Returns number of rows in the DataFrame, serves `len` operator.
+
+        **Examples:**
+
+            >>> import bigframes.pandas as bpd
+            >>> bpd.options.display.progress_bar = None
+
+            >>> df = bpd.DataFrame({
+            ...         'a': [0, 1, 2],
+            ...         'b': [3, 4, 5]
+            ...      })
+            >>> len(df)
+            3
+        """
+        raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
+
+    def __array__(self):
+        """
+        Returns the rows as NumPy array.
+
+        Equivalent to `DataFrame.to_numpy(dtype)`.
+
+        Users should not call this directly. Rather, it is invoked by
+        `numpy.array` and `numpy.asarray`.
+
+        **Examples:**
+
+            >>> import bigframes.pandas as bpd
+            >>> bpd.options.display.progress_bar = None
+            >>> import numpy as np
+
+            >>> df = bpd.DataFrame({"a": [1, 2, 3], "b": [11, 22, 33]})
+
+            >>> np.array(df)
+            array([[1, 11],
+                [2, 22],
+                [3, 33]], dtype=object)
+
+            >>> np.asarray(df)
+            array([[1, 11],
+                [2, 22],
+                [3, 33]], dtype=object)
+
+        Args:
+            dtype (str or numpy.dtype, optional):
+                The dtype to use for the resulting NumPy array. By default,
+                the dtype is inferred from the data.
+
+        Returns:
+            numpy.ndarray:
+                The rows in the DataFrame converted to a `numpy.ndarray` with
+                the specified dtype.
+        """
+        raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
+
+    def __getitem__(self, key):
+        """Gets the specified column(s) from the DataFrame.
+
+        **Examples:**
+
+            >>> import bigframes.pandas as bpd
+            >>> bpd.options.display.progress_bar = None
+
+            >>> df = bpd.DataFrame({
+            ...     "name" : ["alpha", "beta", "gamma"],
+            ...     "age": [20, 30, 40],
+            ...     "location": ["WA", "NY", "CA"]
+            ... })
+            >>> df
+                name  age location
+            0  alpha   20       WA
+            1   beta   30       NY
+            2  gamma   40       CA
+            <BLANKLINE>
+            [3 rows x 3 columns]
+
+        You can specify a column label to retrieve the corresponding Series.
+
+            >>> df["name"]
+            0    alpha
+            1     beta
+            2    gamma
+            Name: name, dtype: string
+
+        You can specify a list of column labels to retrieve a Dataframe.
+
+            >>> df[["name", "age"]]
+                name  age
+            0  alpha   20
+            1   beta   30
+            2  gamma   40
+            <BLANKLINE>
+            [3 rows x 2 columns]
+
+        You can specify a condition as a series of booleans to retrieve matching
+        rows.
+
+            >>> df[df["age"] > 25]
+                name  age location
+            1   beta   30       NY
+            2  gamma   40       CA
+            <BLANKLINE>
+            [2 rows x 3 columns]
+
+        You can specify a pandas Index with desired column labels.
+
+            >>> import pandas as pd
+            >>> df[pd.Index(["age", "location"])]
+               age location
+            0   20       WA
+            1   30       NY
+            2   40       CA
+            <BLANKLINE>
+            [3 rows x 2 columns]
+
+        Args:
+            key (index):
+                Index or list of indices. It can be a column label, a list of
+                column labels, a Series of booleans or a pandas Index of desired
+                column labels
+
+        Returns:
+            Series or Value: Value(s) at the requested index(es).
+        """
+        raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
+
+    def __setitem__(self, key, value):
+        """Modify or insert a column into the DataFrame.
+
+        .. note::
+            This does **not** modify the original table the DataFrame was
+            derived from.
+
+        **Examples:**
+
+            >>> import bigframes.pandas as bpd
+            >>> bpd.options.display.progress_bar = None
+
+            >>> df = bpd.DataFrame({
+            ...     "name" : ["alpha", "beta", "gamma"],
+            ...     "age": [20, 30, 40],
+            ...     "location": ["WA", "NY", "CA"]
+            ... })
+            >>> df
+                name  age location
+            0  alpha   20       WA
+            1   beta   30       NY
+            2  gamma   40       CA
+            <BLANKLINE>
+            [3 rows x 3 columns]
+
+        You can add assign a constant to a new column.
+
+            >>> df["country"] = "USA"
+            >>> df
+                name  age location country
+            0  alpha   20       WA     USA
+            1   beta   30       NY     USA
+            2  gamma   40       CA     USA
+            <BLANKLINE>
+            [3 rows x 4 columns]
+
+        You can assign a Series to a new column.
+
+            >>> df["new_age"] = df["age"] + 5
+            >>> df
+                name  age location country  new_age
+            0  alpha   20       WA     USA       25
+            1   beta   30       NY     USA       35
+            2  gamma   40       CA     USA       45
+            <BLANKLINE>
+            [3 rows x 5 columns]
+
+        You can assign a Series to an existing column.
+
+            >>> df["new_age"] = bpd.Series([29, 39, 19], index=[1, 2, 0])
+            >>> df
+                name  age location country  new_age
+            0  alpha   20       WA     USA       19
+            1   beta   30       NY     USA       29
+            2  gamma   40       CA     USA       39
+            <BLANKLINE>
+            [3 rows x 5 columns]
+
+        Args:
+            key (column index):
+                It can be a new column to be inserted, or an existing column to
+                be modified.
+            value (scalar or Series):
+                Value to be assigned to the column
+        """
+        raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
```

### Comparing `bigframes-1.1.0/third_party/bigframes_vendored/pandas/core/generic.py` & `bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/generic.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,21 +161,28 @@
             0    2023010000246789
             1    1624123244123101
             2    1054834234120101
             dtype: Int64
 
         Args:
             dtype (str or pandas.ExtensionDtype):
-                A dtype supported by BigQuery DataFrame include ``'boolean'``, ``'Float64'``, ``'Int64'``,
-                ``'int64[pyarrow]'``, ``'string'``, ``'string[pyarrow]'``, ``'timestamp[us, tz=UTC][pyarrow]'``,
-                ``'timestamp\[us\]\[pyarrow\]'``, ``'date32\[day\]\[pyarrow\]'``, ``'time64\[us\]\[pyarrow\]'``.
-                A pandas.ExtensionDtype include ``pandas.BooleanDtype()``, ``pandas.Float64Dtype()``,
-                ``pandas.Int64Dtype()``, ``pandas.StringDtype(storage="pyarrow")``,
-                ``pd.ArrowDtype(pa.date32())``, ``pd.ArrowDtype(pa.time64("us"))``,
-                ``pd.ArrowDtype(pa.timestamp("us"))``, ``pd.ArrowDtype(pa.timestamp("us", tz="UTC"))``.
+                A dtype supported by BigQuery DataFrame include ``'boolean'``,
+                ``'Float64'``, ``'Int64'``, ``'int64\\[pyarrow\\]'``,
+                ``'string'``, ``'string\\[pyarrow\\]'``,
+                ``'timestamp\\[us, tz=UTC\\]\\[pyarrow\\]'``,
+                ``'timestamp\\[us\\]\\[pyarrow\\]'``,
+                ``'date32\\[day\\]\\[pyarrow\\]'``,
+                ``'time64\\[us\\]\\[pyarrow\\]'``.
+                A pandas.ExtensionDtype include ``pandas.BooleanDtype()``,
+                ``pandas.Float64Dtype()``, ``pandas.Int64Dtype()``,
+                ``pandas.StringDtype(storage="pyarrow")``,
+                ``pd.ArrowDtype(pa.date32())``,
+                ``pd.ArrowDtype(pa.time64("us"))``,
+                ``pd.ArrowDtype(pa.timestamp("us"))``,
+                ``pd.ArrowDtype(pa.timestamp("us", tz="UTC"))``.
 
         Returns:
             same type as caller
 
         """
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
 
@@ -578,14 +585,26 @@
     def dtypes(self):
         """Return the dtypes in the DataFrame.
 
         This returns a Series with the data type of each column.
         The result's index is the original DataFrame's columns. Columns
         with mixed types aren't supported yet in BigQuery DataFrames.
 
+        **Examples:**
+
+            >>> import bigframes.pandas as bpd
+            >>> bpd.options.display.progress_bar = None
+
+            >>> df = bpd.DataFrame({'float': [1.0], 'int': [1], 'string': ['foo']})
+            >>> df.dtypes
+            float             Float64
+            int                 Int64
+            string    string[pyarrow]
+            dtype: object
+
         Returns:
             A *pandas* Series with the data type of each column.
         """
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
 
     def copy(self):
         """Make a copy of this object's indices and data.
@@ -639,17 +658,17 @@
             0  1  2
             1  3  4
             <BLANKLINE>
             [2 rows x 2 columns]
 
             >>> df.loc[df["b"] == 2, "b"] = 22
             >>> df
-               a     b
-            0  1  22.0
-            1  3   4.0
+               a   b
+            0  1  22
+            1  3   4
             <BLANKLINE>
             [2 rows x 2 columns]
             >>> df_copy
                a  b
             0  1  2
             1  3  4
             <BLANKLINE>
@@ -1097,13 +1116,43 @@
 
         Returns:
             same type as caller
         """
         return common.pipe(self, func, *args, **kwargs)
 
     def __nonzero__(self):
+        """Returns the truth value of the object."""
         raise ValueError(
             f"The truth value of a {type(self).__name__} is ambiguous. "
             "Use a.empty, a.bool(), a.item(), a.any() or a.all()."
         )
 
     __bool__ = __nonzero__
+
+    def __getattr__(self, name: str):
+        """
+        After regular attribute access, try looking up the name
+        This allows simpler access to columns for interactive use.
+        """
+        raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
+
+    def equals(self, other) -> bool:
+        """
+        Test whether two objects contain the same elements.
+
+        This function allows two Series or DataFrames to be compared against
+        each other to see if they have the same shape and elements. NaNs in
+        the same location are considered equal.
+
+        The row/column index do not need to have the same type, as long
+        as the values are considered equal. Corresponding columns must be of
+        the same dtype.
+
+        Args:
+            other (Series or DataFrame):
+                The other Series or DataFrame to be compared with the first.
+
+        Returns:
+            bool: True if all elements are the same in both objects, False
+            otherwise.
+        """
+        raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
```

### Comparing `bigframes-1.1.0/third_party/bigframes_vendored/pandas/core/groupby/__init__.py` & `bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/groupby/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,26 +20,26 @@
     def any(self):
         """
         Return True if any value in the group is true, else False.
 
         Returns:
             Series or DataFrame: DataFrame or Series of boolean values,
                 where a value is True if any element is True within its
-                respective group, False otherwise.
+                respective group; otherwise False.
         """
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
 
     def all(self):
         """
         Return True if all values in the group are true, else False.
 
         Returns:
             Series or DataFrame: DataFrame or Series of boolean values,
                 where a value is True if all elements are True within its
-                respective group, False otherwise.
+                respective group; otherwise False.
         """
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
 
     def count(self):
         """
         Compute count of group, excluding missing values.
 
@@ -335,15 +335,15 @@
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
 
     def expanding(self, *args, **kwargs):
         """
         Provides expanding functionality.
 
         Returns:
-            Series or DataFrame: A expanding grouper, providing expanding functionality per group.
+            Series or DataFrame: An expanding grouper, providing expanding functionality per group.
         """
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
 
 
 class SeriesGroupBy(GroupBy):
     def agg(self, func):
         """
```

### Comparing `bigframes-1.1.0/third_party/bigframes_vendored/pandas/core/indexes/base.py` & `bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/indexes/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 
         Name is set on the new object.
 
         Args:
             name (Label, optional):
                 Set name for new object.
         Returns:
-            Index: Index refer to new object which is a copy of this object.
+            Index: Index reference to new object, which is a copy of this object.
         """
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
 
     def transpose(self) -> Index:
         """
         Return the transpose, which is by definition self.
 
@@ -144,15 +144,15 @@
         """
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
 
     def isin(self, values):
         """
         Return a boolean array where the index values are in `values`.
 
-        Compute boolean array of whether each index value is found in the
+        Compute boolean array to check whether each index value is found in the
         passed set of values. The length of the returned boolean array matches
         the length of the index.
 
         Args:
             values (set or list-like):
                 Sought values.
 
@@ -191,15 +191,15 @@
         Returns:
             scalar: Maximum value.
         """
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
 
     def argmin(self) -> int:
         """
-        Return int position of the smallest value in the Series.
+        Return int position of the smallest value in the series.
 
         If the minimum is achieved in multiple locations,
         the first row position is returned.
 
         Returns:
             int: Row position of the minimum value.
         """
@@ -260,15 +260,15 @@
 
         The resulting object will be in descending order so that the
         first element is the most frequently-occurring element.
         Excludes NA values by default.
 
         Args:
             normalize (bool, default False):
-                If True then the object returned will contain the relative
+                If True, then the object returned will contain the relative
                 frequencies of the unique values.
             sort (bool, default True):
                 Sort by frequencies.
             ascending (bool, default False):
                 Sort in ascending order.
             dropna (bool, default True):
                 Don't include counts of NaN.
@@ -312,15 +312,15 @@
         """
         Make new Index with passed list of labels deleted.
 
         Args:
             labels (array-like or scalar):
 
         Returns:
-            Index: Will be same type as self
+            Index: Will be same type as self.
         """
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
 
     def dropna(self, how: str = "any"):
         """Return Index without NA/NaN values.
 
         Args:
```

### Comparing `bigframes-1.1.0/third_party/bigframes_vendored/pandas/core/indexing.py` & `bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/indexing.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/third_party/bigframes_vendored/pandas/core/reshape/concat.py` & `bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/reshape/concat.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/third_party/bigframes_vendored/pandas/core/reshape/encoding.py` & `bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/reshape/encoding.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/third_party/bigframes_vendored/pandas/core/reshape/merge.py` & `bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/reshape/merge.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/third_party/bigframes_vendored/pandas/core/reshape/tile.py` & `bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/reshape/tile.py`

 * *Files 13% similar despite different names*

```diff
@@ -72,26 +72,40 @@
         >>> bpd.cut(s, bins=bins_tuples)
         0                                            <NA>
         1     {'left_exclusive': 0, 'right_inclusive': 1}
         2                                            <NA>
         3    {'left_exclusive': 5, 'right_inclusive': 20}
         dtype: struct<left_exclusive: int64, right_inclusive: int64>[pyarrow]
 
+    Cut with an iterable of ints:
+
+        >>> bins_ints = [0, 1, 5, 20]
+        >>> bpd.cut(s, bins=bins_ints)
+        0                                            <NA>
+        1     {'left_exclusive': 0, 'right_inclusive': 1}
+        2     {'left_exclusive': 1, 'right_inclusive': 5}
+        3    {'left_exclusive': 5, 'right_inclusive': 20}
+        dtype: struct<left_exclusive: int64, right_inclusive: int64>[pyarrow]
+
     Args:
         x (Series):
             The input Series to be binned. Must be 1-dimensional.
-        bins (int, pd.IntervalIndex, Iterable[Tuple[Union[int, float], Union[int, float]]]):
+        bins (int, pd.IntervalIndex, Iterable):
             The criteria to bin by.
 
             int: Defines the number of equal-width bins in the range of `x`. The
             range of `x` is extended by .1% on each side to include the minimum
             and maximum values of `x`.
 
             pd.IntervalIndex or Iterable of tuples: Defines the exact bins to be used.
             It's important to ensure that these bins are non-overlapping.
+
+            Iterable of numerics: Defines the exact bins by using the interval
+            between each item and its following item. The items must be monotonically
+            increasing.
         labels (None):
             Specifies the labels for the returned bins. Must be the same length as
             the resulting bins. If False, returns only integer indicators of the
             bins. This affects the type of the output container.
 
     Returns:
         Series: A Series representing the respective bin for each value
```

### Comparing `bigframes-1.1.0/third_party/bigframes_vendored/pandas/core/series.py` & `bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/series.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 Data structure for 1-dimensional cross-sectional and time series data
 """
 from __future__ import annotations
 
 from typing import Hashable, IO, Literal, Mapping, Optional, Sequence, TYPE_CHECKING
 
 from bigframes_vendored.pandas.core.generic import NDFrame
+import numpy
 import numpy as np
 from pandas._libs import lib
 from pandas._typing import Axis, FilePath, NaPosition, WriteBuffer
 
 from bigframes import constants
 
 if TYPE_CHECKING:
@@ -115,21 +116,23 @@
         """
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
 
     @property
     def dtype(self):
         """
         Return the dtype object of the underlying data.
-        """
-        raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
 
-    @property
-    def dtypes(self):
-        """
-        Return the dtype object of the underlying data.
+        **Examples:**
+
+            >>> import bigframes.pandas as bpd
+            >>> bpd.options.display.progress_bar = None
+
+            >>> s = bpd.Series([1, 2, 3])
+            >>> s.dtype
+            Int64Dtype()
         """
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
 
     @property
     def name(self) -> Hashable:
         """
         Return the name of the Series.
@@ -170,14 +173,39 @@
         Returns:
             hashable object: The name of the Series, also the column name
                 if part of a DataFrame.
         """
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
 
     @property
+    def hasnans(self) -> bool:
+        """
+        Return True if there are any NaNs.
+
+        **Examples:**
+
+            >>> import bigframes.pandas as bpd
+            >>> bpd.options.display.progress_bar = None
+
+            >>> s = bpd.Series([1, 2, 3, None])
+            >>> s
+            0     1.0
+            1     2.0
+            2     3.0
+            3    <NA>
+            dtype: Float64
+            >>> s.hasnans
+            True
+
+        Returns:
+            bool
+        """
+        raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
+
+    @property
     def T(self) -> Series:
         """Return the transpose, which is by definition self.
 
         **Examples:**
 
             >>> import bigframes.pandas as bpd
             >>> bpd.options.display.progress_bar = None
@@ -813,14 +841,46 @@
 
         Returns:
             float:  Will return NaN if there are fewer than two numeric pairs, either series has a
                 variance or covariance of zero, or any input value is infinite.
         """
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
 
+    def autocorr(self, lag: int = 1) -> float:
+        """
+        Compute the lag-N autocorrelation.
+
+        This method computes the Pearson correlation between
+        the Series and its shifted self.
+
+        **Examples:**
+            >>> import bigframes.pandas as bpd
+            >>> bpd.options.display.progress_bar = None
+
+            >>> s = bpd.Series([0.25, 0.5, 0.2, -0.05])
+            >>> s.autocorr()  # doctest: +ELLIPSIS
+            0.10355...
+            >>> s.autocorr(lag=2)
+            -1.0
+
+            If the Pearson correlation is not well defined, then 'NaN' is returned.
+
+            >>> s = bpd.Series([1, 0, 0, 0])
+            >>> s.autocorr()
+            nan
+
+        Args:
+            lag (int, default 1):
+                Number of lags to apply before performing autocorrelation.
+
+        Returns:
+            float: The Pearson correlation between self and self.shift(lag).
+        """
+        raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
+
     def cov(
         self,
         other,
     ) -> float:
         """
         Compute covariance with Series, excluding missing values.
 
@@ -898,21 +958,21 @@
 
 
         """
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
 
     def __matmul__(self, other):
         """
-        Matrix multiplication using binary `@` operator in Python>=3.5.
+        Matrix multiplication using binary `@` operator.
         """
         return NotImplemented
 
     def __rmatmul__(self, other):
         """
-        Matrix multiplication using binary `@` operator in Python>=3.5.
+        Matrix multiplication using binary `@` operator.
         """
         return NotImplemented
 
     def sort_values(
         self,
         *,
         axis: Axis = 0,
@@ -2110,14 +2170,63 @@
 
         Returns:
             bigframes.series.Series: The result of the operation.
 
         """
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
 
+    def __add__(self, other):
+        """Get addition of Series and other, element-wise, using operator `+`.
+
+        Equivalent to `Series.add(other)`.
+
+        **Examples:**
+
+            >>> import bigframes.pandas as bpd
+            >>> bpd.options.display.progress_bar = None
+
+            >>> s = bpd.Series([1.5, 2.6], index=['elk', 'moose'])
+            >>> s
+            elk      1.5
+            moose    2.6
+            dtype: Float64
+
+        You can add a scalar.
+
+            >>> s + 1.5
+            elk      3.0
+            moose    4.1
+            dtype: Float64
+
+        You can add another Series with index aligned.
+
+            >>> delta = bpd.Series([1.5, 2.6], index=['elk', 'moose'])
+            >>> s + delta
+            elk      3.0
+            moose    5.2
+            dtype: Float64
+
+        Adding any mis-aligned index will result in invalid values.
+
+            >>> delta = bpd.Series([1.5, 2.6], index=['moose', 'bison'])
+            >>> s + delta
+            elk      <NA>
+            moose     4.1
+            bison    <NA>
+            dtype: Float64
+
+        Args:
+            other (scalar or Series):
+                Object to be added to the Series.
+
+        Returns:
+            Series: The result of adding `other` to Series.
+        """
+        raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
+
     def radd(self, other) -> Series:
         """Return addition of Series and other, element-wise (binary operator radd).
 
         Equivalent to ``other + series``, but with support to substitute a fill_value for
         missing data in either one of the inputs.
 
         Args:
@@ -2125,14 +2234,28 @@
 
         Returns:
             bigframes.series.Series: The result of the operation.
 
         """
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
 
+    def __radd__(self, other):
+        """Get addition of Series and other, element-wise, using operator `+`.
+
+        Equivalent to `Series.radd(other)`.
+
+        Args:
+            other (scalar or Series):
+                Object to which Series should be added.
+
+        Returns:
+            Series: The result of adding Series to `other`.
+        """
+        raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
+
     def sub(
         self,
         other,
     ) -> Series:
         """Return subtraction of Series and other, element-wise (binary operator sub).
 
         Equivalent to ``series - other``, but with support to substitute a fill_value for
@@ -2143,14 +2266,63 @@
 
         Returns:
             bigframes.series.Series: The result of the operation.
 
         """
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
 
+    def __sub__(self, other):
+        """Get subtraction of other from Series, element-wise, using operator `-`.
+
+        Equivalent to `Series.sub(other)`.
+
+        **Examples:**
+
+            >>> import bigframes.pandas as bpd
+            >>> bpd.options.display.progress_bar = None
+
+            >>> s = bpd.Series([1.5, 2.6], index=['elk', 'moose'])
+            >>> s
+            elk      1.5
+            moose    2.6
+            dtype: Float64
+
+        You can subtract a scalar.
+
+            >>> s - 1.5
+            elk      0.0
+            moose    1.1
+            dtype: Float64
+
+        You can subtract another Series with index aligned.
+
+            >>> delta = bpd.Series([0.5, 1.0], index=['elk', 'moose'])
+            >>> s - delta
+            elk      1.0
+            moose    1.6
+            dtype: Float64
+
+        Adding any mis-aligned index will result in invalid values.
+
+            >>> delta = bpd.Series([0.5, 1.0], index=['moose', 'bison'])
+            >>> s - delta
+            elk      <NA>
+            moose     2.1
+            bison    <NA>
+            dtype: Float64
+
+        Args:
+            other (scalar or Series):
+                Object to subtract from the Series.
+
+        Returns:
+            Series: The result of subtraction.
+        """
+        raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
+
     def rsub(self, other) -> Series:
         """Return subtraction of Series and other, element-wise (binary operator rsub).
 
         Equivalent to ``other - series``, but with support to substitute a fill_value for
         missing data in either one of the inputs.
 
         Args:
@@ -2158,14 +2330,28 @@
 
         Returns:
             bigframes.series.Series: The result of the operation.
 
         """
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
 
+    def __rsub__(self, other):
+        """Get subtraction of Series from other, element-wise, using operator `-`.
+
+        Equivalent to `Series.rsub(other)`.
+
+        Args:
+            other (scalar or Series):
+                Object to subtract the Series from.
+
+        Returns:
+            Series: The result of subtraction.
+        """
+        raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
+
     def mul(self, other) -> Series:
         """Return multiplication of Series and other, element-wise (binary operator mul).
 
         Equivalent to ``other * series``, but with support to substitute a fill_value for
         missing data in either one of the inputs.
 
         Args:
@@ -2173,28 +2359,81 @@
 
         Returns:
             bigframes.series.Series: The result of the operation.
 
         """
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
 
+    def __mul__(self, other):
+        """
+        Get multiplication of Series with other, element-wise, using operator `*`.
+
+        Equivalent to `Series.mul(other)`.
+
+        **Examples:**
+
+            >>> import bigframes.pandas as bpd
+            >>> bpd.options.display.progress_bar = None
+
+        You can multiply with a scalar:
+
+            >>> s = bpd.Series([1, 2, 3])
+            >>> s * 3
+            0    3
+            1    6
+            2    9
+            dtype: Int64
+
+        You can also multiply with another Series:
+
+            >>> s1 = bpd.Series([2, 3, 4])
+            >>> s * s1
+            0     2
+            1     6
+            2    12
+            dtype: Int64
+
+        Args:
+            other (scalar or Series):
+                Object to multiply with the Series.
+
+        Returns:
+            Series: The result of the multiplication.
+        """
+        raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
+
     def rmul(self, other) -> Series:
         """Return multiplication of Series and other, element-wise (binary operator mul).
 
         Equivalent to ``series * others``, but with support to substitute a fill_value for
         missing data in either one of the inputs.
 
         Args:
             other (Series, or scalar value):
 
         Returns:
             Series: The result of the operation.
         """
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
 
+    def __rmul__(self, other):
+        """
+        Get multiplication of other with Series, element-wise, using operator `*`.
+
+        Equivalent to `Series.rmul(other)`.
+
+        Args:
+            other (scalar or Series):
+                Object to multiply the Series with.
+
+        Returns:
+            Series: The result of the multiplication.
+        """
+        raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
+
     def truediv(self, other) -> Series:
         """Return floating division of Series and other, element-wise (binary operator truediv).
 
         Equivalent to ``series / other``, but with support to substitute a fill_value for
         missing data in either one of the inputs.
 
         Args:
@@ -2202,14 +2441,52 @@
 
         Returns:
             bigframes.series.Series: The result of the operation.
 
         """
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
 
+    def __truediv__(self, other):
+        """
+        Get division of Series by other, element-wise, using operator `/`.
+
+        Equivalent to `Series.truediv(other)`.
+
+        **Examples:**
+
+            >>> import bigframes.pandas as bpd
+            >>> bpd.options.display.progress_bar = None
+
+        You can multiply with a scalar:
+
+            >>> s = bpd.Series([1, 2, 3])
+            >>> s / 2
+            0    0.5
+            1    1.0
+            2    1.5
+            dtype: Float64
+
+        You can also multiply with another Series:
+
+            >>> denominator = bpd.Series([2, 3, 4])
+            >>> s / denominator
+            0         0.5
+            1    0.666667
+            2        0.75
+            dtype: Float64
+
+        Args:
+            other (scalar or Series):
+                Object to divide the Series by.
+
+        Returns:
+            Series: The result of the division.
+        """
+        raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
+
     def rtruediv(self, other) -> Series:
         """Return floating division of Series and other, element-wise (binary operator rtruediv).
 
         Equivalent to ``other / series``, but with support to substitute a fill_value for
         missing data in either one of the inputs.
 
         Args:
@@ -2217,14 +2494,29 @@
 
         Returns:
             bigframes.series.Series: The result of the operation.
 
         """
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
 
+    def __rtruediv__(self, other):
+        """
+        Get division of other by Series, element-wise, using operator `/`.
+
+        Equivalent to `Series.rtruediv(other)`.
+
+        Args:
+            other (scalar or Series):
+                Object to divide by the Series.
+
+        Returns:
+            Series: The result of the division.
+        """
+        raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
+
     def floordiv(self, other) -> Series:
         """Return integer division of Series and other, element-wise (binary operator floordiv).
 
         Equivalent to ``series // other``, but with support to substitute a fill_value for
         missing data in either one of the inputs.
 
         Args:
@@ -2232,14 +2524,52 @@
 
         Returns:
             bigframes.series.Series: The result of the operation.
 
         """
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
 
+    def __floordiv__(self, other):
+        """
+        Get integer divison of Series by other, using arithmatic operator `//`.
+
+        Equivalent to `Series.floordiv(other)`.
+
+        **Examples:**
+
+            >>> import bigframes.pandas as bpd
+            >>> bpd.options.display.progress_bar = None
+
+        You can divide by a scalar:
+
+            >>> s = bpd.Series([15, 30, 45])
+            >>> s // 2
+            0     7
+            1    15
+            2    22
+            dtype: Int64
+
+        You can also divide by another DataFrame:
+
+            >>> divisor = bpd.Series([3, 4, 4])
+            >>> s // divisor
+            0     5
+            1     7
+            2    11
+            dtype: Int64
+
+        Args:
+            other (scalar or Series):
+                Object to divide the Series by.
+
+        Returns:
+            Series: The result of the integer divison.
+        """
+        raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
+
     def rfloordiv(self, other) -> Series:
         """Return integer division of Series and other, element-wise (binary operator rfloordiv).
 
         Equivalent to ``other // series``, but with support to substitute a fill_value for
         missing data in either one of the inputs.
 
         Args:
@@ -2247,14 +2577,29 @@
 
         Returns:
             bigframes.series.Series: The result of the operation.
 
         """
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
 
+    def __rfloordiv__(self, other):
+        """
+        Get integer divison of other by Series, using arithmatic operator `//`.
+
+        Equivalent to `Series.rfloordiv(other)`.
+
+        Args:
+            other (scalar or Series):
+                Object to divide by the Series.
+
+        Returns:
+            Series: The result of the integer divison.
+        """
+        raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
+
     def mod(self, other) -> Series:
         """Return modulo of Series and other, element-wise (binary operator mod).
 
         Equivalent to ``series % other``, but with support to substitute a fill_value for
         missing data in either one of the inputs.
 
         Args:
@@ -2262,14 +2607,52 @@
 
         Returns:
             bigframes.series.Series: The result of the operation.
 
         """
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
 
+    def __mod__(self, other):
+        """
+        Get modulo of Series with other, element-wise, using operator `%`.
+
+        Equivalent to `Series.mod(other)`.
+
+        **Examples:**
+
+            >>> import bigframes.pandas as bpd
+            >>> bpd.options.display.progress_bar = None
+
+        You can modulo with a scalar:
+
+            >>> s = bpd.Series([1, 2, 3])
+            >>> s % 3
+            0    1
+            1    2
+            2    0
+            dtype: Int64
+
+        You can also modulo with another Series:
+
+            >>> modulo = bpd.Series([3, 3, 3])
+            >>> s % modulo
+            0    1
+            1    2
+            2    0
+            dtype: Int64
+
+        Args:
+            other (scalar or Series):
+                Object to modulo the Series by.
+
+        Returns:
+            Series: The result of the modulo.
+        """
+        raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
+
     def rmod(self, other) -> Series:
         """Return modulo of Series and other, element-wise (binary operator mod).
 
         Equivalent to ``series % other``, but with support to substitute a fill_value for
         missing data in either one of the inputs.
 
         Args:
@@ -2277,14 +2660,29 @@
 
         Returns:
             bigframes.series.Series: The result of the operation.
 
         """
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
 
+    def __rmod__(self, other):
+        """
+        Get modulo of other with Series, element-wise, using operator `%`.
+
+        Equivalent to `Series.rmod(other)`.
+
+        Args:
+            other (scalar or Series):
+                Object to modulo by the Series.
+
+        Returns:
+            Series: The result of the modulo.
+        """
+        raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
+
     def pow(self, other) -> Series:
         """Return Exponential power of series and other, element-wise (binary operator `pow`).
 
         Equivalent to ``series ** other``, but with support to substitute a fill_value for
         missing data in either one of the inputs.
 
         Args:
@@ -2292,14 +2690,53 @@
 
         Returns:
             bigframes.series.Series: The result of the operation.
 
         """
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
 
+    def __pow__(self, other):
+        """
+        Get exponentiation of Series with other, element-wise, using operator
+        `**`.
+
+        Equivalent to `Series.pow(other)`.
+
+        **Examples:**
+
+            >>> import bigframes.pandas as bpd
+            >>> bpd.options.display.progress_bar = None
+
+        You can exponentiate with a scalar:
+
+            >>> s = bpd.Series([1, 2, 3])
+            >>> s ** 2
+            0    1
+            1    4
+            2    9
+            dtype: Int64
+
+        You can also exponentiate with another Series:
+
+            >>> exponent = bpd.Series([3, 2, 1])
+            >>> s ** exponent
+            0    1
+            1    4
+            2    3
+            dtype: Int64
+
+        Args:
+            other (scalar or Series):
+                Object to exponentiate the Series with.
+
+        Returns:
+            Series: The result of the exponentiation.
+        """
+        raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
+
     def rpow(self, other) -> Series:
         """Return Exponential power of series and other, element-wise (binary operator `rpow`).
 
         Equivalent to ``other ** series``, but with support to substitute a fill_value for
         missing data in either one of the inputs.
 
         Args:
@@ -2307,14 +2744,30 @@
 
         Returns:
             bigframes.series.Series: The result of the operation.
 
         """
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
 
+    def __rpow__(self, other):
+        """
+        Get exponentiation of other with Series, element-wise, using operator
+        `**`.
+
+        Equivalent to `Series.rpow(other)`.
+
+        Args:
+            other (scalar or Series):
+                Object to exponentiate with the Series.
+
+        Returns:
+            Series: The result of the exponentiation.
+        """
+        raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
+
     def divmod(self, other) -> Series:
         """Return integer division and modulo of Series and other, element-wise (binary operator divmod).
 
         Equivalent to divmod(series, other).
 
         Args:
             other: Series, or scalar value
@@ -2337,14 +2790,127 @@
         Returns:
             2-Tuple of Series: The result of the operation. The result is always
             consistent with (rfloordiv, rmod) (though pandas may not).
 
         """
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
 
+    def combine_first(self, other) -> Series:
+        """
+        Update null elements with value in the same location in 'other'.
+
+        Combine two Series objects by filling null values in one Series with
+        non-null values from the other Series. Result index will be the union
+        of the two indexes.
+
+        **Examples:**
+            >>> import bigframes.pandas as bpd
+            >>> import numpy as np
+            >>> bpd.options.display.progress_bar = None
+
+            >>> s1 = bpd.Series([1, np.nan])
+            >>> s2 = bpd.Series([3, 4, 5])
+            >>> s1.combine_first(s2)
+            0    1.0
+            1    4.0
+            2    5.0
+            dtype: Float64
+
+            Null values still persist if the location of that null value
+            does not exist in `other`
+
+            >>> s1 = bpd.Series({'falcon': np.nan, 'eagle': 160.0})
+            >>> s2 = bpd.Series({'eagle': 200.0, 'duck': 30.0})
+            >>> s1.combine_first(s2)
+            falcon     <NA>
+            eagle     160.0
+            duck       30.0
+            dtype: Float64
+
+        Args:
+            other (Series):
+                The value(s) to be used for filling null values.
+
+        Returns:
+            Series: The result of combining the provided Series with the other object.
+        """
+        raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
+
+    def update(self, other) -> None:
+        """
+        Modify Series in place using values from passed Series.
+
+        Uses non-NA values from passed Series to make updates. Aligns
+        on index.
+
+        **Examples:**
+            >>> import bigframes.pandas as bpd
+            >>> import pandas as pd
+            >>> import numpy as np
+            >>> bpd.options.display.progress_bar = None
+
+            >>> s = bpd.Series([1, 2, 3])
+            >>> s.update(bpd.Series([4, 5, 6]))
+            >>> s
+            0    4
+            1    5
+            2    6
+            dtype: Int64
+
+            >>> s = bpd.Series(['a', 'b', 'c'])
+            >>> s.update(bpd.Series(['d', 'e'], index=[0, 2]))
+            >>> s
+            0    d
+            1    b
+            2    e
+            dtype: string
+
+            >>> s = bpd.Series([1, 2, 3])
+            >>> s.update(bpd.Series([4, 5, 6, 7, 8]))
+            >>> s
+            0    4
+            1    5
+            2    6
+            dtype: Int64
+
+            If ``other`` contains NaNs the corresponding values are not updated
+            in the original Series.
+
+            >>> s = bpd.Series([1, 2, 3])
+            >>> s.update(bpd.Series([4, np.nan, 6], dtype=pd.Int64Dtype()))
+            >>> s
+            0    4
+            1    2
+            2    6
+            dtype: Int64
+
+            ``other`` can also be a non-Series object type
+            that is coercible into a Series
+
+            >>> s = bpd.Series([1, 2, 3])
+            >>> s.update([4, np.nan, 6])
+            >>> s
+            0    4.0
+            1    2.0
+            2    6.0
+            dtype: Float64
+
+            >>> s = bpd.Series([1, 2, 3])
+            >>> s.update({1: 9})
+            >>> s
+            0    1
+            1    9
+            2    3
+            dtype: Int64
+
+        Args:
+            other (Series, or object coercible into Series)
+        """
+        raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
+
     def all(
         self,
     ):
         """
         Return whether all elements are True, potentially over an axis.
 
         Returns True unless there at least one element within a Series or along a
@@ -2832,15 +3398,15 @@
         Returns:
             DataFrame: Unstacked Series.
         """
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
 
     def argmax(self):
         """
-        Return int position of the smallest value in the Series.
+        Return int position of the smallest value in the series.
 
         If the minimum is achieved in multiple locations, the first row position is returned.
 
         **Examples:**
 
             >>> import bigframes.pandas as bpd
             >>> bpd.options.display.progress_bar = None
@@ -3304,23 +3870,56 @@
         """
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
 
     @property
     def iat(self):
         """Access a single value for a row/column pair by integer position.
 
+        **Examples:**
+
+            >>> import bigframes.pandas as bpd
+            >>> s = bpd.Series(bpd.Series([1, 2, 3]))
+            >>> bpd.options.display.progress_bar = None
+            >>> s
+            0    1
+            1    2
+            2    3
+            dtype: Int64
+
+        Get value at specified row number
+
+            >>> s.iat[1]
+            2
+
         Returns:
             bigframes.core.indexers.IatSeriesIndexer: Indexers object.
         """
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
 
     @property
     def at(self):
         """Access a single value for a row/column label pair.
 
+        **Examples:**
+
+            >>> import bigframes.pandas as bpd
+            >>> s = bpd.Series([1, 2, 3], index=['A', 'B', 'C'])
+            >>> bpd.options.display.progress_bar = None
+            >>> s
+            A    1
+            B    2
+            C    3
+            dtype: Int64
+
+        Get value at specified row label
+
+            >>> s.at['B']
+            2
+
+
         Returns:
             bigframes.core.indexers.AtSeriesIndexer: Indexers object.
         """
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
 
     @property
     def values(self):
@@ -3365,7 +3964,176 @@
             >>> idx.size
             3
 
         Returns:
             int: Return the number of elements in the underlying data.
         """
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
+
+    def __array__(self, dtype=None) -> numpy.ndarray:
+        """
+        Returns the values as NumPy array.
+
+        Equivalent to `Series.to_numpy(dtype)`.
+
+        Users should not call this directly. Rather, it is invoked by
+        `numpy.array` and `numpy.asarray`.
+
+        **Examples:**
+
+            >>> import bigframes.pandas as bpd
+            >>> bpd.options.display.progress_bar = None
+            >>> import numpy as np
+
+            >>> ser = bpd.Series([1, 2, 3])
+
+            >>> np.asarray(ser)
+            array([1, 2, 3])
+
+        Args:
+            dtype (str or numpy.dtype, optional):
+                The dtype to use for the resulting NumPy array. By default,
+                the dtype is inferred from the data.
+
+        Returns:
+            numpy.ndarray:
+                The values in the series converted to a `numpy.ndarray` with the
+                specified dtype.
+        """
+        raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
+
+    def __len__(self):
+        """Returns number of values in the Series, serves `len` operator.
+
+        **Examples:**
+
+            >>> import bigframes.pandas as bpd
+            >>> bpd.options.display.progress_bar = None
+
+            >>> s = bpd.Series([1, 2, 3])
+            >>> len(s)
+            3
+        """
+        raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
+
+    def __invert__(self):
+        """
+        Returns the logical inversion (binary NOT) of the Series, element-wise
+        using operator `~`.
+
+        **Examples:**
+
+            >>> import bigframes.pandas as bpd
+            >>> bpd.options.display.progress_bar = None
+
+            >>> ser = bpd.Series([True, False, True])
+            >>> ~ser
+            0    False
+            1     True
+            2    False
+            dtype: boolean
+
+        Returns:
+            Series: The inverted values in the series.
+        """
+        raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
+
+    def __and__(self, other):
+        """Get bitwise AND of Series and other, element-wise, using operator `&`.
+
+        **Examples:**
+
+            >>> import bigframes.pandas as bpd
+            >>> bpd.options.display.progress_bar = None
+
+            >>> s = bpd.Series([0, 1, 2, 3])
+
+        You can operate with a scalar.
+
+            >>> s & 6
+            0    0
+            1    0
+            2    2
+            3    2
+            dtype: Int64
+
+        You can operate with another Series.
+
+            >>> s1 = bpd.Series([5, 6, 7, 8])
+            >>> s & s1
+            0    0
+            1    0
+            2    2
+            3    0
+            dtype: Int64
+
+        Args:
+            other (scalar or Series):
+                Object to bitwise AND with the Series.
+
+        Returns:
+            Series: The result of the operation.
+        """
+        raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
+
+    def __or__(self, other):
+        """Get bitwise OR of Series and other, element-wise, using operator `|`.
+
+        **Examples:**
+
+            >>> import bigframes.pandas as bpd
+            >>> bpd.options.display.progress_bar = None
+
+            >>> s = bpd.Series([0, 1, 2, 3])
+
+        You can operate with a scalar.
+
+            >>> s | 6
+            0    6
+            1    7
+            2    6
+            3    7
+            dtype: Int64
+
+        You can operate with another Series.
+
+            >>> s1 = bpd.Series([5, 6, 7, 8])
+            >>> s | s1
+            0     5
+            1     7
+            2     7
+            3    11
+            dtype: Int64
+
+        Args:
+            other (scalar or Series):
+                Object to bitwise OR with the Series.
+
+        Returns:
+            Series: The result of the operation.
+        """
+        raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
+
+    def __getitem__(self, indexer):
+        """Gets the specified index from the Series.
+
+        **Examples:**
+
+            >>> import bigframes.pandas as bpd
+            >>> bpd.options.display.progress_bar = None
+
+            >>> s = bpd.Series([15, 30, 45])
+            >>> s[1]
+            30
+            >>> s[0:2]
+            0    15
+            1    30
+            dtype: Int64
+
+        Args:
+            indexer (int or slice):
+                Index or slice of indices.
+
+        Returns:
+            Series or Value: Value(s) at the requested index(es).
+        """
+        raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
```

### Comparing `bigframes-1.1.0/third_party/bigframes_vendored/pandas/core/tools/datetimes.py` & `bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/tools/datetimes.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         BigQuery only supports precision up to microseconds (us). Therefore, when working
         with timestamps that have a finer granularity than microseconds, be aware that
         the additional precision will not be represented in BigQuery.
 
     .. note::
         The format strings for specifying datetime representations in BigQuery and pandas
         are not completely identical. Ensure that the format string provided is compatible
-        with BigQuery.
+        with BigQuery (https://cloud.google.com/bigquery/docs/reference/standard-sql/format-elements#format_elements_date_time).
 
     **Examples:**
 
         >>> import bigframes.pandas as bpd
         >>> bpd.options.display.progress_bar = None
 
     Converting a Scalar to datetime:
```

### Comparing `bigframes-1.1.0/third_party/bigframes_vendored/pandas/core/window/rolling.py` & `bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/window/rolling.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/third_party/bigframes_vendored/pandas/io/common.py` & `bigframes-1.2.0/third_party/bigframes_vendored/pandas/io/common.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/third_party/bigframes_vendored/pandas/io/gbq.py` & `bigframes-1.2.0/third_party/bigframes_vendored/pandas/io/gbq.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/third_party/bigframes_vendored/pandas/io/parquet.py` & `bigframes-1.2.0/third_party/bigframes_vendored/pandas/io/parquet.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/third_party/bigframes_vendored/pandas/io/parsers/readers.py` & `bigframes-1.2.0/third_party/bigframes_vendored/pandas/io/parsers/readers.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/third_party/bigframes_vendored/pandas/io/pickle.py` & `bigframes-1.2.0/third_party/bigframes_vendored/pandas/io/pickle.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/third_party/bigframes_vendored/pandas/pandas/_typing.py` & `bigframes-1.2.0/third_party/bigframes_vendored/pandas/pandas/_typing.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/third_party/bigframes_vendored/pandas/plotting/_core.py` & `bigframes-1.2.0/third_party/bigframes_vendored/pandas/plotting/_core.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/third_party/bigframes_vendored/pandas/util/_exceptions.py` & `bigframes-1.2.0/third_party/bigframes_vendored/pandas/util/_exceptions.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/third_party/bigframes_vendored/pandas/util/_validators.py` & `bigframes-1.2.0/third_party/bigframes_vendored/pandas/util/_validators.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/third_party/bigframes_vendored/sklearn/COPYING` & `bigframes-1.2.0/third_party/bigframes_vendored/sklearn/COPYING`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/third_party/bigframes_vendored/sklearn/base.py` & `bigframes-1.2.0/third_party/bigframes_vendored/sklearn/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,17 +77,17 @@
     """Mixin class for all classifiers."""
 
     _estimator_type = "classifier"
 
     def score(self, X, y):
         """Return the mean accuracy on the given test data and labels.
 
-        In multi-label classification, this is the subset accuracy
-        which is a harsh metric since you require for each sample that
-        each label set be correctly predicted.
+        In multi-label classification, this is the subset accuracy,
+        which is a harsh metric since you require that
+        each label set be correctly predicted for each sample.
 
         .. note::
 
             Output matches that of the BigQuery ML.EVALUTE function.
             See: https://cloud.google.com/bigquery/docs/reference/standard-sql/bigqueryml-syntax-evaluate#classification_models
             for the outputs relevant to this model type.
```

### Comparing `bigframes-1.1.0/third_party/bigframes_vendored/sklearn/cluster/_kmeans.py` & `bigframes-1.2.0/third_party/bigframes_vendored/sklearn/cluster/_kmeans.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/third_party/bigframes_vendored/sklearn/compose/_column_transformer.py` & `bigframes-1.2.0/third_party/bigframes_vendored/sklearn/compose/_column_transformer.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/third_party/bigframes_vendored/sklearn/decomposition/_pca.py` & `bigframes-1.2.0/third_party/bigframes_vendored/sklearn/decomposition/_pca.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 
 class PCA(BaseEstimator, metaclass=ABCMeta):
     """Principal component analysis (PCA).
 
     Args:
         n_components (int, float or None, default None):
-            Number of components to keep. If n_components is not set all
+            Number of components to keep. If n_components is not set, all
             components are kept, n_components = min(n_samples, n_features).
             If 0 < n_components < 1, select the number of components such that the amount of variance that needs to be explained is greater than the percentage specified by n_components.
         svd_solver ("full", "randomized" or "auto", default "auto"):
             The solver to use to calculate the principal components. Details: https://cloud.google.com/bigquery/docs/reference/standard-sql/bigqueryml-syntax-create-pca#pca_solver.
 
     """
 
@@ -71,30 +71,30 @@
         """Predict the closest cluster for each sample in X.
 
         Args:
             X (bigframes.dataframe.DataFrame or bigframes.series.Series):
                 Series or a DataFrame to predict.
 
         Returns:
-            bigframes.dataframe.DataFrame: predicted DataFrames."""
+            bigframes.dataframe.DataFrame: Predicted DataFrames."""
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
 
     @property
     def components_(self):
         """Principal axes in feature space, representing the directions of maximum variance in the data.
 
         Returns:
             bigframes.dataframe.DataFrame: DataFrame of principal components, containing following columns:
                 principal_component_id: An integer that identifies the principal component.
 
                 feature: The column name that contains the feature.
 
                 numerical_value: If feature is numeric, the value of feature for the principal component that principal_component_id identifies. If feature isn't numeric, the value is NULL.
 
-                categorical_value: An list of mappings containing information about categorical features. Each mapping contains the following fields:
+                categorical_value: A list of mappings containing information about categorical features. Each mapping contains the following fields:
                     categorical_value.category: The name of each category.
 
                     categorical_value.value: The value of categorical_value.category for the centroid that centroid_id identifies.
 
             The output contains one row per feature per component.
         """
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
```

### Comparing `bigframes-1.1.0/third_party/bigframes_vendored/sklearn/ensemble/_forest.py` & `bigframes-1.2.0/third_party/bigframes_vendored/sklearn/ensemble/_forest.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/third_party/bigframes_vendored/sklearn/linear_model/_base.py` & `bigframes-1.2.0/third_party/bigframes_vendored/sklearn/linear_model/_base.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/third_party/bigframes_vendored/sklearn/linear_model/_logistic.py` & `bigframes-1.2.0/third_party/bigframes_vendored/sklearn/linear_model/_logistic.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/third_party/bigframes_vendored/sklearn/metrics/_classification.py` & `bigframes-1.2.0/third_party/bigframes_vendored/sklearn/metrics/_classification.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/third_party/bigframes_vendored/sklearn/metrics/_ranking.py` & `bigframes-1.2.0/third_party/bigframes_vendored/sklearn/metrics/_ranking.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/third_party/bigframes_vendored/sklearn/metrics/_regression.py` & `bigframes-1.2.0/third_party/bigframes_vendored/sklearn/metrics/_regression.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/third_party/bigframes_vendored/sklearn/metrics/pairwise.py` & `bigframes-1.2.0/third_party/bigframes_vendored/sklearn/metrics/pairwise.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/third_party/bigframes_vendored/sklearn/pipeline.py` & `bigframes-1.2.0/third_party/bigframes_vendored/sklearn/pipeline.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/third_party/bigframes_vendored/sklearn/preprocessing/_data.py` & `bigframes-1.2.0/third_party/bigframes_vendored/sklearn/preprocessing/_data.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/third_party/bigframes_vendored/sklearn/preprocessing/_discretization.py` & `bigframes-1.2.0/third_party/bigframes_vendored/sklearn/preprocessing/_discretization.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/third_party/bigframes_vendored/sklearn/preprocessing/_encoder.py` & `bigframes-1.2.0/third_party/bigframes_vendored/sklearn/preprocessing/_encoder.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/third_party/bigframes_vendored/sklearn/preprocessing/_label.py` & `bigframes-1.2.0/third_party/bigframes_vendored/sklearn/preprocessing/_label.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/third_party/bigframes_vendored/xgboost/LICENSE` & `bigframes-1.2.0/third_party/bigframes_vendored/xgboost/LICENSE`

 * *Files identical despite different names*

### Comparing `bigframes-1.1.0/third_party/bigframes_vendored/xgboost/sklearn.py` & `bigframes-1.2.0/third_party/bigframes_vendored/xgboost/sklearn.py`

 * *Files identical despite different names*

