# Comparing `tmp/pymc-experimental-0.0.9.tar.gz` & `tmp/pymc_experimental-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymc-experimental-0.0.9.tar", last modified: Fri Jul 28 05:55:01 2023, max compression
+gzip compressed data, was "pymc_experimental-0.1.0.tar", last modified: Tue Apr 16 09:38:41 2024, max compression
```

## Comparing `pymc-experimental-0.0.9.tar` & `pymc_experimental-0.1.0.tar`

### file list

```diff
@@ -1,80 +1,129 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 05:55:01.377128 pymc-experimental-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11720 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-07-28 05:55:01.377128 pymc-experimental-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 05:55:01.369126 pymc-experimental-0.0.9/pymc_experimental/
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 05:55:01.373127 pymc-experimental-0.0.9/pymc_experimental/distributions/
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/distributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/distributions/continuous.py
--rw-r--r--   0 runner    (1001) docker     (123)     6422 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/distributions/discrete.py
--rw-r--r--   0 runner    (1001) docker     (123)     5887 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/distributions/histogram_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 05:55:01.373127 pymc-experimental-0.0.9/pymc_experimental/distributions/multivariate/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/distributions/multivariate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15199 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/distributions/multivariate/r2d2m2cp.py
--rw-r--r--   0 runner    (1001) docker     (123)     9140 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/distributions/timeseries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 05:55:01.373127 pymc-experimental-0.0.9/pymc_experimental/gp/
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/gp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/gp/latent_approx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 05:55:01.373127 pymc-experimental-0.0.9/pymc_experimental/inference/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/inference/fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/inference/pathfinder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/linearmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)    19757 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/marginal_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    26219 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/model_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 05:55:01.373127 pymc-experimental-0.0.9/pymc_experimental/model_transform/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/model_transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/model_transform/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     7241 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/model_transform/conditioning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 05:55:01.373127 pymc-experimental-0.0.9/pymc_experimental/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/preprocessing/standard_scaler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 05:55:01.377128 pymc-experimental-0.0.9/pymc_experimental/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 05:55:01.377128 pymc-experimental-0.0.9/pymc_experimental/tests/distributions/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/tests/distributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/tests/distributions/test_continuous.py
--rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/tests/distributions/test_discrete.py
--rw-r--r--   0 runner    (1001) docker     (123)     7496 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/tests/distributions/test_discrete_markov_chain.py
--rw-r--r--   0 runner    (1001) docker     (123)     9844 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/tests/distributions/test_multivariate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 05:55:01.377128 pymc-experimental-0.0.9/pymc_experimental/tests/model_transform/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/tests/model_transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/tests/model_transform/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/tests/model_transform/test_conditioning.py
--rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/tests/test_histogram_approximation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5863 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/tests/test_linearmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)    13951 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/tests/test_marginal_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8223 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/tests/test_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/tests/test_pathfinder.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/tests/test_pivoted_cholesky.py
--rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/tests/test_prior_from_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/tests/test_splines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 05:55:01.377128 pymc-experimental-0.0.9/pymc_experimental/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13097 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/tests/utils/test_model_fgraph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 05:55:01.377128 pymc-experimental-0.0.9/pymc_experimental/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10096 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/utils/linear_cg.py
--rw-r--r--   0 runner    (1001) docker     (123)    14049 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/utils/model_fgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/utils/pivoted_cholesky.py
--rw-r--r--   0 runner    (1001) docker     (123)     6889 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/utils/prior.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/utils/pytensorf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/utils/spline.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/version.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 05:55:01.373127 pymc-experimental-0.0.9/pymc_experimental.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-07-28 05:55:01.000000 pymc-experimental-0.0.9/pymc_experimental.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-07-28 05:55:01.000000 pymc-experimental-0.0.9/pymc_experimental.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 05:55:01.000000 pymc-experimental-0.0.9/pymc_experimental.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-28 05:55:01.000000 pymc-experimental-0.0.9/pymc_experimental.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-28 05:55:01.000000 pymc-experimental-0.0.9/pymc_experimental.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-28 05:55:01.377128 pymc-experimental-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:38:41.757766 pymc_experimental-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-04-16 09:38:37.000000 pymc_experimental-0.1.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-16 09:38:37.000000 pymc_experimental-0.1.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11720 2024-04-16 09:38:37.000000 pymc_experimental-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-16 09:38:37.000000 pymc_experimental-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-04-16 09:38:41.757766 pymc_experimental-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3322 2024-04-16 09:38:37.000000 pymc_experimental-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:38:41.737766 pymc_experimental-0.1.0/pymc_experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:38:41.737766 pymc_experimental-0.1.0/pymc_experimental/distributions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/distributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11327 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/distributions/continuous.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13047 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/distributions/discrete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5847 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/distributions/histogram_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:38:41.737766 pymc_experimental-0.1.0/pymc_experimental/distributions/multivariate/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/distributions/multivariate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16125 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/distributions/multivariate/r2d2m2cp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9390 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/distributions/timeseries.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:38:41.741766 pymc_experimental-0.1.0/pymc_experimental/gp/
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/gp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6687 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/gp/latent_approx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:38:41.741766 pymc_experimental-0.1.0/pymc_experimental/inference/
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/inference/fit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4201 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/inference/pathfinder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:38:41.741766 pymc_experimental-0.1.0/pymc_experimental/inference/smc/
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/inference/smc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15185 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/inference/smc/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/linearmodel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:38:41.741766 pymc_experimental-0.1.0/pymc_experimental/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34367 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/model/marginal_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/model/model_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:38:41.741766 pymc_experimental-0.1.0/pymc_experimental/model/transforms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/model/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11205 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/model/transforms/autoreparam.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26390 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/model_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:38:41.741766 pymc_experimental-0.1.0/pymc_experimental/model_transform/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/model_transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/model_transform/conditioning.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:38:41.741766 pymc_experimental-0.1.0/pymc_experimental/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/preprocessing/standard_scaler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:38:41.741766 pymc_experimental-0.1.0/pymc_experimental/statespace/
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/statespace/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:38:41.741766 pymc_experimental-0.1.0/pymc_experimental/statespace/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/statespace/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18568 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/statespace/core/representation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71855 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/statespace/core/statespace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:38:41.745766 pymc_experimental-0.1.0/pymc_experimental/statespace/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/statespace/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11574 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/statespace/filters/distributions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34917 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/statespace/filters/kalman_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4372 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/statespace/filters/kalman_smoother.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/statespace/filters/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:38:41.745766 pymc_experimental-0.1.0/pymc_experimental/statespace/models/
+-rw-r--r--   0 runner    (1001) docker     (127)    21602 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/statespace/models/SARIMAX.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15987 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/statespace/models/VARMAX.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/statespace/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62197 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/statespace/models/structural.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15381 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/statespace/models/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:38:41.745766 pymc_experimental-0.1.0/pymc_experimental/statespace/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/statespace/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/statespace/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/statespace/utils/coord_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5700 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/statespace/utils/data_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:38:41.749766 pymc_experimental-0.1.0/pymc_experimental/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:38:41.749766 pymc_experimental-0.1.0/pymc_experimental/tests/distributions/
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/tests/distributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5482 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/tests/distributions/test_continuous.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7781 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/tests/distributions/test_discrete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7881 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/tests/distributions/test_discrete_markov_chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10458 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/tests/distributions/test_multivariate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:38:41.749766 pymc_experimental-0.1.0/pymc_experimental/tests/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/tests/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26892 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/tests/model/test_marginal_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/tests/model/test_model_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:38:41.749766 pymc_experimental-0.1.0/pymc_experimental/tests/model_transform/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/tests/model_transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/tests/model_transform/test_conditioning.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:38:41.753766 pymc_experimental-0.1.0/pymc_experimental/tests/statespace/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/tests/statespace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13004 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/tests/statespace/test_SARIMAX.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6393 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/tests/statespace/test_VARMAX.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/tests/statespace/test_coord_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7310 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/tests/statespace/test_distributions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11438 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/tests/statespace/test_kalman_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6264 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/tests/statespace/test_representation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11848 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/tests/statespace/test_statespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28112 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/tests/statespace/test_structural.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:38:41.753766 pymc_experimental-0.1.0/pymc_experimental/tests/statespace/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/tests/statespace/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/tests/statespace/utilities/shared_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/tests/statespace/utilities/statsmodel_local_level.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9037 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/tests/statespace/utilities/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7183 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/tests/test_blackjax_smc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4680 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/tests/test_histogram_approximation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/tests/test_linearmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11288 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/tests/test_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/tests/test_pathfinder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/tests/test_pivoted_cholesky.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/tests/test_prior_from_trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/tests/test_splines.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:38:41.753766 pymc_experimental-0.1.0/pymc_experimental/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/tests/utils/test_model_fgraph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:38:41.753766 pymc_experimental-0.1.0/pymc_experimental/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10094 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/utils/linear_cg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/utils/model_fgraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/utils/pivoted_cholesky.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6875 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/utils/prior.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/utils/pytensorf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/utils/spline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pymc_experimental/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:38:41.753766 pymc_experimental-0.1.0/pymc_experimental.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-04-16 09:38:41.000000 pymc_experimental-0.1.0/pymc_experimental.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4465 2024-04-16 09:38:41.000000 pymc_experimental-0.1.0/pymc_experimental.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 09:38:41.000000 pymc_experimental-0.1.0/pymc_experimental.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-16 09:38:41.000000 pymc_experimental-0.1.0/pymc_experimental.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-16 09:38:41.000000 pymc_experimental-0.1.0/pymc_experimental.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 09:38:41.757766 pymc_experimental-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-04-16 09:38:38.000000 pymc_experimental-0.1.0/setup.py
```

### Comparing `pymc-experimental-0.0.9/CODE_OF_CONDUCT.md` & `pymc_experimental-0.1.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.9/LICENSE` & `pymc_experimental-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.9/PKG-INFO` & `pymc_experimental-0.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,43 @@
 Metadata-Version: 2.1
 Name: pymc-experimental
-Version: 0.0.9
+Version: 0.1.0
 Summary: A home for new additions to PyMC, which may include unusual probability distribitions, advanced model fitting algorithms, or any code that may be inappropriate to include in the pymc repository, but may want to be made available to users.
 Home-page: http://github.com/pymc-devs/pymc-experimental
 Maintainer: PyMC Developers
 Maintainer-email: pymc.devs@gmail.com
 License: Apache License, Version 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
-Provides-Extra: dask_histogram
+License-File: LICENSE
+Requires-Dist: pymc>=5.13.0
+Requires-Dist: scikit-learn
+Provides-Extra: dask-histogram
+Requires-Dist: dask[complete]; extra == "dask-histogram"
+Requires-Dist: xhistogram; extra == "dask-histogram"
 Provides-Extra: histogram
+Requires-Dist: xhistogram; extra == "histogram"
 Provides-Extra: complete
+Requires-Dist: dask[complete]; extra == "complete"
+Requires-Dist: xhistogram; extra == "complete"
 Provides-Extra: dev
-License-File: LICENSE
+Requires-Dist: dask[all]; extra == "dev"
+Requires-Dist: blackjax; extra == "dev"
+Requires-Dist: statsmodels; extra == "dev"
 
 # Welcome to `pymc-experimental`
 <a href="https://gitpod.io/#https://github.com/pymc-devs/pymc-experimental">
   <img
     src="https://img.shields.io/badge/Contribute%20with-Gitpod-908a85?logo=gitpod"
     alt="Contribute with Gitpod"
   />
```

#### html2text {}

```diff
@@ -1,57 +1,62 @@
-Metadata-Version: 2.1 Name: pymc-experimental Version: 0.0.9 Summary: A home
+Metadata-Version: 2.1 Name: pymc-experimental Version: 0.1.0 Summary: A home
 for new additions to PyMC, which may include unusual probability distribitions,
 advanced model fitting algorithms, or any code that may be inappropriate to
 include in the pymc repository, but may want to be made available to users.
 Home-page: http://github.com/pymc-devs/pymc-experimental Maintainer: PyMC
 Developers Maintainer-email: pymc.devs@gmail.com License: Apache License,
 Version 2.0 Classifier: Development Status :: 5 - Production/Stable Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
-Approved :: Apache Software License Classifier: Intended Audience :: Science/
-Research Classifier: Topic :: Scientific/Engineering Classifier: Topic ::
-Scientific/Engineering :: Mathematics Classifier: Operating System :: OS
-Independent Requires-Python: >=3.8 Description-Content-Type: text/markdown
-Provides-Extra: dask_histogram Provides-Extra: histogram Provides-Extra:
-complete Provides-Extra: dev License-File: LICENSE # Welcome to `pymc-
-experimental` _[_C_o_n_t_r_i_b_u_t_e_ _w_i_t_h_ _G_i_t_p_o_d_][Codecov Badge]As PyMC continues to
-mature and expand its functionality to accommodate more domains of application,
-we increasingly see cutting-edge methodologies, highly specialized statistical
-distributions, and complex models appear. While this adds to the functionality
-and relevance of the project, it can also introduce instability and impose a
-burden on testing and quality control. To reduce the burden on the main `pymc`
-repository, this `pymc-experimental` repository can become the aggregator and
-testing ground for new additions to PyMC. This may include unusual probability
-distributions, advanced model fitting algorithms, innovative yet not fully
-tested methods or any code that may be inappropriate to include in the `pymc`
-repository, but may want to be made available to users. The `pymc-experimental`
-repository can be understood as the first step in the PyMC development
-pipeline, where all novel code is introduced until it is obvious that it
-belongs in the main repository. We hope that this organization improves the
-stability and streamlines the testing overhead of the `pymc` repository, while
-allowing users and developers to test and evaluate cutting-edge methods and not
-yet fully mature features. `pymc-experimental` would be designed to mirror the
-namespaces in `pymc` to make usage and migration as easy as possible. For
-example, a `ParabolicFractal` distribution could be used analogously to those
-in `pymc`: ```python import pymc as pm import pymc_experimental as pmx with
-pm.Model(): alpha = pmx.ParabolicFractal('alpha', b=1, c=1) ... ``` ##
-Questions ### What belongs in `pymc-experimental`? - newly-implemented
-statistical methods, for example step methods or model construction helpers -
-distributions that are tricky to sample from or test - infrequently-used
-fitting methods or distributions - any code that requires additional
-optimization before it can be used in practice ### What does not belong in
-`pymc-experimental`? - Case studies - Implementations that cannot be applied
-generically, for example because they are tied to variables from a toy example
-### Should there be more than one add-on repository? Since there is a lot of
-code that we may not want in the main repository, does it make sense to have
-more than one additional repository? For example, `pymc-experimental` may just
-include methods that are not fully developed, tested and trusted, while code
-that is known to work well and has adequate test coverage, but is still too
-specialized to become part of `pymc` could reside in a `pymc-extras` (or
-similar) repository. ### Unanswered questions & ToDos This project is still
-young and many things have not been answered or implemented. Please get
-involved! * What are guidelines for organizing submodules? * Proposal: No
-default imports of WIP/unstable submodules. By importing manually we can avoid
-breaking the package if a submodule breaks, for example because of an updated
-dependency.
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
+Classifier: License :: OSI Approved :: Apache Software License Classifier:
+Intended Audience :: Science/Research Classifier: Topic :: Scientific/
+Engineering Classifier: Topic :: Scientific/Engineering :: Mathematics
+Classifier: Operating System :: OS Independent Requires-Python: >=3.10
+Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+pymc>=5.13.0 Requires-Dist: scikit-learn Provides-Extra: dask-histogram
+Requires-Dist: dask[complete]; extra == "dask-histogram" Requires-Dist:
+xhistogram; extra == "dask-histogram" Provides-Extra: histogram Requires-Dist:
+xhistogram; extra == "histogram" Provides-Extra: complete Requires-Dist: dask
+[complete]; extra == "complete" Requires-Dist: xhistogram; extra == "complete"
+Provides-Extra: dev Requires-Dist: dask[all]; extra == "dev" Requires-Dist:
+blackjax; extra == "dev" Requires-Dist: statsmodels; extra == "dev" # Welcome
+to `pymc-experimental` _[_C_o_n_t_r_i_b_u_t_e_ _w_i_t_h_ _G_i_t_p_o_d_][Codecov Badge]As PyMC continues
+to mature and expand its functionality to accommodate more domains of
+application, we increasingly see cutting-edge methodologies, highly specialized
+statistical distributions, and complex models appear. While this adds to the
+functionality and relevance of the project, it can also introduce instability
+and impose a burden on testing and quality control. To reduce the burden on the
+main `pymc` repository, this `pymc-experimental` repository can become the
+aggregator and testing ground for new additions to PyMC. This may include
+unusual probability distributions, advanced model fitting algorithms,
+innovative yet not fully tested methods or any code that may be inappropriate
+to include in the `pymc` repository, but may want to be made available to
+users. The `pymc-experimental` repository can be understood as the first step
+in the PyMC development pipeline, where all novel code is introduced until it
+is obvious that it belongs in the main repository. We hope that this
+organization improves the stability and streamlines the testing overhead of the
+`pymc` repository, while allowing users and developers to test and evaluate
+cutting-edge methods and not yet fully mature features. `pymc-experimental`
+would be designed to mirror the namespaces in `pymc` to make usage and
+migration as easy as possible. For example, a `ParabolicFractal` distribution
+could be used analogously to those in `pymc`: ```python import pymc as pm
+import pymc_experimental as pmx with pm.Model(): alpha = pmx.ParabolicFractal
+('alpha', b=1, c=1) ... ``` ## Questions ### What belongs in `pymc-
+experimental`? - newly-implemented statistical methods, for example step
+methods or model construction helpers - distributions that are tricky to sample
+from or test - infrequently-used fitting methods or distributions - any code
+that requires additional optimization before it can be used in practice ###
+What does not belong in `pymc-experimental`? - Case studies - Implementations
+that cannot be applied generically, for example because they are tied to
+variables from a toy example ### Should there be more than one add-on
+repository? Since there is a lot of code that we may not want in the main
+repository, does it make sense to have more than one additional repository? For
+example, `pymc-experimental` may just include methods that are not fully
+developed, tested and trusted, while code that is known to work well and has
+adequate test coverage, but is still too specialized to become part of `pymc`
+could reside in a `pymc-extras` (or similar) repository. ### Unanswered
+questions & ToDos This project is still young and many things have not been
+answered or implemented. Please get involved! * What are guidelines for
+organizing submodules? * Proposal: No default imports of WIP/unstable
+submodules. By importing manually we can avoid breaking the package if a
+submodule breaks, for example because of an updated dependency.
```

