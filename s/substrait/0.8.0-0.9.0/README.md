# Comparing `tmp/substrait-0.8.0.tar.gz` & `tmp/substrait-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "substrait-0.8.0.tar", last modified: Tue Nov  7 18:10:53 2023, max compression
+gzip compressed data, was "substrait-0.9.0.tar", last modified: Tue Nov 28 22:23:53 2023, max compression
```

## Comparing `substrait-0.8.0.tar` & `substrait-0.9.0.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 18:10:53.506579 substrait-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2023-11-07 18:10:42.000000 substrait-0.8.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 18:10:53.498579 substrait-0.8.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2023-11-07 18:10:42.000000 substrait-0.8.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 18:10:53.498579 substrait-0.8.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2160 2023-11-07 18:10:42.000000 substrait-0.8.0/.github/workflows/pr_title.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2023-11-07 18:10:42.000000 substrait-0.8.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      782 2023-11-07 18:10:42.000000 substrait-0.8.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2023-11-07 18:10:42.000000 substrait-0.8.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      115 2023-11-07 18:10:42.000000 substrait-0.8.0/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2023-11-07 18:10:42.000000 substrait-0.8.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-11-07 18:10:42.000000 substrait-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5001 2023-11-07 18:10:53.506579 substrait-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4498 2023-11-07 18:10:42.000000 substrait-0.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       65 2023-11-07 18:10:42.000000 substrait-0.8.0/buf.gen.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       42 2023-11-07 18:10:42.000000 substrait-0.8.0/buf.work.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       67 2023-11-07 18:10:42.000000 substrait-0.8.0/buf.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      286 2023-11-07 18:10:42.000000 substrait-0.8.0/environment.yml
--rwxr-xr-x   0 runner    (1001) docker     (127)      966 2023-11-07 18:10:42.000000 substrait-0.8.0/gen_proto.sh
--rw-r--r--   0 runner    (1001) docker     (127)      650 2023-11-07 18:10:42.000000 substrait-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-07 18:10:53.506579 substrait-0.8.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 18:10:53.494579 substrait-0.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 18:10:53.498579 substrait-0.8.0/src/substrait/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2023-11-07 18:10:42.000000 substrait-0.8.0/src/substrait/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-11-07 18:10:53.000000 substrait-0.8.0/src/substrait/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 18:10:53.502580 substrait-0.8.0/src/substrait/extensions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-07 18:10:42.000000 substrait-0.8.0/src/substrait/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      149 2023-11-07 18:10:42.000000 substrait-0.8.0/src/substrait/extensions/extension_types.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      722 2023-11-07 18:10:42.000000 substrait-0.8.0/src/substrait/extensions/functions_aggregate_approx.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      921 2023-11-07 18:10:42.000000 substrait-0.8.0/src/substrait/extensions/functions_aggregate_generic.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    51228 2023-11-07 18:10:42.000000 substrait-0.8.0/src/substrait/extensions/functions_arithmetic.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4467 2023-11-07 18:10:42.000000 substrait-0.8.0/src/substrait/extensions/functions_arithmetic_decimal.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3252 2023-11-07 18:10:42.000000 substrait-0.8.0/src/substrait/extensions/functions_boolean.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6125 2023-11-07 18:10:42.000000 substrait-0.8.0/src/substrait/extensions/functions_comparison.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    23562 2023-11-07 18:10:42.000000 substrait-0.8.0/src/substrait/extensions/functions_datetime.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     7045 2023-11-07 18:10:42.000000 substrait-0.8.0/src/substrait/extensions/functions_geometry.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4213 2023-11-07 18:10:42.000000 substrait-0.8.0/src/substrait/extensions/functions_logarithmic.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    11507 2023-11-07 18:10:42.000000 substrait-0.8.0/src/substrait/extensions/functions_rounding.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      733 2023-11-07 18:10:42.000000 substrait-0.8.0/src/substrait/extensions/functions_set.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    52755 2023-11-07 18:10:42.000000 substrait-0.8.0/src/substrait/extensions/functions_string.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      683 2023-11-07 18:10:42.000000 substrait-0.8.0/src/substrait/extensions/type_variations.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2023-11-07 18:10:42.000000 substrait-0.8.0/src/substrait/extensions/unknown.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 18:10:53.502580 substrait-0.8.0/src/substrait/gen/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-07 18:10:42.000000 substrait-0.8.0/src/substrait/gen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 18:10:53.502580 substrait-0.8.0/src/substrait/gen/proto/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-07 18:10:42.000000 substrait-0.8.0/src/substrait/gen/proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    52166 2023-11-07 18:10:42.000000 substrait-0.8.0/src/substrait/gen/proto/algebra_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2023-11-07 18:10:42.000000 substrait-0.8.0/src/substrait/gen/proto/capabilities_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2268 2023-11-07 18:10:42.000000 substrait-0.8.0/src/substrait/gen/proto/extended_expression_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 18:10:53.502580 substrait-0.8.0/src/substrait/gen/proto/extensions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-07 18:10:42.000000 substrait-0.8.0/src/substrait/gen/proto/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3127 2023-11-07 18:10:42.000000 substrait-0.8.0/src/substrait/gen/proto/extensions/extensions_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     7587 2023-11-07 18:10:42.000000 substrait-0.8.0/src/substrait/gen/proto/function_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     8257 2023-11-07 18:10:42.000000 substrait-0.8.0/src/substrait/gen/proto/parameterized_types_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2023-11-07 18:10:42.000000 substrait-0.8.0/src/substrait/gen/proto/plan_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    10190 2023-11-07 18:10:42.000000 substrait-0.8.0/src/substrait/gen/proto/type_expressions_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    10975 2023-11-07 18:10:42.000000 substrait-0.8.0/src/substrait/gen/proto/type_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 18:10:53.502580 substrait-0.8.0/src/substrait.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5001 2023-11-07 18:10:53.000000 substrait-0.8.0/src/substrait.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2023-11-07 18:10:53.000000 substrait-0.8.0/src/substrait.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-07 18:10:53.000000 substrait-0.8.0/src/substrait.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       88 2023-11-07 18:10:53.000000 substrait-0.8.0/src/substrait.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-11-07 18:10:53.000000 substrait-0.8.0/src/substrait.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 18:10:53.502580 substrait-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      660 2023-11-07 18:10:42.000000 substrait-0.8.0/tests/test_proto.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      668 2023-11-07 18:10:42.000000 substrait-0.8.0/update.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 22:23:53.761477 substrait-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2023-11-28 22:23:41.000000 substrait-0.9.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 22:23:53.753477 substrait-0.9.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2023-11-28 22:23:41.000000 substrait-0.9.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 22:23:53.753477 substrait-0.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2160 2023-11-28 22:23:41.000000 substrait-0.9.0/.github/workflows/pr_title.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2023-11-28 22:23:41.000000 substrait-0.9.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2023-11-28 22:23:41.000000 substrait-0.9.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2023-11-28 22:23:41.000000 substrait-0.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2023-11-28 22:23:41.000000 substrait-0.9.0/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2023-11-28 22:23:41.000000 substrait-0.9.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-11-28 22:23:41.000000 substrait-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5001 2023-11-28 22:23:53.761477 substrait-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4498 2023-11-28 22:23:41.000000 substrait-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2023-11-28 22:23:41.000000 substrait-0.9.0/buf.gen.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2023-11-28 22:23:41.000000 substrait-0.9.0/buf.work.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2023-11-28 22:23:41.000000 substrait-0.9.0/buf.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2023-11-28 22:23:41.000000 substrait-0.9.0/environment.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      966 2023-11-28 22:23:41.000000 substrait-0.9.0/gen_proto.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2023-11-28 22:23:41.000000 substrait-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-28 22:23:53.761477 substrait-0.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 22:23:53.749477 substrait-0.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 22:23:53.753477 substrait-0.9.0/src/substrait/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2023-11-28 22:23:41.000000 substrait-0.9.0/src/substrait/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2023-11-28 22:23:53.000000 substrait-0.9.0/src/substrait/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 22:23:53.757477 substrait-0.9.0/src/substrait/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-28 22:23:41.000000 substrait-0.9.0/src/substrait/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2023-11-28 22:23:41.000000 substrait-0.9.0/src/substrait/extensions/extension_types.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2023-11-28 22:23:41.000000 substrait-0.9.0/src/substrait/extensions/functions_aggregate_approx.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2023-11-28 22:23:41.000000 substrait-0.9.0/src/substrait/extensions/functions_aggregate_generic.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    51228 2023-11-28 22:23:41.000000 substrait-0.9.0/src/substrait/extensions/functions_arithmetic.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4467 2023-11-28 22:23:41.000000 substrait-0.9.0/src/substrait/extensions/functions_arithmetic_decimal.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3252 2023-11-28 22:23:41.000000 substrait-0.9.0/src/substrait/extensions/functions_boolean.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6125 2023-11-28 22:23:41.000000 substrait-0.9.0/src/substrait/extensions/functions_comparison.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    23562 2023-11-28 22:23:41.000000 substrait-0.9.0/src/substrait/extensions/functions_datetime.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     7045 2023-11-28 22:23:41.000000 substrait-0.9.0/src/substrait/extensions/functions_geometry.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4213 2023-11-28 22:23:41.000000 substrait-0.9.0/src/substrait/extensions/functions_logarithmic.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    11507 2023-11-28 22:23:41.000000 substrait-0.9.0/src/substrait/extensions/functions_rounding.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2023-11-28 22:23:41.000000 substrait-0.9.0/src/substrait/extensions/functions_set.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    52755 2023-11-28 22:23:41.000000 substrait-0.9.0/src/substrait/extensions/functions_string.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2023-11-28 22:23:41.000000 substrait-0.9.0/src/substrait/extensions/type_variations.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2023-11-28 22:23:41.000000 substrait-0.9.0/src/substrait/extensions/unknown.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 22:23:53.757477 substrait-0.9.0/src/substrait/gen/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-28 22:23:41.000000 substrait-0.9.0/src/substrait/gen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 22:23:53.761477 substrait-0.9.0/src/substrait/gen/proto/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-28 22:23:41.000000 substrait-0.9.0/src/substrait/gen/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52166 2023-11-28 22:23:41.000000 substrait-0.9.0/src/substrait/gen/proto/algebra_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2023-11-28 22:23:41.000000 substrait-0.9.0/src/substrait/gen/proto/capabilities_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2268 2023-11-28 22:23:41.000000 substrait-0.9.0/src/substrait/gen/proto/extended_expression_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 22:23:53.761477 substrait-0.9.0/src/substrait/gen/proto/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-28 22:23:41.000000 substrait-0.9.0/src/substrait/gen/proto/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3127 2023-11-28 22:23:41.000000 substrait-0.9.0/src/substrait/gen/proto/extensions/extensions_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7587 2023-11-28 22:23:41.000000 substrait-0.9.0/src/substrait/gen/proto/function_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8257 2023-11-28 22:23:41.000000 substrait-0.9.0/src/substrait/gen/proto/parameterized_types_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2023-11-28 22:23:41.000000 substrait-0.9.0/src/substrait/gen/proto/plan_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10190 2023-11-28 22:23:41.000000 substrait-0.9.0/src/substrait/gen/proto/type_expressions_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10975 2023-11-28 22:23:41.000000 substrait-0.9.0/src/substrait/gen/proto/type_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 22:23:53.761477 substrait-0.9.0/src/substrait.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5001 2023-11-28 22:23:53.000000 substrait-0.9.0/src/substrait.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2023-11-28 22:23:53.000000 substrait-0.9.0/src/substrait.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-28 22:23:53.000000 substrait-0.9.0/src/substrait.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2023-11-28 22:23:53.000000 substrait-0.9.0/src/substrait.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2023-11-28 22:23:53.000000 substrait-0.9.0/src/substrait.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 22:23:53.761477 substrait-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2023-11-28 22:23:41.000000 substrait-0.9.0/tests/test_proto.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      668 2023-11-28 22:23:41.000000 substrait-0.9.0/update.sh
```

### Comparing `substrait-0.8.0/.github/workflows/pr_title.yml` & `substrait-0.9.0/.github/workflows/pr_title.yml`

 * *Files identical despite different names*

### Comparing `substrait-0.8.0/.github/workflows/release.yml` & `substrait-0.9.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `substrait-0.8.0/.github/workflows/test.yml` & `substrait-0.9.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `substrait-0.8.0/.gitignore` & `substrait-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `substrait-0.8.0/CONTRIBUTING.md` & `substrait-0.9.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `substrait-0.8.0/LICENSE` & `substrait-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `substrait-0.8.0/PKG-INFO` & `substrait-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: substrait
-Version: 0.8.0
+Version: 0.9.0
 Summary: A python package for Substrait.
 Author-email: Substrait contributors <substrait@googlegroups.com>
 License: Apache-2.0
 Requires-Python: >=3.8.1
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: protobuf>=3.20
```