### Comparing `pymc-experimental-0.0.9/README.md` & `pymc_experimental-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.9/pymc_experimental/__init__.py` & `pymc_experimental-0.1.0/pymc_experimental/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -19,10 +19,11 @@
 
 if not logging.root.handlers:
     _log.setLevel(logging.INFO)
     if len(_log.handlers) == 0:
         handler = logging.StreamHandler()
         _log.addHandler(handler)
 
-from pymc_experimental import distributions, gp, utils
+from pymc_experimental import distributions, gp, statespace, utils
 from pymc_experimental.inference.fit import fit
-from pymc_experimental.marginal_model import MarginalModel
+from pymc_experimental.model.marginal_model import MarginalModel
+from pymc_experimental.model.model_api import as_model
```

### Comparing `pymc-experimental-0.0.9/pymc_experimental/distributions/__init__.py` & `pymc_experimental-0.1.0/pymc_experimental/distributions/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,20 +13,28 @@
 #   limitations under the License.
 
 # coding: utf-8
 """
 Experimental probability distributions for stochastic nodes in PyMC.
 """
 
-from pymc_experimental.distributions.continuous import GenExtreme
-from pymc_experimental.distributions.discrete import GeneralizedPoisson
+from pymc_experimental.distributions.continuous import Chi, GenExtreme, Maxwell
+from pymc_experimental.distributions.discrete import (
+    BetaNegativeBinomial,
+    GeneralizedPoisson,
+    Skellam,
+)
 from pymc_experimental.distributions.histogram_utils import histogram_approximation
 from pymc_experimental.distributions.multivariate import R2D2M2CP
 from pymc_experimental.distributions.timeseries import DiscreteMarkovChain
 
 __all__ = [
+    "BetaNegativeBinomial",
     "DiscreteMarkovChain",
     "GeneralizedPoisson",
     "GenExtreme",
     "R2D2M2CP",
+    "Skellam",
     "histogram_approximation",
+    "Chi",
+    "Maxwell",
 ]
```

### Comparing `pymc-experimental-0.0.9/pymc_experimental/distributions/continuous.py` & `pymc_experimental-0.1.0/pymc_experimental/distributions/continuous.py`

 * *Files 24% similar despite different names*

```diff
@@ -19,20 +19,23 @@
 The imports from pymc are not fully replicated here: add imports as necessary.
 """
 
 from typing import List, Tuple, Union
 
 import numpy as np
 import pytensor.tensor as pt
+from pymc import ChiSquared, CustomDist
+from pymc.distributions import transforms
 from pymc.distributions.dist_math import check_parameters
 from pymc.distributions.distribution import Continuous
 from pymc.distributions.shape_utils import rv_size_is_none
+from pymc.logprob.utils import CheckParameterValue
 from pymc.pytensorf import floatX
 from pytensor.tensor.random.op import RandomVariable
-from pytensor.tensor.var import TensorVariable
+from pytensor.tensor.variable import TensorVariable
 from scipy import stats
 
 
 class GenExtremeRV(RandomVariable):
     name: str = "Generalized Extreme Value"
     ndim_supp: int = 0
     ndims_params: List[int] = [0, 0, 0]
@@ -204,15 +207,147 @@
 
         logc = pt.switch(1 + xi * (value - mu) / sigma > 0, logc_expression, -np.inf)
 
         return check_parameters(
             logc, sigma > 0, pt.and_(xi > -1, xi < 1), msg="sigma > 0 or -1 < xi < 1"
         )
 
-    def moment(rv, size, mu, sigma, xi):
+    def support_point(rv, size, mu, sigma, xi):
         r"""
         Using the mode, as the mean can be infinite when :math:`\xi > 1`
         """
         mode = pt.switch(pt.isclose(xi, 0), mu, mu + sigma * (pt.pow(1 + xi, -xi) - 1) / xi)
         if not rv_size_is_none(size):
             mode = pt.full(size, mode)
         return mode
+
+
+class Chi:
+    r"""
+    :math:`\chi` log-likelihood.
+
+    The pdf of this distribution is
+
+    .. math::
+
+       f(x \mid \nu) = \frac{x^{\nu - 1}e^{-x^2/2}}{2^{\nu/2 - 1}\Gamma(\nu/2)}
+
+    .. plot::
+        :context: close-figs
+
+        import matplotlib.pyplot as plt
+        import numpy as np
+        import scipy.stats as st
+        import arviz as az
+        plt.style.use('arviz-darkgrid')
+        x = np.linspace(0, 10, 200)
+        for df in [1, 2, 3, 6, 9]:
+            pdf = st.chi.pdf(x, df)
+            plt.plot(x, pdf, label=r'$\nu$ = {}'.format(df))
+        plt.xlabel('x', fontsize=12)
+        plt.ylabel('f(x)', fontsize=12)
+        plt.legend(loc=1)
+        plt.show()
+
+    ========  =========================================================================
+    Support   :math:`x \in [0, \infty)`
+    Mean      :math:`\sqrt{2}\frac{\Gamma((\nu + 1)/2)}{\Gamma(\nu/2)}`
+    Variance  :math:`\nu - 2\left(\frac{\Gamma((\nu + 1)/2)}{\Gamma(\nu/2)}\right)^2`
+    ========  =========================================================================
+
+    Parameters
+    ----------
+    nu : tensor_like of float
+        Degrees of freedom (nu > 0).
+
+    Examples
+    --------
+    .. code-block:: python
+        import pymc as pm
+        from pymc_experimental.distributions import Chi
+
+        with pm.Model():
+            x = Chi('x', nu=1)
+    """
+
+    @staticmethod
+    def chi_dist(nu: TensorVariable, size: TensorVariable) -> TensorVariable:
+        return pt.math.sqrt(ChiSquared.dist(nu=nu, size=size))
+
+    def __new__(cls, name, nu, **kwargs):
+        if "observed" not in kwargs:
+            kwargs.setdefault("transform", transforms.log)
+        return CustomDist(name, nu, dist=cls.chi_dist, class_name="Chi", **kwargs)
+
+    @classmethod
+    def dist(cls, nu, **kwargs):
+        return CustomDist.dist(nu, dist=cls.chi_dist, class_name="Chi", **kwargs)
+
+
+class Maxwell:
+    R"""
+    The Maxwell-Boltzmann distribution
+
+    The pdf of this distribution is
+
+    .. math::
+
+       f(x \mid a) = {\displaystyle {\sqrt {\frac {2}{\pi }}}\,{\frac {x^{2}}{a^{3}}}\,\exp \left({\frac {-x^{2}}{2a^{2}}}\right)}
+
+    Read more about it on `Wikipedia <https://en.wikipedia.org/wiki/Maxwell%E2%80%93Boltzmann_distribution>`_
+
+    .. plot::
+        :context: close-figs
+
+        import matplotlib.pyplot as plt
+        import numpy as np
+        import scipy.stats as st
+        import arviz as az
+        plt.style.use('arviz-darkgrid')
+        x = np.linspace(0, 20, 200)
+        for a in [1, 2, 5]:
+            pdf = st.maxwell.pdf(x, scale=a)
+            plt.plot(x, pdf, label=r'$a$ = {}'.format(a))
+        plt.xlabel('x', fontsize=12)
+        plt.ylabel('f(x)', fontsize=12)
+        plt.legend(loc=1)
+        plt.show()
+
+    ========  =========================================================================
+    Support   :math:`x \in (0, \infty)`
+    Mean      :math:`2a \sqrt{\frac{2}{\pi}}`
+    Variance  :math:`\frac{a^2(3 \pi - 8)}{\pi}`
+    ========  =========================================================================
+
+    Parameters
+    ----------
+    a : tensor_like of float
+        Scale parameter (a > 0).
+
+    """
+
+    @staticmethod
+    def maxwell_dist(a: TensorVariable, size: TensorVariable) -> TensorVariable:
+        if rv_size_is_none(size):
+            size = a.shape
+
+        a = CheckParameterValue("a > 0")(a, pt.all(pt.gt(a, 0)))
+
+        return Chi.dist(nu=3, size=size) * a
+
+    def __new__(cls, name, a, **kwargs):
+        return CustomDist(
+            name,
+            a,
+            dist=cls.maxwell_dist,
+            class_name="Maxwell",
+            **kwargs,
+        )
+
+    @classmethod
+    def dist(cls, a, **kwargs):
+        return CustomDist.dist(
+            a,
+            dist=cls.maxwell_dist,
+            class_name="Maxwell",
+            **kwargs,
+        )
```

### Comparing `pymc-experimental-0.0.9/pymc_experimental/distributions/histogram_utils.py` & `pymc_experimental-0.1.0/pymc_experimental/distributions/histogram_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -96,23 +96,23 @@
 def histogram_approximation(name, dist, *, observed, **h_kwargs):
     """Approximate a distribution with a histogram potential.
 
     Parameters
     ----------
     name : str
         Name for the Potential
-    dist : pytensor.tensor.var.TensorVariable
+    dist : TensorVariable
         The output of pm.Distribution.dist()
     observed : ArrayLike
         Observed value to construct a histogram. Histogram is computed over 0th axis.
         Dask is supported.
 
     Returns
     -------
-    pytensor.tensor.var.TensorVariable
+    TensorVariable
         Potential
 
     Examples
     --------
     Discrete variables are reduced to unique repetitions (up to min_count)
 
     >>> import pymc as pm
```

### Comparing `pymc-experimental-0.0.9/pymc_experimental/distributions/multivariate/r2d2m2cp.py` & `pymc_experimental-0.1.0/pymc_experimental/distributions/multivariate/r2d2m2cp.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,31 +9,41 @@
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 
 
-from typing import Sequence, Union
+from collections import namedtuple
+from typing import Sequence, Tuple, Union
 
 import numpy as np
 import pymc as pm
 import pytensor.tensor as pt
 
 __all__ = ["R2D2M2CP"]
 
 
-def _psivar2musigma(psi: pt.TensorVariable, explained_var: pt.TensorVariable, psi_mask):
+def _psivar2musigma(
+    psi: pt.TensorVariable,
+    explained_var: pt.TensorVariable,
+    psi_mask: Union[pt.TensorLike, None],
+) -> Tuple[pt.TensorVariable, pt.TensorVariable]:
+    sign = pt.sign(psi - 0.5)
+    if psi_mask is not None:
+        # any computation might be ignored for ~psi_mask
+        # sign and explained_var are used
+        psi = pt.where(psi_mask, psi, 0.5)
     pi = pt.erfinv(2 * psi - 1)
     f = (1 / (2 * pi**2 + 1)) ** 0.5
     sigma = explained_var**0.5 * f
     mu = sigma * pi * 2**0.5
     if psi_mask is not None:
         return (
-            pt.where(psi_mask, mu, pt.sign(pi) * explained_var**0.5),
+            pt.where(psi_mask, mu, sign * explained_var**0.5),
             pt.where(psi_mask, sigma, 0),
         )
     else:
         return mu, sigma
 
 
 def _R2D2M2CP_beta(
@@ -43,15 +53,15 @@
     r2: pt.TensorVariable,
     phi: pt.TensorVariable,
     psi: pt.TensorVariable,
     *,
     psi_mask,
     dims: Union[str, Sequence[str]],
     centered=False,
-):
+) -> pt.TensorVariable:
     """R2D2M2CP beta prior.
 
     Parameters
     ----------
     name: str
         Name for the distribution
     output_sigma: tensor
@@ -61,15 +71,15 @@
     r2: tensor
         expected R2 for the linear regression
     phi: tensor
         variance weights that sums up to 1
     psi: tensor
         probability of a coefficients to be positive
     """
-    explained_variance = phi * pt.expand_dims(r2 * output_sigma**2, -1)
+    explained_variance = phi * pt.expand_dims(r2 * output_sigma**2, (-1,))
     mu_param, std_param = _psivar2musigma(psi, explained_variance, psi_mask=psi_mask)
     if not centered:
         with pm.Model(name):
             if psi_mask is not None and psi_mask.any():
                 # limit case where some probs are not 1 or 0
                 # setsubtensor is required
                 r_idx = psi_mask.nonzero()
@@ -103,25 +113,33 @@
             # all variables are deterministic
             beta = pm.Deterministic(name, (mu_param / input_sigma), dims=dims)
         else:
             beta = pm.Normal(name, mu_param / input_sigma, std_param / input_sigma, dims=dims)
     return beta
 
 
-def _broadcast_as_dims(*values, dims):
+def _broadcast_as_dims(
+    *values: np.ndarray,
+    dims: Sequence[str],
+) -> Union[Tuple[np.ndarray, ...], np.ndarray]:
     model = pm.modelcontext(None)
     shape = [len(model.coords[d]) for d in dims]
     ret = tuple(np.broadcast_to(v, shape) for v in values)
     # strip output
     if len(values) == 1:
         ret = ret[0]
     return ret
 
 
-def _psi_masked(positive_probs, positive_probs_std, *, dims):
+def _psi_masked(
+    positive_probs: pt.TensorLike,
+    positive_probs_std: pt.TensorLike,
+    *,
+    dims: Sequence[str],
+) -> Tuple[Union[pt.TensorLike, None], pt.TensorVariable]:
     if not (
         isinstance(positive_probs, pt.Constant) and isinstance(positive_probs_std, pt.Constant)
     ):
         raise TypeError(
             "Only constant values for positive_probs and positive_probs_std are accepted"
         )
     positive_probs, positive_probs_std = _broadcast_as_dims(
@@ -148,15 +166,20 @@
         psi = pt.as_tensor(positive_probs)
     else:
         psi = pm.Beta("psi", mu=positive_probs, sigma=positive_probs_std, dims=dims)
         mask = None
     return mask, psi
 
 
-def _psi(positive_probs, positive_probs_std, *, dims):
+def _psi(
+    positive_probs: pt.TensorLike,
+    positive_probs_std: Union[pt.TensorLike, None],
+    *,
+    dims: Sequence[str],
+) -> Tuple[Union[pt.TensorLike, None], pt.TensorVariable]:
     if positive_probs_std is not None:
         mask, psi = _psi_masked(
             positive_probs=pt.as_tensor(positive_probs),
             positive_probs_std=pt.as_tensor(positive_probs_std),
             dims=dims,
         )
     else:
@@ -167,20 +190,20 @@
         mask = np.atleast_1d(~np.bitwise_or(psi == 1, psi == 0))
         if mask.all():
             mask = None
     return mask, psi
 
 
 def _phi(
-    variables_importance,
-    variance_explained,
-    importance_concentration,
+    variables_importance: Union[pt.TensorLike, None],
+    variance_explained: Union[pt.TensorLike, None],
+    importance_concentration: Union[pt.TensorLike, None],
     *,
-    dims,
-):
+    dims: Sequence[str],
+) -> pt.TensorVariable:
     *broadcast_dims, dim = dims
     model = pm.modelcontext(None)
     if variables_importance is not None:
         if variance_explained is not None:
             raise TypeError("Can't use variable importance with variance explained")
         if len(model.coords[dim]) <= 1:
             raise TypeError("Can't use variable importance with less than two variables")
@@ -189,63 +212,65 @@
             variables_importance *= importance_concentration
         return pm.Dirichlet("phi", variables_importance, dims=broadcast_dims + [dim])
     elif variance_explained is not None:
         if len(model.coords[dim]) <= 1:
             raise TypeError("Can't use variance explained with less than two variables")
         phi = pt.as_tensor(variance_explained)
     else:
-        phi = 1 / len(model.coords[dim])
-        phi = _broadcast_as_dims(phi, dims=dims)
+        phi = _broadcast_as_dims(1.0, dims=dims)
     if importance_concentration is not None:
         return pm.Dirichlet("phi", importance_concentration * phi, dims=broadcast_dims + [dim])
     else:
         return phi
 
 
+R2D2M2CPOut = namedtuple("R2D2M2CPOut", ["eps", "beta"])
+
+
 def R2D2M2CP(
-    name,
-    output_sigma,
-    input_sigma,
+    name: str,
+    output_sigma: pt.TensorLike,
+    input_sigma: pt.TensorLike,
     *,
-    dims,
-    r2,
-    variables_importance=None,
-    variance_explained=None,
-    importance_concentration=None,
-    r2_std=None,
-    positive_probs=0.5,
-    positive_probs_std=None,
-    centered=False,
-):
+    dims: Sequence[str],
+    r2: pt.TensorLike,
+    variables_importance: Union[pt.TensorLike, None] = None,
+    variance_explained: Union[pt.TensorLike, None] = None,
+    importance_concentration: Union[pt.TensorLike, None] = None,
+    r2_std: Union[pt.TensorLike, None] = None,
+    positive_probs: Union[pt.TensorLike, None] = 0.5,
+    positive_probs_std: Union[pt.TensorLike, None] = None,
+    centered: bool = False,
+) -> R2D2M2CPOut:
     """R2D2M2CP Prior.
 
     Parameters
     ----------
     name : str
         Name for the distribution
-    output_sigma : tensor
+    output_sigma : Tensor
         Output standard deviation
-    input_sigma : tensor
+    input_sigma : Tensor
         Input standard deviation
     dims : Union[str, Sequence[str]]
         Dims for the distribution
-    r2 : tensor
+    r2 : Tensor
         :math:`R^2` estimate
-    variables_importance : tensor, optional
+    variables_importance : Tensor, optional
         Optional estimate for variables importance, positive, by default None
-    variance_explained : tensor, optional
+    variance_explained : Tensor, optional
         Alternative estimate for variables importance which is point estimate of
         variance explained, should sum up to one, by default None
-    importance_concentration : tensor, optional
+    importance_concentration : Tensor, optional
         Confidence around variance explained or variable importance estimate
-    r2_std : tensor, optional
+    r2_std : Tensor, optional
         Optional uncertainty over :math:`R^2`, by default None
-    positive_probs : tensor, optional
+    positive_probs : Tensor, optional
         Optional probability of variables contribution to be positive, by default 0.5
-    positive_probs_std : tensor, optional
+    positive_probs_std : Tensor, optional
         Optional uncertainty over effect direction probability, by default None
     centered : bool, optional
         Centered or Non-Centered parametrization of the distribution, by default Non-Centered. Advised to check both
 
     Returns
     -------
     residual_sigma, coefficients
@@ -389,17 +414,15 @@
         }
     """
     if not isinstance(dims, (list, tuple)):
         dims = (dims,)
     *broadcast_dims, dim = dims
     input_sigma = pt.as_tensor(input_sigma)
     output_sigma = pt.as_tensor(output_sigma)
-    with pm.Model(name) as model:
-        if not all(isinstance(model.dim_lengths[d], pt.TensorConstant) for d in dims):
-            raise ValueError(f"{dims!r} should be constant length immutable dims")
+    with pm.Model(name):
         if r2_std is not None:
             r2 = pm.Beta("r2", mu=r2, sigma=r2_std, dims=broadcast_dims)
         phi = _phi(
             variables_importance=variables_importance,
             variance_explained=variance_explained,
             importance_concentration=importance_concentration,
             dims=dims,
@@ -416,8 +439,8 @@
         phi,
         psi,
         dims=broadcast_dims + [dim],
         centered=centered,
         psi_mask=mask,
     )
     resid_sigma = (1 - r2) ** 0.5 * output_sigma
-    return resid_sigma, beta
+    return R2D2M2CPOut(resid_sigma, beta)
```

### Comparing `pymc-experimental-0.0.9/pymc_experimental/distributions/timeseries.py` & `pymc_experimental-0.1.0/pymc_experimental/distributions/timeseries.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 import pymc as pm
 import pytensor
 import pytensor.tensor as pt
 from pymc.distributions.dist_math import check_parameters
 from pymc.distributions.distribution import (
     Distribution,
     SymbolicRandomVariable,
-    _moment,
-    moment,
+    _support_point,
+    support_point,
 )
 from pymc.distributions.shape_utils import (
     _change_dist_size,
     change_dist_size,
     get_support_shape_1d,
 )
 from pymc.logprob.abstract import _logprob
 from pymc.logprob.basic import logp
-from pymc.pytensorf import intX
+from pymc.pytensorf import constant_fold, intX
 from pymc.util import check_dist_not_registered
 from pytensor.graph.basic import Node
 from pytensor.tensor import TensorVariable
 from pytensor.tensor.random.op import RandomVariable
 
 
 def _make_outputs_info(n_lags: int, init_dist: Distribution) -> List[Union[Distribution, dict]]:
@@ -198,36 +198,36 @@
         )
 
         (state_next_rng,) = tuple(state_updates.values())
 
         discrete_mc_ = pt.moveaxis(pt.concatenate([init_dist_, markov_chain], axis=0), 0, -1)
 
         discrete_mc_op = DiscreteMarkovChainRV(
-            inputs=[P_, steps_, init_dist_],
+            inputs=[P_, steps_, init_dist_, state_rng],
             outputs=[state_next_rng, discrete_mc_],
             ndim_supp=1,
             n_lags=n_lags,
         )
 
-        discrete_mc = discrete_mc_op(P, steps, init_dist)
+        discrete_mc = discrete_mc_op(P, steps, init_dist, state_rng)
         return discrete_mc
 
 
 @_change_dist_size.register(DiscreteMarkovChainRV)
 def change_mc_size(op, dist, new_size, expand=False):
     if expand:
         old_size = dist.shape[:-1]
         new_size = tuple(new_size) + tuple(old_size)
 
     return DiscreteMarkovChain.rv_op(*dist.owner.inputs[:-1], size=new_size, n_lags=op.n_lags)
 
 
-@_moment.register(DiscreteMarkovChainRV)
+@_support_point.register(DiscreteMarkovChainRV)
 def discrete_mc_moment(op, rv, P, steps, init_dist, state_rng):
-    init_dist_moment = moment(init_dist)
+    init_dist_moment = support_point(init_dist)
     n_lags = op.n_lags
 
     def greedy_transition(*args):
         *states, transition_probs, old_rng = args
         p = transition_probs[tuple(states)]
         return pt.argmax(p)
 
@@ -248,16 +248,21 @@
     n_lags = op.n_lags
 
     indexes = [value[..., i : -(n_lags - i) if n_lags != i else None] for i in range(n_lags + 1)]
 
     mc_logprob = logp(init_dist, value[..., :n_lags]).sum(axis=-1)
     mc_logprob += pt.log(P[tuple(indexes)]).sum(axis=-1)
 
+    # We cannot leave any RV in the logp graph, even if just for an assert
+    [init_dist_leading_dim] = constant_fold(
+        [pt.atleast_1d(init_dist).shape[0]], raise_not_constant=False
+    )
+
     return check_parameters(
         mc_logprob,
         pt.all(pt.eq(P.shape[-(n_lags + 1) :], P.shape[-1])),
         pt.all(pt.allclose(P.sum(axis=-1), 1.0)),
-        pt.eq(pt.atleast_1d(init_dist).shape[0], n_lags),
+        pt.eq(init_dist_leading_dim, n_lags),
         msg="Last (n_lags + 1) dimensions of P must be square, "
         "P must sum to 1 along the last axis, "
         "First dimension of init_dist must be n_lags",
     )
```

### Comparing `pymc-experimental-0.0.9/pymc_experimental/gp/__init__.py` & `pymc_experimental-0.1.0/pymc_experimental/gp/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.9/pymc_experimental/gp/latent_approx.py` & `pymc_experimental-0.1.0/pymc_experimental/gp/latent_approx.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,74 +7,122 @@
 #       http://www.apache.org/licenses/LICENSE-2.0
 #
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
-
+from functools import partial
+from typing import Optional
 
 import numpy as np
 import pymc as pm
 import pytensor.tensor as pt
-from pymc.gp.util import JITTER_DEFAULT, cholesky, solve_lower, solve_upper, stabilize
+from pymc.gp.util import JITTER_DEFAULT, stabilize
+from pytensor.tensor.linalg import cholesky, solve_triangular
+
+solve_lower = partial(solve_triangular, lower=True)
+solve_upper = partial(solve_triangular, lower=False)
 
 
 class LatentApprox(pm.gp.Latent):
     ## TODO: use strings to select approximation, like pm.gp.MarginalApprox?
     pass
 
 
 class ProjectedProcess(pm.gp.Latent):
     ## AKA: DTC
     def __init__(
-        self, n_inducing, *, mean_func=pm.gp.mean.Zero(), cov_func=pm.gp.cov.Constant(0.0)
+        self,
+        n_inducing: Optional[int] = None,
+        *,
+        mean_func=pm.gp.mean.Zero(),
+        cov_func=pm.gp.cov.Constant(0.0),
     ):
         self.n_inducing = n_inducing
         super().__init__(mean_func=mean_func, cov_func=cov_func)
 
-    def _build_prior(self, name, X, Xu, jitter=JITTER_DEFAULT, **kwargs):
+    def _build_prior(self, name, X, X_inducing, jitter=JITTER_DEFAULT, **kwargs):
         mu = self.mean_func(X)
-        Kuu = self.cov_func(Xu)
+        Kuu = self.cov_func(X_inducing)
         L = cholesky(stabilize(Kuu, jitter))
 
-        n_inducing_points = np.shape(Xu)[0]
+        n_inducing_points = np.shape(X_inducing)[0]
         v = pm.Normal(name + "_u_rotated_", mu=0.0, sigma=1.0, size=n_inducing_points, **kwargs)
         u = pm.Deterministic(name + "_u", L @ v)
 
-        Kfu = self.cov_func(X, Xu)
+        Kfu = self.cov_func(X, X_inducing)
         Kuuiu = solve_upper(pt.transpose(L), solve_lower(L, u))
 
         return pm.Deterministic(name, mu + Kfu @ Kuuiu), Kuuiu, L
 
-    def prior(self, name, X, Xu=None, jitter=JITTER_DEFAULT, **kwargs):
-        if Xu is None and self.n_inducing is None:
-            raise ValueError
-        elif Xu is None:
-            if isinstance(X, np.ndarray):
-                Xu = pm.gp.util.kmeans_inducing_points(self.n_inducing, X, **kwargs)
+    def prior(
+        self,
+        name: str,
+        X: np.ndarray,
+        X_inducing: Optional[np.ndarray] = None,
+        jitter: float = JITTER_DEFAULT,
+        **kwargs,
+    ) -> np.ndarray:
+        """
+        Builds the GP prior with optional inducing points locations.
+
+        Parameters:
+        - name: Name for the GP variable.
+        - X: Input data.
+        - X_inducing: Optional. Inducing points for the GP.
+        - jitter: Jitter to ensure numerical stability.
+
+        Returns:
+        - GP function
+        """
+        # Check if X is a numpy array
+        if not isinstance(X, np.ndarray):
+            raise ValueError("'X' must be a numpy array.")
+
+        # Proceed with provided X_inducing or determine X_inducing based on n_inducing
+        if X_inducing is not None:
+            pass  # X_inducing is directly used
+
+        elif self.n_inducing is not None:
+            # Validate n_inducing
+            if not isinstance(self.n_inducing, int) or self.n_inducing <= 0:
+                raise ValueError(
+                    "The number of inducing points, 'n_inducing', must be a positive integer."
+                )
+            if self.n_inducing > len(X):
+                raise ValueError(
+                    "The number of inducing points, 'n_inducing', cannot be greater than the number of data points in 'X'."
+                )
+            # Use k-means to select X_inducing from X based on n_inducing
+            X_inducing = pm.gp.util.kmeans_inducing_points(self.n_inducing, X, **kwargs)
+        else:
+            # Neither X_inducing nor n_inducing provided
+            raise ValueError(
+                "Either 'X_inducing' (inducing points) or 'n_inducing' (number of inducing points) must be specified."
+            )
 
-        f, Kuuiu, L = self._build_prior(name, X, Xu, jitter, **kwargs)
-        self.X, self.Xu = X, Xu
+        f, Kuuiu, L = self._build_prior(name, X, X_inducing, jitter, **kwargs)
+        self.X, self.X_inducing = X, X_inducing
         self.L, self.Kuuiu = L, Kuuiu
         self.f = f
         return f
 