### Comparing `substrait-0.8.0/README.md` & `substrait-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `substrait-0.8.0/gen_proto.sh` & `substrait-0.9.0/gen_proto.sh`

 * *Files identical despite different names*

### Comparing `substrait-0.8.0/pyproject.toml` & `substrait-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `substrait-0.8.0/src/substrait/extensions/functions_aggregate_approx.yaml` & `substrait-0.9.0/src/substrait/extensions/functions_aggregate_approx.yaml`

 * *Files identical despite different names*

### Comparing `substrait-0.8.0/src/substrait/extensions/functions_aggregate_generic.yaml` & `substrait-0.9.0/src/substrait/extensions/functions_aggregate_generic.yaml`

 * *Files identical despite different names*

### Comparing `substrait-0.8.0/src/substrait/extensions/functions_arithmetic.yaml` & `substrait-0.9.0/src/substrait/extensions/functions_arithmetic.yaml`

 * *Files identical despite different names*

### Comparing `substrait-0.8.0/src/substrait/extensions/functions_arithmetic_decimal.yaml` & `substrait-0.9.0/src/substrait/extensions/functions_arithmetic_decimal.yaml`

 * *Files identical despite different names*

### Comparing `substrait-0.8.0/src/substrait/extensions/functions_boolean.yaml` & `substrait-0.9.0/src/substrait/extensions/functions_boolean.yaml`

 * *Files identical despite different names*