-    def _build_conditional(self, name, Xnew, Xu, L, Kuuiu, jitter, **kwargs):
-        Ksu = self.cov_func(Xnew, Xu)
+    def _build_conditional(self, name, Xnew, X_inducing, L, Kuuiu, jitter, **kwargs):
+        Ksu = self.cov_func(Xnew, X_inducing)
         mu = self.mean_func(Xnew) + Ksu @ Kuuiu
         tmp = solve_lower(L, pt.transpose(Ksu))
         Qss = pt.transpose(tmp) @ tmp  # Qss = tt.dot(tt.dot(Ksu, tt.nlinalg.pinv(Kuu)), Ksu.T)
         Kss = self.cov_func(Xnew)
         Lss = cholesky(stabilize(Kss - Qss, jitter))
         return mu, Lss
 
     def conditional(self, name, Xnew, jitter=1e-6, **kwargs):
         mu, chol = self._build_conditional(
-            name, Xnew, self.Xu, self.L, self.Kuuiu, jitter, **kwargs
+            name, Xnew, self.X_inducing, self.L, self.Kuuiu, jitter, **kwargs
         )
         return pm.MvNormal(name, mu=mu, chol=chol)
 
 
 class KarhunenLoeveExpansion(pm.gp.Latent):
     def __init__(
         self,
@@ -119,15 +167,15 @@
 
     def _build_conditional(self, Xnew, X, f, U, s, jitter):
         Kxs = self.cov_func(X, Xnew)
         Kss = self.cov_func(Xnew)
         Kxxpinv = U @ pt.diag(1.0 / s) @ U.T
         mus = Kxs.T @ Kxxpinv @ f
         K = Kss - Kxs.T @ Kxxpinv @ Kxs
-        L = pm.gp.util.cholesky(pm.gp.util.stabilize(K, jitter))
+        L = cholesky(stabilize(K, jitter))
         return mus, L
 
     def conditional(self, name, Xnew, jitter=1e-6, **kwargs):
         X, f = self.X, self.f
         U, s = self.U, self.s
         mu, L = self._build_conditional(Xnew, X, f, U, s, jitter)
         return pm.MvNormal(name, mu=mu, chol=L, **kwargs)
```

### Comparing `pymc-experimental-0.0.9/pymc_experimental/inference/__init__.py` & `pymc_experimental-0.1.0/pymc_experimental/inference/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.9/pymc_experimental/inference/fit.py` & `pymc_experimental-0.1.0/pymc_experimental/inference/fit.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,11 +27,14 @@
 
     Returns
     -------
     arviz.InferenceData
     """
     if method == "pathfinder":
         try:
-            from pymc_experimental.inference.pathfinder import fit_pathfinder
+            import blackjax
         except ImportError as exc:
             raise RuntimeError("Need BlackJAX to use `pathfinder`") from exc
+
+        from pymc_experimental.inference.pathfinder import fit_pathfinder
+
         return fit_pathfinder(**kwargs)
```

### Comparing `pymc-experimental-0.0.9/pymc_experimental/inference/pathfinder.py` & `pymc_experimental-0.1.0/pymc_experimental/inference/pathfinder.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,141 +8,127 @@
 #
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 
-
 import collections
 import sys
 from typing import Optional
 
 import arviz as az
 import blackjax
 import jax
-import jax.numpy as jnp
-import jax.random as random
 import numpy as np
 import pymc as pm
-from pymc import modelcontext
-from pymc.sampling_jax import get_jaxified_graph
+from packaging import version
+from pymc.backends.arviz import coords_and_dims_for_inferencedata
+from pymc.blocking import DictToArrayBijection, RaveledVars
+from pymc.model import modelcontext
+from pymc.sampling.jax import get_jaxified_graph
 from pymc.util import RandomSeed, _get_seeds_per_chain, get_default_varnames
 
 
 def convert_flat_trace_to_idata(
     samples,
-    dims=None,
-    coords=None,
     include_transformed=False,
     postprocessing_backend="cpu",
     model=None,
 ):
-
     model = modelcontext(model)
-    init_position_dict = model.initial_point()
+    ip = model.initial_point()
+    ip_point_map_info = pm.blocking.DictToArrayBijection.map(ip).point_map_info
     trace = collections.defaultdict(list)
-    astart = pm.blocking.DictToArrayBijection.map(init_position_dict)
     for sample in samples:
-        raveld_vars = pm.blocking.RaveledVars(sample, astart.point_map_info)
-        point = pm.blocking.DictToArrayBijection.rmap(raveld_vars, init_position_dict)
+        raveld_vars = RaveledVars(sample, ip_point_map_info)
+        point = DictToArrayBijection.rmap(raveld_vars, ip)
         for p, v in point.items():
             trace[p].append(v.tolist())
 
     trace = {k: np.asarray(v)[None, ...] for k, v in trace.items()}
 
     var_names = model.unobserved_value_vars
     vars_to_sample = list(get_default_varnames(var_names, include_transformed=include_transformed))
     print("Transforming variables...", file=sys.stdout)
     jax_fn = get_jaxified_graph(inputs=model.value_vars, outputs=vars_to_sample)
     result = jax.vmap(jax.vmap(jax_fn))(
         *jax.device_put(list(trace.values()), jax.devices(postprocessing_backend)[0])
     )
-
     trace = {v.name: r for v, r in zip(vars_to_sample, result)}
+    coords, dims = coords_and_dims_for_inferencedata(model)
     idata = az.from_dict(trace, dims=dims, coords=coords)
 
     return idata
 
 
 def fit_pathfinder(
-    iterations=5_000,
+    samples=1000,
     random_seed: Optional[RandomSeed] = None,
     postprocessing_backend="cpu",
-    ftol=1e-4,
     model=None,
+    **pathfinder_kwargs,
 ):
     """
     Fit the pathfinder algorithm as implemented in blackjax
 
     Requires the JAX backend
 
     Parameters
     ----------
-    iterations : int
-        Number of iterations to run.
+    samples : int
+        Number of samples to draw from the fitted approximation.
     random_seed : int
         Random seed to set.
     postprocessing_backend : str
         Where to compute transformations of the trace.
         "cpu" or "gpu".
-    ftol : float
-        Floating point tolerance
+    pathfinder_kwargs:
+        kwargs for blackjax.vi.pathfinder.approximate
 
     Returns
     -------
     arviz.InferenceData
 
     Reference
     ---------
     https://arxiv.org/abs/2108.03782
     """
-
-    (random_seed,) = _get_seeds_per_chain(random_seed, 1)
+    # Temporarily helper
+    if version.parse(blackjax.__version__).major < 1:
+        raise ImportError("fit_pathfinder requires blackjax 1.0 or above")
 
     model = modelcontext(model)
 
-    rvs = [rv.name for rv in model.value_vars]
-    init_position_dict = model.initial_point()
-    init_position = [init_position_dict[rv] for rv in rvs]
+    ip = model.initial_point()
+    ip_map = DictToArrayBijection.map(ip)
 
     new_logprob, new_input = pm.pytensorf.join_nonshared_inputs(
-        init_position_dict, (model.logp(),), model.value_vars, ()
+        ip, (model.logp(),), model.value_vars, ()
     )
 
     logprob_fn_list = get_jaxified_graph([new_input], new_logprob)
 
     def logprob_fn(x):
         return logprob_fn_list(x)[0]
 
-    dim = sum(v.size for v in init_position_dict.values())
-
-    rng_key = random.PRNGKey(random_seed)
-    w0 = random.multivariate_normal(rng_key, 2.0 + jnp.zeros(dim), jnp.eye(dim))
-    path = blackjax.vi.pathfinder.init(rng_key, logprob_fn, w0, return_path=True, ftol=ftol)
-
-    pathfinder = blackjax.kernels.pathfinder(rng_key, logprob_fn, ftol=ftol)
-    state = pathfinder.init(w0)
+    [pathfinder_seed, sample_seed] = _get_seeds_per_chain(random_seed, 2)
 
-    def inference_loop(rng_key, kernel, initial_state, num_samples):
-        @jax.jit
-        def one_step(state, rng_key):
-            state, info = kernel(rng_key, state)
-            return state, (state, info)
-
-        keys = jax.random.split(rng_key, num_samples)
-        return jax.lax.scan(one_step, initial_state, keys)
-
-    _, rng_key = random.split(rng_key)
     print("Running pathfinder...", file=sys.stdout)
-    _, (_, samples) = inference_loop(rng_key, pathfinder.step, state, iterations)
-
-    dims = {
-        var_name: [dim for dim in dims if dim is not None]
-        for var_name, dims in model.named_vars_to_dims.items()
-    }
+    pathfinder_state, _ = blackjax.vi.pathfinder.approximate(
+        rng_key=jax.random.key(pathfinder_seed),
+        logdensity_fn=logprob_fn,
+        initial_position=ip_map.data,
+        **pathfinder_kwargs,
+    )
+    samples, _ = blackjax.vi.pathfinder.sample(
+        rng_key=jax.random.key(sample_seed),
+        state=pathfinder_state,
+        num_samples=samples,
+    )
 
     idata = convert_flat_trace_to_idata(
-        samples, postprocessing_backend=postprocessing_backend, coords=model.coords, dims=dims
+        samples,
+        postprocessing_backend=postprocessing_backend,
+        model=model,
     )
-
     return idata
```

### Comparing `pymc-experimental-0.0.9/pymc_experimental/linearmodel.py` & `pymc_experimental-0.1.0/pymc_experimental/linearmodel.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,24 +16,24 @@
     This class is an implementation of a single-input linear regression model in PYMC using the
     BayesianEstimator base class for interoperability with scikit-learn.
     """
 
     _model_type = "LinearModel"
     version = "0.1"
 
-    @property
-    def default_model_config(self):
+    @staticmethod
+    def get_default_model_config():
         return {
             "intercept": {"loc": 0, "scale": 10},
             "slope": {"loc": 0, "scale": 10},
             "obs_error": 2,
         }
 
-    @property
-    def default_sampler_config(self):
+    @staticmethod
+    def get_default_sampler_config():
         return {
             "draws": 1_000,
             "tune": 1_000,
             "chains": 3,
             "target_accept": 0.95,
         }
 
@@ -63,20 +63,18 @@
         >>> assert "σ_model_fmc" in self.model.named_vars
         >>> assert "y_model" in self.model.named_vars
         >>> assert "y_hat" in self.model.named_vars
         >>> assert self.output_var == "y_hat"
         """
         cfg = self.model_config
 
-        # The model is built with placeholder data.
-        # Actual data will be set by _data_setter when fitting or evaluating the model.
         # Data array size can change but number of dimensions must stay the same.
         with pm.Model() as self.model:
-            x = pm.MutableData("x", np.zeros((1,)), dims="observation")
-            y_data = pm.MutableData("y_data", np.zeros((1,)), dims="observation")
+            x = pm.Data("x", np.zeros((1,)), dims="observation")
+            y_data = pm.Data("y_data", np.zeros((1,)), dims="observation")
 
             # priors
             intercept = pm.Normal(
                 "intercept", cfg["intercept"]["loc"], sigma=cfg["intercept"]["scale"]
             )
             slope = pm.Normal("slope", cfg["slope"]["loc"], sigma=cfg["slope"]["scale"])
             obs_error = pm.HalfNormal("σ_model_fmc", cfg["obs_error"])
@@ -90,21 +88,23 @@
                 y_model,
                 sigma=obs_error,
                 shape=x.shape,
                 observed=y_data,
                 dims="observation",
             )
 
+        self._data_setter(X, y)
+
     def _data_setter(self, X: pd.DataFrame, y: Optional[Union[pd.DataFrame, pd.Series]] = None):
         with self.model:
             pm.set_data({"x": X.squeeze()})
             if y is not None:
                 pm.set_data({"y_data": y.squeeze()})
 
-    def generate_and_preprocess_model_data(
+    def _generate_and_preprocess_model_data(
         self, X: Union[pd.DataFrame, pd.Series], y: pd.Series
     ) -> None:
         """
         Generate model data for linear regression.
 
         Parameters
         ----------
```

### Comparing `pymc-experimental-0.0.9/pymc_experimental/marginal_model.py` & `pymc_experimental-0.1.0/pymc_experimental/model/marginal_model.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,39 @@
 import warnings
 from typing import Sequence, Tuple, Union
 
 import numpy as np
+import pymc
 import pytensor.tensor as pt
+from arviz import dict_to_dataset
 from pymc import SymbolicRandomVariable
+from pymc.backends.arviz import coords_and_dims_for_inferencedata, dataset_to_point_list
 from pymc.distributions.discrete import Bernoulli, Categorical, DiscreteUniform
 from pymc.distributions.transforms import Chain
 from pymc.logprob.abstract import _logprob
-from pymc.logprob.basic import conditional_logp
+from pymc.logprob.basic import conditional_logp, logp
 from pymc.logprob.transforms import IntervalTransform
 from pymc.model import Model
-from pymc.pytensorf import constant_fold, inputvars
-from pytensor import Mode
+from pymc.pytensorf import compile_pymc, constant_fold, inputvars
+from pymc.util import _get_seeds_per_chain, treedict
+from pytensor import Mode, scan
 from pytensor.compile import SharedVariable
 from pytensor.compile.builders import OpFromGraph
 from pytensor.graph import Constant, FunctionGraph, ancestors, clone_replace
+from pytensor.graph.replace import vectorize_graph
 from pytensor.scan import map as scan_map
-from pytensor.tensor import TensorVariable
+from pytensor.tensor import TensorType, TensorVariable
 from pytensor.tensor.elemwise import Elemwise
+from pytensor.tensor.shape import Shape
+from pytensor.tensor.special import log_softmax
 
 __all__ = ["MarginalModel"]
 
+from pymc_experimental.distributions import DiscreteMarkovChain
+
 
 class MarginalModel(Model):
     """Subclass of PyMC Model that implements functionality for automatic
     marginalization of variables in the logp transformation
 
     After defining the full Model, the `marginalize` method can be used to indicate a
     subset of variables that should be marginalized
@@ -68,14 +77,15 @@
             idata = pm.sample()
 
     """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.marginalized_rvs = []
+        self._marginalized_named_vars_to_dims = {}
 
     def _delete_rv_mappings(self, rv: TensorVariable) -> None:
         """Remove all model mappings referring to rv
 
         This can be used to "delete" an RV from a model
         """
         assert rv in self.basic_RVs, "rv is not part of the Model"
@@ -195,69 +205,325 @@
         if vars is not None:
             if not isinstance(vars, Sequence):
                 vars = (vars,)
             vars = [m[var.name] for var in vars]
         return m._logp(vars=vars, **kwargs)
 
     def clone(self):
-        m = MarginalModel()
-        vars = self.basic_RVs + self.potentials + self.deterministics + self.marginalized_rvs
+        m = MarginalModel(coords=self.coords)
+        model_vars = self.basic_RVs + self.potentials + self.deterministics + self.marginalized_rvs
+        data_vars = [var for name, var in self.named_vars.items() if var not in model_vars]
+        vars = model_vars + data_vars
         cloned_vars = clone_replace(vars)
         vars_to_clone = {var: cloned_var for var, cloned_var in zip(vars, cloned_vars)}
+        m.vars_to_clone = vars_to_clone
 
-        m.named_vars = {name: vars_to_clone[var] for name, var in self.named_vars.items()}
+        m.named_vars = treedict({name: vars_to_clone[var] for name, var in self.named_vars.items()})
         m.named_vars_to_dims = self.named_vars_to_dims
         m.values_to_rvs = {i: vars_to_clone[rv] for i, rv in self.values_to_rvs.items()}
         m.rvs_to_values = {vars_to_clone[rv]: i for rv, i in self.rvs_to_values.items()}
         m.rvs_to_transforms = {vars_to_clone[rv]: i for rv, i in self.rvs_to_transforms.items()}
         m.rvs_to_initial_values = {
             vars_to_clone[rv]: i for rv, i in self.rvs_to_initial_values.items()
         }
         m.free_RVs = [vars_to_clone[rv] for rv in self.free_RVs]
         m.observed_RVs = [vars_to_clone[rv] for rv in self.observed_RVs]
         m.potentials = [vars_to_clone[pot] for pot in self.potentials]
         m.deterministics = [vars_to_clone[det] for det in self.deterministics]
 
         m.marginalized_rvs = [vars_to_clone[rv] for rv in self.marginalized_rvs]
+        m._marginalized_named_vars_to_dims = self._marginalized_named_vars_to_dims
         return m
 
-    def marginalize(self, rvs_to_marginalize: Union[TensorVariable, Sequence[TensorVariable]]):
+    def marginalize(
+        self,
+        rvs_to_marginalize: Union[TensorVariable, str, Sequence[TensorVariable], Sequence[str]],
+    ):
         if not isinstance(rvs_to_marginalize, Sequence):
             rvs_to_marginalize = (rvs_to_marginalize,)
+        rvs_to_marginalize = [
+            self[var] if isinstance(var, str) else var for var in rvs_to_marginalize
+        ]
 
-        supported_dists = (Bernoulli, Categorical, DiscreteUniform)
         for rv_to_marginalize in rvs_to_marginalize:
             if rv_to_marginalize not in self.free_RVs:
                 raise ValueError(
                     f"Marginalized RV {rv_to_marginalize} is not a free RV in the model"
                 )
-            if not isinstance(rv_to_marginalize.owner.op, supported_dists):
+
+            rv_op = rv_to_marginalize.owner.op
+            if isinstance(rv_op, DiscreteMarkovChain):
+                if rv_op.n_lags > 1:
+                    raise NotImplementedError(
+                        "Marginalization for DiscreteMarkovChain with n_lags > 1 is not supported"
+                    )
+                if rv_to_marginalize.owner.inputs[0].type.ndim > 2:
+                    raise NotImplementedError(
+                        "Marginalization for DiscreteMarkovChain with non-matrix transition probability is not supported"
+                    )
+            elif not isinstance(rv_op, (Bernoulli, Categorical, DiscreteUniform)):
                 raise NotImplementedError(
-                    f"RV with distribution {rv_to_marginalize.owner.op} cannot be marginalized. "
-                    f"Supported distribution include {supported_dists}"
+                    f"Marginalization of RV with distribution {rv_to_marginalize.owner.op} is not supported"
                 )
 
+            if rv_to_marginalize.name in self.named_vars_to_dims:
+                dims = self.named_vars_to_dims[rv_to_marginalize.name]
+                self._marginalized_named_vars_to_dims[rv_to_marginalize.name] = dims
+
             self._delete_rv_mappings(rv_to_marginalize)
             self.marginalized_rvs.append(rv_to_marginalize)
 
         # Raise errors and warnings immediately
         self.clone()._marginalize(user_warnings=True)
 
+    def _to_transformed(self):
+        "Create a function from the untransformed space to the transformed space"
+        transformed_rvs = []
+        transformed_names = []
+
+        for rv in self.free_RVs:
+            transform = self.rvs_to_transforms.get(rv)
+            if transform is None:
+                transformed_rvs.append(rv)
+                transformed_names.append(rv.name)
+            else:
+                transformed_rv = transform.forward(rv, *rv.owner.inputs)
+                transformed_rvs.append(transformed_rv)
+                transformed_names.append(self.rvs_to_values[rv].name)
+
+        fn = self.compile_fn(inputs=self.free_RVs, outs=transformed_rvs)
+        return fn, transformed_names
+
+    def unmarginalize(self, rvs_to_unmarginalize):
+        for rv in rvs_to_unmarginalize:
+            self.marginalized_rvs.remove(rv)
+            if rv.name in self._marginalized_named_vars_to_dims:
+                dims = self._marginalized_named_vars_to_dims.pop(rv.name)
+            else:
+                dims = None
+            self.register_rv(rv, name=rv.name, dims=dims)
+
+    def recover_marginals(
+        self,
+        idata,
+        var_names=None,
+        return_samples=True,
+        extend_inferencedata=True,
+        random_seed=None,
+    ):
+        """Computes posterior log-probabilities and samples of marginalized variables
+        conditioned on parameters of the model given InferenceData with posterior group
+
+        When there are multiple marginalized variables, each marginalized variable is
+        conditioned on both the parameters and the other variables still marginalized
+
+        All log-probabilities are within the transformed space
+
+        Parameters
+        ----------
+        idata : InferenceData
+            InferenceData with posterior group
+        var_names : sequence of str, optional
+            List of variable names for which to compute posterior log-probabilities and samples. Defaults to all marginalized variables
+        return_samples : bool, default True
+            If True, also return samples of the marginalized variables
+        extend_inferencedata : bool, default True
+            Whether to extend the original InferenceData or return a new one
+        random_seed: int, array-like of int or SeedSequence, optional
+            Seed used to generating samples
+
+        Returns
+        -------
+        idata : InferenceData
+            InferenceData with where a lp_{varname} and {varname} for each marginalized variable in var_names added to the posterior group
+
+        .. code-block:: python
+
+            import pymc as pm
+            from pymc_experimental import MarginalModel
+
+            with MarginalModel() as m:
+                p = pm.Beta("p", 1, 1)
+                x = pm.Bernoulli("x", p=p, shape=(3,))
+                y = pm.Normal("y", pm.math.switch(x, -10, 10), observed=[10, 10, -10])
+
+                m.marginalize([x])
+
+                idata = pm.sample()
+                m.recover_marginals(idata, var_names=["x"])
+
+
+        """
+        if var_names is None:
+            var_names = [var.name for var in self.marginalized_rvs]
+
+        var_names = [var if isinstance(var, str) else var.name for var in var_names]
+        vars_to_recover = [v for v in self.marginalized_rvs if v.name in var_names]
+        missing_names = [v.name for v in vars_to_recover if v not in self.marginalized_rvs]
+        if missing_names:
+            raise ValueError(f"Unrecognized var_names: {missing_names}")
+
+        if return_samples and random_seed is not None:
+            seeds = _get_seeds_per_chain(random_seed, len(vars_to_recover))
+        else:
+            seeds = [None] * len(vars_to_recover)
+
+        posterior = idata.posterior
+
+        # Remove Deterministics
+        posterior_values = posterior[
+            [rv.name for rv in self.free_RVs if rv not in self.marginalized_rvs]
+        ]
+
+        sample_dims = ("chain", "draw")
+        posterior_pts, stacked_dims = dataset_to_point_list(posterior_values, sample_dims)
+
+        # Handle Transforms
+        transform_fn, transform_names = self._to_transformed()
+
+        def transform_input(inputs):
+            return dict(zip(transform_names, transform_fn(inputs)))
+
+        posterior_pts = [transform_input(vs) for vs in posterior_pts]
+
+        rv_dict = {}
+        rv_dims = {}
+        for seed, marginalized_rv in zip(seeds, vars_to_recover):
+            supported_dists = (Bernoulli, Categorical, DiscreteUniform)
+            if not isinstance(marginalized_rv.owner.op, supported_dists):
+                raise NotImplementedError(
+                    f"RV with distribution {marginalized_rv.owner.op} cannot be recovered. "
+                    f"Supported distribution include {supported_dists}"
+                )
+
+            m = self.clone()
+            marginalized_rv = m.vars_to_clone[marginalized_rv]
+            m.unmarginalize([marginalized_rv])
+            dependent_vars = find_conditional_dependent_rvs(marginalized_rv, m.basic_RVs)
+            joint_logps = m.logp(vars=[marginalized_rv] + dependent_vars, sum=False)
+
+            marginalized_value = m.rvs_to_values[marginalized_rv]
+            other_values = [v for v in m.value_vars if v is not marginalized_value]
+
+            # Handle batch dims for marginalized value and its dependent RVs
+            marginalized_logp, *dependent_logps = joint_logps
+            joint_logp = marginalized_logp + _add_reduce_batch_dependent_logps(
+                marginalized_rv.type, dependent_logps
+            )
+
+            rv_shape = constant_fold(tuple(marginalized_rv.shape), raise_not_constant=False)
+            rv_domain = get_domain_of_finite_discrete_rv(marginalized_rv)
+            rv_domain_tensor = pt.moveaxis(
+                pt.full(
+                    (*rv_shape, len(rv_domain)),
+                    rv_domain,
+                    dtype=marginalized_rv.dtype,
+                ),
+                -1,
+                0,
+            )
+
+            joint_logps = vectorize_graph(
+                joint_logp,
+                replace={marginalized_value: rv_domain_tensor},
+            )
+            joint_logps = pt.moveaxis(joint_logps, 0, -1)
+
+            rv_loglike_fn = None
+            joint_logps_norm = log_softmax(joint_logps, axis=-1)
+            if return_samples:
+                sample_rv_outs = pymc.Categorical.dist(logit_p=joint_logps)
+                if isinstance(marginalized_rv.owner.op, DiscreteUniform):
+                    sample_rv_outs += rv_domain[0]
+
+                rv_loglike_fn = compile_pymc(
+                    inputs=other_values,
+                    outputs=[joint_logps_norm, sample_rv_outs],
+                    on_unused_input="ignore",
+                    random_seed=seed,
+                )
+            else:
+                rv_loglike_fn = compile_pymc(
+                    inputs=other_values,
+                    outputs=joint_logps_norm,
+                    on_unused_input="ignore",
+                    random_seed=seed,
+                )
+
+            logvs = [rv_loglike_fn(**vs) for vs in posterior_pts]
+
+            logps = None
+            samples = None
+            if return_samples:
+                logps, samples = zip(*logvs)
+                logps = np.array(logps)
+                samples = np.array(samples)
+                rv_dict[marginalized_rv.name] = samples.reshape(
+                    tuple(len(coord) for coord in stacked_dims.values()) + samples.shape[1:],
+                )
+            else:
+                logps = np.array(logvs)
+
+            rv_dict["lp_" + marginalized_rv.name] = logps.reshape(
+                tuple(len(coord) for coord in stacked_dims.values()) + logps.shape[1:],
+            )
+            if marginalized_rv.name in m.named_vars_to_dims:
+                rv_dims[marginalized_rv.name] = list(m.named_vars_to_dims[marginalized_rv.name])
+                rv_dims["lp_" + marginalized_rv.name] = rv_dims[marginalized_rv.name] + [
+                    "lp_" + marginalized_rv.name + "_dim"
+                ]
+
+        coords, dims = coords_and_dims_for_inferencedata(self)
+        dims.update(rv_dims)
+        rv_dataset = dict_to_dataset(
+            rv_dict,
+            library=pymc,
+            dims=dims,
+            coords=coords,
+            default_dims=list(sample_dims),
+            skip_event_dims=True,
+        )
+
+        if extend_inferencedata:
+            idata.posterior = idata.posterior.assign(rv_dataset)
+            return idata
+        else:
+            return rv_dataset
+
 
 class MarginalRV(SymbolicRandomVariable):
     """Base class for Marginalized RVs"""
 
 
 class FiniteDiscreteMarginalRV(MarginalRV):
     """Base class for Finite Discrete Marginalized RVs"""
 
 
+class DiscreteMarginalMarkovChainRV(MarginalRV):
+    """Base class for Discrete Marginal Markov Chain RVs"""
+
+
+def static_shape_ancestors(vars):
+    """Identify ancestors Shape Ops of static shapes (therefore constant in a valid graph)."""
+    return [
+        var
+        for var in ancestors(vars)
+        if (
+            var.owner
+            and isinstance(var.owner.op, Shape)
+            # All static dims lengths of Shape input are known
+            and None not in var.owner.inputs[0].type.shape
+        )
+    ]
+
+
 def find_conditional_input_rvs(output_rvs, all_rvs):
-    """Find conditionally indepedent input RVs"""
+    """Find conditionally indepedent input RVs."""
     blockers = [other_rv for other_rv in all_rvs if other_rv not in output_rvs]
+    blockers += static_shape_ancestors(tuple(all_rvs) + tuple(output_rvs))
     return [
         var
         for var in ancestors(output_rvs, blockers=blockers)
         if var in blockers
         or (var.owner is None and not isinstance(var, (Constant, SharedVariable)))
     ]
 
@@ -309,86 +575,117 @@
     if rv_to_marginalize in ancestors(
         other_truncated_inputs, blockers=[rv_to_marginalize, *other_input_rvs]
     ):
         return False
     return True
 
 
+from pytensor.graph.basic import graph_inputs
+
+
+def collect_shared_vars(outputs, blockers):
+    return [
+        inp for inp in graph_inputs(outputs, blockers=blockers) if isinstance(inp, SharedVariable)
+    ]
+
+
 def replace_finite_discrete_marginal_subgraph(fgraph, rv_to_marginalize, all_rvs):
     # TODO: This should eventually be integrated in a more general routine that can
     #  identify other types of supported marginalization, of which finite discrete
     #  RVs is just one
 
     dependent_rvs = find_conditional_dependent_rvs(rv_to_marginalize, all_rvs)
     if not dependent_rvs:
         raise ValueError(f"No RVs depend on marginalized RV {rv_to_marginalize}")
 
     ndim_supp = {rv.owner.op.ndim_supp for rv in dependent_rvs}
-    if max(ndim_supp) > 0:
+    if len(ndim_supp) != 1:
         raise NotImplementedError(
-            "Marginalization of withe dependent Multivariate RVs not implemented"
+            "Marginalization with dependent variables of different support dimensionality not implemented"
         )
+    [ndim_supp] = ndim_supp
+    if ndim_supp > 0:
+        raise NotImplementedError("Marginalization with dependent Multivariate RVs not implemented")
 
     marginalized_rv_input_rvs = find_conditional_input_rvs([rv_to_marginalize], all_rvs)
     dependent_rvs_input_rvs = [
         rv
         for rv in find_conditional_input_rvs(dependent_rvs, all_rvs)
         if rv is not rv_to_marginalize
     ]
 
     # If the marginalized RV has batched dimensions, check that graph between
     # marginalized RV and dependent RVs is composed strictly of Elemwise Operations.
     # This implies (?) that the dimensions are completely independent and a logp graph
     # can ultimately be generated that is proportional to the support domain and not
     # to the variables dimensions
     # We don't need to worry about this if the  RV is scalar.
-    if np.prod(constant_fold(tuple(rv_to_marginalize.shape))) > 1:
+    if np.prod(constant_fold(tuple(rv_to_marginalize.shape), raise_not_constant=False)) != 1:
         if not is_elemwise_subgraph(rv_to_marginalize, dependent_rvs_input_rvs, dependent_rvs):
             raise NotImplementedError(
                 "The subgraph between a marginalized RV and its dependents includes non Elemwise operations. "
                 "This is currently not supported",
             )
 
     input_rvs = [*marginalized_rv_input_rvs, *dependent_rvs_input_rvs]
     rvs_to_marginalize = [rv_to_marginalize, *dependent_rvs]
 
     outputs = rvs_to_marginalize
-    # Clone replace inner RV rng inputs so that we can be sure of the update order
-    # replace_inputs = {rng: rng.type() for rng in updates_rvs_to_marginalize.keys()}
-    # Clone replace outter RV inputs, so that their shared RNGs don't make it into
-    # the inner graph of the marginalized RVs
-    # FIXME: This shouldn't be needed!
-    replace_inputs = {}
-    replace_inputs.update({input_rv: input_rv.type() for input_rv in input_rvs})
-    cloned_outputs = clone_replace(outputs, replace=replace_inputs)
-
-    marginalization_op = FiniteDiscreteMarginalRV(
-        inputs=list(replace_inputs.values()),
-        outputs=cloned_outputs,
-        ndim_supp=0,
+    # We are strict about shared variables in SymbolicRandomVariables
+    inputs = input_rvs + collect_shared_vars(rvs_to_marginalize, blockers=input_rvs)
+
+    if isinstance(rv_to_marginalize.owner.op, DiscreteMarkovChain):
+        marginalize_constructor = DiscreteMarginalMarkovChainRV
+    else:
+        marginalize_constructor = FiniteDiscreteMarginalRV
+
+    marginalization_op = marginalize_constructor(
+        inputs=inputs,
+        outputs=outputs,
+        ndim_supp=ndim_supp,
     )
-    marginalized_rvs = marginalization_op(*replace_inputs.keys())
+
+    marginalized_rvs = marginalization_op(*inputs)
     fgraph.replace_all(tuple(zip(rvs_to_marginalize, marginalized_rvs)))
     return rvs_to_marginalize, marginalized_rvs
 
 
 def get_domain_of_finite_discrete_rv(rv: TensorVariable) -> Tuple[int, ...]:
     op = rv.owner.op
     if isinstance(op, Bernoulli):
         return (0, 1)
     elif isinstance(op, Categorical):
         p_param = rv.owner.inputs[3]
         return tuple(range(pt.get_vector_length(p_param)))
     elif isinstance(op, DiscreteUniform):
         lower, upper = constant_fold(rv.owner.inputs[3:])
-        return tuple(range(lower, upper + 1))
+        return tuple(np.arange(lower, upper + 1))
+    elif isinstance(op, DiscreteMarkovChain):
+        P = rv.owner.inputs[0]
+        return tuple(range(pt.get_vector_length(P[-1])))
 
     raise NotImplementedError(f"Cannot compute domain for op {op}")
 
 
+def _add_reduce_batch_dependent_logps(
+    marginalized_type: TensorType, dependent_logps: Sequence[TensorVariable]
+):
+    """Add the logps of dependent RVs while reducing extra batch dims relative to `marginalized_type`."""
+
+    mbcast = marginalized_type.broadcastable
+    reduced_logps = []
+    for dependent_logp in dependent_logps:
+        dbcast = dependent_logp.type.broadcastable
+        dim_diff = len(dbcast) - len(mbcast)
+        mbcast_aligned = (True,) * dim_diff + mbcast
+        vbcast_axis = [i for i, (m, v) in enumerate(zip(mbcast_aligned, dbcast)) if m and not v]
+        reduced_logps.append(dependent_logp.sum(vbcast_axis))
+    return pt.add(*reduced_logps)
+
+
 @_logprob.register(FiniteDiscreteMarginalRV)
 def finite_discrete_marginal_rv_logp(op, values, *inputs, **kwargs):
     # Clone the inner RV graph of the Marginalized RV
     marginalized_rvs_node = op.make_node(*inputs)
     inner_rvs = clone_replace(
         op.inner_outputs,
         replace={u: v for u, v in zip(op.inner_inputs, marginalized_rvs_node.inputs)},
@@ -396,60 +693,54 @@
     marginalized_rv = inner_rvs[0]
 
     # Obtain the joint_logp graph of the inner RV graph
     inner_rvs_to_values = {rv: rv.clone() for rv in inner_rvs}
     logps_dict = conditional_logp(rv_values=inner_rvs_to_values, **kwargs)
 
     # Reduce logp dimensions corresponding to broadcasted variables
-    joint_logp = logps_dict[inner_rvs_to_values[marginalized_rv]]
-    for inner_rv, inner_value in inner_rvs_to_values.items():
-        if inner_rv is marginalized_rv:
-            continue
-        vbcast = inner_value.type.broadcastable
-        mbcast = marginalized_rv.type.broadcastable
-        mbcast = (True,) * (len(vbcast) - len(mbcast)) + mbcast
-        values_axis_bcast = [i for i, (m, v) in enumerate(zip(mbcast, vbcast)) if m != v]
-        joint_logp += logps_dict[inner_value].sum(values_axis_bcast, keepdims=True)
+    marginalized_logp = logps_dict.pop(inner_rvs_to_values[marginalized_rv])
+    joint_logp = marginalized_logp + _add_reduce_batch_dependent_logps(
+        marginalized_rv.type, logps_dict.values()
+    )
 
-    # Wrap the joint_logp graph in an OpFromGrah, so that we can evaluate it at different
+    # Wrap the joint_logp graph in an OpFromGraph, so that we can evaluate it at different
     # values of the marginalized RV
     # Some inputs are not root inputs (such as transformed projections of value variables)
     # Or cannot be used as inputs to an OpFromGraph (shared variables and constants)
     inputs = list(inputvars(inputs))
     joint_logp_op = OpFromGraph(
         list(inner_rvs_to_values.values()) + inputs, [joint_logp], inline=True
     )
 
     # Compute the joint_logp for all possible n values of the marginalized RV. We assume
     # each original dimension is independent so that it suffices to evaluate the graph
     # n times, once with each possible value of the marginalized RV replicated across
     # batched dimensions of the marginalized RV
 
     # PyMC does not allow RVs in the logp graph, even if we are just using the shape
-    marginalized_rv_shape = constant_fold(tuple(marginalized_rv.shape))
+    marginalized_rv_shape = constant_fold(tuple(marginalized_rv.shape), raise_not_constant=False)
     marginalized_rv_domain = get_domain_of_finite_discrete_rv(marginalized_rv)
-    marginalized_rv_domain_tensor = pt.swapaxes(
+    marginalized_rv_domain_tensor = pt.moveaxis(
         pt.full(
             (*marginalized_rv_shape, len(marginalized_rv_domain)),
             marginalized_rv_domain,
             dtype=marginalized_rv.dtype,
         ),
-        axis1=0,
-        axis2=-1,
+        -1,
+        0,
     )
 
     # Arbitrary cutoff to switch to Scan implementation to keep graph size under control
+    # TODO: Try vectorize here
     if len(marginalized_rv_domain) <= 10:
         joint_logps = [
             joint_logp_op(marginalized_rv_domain_tensor[i], *values, *inputs)
             for i in range(len(marginalized_rv_domain))
         ]
     else:
-        # Make sure this rewrite is registered
-        from pymc.pytensorf import local_remove_check_parameter
 
         def logp_fn(marginalized_rv_const, *non_sequences):
             return joint_logp_op(marginalized_rv_const, *non_sequences)
 
         joint_logps, _ = scan_map(
             fn=logp_fn,
             sequences=marginalized_rv_domain_tensor,
@@ -457,7 +748,73 @@
             mode=Mode().including("local_remove_check_parameter"),
         )
 
     joint_logps = pt.logsumexp(joint_logps, axis=0)
 
     # We have to add dummy logps for the remaining value variables, otherwise PyMC will raise
     return joint_logps, *(pt.constant(0),) * (len(values) - 1)
+
+
+@_logprob.register(DiscreteMarginalMarkovChainRV)
+def marginal_hmm_logp(op, values, *inputs, **kwargs):
+
+    marginalized_rvs_node = op.make_node(*inputs)
+    inner_rvs = clone_replace(
+        op.inner_outputs,
+        replace={u: v for u, v in zip(op.inner_inputs, marginalized_rvs_node.inputs)},
+    )
+
+    chain_rv, *dependent_rvs = inner_rvs
+    P, n_steps_, init_dist_, rng = chain_rv.owner.inputs
+    domain = pt.arange(P.shape[-1], dtype="int32")
+
+    # Construct logp in two steps
+    # Step 1: Compute the probability of the data ("emissions") under every possible state (vec_logp_emission)
+
+    # First we need to vectorize the conditional logp graph of the data, in case there are batch dimensions floating
+    # around. To do this, we need to break the dependency between chain and the init_dist_ random variable. Otherwise,
+    # PyMC will detect a random variable in the logp graph (init_dist_), that isn't relevant at this step.
+    chain_value = chain_rv.clone()
+    dependent_rvs = clone_replace(dependent_rvs, {chain_rv: chain_value})
+    logp_emissions_dict = conditional_logp(dict(zip(dependent_rvs, values)))
+
+    # Reduce and add the batch dims beyond the chain dimension
+    reduced_logp_emissions = _add_reduce_batch_dependent_logps(
+        chain_rv.type, logp_emissions_dict.values()
+    )
+
+    # Add a batch dimension for the domain of the chain
+    chain_shape = constant_fold(tuple(chain_rv.shape))
+    batch_chain_value = pt.moveaxis(pt.full((*chain_shape, domain.size), domain), -1, 0)
+    batch_logp_emissions = vectorize_graph(reduced_logp_emissions, {chain_value: batch_chain_value})
+
+    # Step 2: Compute the transition probabilities
+    # This is the "forward algorithm", alpha_t = p(y | s_t) * sum_{s_{t-1}}(p(s_t | s_{t-1}) * alpha_{t-1})
+    # We do it entirely in logs, though.
+
+    # To compute the prior probabilities of each state, we evaluate the logp of the domain (all possible states) under
+    # the initial distribution. This is robust to everything the user can throw at it.
+    batch_logp_init_dist = pt.vectorize(lambda x: logp(init_dist_, x), "()->()")(
+        batch_chain_value[..., 0]
+    )
+    log_alpha_init = batch_logp_init_dist + batch_logp_emissions[..., 0]
+
+    def step_alpha(logp_emission, log_alpha, log_P):
+        step_log_prob = pt.logsumexp(log_alpha[:, None] + log_P, axis=0)
+        return logp_emission + step_log_prob
+
+    P_bcast_dims = (len(chain_shape) - 1) - (P.type.ndim - 2)
+    log_P = pt.shape_padright(pt.log(P), P_bcast_dims)
+    log_alpha_seq, _ = scan(
+        step_alpha,
+        non_sequences=[log_P],
+        outputs_info=[log_alpha_init],
+        # Scan needs the time dimension first, and we already consumed the 1st logp computing the initial value
+        sequences=pt.moveaxis(batch_logp_emissions[..., 1:], -1, 0),
+    )
+    # Final logp is just the sum of the last scan state
+    joint_logp = pt.logsumexp(log_alpha_seq[-1], axis=0)
+
+    # If there are multiple emission streams, we have to add dummy logps for the remaining value variables. The first
+    # return is the joint probability of everything together, but PyMC still expects one logp for each one.
+    dummy_logps = (pt.constant(0),) * (len(values) - 1)
+    return joint_logp, *dummy_logps
```

### Comparing `pymc-experimental-0.0.9/pymc_experimental/model_builder.py` & `pymc_experimental-0.1.0/pymc_experimental/model_builder.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,17 +67,19 @@
             dictionary of parameters that initialise sampler configuration. Class-default defined by the user default_sampler_config method.
         Examples
         --------
         >>> class MyModel(ModelBuilder):
         >>>     ...
         >>> model = MyModel(model_config, sampler_config)
         """
-        sampler_config = self.default_sampler_config if sampler_config is None else sampler_config
+        sampler_config = (
+            self.get_default_sampler_config() if sampler_config is None else sampler_config
+        )
         self.sampler_config = sampler_config
-        model_config = self.default_model_config if model_config is None else model_config
+        model_config = self.get_default_model_config() if model_config is None else model_config
 
         self.model_config = model_config  # parameters for priors etc.
         self.model = None  # Set by build_model
         self.idata: Optional[az.InferenceData] = None  # idata is generated during fitting
         self.is_fitted_ = False
 
     def _validate_data(self, X, y=None):
@@ -129,25 +131,25 @@
         Returns
         -------
         output_var : str
             Name of the output variable of the model.
         """
         raise NotImplementedError
 
-    @property
+    @staticmethod
     @abstractmethod
-    def default_model_config(self) -> Dict:
+    def get_default_model_config() -> Dict:
         """
         Returns a class default config dict for model builder if no model_config is provided on class initialization
         Useful for understanding structure of required model_config to allow its customization by users
         Examples
         --------
-        >>>     @classmethod
-        >>>     def default_model_config(self):
-        >>>         Return {
+        >>>     @staticmethod
+        >>>     def default_model_config():
+        >>>         return {
         >>>             'a' : {
         >>>                 'loc': 7,
         >>>                 'scale' : 3
         >>>             },
         >>>             'b' : {
         >>>                 'loc': 3,
         >>>                 'scale': 5
@@ -158,59 +160,61 @@
         Returns
         -------
         model_config : dict
             A set of default parameters for predictor distributions that allow to save and recreate the model.
         """
         raise NotImplementedError
 
-    @property
+    @staticmethod
     @abstractmethod
-    def default_sampler_config(self) -> Dict:
+    def get_default_sampler_config(self) -> Dict:
         """
         Returns a class default sampler dict for model builder if no sampler_config is provided on class initialization
         Useful for understanding structure of required sampler_config to allow its customization by users
         Examples
         --------
-        >>>     @classmethod
-        >>>     def default_sampler_config(self):
-        >>>         Return {
+        >>>     @staticmethod
+        >>>     def default_sampler_config():
+        >>>         return {
         >>>             'draws': 1_000,
         >>>             'tune': 1_000,
         >>>             'chains': 1,
         >>>             'target_accept': 0.95,
         >>>         }
 
         Returns
         -------
         sampler_config : dict
             A set of default settings for used by model in fit process.
         """
         raise NotImplementedError
 
     @abstractmethod
-    def generate_and_preprocess_model_data(
+    def _generate_and_preprocess_model_data(
         self, X: Union[pd.DataFrame, pd.Series], y: pd.Series
     ) -> None:
         """
         Applies preprocessing to the data before fitting the model.
         if validate is True, it will check if the data is valid for the model.
         sets self.model_coords based on provided dataset
 
+        In case of optional parameters being passed into the model, this method should implement the conditional
+        logic responsible for correct handling of the optional parameters, and including them into the dataset.
+
         Parameters:
         X : array, shape (n_obs, n_features)
         y : array, shape (n_obs,)
 
         Examples
         --------
         >>>     @classmethod
-        >>>     def generate_and_preprocess_model_data(self, X, y):
-        >>>         x = np.linspace(start=1, stop=50, num=100)
-        >>>         y = 5 * x + 3 + np.random.normal(0, 1, len(x)) * np.random.rand(100)*10 +  np.random.rand(100)*6.4
-        >>>         X = pd.DataFrame(x, columns=['x'])
-        >>>         y = pd.Series(y, name='y')
+        >>>     def _generate_and_preprocess_model_data(self, X, y):
+                    coords = {
+                        'x_dim': X.dim_variable,
+                    } #only include if applicable for your model
         >>>         self.X = X
         >>>         self.y = y
 
         Returns
         -------
         None
 
@@ -291,16 +295,16 @@
             raise RuntimeError(
                 "The model hasn't been built yet, call .build_model() first or call .fit() instead."
             )
 
         with self.model:
             sampler_args = {**self.sampler_config, **kwargs}
             idata = pm.sample(**sampler_args)
-            idata.extend(pm.sample_prior_predictive())
-            idata.extend(pm.sample_posterior_predictive(idata))
+            idata.extend(pm.sample_prior_predictive(), join="right")
+            idata.extend(pm.sample_posterior_predictive(idata), join="right")
 
         idata = self.set_idata_attrs(idata)
         return idata
 
     def set_idata_attrs(self, idata=None):
         """
         Set attributes on an InferenceData object.
@@ -488,15 +492,15 @@
         Initializing NUTS using jitter+adapt_diag...
         """
         if predictor_names is None:
             predictor_names = []
         if y is None:
             y = np.zeros(X.shape[0])
         y = pd.DataFrame({self.output_var: y})
-        self.generate_and_preprocess_model_data(X, y.values.flatten())
+        self._generate_and_preprocess_model_data(X, y.values.flatten())
         self.build_model(self.X, self.y)
 
         sampler_config = self.sampler_config.copy()
         sampler_config["progressbar"] = progressbar
         sampler_config["random_seed"] = random_seed
         sampler_config.update(**kwargs)
         self.idata = self.sample_model(**sampler_config)
@@ -587,31 +591,30 @@
 
         Returns
         -------
         prior_predictive_samples : DataArray, shape (n_pred, samples)
             Prior predictive samples for each input X_pred
         """
         if y_pred is None:
-            y_pred = np.zeros(len(X_pred))
+            y_pred = pd.Series(np.zeros(len(X_pred)), name=self.output_var)
         if samples is None:
             samples = self.sampler_config.get("draws", 500)
 
         if self.model is None:
             self.build_model(X_pred, y_pred)
-
-        self._data_setter(X_pred, y_pred)
-        if self.model is not None:
-            with self.model:  # sample with new input data
-                prior_pred: az.InferenceData = pm.sample_prior_predictive(samples, **kwargs)
-                self.set_idata_attrs(prior_pred)
-                if extend_idata:
-                    if self.idata is not None:
-                        self.idata.extend(prior_pred)
-                    else:
-                        self.idata = prior_pred
+        else:
+            self._data_setter(X_pred, y_pred)
+        with self.model:  # sample with new input data
+            prior_pred: az.InferenceData = pm.sample_prior_predictive(samples, **kwargs)
+            self.set_idata_attrs(prior_pred)
+            if extend_idata:
+                if self.idata is not None:
+                    self.idata.extend(prior_pred, join="right")
+                else:
+                    self.idata = prior_pred
 
         prior_predictive_samples = az.extract(prior_pred, "prior_predictive", combined=combined)
 
         return prior_predictive_samples
 
     def sample_posterior_predictive(self, X_pred, extend_idata, combined, **kwargs):
         """
@@ -633,15 +636,15 @@
             Posterior predictive samples for each input X_pred
         """
         self._data_setter(X_pred)
 
         with self.model:  # sample with new input data
             post_pred = pm.sample_posterior_predictive(self.idata, **kwargs)
             if extend_idata:
-                self.idata.extend(post_pred)
+                self.idata.extend(post_pred, join="right")
 
         posterior_predictive_samples = az.extract(
             post_pred, "posterior_predictive", combined=combined
         )
 
         return posterior_predictive_samples
```

### Comparing `pymc-experimental-0.0.9/pymc_experimental/preprocessing/standard_scaler.py` & `pymc_experimental-0.1.0/pymc_experimental/preprocessing/standard_scaler.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.9/pymc_experimental/tests/__init__.py` & `pymc_experimental-0.1.0/pymc_experimental/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.9/pymc_experimental/tests/distributions/__init__.py` & `pymc_experimental-0.1.0/pymc_experimental/tests/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.9/pymc_experimental/tests/distributions/test_continuous.py` & `pymc_experimental-0.1.0/pymc_experimental/tests/distributions/test_continuous.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,53 +7,47 @@
 #       http://www.apache.org/licenses/LICENSE-2.0
 #
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
-import platform
-
 import numpy as np
 import pymc as pm
 
 # general imports
-import pytensor
 import pytest
 import scipy.stats.distributions as sp
 
 # test support imports from pymc
 from pymc.testing import (
     BaseTestDistributionRandom,
     Domain,
     R,
+    Rplus,
     Rplusbig,
-    assert_moment_is_expected,
+    assert_support_point_is_expected,
     check_logcdf,
     check_logp,
     seeded_scipy_distribution_builder,
     select_by_precision,
 )
 
 # the distributions to be tested
-from pymc_experimental.distributions import GenExtreme
+from pymc_experimental.distributions import Chi, GenExtreme, Maxwell
 
 
 class TestGenExtremeClass:
     """
     Wrapper class so that tests of experimental additions can be dropped into
     PyMC directly on adoption.
 
     pm.logp(GenExtreme.dist(mu=0.,sigma=1.,xi=0.5),value=-0.01)
     """
 
-    @pytest.mark.xfail(
-        condition=(pytensor.config.floatX == "float32"),
-        reason="PyMC underflows earlier than scipy on float32",
-    )
     def test_logp(self):
         def ref_logp(value, mu, sigma, xi):
             if 1 + xi * (value - mu) / sigma > 0:
                 return sp.genextreme.logpdf(value, c=-xi, loc=mu, scale=sigma)
             else:
                 return -np.inf
 
@@ -64,21 +58,14 @@
                 "mu": R,
                 "sigma": Rplusbig,
                 "xi": Domain([-1, -0.99, -0.5, 0, 0.5, 0.99, 1]),
             },
             ref_logp,
         )
 
-        if pytensor.config.floatX == "float32":
-            raise Exception("Flaky test: It passed this time, but XPASS is not allowed.")
-
-    @pytest.mark.skipif(
-        (pytensor.config.floatX == "float32" and platform.system() == "Windows"),
-        reason="Scipy gives different results on Windows and does not match with desired accuracy",
-    )
     def test_logcdf(self):
         def ref_logcdf(value, mu, sigma, xi):
             if 1 + xi * (value - mu) / sigma > 0:
                 return sp.genextreme.logcdf(value, c=-xi, loc=mu, scale=sigma)
             else:
                 return -np.inf
 
@@ -120,18 +107,18 @@
                     + np.arange(1, 7)
                     * ((1 + np.linspace(-0.2, 0.2, 6)) ** -np.linspace(-0.2, 0.2, 6) - 1)
                     / np.linspace(-0.2, 0.2, 6),
                 ),
             ),
         ],
     )
-    def test_genextreme_moment(self, mu, sigma, xi, size, expected):
+    def test_genextreme_support_point(self, mu, sigma, xi, size, expected):
         with pm.Model() as model:
             GenExtreme("x", mu=mu, sigma=sigma, xi=xi, size=size)
-        assert_moment_is_expected(model, expected)
+        assert_support_point_is_expected(model, expected)
 
     def test_gen_extreme_scipy_kwarg(self):
         dist = GenExtreme.dist(xi=1, scipy=False)
         assert dist.owner.inputs[-1].eval() == 1
 
         dist = GenExtreme.dist(xi=1, scipy=True)
         assert dist.owner.inputs[-1].eval() == -1
@@ -145,7 +132,53 @@
     reference_dist_params = {"loc": 0, "scale": 1, "c": 0.1}
     reference_dist = seeded_scipy_distribution_builder("genextreme")
     tests_to_run = [
         "check_pymc_params_match_rv_op",
         "check_pymc_draws_match_reference",
         "check_rv_size",
     ]
+
+
+class TestChiClass:
+    """
+    Wrapper class so that tests of experimental additions can be dropped into
+    PyMC directly on adoption.
+    """
+
+    def test_logp(self):
+        check_logp(
+            Chi,
+            Rplus,
+            {"nu": Rplus},
+            lambda value, nu: sp.chi.logpdf(value, df=nu),
+        )
+
+    def test_logcdf(self):
+        check_logcdf(
+            Chi,
+            Rplus,
+            {"nu": Rplus},
+            lambda value, nu: sp.chi.logcdf(value, df=nu),
+        )
+
+
+class TestMaxwell:
+    """
+    Wrapper class so that tests of experimental additions can be dropped into
+    PyMC directly on adoption.
+    """
+
+    def test_logp(self):
+        check_logp(
+            Maxwell,
+            Rplus,
+            {"a": Rplus},
+            lambda value, a: sp.maxwell.logpdf(value, scale=a),
+        )
+
+    def test_logcdf(self):
+        check_logcdf(
+            Maxwell,
+            Rplus,
+            {"a": Rplus},
+            lambda value, a: sp.maxwell.logcdf(value, scale=a),
+        )
```

### Comparing `pymc-experimental-0.0.9/pymc_experimental/tests/distributions/test_discrete_markov_chain.py` & `pymc_experimental-0.1.0/pymc_experimental/tests/distributions/test_discrete_markov_chain.py`

 * *Files 6% similar despite different names*

```diff
@@ -86,18 +86,27 @@
 
         assert logp.shape == (5,)
 
     def test_logp_with_default_init_dist(self):
         P = pt.as_tensor_variable(np.array([[0.1, 0.5, 0.4], [0.3, 0.4, 0.3], [0.9, 0.05, 0.05]]))
         x0 = pm.Categorical.dist(p=np.ones(3) / 3)
 