### Comparing `substrait-0.8.0/src/substrait/extensions/functions_comparison.yaml` & `substrait-0.9.0/src/substrait/extensions/functions_comparison.yaml`

 * *Files identical despite different names*

### Comparing `substrait-0.8.0/src/substrait/extensions/functions_datetime.yaml` & `substrait-0.9.0/src/substrait/extensions/functions_datetime.yaml`

 * *Files identical despite different names*

### Comparing `substrait-0.8.0/src/substrait/extensions/functions_geometry.yaml` & `substrait-0.9.0/src/substrait/extensions/functions_geometry.yaml`

 * *Files identical despite different names*

### Comparing `substrait-0.8.0/src/substrait/extensions/functions_logarithmic.yaml` & `substrait-0.9.0/src/substrait/extensions/functions_logarithmic.yaml`

 * *Files identical despite different names*

### Comparing `substrait-0.8.0/src/substrait/extensions/functions_rounding.yaml` & `substrait-0.9.0/src/substrait/extensions/functions_rounding.yaml`

 * *Files identical despite different names*

### Comparing `substrait-0.8.0/src/substrait/extensions/functions_set.yaml` & `substrait-0.9.0/src/substrait/extensions/functions_set.yaml`

 * *Files identical despite different names*

### Comparing `substrait-0.8.0/src/substrait/extensions/functions_string.yaml` & `substrait-0.9.0/src/substrait/extensions/functions_string.yaml`

 * *Files identical despite different names*