+        value = np.array([0, 1, 2])
+        logp_expected = np.log((1 / 3) * 0.5 * 0.3)
+
+        # Test dist directly
         chain = DiscreteMarkovChain.dist(P=P, init_dist=x0, steps=3)
+        logp_eval = pm.logp(chain, value).eval()
+        np.testing.assert_allclose(logp_eval, logp_expected, rtol=1e-6)
 
-        logp = pm.logp(chain, [0, 1, 2]).eval()
-        assert logp == pytest.approx(np.log((1 / 3) * 0.5 * 0.3), rel=1e-6)
+        # Test via Model
+        with pm.Model() as m:
+            DiscreteMarkovChain("chain", P=P, init_dist=x0, steps=3)
+        model_logp_eval = m.compile_logp()({"chain": value})
+        np.testing.assert_allclose(model_logp_eval, logp_expected, rtol=1e-6)
 
     def test_logp_with_user_defined_init_dist(self):
         P = pt.as_tensor_variable(np.array([[0.1, 0.5, 0.4], [0.3, 0.4, 0.3], [0.9, 0.05, 0.05]]))
         x0 = pm.Categorical.dist(p=[0.2, 0.6, 0.2])
         chain = DiscreteMarkovChain.dist(P=P, init_dist=x0, steps=3)
 
         logp = pm.logp(chain, [0, 1, 2]).eval()
@@ -116,15 +125,15 @@
 
         chain_np = np.empty(shape=n_steps + 1, dtype="int8")
         chain_np[0] = np.argmax(x0_np)
         for i in range(n_steps):
             state = chain_np[i]
             chain_np[i + 1] = np.argmax(P_np[state])
 
-        dmc_chain = pm.distributions.distribution.moment(chain).eval()
+        dmc_chain = pm.distributions.distribution.support_point(chain).eval()
 
         assert np.allclose(dmc_chain, chain_np)
 
     def test_define_steps_via_shape_arg(self):
         P = pt.full((3, 3), 1 / 3)
         x0 = pm.Categorical.dist(p=np.ones(3) / 3)
```

### Comparing `pymc-experimental-0.0.9/pymc_experimental/tests/distributions/test_multivariate.py` & `pymc_experimental-0.1.0/pymc_experimental/tests/distributions/test_multivariate.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,14 +4,19 @@
 import pytest
 
 import pymc_experimental as pmx
 
 
 class TestR2D2M2CP:
     @pytest.fixture(autouse=True)
+    def fast_compile(self):
+        with pytensor.config.change_flags(mode="FAST_COMPILE", exception_verbosity="high"):
+            yield
+
+    @pytest.fixture(autouse=True)
     def model(self):
         # every method is within a model
         with pm.Model() as model:
             yield model
 
     @pytest.fixture(params=[True, False], ids=["centered", "non-centered"])
     def centered(self, request):
@@ -92,53 +97,95 @@
 
     @pytest.fixture(params=["concentration", "no-concentration"])
     def phi_args(self, request, phi_args_base):
         if request.param == "concentration":
             phi_args_base["importance_concentration"] = 10
         return phi_args_base
 
-    @pytest.mark.skipif(
-        pytensor.config.floatX == "float32",
-        reason="pytensor.config.floatX == 'float32', https://github.com/pymc-devs/pymc/issues/6779",
-    )
-    def test_init(
+    def test_init_r2(
         self,
         dims,
-        centered,
         input_std,
         output_std,
         r2,
         r2_std,
-        positive_probs,
-        positive_probs_std,
-        phi_args,
         model: pm.Model,
     ):
         eps, beta = pmx.distributions.R2D2M2CP(
             "beta",
             output_std,
             input_std,
             dims=dims,
             r2=r2,
             r2_std=r2_std,
-            centered=centered,
-            positive_probs_std=positive_probs_std,
-            positive_probs=positive_probs,
-            **phi_args
         )
         assert not np.isnan(beta.eval()).any()
         assert eps.eval().shape == output_std.shape
         assert beta.eval().shape == input_std.shape
         # r2 rv is only created if r2 std is not None
         assert "beta" in model.named_vars
         assert ("beta::r2" in model.named_vars) == (r2_std is not None), set(model.named_vars)
         # phi is only created if variable importance is not None and there is more than one var
+        assert np.isfinite(model.compile_logp()(model.initial_point()))
+
+    def test_init_importance(
+        self,
+        dims,
+        centered,
+        input_std,
+        output_std,
+        phi_args,
+        model: pm.Model,
+    ):
+        eps, beta = pmx.distributions.R2D2M2CP(
+            "beta",
+            output_std,
+            input_std,
+            dims=dims,
+            r2=1,
+            centered=centered,
+            **phi_args,
+        )
+        assert not np.isnan(beta.eval()).any()
+        assert eps.eval().shape == output_std.shape
+        assert beta.eval().shape == input_std.shape
+        # r2 rv is only created if r2 std is not None
+        assert "beta" in model.named_vars
+        # phi is only created if variable importance is not None and there is more than one var
         assert ("beta::phi" in model.named_vars) == (
             "variables_importance" in phi_args or "importance_concentration" in phi_args
         ), set(model.named_vars)
+        assert np.isfinite(model.compile_logp()(model.initial_point()))
+
+    def test_init_positive_probs(
+        self,
+        dims,
+        centered,
+        input_std,
+        output_std,
+        positive_probs,
+        positive_probs_std,
+        model: pm.Model,
+    ):
+        eps, beta = pmx.distributions.R2D2M2CP(
+            "beta",
+            output_std,
+            input_std,
+            dims=dims,
+            r2=1.0,
+            centered=centered,
+            positive_probs_std=positive_probs_std,
+            positive_probs=positive_probs,
+        )
+        assert not np.isnan(beta.eval()).any()
+        assert eps.eval().shape == output_std.shape
+        assert beta.eval().shape == input_std.shape
+        # r2 rv is only created if r2 std is not None
+        assert "beta" in model.named_vars
+        # phi is only created if variable importance is not None and there is more than one var
         assert ("beta::psi" in model.named_vars) == (
             positive_probs_std is not None and positive_probs_std.any()
         ), set(model.named_vars)
         assert np.isfinite(sum(model.point_logps().values()))
 
     def test_failing_importance(self, dims, input_shape, output_std, input_std):
         if input_shape[-1] < 2:
@@ -251,31 +298,7 @@
         b = pmx.distributions.R2D2M2CP("b1", 1, [1, 1], r2=0.5, positive_probs=[1, 1], dims="a")
         assert not model.free_RVs, model.free_RVs
 
         b = pmx.distributions.R2D2M2CP(
             "b2", 1, [1, 1], r2=0.5, positive_probs=[1, 1], positive_probs_std=[0, 0], dims="a"
         )
         assert not model.free_RVs, model.free_RVs
-
-    def test_immutable_dims(self, model: pm.Model):
-        model.add_coord("a", range(2), mutable=True)
-        model.add_coord("b", range(2), mutable=False)
-        with pytest.raises(ValueError, match="should be constant length immutable dims"):
-            pmx.distributions.R2D2M2CP(
-                "beta0",
-                1,
-                [1, 1],
-                dims="a",
-                r2=0.8,
-                positive_probs=[0.5, 1],
-                positive_probs_std=[0.3, 0],
-            )
-        with pytest.raises(ValueError, match="should be constant length immutable dims"):
-            pmx.distributions.R2D2M2CP(
-                "beta0",
-                1,
-                [1, 1],
-                dims=("a", "b"),
-                r2=0.8,
-                positive_probs=[0.5, 1],
-                positive_probs_std=[0.3, 0],
-            )
```

### Comparing `pymc-experimental-0.0.9/pymc_experimental/tests/test_histogram_approximation.py` & `pymc_experimental-0.1.0/pymc_experimental/tests/test_histogram_approximation.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.9/pymc_experimental/tests/test_linearmodel.py` & `pymc_experimental-0.1.0/pymc_experimental/tests/test_linearmodel.py`

 * *Files 21% similar despite different names*

```diff
@@ -33,38 +33,48 @@
     set_config(transform_output="pandas")
     sklearn_available = True
 except ImportError:
     sklearn_available = False
 
 
 @pytest.fixture(scope="module")
+def toy_actual_params():
+    return {
+        "intercept": 3,
+        "slope": 5,
+        "obs_error": 0.5,
+    }
+
+
+@pytest.fixture(scope="module")
 def toy_X():
     x = np.linspace(start=0, stop=1, num=100)
     X = pd.DataFrame({"input": x})
     return X
 
 
 @pytest.fixture(scope="module")
-def toy_y(toy_X):
-    y = 5 * toy_X["input"] + 3
-    y = y + np.random.normal(0, 1, size=len(toy_X))
+def toy_y(toy_X, toy_actual_params):
+    y = toy_actual_params["slope"] * toy_X["input"] + toy_actual_params["intercept"]
+    rng = np.random.default_rng(427)
+    y = y + rng.normal(0, toy_actual_params["obs_error"], size=len(toy_X))
     y = pd.Series(y, name="output")
     return y
 
 
 @pytest.fixture(scope="module")
 def fitted_linear_model_instance(toy_X, toy_y):
     sampler_config = {
-        "draws": 500,
-        "tune": 300,
+        "draws": 50,
+        "tune": 30,
         "chains": 2,
         "target_accept": 0.95,
     }
     model = LinearModel(sampler_config=sampler_config)
-    model.fit(toy_X, toy_y)
+    model.fit(toy_X, toy_y, random_seed=312)
     return model
 
 
 @pytest.mark.skipif(
     sys.platform == "win32", reason="Permissions for temp files not granted on windows CI."
 )
 def test_save_load(fitted_linear_model_instance):
@@ -97,30 +107,47 @@
     assert len(new_X_pred) == len(pred)
     assert isinstance(pred, np.ndarray)
     post_pred = model.predict_posterior(new_X_pred)
     assert len(new_X_pred) == len(post_pred)
     assert isinstance(post_pred, xr.DataArray)
 
 
+def test_parameter_fit(toy_X, toy_y, toy_actual_params):
+    """Check that the fit model recovered the data-generating parameters."""
+    # Fit the model with a sufficient number of samples
+    sampler_config = {
+        "draws": 500,
+        "tune": 300,
+        "chains": 2,
+        "target_accept": 0.95,
+    }
+    model = LinearModel(sampler_config=sampler_config)
+    model.fit(toy_X, toy_y, random_seed=312)
+    fit_params = model.idata.posterior.mean()
+    np.testing.assert_allclose(fit_params["intercept"], toy_actual_params["intercept"], rtol=0.1)
+    np.testing.assert_allclose(fit_params["slope"], toy_actual_params["slope"], rtol=0.1)
+    np.testing.assert_allclose(fit_params["σ_model_fmc"], toy_actual_params["obs_error"], rtol=0.1)
+
+
 def test_predict(fitted_linear_model_instance):
     model = fitted_linear_model_instance
     X_pred = pd.DataFrame({"input": np.random.uniform(low=0, high=1, size=100)})
     pred = model.predict(X_pred)
     assert len(X_pred) == len(pred)
     assert np.issubdtype(pred.dtype, np.floating)
 
 
 @pytest.mark.parametrize("combined", [True, False])
 def test_predict_posterior(fitted_linear_model_instance, combined):
     model = fitted_linear_model_instance
     n_pred = 150
     X_pred = pd.DataFrame({"input": np.random.uniform(low=0, high=1, size=n_pred)})
     pred = model.predict_posterior(X_pred, combined=combined)
-    chains = model.idata.sample_stats.dims["chain"]
-    draws = model.idata.sample_stats.dims["draw"]
+    chains = model.idata.sample_stats.sizes["chain"]
+    draws = model.idata.sample_stats.sizes["draw"]
     expected_shape = (n_pred, chains * draws) if combined else (chains, draws, n_pred)
     assert pred.shape == expected_shape
     assert np.issubdtype(pred.dtype, np.floating)
     # TODO: check that extend_idata has the expected effect
 
 
 @pytest.mark.parametrize("samples", [None, 300])
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pymc-experimental-0.0.9/pymc_experimental/tests/test_model_builder.py` & `pymc_experimental-0.1.0/pymc_experimental/tests/test_model_builder.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 
 import hashlib
 import json
 import sys
 import tempfile
-from typing import Dict
+from typing import Dict, Union
 
 import numpy as np
 import pandas as pd
 import pymc as pm
 import pytest
 
 from pymc_experimental.model_builder import ModelBuilder
@@ -37,31 +37,56 @@
 def toy_y(toy_X):
     y = 5 * toy_X["input"] + 3
     y = y + np.random.normal(0, 1, size=len(toy_X))
     y = pd.Series(y, name="output")
     return y
 
 
-@pytest.fixture(scope="module")
-def fitted_model_instance(toy_X, toy_y):
+def get_unfitted_model_instance(X, y):
+    """Creates an unfitted model instance to which idata can be copied in
+    and then used as a fitted model instance. That way a fitted model
+    can be used multiple times without having to run `fit` multiple times."""
     sampler_config = {
-        "draws": 100,
-        "tune": 100,
+        "draws": 20,
+        "tune": 10,
         "chains": 2,
         "target_accept": 0.95,
     }
     model_config = {
         "a": {"loc": 0, "scale": 10, "dims": ("numbers",)},
         "b": {"loc": 0, "scale": 10},
         "obs_error": 2,
     }
     model = test_ModelBuilder(
         model_config=model_config, sampler_config=sampler_config, test_parameter="test_paramter"
     )
-    model.fit(toy_X)
+    # Do the things that `model.fit` does except sample to create idata.
+    model._generate_and_preprocess_model_data(X, y.values.flatten())
+    model.build_model(X, y)
+    return model
+
+
+@pytest.fixture(scope="module")
+def fitted_model_instance_base(toy_X, toy_y):
+    """Because fitting takes a relatively long time, this is intended to
+    be used only once and then have new instances created and fit data patched in
+    for tests that use a fitted model instance. Tests should use
+    `fitted_model_instance` instead of this."""
+    model = get_unfitted_model_instance(toy_X, toy_y)
+    model.fit(toy_X, toy_y)
+    return model
+
+
+@pytest.fixture
+def fitted_model_instance(toy_X, toy_y, fitted_model_instance_base):
+    """Get a fitted model instance. A new instance is created and fit data is
+    patched in, so tests using this fixture can modify the model object without
+    affecting other tests."""
+    model = get_unfitted_model_instance(toy_X, toy_y)
+    model.idata = fitted_model_instance_base.idata.copy()
     return model
 
 
 class test_ModelBuilder(ModelBuilder):
     def __init__(self, model_config=None, sampler_config=None, test_parameter=None):
         self.test_parameter = test_parameter
         super().__init__(model_config=model_config, sampler_config=sampler_config)
@@ -70,17 +95,17 @@
     version = "0.1"
 
     def build_model(self, X: pd.DataFrame, y: pd.Series, model_config=None):
         coords = {"numbers": np.arange(len(X))}
         self.generate_and_preprocess_model_data(X, y)
         with pm.Model(coords=coords) as self.model:
             if model_config is None:
-                model_config = self.default_model_config
-            x = pm.MutableData("x", self.X["input"].values)
-            y_data = pm.MutableData("y_data", self.y)
+                model_config = self.model_config
+            x = pm.Data("x", self.X["input"].values)
+            y_data = pm.Data("y_data", self.y)
 
             # prior parameters
             a_loc = model_config["a"]["loc"]
             a_scale = model_config["a"]["scale"]
             b_loc = model_config["b"]["loc"]
             b_scale = model_config["b"]["scale"]
             obs_error = model_config["obs_error"]
@@ -110,36 +135,45 @@
     def _serializable_model_config(self):
         return self.model_config
 
     def generate_and_preprocess_model_data(self, X: pd.DataFrame, y: pd.Series):
         self.X = X
         self.y = y
 
-    @property
-    def default_model_config(self) -> Dict:
+    @staticmethod
+    def get_default_model_config() -> Dict:
         return {
             "a": {"loc": 0, "scale": 10, "dims": ("numbers",)},
             "b": {"loc": 0, "scale": 10},
             "obs_error": 2,
         }
 
-    @property
-    def default_sampler_config(self) -> Dict:
+    def _generate_and_preprocess_model_data(
+        self, X: Union[pd.DataFrame, pd.Series], y: pd.Series
+    ) -> None:
+        self.X = X
+        self.y = y
+
+    @staticmethod
+    def get_default_sampler_config() -> Dict:
         return {
-            "draws": 1_000,
-            "tune": 1_000,
+            "draws": 10,
+            "tune": 10,
             "chains": 3,
             "target_accept": 0.95,
         }
 
 
 def test_save_input_params(fitted_model_instance):
     assert fitted_model_instance.idata.attrs["test_paramter"] == '"test_paramter"'
 
 
+@pytest.mark.skipif(
+    sys.platform == "win32", reason="Permissions for temp files not granted on windows CI."
+)
 def test_save_load(fitted_model_instance):
     temp = tempfile.NamedTemporaryFile(mode="w", encoding="utf-8", delete=False)
     fitted_model_instance.save(temp.name)
     test_builder2 = test_ModelBuilder.load(temp.name)
     assert fitted_model_instance.idata.groups() == test_builder2.idata.groups()
     assert fitted_model_instance.id == test_builder2.id
     x_pred = np.random.uniform(low=0, high=1, size=100)
@@ -177,23 +211,20 @@
         prediction_data["input"], extend_idata=True, combined=True
     )
     post_pred[fitted_model_instance.output_var].shape[0] == prediction_data.input.shape
 
 
 def test_fit_no_y(toy_X):
     model_builder = test_ModelBuilder()
-    model_builder.idata = model_builder.fit(X=toy_X)
+    model_builder.idata = model_builder.fit(X=toy_X, chains=1, tune=1, draws=1)
     assert model_builder.model is not None
     assert model_builder.idata is not None
     assert "posterior" in model_builder.idata.groups()
 
 
-@pytest.mark.skipif(
-    sys.platform == "win32", reason="Permissions for temp files not granted on windows CI."
-)
 def test_predict(fitted_model_instance):
     x_pred = np.random.uniform(low=0, high=1, size=100)
     prediction_data = pd.DataFrame({"input": x_pred})
     pred = fitted_model_instance.predict(prediction_data["input"])
     # Perform elementwise comparison using numpy
     assert type(pred) == np.ndarray
     assert len(pred) > 0
@@ -203,21 +234,56 @@
 def test_sample_posterior_predictive(fitted_model_instance, combined):
     n_pred = 100
     x_pred = np.random.uniform(low=0, high=1, size=n_pred)
     prediction_data = pd.DataFrame({"input": x_pred})
     pred = fitted_model_instance.sample_posterior_predictive(
         prediction_data["input"], combined=combined, extend_idata=True
     )
-    chains = fitted_model_instance.idata.sample_stats.dims["chain"]
-    draws = fitted_model_instance.idata.sample_stats.dims["draw"]
+    chains = fitted_model_instance.idata.sample_stats.sizes["chain"]
+    draws = fitted_model_instance.idata.sample_stats.sizes["draw"]
     expected_shape = (n_pred, chains * draws) if combined else (chains, draws, n_pred)
     assert pred[fitted_model_instance.output_var].shape == expected_shape
     assert np.issubdtype(pred[fitted_model_instance.output_var].dtype, np.floating)
 
 