### Comparing `substrait-0.8.0/src/substrait/extensions/type_variations.yaml` & `substrait-0.9.0/src/substrait/extensions/type_variations.yaml`

 * *Files identical despite different names*

### Comparing `substrait-0.8.0/src/substrait/extensions/unknown.yaml` & `substrait-0.9.0/src/substrait/extensions/unknown.yaml`

 * *Files identical despite different names*

### Comparing `substrait-0.8.0/src/substrait/gen/proto/algebra_pb2.py` & `substrait-0.9.0/src/substrait/gen/proto/algebra_pb2.py`

 * *Files identical despite different names*

### Comparing `substrait-0.8.0/src/substrait/gen/proto/capabilities_pb2.py` & `substrait-0.9.0/src/substrait/gen/proto/capabilities_pb2.py`

 * *Files identical despite different names*

### Comparing `substrait-0.8.0/src/substrait/gen/proto/extended_expression_pb2.py` & `substrait-0.9.0/src/substrait/gen/proto/extended_expression_pb2.py`

 * *Files identical despite different names*

### Comparing `substrait-0.8.0/src/substrait/gen/proto/extensions/extensions_pb2.py` & `substrait-0.9.0/src/substrait/gen/proto/extensions/extensions_pb2.py`

 * *Files identical despite different names*

### Comparing `substrait-0.8.0/src/substrait/gen/proto/function_pb2.py` & `substrait-0.9.0/src/substrait/gen/proto/function_pb2.py`

 * *Files identical despite different names*

### Comparing `substrait-0.8.0/src/substrait/gen/proto/parameterized_types_pb2.py` & `substrait-0.9.0/src/substrait/gen/proto/parameterized_types_pb2.py`

 * *Files identical despite different names*

### Comparing `substrait-0.8.0/src/substrait/gen/proto/plan_pb2.py` & `substrait-0.9.0/src/substrait/gen/proto/plan_pb2.py`

 * *Files identical despite different names*

### Comparing `substrait-0.8.0/src/substrait/gen/proto/type_expressions_pb2.py` & `substrait-0.9.0/src/substrait/gen/proto/type_expressions_pb2.py`

 * *Files identical despite different names*

### Comparing `substrait-0.8.0/src/substrait/gen/proto/type_pb2.py` & `substrait-0.9.0/src/substrait/gen/proto/type_pb2.py`

 * *Files identical despite different names*

### Comparing `substrait-0.8.0/src/substrait.egg-info/PKG-INFO` & `substrait-0.9.0/src/substrait.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: substrait
-Version: 0.8.0
+Version: 0.9.0
 Summary: A python package for Substrait.
 Author-email: Substrait contributors <substrait@googlegroups.com>
 License: Apache-2.0
 Requires-Python: >=3.8.1
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: protobuf>=3.20
```

### Comparing `substrait-0.8.0/src/substrait.egg-info/SOURCES.txt` & `substrait-0.9.0/src/substrait.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `substrait-0.8.0/tests/test_proto.py` & `substrait-0.9.0/tests/test_proto.py`

 * *Files identical despite different names*

### Comparing `substrait-0.8.0/update.sh` & `substrait-0.9.0/update.sh`

 * *Files identical despite different names*