+@pytest.mark.parametrize("group", ["prior_predictive", "posterior_predictive"])
+@pytest.mark.parametrize("extend_idata", [True, False])
+def test_sample_xxx_extend_idata_param(fitted_model_instance, group, extend_idata):
+    output_var = fitted_model_instance.output_var
+    idata_prev = fitted_model_instance.idata[group][output_var]
+
+    # Since coordinates are provided, the dimension must match
+    n_pred = 100  # Must match toy_x
+    x_pred = np.random.uniform(0, 1, n_pred)
+
+    prediction_data = pd.DataFrame({"input": x_pred})
+    if group == "prior_predictive":
+        prediction_method = fitted_model_instance.sample_prior_predictive
+    else:  # group == "posterior_predictive":
+        prediction_method = fitted_model_instance.sample_posterior_predictive
+
+    pred = prediction_method(prediction_data["input"], combined=False, extend_idata=extend_idata)
+
+    pred_unstacked = pred[output_var].values
+    idata_now = fitted_model_instance.idata[group][output_var].values
+
+    if extend_idata:
+        # After sampling, data in the model should be the same as the predictions
+        np.testing.assert_array_equal(idata_now, pred_unstacked)
+        # Data in the model should NOT be the same as before
+        if idata_now.shape == idata_prev.values.shape:
+            assert np.sum(np.abs(idata_now - idata_prev.values) < 1e-5) <= 2
+    else:
+        # After sampling, data in the model should be the same as it was before
+        np.testing.assert_array_equal(idata_now, idata_prev.values)
+        # Data in the model should NOT be the same as the predictions
+        if idata_now.shape == pred_unstacked.shape:
+            assert np.sum(np.abs(idata_now - pred_unstacked) < 1e-5) <= 2
+
+
 def test_model_config_formatting():
     model_config = {
         "a": {
             "loc": [0, 0],
             "scale": 10,
             "dims": [
                 "x",
```

### Comparing `pymc-experimental-0.0.9/pymc_experimental/tests/test_pathfinder.py` & `pymc_experimental-0.1.0/pymc_experimental/tests/test_pathfinder.py`

 * *Files 18% similar despite different names*

```diff
@@ -25,23 +25,21 @@
 def test_pathfinder():
     # Data of the Eight Schools Model
     J = 8
     y = np.array([28.0, 8.0, -3.0, 7.0, -1.0, 1.0, 18.0, 12.0])
     sigma = np.array([15.0, 10.0, 16.0, 11.0, 9.0, 11.0, 10.0, 18.0])
 
     with pm.Model() as model:
-
         mu = pm.Normal("mu", mu=0.0, sigma=10.0)
         tau = pm.HalfCauchy("tau", 5.0)
 
         theta = pm.Normal("theta", mu=0, sigma=1, shape=J)
         obs = pm.Normal("obs", mu=mu + tau * theta, sigma=sigma, shape=J, observed=y)
 
-        idata = pmx.fit(method="pathfinder", iterations=100)
+        idata = pmx.fit(method="pathfinder", random_seed=41)
 
-        assert idata is not None
-        assert "theta" in idata.posterior._variables.keys()
-        assert "tau" in idata.posterior._variables.keys()
-        assert "mu" in idata.posterior._variables.keys()
-        assert idata.posterior["mu"].shape == (1, 100)
-        assert idata.posterior["tau"].shape == (1, 100)
-        assert idata.posterior["theta"].shape == (1, 100, 8)
+    assert idata.posterior["mu"].shape == (1, 1000)
+    assert idata.posterior["tau"].shape == (1, 1000)
+    assert idata.posterior["theta"].shape == (1, 1000, 8)
+    # FIXME: pathfinder doesn't find a reasonable mean! Fix bug or choose model pathfinder can handle
+    # np.testing.assert_allclose(idata.posterior["mu"].mean(), 5.0)
+    np.testing.assert_allclose(idata.posterior["tau"].mean(), 4.15, atol=0.5)
```

### Comparing `pymc-experimental-0.0.9/pymc_experimental/tests/test_pivoted_cholesky.py` & `pymc_experimental-0.1.0/pymc_experimental/tests/test_pivoted_cholesky.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.9/pymc_experimental/tests/test_prior_from_trace.py` & `pymc_experimental-0.1.0/pymc_experimental/tests/test_prior_from_trace.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.9/pymc_experimental/tests/test_splines.py` & `pymc_experimental-0.1.0/pymc_experimental/tests/test_splines.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.9/pymc_experimental/utils/__init__.py` & `pymc_experimental-0.1.0/pymc_experimental/utils/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,15 +11,13 @@
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 
 
 from pymc_experimental.utils import prior, spline
 from pymc_experimental.utils.linear_cg import linear_cg
-from pymc_experimental.utils.model_fgraph import clone_model
 
 __all__ = (
-    "clone_model",
     "linear_cg",
     "prior",
     "spline",
 )
```

### Comparing `pymc-experimental-0.0.9/pymc_experimental/utils/linear_cg.py` & `pymc_experimental-0.1.0/pymc_experimental/utils/linear_cg.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,14 @@
     vector = masked_vector.filled(fill_value=fill_value)
     return vector
 
 
 def linear_cg_updates(
     result, alpha, residual_inner_prod, eps, beta, residual, precond_residual, curr_conjugate_vec
 ):
-
     # Everything inside _jit_linear_cg_updates
     result = result + alpha * curr_conjugate_vec
     beta = np.copy(residual_inner_prod)
 
     residual_inner_prod = residual.T @ precond_residual
 
     # safe division
@@ -64,15 +63,14 @@
     max_iter=1000,
     max_tridiag_iter=20,
     initial_guess=None,
     preconditioner=None,
     terminate_cg_by_size=False,
     use_eval_tolerange=False,
 ):
-
     if initial_guess is None:
         initial_guess = np.zeros_like(rhs)
 
     if preconditioner is None:
         preconditioner = lambda x: x
         precond = False
     else:
```

### Comparing `pymc-experimental-0.0.9/pymc_experimental/utils/pivoted_cholesky.py` & `pymc_experimental-0.1.0/pymc_experimental/utils/pivoted_cholesky.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.9/pymc_experimental/utils/prior.py` & `pymc_experimental-0.1.0/pymc_experimental/utils/prior.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,20 +15,20 @@
 
 from typing import Dict, List, Optional, Sequence, Tuple, TypedDict, Union
 
 import arviz
 import numpy as np
 import pymc as pm
 import pytensor.tensor as pt
-from pymc.logprob.transforms import RVTransform
+from pymc.logprob.transforms import Transform
 
 
 class ParamCfg(TypedDict):
     name: str
-    transform: Optional[RVTransform]
+    transform: Optional[Transform]
     dims: Optional[Union[str, Tuple[str]]]
 
 
 class ShapeInfo(TypedDict):
     # shape might not match slice due to a transform
     shape: Tuple[int]  # transformed shape
     slice: slice
@@ -40,33 +40,33 @@
 
 
 class FlatInfo(TypedDict):
     data: np.ndarray
     info: List[VarInfo]
 
 
-def _arg_to_param_cfg(key, value: Optional[Union[ParamCfg, RVTransform, str, Tuple]] = None):
+def _arg_to_param_cfg(key, value: Optional[Union[ParamCfg, Transform, str, Tuple]] = None):
     if value is None:
         cfg = ParamCfg(name=key, transform=None, dims=None)
     elif isinstance(value, Tuple):
         cfg = ParamCfg(name=key, transform=None, dims=value)
     elif isinstance(value, str):
         cfg = ParamCfg(name=value, transform=None, dims=None)
-    elif isinstance(value, RVTransform):
+    elif isinstance(value, Transform):
         cfg = ParamCfg(name=key, transform=value, dims=None)
     else:
         cfg = value.copy()
         cfg.setdefault("name", key)
         cfg.setdefault("transform", None)
         cfg.setdefault("dims", None)
     return cfg
 
 
 def _parse_args(
-    var_names: Sequence[str], **kwargs: Union[ParamCfg, RVTransform, str, Tuple]
+    var_names: Sequence[str], **kwargs: Union[ParamCfg, Transform, str, Tuple]
 ) -> Dict[str, ParamCfg]:
     results = dict()
     for var in var_names:
         results[var] = _arg_to_param_cfg(var)
     for key, val in kwargs.items():
         results[key] = _arg_to_param_cfg(key, val)
     return results
@@ -129,15 +129,15 @@
 
 
 def prior_from_idata(
     idata: arviz.InferenceData,
     name="trace_prior_",
     *,
     var_names: Sequence[str] = (),
-    **kwargs: Union[ParamCfg, RVTransform, str, Tuple]
+    **kwargs: Union[ParamCfg, Transform, str, Tuple]
 ) -> Dict[str, pt.TensorVariable]:
     """
     Create a prior from posterior using MvNormal approximation.
 
     The approximation uses MvNormal distribution.
     Keep in mind that this function will only work well for unimodal
     posteriors and will fail when complicated interactions happen.
@@ -149,15 +149,15 @@
 
     Parameters
     ----------
     idata: arviz.InferenceData
         Inference data with posterior group
     var_names: Sequence[str]
         names of variables to take as is from the posterior
-    kwargs: Union[ParamCfg, RVTransform, str, Tuple]
+    kwargs: Union[ParamCfg, Transform, str, Tuple]
         names of variables with additional configuration, see more in Examples
 
     Examples
     --------
     >>> import pymc as pm
     >>> import pymc.distributions.transforms as transforms
     >>> import numpy as np
```

### Comparing `pymc-experimental-0.0.9/pymc_experimental/utils/pytensorf.py` & `pymc_experimental-0.1.0/pymc_experimental/utils/pytensorf.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,14 @@
 
 class StringConstant(Constant):
     pass
 
 
 @pytensor._as_symbolic.register(str)
 def as_symbolic_string(x, **kwargs):
-
     return StringConstant(stringtype, x)
 
 
 def rvs_in_graph(vars: Sequence[Variable]) -> bool:
     """Check if there are any rvs in the graph of vars"""
 
     def expand(r):
```

### Comparing `pymc-experimental-0.0.9/pymc_experimental/utils/spline.py` & `pymc_experimental-0.1.0/pymc_experimental/utils/spline.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.9/pymc_experimental.egg-info/PKG-INFO` & `pymc_experimental-0.1.0/pymc_experimental.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,43 @@
 Metadata-Version: 2.1
 Name: pymc-experimental
-Version: 0.0.9
+Version: 0.1.0
 Summary: A home for new additions to PyMC, which may include unusual probability distribitions, advanced model fitting algorithms, or any code that may be inappropriate to include in the pymc repository, but may want to be made available to users.
 Home-page: http://github.com/pymc-devs/pymc-experimental
 Maintainer: PyMC Developers
 Maintainer-email: pymc.devs@gmail.com
 License: Apache License, Version 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
-Provides-Extra: dask_histogram
+License-File: LICENSE
+Requires-Dist: pymc>=5.13.0
+Requires-Dist: scikit-learn
+Provides-Extra: dask-histogram
+Requires-Dist: dask[complete]; extra == "dask-histogram"
+Requires-Dist: xhistogram; extra == "dask-histogram"
 Provides-Extra: histogram
+Requires-Dist: xhistogram; extra == "histogram"
 Provides-Extra: complete
+Requires-Dist: dask[complete]; extra == "complete"
+Requires-Dist: xhistogram; extra == "complete"
 Provides-Extra: dev
-License-File: LICENSE
+Requires-Dist: dask[all]; extra == "dev"
+Requires-Dist: blackjax; extra == "dev"
+Requires-Dist: statsmodels; extra == "dev"
 
 # Welcome to `pymc-experimental`
 <a href="https://gitpod.io/#https://github.com/pymc-devs/pymc-experimental">
   <img
     src="https://img.shields.io/badge/Contribute%20with-Gitpod-908a85?logo=gitpod"
     alt="Contribute with Gitpod"
   />
```

#### html2text {}

```diff
@@ -1,57 +1,62 @@
-Metadata-Version: 2.1 Name: pymc-experimental Version: 0.0.9 Summary: A home
+Metadata-Version: 2.1 Name: pymc-experimental Version: 0.1.0 Summary: A home
 for new additions to PyMC, which may include unusual probability distribitions,
 advanced model fitting algorithms, or any code that may be inappropriate to
 include in the pymc repository, but may want to be made available to users.
 Home-page: http://github.com/pymc-devs/pymc-experimental Maintainer: PyMC
 Developers Maintainer-email: pymc.devs@gmail.com License: Apache License,
 Version 2.0 Classifier: Development Status :: 5 - Production/Stable Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
-Approved :: Apache Software License Classifier: Intended Audience :: Science/
-Research Classifier: Topic :: Scientific/Engineering Classifier: Topic ::
-Scientific/Engineering :: Mathematics Classifier: Operating System :: OS
-Independent Requires-Python: >=3.8 Description-Content-Type: text/markdown
-Provides-Extra: dask_histogram Provides-Extra: histogram Provides-Extra:
-complete Provides-Extra: dev License-File: LICENSE # Welcome to `pymc-
-experimental` _[_C_o_n_t_r_i_b_u_t_e_ _w_i_t_h_ _G_i_t_p_o_d_][Codecov Badge]As PyMC continues to
-mature and expand its functionality to accommodate more domains of application,
-we increasingly see cutting-edge methodologies, highly specialized statistical
-distributions, and complex models appear. While this adds to the functionality
-and relevance of the project, it can also introduce instability and impose a
-burden on testing and quality control. To reduce the burden on the main `pymc`
-repository, this `pymc-experimental` repository can become the aggregator and
-testing ground for new additions to PyMC. This may include unusual probability
-distributions, advanced model fitting algorithms, innovative yet not fully
-tested methods or any code that may be inappropriate to include in the `pymc`
-repository, but may want to be made available to users. The `pymc-experimental`
-repository can be understood as the first step in the PyMC development
-pipeline, where all novel code is introduced until it is obvious that it
-belongs in the main repository. We hope that this organization improves the
-stability and streamlines the testing overhead of the `pymc` repository, while
-allowing users and developers to test and evaluate cutting-edge methods and not
-yet fully mature features. `pymc-experimental` would be designed to mirror the
-namespaces in `pymc` to make usage and migration as easy as possible. For
-example, a `ParabolicFractal` distribution could be used analogously to those
-in `pymc`: ```python import pymc as pm import pymc_experimental as pmx with
-pm.Model(): alpha = pmx.ParabolicFractal('alpha', b=1, c=1) ... ``` ##
-Questions ### What belongs in `pymc-experimental`? - newly-implemented
-statistical methods, for example step methods or model construction helpers -
-distributions that are tricky to sample from or test - infrequently-used
-fitting methods or distributions - any code that requires additional
-optimization before it can be used in practice ### What does not belong in
-`pymc-experimental`? - Case studies - Implementations that cannot be applied
-generically, for example because they are tied to variables from a toy example
-### Should there be more than one add-on repository? Since there is a lot of
-code that we may not want in the main repository, does it make sense to have
-more than one additional repository? For example, `pymc-experimental` may just
-include methods that are not fully developed, tested and trusted, while code
-that is known to work well and has adequate test coverage, but is still too
-specialized to become part of `pymc` could reside in a `pymc-extras` (or
-similar) repository. ### Unanswered questions & ToDos This project is still
-young and many things have not been answered or implemented. Please get
-involved! * What are guidelines for organizing submodules? * Proposal: No
-default imports of WIP/unstable submodules. By importing manually we can avoid
-breaking the package if a submodule breaks, for example because of an updated
-dependency.
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
+Classifier: License :: OSI Approved :: Apache Software License Classifier:
+Intended Audience :: Science/Research Classifier: Topic :: Scientific/
+Engineering Classifier: Topic :: Scientific/Engineering :: Mathematics
+Classifier: Operating System :: OS Independent Requires-Python: >=3.10
+Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+pymc>=5.13.0 Requires-Dist: scikit-learn Provides-Extra: dask-histogram
+Requires-Dist: dask[complete]; extra == "dask-histogram" Requires-Dist:
+xhistogram; extra == "dask-histogram" Provides-Extra: histogram Requires-Dist:
+xhistogram; extra == "histogram" Provides-Extra: complete Requires-Dist: dask
+[complete]; extra == "complete" Requires-Dist: xhistogram; extra == "complete"
+Provides-Extra: dev Requires-Dist: dask[all]; extra == "dev" Requires-Dist:
+blackjax; extra == "dev" Requires-Dist: statsmodels; extra == "dev" # Welcome
+to `pymc-experimental` _[_C_o_n_t_r_i_b_u_t_e_ _w_i_t_h_ _G_i_t_p_o_d_][Codecov Badge]As PyMC continues
+to mature and expand its functionality to accommodate more domains of
+application, we increasingly see cutting-edge methodologies, highly specialized
+statistical distributions, and complex models appear. While this adds to the
+functionality and relevance of the project, it can also introduce instability
+and impose a burden on testing and quality control. To reduce the burden on the
+main `pymc` repository, this `pymc-experimental` repository can become the
+aggregator and testing ground for new additions to PyMC. This may include
+unusual probability distributions, advanced model fitting algorithms,
+innovative yet not fully tested methods or any code that may be inappropriate
+to include in the `pymc` repository, but may want to be made available to
+users. The `pymc-experimental` repository can be understood as the first step
+in the PyMC development pipeline, where all novel code is introduced until it
+is obvious that it belongs in the main repository. We hope that this
+organization improves the stability and streamlines the testing overhead of the
+`pymc` repository, while allowing users and developers to test and evaluate
+cutting-edge methods and not yet fully mature features. `pymc-experimental`
+would be designed to mirror the namespaces in `pymc` to make usage and
+migration as easy as possible. For example, a `ParabolicFractal` distribution
+could be used analogously to those in `pymc`: ```python import pymc as pm
+import pymc_experimental as pmx with pm.Model(): alpha = pmx.ParabolicFractal
+('alpha', b=1, c=1) ... ``` ## Questions ### What belongs in `pymc-
+experimental`? - newly-implemented statistical methods, for example step
+methods or model construction helpers - distributions that are tricky to sample
+from or test - infrequently-used fitting methods or distributions - any code
+that requires additional optimization before it can be used in practice ###
+What does not belong in `pymc-experimental`? - Case studies - Implementations
+that cannot be applied generically, for example because they are tied to
+variables from a toy example ### Should there be more than one add-on
+repository? Since there is a lot of code that we may not want in the main
+repository, does it make sense to have more than one additional repository? For
+example, `pymc-experimental` may just include methods that are not fully
+developed, tested and trusted, while code that is known to work well and has
+adequate test coverage, but is still too specialized to become part of `pymc`
+could reside in a `pymc-extras` (or similar) repository. ### Unanswered
+questions & ToDos This project is still young and many things have not been
+answered or implemented. Please get involved! * What are guidelines for
+organizing submodules? * Proposal: No default imports of WIP/unstable
+submodules. By importing manually we can avoid breaking the package if a
+submodule breaks, for example because of an updated dependency.
```

### Comparing `pymc-experimental-0.0.9/setup.py` & `pymc_experimental-0.1.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,18 +25,17 @@
 URL = "http://github.com/pymc-devs/pymc-experimental"
 LICENSE = "Apache License, Version 2.0"
 
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "License :: OSI Approved :: Apache Software License",
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Mathematics",
     "Operating System :: OS Independent",
 ]
 
@@ -73,15 +72,14 @@
     here = os.path.abspath(os.path.dirname(__file__))
     with open(os.path.join(here, "pymc_experimental", "version.txt")) as f:
         version = f.read().strip()
     return version
 
 
 if __name__ == "__main__":
-
     setup(
         name="pymc-experimental",
         version=read_version(),
         maintainer=AUTHOR,
         maintainer_email=AUTHOR_EMAIL,
         description=DESCRIPTION,
         license=LICENSE,
@@ -90,11 +88,11 @@
         long_description_content_type="text/markdown",
         packages=find_packages(),
         # because of an upload-size limit by PyPI, we're temporarily removing docs from the tarball.
         # Also see MANIFEST.in
         # package_data={'docs': ['*']},
         include_package_data=True,
         classifiers=classifiers,
-        python_requires=">=3.8",
+        python_requires=">=3.10",
         install_requires=install_reqs,
         extras_require=extras_require,
     )
```

