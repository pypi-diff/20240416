# Comparing `tmp/nemos-0.1.0.tar.gz` & `tmp/nemos-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nemos-0.1.0.tar", last modified: Tue Nov  7 22:43:40 2023, max compression
+gzip compressed data, was "nemos-0.1.1.tar", last modified: Tue Apr 16 19:53:26 2024, max compression
```

## Comparing `nemos-0.1.0.tar` & `nemos-0.1.1.tar`

### file list

```diff
@@ -1,53 +1,123 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 22:43:40.056860 nemos-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 22:43:40.048860 nemos-0.1.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-11-07 22:43:32.000000 nemos-0.1.0/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 22:43:40.048860 nemos-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2023-11-07 22:43:32.000000 nemos-0.1.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2023-11-07 22:43:32.000000 nemos-0.1.0/.github/workflows/connect.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2900 2023-11-07 22:43:32.000000 nemos-0.1.0/.github/workflows/deploy-pure-python.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2023-11-07 22:43:32.000000 nemos-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      498 2023-11-07 22:43:32.000000 nemos-0.1.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    45579 2023-11-07 22:43:32.000000 nemos-0.1.0/CCN-letterFoot.png
--rw-r--r--   0 runner    (1001) docker     (127)    57441 2023-11-07 22:43:32.000000 nemos-0.1.0/CCN-logo-wText.png
--rw-r--r--   0 runner    (1001) docker     (127)     5581 2023-11-07 22:43:32.000000 nemos-0.1.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)      997 2023-11-07 22:43:32.000000 nemos-0.1.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2023-11-07 22:43:32.000000 nemos-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3775 2023-11-07 22:43:40.052860 nemos-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      910 2023-11-07 22:43:32.000000 nemos-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 22:43:40.048860 nemos-0.1.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 22:43:40.048860 nemos-0.1.0/docs/developers_notes/
--rw-r--r--   0 runner    (1001) docker     (127)     3265 2023-11-07 22:43:32.000000 nemos-0.1.0/docs/developers_notes/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4139 2023-11-07 22:43:32.000000 nemos-0.1.0/docs/developers_notes/basis_module.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 22:43:40.048860 nemos-0.1.0/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2023-11-07 22:43:32.000000 nemos-0.1.0/docs/examples/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3386 2023-11-07 22:43:32.000000 nemos-0.1.0/docs/examples/plot_1D_basis_function.py
--rw-r--r--   0 runner    (1001) docker     (127)    12221 2023-11-07 22:43:32.000000 nemos-0.1.0/docs/examples/plot_ND_basis_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     4303 2023-11-07 22:43:32.000000 nemos-0.1.0/docs/examples/plot_example_convolution.py
--rw-r--r--   0 runner    (1001) docker     (127)     1762 2023-11-07 22:43:32.000000 nemos-0.1.0/docs/gen_ref_pages.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2023-11-07 22:43:32.000000 nemos-0.1.0/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 22:43:40.048860 nemos-0.1.0/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (127)      308 2023-11-07 22:43:32.000000 nemos-0.1.0/docs/javascripts/katex.js
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2023-11-07 22:43:32.000000 nemos-0.1.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3552 2023-11-07 22:43:32.000000 nemos-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-07 22:43:40.056860 nemos-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 22:43:40.044860 nemos-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 22:43:40.052860 nemos-0.1.0/src/nemos/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2023-11-07 22:43:32.000000 nemos-0.1.0/src/nemos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35039 2023-11-07 22:43:32.000000 nemos-0.1.0/src/nemos/basis.py
--rw-r--r--   0 runner    (1001) docker     (127)    16853 2023-11-07 22:43:32.000000 nemos-0.1.0/src/nemos/glm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2023-11-07 22:43:32.000000 nemos-0.1.0/src/nemos/sample_points.py
--rw-r--r--   0 runner    (1001) docker     (127)    12504 2023-11-07 22:43:32.000000 nemos-0.1.0/src/nemos/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 22:43:40.052860 nemos-0.1.0/src/nemos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3775 2023-11-07 22:43:40.000000 nemos-0.1.0/src/nemos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      979 2023-11-07 22:43:40.000000 nemos-0.1.0/src/nemos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-07 22:43:40.000000 nemos-0.1.0/src/nemos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      289 2023-11-07 22:43:40.000000 nemos-0.1.0/src/nemos.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-11-07 22:43:40.000000 nemos-0.1.0/src/nemos.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 22:43:40.052860 nemos-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    72030 2023-11-07 22:43:32.000000 nemos-0.1.0/tests/test_basis.py
--rw-r--r--   0 runner    (1001) docker     (127)    11021 2023-11-07 22:43:32.000000 nemos-0.1.0/tests/test_convolution_1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2137 2023-11-07 22:43:32.000000 nemos-0.1.0/tests/test_glm_runs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2968 2023-11-07 22:43:32.000000 nemos-0.1.0/tests/test_glm_synthetic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2023-11-07 22:43:32.000000 nemos-0.1.0/tests/test_glm_synthetic_single_neuron.py
--rw-r--r--   0 runner    (1001) docker     (127)     6181 2023-11-07 22:43:32.000000 nemos-0.1.0/tests/utils_testing.py
--rw-r--r--   0 runner    (1001) docker     (127)      937 2023-11-07 22:43:32.000000 nemos-0.1.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:53:26.458010 nemos-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:53:26.438010 nemos-0.1.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-16 19:53:22.000000 nemos-0.1.1/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:53:26.438010 nemos-0.1.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-16 19:53:22.000000 nemos-0.1.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-16 19:53:22.000000 nemos-0.1.1/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:53:26.438010 nemos-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-16 19:53:22.000000 nemos-0.1.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-16 19:53:22.000000 nemos-0.1.1/.github/workflows/connect.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-16 19:53:22.000000 nemos-0.1.1/.github/workflows/deploy-pure-python.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-16 19:53:22.000000 nemos-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-16 19:53:22.000000 nemos-0.1.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    45579 2024-04-16 19:53:22.000000 nemos-0.1.1/CCN-letterFoot.png
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-16 19:53:22.000000 nemos-0.1.1/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     5581 2024-04-16 19:53:22.000000 nemos-0.1.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-16 19:53:22.000000 nemos-0.1.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-16 19:53:22.000000 nemos-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10506 2024-04-16 19:53:26.458010 nemos-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7563 2024-04-16 19:53:22.000000 nemos-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:53:26.442010 nemos-0.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)    57441 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/CCN-logo-wText.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:53:26.442010 nemos-0.1.1/docs/api_guide/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/api_guide/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/api_guide/_plot_01_basis_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/api_guide/_plot_04_pynapple_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/api_guide/_plot_05_sklearn_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/api_guide/_plot_06_magic_designer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12607 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/api_guide/plot_02_glm_demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10179 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/api_guide/plot_03_glm_pytree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6329 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/api_guide/plot_04_population_glm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:53:26.446009 nemos-0.1.1/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)   101811 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/assets/allen_data.png
+-rw-r--r--   0 runner    (1001) docker     (127)   141981 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/assets/allen_data_annotated-epochs.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   141785 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/assets/allen_data_annotated-response.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   141744 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/assets/allen_data_annotated-stimulus.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   142136 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/assets/allen_data_annotated-units.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    85629 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/assets/allen_data_annotated.gif
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/assets/extra.css
+-rw-r--r--   0 runner    (1001) docker     (127)   130022 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/assets/glm_features_scheme.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    62970 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/assets/glm_population_scheme.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   133950 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/assets/glm_scheme.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    24604 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/assets/lnp_model.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:53:26.446009 nemos-0.1.1/docs/background/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/background/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/background/_plot_04_modeling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:53:26.446009 nemos-0.1.1/docs/background/background_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/background/background_utils/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7874 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/background/plot_00_conceptual_intro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5344 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/background/plot_01_1D_basis_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12123 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/background/plot_02_ND_basis_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5158 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/background/plot_03_1D_convolution.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:53:26.446009 nemos-0.1.1/docs/developers_notes/
+-rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/developers_notes/01-basis_module.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6673 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/developers_notes/02-base_class.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/developers_notes/03-observation_models.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10869 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/developers_notes/04-regularizer.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5355 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/developers_notes/05-glm.md
+-rw-r--r--   0 runner    (1001) docker     (127)   294441 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/developers_notes/GLM_scheme.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/developers_notes/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/gallery_conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/gen_ref_pages.py
+-rw-r--r--   0 runner    (1001) docker     (127)   100847 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/head_dir_tuning.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     7513 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/installation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:53:26.450010 nemos-0.1.1/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/javascripts/katex.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:53:26.450010 nemos-0.1.1/docs/neural_modeling/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/neural_modeling/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:53:26.450010 nemos-0.1.1/docs/neural_modeling/examples_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/neural_modeling/examples_utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8886 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/neural_modeling/examples_utils/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/neural_modeling/examples_utils/nemos.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (127)    31660 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/neural_modeling/examples_utils/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28528 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/neural_modeling/plot_01_current_injection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21504 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/neural_modeling/plot_02_head_direction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7636 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/neural_modeling/plot_03_grid_cells.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8032 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/neural_modeling/plot_04_v1_cells.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14979 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/neural_modeling/plot_05_place_cells.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6310 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-04-16 19:53:22.000000 nemos-0.1.1/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-04-16 19:53:22.000000 nemos-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 19:53:26.458010 nemos-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:53:26.434010 nemos-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:53:26.454010 nemos-0.1.1/src/nemos/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-16 19:53:22.000000 nemos-0.1.1/src/nemos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10093 2024-04-16 19:53:22.000000 nemos-0.1.1/src/nemos/base_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61643 2024-04-16 19:53:22.000000 nemos-0.1.1/src/nemos/basis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12222 2024-04-16 19:53:22.000000 nemos-0.1.1/src/nemos/convolve.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-16 19:53:22.000000 nemos-0.1.1/src/nemos/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41490 2024-04-16 19:53:22.000000 nemos-0.1.1/src/nemos/glm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20962 2024-04-16 19:53:22.000000 nemos-0.1.1/src/nemos/observation_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5731 2024-04-16 19:53:22.000000 nemos-0.1.1/src/nemos/proximal_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-04-16 19:53:22.000000 nemos-0.1.1/src/nemos/pytrees.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17005 2024-04-16 19:53:22.000000 nemos-0.1.1/src/nemos/regularizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12561 2024-04-16 19:53:22.000000 nemos-0.1.1/src/nemos/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5431 2024-04-16 19:53:22.000000 nemos-0.1.1/src/nemos/tree_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11651 2024-04-16 19:53:22.000000 nemos-0.1.1/src/nemos/type_casting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16789 2024-04-16 19:53:22.000000 nemos-0.1.1/src/nemos/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8715 2024-04-16 19:53:22.000000 nemos-0.1.1/src/nemos/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:53:26.458010 nemos-0.1.1/src/nemos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10506 2024-04-16 19:53:26.000000 nemos-0.1.1/src/nemos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-04-16 19:53:26.000000 nemos-0.1.1/src/nemos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 19:53:26.000000 nemos-0.1.1/src/nemos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-16 19:53:26.000000 nemos-0.1.1/src/nemos.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-16 19:53:26.000000 nemos-0.1.1/src/nemos.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:53:26.458010 nemos-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    14454 2024-04-16 19:53:22.000000 nemos-0.1.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)   103841 2024-04-16 19:53:22.000000 nemos-0.1.1/tests/simulate_coupled_neurons_params.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-04-16 19:53:22.000000 nemos-0.1.1/tests/test_base_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)   162098 2024-04-16 19:53:22.000000 nemos-0.1.1/tests/test_basis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15751 2024-04-16 19:53:22.000000 nemos-0.1.1/tests/test_convolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74427 2024-04-16 19:53:22.000000 nemos-0.1.1/tests/test_glm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8974 2024-04-16 19:53:22.000000 nemos-0.1.1/tests/test_observation_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5202 2024-04-16 19:53:22.000000 nemos-0.1.1/tests/test_proximal_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5969 2024-04-16 19:53:22.000000 nemos-0.1.1/tests/test_pytrees.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34407 2024-04-16 19:53:22.000000 nemos-0.1.1/tests/test_regularizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19890 2024-04-16 19:53:22.000000 nemos-0.1.1/tests/test_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-04-16 19:53:22.000000 nemos-0.1.1/tests/test_tree_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13436 2024-04-16 19:53:22.000000 nemos-0.1.1/tests/test_type_casting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18485 2024-04-16 19:53:22.000000 nemos-0.1.1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6657 2024-04-16 19:53:22.000000 nemos-0.1.1/tests/test_vallidation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6181 2024-04-16 19:53:22.000000 nemos-0.1.1/tests/utils_testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-16 19:53:22.000000 nemos-0.1.1/tox.ini
```

### Comparing `nemos-0.1.0/.github/workflows/ci.yml` & `nemos-0.1.1/.github/workflows/ci.yml`

 * *Files 12% similar despite different names*

```diff
@@ -4,21 +4,24 @@
    workflow_dispatch:
    schedule:
      - cron: 0 0 1 * 0     # monthly
    pull_request:
      branches:
        - main
        - development
+   push:
+     branches:
+       - main
 
 jobs:
   tox:
     strategy:
       matrix:
-        os: [ubuntu-latest] #[ubuntu-latest, macos-latest, windows-latest]
-        python-version: ['3.10'] #['3.8', '3.9', '3.10']
+        os: [ubuntu-latest, macos-latest, windows-latest]
+        python-version: ['3.9','3.10', '3.11']
     runs-on: ${{ matrix.os }}
     steps:
       - name: Checkout code
         uses: actions/checkout@v3
 
       - name: Set up Python
         uses: actions/setup-python@v4 # Use v4 for compatibility with pyproject.toml
@@ -31,14 +34,19 @@
           python -m pip install --upgrade pip
           python -m pip install .
           pip install tox
 
       - name: Run tox
         run: tox -e py
 
+      - name: Upload coverage reports to Codecov
+        uses: codecov/codecov-action@v3
+        env:
+          CODECOV_TOKEN: ${{ secrets.CODECOV_TOKEN }}
+
   check:
     if: always()
     needs: tox
     runs-on: ubuntu-latest
     steps:
       - name: Decide whether all tests and notebooks succeeded
         uses: re-actors/alls-green@v1.2.2
```

### Comparing `nemos-0.1.0/.github/workflows/connect.yml` & `nemos-0.1.1/.github/workflows/connect.yml`

 * *Files identical despite different names*

### Comparing `nemos-0.1.0/.github/workflows/deploy-pure-python.yml` & `nemos-0.1.1/.github/workflows/deploy-pure-python.yml`

 * *Files identical despite different names*

### Comparing `nemos-0.1.0/.gitignore` & `nemos-0.1.1/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -139,7 +139,10 @@
 .DS_Store
 
 # mkdocs generated folder
 docs/generated/
 
 # vscode
 .vscode/
+
+# nwb cahce
+nwb-cache/
```

### Comparing `nemos-0.1.0/CCN-letterFoot.png` & `nemos-0.1.1/CCN-letterFoot.png`

 * *Files identical despite different names*

### Comparing `nemos-0.1.0/CCN-logo-wText.png` & `nemos-0.1.1/docs/CCN-logo-wText.png`

 * *Files identical despite different names*

### Comparing `nemos-0.1.0/CODE_OF_CONDUCT.md` & `nemos-0.1.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `nemos-0.1.0/CONTRIBUTING.md` & `nemos-0.1.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `nemos-0.1.0/LICENSE` & `nemos-0.1.1/LICENSE`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 William F. Broderick
+Copyright (c) 2023 nemos authors
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `nemos-0.1.0/docs/developers_notes/README.md` & `nemos-0.1.1/docs/developers_notes/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Introduction
 
+!!! warning
+    This note is out-of-sync with the current API. Please, do not rely on this yet for contributing to `nemos`.
+
 Welcome to the Developer Notes of the `nemos` project. These notes aim to provide detailed technical information about the various modules, classes, and functions that make up this library, as well as guidelines on how to write code that integrates nicely with our package. They are intended to help current and future developers understand the design decisions, structure, and functioning of the library, and to provide guidance on how to modify, extend, and maintain the codebase.
 
+
 ## Intended Audience
 
 These notes are primarily intended for the following groups:
 
 - **Current Developers**: The Developer Notes can serve as a comprehensive guide to understanding the library, making it easier to debug, modify and maintain the code.
 
 - **Future Developers**: These notes can help onboard new developers to the project, providing them with detailed explanations of the codebase and its underlying architecture.
```

### Comparing `nemos-0.1.0/docs/developers_notes/basis_module.md` & `nemos-0.1.1/docs/developers_notes/01-basis_module.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# The Basis Module
+# The `basis` Module
 
 ## Introduction
 
 The `nemos.basis` module provides objects that allow users to construct and evaluate basis functions of various types. The classes are hierarchically organized as follows:
 
 ```
 Abstract Class Basis
@@ -15,17 +15,15 @@
 │   │
 │   ├─ Concrete Subclass MSplineBasis
 │   │
 │   ├─ Concrete Subclass BSplineBasis
 │   │
 │   └─ Concrete Subclass CyclicBSplineBasis
 │
-├─ Abstract Subclass RaisedCosineBasis
-│   │
-│   ├─ Concrete Subclass RaisedCosineBasisLinear
+├─ Concrete Subclass RaisedCosineBasisLinear 
 │   │
 │   └─ Concrete Subclass RaisedCosineBasisLog
 │
 └─ Concrete Subclass OrthExponentialBasis
 ```
 
 The super-class `Basis` provides two public methods, [`evaluate`](#the-public-method-evaluate) and [`evaluate_on_grid`](#the-public-method-evaluate_on_grid). These methods perform checks on both the input provided by the user and the output of the evaluation to ensure correctness, and are thus considered "safe". They both make use of the private abstract method `_evaluate` that is specific for each concrete class. See below for more details.
```

### Comparing `nemos-0.1.0/docs/examples/plot_ND_basis_function.py` & `nemos-0.1.1/docs/background/plot_02_ND_basis_function.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,16 +59,17 @@
 # One way to model the response to our 2D stimuli is to hypothesize that it decomposes into two factors:
 # one due to the x-coordinate and another due to the y-coordinate. We can express this relationship as:
 # $$
 # f(x,y) \\approx \sum_i \alpha_i \cdot a_i(x) + \sum_j \beta_j \cdot b_j(y).
 # $$
 # Here, we simply add two basis objects, `a_basis` and `b_basis`, together to define the additive basis.
 
-import numpy as np
 import matplotlib.pyplot as plt
+import numpy as np
+
 import nemos as nmo
 
 # Define 1D basis objects
 a_basis = nmo.basis.MSplineBasis(n_basis_funcs=15, order=3)
 b_basis = nmo.basis.RaisedCosineBasisLog(n_basis_funcs=14)
 
 # Define the 2D additive basis object
@@ -82,15 +83,15 @@
 T = 1000
 
 # Define two variables
 x_coord = np.linspace(0, 1, 1000)
 y_coord = np.linspace(0, 1, 1000)
 
 # Evaluate the basis functions for the given trajectory.
-eval_basis = additive_basis.evaluate(x_coord, y_coord)
+eval_basis = additive_basis(x_coord, y_coord)
 
 print(f"Sum of two 1D splines with {eval_basis.shape[1]} "
       f"basis element and {eval_basis.shape[0]} samples:\n"
       f"\t- a_basis had {a_basis.n_basis_funcs} elements\n\t- b_basis had {b_basis.n_basis_funcs} elements.")
 
 # %%
 # #### Plotting 2D Additive Basis Elements
@@ -98,21 +99,21 @@
 
 basis_a_element = 5
 basis_b_element = 1
 # Plot the 1D basis elements
 fig, axs = plt.subplots(1, 2, figsize=(6, 3))
 
 axs[0].set_title(f"$a_{{{basis_a_element}}}(x)$", color="b")
-axs[0].plot(x_coord, a_basis.evaluate(x_coord), "grey", alpha=.3)
-axs[0].plot(x_coord, a_basis.evaluate(x_coord)[:, basis_a_element], "b")
+axs[0].plot(x_coord, a_basis(x_coord), "grey", alpha=.3)
+axs[0].plot(x_coord, a_basis(x_coord)[:, basis_a_element], "b")
 axs[0].set_xlabel("x-coord")
 
 axs[1].set_title(f"$b_{{{basis_b_element}}}(x)$", color="b")
-axs[1].plot(y_coord, b_basis.evaluate(x_coord), "grey", alpha=.3)
-axs[1].plot(y_coord, b_basis.evaluate(x_coord)[:, basis_b_element], "b")
+axs[1].plot(y_coord, b_basis(x_coord), "grey", alpha=.3)
+axs[1].plot(y_coord, b_basis(x_coord)[:, basis_b_element], "b")
 axs[1].set_xlabel("y-coord")
 plt.tight_layout()
 
 # %%
 # We can visualize how these elements are extended in 2D by evaluating the additive basis
 # on a grid of points that spans its domain and plotting the result.
 # We use the `evaluate_on_grid` method for this.
@@ -160,15 +161,15 @@
 prod_basis = a_basis * b_basis
 
 # %%
 # Again evaluating the basis will require 2 inputs.
 # The number of elements of the product basis will be the product of the elements of the two 1D bases.
 
 # Evaluate the product basis at the x and y coordinates
-eval_basis = prod_basis.evaluate(x_coord, y_coord)
+eval_basis = prod_basis(x_coord, y_coord)
 
 # Output the number of elements and samples of the evaluated basis, 
 # as well as the number of elements in the original 1D basis objects
 print(f"Product of two 1D splines with {eval_basis.shape[1]} "
       f"basis element and {eval_basis.shape[0]} samples:\n"
       f"\t- a_basis had {a_basis.n_basis_funcs} elements\n\t- b_basis had {b_basis.n_basis_funcs} elements.")
 
@@ -186,21 +187,21 @@
 element_pairs = [[0, 0], [5, 1], [10, 5]]
 
 # plot the 1D basis element and their product
 fig, axs = plt.subplots(3,3,figsize=(8, 6))
 cc = 0
 for i, j in element_pairs:
     # plot the element form a_basis
-    axs[cc, 0].plot(x_coord, a_basis.evaluate(x_coord), "grey", alpha=.3)
-    axs[cc, 0].plot(x_coord, a_basis.evaluate(x_coord)[:, i], "b")
+    axs[cc, 0].plot(x_coord, a_basis(x_coord), "grey", alpha=.3)
+    axs[cc, 0].plot(x_coord, a_basis(x_coord)[:, i], "b")
     axs[cc, 0].set_title(f"$a_{{{i}}}(x)$",color='b')
 
     # plot the element form b_basis
-    axs[cc, 1].plot(y_coord, b_basis.evaluate(y_coord), "grey", alpha=.3)
-    axs[cc, 1].plot(y_coord, b_basis.evaluate(y_coord)[:, j], "b")
+    axs[cc, 1].plot(y_coord, b_basis(y_coord), "grey", alpha=.3)
+    axs[cc, 1].plot(y_coord, b_basis(y_coord)[:, j], "b")
     axs[cc, 1].set_title(f"$b_{{{j}}}(y)$",color='b')
 
     # select & plot the corresponding product basis element
     k = i * b_basis.n_basis_funcs + j
     axs[cc, 2].contourf(X, Y, Z[:, :, k], cmap='Blues')
     axs[cc, 2].set_title(f"$A_{{{k}}}(x,y) = a_{{{i}}}(x) \cdot b_{{{j}}}(y)$", color='b')
     axs[cc, 2].set_xlabel('x-coord')
@@ -240,15 +241,15 @@
 
 a_basis = nmo.basis.RaisedCosineBasisLinear(n_basis_funcs=n_basis)
 b_basis = nmo.basis.RaisedCosineBasisLinear(n_basis_funcs=n_basis)
 c_basis = nmo.basis.RaisedCosineBasisLinear(n_basis_funcs=n_basis)
 
 prod_basis_3 = a_basis * b_basis * c_basis
 samples = np.linspace(0, 1, T)
-eval_basis = prod_basis_3.evaluate(samples, samples, samples)
+eval_basis = prod_basis_3(samples, samples, samples)
 
 print(f"Product of three 1D splines results in {prod_basis_3.n_basis_funcs} "
       f"basis elements.\nEvaluation output of shape {eval_basis.shape}")
 
 # %%
 # The evaluation of the product of 3 basis is a 4 dimensional tensor; we can visualize slices of it.
```

### Comparing `nemos-0.1.0/docs/gen_ref_pages.py` & `nemos-0.1.1/docs/gen_ref_pages.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 See [CCN template repo](https://ccn-template.readthedocs.io/en/latest/notes/03-documentation/) for why.
 """
 
 from pathlib import Path
 
 import mkdocs_gen_files
+
 nav = mkdocs_gen_files.Nav()
 
 for path in sorted(Path("src").rglob("*.py")):
     module_path = path.relative_to("src").with_suffix("")
     doc_path = path.relative_to("src").with_suffix(".md")
     full_doc_path = Path("reference", doc_path)
```

### Comparing `nemos-0.1.0/pyproject.toml` & `nemos-0.1.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,16 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nemos"
-version = "0.1.0"
-authors = [
-    {name = "Edoardo Balzani", email = "ebalzani@flatironinstitute.org"},
-    {name = "William Broderick", email = "wbroderick@flatironinstitute.org"},
-    {name = "Guillaume Vejo", email = "gviejo@flatironinstitute.org"},
-    {name = "Alex Williams", email = "alex.h.williams@nyu.edu"}
-]
-description = "Toolbox for basic Generalized Linear Models (GLMs) for neural data analysis"
+version = "0.1.1"
+authors = [{name = "nemos authors"}]
+description = "NEural MOdelS, a statistical modeling framework for neuroscience."
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["neuroscience", "Poisson-GLM"]
 license = { file = "LICENSE" }
 classifiers = [
     "Intended Audience :: Science/Research",
     "Natural Language :: English",
@@ -23,50 +18,56 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10"
 ]
 
 # Define dependencies for the project
 dependencies = [
-    'jax>=0.4',                     # Numerical computing library
-    'jaxopt>=0.6',                  # Optimization library built on JAX
-    'matplotlib>=3.7',              # Plotting library
-    'numpy>1.20',                   # Numerical computing library
-    'scikit-learn>=1.2',            # Machine learning library
-    'scipy>=1.10',                  # Scientific computing library
-    'typing_extensions>=4.6'        # Typing extensions for Python
+    "jax>=0.4",                     # Numerical computing library
+    "jaxopt>=0.6",                  # Optimization library built on JAX
+    "numpy>1.20",                   # Numerical computing library
+    "scipy>=1.10",                  # Scientific computing library
+    "typing_extensions>=4.6",       # Typing extensions for Python
+    "pynapple"
 ]
 
 
 
 # Configure package discovery for setuptools
 [tool.setuptools.packages.find]
-where = ["src"]             # The directory where package modules are located
+where = ["src"]     # The directory where package modules are located
 include = ["nemos"] # The specific package(s) to include in the distribution
 
 
 # Define optional dependencies for the project
 [project.optional-dependencies]
 dev = [
     "black",                        # Code formatter
     "isort",                        # Import sorter
     "pip-tools",                    # Dependency management
     "pytest",                       # Testing framework
     "flake8",                       # Code linter
     "coverage",                     # Test coverage measurement
     "pytest-cov",                   # Test coverage plugin for pytest
+    "statsmodels",                  # Used to compare model pseudo-r2 in testing
+    "scikit-learn",                 # Testing compatibility with CV & pipelines
 ]
 docs = [
     "mkdocs",                       # Documentation generator
     "mkdocstrings[python]",         # Python-specific plugin for mkdocs
     "mkdocs-section-index",         # Plugin for generating a section index in mkdocs
     "mkdocs-gen-files",             # Plugin for generating additional files in mkdocs
-    "mkdocs-literate-nav",          # Plugin for literate-style navigation in mkdocs
+    "mkdocs-literate-nav>=0.6.1",   # Plugin for literate-style navigation in mkdocs
     "mkdocs-gallery",               # Plugin for adding image galleries to mkdocs
-    "mkdocs-material"
+    "mkdocs-material",              # Material theme for mkdocs
+    "mkdocs-autorefs>=0.5",
+    "scikit-learn",
+    "dandi",
+    "ipython",
+    "matplotlib>=3.7"
 ]
 
 
 [tool.black]
 target-version = ['py38', 'py39', 'py310']
 skip-string-normalization = false
 exclude = '''
@@ -92,15 +93,14 @@
 [tool.isort]
 multi_line_output = 3             # Use three-line style for multi-line imports
 include_trailing_comma = true     # Include trailing comma in multi-line imports
 profile = "black"
 
 # Configure pytest
 [tool.pytest.ini_options]
-addopts = "--cov=nemos"   # Additional options to pass to pytest, enabling coverage for the 'nemos' package
 testpaths = ["tests"]             # Specify the directory where test files are located
 
 [tool.coverage.report]
 exclude_lines = [
     "@abc.abstractmethod",
     "if __name__ == .__main__.:"
-]
+]
```

### Comparing `nemos-0.1.0/src/nemos/basis.py` & `nemos-0.1.1/src/nemos/basis.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 """Bases classes."""
 
 # required to get ArrayLike to render correctly, unnecessary as of python 3.10
 from __future__ import annotations
 
 import abc
-from typing import Generator, Tuple
+import warnings
+from typing import Callable, Generator, Literal, Optional, Tuple, Union
 
-import jax.numpy
 import numpy as np
 import scipy.linalg
 from numpy.typing import ArrayLike, NDArray
+from pynapple import Tsd, TsdFrame
 from scipy.interpolate import splev
 
+from .convolve import create_convolutional_predictor
+from .type_casting import support_pynapple
 from .utils import row_wise_kron
 
+FeatureMatrix = Union[NDArray, TsdFrame]
+
 __all__ = [
     "MSplineBasis",
     "BSplineBasis",
     "CyclicBSplineBasis",
     "RaisedCosineBasisLinear",
     "RaisedCosineBasisLog",
     "OrthExponentialBasis",
@@ -26,49 +31,371 @@
 ]
 
 
 def __dir__() -> list[str]:
     return __all__
 
 
-class Basis(abc.ABC):
+def check_transform_input(func: Callable) -> Callable:
+    """Check input before calling basis.
+
+    This decorator allows to raise an exception that is more readable
+    when the wrong number of input is provided to __call__.
     """
-    Abstract class for basis functions.
+
+    def wrapper(self: Basis, *xi: ArrayLike, **kwargs) -> NDArray:
+        xi = self._check_transform_input(*xi)
+        return func(self, *xi, **kwargs)  # Call the basis
+
+    return wrapper
+
+
+def check_one_dimensional(func: Callable) -> Callable:
+    def wrapper(self: Basis, *xi: ArrayLike, **kwargs):
+        if any(x.ndim != 1 for x in xi):
+            raise ValueError("Input sample must be one dimensional!")
+        return func(self, *xi, **kwargs)
+
+    return wrapper
+
+
+def min_max_rescale_samples(sample_pts: NDArray) -> NDArray:
+    """Rescale samples to [0,1]."""
+    if np.any(sample_pts < 0) or np.any(sample_pts > 1):
+        sample_pts -= np.min(sample_pts)
+        sample_pts /= np.max(sample_pts)
+        warnings.warn(
+            "Rescaling sample points for RaisedCosine basis to [0,1]!", UserWarning
+        )
+    return sample_pts
+
+
+class TransformerBasis:
+    """Basis as `scikit-learn` transformers.
+
+    This class abstracts the underlying basis function details, offering methods
+    similar to scikit-learn's transformers but specifically designed for basis
+    transformations. It supports fitting to data (calculating any necessary parameters
+    of the basis functions), transforming data (applying the basis functions to
+    data), and both fitting and transforming in one step.
 
     Parameters
     ----------
-    n_basis_funcs :
-        Number of basis functions.
+    basis :
+        A concrete subclass of `Basis`.
+    """
 
-    Attributes
+    def __init__(self, basis: Basis):
+        self._basis = basis
+
+    @staticmethod
+    def _unpack_inputs(X: FeatureMatrix):
+        """Unpack impute without using transpose.
+
+        Unpack horizontally stacked inputs using slicing. This works gracefully with `pynapple`,
+        returning a list of Tsd objects. Attempt to unpack using *X.T will raise a `pynapple`
+        exception since `pynapple` assumes that the time axis is the first axis.
+
+        Parameters
+        ----------
+        X:
+            The inputs horizontally stacked.
+
+        Returns
+        -------
+        :
+            A tuple of each individual input.
+
+        """
+        return (X[:, k] for k in range(X.shape[1]))
+
+    def fit(self, X: FeatureMatrix, y=None):
+        """
+        Compute the convolutional kernels.
+
+        If any of the 1D basis in self._basis is in "conv" mode, it computes the convolutional kernels.
+
+        Parameters
+        ----------
+        X :
+           The data to fit the basis functions to, shape (num_samples, num_input).
+        y : ignored
+           Not used, present for API consistency by convention.
+
+        Returns
+        -------
+        self :
+            The transformer object.
+        """
+        self._basis._set_kernel(*self._unpack_inputs(X))
+        return self
+
+    def transform(self, X: FeatureMatrix, y=None) -> FeatureMatrix:
+        """
+        Transform the data using the fitted basis functions.
+
+        Parameters
+        ----------
+        X :
+            The data to transform using the basis functions, shape (num_samples, num_input).
+        y :
+            Not used, present for API consistency by convention.
+
+        Returns
+        -------
+        :
+            The data transformed by the basis functions.
+        """
+        # transpose does not work with pynapple
+        # can't use func(*X.T) to unwrap
+
+        return self._basis._compute_features(*self._unpack_inputs(X))
+
+    def fit_transform(self, X: FeatureMatrix, y=None) -> FeatureMatrix:
+        """
+        Compute the kernels and the features.
+
+        This method is a convenience that combines fit and transform into
+        one step.
+
+        Parameters
+        ----------
+        X :
+            The data to fit the basis functions to and then transform.
+        y :
+            Not used, present for API consistency by convention.
+
+        Returns
+        -------
+        array-like
+            The data transformed by the basis functions, after fitting the basis
+            functions to the data.
+        """
+        return self._basis.compute_features(*self._unpack_inputs(X))
+
+
+class Basis(abc.ABC):
+    """
+    Abstract base class for defining basis functions for feature transformation.
+
+    Basis functions are mathematical constructs that can represent data in alternative,
+    often more compact or interpretable forms. This class provides a template for such
+    transformations, with specific implementations defining the actual behavior.
+
+    Parameters
     ----------
-    n_basis_funcs : int
-        Number of basis functions.
+    n_basis_funcs :
+        The number of basis functions.
+    mode :
+        The mode of operation. 'eval' for evaluation at sample points,
+        'conv' for convolutional operation.
+    window_size :
+        The window size for convolution. Required if mode is 'conv'.
+    *args:
+        Only used in "conv" mode. Additional positional arguments that are passed to
+        `nemos.convolve.create_convolutional_predictor`
+    **kwargs:
+        Only used in "conv" mode. Additional keyword arguments that are passed to
+        `nemos.convolve.create_convolutional_predictor`
 
     """
 
-    def __init__(self, n_basis_funcs: int) -> None:
+    def __init__(
+        self,
+        n_basis_funcs: int,
+        *args,
+        mode: Literal["eval", "conv"] = "eval",
+        window_size: Optional[int] = None,
+        **kwargs,
+    ) -> None:
         self.n_basis_funcs = n_basis_funcs
         self._n_input_dimensionality = 0
         self._check_n_basis_min()
+        self._conv_args = args
+        self._conv_kwargs = kwargs
+        # check mode
+        if mode not in ["conv", "eval"]:
+            raise ValueError(
+                f"`mode` should be either 'conv' or 'eval'. '{mode}' provided instead!"
+            )
+        if mode == "conv":
+            if window_size is None:
+                raise ValueError(
+                    "If the basis is in `conv` mode, you must provide a window_size!"
+                )
+            elif not (isinstance(window_size, int) and window_size > 0):
+                raise ValueError(
+                    f"`window_size` must be a positive integer. {window_size} provided instead!"
+                )
+
+        self._window_size = window_size
+        self._mode = mode
+        self._kernel = None
+
+    @property
+    def mode(self):
+        return self._mode
+
+    @property
+    def window_size(self):
+        return self._window_size
+
+    @check_transform_input
+    def _compute_features(self, *xi: ArrayLike) -> FeatureMatrix:
+        r"""
+        Apply the basis transformation to the input data.
+
+        This method operates in two modes:
+        - 'eval': Evaluates the basis functions at the given sample points.
+        - 'conv': Applies a convolution operation between the input data and the basis functions,
+          using a window size defined at initialization.
+
+        Parameters
+        ----------
+        *xi:
+            The input samples over which to apply the basis transformation. The samples can be passed
+            as multiple arguments, each representing a different dimension for multivariate inputs.
+
+        Returns
+        -------
+        :
+            A matrix with the transformed features. The shape of the output depends on the operation mode:
+                - If `mode == 'eval'`, the basis evaluated at the samples, or $b_i(*xi)$, where $b_i$ is a
+                basis element. xi[k] must be a one-dimensional array or a pynapple Tsd.
+
+                - If `mode == 'conv'`, a bank of basis filters (created by calling fit) is convolved with the
+                samples. Samples can be a NDArray, or a pynapple Tsd/TsdFrame/TsdTensor. All the dimensions
+                except for the sample-axis are flattened, so that the method always returns a matrix.
+                For example, if samples are of shape (num_samples, 2, 3), the output will be
+                (num_samples, num_basis_funcs * 2 * 3).
+                The time-axis can be specified at basis initialization by setting the keyword argument `axis`.
+                For example, if `axis == 1` your samples should be (N1, num_samples N3, ...), the output of
+                transform will be (num_samples, num_basis_funcs * N1 * N3 *...).
+
+        Raises
+        ------
+        ValueError:
+            If an invalid mode is specified or necessary parameters for the chosen mode are missing.
+        """
+        # check if self._kernel is not None for mode="conv"
+        self._check_has_kernel()
+        if self.mode == "eval":  # evaluate at the sample
+            return self.__call__(*xi)
+        else:  # convolve, called only at the last layer
+            if "axis" not in self._conv_kwargs:
+                axis = 0
+            else:
+                axis = self._conv_kwargs["axis"]
+            # convolve called at the end of any recursive call
+            # this ensures that len(xi) == 1.
+            conv = create_convolutional_predictor(
+                self._kernel, *xi, *self._conv_args, **self._conv_kwargs
+            )
+            # move the time axis to the first dimension
+            new_axis = (np.arange(conv.ndim) + axis) % conv.ndim
+            conv = np.transpose(conv, new_axis)
+            # make sure to return a matrix
+            return np.reshape(conv, newshape=(conv.shape[0], -1))
+
+    def compute_features(self, *xi: ArrayLike) -> FeatureMatrix:
+        """
+        Compute the basis functions and transform input data into model features.
+
+        This method is designed to be a high-level interface for transforming input
+        data using the basis functions defined by the subclass. Depending on the basis'
+        mode ('eval' or 'conv'), it either evaluates the basis functions at the sample
+        points or performs a convolution operation between the input data and the
+        basis functions.
+
+        Parameters
+        ----------
+        *xi :
+            Input data arrays to be transformed. The shape and content requirements
+            depend on the subclass and mode of operation ('eval' or 'conv').
+
+        Returns
+        -------
+        :
+            Transformed features. In 'eval' mode, it corresponds to the basis functions
+            evaluated at the input samples. In 'conv' mode, it consists of convolved
+            input samples with the basis functions. The output shape varies based on
+            the subclass and mode.
+
+        Notes
+        -----
+        Subclasses should implement how to handle the transformation specific to their
+        basis function types and operation modes.
+        """
+        if self._kernel is None:
+            self._set_kernel(*xi)
+        return self._compute_features(*xi)
+
+    def _set_kernel(self, *xi: ArrayLike) -> Basis:
+        """
+        Prepare or compute the convolutional kernel for the basis functions.
+
+        This method is called to prepare the basis functions for convolution operations
+        in subclasses where the 'conv' mode is used. It typically involves computing a
+        kernel based on the basis functions that will be used for convolution with the
+        input data. The specifics of kernel computation depend on the subclass implementation
+        and the nature of the basis functions.
+
+        In 'eval' mode, this method might not perform any operation but simply return the
+        instance itself, as no kernel preparation is necessary.
+
+        Parameters
+        ----------
+        *xi :
+            The input data based on which the kernel might be computed. The actual use of
+            these inputs is subclass-specific and might not be applicable for all basis types.
+
+        Returns
+        -------
+        self :
+            The instance itself, modified to include the computed kernel if applicable. This
+            allows for method chaining and integration into transformation pipelines.
+
+        Notes
+        -----
+        Subclasses implementing this method should detail the specifics of how the kernel is
+        computed and how the input parameters are utilized. If the basis operates in 'eval'
+        mode exclusively, this method should simply return `self` without modification.
+        """
+        if self.mode == "conv":
+            self._kernel = self.__call__(np.linspace(0, 1, self.window_size))
+        return self
 
     @abc.abstractmethod
-    def _evaluate(self, *xi: NDArray) -> NDArray:
+    def __call__(self, *xi: ArrayLike) -> FeatureMatrix:
         """
-        Evaluate the basis set at the given samples x1,...,xn using the subclass-specific "_evaluate" method.
+        Abstract method to evaluate the basis functions at given points.
+
+        This method must be implemented by subclasses to define the specific behavior
+        of the basis transformation. The implementation depends on the type of basis
+        (e.g., spline, raised cosine), and it should evaluate the basis functions at
+        the specified points in the domain.
 
         Parameters
         ----------
-        *xi: (number of samples, )
-            The input samples xi[0],...,xi[n] .
+        *xi :
+            Variable number of arguments, each representing an array of points at which
+            to evaluate the basis functions. The dimensions and requirements of these
+            inputs vary depending on the specific basis implementation.
+
+        Returns
+        -------
+        :
+            An array containing the evaluated values of the basis functions at the input
+            points. The shape and structure of this array are specific to the subclass
+            implementation.
         """
         pass
 
     @staticmethod
-    def _get_samples(*n_samples: int) -> Generator[NDArray, ...]:
+    def _get_samples(*n_samples: int) -> Generator[NDArray]:
         """Get equi-spaced samples for all the input dimensions.
 
         This will be used to evaluate the basis on a grid of
         points derived by the samples.
 
         Parameters
         ----------
@@ -78,67 +405,71 @@
         Returns
         -------
         :
             A generator yielding numpy arrays of linspaces from 0 to 1 of sizes specified by `n_samples`.
         """
         return (np.linspace(0, 1, n_samples[k]) for k in range(len(n_samples)))
 
-    def evaluate(self, *xi: ArrayLike) -> NDArray:
-        """
-        Evaluate the basis set at the given samples x[0],...,x[n] using the subclass-specific "_evaluate" method.
+    @support_pynapple(conv_type="numpy")
+    def _check_transform_input(
+        self, *xi: ArrayLike
+    ) -> Tuple[Union[NDArray, Tsd, TsdFrame]]:
+        """Check transform input.
 
         Parameters
         ----------
         xi[0],...,xi[n] :
             The input samples, each  with shape (number of samples, ).
 
-        Returns
-        -------
-        :
-            The generated basis functions.
-
         Raises
         ------
         ValueError
             - If the time point number is inconsistent between inputs.
             - If the number of inputs doesn't match what the Basis object requires.
             - At least one of the samples is empty.
-        """
-        # check that the input is array-like
-        if any(
-            not isinstance(x, (list, tuple, np.ndarray, jax.numpy.ndarray)) for x in xi
-        ):
-            raise TypeError("Input samples must be array-like!")
 
-        # convert to numpy.array of floats
-        xi = tuple(np.asarray(x, dtype=float) for x in xi)
+        """
+        # check that the input is array-like (i.e., whether we can cast it to
+        # numeric arrays)
+        try:
+            # make sure array is at least 1d (so that we succeed when only
+            # passed a scalar)
+            xi = tuple(np.atleast_1d(np.asarray(x, dtype=float)) for x in xi)
+        except TypeError:
+            raise TypeError("Input samples must be array-like of floats!")
 
         # check for non-empty samples
         if self._has_zero_samples(tuple(len(x) for x in xi)):
             raise ValueError("All sample provided must be non empty.")
 
         # checks on input and outputs
         self._check_samples_consistency(*xi)
         self._check_input_dimensionality(xi)
 
-        eval_basis = self._evaluate(*xi)
+        return xi
 
-        return eval_basis
+    def _check_has_kernel(self) -> None:
+        """Check that the kernel is pre-computed."""
+        if self.mode == "conv" and self._kernel is None:
+            raise ValueError(
+                "You must call `_set_kernel` before `_compute_features` when mode =`conv`."
+            )
 
     def evaluate_on_grid(self, *n_samples: int) -> Tuple[Tuple[NDArray], NDArray]:
         """Evaluate the basis set on a grid of equi-spaced sample points.
 
         The i-th axis of the grid will be sampled with n_samples[i] equi-spaced points.
         The method uses numpy.meshgrid with `indexing="ij"`, returning matrix indexing
         instead of the default cartesian indexing, see Notes.
 
         Parameters
         ----------
         n_samples[0],...,n_samples[n]
-            The number of samples in each axis of the grid.
+            The number of samples in each axis of the grid. The length of
+            n_samples must equal the number of combined bases.
 
         Returns
         -------
         *Xs :
             A tuple of arrays containing the meshgrid values, one element for each of the n dimension of the grid,
             where n equals to the number of inputs.
             The size of Xs[i] is (n_samples[0], ... , n_samples[n]).
@@ -166,23 +497,23 @@
         if self._has_zero_samples(n_samples):
             raise ValueError("All sample counts provided must be greater than zero.")
 
         # get the samples
         sample_tuple = self._get_samples(*n_samples)
         Xs = np.meshgrid(*sample_tuple, indexing="ij")
 
-        # call evaluate to evaluate the basis on a flat NDArray and reshape to match meshgrid output
-        Y = self.evaluate(*tuple(grid_axis.flatten() for grid_axis in Xs)).reshape(
+        # evaluates the basis on a flat NDArray and reshape to match meshgrid output
+        Y = self.__call__(*tuple(grid_axis.flatten() for grid_axis in Xs)).reshape(
             (*n_samples, self.n_basis_funcs)
         )
 
         return *Xs, Y
 
     @staticmethod
-    def _has_zero_samples(n_samples: Tuple[int]) -> bool:
+    def _has_zero_samples(n_samples: Tuple[int, ...]) -> bool:
         return any([n <= 0 for n in n_samples])
 
     def _check_input_dimensionality(self, xi: Tuple) -> None:
         """
         Check that the number of inputs provided by the user matches the number of inputs required.
 
         Parameters
@@ -192,15 +523,15 @@
 
         Raises
         ------
         ValueError
             If the number of inputs doesn't match what the Basis object requires.
         """
         if len(xi) != self._n_input_dimensionality:
-            raise ValueError(
+            raise TypeError(
                 f"Input dimensionality mismatch. This basis evaluation requires {self._n_input_dimensionality} inputs, "
                 f"{len(xi)} inputs provided instead."
             )
 
     @staticmethod
     def _check_samples_consistency(*xi: NDArray) -> None:
         """
@@ -318,48 +649,103 @@
     ----------
     n_basis_funcs : int
         Number of basis functions.
 
 
     """
 
-    def __init__(self, basis1: Basis, basis2: Basis) -> None:
+    def __init__(self, basis1: Basis, basis2: Basis, *args, **kwargs) -> None:
         self.n_basis_funcs = basis1.n_basis_funcs + basis2.n_basis_funcs
-        super().__init__(self.n_basis_funcs)
+        super().__init__(self.n_basis_funcs, *args, mode="eval", **kwargs)
         self._n_input_dimensionality = (
             basis1._n_input_dimensionality + basis2._n_input_dimensionality
         )
         self._basis1 = basis1
         self._basis2 = basis2
         return
 
     def _check_n_basis_min(self) -> None:
         pass
 
-    def _evaluate(self, *xi: NDArray) -> NDArray:
+    @support_pynapple(conv_type="numpy")
+    @check_transform_input
+    @check_one_dimensional
+    def __call__(self, *xi: ArrayLike) -> FeatureMatrix:
         """
         Evaluate the basis at the input samples.
 
         Parameters
         ----------
-        xi[0], ..., xi[n] : (number of samples, )
-            Tuple of input samples.
+        xi[0], ..., xi[n] : (n_samples,)
+            Tuple of input samples, each with the same number of samples. The
+            number of input arrays must equal the number of combined bases.
 
         Returns
         -------
         :
             The basis function evaluated at the samples, shape (n_samples, n_basis_funcs)
+
         """
         return np.hstack(
             (
-                self._basis1._evaluate(*xi[: self._basis1._n_input_dimensionality]),
-                self._basis2._evaluate(*xi[self._basis1._n_input_dimensionality :]),
+                self._basis1.__call__(*xi[: self._basis1._n_input_dimensionality]),
+                self._basis2.__call__(*xi[self._basis1._n_input_dimensionality :]),
             )
         )
 
+    @check_transform_input
+    def _compute_features(self, *xi: ArrayLike) -> FeatureMatrix:
+        """
+        Compute features for added bases and concatenate.
+
+        Parameters
+        ----------
+        xi[0], ..., xi[n] : (n_samples,)
+            Tuple of input samples, each with the same number of samples. The
+            number of input arrays must equal the number of combined bases.
+
+        Returns
+        -------
+        :
+            The features, shape (n_samples, n_basis_funcs)
+
+        """
+        # the numpy conversion is important, there is some in-place
+        # array modification in basis.
+        hstack_pynapple = support_pynapple(conv_type="numpy")(np.hstack)
+        return hstack_pynapple(
+            (
+                self._basis1._compute_features(
+                    *xi[: self._basis1._n_input_dimensionality]
+                ),
+                self._basis2._compute_features(
+                    *xi[self._basis1._n_input_dimensionality :]
+                ),
+            ),
+        )
+
+    def _set_kernel(self, *xi: ArrayLike) -> Basis:
+        """Call fit on the added basis.
+
+        If any of the added basis is in "conv" mode, it will prepare its kernels for the convolution.
+
+        Parameters
+        ----------
+        *xi:
+            The sample inputs. Unused, necessary to conform to `scikit-learn` API.
+
+        Returns
+        -------
+        :
+            The AdditiveBasis ready to be evaluated.
+        """
+        self._basis1._set_kernel(*xi)
+        self._basis2._set_kernel(*xi)
+        return self
+
 
 class MultiplicativeBasis(Basis):
     """
     Class representing the multiplication (external product) of two Basis objects.
 
     Parameters
     ----------
@@ -371,49 +757,96 @@
     Attributes
     ----------
     n_basis_funcs : int
         Number of basis functions.
 
     """
 
-    def __init__(self, basis1: Basis, basis2: Basis) -> None:
+    def __init__(self, basis1: Basis, basis2: Basis, *args, **kwargs) -> None:
         self.n_basis_funcs = basis1.n_basis_funcs * basis2.n_basis_funcs
-        super().__init__(self.n_basis_funcs)
+        super().__init__(self.n_basis_funcs, *args, mode="eval", **kwargs)
         self._n_input_dimensionality = (
             basis1._n_input_dimensionality + basis2._n_input_dimensionality
         )
         self._basis1 = basis1
         self._basis2 = basis2
         return
 
     def _check_n_basis_min(self) -> None:
         pass
 
-    def _evaluate(self, *xi: NDArray) -> NDArray:
+    def _set_kernel(self, *xi: NDArray) -> Basis:
+        """Call fit on the multiplied basis.
+
+        If any of the added basis is in "conv" mode, it will prepare its kernels for the convolution.
+
+        Parameters
+        ----------
+        *xi:
+            The sample inputs. Unused, necessary to conform to `scikit-learn` API.
+
+        Returns
+        -------
+        :
+            The MultiplicativeBasis ready to be evaluated.
+        """
+        self._basis1._set_kernel(*xi)
+        self._basis2._set_kernel(*xi)
+        return self
+
+    @support_pynapple(conv_type="numpy")
+    @check_transform_input
+    @check_one_dimensional
+    def __call__(self, *xi: ArrayLike) -> FeatureMatrix:
         """
         Evaluate the basis at the input samples.
 
         Parameters
         ----------
-        xi[0], ..., xi[n] : (number of samples, )
-            Tuple of input samples.
+        xi[0], ..., xi[n] : (n_samples,)
+            Tuple of input samples, each with the same number of samples. The
+            number of input arrays must equal the number of combined bases.
 
         Returns
         -------
         :
             The basis function evaluated at the samples, shape (n_samples, n_basis_funcs)
         """
-        return np.array(
+        return np.asarray(
             row_wise_kron(
-                self._basis1._evaluate(*xi[: self._basis1._n_input_dimensionality]),
-                self._basis2._evaluate(*xi[self._basis1._n_input_dimensionality :]),
+                self._basis1.__call__(*xi[: self._basis1._n_input_dimensionality]),
+                self._basis2.__call__(*xi[self._basis1._n_input_dimensionality :]),
                 transpose=False,
             )
         )
 
+    @check_transform_input
+    def _compute_features(self, *xi: ArrayLike) -> FeatureMatrix:
+        """
+        Compute the features for the multiplied bases, and compute their outer product.
+
+        Parameters
+        ----------
+        xi[0], ..., xi[n] : (n_samples,)
+            Tuple of input samples, each with the same number of samples. The
+            number of input arrays must equal the number of combined bases.
+
+        Returns
+        -------
+        :
+            The  features, shape (n_samples, n_basis_funcs)
+
+        """
+        kron = support_pynapple(conv_type="numpy")(row_wise_kron)
+        return kron(
+            self._basis1._compute_features(*xi[: self._basis1._n_input_dimensionality]),
+            self._basis2._compute_features(*xi[self._basis1._n_input_dimensionality :]),
+            transpose=False,
+        )
+
 
 class SplineBasis(Basis, abc.ABC):
     """
     SplineBasis class inherits from the Basis class and represents spline basis functions.
 
     Parameters
     ----------
@@ -425,17 +858,19 @@
     Attributes
     ----------
     order : int
         Spline order.
 
     """
 
-    def __init__(self, n_basis_funcs: int, order: int = 2) -> None:
+    def __init__(
+        self, n_basis_funcs: int, *args, mode="eval", order: int = 2, **kwargs
+    ) -> None:
         self.order = order
-        super().__init__(n_basis_funcs)
+        super().__init__(n_basis_funcs, *args, mode=mode, **kwargs)
         self._n_input_dimensionality = 1
         if self.order < 1:
             raise ValueError("Spline order must be positive!")
 
     def _generate_knots(
         self,
         sample_pts: NDArray,
@@ -444,15 +879,15 @@
         is_cyclic: bool = False,
     ) -> NDArray:
         """
         Generate knot locations for spline basis functions.
 
         Parameters
         ----------
-        sample_pts : (number of samples, )
+        sample_pts : (n_samples,)
             The sample points.
         perc_low
             The low percentile value, between [0,1).
         perc_high
             The high percentile value, between (0,1].
         is_cyclic : optional
             Whether the spline is cyclic.
@@ -504,69 +939,144 @@
             raise ValueError(
                 f"{self.__class__.__name__} `order` parameter cannot be larger "
                 "than `n_basis_funcs` parameter."
             )
 
 
 class MSplineBasis(SplineBasis):
-    """M-spline 1-dimensional basis functions.
+    """
+    M-spline[$^1$](#references) basis functions for modeling and data transformation.
+
+    M-splines are a type of spline basis function used for smooth curve fitting
+    and data representation. They are positive and integrate to one, making them
+    suitable for probabilistic models and density estimation. The order of an
+    M-spline defines its smoothness, with higher orders resulting in smoother
+    splines.
+
+    This class provides functionality to create M-spline basis functions, allowing
+    for flexible and smooth modeling of data. It inherits from the `SplineBasis`
+    abstract class, providing specific implementations for M-splines.
 
     Parameters
     ----------
     n_basis_funcs :
-        Number of basis functions.
+        The number of basis functions to generate. More basis functions allow for
+        more flexible data modeling but can lead to overfitting.
     order :
-        Order of the splines used in basis functions. Must lie within [1,
-        n_basis_funcs]. The m-splines have ``order-2`` continuous derivatives
-        at each interior knot. The higher this number, the smoother the basis
-        representation will be.
-
+        The order of the splines used in basis functions. Must be between [1,
+        n_basis_funcs]. Default is 2. Higher order splines have more continuous
+        derivatives at each interior knot, resulting in smoother basis functions.
+
+    Examples
+    --------
+    >>> from numpy import linspace
+    >>> from nemos.basis import MSplineBasis
+    >>> n_basis_funcs = 5
+    >>> order = 3
+    >>> mspline_basis = MSplineBasis(n_basis_funcs, order=order)
+    >>> sample_points = linspace(0, 1, 100)
+    >>> basis_functions = mspline_basis(sample_points)
 
     References
     ----------
-    .. [1] Ramsay, J. O. (1988). Monotone regression splines in action.
-       Statistical science, 3(4), 425-441.
-
+    [1] Ramsay, J. O. (1988). Monotone regression splines in action. Statistical science,
+        3(4), 425-441.
     """
 
-    def __init__(self, n_basis_funcs: int, order: int = 2) -> None:
-        super().__init__(n_basis_funcs, order)
-
-    def _evaluate(self, sample_pts: NDArray) -> NDArray:
-        """Generate basis functions with given spacing.
+    def __init__(
+        self, n_basis_funcs: int, *args, mode="eval", order: int = 2, **kwargs
+    ) -> None:
+        super().__init__(n_basis_funcs, *args, mode=mode, order=order, **kwargs)
+
+    @support_pynapple(conv_type="numpy")
+    @check_transform_input
+    @check_one_dimensional
+    def __call__(self, sample_pts: ArrayLike) -> FeatureMatrix:
+        """
+        Evaluate the M-spline basis functions at given sample points.
 
         Parameters
         ----------
         sample_pts :
-            Spacing for basis functions, holding elements on the interval [min(sample_pts),
-            max(sample_pts)], shape (number of samples, )
+            An array of sample points where the M-spline basis functions are to be
+            evaluated.
 
         Returns
         -------
-        basis_funcs :
-            Evaluated spline basis functions, shape (n_samples, n_basis_funcs).
+        :
+            An array where each column corresponds to one M-spline basis function
+            evaluated at the input sample points. The shape of the array is
+            (len(sample_pts), n_basis_funcs).
 
+        Notes
+        -----
+        The implementation uses a recursive definition of M-splines. Boundary
+        conditions are handled such that the basis functions are positive and
+        integrate to one over the domain defined by the sample points.
         """
         # add knots if not passed
         knot_locs = self._generate_knots(
             sample_pts, perc_low=0.0, perc_high=1.0, is_cyclic=False
         )
 
         return np.stack(
             [
                 mspline(sample_pts, self.order, i, knot_locs)
                 for i in range(self.n_basis_funcs)
             ],
             axis=1,
         )
 
+    def evaluate_on_grid(self, n_samples: int) -> Tuple[NDArray, NDArray]:
+        """
+        Evaluate the M-spline basis functions on a uniformly spaced grid.
+
+        This method creates a uniformly spaced grid of sample points within the domain
+        [0, 1] and evaluates all the M-spline basis functions at these points. It is
+        particularly useful for visualizing the shape and distribution of the basis
+        functions across their domain.
+
+        Parameters
+        ----------
+        n_samples :
+            The number of points in the uniformly spaced grid. A higher number of
+            samples will result in a more detailed visualization of the basis functions.
+
+        Returns
+        -------
+        X : NDArray
+            A 1D array of uniformly spaced sample points within the domain [0, 1].
+            Shape: `(n_samples,)`.
+        Y : NDArray
+            A 2D array where each row corresponds to the evaluated M-spline basis
+            function values at the points in X. Shape: `(n_samples, n_basis_funcs)`.
+
+        Examples
+        --------
+        Evaluate and visualize 4 M-spline basis functions of order 3:
+
+        >>> import numpy as np
+        >>> import matplotlib.pyplot as plt
+        >>> from nemos.basis import MSplineBasis
+        >>> mspline_basis = MSplineBasis(n_basis_funcs=4, order=3)
+        >>> sample_points, basis_values = mspline_basis.evaluate_on_grid(100)
+        >>> for i in range(4):
+        ...     plt.plot(sample_points, basis_values[:, i], label=f'Function {i+1}')
+        >>> plt.title('M-Spline Basis Functions')
+        >>> plt.xlabel('Domain')
+        >>> plt.ylabel('Basis Function Value')
+        >>> plt.legend()
+        >>> plt.show()
+        """
+        return super().evaluate_on_grid(n_samples)
+
 
 class BSplineBasis(SplineBasis):
     """
-    B-spline 1-dimensional basis functions.
+    B-spline[$^1$](#references) 1-dimensional basis functions.
 
     Parameters
     ----------
     n_basis_funcs :
         Number of basis functions.
     order :
         Order of the splines used in basis functions. Must lie within [1, n_basis_funcs].
@@ -577,56 +1087,83 @@
     ----------
     order :
         Spline order.
 
 
     References
     ----------
-    ..[2] Prautzsch, H., Boehm, W., Paluszny, M. (2002). B-spline representation. In: Bézier and B-Spline Techniques.
-    Mathematics and Visualization. Springer, Berlin, Heidelberg. https://doi.org/10.1007/978-3-662-04919-8_5
+    1. Prautzsch, H., Boehm, W., Paluszny, M. (2002). B-spline representation. In: Bézier and B-Spline Techniques.
+        Mathematics and Visualization. Springer, Berlin, Heidelberg. https://doi.org/10.1007/978-3-662-04919-8_5
 
     """
 
-    def __init__(self, n_basis_funcs: int, order: int = 2):
-        super().__init__(n_basis_funcs, order=order)
-
-    def _evaluate(self, sample_pts: NDArray) -> NDArray:
+    def __init__(
+        self, n_basis_funcs: int, *args, mode="eval", order: int = 4, **kwargs
+    ):
+        super().__init__(n_basis_funcs, *args, mode=mode, order=order, **kwargs)
+
+    @support_pynapple(conv_type="numpy")
+    @check_transform_input
+    @check_one_dimensional
+    def __call__(self, sample_pts: ArrayLike) -> FeatureMatrix:
         """
         Evaluate the B-spline basis functions with given sample points.
 
         Parameters
         ----------
         sample_pts :
-            The sample points at which the B-spline is evaluated.
+            The sample points at which the B-spline is evaluated, shape (n_samples,).
 
         Returns
         -------
-        NDArray
+        basis_funcs :
             The basis function evaluated at the samples, shape (n_samples, n_basis_funcs)
 
         Raises
         ------
         AssertionError
-            If the sample points are not within the B-spline knots range unless `outer_ok=True`.
+            If the sample points are not within the B-spline knots.
 
         Notes
         -----
         The evaluation is performed by looping over each element and using `splev`
         from SciPy to compute the basis values.
         """
-
         # add knots
         knot_locs = self._generate_knots(sample_pts, 0.0, 1.0)
 
         basis_eval = bspline(
             sample_pts, knot_locs, order=self.order, der=0, outer_ok=False
         )
 
         return basis_eval
 
+    def evaluate_on_grid(self, n_samples: int) -> Tuple[NDArray, NDArray]:
+        """Evaluate the B-spline basis set on a grid of equi-spaced sample points.
+
+        Parameters
+        ----------
+        n_samples :
+            The number of samples.
+
+        Returns
+        -------
+        X :
+            Array of shape (n_samples,) containing the equi-spaced sample
+            points where we've evaluated the basis.
+        basis_funcs :
+            Raised cosine basis functions, shape (n_samples, n_basis_funcs)
+
+        Notes
+        -----
+        The evaluation is performed by looping over each element and using `splev` from
+        SciPy to compute the basis values.
+        """
+        return super().evaluate_on_grid(n_samples)
+
 
 class CyclicBSplineBasis(SplineBasis):
     """
     B-spline 1-dimensional basis functions for cyclic splines.
 
     Parameters
     ----------
@@ -641,47 +1178,47 @@
     ----------
     n_basis_funcs : int
         Number of basis functions.
     order : int
         Order of the splines used in basis functions.
     """
 
-    def __init__(self, n_basis_funcs: int, order: int = 2):
-        super().__init__(n_basis_funcs, order=order)
+    def __init__(
+        self, n_basis_funcs: int, *args, mode="eval", order: int = 4, **kwargs
+    ):
+        super().__init__(n_basis_funcs, *args, mode=mode, order=order, **kwargs)
         if self.order < 2:
             raise ValueError(
                 f"Order >= 2 required for cyclic B-spline, "
                 f"order {self.order} specified instead!"
             )
 
-    def _evaluate(self, sample_pts: NDArray) -> NDArray:
-        """
-        Evaluate the B-spline basis functions with given sample points.
+    @support_pynapple(conv_type="numpy")
+    @check_transform_input
+    @check_one_dimensional
+    def __call__(self, sample_pts: ArrayLike) -> FeatureMatrix:
+        """Evaluate the Cyclic B-spline basis functions with given sample points.
 
         Parameters
         ----------
         sample_pts :
-            The sample points at which the B-spline is evaluated. Must be a tuple of length 1.
+            The sample points at which the cyclic B-spline is evaluated, shape
+            (n_samples,).
 
         Returns
         -------
-        NDArray
+        basis_funcs :
             The basis function evaluated at the samples, shape (n_samples, n_basis_funcs)
 
-        Raises
-        ------
-        AssertionError
-            If the sample points are not within the B-spline knots range unless `outer_ok=True`.
-
         Notes
         -----
         The evaluation is performed by looping over each element and using `splev` from
         SciPy to compute the basis values.
-        """
 
+        """
         knot_locs = self._generate_knots(sample_pts, 0.0, 1.0, is_cyclic=True)
 
         # for cyclic, do not repeat knots
         knot_locs = np.unique(knot_locs)
 
         nk = knot_locs.shape[0]
 
@@ -706,202 +1243,341 @@
                 sample_pts[ind], knots, order=self.order, outer_ok=True, der=0
             )
         # restore points
         sample_pts[ind] = sample_pts[ind] + knots.max() - knot_locs[0]
 
         return basis_eval
 
+    def evaluate_on_grid(self, n_samples: int) -> Tuple[NDArray, NDArray]:
+        """Evaluate the Cyclic B-spline basis set on a grid of equi-spaced sample points.
 
-class RaisedCosineBasis(Basis, abc.ABC):
-    def __init__(self, n_basis_funcs: int) -> None:
-        super().__init__(n_basis_funcs)
-        self._n_input_dimensionality = 1
+        Parameters
+        ----------
+        n_samples :
+            The number of samples.
 
-    @abc.abstractmethod
-    def _transform_samples(self, sample_pts: NDArray) -> NDArray:
+        Returns
+        -------
+        X :
+            Array of shape (n_samples,) containing the equi-spaced sample
+            points where we've evaluated the basis.
+        basis_funcs :
+            Raised cosine basis functions, shape (n_samples, n_basis_funcs)
+
+        Notes
+        -----
+        The evaluation is performed by looping over each element and using `splev` from
+        SciPy to compute the basis values.
         """
-        Abstract method for transforming sample points.
+        return super().evaluate_on_grid(n_samples)
+
+
+class RaisedCosineBasisLinear(Basis):
+    """Represent linearly-spaced raised cosine basis functions.
+
+    This implementation is based on the cosine bumps used by Pillow et al.[$^1$](#references)
+    to uniformly tile the internal points of the domain.
+
+    Parameters
+    ----------
+    n_basis_funcs :
+        The number of basis functions.
+    width :
+        Width of the raised cosine. By default, it's set to 2.0.
+
+    References
+    ----------
+    1. Pillow, J. W., Paninski, L., Uzzel, V. J., Simoncelli, E. P., & J.,
+        C. E. (2005). Prediction and decoding of retinal ganglion cell responses
+        with a probabilistic spiking model. Journal of Neuroscience, 25(47),
+        11003–11013. http://dx.doi.org/10.1523/jneurosci.3305-05.2005
+    """
+
+    def __init__(
+        self, n_basis_funcs: int, *args, mode="eval", width: float = 2.0, **kwargs
+    ) -> None:
+        super().__init__(n_basis_funcs, *args, mode=mode, **kwargs)
+        self._n_input_dimensionality = 1
+        self._check_width(width)
+        self._width = width
+
+    @property
+    def width(self):
+        """Return width of the raised cosine."""
+        return self._width
+
+    @staticmethod
+    def _check_width(width: float) -> None:
+        """Validate the width value.
 
         Parameters
         ----------
-        sample_pts :
-           The sample points to be transformed, shape (number of samples, ).
+        width :
+            The width value to validate.
+
+        Raises
+        ------
+        ValueError
+            If width <= 1 or 2*width is not a positive integer. Values that do not match
+            this constraint will result in:
+            - No overlap between bumps (width < 1).
+            - Oscillatory behavior when summing the basis elements (2*width not integer).
         """
-        pass
+        if width <= 1 or (not np.isclose(width * 2, round(2 * width))):
+            raise ValueError(
+                f"Invalid raised cosine width. "
+                f"2*width must be a positive integer, 2*width = {2 * width} instead!"
+            )
 
-    def _evaluate(self, sample_pts: NDArray) -> NDArray:
+    @support_pynapple(conv_type="numpy")
+    @check_transform_input
+    @check_one_dimensional
+    def __call__(self, sample_pts: ArrayLike, rescale_samples=True) -> FeatureMatrix:
         """Generate basis functions with given samples.
 
         Parameters
         ----------
-        sample_pts : (number of samples,)
-            Spacing for basis functions, holding elements on interval [0,
-            1). A good default is
-            ``nmo.sample_points.raised_cosine_log`` for log spacing (as used in
-            [2]_) or ``nmo.sample_points.raised_cosine_linear`` for linear
-            spacing.
+        sample_pts :
+            Spacing for basis functions, holding elements on interval [0, 1], Shape (number of samples, ).
 
         Returns
         -------
         basis_funcs :
             Raised cosine basis functions, shape (n_samples, n_basis_funcs).
 
         Raises
         ------
         ValueError
             If the sample provided do not lie in [0,1].
-        """
-        if any(sample_pts < 0) or any(sample_pts > 1):
-            raise ValueError("Sample points for RaisedCosine basis must lie in [0,1]!")
-
-        # transform to the proper domain
-        transform_sample_pts = self._transform_samples(sample_pts)
 
-        shifted_sample_pts = (
-            transform_sample_pts[:, None]
-            - (np.pi * np.arange(self.n_basis_funcs))[None, :]
+        """
+        if rescale_samples:
+            # note that sample points is converted to NDArray
+            # with the decorator.
+            # copy is necessary otherwise:
+            # basis1 = nmo.basis.RaisedCosineBasisLinear(5)
+            # basis2 = nmo.basis.RaisedCosineBasisLog(5)
+            # additive_basis = basis1 + basis2
+            # additive_basis(*([x] * 2)) would modify both inputs
+            sample_pts = min_max_rescale_samples(np.copy(sample_pts))
+
+        peaks = self._compute_peaks()
+        delta = peaks[1] - peaks[0]
+        # generate a set of shifted cosines, and constrain them to be non-zero
+        # over a single period, then enforce the codomain to be [0,1], by adding 1
+        # and then multiply by 0.5
+        basis_funcs = 0.5 * (
+            np.cos(
+                np.clip(
+                    np.pi * (sample_pts[:, None] - peaks[None]) / (delta * self.width),
+                    -np.pi,
+                    np.pi,
+                )
+            )
+            + 1
         )
-        basis_funcs = 0.5 * (np.cos(np.clip(shifted_sample_pts, -np.pi, np.pi)) + 1)
 
         return basis_funcs
 
+    def _compute_peaks(self) -> NDArray:
+        """
+        Compute the location of raised cosine peaks.
 
-class RaisedCosineBasisLinear(RaisedCosineBasis):
-    """Linearly-spaced raised cosine basis functions used by Pillow et al. [2]_.
-
-    These are "cosine bumps" that uniformly tile the space.
-
-    Parameters
-    ----------
-    n_basis_funcs
-        Number of basis functions.
-
-    References
-    ----------
-    .. [2] Pillow, J. W., Paninski, L., Uzzel, V. J., Simoncelli, E. P., & J.,
-       C. E. (2005). Prediction and decoding of retinal ganglion cell responses
-       with a probabilistic spiking model. Journal of Neuroscience, 25(47),
-       11003–11013. http://dx.doi.org/10.1523/jneurosci.3305-05.2005
-
-    """
-
-    def __init__(self, n_basis_funcs: int) -> None:
-        super().__init__(n_basis_funcs)
-
-    def _transform_samples(self, sample_pts: NDArray) -> NDArray:
+        Returns
+        -------
+            Peak locations of each basis element.
         """
-        Linearly map the samples from [0,1] to the the [0, (n_basis_funcs - 1) * pi].
+        return np.linspace(0, 1, self.n_basis_funcs)
+
+    def evaluate_on_grid(self, n_samples: int) -> Tuple[NDArray, NDArray]:
+        """Evaluate the basis set on a grid of equi-spaced sample points.
 
         Parameters
         ----------
-        sample_pts :
-            The sample points used for evaluating the splines, shape (number of samples, )
+        n_samples :
+            The number of samples.
 
         Returns
         -------
-        :
-            A transformed version of the sample points that matches the Raised Cosine basis domain,
-            shape (number of samples, ).
+        X :
+            Array of shape (n_samples,) containing the equi-spaced sample
+            points where we've evaluated the basis.
+        basis_funcs :
+            Raised cosine basis functions, shape (n_samples, n_basis_funcs)
+
         """
-        return sample_pts * np.pi * (self.n_basis_funcs - 1)
+        return super().evaluate_on_grid(n_samples)
 
     def _check_n_basis_min(self) -> None:
         """Check that the user required enough basis elements.
 
-        Check that the number of basis is at least 1.
+        Check that the number of basis is at least 2.
 
         Raises
         ------
         ValueError
-            If an insufficient number of basis element is requested for the basis type
+            If n_basis_funcs < 2.
         """
-        if self.n_basis_funcs < 1:
+        if self.n_basis_funcs < 2:
             raise ValueError(
-                f"Object class {self.__class__.__name__} requires >= 1 basis elements. "
+                f"Object class {self.__class__.__name__} requires >= 2 basis elements. "
                 f"{self.n_basis_funcs} basis elements specified instead"
             )
 
 
-class RaisedCosineBasisLog(RaisedCosineBasis):
-    """Log-spaced raised cosine basis functions used by Pillow et al. [2]_.
+class RaisedCosineBasisLog(RaisedCosineBasisLinear):
+    """Represent log-spaced raised cosine basis functions.
 
-    These are "cosine bumps" that uniformly tile the space.
+    Similar to `RaisedCosineBasisLinear` but the basis functions are log-spaced.
+    This implementation is based on the cosine bumps used by Pillow et al.[$^1$](#references)
+    to uniformly tile the internal points of the domain.
 
     Parameters
     ----------
-    n_basis_funcs
-        Number of basis functions.
+    n_basis_funcs :
+        The number of basis functions.
+    width :
+        Width of the raised cosine. By default, it's set to 2.0.
+    enforce_decay_to_zero:
+        If set to True, the algorithm first constructs a basis with `n_basis_funcs + ceil(width)` elements
+        and subsequently trims off the extra basis elements. This ensures that the final basis element
+        decays to 0.
 
     References
     ----------
-    .. [2] Pillow, J. W., Paninski, L., Uzzel, V. J., Simoncelli, E. P., & J.,
+    1. Pillow, J. W., Paninski, L., Uzzel, V. J., Simoncelli, E. P., & J.,
        C. E. (2005). Prediction and decoding of retinal ganglion cell responses
        with a probabilistic spiking model. Journal of Neuroscience, 25(47),
        11003–11013. http://dx.doi.org/10.1523/jneurosci.3305-05.2005
-
     """
 
-    def __init__(self, n_basis_funcs: int) -> None:
-        super().__init__(n_basis_funcs)
+    def __init__(
+        self,
+        n_basis_funcs: int,
+        *args,
+        mode="eval",
+        width: float = 2.0,
+        time_scaling: float = None,
+        enforce_decay_to_zero: bool = True,
+        **kwargs,
+    ) -> None:
+        super().__init__(n_basis_funcs, *args, mode=mode, width=width, **kwargs)
+        self.enforce_decay_to_zero = enforce_decay_to_zero
+        if time_scaling is None:
+            self._time_scaling = 50.0
+        else:
+            self._check_time_scaling(time_scaling)
+            self._time_scaling = time_scaling
+
+    @property
+    def time_scaling(self):
+        """Getter property for time_scaling."""
+        return self._time_scaling
 
-    def _transform_samples(self, sample_pts: NDArray) -> NDArray:
-        """Map the sample domain to log-space.
+    @staticmethod
+    def _check_time_scaling(time_scaling: float) -> None:
+        if time_scaling <= 0:
+            raise ValueError(
+                f"Only strictly positive time_scaling are allowed, {time_scaling} provided instead."
+            )
 
-        Map the equi-spaced samples from [0,1] to log equi-spaced samples [0, (n_basis_funcs - 1) * pi].
+    def _transform_samples(self, sample_pts: ArrayLike) -> NDArray:
+        """
+        Map the sample domain to log-space.
 
         Parameters
         ----------
         sample_pts :
-            The sample points used for evaluating the splines, shape (number of samples, ).
+            Sample points used for evaluating the splines,
+            shape (n_samples, ).
 
         Returns
         -------
-        :
-            A transformed version of the sample points that matches the Raised Cosine basis domain,
-            shape (n_sample_points, ).
+            Transformed version of the sample points that matches the Raised Cosine basis domain,
+            shape (n_samples, ).
         """
-        return (
-            np.power(
-                10,
-                -(np.log10((self.n_basis_funcs - 1) * np.pi) + 1) * sample_pts
-                + np.log10((self.n_basis_funcs - 1) * np.pi),
-            )
-            - 0.1
+        # rescale to [0,1]
+        # copy is necessary to avoid unwanted rescaling in additive/multiplicative basis.
+        sample_pts = min_max_rescale_samples(np.copy(sample_pts))
+        # This log-stretching of the sample axis has the following effect:
+        # - as the time_scaling tends to 0, the points will be linearly spaced across the whole domain.
+        # - as the time_scaling tends to inf, basis will be small and dense around 0 and
+        # progressively larger and less dense towards 1.
+        log_spaced_pts = np.log(self.time_scaling * sample_pts + 1) / np.log(
+            self.time_scaling + 1
         )
+        return log_spaced_pts
 
-    def _check_n_basis_min(self) -> None:
-        """Check that the user required enough basis elements.
+    def _compute_peaks(self) -> NDArray:
+        """
+        Peak location of each log-spaced cosine basis element.
 
-        Checks that the number of basis is at least 2.
+        Compute the peak location for the log-spaced raised cosine basis.
+        Enforcing that the last basis decays to zero is equivalent to
+        setting the last peak to a value smaller than 1.
+
+        Returns
+        -------
+            Peak locations of each basis element.
+
+        """
+        if self.enforce_decay_to_zero:
+            # compute the last peak location such that the last
+            # basis element decays to zero at the last sample.
+            last_peak = 1 - self.width / (self.n_basis_funcs + self.width - 1)
+        else:
+            last_peak = 1
+        return np.linspace(0, last_peak, self.n_basis_funcs)
+
+    @support_pynapple(conv_type="numpy")
+    @check_transform_input
+    @check_one_dimensional
+    def __call__(self, sample_pts: ArrayLike) -> FeatureMatrix:
+        """Generate log-spaced raised cosine basis with given samples.
+
+        Parameters
+        ----------
+        sample_pts :
+            Spacing for basis functions, holding elements on interval [0, 1].
+
+        Returns
+        -------
+        basis_funcs :
+            Log-raised cosine basis functions, shape (n_samples, n_basis_funcs).
 
         Raises
         ------
         ValueError
-            If an insufficient number of basis element is requested for the basis type
+            If the sample provided do not lie in [0,1].
         """
-        if self.n_basis_funcs < 2:
-            raise ValueError(
-                f"Object class {self.__class__.__name__} requires >= 2 basis elements. "
-                f"{self.n_basis_funcs} basis elements specified instead"
-            )
+        return super().__call__(
+            self._transform_samples(sample_pts), rescale_samples=False
+        )
 
 
 class OrthExponentialBasis(Basis):
     """Set of 1D basis decaying exponential functions numerically orthogonalized.
 
     Parameters
     ----------
     n_basis_funcs
             Number of basis functions.
     decay_rates :
             Decay rates of the exponentials, shape (n_basis_funcs,).
     """
 
-    def __init__(self, n_basis_funcs: int, decay_rates: NDArray[np.floating]):
-        super().__init__(n_basis_funcs=n_basis_funcs)
+    def __init__(
+        self,
+        n_basis_funcs: int,
+        decay_rates: NDArray[np.floating],
+        *args,
+        mode="eval",
+        **kwargs,
+    ):
+        super().__init__(n_basis_funcs=n_basis_funcs, *args, mode=mode, **kwargs)
         self._decay_rates = np.asarray(decay_rates)
         if self._decay_rates.shape[0] != n_basis_funcs:
             raise ValueError(
                 f"The number of basis functions must match the number of decay rates provided. "
                 f"Number of basis functions provided: {n_basis_funcs}, "
                 f"Number of decay rates provided: {self._decay_rates.shape[0]}"
             )
@@ -921,15 +1597,15 @@
         """
         if self.n_basis_funcs < 1:
             raise ValueError(
                 f"Object class {self.__class__.__name__} requires >= 1 basis elements. "
                 f"{self.n_basis_funcs} basis elements specified instead"
             )
 
-    def _check_rates(self):
+    def _check_rates(self) -> None:
         """
         Check if the decay rates list has duplicate entries.
 
         Raises
         ------
         ValueError
             If two or more decay rates are repeated, which would result in a linearly
@@ -937,15 +1613,16 @@
         """
         if len(set(self._decay_rates)) != len(self._decay_rates):
             raise ValueError(
                 "Two or more rate are repeated! Repeating rate will result in a "
                 "linearly dependent set of function for the basis."
             )
 
-    def _check_sample_range(self, sample_pts: NDArray):
+    @staticmethod
+    def _check_sample_range(sample_pts: NDArray) -> None:
         """
         Check if the sample points are all positive.
 
         Parameters
         ----------
         sample_pts
             Sample points to check.
@@ -957,15 +1634,15 @@
             positive samples.
         """
         if any(sample_pts < 0):
             raise ValueError(
                 "OrthExponentialBasis requires positive samples. Negative values provided instead!"
             )
 
-    def _check_sample_size(self, *sample_pts: NDArray):
+    def _check_sample_size(self, *sample_pts: NDArray) -> None:
         """Check that the sample size is greater than the number of basis.
 
         This is necessary for the orthogonalization procedure,
         that otherwise will return (sample_size, ) basis elements instead of the expected number.
 
         Parameters
         ----------
@@ -980,40 +1657,65 @@
         if sample_pts[0].size < self.n_basis_funcs:
             raise ValueError(
                 "OrthExponentialBasis requires at least as many samples as basis functions!\n"
                 f"Class instantiated with {self.n_basis_funcs} basis functions "
                 f"but only {sample_pts[0].size} samples provided!"
             )
 
-    def _evaluate(self, sample_pts: NDArray) -> NDArray:
+    @support_pynapple(conv_type="numpy")
+    @check_transform_input
+    @check_one_dimensional
+    def __call__(self, sample_pts: NDArray) -> FeatureMatrix:
         """Generate basis functions with given spacing.
 
         Parameters
         ----------
         sample_pts
-            Spacing for basis functions, holding elements on the interval [0, inf), shape (n_pts,).
+            Spacing for basis functions, holding elements on the interval [0,
+            inf), shape (n_samples,).
 
         Returns
         -------
         basis_funcs
-            Evaluated exponentially decaying basis functions,
-            numerically orthogonalized, shape (number of basis, number of samples).
+            Evaluated exponentially decaying basis functions, numerically
+            orthogonalized, shape (n_samples, n_basis_funcs)
+
         """
         self._check_sample_range(sample_pts)
         self._check_sample_size(sample_pts)
         # because of how scipy.linalg.orth works, have to create a matrix of
         # shape (n_pts, n_basis_funcs) and then transpose, rather than
         # directly computing orth on the matrix of shape (n_basis_funcs,
         # n_pts)
         return scipy.linalg.orth(
             np.stack([np.exp(-lam * sample_pts) for lam in self._decay_rates], axis=1)
         )
 
+    def evaluate_on_grid(self, n_samples: int) -> Tuple[NDArray, NDArray]:
+        """Evaluate the basis set on a grid of equi-spaced sample points.
+
+        Parameters
+        ----------
+        n_samples :
+            The number of samples.
+
+        Returns
+        -------
+        X :
+            Array of shape (n_samples,) containing the equi-spaced sample
+            points where we've evaluated the basis.
+        basis_funcs :
+            Evaluated exponentially decaying basis functions, numerically
+            orthogonalized, shape (n_samples, n_basis_funcs)
+
+        """
+        return super().evaluate_on_grid(n_samples)
+
 
-def mspline(x: NDArray, k: int, i: int, T: NDArray):
+def mspline(x: NDArray, k: int, i: int, T: NDArray) -> NDArray:
     """Compute M-spline basis function.
 
     Parameters
     ----------
     x
         Spacing for basis functions, shape (n_sample_points, ).
     k
@@ -1052,25 +1754,26 @@
 
 def bspline(
     sample_pts: NDArray,
     knots: NDArray,
     order: int = 4,
     der: int = 0,
     outer_ok: bool = False,
-):
+) -> NDArray:
     """
     Calculate and return the evaluation of B-spline basis.
 
     This function evaluates B-spline basis for given sample points. It checks for
     out of range points and optionally handles them. It also handles the NaNs if present.
 
     Parameters
     ----------
     sample_pts :
-        An array containing sample points for which B-spline basis needs to be evaluated.
+        An array containing sample points for which B-spline basis needs to be evaluated,
+        shape (n_samples,)
     knots :
         An array containing knots for the B-spline basis. The knots are sorted in ascending order.
     order :
         The order of the B-spline basis.
     der :
         The derivative of the B-spline basis to be evaluated.
     outer_ok :
@@ -1114,15 +1817,15 @@
     else:
         reps = 0
 
     # number of basis elements
     n_basis = nk - order
 
     # initialize the basis element container
-    basis_eval = np.zeros((n_basis - 2 * reps, sample_pts.shape[0]))
+    basis_eval = np.full((n_basis - 2 * reps, sample_pts.shape[0]), np.nan)
 
     # loop one element at the time and evaluate the basis using splev
     id_basis = np.eye(n_basis, nk, dtype=np.int8)
     for i in range(reps, len(knots) - order - reps):
         basis_eval[i - reps, in_sample] = splev(
             sample_pts[in_sample], (knots, id_basis[i], order - 1), der=der
         )
```

### Comparing `nemos-0.1.0/tests/test_basis.py` & `nemos-0.1.1/tests/test_glm.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,1696 +1,2013 @@
-import abc
-import inspect
+from contextlib import nullcontext as does_not_raise
 
-import jax.numpy
+import jax
+import jax.numpy as jnp
 import numpy as np
 import pytest
-import utils_testing
+import statsmodels.api as sm
+from sklearn.model_selection import GridSearchCV
 
-import nemos.basis as basis
+import nemos as nmo
+from nemos.pytrees import FeaturePytree
 
-# automatic define user accessible basis and check the methods
 
+def test_validate_higher_dimensional_data_X(mock_glm):
+    """Test behavior with higher-dimensional input data."""
+    X = jnp.array([[[[1, 2], [3, 4]]]])
+    y = jnp.array([1, 2])
+    with pytest.raises(ValueError, match="X must be two-dimensional"):
+        mock_glm._validate(X, y, mock_glm._initialize_parameters(X, y))
 
-def test_all_basis_are_tested() -> None:
-    """Meta-test.
 
-    Ensure that all concrete classes in the 'basis' module are tested.
-    """
-    # Get all classes from the current module.
-    all_classes = inspect.getmembers(
-        inspect.getmodule(inspect.currentframe()), inspect.isclass
-    )
-
-    # Filter the classes that are subclasses of 'SuperClass'.
-    subclasses = [
-        cls
-        for _, cls in all_classes
-        if issubclass(cls, BasisFuncsTesting) and cls != BasisFuncsTesting
-    ]
-
-    # Create the set of basis function objects that are tested using the cls definition
-    tested_bases = {test_cls.cls for test_cls in subclasses}
-
-    # Create the set of all the concrete basis classes
-    all_bases = {
-        class_obj for _, class_obj in utils_testing.get_non_abstract_classes(basis)
-    }
-
-    if all_bases != all_bases.intersection(tested_bases):
-        raise ValueError(
-            "Test should be implemented for each of the concrete classes in the basis module.\n"
-            f"The following classes are not tested: {[bas.__qualname__ for bas in all_bases.difference(tested_bases)]}"
-        )
+def test_preprocess_fit_higher_dimensional_data_y(mock_glm):
+    """Test behavior with higher-dimensional input data."""
+    X = jnp.array([[[1, 2], [3, 4]]])
+    y = jnp.array([[[1, 2]]])
+    with pytest.raises(ValueError, match="y must be one-dimensional"):
+        mock_glm._validate(X, y, mock_glm._initialize_parameters(X, y))
 
 
-class BasisFuncsTesting(abc.ABC):
-    """
-    An abstract base class that sets the foundation for individual basis function testing.
-    This class requires an implementation of a 'cls' method, which is utilized by the meta-test
-    that verifies if all basis functions are properly tested.
-    """
+def test_validate_lower_dimensional_data_X(mock_glm):
+    """Test behavior with lower-dimensional input data."""
+    X = jnp.array([1, 2])
+    y = jnp.array([1, 2])
+    with pytest.raises(ValueError, match="X must be two-dimensional"):
+        mock_glm._validate(X, y, mock_glm._initialize_parameters(X, y))
 
-    @abc.abstractmethod
-    def cls(self):
-        pass
 
+class TestGLM:
+    """
+    Unit tests for the PoissonGLM class.
+    """
 
-class TestRaisedCosineLogBasis(BasisFuncsTesting):
-    cls = basis.RaisedCosineBasisLog
-
-    @pytest.mark.parametrize("samples", [[], [0], [0, 0]])
-    def test_non_empty_samples(self, samples):
-        if len(samples) == 0:
-            with pytest.raises(
-                ValueError, match="All sample provided must be non empty"
-            ):
-                self.cls(5).evaluate(samples)
-        else:
-            self.cls(5).evaluate(samples)
-
+    #######################
+    # Test model.__init__
+    #######################
     @pytest.mark.parametrize(
-        "arraylike", [0, [0], (0,), np.array([0]), jax.numpy.array([0])]
+        "regularizer, expectation",
+        [
+            (nmo.regularizer.Ridge("BFGS"), does_not_raise()),
+            (
+                None,
+                pytest.raises(
+                    AttributeError, match="The provided `solver` doesn't implement "
+                ),
+            ),
+            (
+                nmo.regularizer.Ridge,
+                pytest.raises(
+                    TypeError, match="The provided `solver` cannot be instantiated"
+                ),
+            ),
+        ],
     )
-    def test_input_to_evaluate_is_arraylike(self, arraylike):
+    def test_solver_type(self, regularizer, expectation, glm_class):
         """
-        Checks that the sample size of the output from the evaluate() method matches the input sample size.
+        Test that an error is raised if a non-compatible solver is passed.
         """
-        basis_obj = self.cls(n_basis_funcs=5)
-        raise_exception = not isinstance(
-            arraylike, (tuple, list, np.ndarray, jax.numpy.ndarray)
-        )
-        if raise_exception:
-            with pytest.raises(TypeError, match="Input samples must be array-like"):
-                basis_obj.evaluate(arraylike)
-        else:
-            basis_obj.evaluate(arraylike)
+        with expectation:
+            glm_class(regularizer=regularizer)
 
     @pytest.mark.parametrize(
-        "args, sample_size",
-        [[{"n_basis_funcs": n_basis}, 100] for n_basis in [2, 10, 100]],
+        "observation, expectation",
+        [
+            (nmo.observation_models.PoissonObservations(), does_not_raise()),
+            (
+                nmo.regularizer.Regularizer,
+                pytest.raises(
+                    AttributeError,
+                    match="The provided object does not have the required",
+                ),
+            ),
+            (
+                1,
+                pytest.raises(
+                    AttributeError,
+                    match="The provided object does not have the required",
+                ),
+            ),
+        ],
     )
-    def test_evaluate_returns_expected_number_of_basis(self, args, sample_size):
-        """
-        Verifies the number of basis functions returned by the evaluate() method matches
-        the expected number of basis functions.
-        """
-        basis_obj = self.cls(**args)
-        eval_basis = basis_obj.evaluate(np.linspace(0, 1, sample_size))
-        if eval_basis.shape[1] != args["n_basis_funcs"]:
-            raise ValueError(
-                "Dimensions do not agree: The number of basis should match the first dimension of the evaluated basis."
-                f"The number of basis is {args['n_basis_funcs']}",
-                f"The first dimension of the evaluated basis is {eval_basis.shape[1]}",
-            )
-        return
-
-    @pytest.mark.parametrize("sample_size", [100, 1000])
-    @pytest.mark.parametrize("n_basis_funcs", [2, 10, 100])
-    def test_sample_size_of_evaluate_matches_that_of_input(
-        self, n_basis_funcs, sample_size
+    def test_init_observation_type(
+        self, observation, expectation, glm_class, ridge_regularizer
     ):
         """
-        Checks that the sample size of the output from the evaluate() method matches the input sample size.
-        """
-        basis_obj = self.cls(n_basis_funcs=n_basis_funcs)
-        eval_basis = basis_obj.evaluate(np.linspace(0, 1, sample_size))
-        if eval_basis.shape[0] != sample_size:
-            raise ValueError(
-                f"Dimensions do not agree: The window size should match the second dimension of the evaluated basis."
-                f"The window size is {sample_size}",
-                f"The second dimension of the evaluated basis is {eval_basis.shape[0]}",
-            )
-
-    @pytest.mark.parametrize("n_basis_funcs", [-1, 0, 1, 3, 10, 20])
-    def test_minimum_number_of_basis_required_is_matched(self, n_basis_funcs):
-        """
-        Verifies that the minimum number of basis functions required (i.e., 2) is enforced.
+        Test initialization with different regularizer names. Check if an appropriate exception is raised
+        when the regularizer name is not present in jaxopt.
         """
-        raise_exception = n_basis_funcs < 2
-        if raise_exception:
-            with pytest.raises(
-                ValueError,
-                match=f"Object class {self.cls.__name__} "
-                "requires >= 2 basis elements.",
-            ):
-                self.cls(n_basis_funcs=n_basis_funcs)
-        else:
-            self.cls(n_basis_funcs=n_basis_funcs)
+        with expectation:
+            glm_class(regularizer=ridge_regularizer, observation_model=observation)
 
     @pytest.mark.parametrize(
-        "sample_range", [(0, 1), (0.1, 0.9), (-0.5, 1), (0, 1.5), (-0.5, 1.5)]
+        "X, y",
+        [
+            (jnp.zeros((2, 4)), jnp.zeros((2,))),
+            (jnp.zeros((2, 4)), jnp.zeros((2,))),
+        ],
     )
-    def test_samples_range_matches_evaluate_requirements(self, sample_range: tuple):
-        """
-        Ensures that the evaluate() method correctly handles sample range inputs that are outside of its required bounds (0, 1).
-        """
-        raise_exception = (sample_range[0] < 0) | (sample_range[1] > 1)
-        basis_obj = self.cls(n_basis_funcs=5)
-        if raise_exception:
-            with pytest.raises(
-                ValueError, match="Sample points for RaisedCosine basis must lie in"
-            ):
-                basis_obj.evaluate(np.linspace(*sample_range, 100))
-        else:
-            basis_obj.evaluate(np.linspace(*sample_range, 100))
-
-    @pytest.mark.parametrize("n_input", [0, 1, 2, 3])
-    def test_number_of_required_inputs_evaluate(self, n_input):
-        """
-        Confirms that the evaluate() method correctly handles the number of input samples that are provided.
-        """
-        basis_obj = self.cls(n_basis_funcs=5)
-        raise_exception = n_input != basis_obj._n_input_dimensionality
-        inputs = [np.linspace(0, 1, 20)] * n_input
-        if raise_exception:
-            with pytest.raises(
-                ValueError,
-                match="Input dimensionality mismatch. This basis evaluation requires [0-9]+ "
-                "inputs,",
-            ):
-                basis_obj.evaluate(*inputs)
-        else:
-            basis_obj.evaluate(*inputs)
-
-    @pytest.mark.parametrize("sample_size", [-1, 0, 1, 10, 11, 100])
-    def test_evaluate_on_grid_meshgrid_size(self, sample_size):
-        """
-        Checks that the evaluate_on_grid() method returns a grid of the expected size.
-        """
-        basis_obj = self.cls(n_basis_funcs=5)
-        raise_exception = sample_size <= 0
-        if raise_exception:
-            with pytest.raises(
-                ValueError, match=r"All sample counts provided must be greater"
-            ):
-                basis_obj.evaluate_on_grid(sample_size)
-        else:
-            grid, _ = basis_obj.evaluate_on_grid(sample_size)
-            assert grid.shape[0] == sample_size
-
-    @pytest.mark.parametrize("sample_size", [-1, 0, 1, 10, 11, 100])
-    def test_evaluate_on_grid_basis_size(self, sample_size):
+    def test_parameter_initialization(self, X, y, poissonGLM_model_instantiation):
+        _, _, model, _, _ = poissonGLM_model_instantiation
+        coef, inter = model._initialize_parameters(X, y)
+        assert coef.shape == (X.shape[1],)
+        assert inter.shape == (1,)
+
+    #######################
+    # Test model.fit
+    #######################
+    @pytest.mark.parametrize(
+        "n_params, expectation",
+        [
+            (0, pytest.raises(ValueError, match="Params must have length two.")),
+            (1, pytest.raises(ValueError, match="Params must have length two.")),
+            (2, does_not_raise()),
+            (3, pytest.raises(ValueError, match="Params must have length two.")),
+        ],
+    )
+    def test_fit_param_length(
+        self, n_params, expectation, poissonGLM_model_instantiation
+    ):
         """
-        Ensures that the evaluate_on_grid() method returns basis functions of the expected size.
+        Test the `fit` method with different numbers of initial parameters.
+        Check for correct number of parameters.
         """
-        basis_obj = self.cls(n_basis_funcs=5)
-        raise_exception = sample_size <= 0
-        if raise_exception:
-            with pytest.raises(
-                ValueError, match=r"All sample counts provided must be greater"
-            ):
-                basis_obj.evaluate_on_grid(sample_size)
+        X, y, model, true_params, firing_rate = poissonGLM_model_instantiation
+        if n_params == 0:
+            init_params = tuple()
+        elif n_params == 1:
+            init_params = (true_params[0],)
         else:
-            _, eval_basis = basis_obj.evaluate_on_grid(sample_size)
-            assert eval_basis.shape[0] == sample_size
+            init_params = true_params + (true_params[0],) * (n_params - 2)
+        with expectation:
+            model.fit(X, y, init_params=init_params)
 
-    @pytest.mark.parametrize("n_input", [0, 1, 2])
-    def test_evaluate_on_grid_input_number(self, n_input):
+    @pytest.mark.parametrize(
+        "add_entry, add_to, expectation",
+        [
+            (0, "X", does_not_raise()),
+            (
+                np.nan,
+                "X",
+                pytest.warns(UserWarning, match="The provided trees contain"),
+            ),
+            (
+                np.inf,
+                "X",
+                pytest.warns(UserWarning, match="The provided trees contain"),
+            ),
+            (0, "y", does_not_raise()),
+            (
+                np.nan,
+                "y",
+                pytest.warns(UserWarning, match="The provided trees contain"),
+            ),
+            (
+                np.inf,
+                "y",
+                pytest.warns(UserWarning, match="The provided trees contain"),
+            ),
+        ],
+    )
+    def test_fit_param_values(
+        self, add_entry, add_to, expectation, poissonGLM_model_instantiation
+    ):
         """
-        Validates that the evaluate_on_grid() method correctly handles the number of input samples that are provided.
+        Test the `fit` method with altered X or y values. Ensure the method raises exceptions for NaN or Inf values.
         """
-        basis_obj = self.cls(n_basis_funcs=5)
-        inputs = [10] * n_input
-        raise_exception = n_input != basis_obj._n_input_dimensionality
-        if raise_exception:
-            with pytest.raises(
-                ValueError,
-                match=r"Input dimensionality mismatch\. This basis evaluation requires [0-9]+ inputs, "
-                r"[0-9]+ inputs provided instead.",
-            ):
-                basis_obj.evaluate_on_grid(*inputs)
-        else:
-            basis_obj.evaluate_on_grid(*inputs)
-
-
-class TestRaisedCosineLinearBasis(BasisFuncsTesting):
-    cls = basis.RaisedCosineBasisLinear
-
-    @pytest.mark.parametrize("samples", [[], [0], [0, 0]])
-    def test_non_empty_samples(self, samples):
-        if len(samples) == 0:
-            with pytest.raises(
-                ValueError, match="All sample provided must be non empty"
-            ):
-                self.cls(5).evaluate(samples)
-        else:
-            self.cls(5).evaluate(samples)
+        X, y, model, true_params, firing_rate = poissonGLM_model_instantiation
+        if add_to == "X":
+            # get an index to be edited
+            idx = np.unravel_index(np.random.choice(X.size), X.shape)
+            X[idx] = add_entry
+        elif add_to == "y":
+            idx = np.unravel_index(np.random.choice(y.size), y.shape)
+            y = np.asarray(y, dtype=np.float32)
+            y[idx] = add_entry
+        with expectation:
+            model.fit(X, y, init_params=true_params)
 
     @pytest.mark.parametrize(
-        "arraylike", [0, [0], (0,), np.array([0]), jax.numpy.array([0])]
+        "dim_weights, expectation",
+        [
+            (
+                0,
+                pytest.raises(
+                    ValueError,
+                    match=r"Inconsistent number of features",
+                ),
+            ),
+            (
+                1,
+                does_not_raise(),
+            ),
+            (
+                2,
+                pytest.raises(
+                    ValueError,
+                    match=r"params\[0\] must be an array or .* of shape \(n_features",
+                ),
+            ),
+            (
+                3,
+                pytest.raises(
+                    ValueError,
+                    match=r"params\[0\] must be an array or .* of shape \(n_features",
+                ),
+            ),
+        ],
     )
-    def test_input_to_evaluate_is_arraylike(self, arraylike):
+    def test_fit_weights_dimensionality(
+        self, dim_weights, expectation, poissonGLM_model_instantiation
+    ):
         """
-        Checks that the sample size of the output from the evaluate() method matches the input sample size.
+        Test the `fit` method with weight matrices of different dimensionalities.
+        Check for correct dimensionality.
         """
-        basis_obj = self.cls(n_basis_funcs=5)
-        raise_exception = not isinstance(
-            arraylike, (tuple, list, np.ndarray, jax.numpy.ndarray)
-        )
-        if raise_exception:
-            with pytest.raises(TypeError, match="Input samples must be array-like"):
-                basis_obj.evaluate(arraylike)
+        X, y, model, true_params, firing_rate = poissonGLM_model_instantiation
+        n_samples, n_features = X.shape
+        n_neurons = 4
+        if dim_weights == 0:
+            init_w = jnp.array([])
+        elif dim_weights == 1:
+            init_w = jnp.zeros((n_features,))
+        elif dim_weights == 2:
+            init_w = jnp.zeros((n_features, n_neurons))
         else:
-            basis_obj.evaluate(arraylike)
+            init_w = jnp.zeros((n_features, n_neurons) + (1,) * (dim_weights - 2))
+        with expectation:
+            model.fit(X, y, init_params=(init_w, true_params[1]))
 
     @pytest.mark.parametrize(
-        "args, sample_size",
-        [[{"n_basis_funcs": n_basis}, 100] for n_basis in [1, 2, 10, 100]],
+        "dim_intercepts, expectation",
+        [
+            (0, pytest.raises(ValueError, match=r"params\[1\] must be of shape")),
+            (1, does_not_raise()),
+            (2, pytest.raises(ValueError, match=r"params\[1\] must be of shape")),
+            (3, pytest.raises(ValueError, match=r"params\[1\] must be of shape")),
+        ],
     )
-    def test_evaluate_returns_expected_number_of_basis(self, args, sample_size):
-        """
-        Verifies that the evaluate() method returns the expected number of basis functions.
-        """
-        basis_obj = self.cls(**args)
-        eval_basis = basis_obj.evaluate(np.linspace(0, 1, sample_size))
-        if eval_basis.shape[1] != args["n_basis_funcs"]:
-            raise ValueError(
-                "Dimensions do not agree: The number of basis should match the first dimension of the evaluated basis."
-                f"The number of basis is {args['n_basis_funcs']}",
-                f"The first dimension of the evaluated basis is {eval_basis.shape[1]}",
-            )
-        return
-
-    @pytest.mark.parametrize("sample_size", [100, 1000])
-    @pytest.mark.parametrize("n_basis_funcs", [2, 10, 100])
-    def test_sample_size_of_evaluate_matches_that_of_input(
-        self, n_basis_funcs, sample_size
+    def test_fit_intercepts_dimensionality(
+        self, dim_intercepts, expectation, poissonGLM_model_instantiation
     ):
         """
-        Checks that the sample size of the output from the evaluate() method matches the input sample size.
+        Test the `fit` method with intercepts of different dimensionalities. Check for correct dimensionality.
         """
-        basis_obj = self.cls(n_basis_funcs=n_basis_funcs)
-        eval_basis = basis_obj.evaluate(np.linspace(0, 1, sample_size))
-        if eval_basis.shape[0] != sample_size:
-            raise ValueError(
-                f"Dimensions do not agree: The window size should match the second dimension of the evaluated basis."
-                f"The window size is {sample_size}",
-                f"The second dimension of the evaluated basis is {eval_basis.shape[0]}",
-            )
+        X, y, model, true_params, firing_rate = poissonGLM_model_instantiation
+        n_samples, n_features = X.shape
+        init_b = jnp.zeros((1,) * dim_intercepts)
+        init_w = jnp.zeros((n_features,))
+        with expectation:
+            model.fit(X, y, init_params=(init_w, init_b))
 
-    @pytest.mark.parametrize("n_basis_funcs", [-1, 0, 1, 3, 10, 20])
-    def test_minimum_number_of_basis_required_is_matched(self, n_basis_funcs):
+    @pytest.mark.parametrize(
+        "init_params, expectation",
+        [
+            ([jnp.zeros((5,)), jnp.zeros((1,))], does_not_raise()),
+            (
+                [[jnp.zeros((1, 5)), jnp.zeros((1,))]],
+                pytest.raises(ValueError, match="Params must have length two."),
+            ),
+            (dict(p1=jnp.zeros((5,)), p2=jnp.zeros((1,))), pytest.raises(KeyError)),
+            (
+                (dict(p1=jnp.zeros((5,)), p2=jnp.zeros((1,))), jnp.zeros((1,))),
+                pytest.raises(
+                    TypeError, match=r"X and params\[0\] must be the same type"
+                ),
+            ),
+            (
+                (
+                    FeaturePytree(p1=jnp.zeros((5,)), p2=jnp.zeros((5,))),
+                    jnp.zeros((1,)),
+                ),
+                pytest.raises(
+                    TypeError, match=r"X and params\[0\] must be the same type"
+                ),
+            ),
+            (0, pytest.raises(ValueError, match="Params must have length two.")),
+            (
+                {0, 1},
+                pytest.raises(TypeError, match="Initial parameters must be array-like"),
+            ),
+            (
+                [jnp.zeros((1, 5)), ""],
+                pytest.raises(TypeError, match="Initial parameters must be array-like"),
+            ),
+            (
+                ["", jnp.zeros((1,))],
+                pytest.raises(TypeError, match="Initial parameters must be array-like"),
+            ),
+        ],
+    )
+    def test_fit_init_params_type(
+        self, init_params, expectation, poissonGLM_model_instantiation
+    ):
         """
-        Verifies that the minimum number of basis functions required (i.e., 1) is enforced.
+        Test the `fit` method with various types of initial parameters. Ensure that the provided initial parameters
+        are array-like.
         """
-        raise_exception = n_basis_funcs < 1
-        if raise_exception:
-            with pytest.raises(
-                ValueError,
-                match=f"Object class {self.cls.__name__} "
-                "requires >= 1 basis elements\.",
-            ):
-                self.cls(n_basis_funcs=n_basis_funcs)
-        else:
-            self.cls(n_basis_funcs=n_basis_funcs)
+        X, y, model, true_params, firing_rate = poissonGLM_model_instantiation
+        with expectation:
+            model.fit(X, y, init_params=init_params)
 
     @pytest.mark.parametrize(
-        "sample_range", [(0, 1), (0.1, 0.9), (-0.5, 1), (0, 1.5), (-0.5, 1.5)]
+        "delta_dim, expectation",
+        [
+            (-1, pytest.raises(ValueError, match="X must be two-dimensional")),
+            (0, does_not_raise()),
+            (1, pytest.raises(ValueError, match="X must be two-dimensional")),
+        ],
     )
-    def test_samples_range_matches_evaluate_requirements(self, sample_range: tuple):
+    def test_fit_x_dimensionality(
+        self, delta_dim, expectation, poissonGLM_model_instantiation
+    ):
         """
-        Ensures that the evaluate() method correctly handles sample range inputs that are outside of its required bounds (0, 1).
+        Test the `fit` method with X input data of different dimensionalities. Ensure correct dimensionality for X.
         """
-        raise_exception = (sample_range[0] < 0) | (sample_range[1] > 1)
-        basis_obj = self.cls(n_basis_funcs=5)
-        if raise_exception:
-            with pytest.raises(
-                ValueError, match="Sample points for RaisedCosine basis must lie in"
-            ):
-                basis_obj.evaluate(np.linspace(*sample_range, 100))
-        else:
-            basis_obj.evaluate(np.linspace(*sample_range, 100))
+        X, y, model, true_params, firing_rate = poissonGLM_model_instantiation
+        if delta_dim == -1:
+            X = np.zeros((X.shape[0],))
+        elif delta_dim == 1:
+            X = np.zeros((X.shape[0], 1, X.shape[1]))
+        with expectation:
+            model.fit(X, y, init_params=true_params)
 
-    @pytest.mark.parametrize("n_input", [0, 1, 2, 3])
-    def test_number_of_required_inputs_evaluate(self, n_input):
+    @pytest.mark.parametrize(
+        "delta_dim, expectation",
+        [
+            (-1, pytest.raises(ValueError, match="y must be one-dimensional")),
+            (0, does_not_raise()),
+            (1, pytest.raises(ValueError, match="y must be one-dimensional")),
+        ],
+    )
+    def test_fit_y_dimensionality(
+        self, delta_dim, expectation, poissonGLM_model_instantiation
+    ):
         """
-        Confirms that the evaluate() method correctly handles the number of input samples that are provided.
+        Test the `fit` method with y target data of different dimensionalities. Ensure correct dimensionality for y.
         """
-        basis_obj = self.cls(n_basis_funcs=5)
-        raise_exception = n_input != basis_obj._n_input_dimensionality
-        inputs = [np.linspace(0, 1, 20)] * n_input
-        if raise_exception:
-            with pytest.raises(
-                ValueError,
-                match="Input dimensionality mismatch. This basis evaluation requires [0-9]+ inputs,",
-            ):
-                basis_obj.evaluate(*inputs)
-        else:
-            basis_obj.evaluate(*inputs)
+        X, y, model, true_params, firing_rate = poissonGLM_model_instantiation
+        if delta_dim == -1:
+            y = np.zeros([])
+        elif delta_dim == 1:
+            y = np.zeros((y.shape[0], 1))
+        with expectation:
+            model.fit(X, y, init_params=true_params)
 
-    @pytest.mark.parametrize("sample_size", [-1, 0, 1, 10, 11, 100])
-    def test_evaluate_on_grid_meshgrid_size(self, sample_size):
+    @pytest.mark.parametrize(
+        "delta_n_features, expectation",
+        [
+            (-1, pytest.raises(ValueError, match="Inconsistent number of features")),
+            (0, does_not_raise()),
+            (1, pytest.raises(ValueError, match="Inconsistent number of features")),
+        ],
+    )
+    def test_fit_n_feature_consistency_weights(
+        self, delta_n_features, expectation, poissonGLM_model_instantiation
+    ):
         """
-        Checks that the evaluate_on_grid() method returns a grid of the expected size.
+        Test the `fit` method for inconsistencies between data features and initial weights provided.
+        Ensure the number of features align.
         """
-        basis_obj = self.cls(n_basis_funcs=5)
-        raise_exception = sample_size <= 0
-        if raise_exception:
-            with pytest.raises(
-                ValueError, match=r"All sample counts provided must be greater"
-            ):
-                basis_obj.evaluate_on_grid(sample_size)
-        else:
-            grid, _ = basis_obj.evaluate_on_grid(sample_size)
-            assert grid.shape[0] == sample_size
+        X, y, model, true_params, firing_rate = poissonGLM_model_instantiation
+        init_w = jnp.zeros((X.shape[1] + delta_n_features))
+        init_b = jnp.zeros(
+            1,
+        )
+        with expectation:
+            model.fit(X, y, init_params=(init_w, init_b))
 
-    @pytest.mark.parametrize("sample_size", [-1, 0, 1, 10, 11, 100])
-    def test_evaluate_on_grid_basis_size(self, sample_size):
+    @pytest.mark.parametrize(
+        "delta_n_features, expectation",
+        [
+            (-1, pytest.raises(ValueError, match="Inconsistent number of features")),
+            (0, does_not_raise()),
+            (1, pytest.raises(ValueError, match="Inconsistent number of features")),
+        ],
+    )
+    def test_fit_n_feature_consistency_x(
+        self, delta_n_features, expectation, poissonGLM_model_instantiation
+    ):
         """
-        Ensures that the evaluate_on_grid() method returns basis functions of the expected size.
+        Test the `fit` method for inconsistencies between data features and model's expectations.
+        Ensure the number of features in X aligns.
         """
-        basis_obj = self.cls(n_basis_funcs=5)
-        raise_exception = sample_size <= 0
-        if raise_exception:
-            with pytest.raises(
-                ValueError, match=r"All sample counts provided must be greater"
-            ):
-                basis_obj.evaluate_on_grid(sample_size)
-        else:
-            _, eval_basis = basis_obj.evaluate_on_grid(sample_size)
-            assert eval_basis.shape[0] == sample_size
+        X, y, model, true_params, firing_rate = poissonGLM_model_instantiation
+        if delta_n_features == 1:
+            X = jnp.concatenate((X, jnp.zeros((X.shape[0], 1))), axis=1)
+        elif delta_n_features == -1:
+            X = X[..., :-1]
+        with expectation:
+            model.fit(X, y, init_params=true_params)
 
-    @pytest.mark.parametrize("n_input", [0, 1, 2])
-    def test_evaluate_on_grid_input_number(self, n_input):
+    @pytest.mark.parametrize(
+        "delta_tp, expectation",
+        [
+            (
+                -1,
+                pytest.raises(ValueError, match="The number of time-points in X and y"),
+            ),
+            (0, does_not_raise()),
+            (
+                1,
+                pytest.raises(ValueError, match="The number of time-points in X and y"),
+            ),
+        ],
+    )
+    def test_fit_time_points_x(
+        self, delta_tp, expectation, poissonGLM_model_instantiation
+    ):
         """
-        Validates that the evaluate_on_grid() method correctly handles the number of input samples that are provided.
+        Test the `fit` method for inconsistencies in time-points in data X. Ensure the correct number of time-points.
         """
-        basis_obj = self.cls(n_basis_funcs=5)
-        inputs = [10] * n_input
-        raise_exception = n_input != basis_obj._n_input_dimensionality
-        if raise_exception:
-            with pytest.raises(
-                ValueError,
-                match=r"Input dimensionality mismatch\. This basis evaluation requires [0-9]+ inputs, "
-                r"[0-9]+ inputs provided instead.",
-            ):
-                basis_obj.evaluate_on_grid(*inputs)
-        else:
-            basis_obj.evaluate_on_grid(*inputs)
-
-
-class TestMSplineBasis(BasisFuncsTesting):
-    cls = basis.MSplineBasis
-
-    @pytest.mark.parametrize("samples", [[], [0], [0, 0]])
-    def test_non_empty_samples(self, samples):
-        if len(samples) == 0:
-            with pytest.raises(
-                ValueError, match="All sample provided must be non empty"
-            ):
-                self.cls(5).evaluate(samples)
-        else:
-            self.cls(5).evaluate(samples)
+        X, y, model, true_params, firing_rate = poissonGLM_model_instantiation
+        X = jnp.zeros((X.shape[0] + delta_tp,) + X.shape[1:])
+        with expectation:
+            model.fit(X, y, init_params=true_params)
 
     @pytest.mark.parametrize(
-        "arraylike", [0, [0], (0,), np.array([0]), jax.numpy.array([0])]
+        "delta_tp, expectation",
+        [
+            (
+                -1,
+                pytest.raises(ValueError, match="The number of time-points in X and y"),
+            ),
+            (0, does_not_raise()),
+            (
+                1,
+                pytest.raises(ValueError, match="The number of time-points in X and y"),
+            ),
+        ],
     )
-    def test_input_to_evaluate_is_arraylike(self, arraylike):
+    def test_fit_time_points_y(
+        self, delta_tp, expectation, poissonGLM_model_instantiation
+    ):
         """
-        Checks that the sample size of the output from the evaluate() method matches the input sample size.
+        Test the `fit` method for inconsistencies in time-points in y. Ensure the correct number of time-points.
         """
-        basis_obj = self.cls(n_basis_funcs=5)
-        raise_exception = not isinstance(
-            arraylike, (tuple, list, np.ndarray, jax.numpy.ndarray)
+        X, y, model, true_params, firing_rate = poissonGLM_model_instantiation
+        y = jnp.zeros((y.shape[0] + delta_tp,) + y.shape[1:])
+        with expectation:
+            model.fit(X, y, init_params=true_params)
+
+    def test_fit_mask_grouplasso(self, group_sparse_poisson_glm_model_instantiation):
+        """Test that the group lasso fit goes through"""
+        X, y, model, params, rate, mask = group_sparse_poisson_glm_model_instantiation
+        model.set_params(
+            regularizer=nmo.regularizer.GroupLasso(
+                solver_name="ProximalGradient", mask=mask
+            )
         )
-        if raise_exception:
-            with pytest.raises(TypeError, match="Input samples must be array-like"):
-                basis_obj.evaluate(arraylike)
-        else:
-            basis_obj.evaluate(arraylike)
+        model.fit(X, y)
 
-    @pytest.mark.parametrize("n_basis_funcs", [6, 8, 10])
-    @pytest.mark.parametrize("order", range(1, 6))
-    def test_evaluate_returns_expected_number_of_basis(
-        self, n_basis_funcs: int, order: int
+    def test_fit_pytree_equivalence(
+        self, poissonGLM_model_instantiation, poissonGLM_model_instantiation_pytree
     ):
-        """
-        Verifies that the evaluate() method returns the expected number of basis functions.
-        """
-        basis_obj = self.cls(n_basis_funcs=n_basis_funcs, order=order)
-        eval_basis = basis_obj.evaluate(np.linspace(0, 1, 100))
-        if eval_basis.shape[1] != n_basis_funcs:
-            raise ValueError(
-                "Dimensions do not agree: The number of basis should match the first dimension of the evaluated basis."
-                f"The number of basis is {n_basis_funcs}",
-                f"The first dimension of the evaluated basis is {eval_basis.shape[1]}",
-            )
-        return
+        """Check that the glm fit with pytree learns the same parameters."""
+        # required for numerical precision of coeffs
+        jax.config.update("jax_enable_x64", True)
+        X, y, model, true_params, firing_rate = poissonGLM_model_instantiation
+        X_tree, _, model_tree, true_params_tree, _ = (
+            poissonGLM_model_instantiation_pytree
+        )
+        # fit both models
+        model.fit(X, y, init_params=true_params)
+        model_tree.fit(X_tree, y, init_params=true_params_tree)
+
+        # get the flat parameters
+        flat_coef = np.concatenate(
+            jax.tree_util.tree_flatten(model_tree.coef_)[0], axis=-1
+        )
+
+        # assert equivalence of solutions
+        assert np.allclose(model.coef_, flat_coef)
+        assert np.allclose(model.intercept_, model_tree.intercept_)
+        assert np.allclose(model.score(X, y), model_tree.score(X_tree, y))
+        assert np.allclose(model.predict(X), model_tree.predict(X_tree))
 
-    @pytest.mark.parametrize("sample_size", [100, 1000])
-    @pytest.mark.parametrize("n_basis_funcs", [4, 10, 100])
-    @pytest.mark.parametrize("order", [1, 2, 3])
-    def test_sample_size_of_evaluate_matches_that_of_input(
-        self, n_basis_funcs, sample_size, order
+    @pytest.mark.parametrize(
+        "fill_val, expectation",
+        [
+            (0, does_not_raise()),
+            (
+                jnp.inf,
+                pytest.raises(
+                    ValueError, match="At least a NaN or an Inf at all sample points"
+                ),
+            ),
+            (
+                jnp.nan,
+                pytest.raises(
+                    ValueError, match="At least a NaN or an Inf at all sample points"
+                ),
+            ),
+        ],
+    )
+    def test_fit_all_invalid_X(
+        self, fill_val, expectation, poissonGLM_model_instantiation
+    ):
+        X, y, model, true_params, firing_rate = poissonGLM_model_instantiation
+        X.fill(fill_val)
+        with expectation:
+            model.fit(X, y)
+
+    #######################
+    # Test model.score
+    #######################
+    @pytest.mark.parametrize(
+        "delta_dim, expectation",
+        [
+            (-1, pytest.raises(ValueError, match="X must be two-dimensional")),
+            (0, does_not_raise()),
+            (1, pytest.raises(ValueError, match="X must be two-dimensional")),
+        ],
+    )
+    def test_score_x_dimensionality(
+        self, delta_dim, expectation, poissonGLM_model_instantiation
     ):
         """
-        Checks that the sample size of the output from the evaluate() method matches the input sample size.
+        Test the `score` method with X input data of different dimensionalities. Ensure correct dimensionality for X.
         """
-        basis_obj = self.cls(n_basis_funcs=n_basis_funcs, order=order)
-        eval_basis = basis_obj.evaluate(np.linspace(0, 1, sample_size))
-        if eval_basis.shape[0] != sample_size:
-            raise ValueError(
-                f"Dimensions do not agree: The window size should match the second dimension of the evaluated basis."
-                f"The window size is {sample_size}",
-                f"The second dimension of the evaluated basis is {eval_basis.shape[0]}",
-            )
-
-    @pytest.mark.parametrize("n_basis_funcs", [-1, 0, 1, 3, 10, 20])
-    @pytest.mark.parametrize("order", [-1, 0, 1, 2, 3, 4, 5])
-    def test_minimum_number_of_basis_required_is_matched(self, n_basis_funcs, order):
-        """
-        Verifies that the minimum number of basis functions and order required (i.e., at least 1) and
-        order < #basis are enforced.
-        """
-        raise_exception = (order < 1) | (n_basis_funcs < 1) | (order > n_basis_funcs)
-        if raise_exception:
-            with pytest.raises(
-                ValueError,
-                match=r"Spline order must be positive!|"
-                rf"{self.cls.__name__} `order` parameter cannot be larger than",
-            ):
-                basis_obj = self.cls(n_basis_funcs=n_basis_funcs, order=order)
-                basis_obj.evaluate(np.linspace(0, 1, 10))
-        else:
-            basis_obj = self.cls(n_basis_funcs=n_basis_funcs, order=order)
-            basis_obj.evaluate(np.linspace(0, 1, 10))
+        X, y, model, true_params, firing_rate = poissonGLM_model_instantiation
+        model.coef_ = true_params[0]
+        model.intercept_ = true_params[1]
+        if delta_dim == -1:
+            X = np.zeros((X.shape[0],))
+        elif delta_dim == 1:
+            X = np.zeros((X.shape[0], X.shape[1], 1))
+        with expectation:
+            model.score(X, y)
 
     @pytest.mark.parametrize(
-        "sample_range", [(0, 1), (0.1, 0.9), (-0.5, 1), (0, 1.5), (-0.5, 1.5)]
+        "delta_dim, expectation",
+        [
+            (
+                -1,
+                pytest.raises(
+                    ValueError, match="y must be one-dimensional, with shape"
+                ),
+            ),
+            (0, does_not_raise()),
+            (
+                1,
+                pytest.raises(
+                    ValueError, match="y must be one-dimensional, with shape"
+                ),
+            ),
+        ],
     )
-    def test_samples_range_matches_evaluate_requirements(self, sample_range: tuple):
+    def test_score_y_dimensionality(
+        self, delta_dim, expectation, poissonGLM_model_instantiation
+    ):
         """
-        Verifies that the evaluate() method can handle input range.
+        Test the `score` method with y of different dimensionalities.
+        Ensure correct dimensionality for y.
         """
-        basis_obj = self.cls(n_basis_funcs=5, order=3)
-        basis_obj.evaluate(np.linspace(*sample_range, 100))
+        X, y, model, true_params, firing_rate = poissonGLM_model_instantiation
+        model.coef_ = true_params[0]
+        model.intercept_ = true_params[1]
+        if delta_dim == -1:
+            y = np.zeros([])
+        elif delta_dim == 1:
+            y = np.zeros((X.shape[0], X.shape[1]))
+        with expectation:
+            model.score(X, y)
 
-    @pytest.mark.parametrize("n_input", [0, 1, 2, 3])
-    def test_number_of_required_inputs_evaluate(self, n_input):
+    @pytest.mark.parametrize(
+        "delta_n_features, expectation",
+        [
+            (-1, pytest.raises(ValueError, match="Inconsistent number of features")),
+            (0, does_not_raise()),
+            (1, pytest.raises(ValueError, match="Inconsistent number of features")),
+        ],
+    )
+    def test_score_n_feature_consistency_x(
+        self, delta_n_features, expectation, poissonGLM_model_instantiation
+    ):
         """
-        Confirms that the evaluate() method correctly handles the number of input samples that are provided.
+        Test the `score` method for inconsistencies in features of X.
+        Ensure the number of features in X aligns with the model params.
         """
-        basis_obj = self.cls(n_basis_funcs=5, order=3)
-        raise_exception = n_input != basis_obj._n_input_dimensionality
-        inputs = [np.linspace(0, 1, 20)] * n_input
-        if raise_exception:
-            with pytest.raises(
-                ValueError,
-                match="Input dimensionality mismatch. This basis evaluation requires [0-9]+ inputs,",
-            ):
-                basis_obj.evaluate(*inputs)
-        else:
-            basis_obj.evaluate(*inputs)
+        X, y, model, true_params, firing_rate = poissonGLM_model_instantiation
+        model.coef_ = true_params[0]
+        model.intercept_ = true_params[1]
+        if delta_n_features == 1:
+            X = jnp.concatenate((X, jnp.zeros((X.shape[0], 1))), axis=1)
+        elif delta_n_features == -1:
+            X = X[..., :-1]
+        with expectation:
+            model.score(X, y)
 
-    @pytest.mark.parametrize("sample_size", [-1, 0, 1, 10, 11, 100])
-    def test_evaluate_on_grid_meshgrid_size(self, sample_size):
+    @pytest.mark.parametrize(
+        "is_fit, expectation",
+        [
+            (True, does_not_raise()),
+            (
+                False,
+                pytest.raises(ValueError, match="This GLM instance is not fitted yet"),
+            ),
+        ],
+    )
+    def test_predict_is_fit(self, is_fit, expectation, poissonGLM_model_instantiation):
         """
-        Checks that the evaluate_on_grid() method returns a grid of the expected size.
+        Test the `score` method on models based on their fit status.
+        Ensure scoring is only possible on fitted models.
         """
-        basis_obj = self.cls(n_basis_funcs=5, order=3)
-        raise_exception = sample_size <= 0
-        if raise_exception:
-            with pytest.raises(
-                ValueError, match=r"All sample counts provided must be greater"
-            ):
-                basis_obj.evaluate_on_grid(sample_size)
-        else:
-            grid, _ = basis_obj.evaluate_on_grid(sample_size)
-            assert grid.shape[0] == sample_size
+        X, y, model, true_params, firing_rate = poissonGLM_model_instantiation
+        if is_fit:
+            model.fit(X, y)
+        with expectation:
+            model.predict(X)
 
-    @pytest.mark.parametrize("sample_size", [-1, 0, 1, 10, 11, 100])
-    def test_evaluate_on_grid_basis_size(self, sample_size):
+    @pytest.mark.parametrize(
+        "delta_tp, expectation",
+        [
+            (
+                -1,
+                pytest.raises(ValueError, match="The number of time-points in X and y"),
+            ),
+            (0, does_not_raise()),
+            (
+                1,
+                pytest.raises(ValueError, match="The number of time-points in X and y"),
+            ),
+        ],
+    )
+    def test_score_time_points_x(
+        self, delta_tp, expectation, poissonGLM_model_instantiation
+    ):
         """
-        Ensures that the evaluate_on_grid() method returns basis functions of the expected size.
+        Test the `score` method for inconsistencies in time-points in X.
+        Ensure that the number of time-points in X and y matches.
         """
-        basis_obj = self.cls(n_basis_funcs=5, order=3)
-        raise_exception = sample_size <= 0
-        if raise_exception:
-            with pytest.raises(
-                ValueError, match=r"All sample counts provided must be greater"
-            ):
-                basis_obj.evaluate_on_grid(sample_size)
-        else:
-            _, eval_basis = basis_obj.evaluate_on_grid(sample_size)
-            assert eval_basis.shape[0] == sample_size
+        X, y, model, true_params, firing_rate = poissonGLM_model_instantiation
+        model.coef_ = true_params[0]
+        model.intercept_ = true_params[1]
+        X = jnp.zeros((X.shape[0] + delta_tp,) + X.shape[1:])
+        with expectation:
+            model.score(X, y)
 
-    @pytest.mark.parametrize("n_input", [0, 1, 2])
-    def test_evaluate_on_grid_input_number(self, n_input):
+    @pytest.mark.parametrize(
+        "delta_tp, expectation",
+        [
+            (
+                -1,
+                pytest.raises(ValueError, match="The number of time-points in X and y"),
+            ),
+            (0, does_not_raise()),
+            (
+                1,
+                pytest.raises(ValueError, match="The number of time-points in X and y"),
+            ),
+        ],
+    )
+    def test_score_time_points_y(
+        self, delta_tp, expectation, poissonGLM_model_instantiation
+    ):
         """
-        Validates that the evaluate_on_grid() method correctly handles the number of input samples that are provided.
+        Test the `score` method for inconsistencies in time-points in y.
+        Ensure that the number of time-points in X and y matches.
         """
-        basis_obj = self.cls(n_basis_funcs=5, order=3)
-        inputs = [10] * n_input
-        raise_exception = n_input != basis_obj._n_input_dimensionality
-        if raise_exception:
-            with pytest.raises(
-                ValueError,
-                match=r"Input dimensionality mismatch\. This basis evaluation requires [0-9]+ inputs, "
-                r"[0-9]+ inputs provided instead.",
-            ):
-                basis_obj.evaluate_on_grid(*inputs)
-        else:
-            basis_obj.evaluate_on_grid(*inputs)
-
-
-class TestOrthExponentialBasis(BasisFuncsTesting):
-    cls = basis.OrthExponentialBasis
-
-    # this class requires at leas `n_basis` samples
-    @pytest.mark.parametrize("samples", [[], [0] * 6, [0] * 7])
-    def test_non_empty_samples(self, samples):
-        if len(samples) == 0:
-            with pytest.raises(
-                ValueError, match="All sample provided must be non empty"
-            ):
-                self.cls(5, decay_rates=np.arange(1, 6)).evaluate(samples)
-        else:
-            self.cls(5, decay_rates=np.arange(1, 6)).evaluate(samples)
+        X, y, model, true_params, firing_rate = poissonGLM_model_instantiation
+        model.coef_ = true_params[0]
+        model.intercept_ = true_params[1]
+        y = jnp.zeros((y.shape[0] + delta_tp,) + y.shape[1:])
+        with expectation:
+            model.score(X, y)
 
     @pytest.mark.parametrize(
-        "arraylike", [0, [0]*6, (0,)*6, np.array([0]*6), jax.numpy.array([0]*6)]
+        "score_type, expectation",
+        [
+            ("pseudo-r2-McFadden", does_not_raise()),
+            ("pseudo-r2-Cohen", does_not_raise()),
+            ("log-likelihood", does_not_raise()),
+            (
+                "not-implemented",
+                pytest.raises(
+                    NotImplementedError,
+                    match="Scoring method not-implemented not implemented",
+                ),
+            ),
+        ],
     )
-    def test_input_to_evaluate_is_arraylike(self, arraylike):
+    def test_score_type_r2(
+        self, score_type, expectation, poissonGLM_model_instantiation
+    ):
         """
-        Checks that the sample size of the output from the evaluate() method matches the input sample size.
+        Test the `score` method for unsupported scoring types.
+        Ensure only valid score types are used.
         """
-        basis_obj = self.cls(n_basis_funcs=5, decay_rates=np.arange(1, 6))
-        raise_exception = not isinstance(
-            arraylike, (tuple, list, np.ndarray, jax.numpy.ndarray)
-        )
-        if raise_exception:
-            with pytest.raises(TypeError, match="Input samples must be array-like"):
-                basis_obj.evaluate(arraylike)
-        else:
-            basis_obj.evaluate(arraylike)
-
-    @pytest.mark.parametrize("n_basis_funcs", [1, 2, 4, 8])
-    @pytest.mark.parametrize("sample_size", [10, 1000])
-    def test_evaluate_returns_expected_number_of_basis(
-        self, n_basis_funcs, sample_size
-    ):
-        """Tests whether the evaluate method returns the expected number of basis functions."""
-        decay_rates = np.arange(1, 1 + n_basis_funcs)
-        basis_obj = self.cls(n_basis_funcs=n_basis_funcs, decay_rates=decay_rates)
-        eval_basis = basis_obj.evaluate(np.linspace(0, 1, sample_size))
-        if eval_basis.shape[1] != n_basis_funcs:
+        X, y, model, true_params, firing_rate = poissonGLM_model_instantiation
+        model.coef_ = true_params[0]
+        model.intercept_ = true_params[1]
+        with expectation:
+            model.score(X, y, score_type=score_type)
+
+    def test_loglikelihood_against_scipy_stats(self, poissonGLM_model_instantiation):
+        """
+        Compare the model's log-likelihood computation against `jax.scipy`.
+        Ensure consistent and correct calculations.
+        """
+        X, y, model, true_params, firing_rate = poissonGLM_model_instantiation
+        # set model coeff
+        model.coef_ = true_params[0]
+        model.intercept_ = true_params[1]
+        # get the rate
+        mean_firing = model.predict(X)
+        # compute the log-likelihood using jax.scipy
+        mean_ll_jax = jax.scipy.stats.poisson.logpmf(y, mean_firing).mean()
+        model_ll = model.score(X, y, score_type="log-likelihood")
+        if not np.allclose(mean_ll_jax, model_ll):
             raise ValueError(
-                "Dimensions do not agree: The number of basis should match the first dimension of the evaluated basis."
-                f"The number of basis is {n_basis_funcs}",
-                f"The first dimension of the evaluated basis is {eval_basis.shape[1]}",
+                "Log-likelihood of PoissonModel does not match" "that of jax.scipy!"
             )
-        return
-
-    @pytest.mark.parametrize("sample_size", [100, 1000])
-    @pytest.mark.parametrize("n_basis_funcs", [2, 10, 20])
-    def test_sample_size_of_evaluate_matches_that_of_input(
-        self, n_basis_funcs, sample_size
-    ):
-        """Tests whether the sample size of the evaluated result matches that of the input."""
-        decay_rates = np.arange(1, 1 + n_basis_funcs)
-        basis_obj = self.cls(n_basis_funcs=n_basis_funcs, decay_rates=decay_rates)
-        eval_basis = basis_obj.evaluate(np.linspace(0, 1, sample_size))
-        if eval_basis.shape[0] != sample_size:
-            raise ValueError(
-                f"Dimensions do not agree: The window size should match the second dimension of the evaluated basis."
-                f"The window size is {sample_size}",
-                f"The second dimension of the evaluated basis is {eval_basis.shape[0]}",
-            )
-
-    @pytest.mark.parametrize("n_basis_funcs", [-1, 0, 1, 3, 10, 20])
-    def test_minimum_number_of_basis_required_is_matched(self, n_basis_funcs):
-        """Tests whether the class instance has a minimum number of basis functions."""
-        raise_exception = n_basis_funcs < 1
-        decay_rates = np.arange(1, 1 + n_basis_funcs)
-        if raise_exception:
-            with pytest.raises(
-                ValueError,
-                match=f"Object class {self.cls.__name__} "
-                r"requires >= 1 basis elements\.",
-            ):
-                self.cls(n_basis_funcs=n_basis_funcs, decay_rates=decay_rates)
-        else:
-            self.cls(n_basis_funcs=n_basis_funcs, decay_rates=decay_rates)
 
+    #######################
+    # Test model.predict
+    #######################
     @pytest.mark.parametrize(
-        "sample_range", [(0, 1), (0.1, 0.9), (-0.5, 1), (0, 1.5), (-0.5, 1.5)]
+        "delta_dim, expectation",
+        [
+            (-1, pytest.raises(ValueError, match="X must be two-dimensional")),
+            (0, does_not_raise()),
+            (1, pytest.raises(ValueError, match="X must be two-dimensional")),
+        ],
     )
-    def test_samples_range_matches_evaluate_requirements(self, sample_range: tuple):
+    def test_predict_x_dimensionality(
+        self, delta_dim, expectation, poissonGLM_model_instantiation
+    ):
         """
-        Tests whether the evaluate method correctly processes the given sample range.
-        Raises an exception for negative samples
+        Test the `predict` method with x input data of different dimensionalities.
+        Ensure correct dimensionality for x.
         """
-        raise_exception = sample_range[0] < 0
-        basis_obj = self.cls(n_basis_funcs=5, decay_rates=np.arange(1, 6))
-        if raise_exception:
-            with pytest.raises(
-                ValueError,
-                match=rf"{self.cls.__name__} requires positive samples\. "
-                r"Negative values provided instead\!",
-            ):
-                basis_obj.evaluate(np.linspace(*sample_range, 100))
-        else:
-            basis_obj.evaluate(np.linspace(*sample_range, 100))
-
-    @pytest.mark.parametrize("n_input", [0, 1, 2, 3])
-    def test_number_of_required_inputs_evaluate(self, n_input):
-        """Tests whether the evaluate method correctly processes the number of required inputs."""
-        basis_obj = self.cls(n_basis_funcs=5, decay_rates=np.arange(1, 6))
-        raise_exception = n_input != basis_obj._n_input_dimensionality
-        inputs = [np.linspace(0, 1, 20)] * n_input
-        if raise_exception:
-            with pytest.raises(
-                ValueError,
-                match="Input dimensionality mismatch. This basis evaluation requires [0-9]+ inputs,",
-            ):
-                basis_obj.evaluate(*inputs)
-        else:
-            basis_obj.evaluate(*inputs)
-
-    @pytest.mark.parametrize("sample_size", [-1, 0, 1, 2, 3, 4, 5, 6, 10, 11, 100])
-    def test_evaluate_on_grid_meshgrid_size(self, sample_size):
-        """Tests whether the evaluate_on_grid method correctly outputs the grid mesh size."""
-        basis_obj = self.cls(n_basis_funcs=5, decay_rates=np.arange(1, 6))
-        raise_exception = sample_size < 5
-        if raise_exception:
-            with pytest.raises(
-                ValueError,
-                match=rf"{self.cls.__name__} requires at least as "
-                r"many samples as basis functions\!|"
-                r"All sample counts provided must be greater",
-            ):
-                basis_obj.evaluate_on_grid(sample_size)
-        else:
-            grid, _ = basis_obj.evaluate_on_grid(sample_size)
-            assert grid.shape[0] == sample_size
-
-    @pytest.mark.parametrize("sample_size", [-1, 0, 1, 10, 11, 100])
-    def test_evaluate_on_grid_basis_size(self, sample_size):
-        """Tests whether the evaluate_on_grid method correctly outputs the basis size."""
-        basis_obj = self.cls(n_basis_funcs=5, decay_rates=np.arange(1, 6))
-        raise_exception = sample_size < 5
-        if raise_exception:
-            with pytest.raises(
-                ValueError,
-                match=r"All sample counts provided must be greater|"
-                rf"{self.cls.__name__} requires at least as many samples as basis",
-            ):
-                basis_obj.evaluate_on_grid(sample_size)
-        else:
-            _, eval_basis = basis_obj.evaluate_on_grid(sample_size)
-            assert eval_basis.shape[0] == sample_size
-
-    @pytest.mark.parametrize("n_input", [0, 1, 2])
-    def test_evaluate_on_grid_input_number(self, n_input):
-        """Tests whether the evaluate_on_grid method correctly processes the Input dimensionality."""
-        basis_obj = self.cls(n_basis_funcs=5, decay_rates=np.arange(1, 6))
-        inputs = [10] * n_input
-        raise_exception = n_input != basis_obj._n_input_dimensionality
-        if raise_exception:
-            with pytest.raises(
-                ValueError,
-                match=r"Input dimensionality mismatch\. This basis evaluation requires [0-9]+ inputs, "
-                r"[0-9]+ inputs provided instead.",
-            ):
-                basis_obj.evaluate_on_grid(*inputs)
-        else:
-            basis_obj.evaluate_on_grid(*inputs)
+        X, y, model, true_params, firing_rate = poissonGLM_model_instantiation
+        model.coef_ = true_params[0]
+        model.intercept_ = true_params[1]
+        if delta_dim == -1:
+            X = np.zeros((X.shape[0],))
+        elif delta_dim == 1:
+            X = np.zeros((X.shape[0], X.shape[1], 1))
+        with expectation:
+            model.predict(X)
 
     @pytest.mark.parametrize(
-        "decay_rates", [[1, 2, 3], [0.01, 0.02, 0.001], [2, 1, 1, 2.4]]
+        "delta_n_features, expectation",
+        [
+            (-1, pytest.raises(ValueError, match="Inconsistent number of features")),
+            (0, does_not_raise()),
+            (1, pytest.raises(ValueError, match="Inconsistent number of features")),
+        ],
     )
-    def test_decay_rate_repetition(self, decay_rates):
+    def test_predict_n_feature_consistency_x(
+        self, delta_n_features, expectation, poissonGLM_model_instantiation
+    ):
         """
-        Tests whether the class instance correctly processes the decay rates without repetition.
-        A repeated rate causes linear algebra issues, and should raise a ValyeError exception.
+        Test the `predict` method ensuring the number of features in x input data
+        is consistent with the model's `model.coef_`.
         """
-        decay_rates = np.asarray(decay_rates, dtype=float)
-        # raise exception if any of the decay rate is repeated
-        raise_exception = len(set(decay_rates)) != len(decay_rates)
-        if raise_exception:
-            with pytest.raises(
-                ValueError, match=r"Two or more rate are repeated\! Repeating rate will"
-            ):
-                self.cls(n_basis_funcs=len(decay_rates), decay_rates=decay_rates)
-        else:
-            self.cls(n_basis_funcs=len(decay_rates), decay_rates=decay_rates)
-
-    @pytest.mark.parametrize(
-        "decay_rates", [[], [1], [1, 2, 3], [1, 0.01, 0.02, 0.001]]
-    )
-    @pytest.mark.parametrize("n_basis_func", [1, 2, 3, 4])
-    def test_decay_rate_size_match_n_basis_func(self, decay_rates, n_basis_func):
-        """Tests whether the size of decay rates matches the number of basis functions."""
-        raise_exception = len(decay_rates) != n_basis_func
-        decay_rates = np.asarray(decay_rates, dtype=float)
-        if raise_exception:
-            with pytest.raises(
-                ValueError, match="The number of basis functions must match the"
-            ):
-                self.cls(n_basis_funcs=n_basis_func, decay_rates=decay_rates)
-        else:
-            self.cls(n_basis_funcs=n_basis_func, decay_rates=decay_rates)
-
-
-class TestBSplineBasis(BasisFuncsTesting):
-    cls = basis.BSplineBasis
-
-    @pytest.mark.parametrize("samples", [[], [0], [0, 0]])
-    def test_non_empty_samples(self, samples):
-        if len(samples) == 0:
-            with pytest.raises(
-                ValueError, match="All sample provided must be non empty"
-            ):
-                self.cls(5).evaluate(samples)
-        else:
-            self.cls(5).evaluate(samples)
+        X, y, model, true_params, firing_rate = poissonGLM_model_instantiation
+        model.coef_ = true_params[0]
+        model.intercept_ = true_params[1]
+        if delta_n_features == 1:
+            X = jnp.concatenate((X, jnp.zeros((X.shape[0], 1))), axis=1)
+        elif delta_n_features == -1:
+            X = X[..., :-1]
+        with expectation:
+            model.predict(X)
 
     @pytest.mark.parametrize(
-        "arraylike", [0, [0], (0,), np.array([0]), jax.numpy.array([0])]
+        "is_fit, expectation",
+        [
+            (True, does_not_raise()),
+            (
+                False,
+                pytest.raises(ValueError, match="This GLM instance is not fitted yet"),
+            ),
+        ],
     )
-    def test_input_to_evaluate_is_arraylike(self, arraylike):
+    def test_predict_is_fit(self, is_fit, expectation, poissonGLM_model_instantiation):
         """
-        Checks that the sample size of the output from the evaluate() method matches the input sample size.
+        Test the `score` method on models based on their fit status.
+        Ensure scoring is only possible on fitted models.
         """
-        basis_obj = self.cls(n_basis_funcs=5)
-        raise_exception = not isinstance(
-            arraylike, (tuple, list, np.ndarray, jax.numpy.ndarray)
-        )
-        if raise_exception:
-            with pytest.raises(TypeError, match="Input samples must be array-like"):
-                basis_obj.evaluate(arraylike)
-        else:
-            basis_obj.evaluate(arraylike)
-
-    @pytest.mark.parametrize("n_basis_funcs", [6, 8, 10])
-    @pytest.mark.parametrize("order", range(1, 6))
-    def test_evaluate_returns_expected_number_of_basis(
-        self, n_basis_funcs: int, order: int
+        X, y, model, true_params, firing_rate = poissonGLM_model_instantiation
+        if is_fit:
+            model.fit(X, y)
+        with expectation:
+            model.predict(X)
+
+    #######################
+    # Test model.simulate
+    #######################
+    @pytest.mark.parametrize(
+        "delta_dim, expectation",
+        [
+            (-1, pytest.raises(ValueError, match="X must be two-dimensional")),
+            (0, does_not_raise()),
+            (1, pytest.raises(ValueError, match="X must be two-dimensional")),
+        ],
+    )
+    def test_simulate_input_dimensionality(
+        self, delta_dim, expectation, poissonGLM_model_instantiation
     ):
         """
-        Verifies that the evaluate() method returns the expected number of basis functions.
+        Test the `simulate` method with input data of different dimensionalities.
+        Ensure correct dimensionality for input.
         """
-        basis_obj = self.cls(n_basis_funcs=n_basis_funcs, order=order)
-        eval_basis = basis_obj.evaluate(np.linspace(0, 1, 100))
-        if eval_basis.shape[1] != n_basis_funcs:
-            raise ValueError(
-                "Dimensions do not agree: The number of basis should match the first dimension of the evaluated basis."
-                f"The number of basis is {n_basis_funcs}",
-                f"The first dimension of the evaluated basis is {eval_basis.shape[1]}",
+        X, y, model, true_params, firing_rate = poissonGLM_model_instantiation
+        model.coef_ = true_params[0]
+        model.intercept_ = true_params[1]
+        if delta_dim == -1:
+            X = np.zeros(X.shape[:-1])
+        elif delta_dim == 1:
+            X = np.zeros(X.shape + (1,))
+        with expectation:
+            model.simulate(
+                random_key=jax.random.key(123),
+                feedforward_input=X,
             )
-        return
 
-    @pytest.mark.parametrize("sample_size", [100, 1000])
-    @pytest.mark.parametrize("n_basis_funcs", [4, 10, 100])
-    @pytest.mark.parametrize("order", [1, 2, 3])
-    def test_sample_size_of_evaluate_matches_that_of_input(
-        self, n_basis_funcs, sample_size, order
-    ):
+    @pytest.mark.parametrize(
+        "is_fit, expectation",
+        [
+            (True, does_not_raise()),
+            (
+                False,
+                pytest.raises(ValueError, match="This GLM instance is not fitted yet"),
+            ),
+        ],
+    )
+    def test_simulate_is_fit(self, is_fit, expectation, poissonGLM_model_instantiation):
         """
-        Checks that the sample size of the output from the evaluate() method matches the input sample size.
+        Test if the model raises a ValueError when trying to simulate before it's fitted.
         """
-        basis_obj = self.cls(n_basis_funcs=n_basis_funcs, order=order)
-        eval_basis = basis_obj.evaluate(np.linspace(0, 1, sample_size))
-        if eval_basis.shape[0] != sample_size:
-            raise ValueError(
-                f"Dimensions do not agree: The window size should match the second dimension of the evaluated basis."
-                f"The window size is {sample_size}",
-                f"The second dimension of the evaluated basis is {eval_basis.shape[0]}",
+        X, y, model, true_params, firing_rate = poissonGLM_model_instantiation
+        if is_fit:
+            model.coef_ = true_params[0]
+            model.intercept_ = true_params[1]
+        with expectation:
+            model.simulate(
+                random_key=jax.random.key(123),
+                feedforward_input=X,
             )
 
-    @pytest.mark.parametrize("n_basis_funcs", [-1, 0, 1, 3, 10, 20])
-    @pytest.mark.parametrize("order", [1, 2, 3, 4, 5])
-    def test_minimum_number_of_basis_required_is_matched(self, n_basis_funcs, order):
-        """
-        Verifies that the minimum number of basis functions and order required (i.e., at least 1) and
-        order < #basis are enforced.
-        """
-        raise_exception = order > n_basis_funcs
-        if raise_exception:
-            with pytest.raises(
-                ValueError,
-                match=rf"{self.cls.__name__} `order` parameter cannot be larger than",
-            ):
-                basis_obj = self.cls(n_basis_funcs=n_basis_funcs, order=order)
-                basis_obj.evaluate(np.linspace(0, 1, 10))
-        else:
-            basis_obj = self.cls(n_basis_funcs=n_basis_funcs, order=order)
-            basis_obj.evaluate(np.linspace(0, 1, 10))
-
-    @pytest.mark.parametrize("n_basis_funcs", [10])
-    @pytest.mark.parametrize("order", [-1, 0, 1, 2])
-    def test_order_is_positive(self, n_basis_funcs, order):
-        """
-        Verifies that the minimum number of basis functions and order required (i.e., at least 1) and
-        order < #basis are enforced.
-        """
-        raise_exception = order < 1
-        if raise_exception:
-            with pytest.raises(ValueError, match=r"Spline order must be positive!"):
-                basis_obj = self.cls(n_basis_funcs=n_basis_funcs, order=order)
-                basis_obj.evaluate(np.linspace(0, 1, 10))
-        else:
-            basis_obj = self.cls(n_basis_funcs=n_basis_funcs, order=order)
-            basis_obj.evaluate(np.linspace(0, 1, 10))
-
     @pytest.mark.parametrize(
-        "sample_range", [(0, 1), (0.1, 0.9), (-0.5, 1), (0, 1.5), (-0.5, 1.5)]
+        "delta_features, expectation",
+        [
+            (
+                -1,
+                pytest.raises(
+                    ValueError,
+                    match="Inconsistent number of features. spike basis coefficients has",
+                ),
+            ),
+            (0, does_not_raise()),
+            (
+                1,
+                pytest.raises(
+                    ValueError,
+                    match="Inconsistent number of features. spike basis coefficients has",
+                ),
+            ),
+        ],
     )
-    def test_samples_range_matches_evaluate_requirements(self, sample_range: tuple):
-        """
-        Verifies that the evaluate() method can handle input range.
-        """
-        basis_obj = self.cls(n_basis_funcs=5, order=3)
-        basis_obj.evaluate(np.linspace(*sample_range, 100))
-
-    @pytest.mark.parametrize("n_input", [0, 1, 2, 3])
-    def test_number_of_required_inputs_evaluate(self, n_input):
-        """
-        Confirms that the evaluate() method correctly handles the number of input samples that are provided.
-        """
-        basis_obj = self.cls(n_basis_funcs=5, order=3)
-        raise_exception = n_input != basis_obj._n_input_dimensionality
-        inputs = [np.linspace(0, 1, 20)] * n_input
-        if raise_exception:
-            with pytest.raises(
-                ValueError,
-                match="Input dimensionality mismatch. This basis evaluation requires [0-9]+ inputs,",
-            ):
-                basis_obj.evaluate(*inputs)
-        else:
-            basis_obj.evaluate(*inputs)
-
-    @pytest.mark.parametrize("sample_size", [-1, 0, 1, 10, 11, 100])
-    def test_evaluate_on_grid_meshgrid_size(self, sample_size):
-        """
-        Checks that the evaluate_on_grid() method returns a grid of the expected size.
+    def test_simulate_feature_consistency_input(
+        self, delta_features, expectation, poissonGLM_model_instantiation
+    ):
         """
-        basis_obj = self.cls(n_basis_funcs=5, order=3)
-        raise_exception = sample_size <= 0
-        if raise_exception:
-            with pytest.raises(
-                ValueError,
-                match=r"Invalid input data|"
-                rf"All sample counts provided must be greater",
-            ):
-                basis_obj.evaluate_on_grid(sample_size)
-        else:
-            grid, _ = basis_obj.evaluate_on_grid(sample_size)
-            assert grid.shape[0] == sample_size
+        Test the `simulate` method ensuring the number of features in `feedforward_input` is
+        consistent with the model's expected number of features.
 
-    @pytest.mark.parametrize("sample_size", [-1, 0, 1, 10, 11, 100])
-    def test_evaluate_on_grid_basis_size(self, sample_size):
-        """
-        Ensures that the evaluate_on_grid() method returns basis functions of the expected size.
-        """
-        basis_obj = self.cls(n_basis_funcs=5, order=3)
-        raise_exception = sample_size <= 0
-        if raise_exception:
-            with pytest.raises(
-                ValueError,
-                match=r"All sample counts provided must be greater|"
-                r"Invalid input data",
-            ):
-                basis_obj.evaluate_on_grid(sample_size)
-        else:
-            _, eval_basis = basis_obj.evaluate_on_grid(sample_size)
-            assert eval_basis.shape[0] == sample_size
+        Notes
+        -----
+        The total feature number `model.coef_.shape[1]` must be equal to
+        `feedforward_input.shape[2] + coupling_basis.shape[1]*n_neurons`
+        """
+        X, y, model, true_params, firing_rate = poissonGLM_model_instantiation
+        model.coef_ = true_params[0]
+        model.intercept_ = true_params[1]
+        feedforward_input = jnp.zeros(
+            (
+                X.shape[0],
+                X.shape[1] + delta_features,
+            )
+        )
+        with expectation:
+            model.simulate(
+                random_key=jax.random.key(123),
+                feedforward_input=feedforward_input,
+            )
 
-    @pytest.mark.parametrize("n_input", [0, 1, 2])
-    def test_evaluate_on_grid_input_number(self, n_input):
-        """
-        Validates that the evaluate_on_grid() method correctly handles the number of input samples that are provided.
-        """
-        basis_obj = self.cls(n_basis_funcs=5, order=3)
-        inputs = [10] * n_input
-        raise_exception = n_input != basis_obj._n_input_dimensionality
-        if raise_exception:
-            with pytest.raises(
-                ValueError,
-                match=r"Input dimensionality mismatch\. This basis evaluation requires [0-9]+ inputs",
-            ):
-                basis_obj.evaluate_on_grid(*inputs)
-        else:
-            basis_obj.evaluate_on_grid(*inputs)
+    def test_simulate_feedforward_glm(self, poissonGLM_model_instantiation):
+        """Test that simulate goes through"""
+        X, y, model, params, rate = poissonGLM_model_instantiation
+        model.coef_ = params[0]
+        model.intercept_ = params[1]
+        ysim, ratesim = model.simulate(jax.random.key(123), X)
+        # check that the expected dimensionality is returned
+        assert ysim.ndim == 1
+        assert ratesim.ndim == 1
+        # check that the rates and spikes has the same shape
+        assert ratesim.shape[0] == ysim.shape[0]
+        # check the time point number is that expected (same as the input)
+        assert ysim.shape[0] == X.shape[0]
 
+    @pytest.mark.parametrize(
+        "insert, expectation",
+        [
+            (0, does_not_raise()),
+            (np.nan, pytest.warns(UserWarning, match=r"The provided trees contain")),
+            (np.inf, pytest.warns(UserWarning, match=r"The provided trees contain")),
+        ],
+    )
+    def test_simulate_invalid_feedforward(
+        self, insert, expectation, poissonGLM_model_instantiation
+    ):
+        X, y, model, params, rate = poissonGLM_model_instantiation
+        model.coef_ = params[0]
+        model.intercept_ = params[1]
+        X[0] = insert
+        with expectation:
+            model.simulate(jax.random.key(123), X)
+
+    #######################################
+    # Compare with standard implementation
+    #######################################
+    def test_deviance_against_statsmodels(self, poissonGLM_model_instantiation):
+        """
+        Compare fitted parameters to statsmodels.
+        Assesses if the model estimates are close to statsmodels' results.
+        """
+        X, y, model, true_params, firing_rate = poissonGLM_model_instantiation
+        # set model coeff
+        model.coef_ = true_params[0]
+        model.intercept_ = true_params[1]
+        # get the rate
+        dev = sm.families.Poisson().deviance(y, firing_rate)
+        dev_model = model.observation_model.deviance(firing_rate, y).sum()
+        if not np.allclose(dev, dev_model):
+            raise ValueError("Deviance doesn't match statsmodels!")
+
+    def test_compatibility_with_sklearn_cv(self, poissonGLM_model_instantiation):
+        X, y, model, true_params, firing_rate = poissonGLM_model_instantiation
+        param_grid = {"regularizer__solver_name": ["BFGS", "GradientDescent"]}
+        GridSearchCV(model, param_grid).fit(X, y)
 
-class TestCyclicBSplineBasis(BasisFuncsTesting):
-    cls = basis.CyclicBSplineBasis
 
-    @pytest.mark.parametrize("samples", [[], [0], [0, 0]])
-    def test_non_empty_samples(self, samples):
-        if len(samples) == 0:
-            with pytest.raises(
-                ValueError, match="All sample provided must be non empty"
-            ):
-                self.cls(5).evaluate(samples)
-        else:
-            self.cls(5).evaluate(samples)
+class TestPopulationGLM:
+    """
+    Unit tests for the PoissonGLM class.
+    """
 
+    #######################
+    # Test model.__init__
+    #######################
     @pytest.mark.parametrize(
-        "arraylike", [0, [0], (0,), np.array([0]), jax.numpy.array([0])]
+        "regularizer, expectation",
+        [
+            (nmo.regularizer.Ridge("BFGS"), does_not_raise()),
+            (
+                None,
+                pytest.raises(
+                    AttributeError, match="The provided `solver` doesn't implement "
+                ),
+            ),
+            (
+                nmo.regularizer.Ridge,
+                pytest.raises(
+                    TypeError, match="The provided `solver` cannot be instantiated"
+                ),
+            ),
+        ],
     )
-    def test_input_to_evaluate_is_arraylike(self, arraylike):
+    def test_solver_type(self, regularizer, expectation, population_glm_class):
         """
-        Checks that the sample size of the output from the evaluate() method matches the input sample size.
+        Test that an error is raised if a non-compatible solver is passed.
         """
-        basis_obj = self.cls(n_basis_funcs=5)
-        raise_exception = not isinstance(
-            arraylike, (tuple, list, np.ndarray, jax.numpy.ndarray)
-        )
-        if raise_exception:
-            with pytest.raises(TypeError, match="Input samples must be array-like"):
-                basis_obj.evaluate(arraylike)
-        else:
-            basis_obj.evaluate(arraylike)
+        with expectation:
+            population_glm_class(regularizer=regularizer)
 
-    @pytest.mark.parametrize("n_basis_funcs", [8, 10])
-    @pytest.mark.parametrize("order", range(2, 6))
-    def test_evaluate_returns_expected_number_of_basis(
-        self, n_basis_funcs: int, order: int
+    @pytest.mark.parametrize(
+        "observation, expectation",
+        [
+            (nmo.observation_models.PoissonObservations(), does_not_raise()),
+            (
+                nmo.regularizer.Regularizer,
+                pytest.raises(
+                    AttributeError,
+                    match="The provided object does not have the required",
+                ),
+            ),
+            (
+                1,
+                pytest.raises(
+                    AttributeError,
+                    match="The provided object does not have the required",
+                ),
+            ),
+        ],
+    )
+    def test_init_observation_type(
+        self, observation, expectation, population_glm_class, ridge_regularizer
     ):
         """
-        Verifies that the evaluate() method returns the expected number of basis functions.
+        Test initialization with different regularizer names. Check if an appropriate exception is raised
+        when the regularizer name is not present in jaxopt.
         """
-        basis_obj = self.cls(n_basis_funcs=n_basis_funcs, order=order)
-        eval_basis = basis_obj.evaluate(np.linspace(0, 1, 100))
-        if eval_basis.shape[1] != n_basis_funcs:
-            raise ValueError(
-                "Dimensions do not agree: The number of basis should match the first dimension of the evaluated basis."
-                f"The number of basis is {n_basis_funcs}",
-                f"The first dimension of the evaluated basis is {eval_basis.shape[0]}",
-            )
-        return
+        with expectation:
+            population_glm_class(regularizer=ridge_regularizer, observation_model=observation)
 
-    @pytest.mark.parametrize("sample_size", [100, 1000])
-    @pytest.mark.parametrize("n_basis_funcs", [8, 10, 100])
-    @pytest.mark.parametrize("order", [2, 3])
-    def test_sample_size_of_evaluate_matches_that_of_input(
-        self, n_basis_funcs, sample_size, order
+    @pytest.mark.parametrize(
+        "X, y",
+        [
+            (jnp.zeros((2, 4)), jnp.zeros((2, 2))),
+            (jnp.zeros((2, 4)), jnp.zeros((2, 3))),
+        ],
+    )
+    def test_parameter_initialization(self, X, y, poisson_population_GLM_model):
+        _, _, model, _, _ = poisson_population_GLM_model
+        coef, inter = model._initialize_parameters(X, y)
+        assert coef.shape == (X.shape[1], y.shape[1])
+        assert inter.shape == (y.shape[1],)
+
+    #######################
+    # Test model.fit
+    #######################
+    @pytest.mark.parametrize(
+        "n_params, expectation",
+        [
+            (0, pytest.raises(ValueError, match="Params must have length two.")),
+            (1, pytest.raises(ValueError, match="Params must have length two.")),
+            (2, does_not_raise()),
+            (3, pytest.raises(ValueError, match="Params must have length two.")),
+        ],
+    )
+    def test_fit_param_length(
+        self, n_params, expectation, poisson_population_GLM_model
     ):
         """
-        Checks that the sample size of the output from the evaluate() method matches the input sample size.
+        Test the `fit` method with different numbers of initial parameters.
+        Check for correct number of parameters.
         """
-        basis_obj = self.cls(n_basis_funcs=n_basis_funcs, order=order)
-        eval_basis = basis_obj.evaluate(np.linspace(0, 1, sample_size))
-        if eval_basis.shape[0] != sample_size:
-            raise ValueError(
-                f"Dimensions do not agree: The window size should match the second dimension of the evaluated basis."
-                f"The window size is {sample_size}",
-                f"The second dimension of the evaluated basis is {eval_basis.shape[1]}",
-            )
-
-    @pytest.mark.parametrize("n_basis_funcs", [-1, 0, 1, 3, 10, 20])
-    @pytest.mark.parametrize("order", [2, 3, 4, 5])
-    def test_minimum_number_of_basis_required_is_matched(self, n_basis_funcs, order):
-        """
-        Verifies that the minimum number of basis functions and order required (i.e., at least 1) and
-        order < #basis are enforced.
-        """
-        raise_exception = order > n_basis_funcs
-        if raise_exception:
-            with pytest.raises(
-                ValueError,
-                match=rf"{self.cls.__name__} `order` parameter cannot be larger than",
-            ):
-                basis_obj = self.cls(n_basis_funcs=n_basis_funcs, order=order)
-                basis_obj.evaluate(np.linspace(0, 1, 10))
+        X, y, model, true_params, firing_rate = poisson_population_GLM_model
+        if n_params == 0:
+            init_params = tuple()
+        elif n_params == 1:
+            init_params = (true_params[0],)
         else:
-            basis_obj = self.cls(n_basis_funcs=n_basis_funcs, order=order)
-            basis_obj.evaluate(np.linspace(0, 1, 10))
-
-    @pytest.mark.parametrize("n_basis_funcs", [10])
-    @pytest.mark.parametrize("order", [-1, 0, 2, 3])
-    def test_order_is_positive(self, n_basis_funcs, order):
-        """
-        Verifies that the minimum number of basis functions and order required (i.e., at least 1) and
-        order < #basis are enforced.
-        """
-        raise_exception = order < 1
-        if raise_exception:
-            with pytest.raises(ValueError, match=r"Spline order must be positive!"):
-                basis_obj = self.cls(n_basis_funcs=n_basis_funcs, order=order)
-                basis_obj.evaluate(np.linspace(0, 1, 10))
-        else:
-            basis_obj = self.cls(n_basis_funcs=n_basis_funcs, order=order)
-            basis_obj.evaluate(np.linspace(0, 1, 10))
-
-    @pytest.mark.parametrize("n_basis_funcs", [10])
-    @pytest.mark.parametrize("order", [1, 2, 3])
-    def test_order_1_invalid(self, n_basis_funcs, order):
-        """
-        Verifies that the minimum number of basis functions and order required (i.e., at least 1) and
-        order < #basis are enforced.
-        """
-        raise_exception = order == 1
-        if raise_exception:
-            with pytest.raises(
-                ValueError, match=r"Order >= 2 required for cyclic B-spline"
-            ):
-                basis_obj = self.cls(n_basis_funcs=n_basis_funcs, order=order)
-                basis_obj.evaluate(np.linspace(0, 1, 10))
-        else:
-            basis_obj = self.cls(n_basis_funcs=n_basis_funcs, order=order)
-            basis_obj.evaluate(np.linspace(0, 1, 10))
+            init_params = true_params + (true_params[0],) * (n_params - 2)
+        with expectation:
+            model.fit(X, y, init_params=init_params)
 
     @pytest.mark.parametrize(
-        "sample_range", [(0, 1), (0.1, 0.9), (-0.5, 1), (0, 1.5), (-0.5, 1.5)]
+        "add_entry, add_to, expectation",
+        [
+            (0, "X", does_not_raise()),
+            (
+                np.nan,
+                "X",
+                pytest.warns(UserWarning, match="The provided trees contain"),
+            ),
+            (
+                np.inf,
+                "X",
+                pytest.warns(UserWarning, match="The provided trees contain"),
+            ),
+            (0, "y", does_not_raise()),
+            (
+                np.nan,
+                "y",
+                pytest.warns(UserWarning, match="The provided trees contain"),
+            ),
+            (
+                np.inf,
+                "y",
+                pytest.warns(UserWarning, match="The provided trees contain"),
+            ),
+        ],
     )
-    def test_samples_range_matches_evaluate_requirements(self, sample_range: tuple):
+    def test_fit_param_values(
+        self, add_entry, add_to, expectation, poisson_population_GLM_model
+    ):
         """
-        Verifies that the evaluate() method can handle input range.
+        Test the `fit` method with altered X or y values. Ensure the method raises exceptions for NaN or Inf values.
         """
-        basis_obj = self.cls(n_basis_funcs=5, order=3)
-        basis_obj.evaluate(np.linspace(*sample_range, 100))
+        X, y, model, true_params, firing_rate = poisson_population_GLM_model
+        if add_to == "X":
+            # get an index to be edited
+            idx = np.unravel_index(np.random.choice(X.size), X.shape)
+            X[idx] = add_entry
+        elif add_to == "y":
+            idx = np.unravel_index(np.random.choice(y.size), y.shape)
+            y = np.asarray(y, dtype=np.float32)
+            y[idx] = add_entry
+        with expectation:
+            model.fit(X, y, init_params=true_params)
 
-    @pytest.mark.parametrize("n_input", [0, 1, 2, 3])
-    def test_number_of_required_inputs_evaluate(self, n_input):
+    @pytest.mark.parametrize(
+        "dim_weights, expectation",
+        [
+            (
+                0,
+                pytest.raises(
+                    ValueError,
+                    match=r"params\[0\] must be an array or .* of shape \(n_features",
+                ),
+            ),
+            (
+                1,
+                pytest.raises(
+                    ValueError,
+                    match=r"params\[0\] must be an array or .* of shape \(n_features",
+                ),
+            ),
+            (
+                2,
+                does_not_raise(),
+            ),
+            (
+                3,
+                pytest.raises(
+                    ValueError,
+                    match=r"params\[0\] must be an array or .* of shape \(n_features",
+                ),
+            ),
+        ],
+    )
+    def test_fit_weights_dimensionality(
+        self, dim_weights, expectation, poisson_population_GLM_model
+    ):
         """
-        Confirms that the evaluate() method correctly handles the number of input samples that are provided.
+        Test the `fit` method with weight matrices of different dimensionalities.
+        Check for correct dimensionality.
         """
-        basis_obj = self.cls(n_basis_funcs=5, order=3)
-        raise_exception = n_input != basis_obj._n_input_dimensionality
-        inputs = [np.linspace(0, 1, 20)] * n_input
-        if raise_exception:
-            with pytest.raises(
-                ValueError,
-                match="Input dimensionality mismatch. This basis evaluation requires [0-9]+ inputs",
-            ):
-                basis_obj.evaluate(*inputs)
+        X, y, model, true_params, firing_rate = poisson_population_GLM_model
+        n_samples, n_features = X.shape
+        n_neurons = 3
+        if dim_weights == 0:
+            init_w = jnp.array([])
+        elif dim_weights == 1:
+            init_w = jnp.zeros((n_features,))
+        elif dim_weights == 2:
+            init_w = jnp.zeros((n_features, n_neurons))
         else:
-            basis_obj.evaluate(*inputs)
+            init_w = jnp.zeros((n_features, n_neurons) + (1,) * (dim_weights - 2))
+        with expectation:
+            model.fit(X, y, init_params=(init_w, true_params[1]))
 
-    @pytest.mark.parametrize("sample_size", [-1, 0, 1, 10, 11, 100])
-    def test_evaluate_on_grid_meshgrid_size(self, sample_size):
+    @pytest.mark.parametrize(
+        "dim_intercepts, expectation",
+        [
+            (0, pytest.raises(ValueError, match=r"params\[1\] must be of shape")),
+            (1, does_not_raise()),
+            (2, pytest.raises(ValueError, match=r"params\[1\] must be of shape")),
+            (3, pytest.raises(ValueError, match=r"params\[1\] must be of shape")),
+        ],
+    )
+    def test_fit_intercepts_dimensionality(
+        self, dim_intercepts, expectation, poisson_population_GLM_model
+    ):
         """
-        Checks that the evaluate_on_grid() method returns a grid of the expected size.
+        Test the `fit` method with intercepts of different dimensionalities. Check for correct dimensionality.
         """
-        basis_obj = self.cls(n_basis_funcs=5, order=3)
-        raise_exception = sample_size <= 0
-        if raise_exception:
-            with pytest.raises(
-                ValueError,
-                match=r"Empty sample array provided\. At least one sample is required|"
-                "All sample counts provided must be greater",
-            ):
-                basis_obj.evaluate_on_grid(sample_size)
-        else:
-            grid, _ = basis_obj.evaluate_on_grid(sample_size)
-            assert grid.shape[0] == sample_size
+        X, y, model, true_params, firing_rate = poisson_population_GLM_model
+        n_samples, n_features = X.shape
+        init_b = jnp.zeros((y.shape[1],) * dim_intercepts)
+        init_w = jnp.zeros((n_features, y.shape[1]))
+        with expectation:
+            model.fit(X, y, init_params=(init_w, init_b))
 
-    @pytest.mark.parametrize("sample_size", [-1, 0, 1, 10, 11, 100])
-    def test_evaluate_on_grid_basis_size(self, sample_size):
+    @pytest.mark.parametrize(
+        "init_params, expectation",
+        [
+            ([jnp.zeros((5, 3)), jnp.zeros((3,))], does_not_raise()),
+            (
+                [[jnp.zeros((1, 5)), jnp.zeros((3,))]],
+                pytest.raises(ValueError, match="Params must have length two."),
+            ),
+            (dict(p1=jnp.zeros((3, 3)), p2=jnp.zeros((3, 2))), pytest.raises(KeyError)),
+            (
+                (dict(p1=jnp.zeros((3, 3)), p2=jnp.zeros((2, 3))), jnp.zeros((3,))),
+                pytest.raises(
+                    TypeError, match=r"X and params\[0\] must be the same type"
+                ),
+            ),
+            (0, pytest.raises(ValueError, match="Params must have length two.")),
+            (
+                {0, 1},
+                pytest.raises(TypeError, match="Initial parameters must be array-like"),
+            ),
+            (
+                [jnp.zeros((1, 5)), ""],
+                pytest.raises(TypeError, match="Initial parameters must be array-like"),
+            ),
+            (
+                ["", jnp.zeros((1,))],
+                pytest.raises(TypeError, match="Initial parameters must be array-like"),
+            ),
+        ],
+    )
+    def test_fit_init_params_type(
+        self, init_params, expectation, poisson_population_GLM_model
+    ):
         """
-        Ensures that the evaluate_on_grid() method returns basis functions of the expected size.
+        Test the `fit` method with various types of initial parameters. Ensure that the provided initial parameters
+        are array-like.
         """
-        basis_obj = self.cls(n_basis_funcs=5, order=3)
-        raise_exception = sample_size <= 0
-        if raise_exception:
-            with pytest.raises(
-                ValueError,
-                match="All sample counts provided must be greater|"
-                r"Empty sample array provided\. At least one sample is required for",
-            ):
-                basis_obj.evaluate_on_grid(sample_size)
-        else:
-            _, eval_basis = basis_obj.evaluate_on_grid(sample_size)
-            assert eval_basis.shape[0] == sample_size
+        X, y, model, true_params, firing_rate = poisson_population_GLM_model
+        with expectation:
+            model.fit(X, y, init_params=init_params)
 
-    @pytest.mark.parametrize("n_input", [0, 1, 2])
-    def test_evaluate_on_grid_input_number(self, n_input):
+    @pytest.mark.parametrize(
+        "delta_dim, expectation",
+        [
+            (-1, pytest.raises(ValueError, match="X must be two-dimensional")),
+            (0, does_not_raise()),
+            (1, pytest.raises(ValueError, match="X must be two-dimensional")),
+        ],
+    )
+    def test_fit_x_dimensionality(
+        self, delta_dim, expectation, poisson_population_GLM_model
+    ):
         """
-        Validates that the evaluate_on_grid() method correctly handles the number of input samples that are provided.
+        Test the `fit` method with X input data of different dimensionalities. Ensure correct dimensionality for X.
         """
-        basis_obj = self.cls(n_basis_funcs=5, order=3)
-        inputs = [10] * n_input
-        raise_exception = n_input != basis_obj._n_input_dimensionality
-        if raise_exception:
-            with pytest.raises(
-                ValueError,
-                match=r"Input dimensionality mismatch\. This basis evaluation requires [0-9]+ inputs",
-            ):
-                basis_obj.evaluate_on_grid(*inputs)
-        else:
-            basis_obj.evaluate_on_grid(*inputs)
-
-
-class CombinedBasis(BasisFuncsTesting):
-    """
-    This class is used to run tests on combination operations (e.g., addition, multiplication) among Basis functions.
-
-    Properties:
-    - cls: Class (default = None)
-    """
-
-    cls = None
-
-    @staticmethod
-    def instantiate_basis(n_basis, basis_class):
-        """Instantiate and return two basis of the type specified."""
-        if basis_class == basis.MSplineBasis:
-            basis_obj = basis_class(n_basis_funcs=n_basis, order=4)
-        elif basis_class in [basis.RaisedCosineBasisLinear, basis.RaisedCosineBasisLog]:
-            basis_obj = basis_class(n_basis_funcs=n_basis)
-        elif basis_class == basis.OrthExponentialBasis:
-            basis_obj = basis_class(
-                n_basis_funcs=n_basis, decay_rates=np.arange(1, 1 + n_basis)
-            )
-        elif basis_class == basis.BSplineBasis:
-            basis_obj = basis_class(n_basis_funcs=n_basis, order=3)
-        elif basis_class == basis.CyclicBSplineBasis:
-            basis_obj = basis_class(n_basis_funcs=n_basis, order=3)
-        elif basis_class == basis.AdditiveBasis:
-            b1 = basis.MSplineBasis(n_basis_funcs=n_basis, order=2)
-            b2 = basis.RaisedCosineBasisLinear(n_basis_funcs=n_basis + 1)
-            basis_obj = b1 + b2
-        elif basis_class == basis.MultiplicativeBasis:
-            b1 = basis.MSplineBasis(n_basis_funcs=n_basis, order=2)
-            b2 = basis.RaisedCosineBasisLinear(n_basis_funcs=n_basis + 1)
-            basis_obj = b1 * b2
-        else:
-            raise ValueError(
-                f"Test for basis addition not implemented for basis of type {basis_class}!"
-            )
-        return basis_obj
-
-
-class TestAdditiveBasis(CombinedBasis):
-    cls = basis.AdditiveBasis
+        X, y, model, true_params, firing_rate = poisson_population_GLM_model
+        if delta_dim == -1:
+            X = np.zeros((X.shape[0],))
+        elif delta_dim == 1:
+            X = np.zeros((X.shape[0], 1, X.shape[1]))
+        with expectation:
+            model.fit(X, y, init_params=true_params)
 
     @pytest.mark.parametrize(
-        "samples", [[[0], []], [[], [0]], [[0], [0]], [[0, 0], [0, 0]]]
+        "delta_dim, expectation",
+        [
+            (-1, pytest.raises(ValueError, match="y must be two-dimensional")),
+            (0, does_not_raise()),
+            (1, pytest.raises(ValueError, match="y must be two-dimensional")),
+        ],
     )
-    def test_non_empty_samples(self, samples):
-        basis_obj = basis.MSplineBasis(5) + basis.MSplineBasis(5)
-        if any(tuple(len(s) == 0 for s in samples)):
-            with pytest.raises(
-                ValueError, match="All sample provided must be non empty"
-            ):
-                basis_obj.evaluate(*samples)
-        else:
-            basis_obj.evaluate(*samples)
+    def test_fit_y_dimensionality(
+        self, delta_dim, expectation, poisson_population_GLM_model
+    ):
+        """
+        Test the `fit` method with y target data of different dimensionalities. Ensure correct dimensionality for y.
+        """
+        X, y, model, true_params, firing_rate = poisson_population_GLM_model
+        if delta_dim == -1:
+            y = y[:, 0]
+        elif delta_dim == 1:
+            y = np.zeros((*y.shape, 1))
+        with expectation:
+            model.fit(X, y, init_params=true_params)
 
     @pytest.mark.parametrize(
-        "arraylike",
+        "delta_n_features, expectation",
         [
-            [0, 0],
-            [[0], [0]],
-            [(0,), (0,)],
-            [np.array([0]), [0]],
-            [jax.numpy.array([0]), [0]],
+            (-1, pytest.raises(ValueError, match="Inconsistent number of features")),
+            (0, does_not_raise()),
+            (1, pytest.raises(ValueError, match="Inconsistent number of features")),
         ],
     )
-    def test_input_to_evaluate_is_arraylike(self, arraylike):
+    def test_fit_n_feature_consistency_weights(
+        self, delta_n_features, expectation, poisson_population_GLM_model
+    ):
         """
-        Checks that the sample size of the output from the evaluate() method matches the input sample size.
+        Test the `fit` method for inconsistencies between data features and initial weights provided.
+        Ensure the number of features align.
         """
-        basis_obj = basis.MSplineBasis(5) + basis.MSplineBasis(5)
-        raise_exception = not all(
-            isinstance(a, (tuple, list, np.ndarray, jax.numpy.ndarray))
-            for a in arraylike
+        X, y, model, true_params, firing_rate = poisson_population_GLM_model
+        init_w = jnp.zeros((X.shape[1] + delta_n_features, y.shape[1]))
+        init_b = jnp.zeros(
+            y.shape[1],
         )
-        if raise_exception:
-            with pytest.raises(TypeError, match="Input samples must be array-like"):
-                basis_obj.evaluate(*arraylike)
-        else:
-            basis_obj.evaluate(*arraylike)
+        with expectation:
+            model.fit(X, y, init_params=(init_w, init_b))
 
-    @pytest.mark.parametrize("n_basis_a", [5, 6])
-    @pytest.mark.parametrize("n_basis_b", [5, 6])
-    @pytest.mark.parametrize("sample_size", [10, 1000])
     @pytest.mark.parametrize(
-        "basis_a",
-        [class_obj for _, class_obj in utils_testing.get_non_abstract_classes(basis)],
-    )
-    @pytest.mark.parametrize(
-        "basis_b",
-        [class_obj for _, class_obj in utils_testing.get_non_abstract_classes(basis)],
+        "delta_n_features, expectation",
+        [
+            (-1, pytest.raises(ValueError, match="Inconsistent number of features")),
+            (0, does_not_raise()),
+            (1, pytest.raises(ValueError, match="Inconsistent number of features")),
+        ],
     )
-    def test_evaluate_returns_expected_number_of_basis(
-        self, n_basis_a, n_basis_b, sample_size, basis_a, basis_b
+    def test_fit_n_feature_consistency_x(
+        self, delta_n_features, expectation, poisson_population_GLM_model
     ):
         """
-        Test whether the evaluation of the `AdditiveBasis` results in a number of basis
-        that is the sum of the number of basis functions from two individual bases.
+        Test the `fit` method for inconsistencies between data features and model's expectations.
+        Ensure the number of features in X aligns.
         """
-        # define the two basis
-        basis_a_obj = self.instantiate_basis(n_basis_a, basis_a)
-        basis_b_obj = self.instantiate_basis(n_basis_b, basis_b)
+        X, y, model, true_params, firing_rate = poisson_population_GLM_model
+        if delta_n_features == 1:
+            X = jnp.concatenate((X, jnp.zeros((X.shape[0], 1))), axis=1)
+        elif delta_n_features == -1:
+            X = X[..., :-1]
+        with expectation:
+            model.fit(X, y, init_params=true_params)
 
-        basis_obj = basis_a_obj + basis_b_obj
-        eval_basis = basis_obj.evaluate(
-            *[np.linspace(0, 1, sample_size)] * basis_obj._n_input_dimensionality
-        )
-        if eval_basis.shape[1] != basis_a_obj.n_basis_funcs + basis_b_obj.n_basis_funcs:
-            raise ValueError(
-                "Dimensions do not agree: The number of basis should match the first dimension of the evaluated basis."
-                f"The number of basis is {n_basis_a + n_basis_b}",
-                f"The first dimension of the evaluated basis is {eval_basis.shape[1]}",
-            )
-
-    @pytest.mark.parametrize("sample_size", [100, 1000])
-    @pytest.mark.parametrize("n_basis_a", [5, 6])
-    @pytest.mark.parametrize("n_basis_b", [5, 6])
-    @pytest.mark.parametrize(
-        "basis_a",
-        [class_obj for _, class_obj in utils_testing.get_non_abstract_classes(basis)],
-    )
     @pytest.mark.parametrize(
-        "basis_b",
-        [class_obj for _, class_obj in utils_testing.get_non_abstract_classes(basis)],
+        "delta_tp, expectation",
+        [
+            (
+                -1,
+                pytest.raises(ValueError, match="The number of time-points in X and y"),
+            ),
+            (0, does_not_raise()),
+            (
+                1,
+                pytest.raises(ValueError, match="The number of time-points in X and y"),
+            ),
+        ],
     )
-    def test_sample_size_of_evaluate_matches_that_of_input(
-        self, n_basis_a, n_basis_b, sample_size, basis_a, basis_b
+    def test_fit_time_points_x(
+        self, delta_tp, expectation, poisson_population_GLM_model
     ):
         """
-        Test whether the output sample size from the `AdditiveBasis` evaluate function matches the input sample size.
+        Test the `fit` method for inconsistencies in time-points in data X. Ensure the correct number of time-points.
         """
-        basis_a_obj = self.instantiate_basis(n_basis_a, basis_a)
-        basis_b_obj = self.instantiate_basis(n_basis_b, basis_b)
-        basis_obj = basis_a_obj + basis_b_obj
-        eval_basis = basis_obj.evaluate(
-            *[np.linspace(0, 1, sample_size)] * basis_obj._n_input_dimensionality
-        )
-        if eval_basis.shape[0] != sample_size:
-            raise ValueError(
-                f"Dimensions do not agree: The window size should match the second dimension of the evaluated basis."
-                f"The window size is {sample_size}",
-                f"The second dimension of the evaluated basis is {eval_basis.shape[0]}",
-            )
+        X, y, model, true_params, firing_rate = poisson_population_GLM_model
+        X = jnp.zeros((X.shape[0] + delta_tp,) + X.shape[1:])
+        with expectation:
+            model.fit(X, y, init_params=true_params)
 
     @pytest.mark.parametrize(
-        "basis_a",
-        [class_obj for _, class_obj in utils_testing.get_non_abstract_classes(basis)],
-    )
-    @pytest.mark.parametrize(
-        "basis_b",
-        [class_obj for _, class_obj in utils_testing.get_non_abstract_classes(basis)],
+        "delta_tp, expectation",
+        [
+            (
+                -1,
+                pytest.raises(ValueError, match="The number of time-points in X and y"),
+            ),
+            (0, does_not_raise()),
+            (
+                1,
+                pytest.raises(ValueError, match="The number of time-points in X and y"),
+            ),
+        ],
     )
-    @pytest.mark.parametrize("n_input", [0, 1, 2, 3, 10, 30])
-    @pytest.mark.parametrize("n_basis_a", [5, 6])
-    @pytest.mark.parametrize("n_basis_b", [5, 6])
-    def test_number_of_required_inputs_evaluate(
-        self, n_input, n_basis_a, n_basis_b, basis_a, basis_b
+    def test_fit_time_points_y(
+        self, delta_tp, expectation, poisson_population_GLM_model
     ):
         """
-        Test whether the number of required inputs for the `evaluate` function matches
-        the sum of the number of input samples from the two bases.
+        Test the `fit` method for inconsistencies in time-points in y. Ensure the correct number of time-points.
         """
-        basis_a_obj = self.instantiate_basis(n_basis_a, basis_a)
-        basis_b_obj = self.instantiate_basis(n_basis_b, basis_b)
-        basis_obj = basis_a_obj + basis_b_obj
-        raise_exception = (
-            n_input
-            != basis_a_obj._n_input_dimensionality + basis_b_obj._n_input_dimensionality
+        X, y, model, true_params, firing_rate = poisson_population_GLM_model
+        y = jnp.zeros((y.shape[0] + delta_tp,) + y.shape[1:])
+        with expectation:
+            model.fit(X, y, init_params=true_params)
+
+    def test_fit_mask_grouplasso(self, group_sparse_poisson_glm_model_instantiation):
+        """Test that the group lasso fit goes through"""
+        X, y, model, params, rate, mask = group_sparse_poisson_glm_model_instantiation
+        model.set_params(
+            regularizer=nmo.regularizer.GroupLasso(
+                solver_name="ProximalGradient", mask=mask
+            )
         )
-        inputs = [np.linspace(0, 1, 20)] * n_input
-        if raise_exception:
-            with pytest.raises(
-                ValueError,
-                match="Input dimensionality mismatch. This basis evaluation requires [0-9]+ inputs,",
-            ):
-                basis_obj.evaluate(*inputs)
-        else:
-            basis_obj.evaluate(*inputs)
+        model.fit(X, y)
+
+    def test_fit_pytree_equivalence(
+        self, poisson_population_GLM_model, poisson_population_GLM_model_pytree
+    ):
+        """Check that the glm fit with pytree learns the same parameters."""
+        # required for numerical precision of coeffs
+        jax.config.update("jax_enable_x64", True)
+        X, y, model, true_params, firing_rate = poisson_population_GLM_model
+        X_tree, _, model_tree, true_params_tree, _ = (
+            poisson_population_GLM_model_pytree
+        )
+        # fit both models
+        model.fit(X, y, init_params=true_params)
+        model_tree.fit(X_tree, y, init_params=true_params_tree)
+
+        # get the flat parameters
+        flat_coef = np.concatenate(
+            jax.tree_util.tree_flatten(model_tree.coef_)[0], axis=0
+        )
+
+        # assert equivalence of solutions
+        assert np.allclose(model.coef_, flat_coef)
+        assert np.allclose(model.intercept_, model_tree.intercept_)
+        assert np.allclose(model.score(X, y), model_tree.score(X_tree, y))
+        assert np.allclose(model.predict(X), model_tree.predict(X_tree))
 
-    @pytest.mark.parametrize("sample_size", [11, 20])
     @pytest.mark.parametrize(
-        "basis_a",
-        [class_obj for _, class_obj in utils_testing.get_non_abstract_classes(basis)],
+        "fill_val, expectation",
+        [
+            (0, does_not_raise()),
+            (
+                jnp.inf,
+                pytest.raises(
+                    ValueError, match="At least a NaN or an Inf at all sample points"
+                ),
+            ),
+            (
+                jnp.nan,
+                pytest.raises(
+                    ValueError, match="At least a NaN or an Inf at all sample points"
+                ),
+            ),
+        ],
     )
+    def test_fit_all_invalid_X(
+        self, fill_val, expectation, poisson_population_GLM_model
+    ):
+        X, y, model, true_params, firing_rate = poisson_population_GLM_model
+        X.fill(fill_val)
+        with expectation:
+            model.fit(X, y)
+
+    #######################
+    # Test model.score
+    #######################
     @pytest.mark.parametrize(
-        "basis_b",
-        [class_obj for _, class_obj in utils_testing.get_non_abstract_classes(basis)],
+        "delta_dim, expectation",
+        [
+            (-1, pytest.raises(ValueError, match="X must be two-dimensional")),
+            (0, does_not_raise()),
+            (1, pytest.raises(ValueError, match="X must be two-dimensional")),
+        ],
     )
-    @pytest.mark.parametrize("n_basis_a", [5])
-    @pytest.mark.parametrize("n_basis_b", [6])
-    def test_evaluate_on_grid_meshgrid_size(
-        self, sample_size, n_basis_a, n_basis_b, basis_a, basis_b
+    def test_score_x_dimensionality(
+        self, delta_dim, expectation, poisson_population_GLM_model
     ):
         """
-        Test whether the resulting meshgrid size matches the sample size input.
+        Test the `score` method with X input data of different dimensionalities. Ensure correct dimensionality for X.
         """
-        basis_a_obj = self.instantiate_basis(n_basis_a, basis_a)
-        basis_b_obj = self.instantiate_basis(n_basis_b, basis_b)
-        basis_obj = basis_a_obj + basis_b_obj
-        res = basis_obj.evaluate_on_grid(
-            *[sample_size] * basis_obj._n_input_dimensionality
-        )
-        for grid in res[:-1]:
-            assert grid.shape[0] == sample_size
+        X, y, model, true_params, firing_rate = poisson_population_GLM_model
+        model.coef_ = true_params[0]
+        model.intercept_ = true_params[1]
+        if delta_dim == -1:
+            X = np.zeros((X.shape[0],))
+        elif delta_dim == 1:
+            X = np.zeros((X.shape[0], X.shape[1], 1))
+        with expectation:
+            model.score(X, y)
 
-    @pytest.mark.parametrize("sample_size", [11, 20])
-    @pytest.mark.parametrize(
-        "basis_a",
-        [class_obj for _, class_obj in utils_testing.get_non_abstract_classes(basis)],
-    )
     @pytest.mark.parametrize(
-        "basis_b",
-        [class_obj for _, class_obj in utils_testing.get_non_abstract_classes(basis)],
+        "delta_dim, expectation",
+        [
+            (
+                -1,
+                pytest.raises(
+                    ValueError, match="y must be two-dimensional, with shape"
+                ),
+            ),
+            (0, does_not_raise()),
+            (
+                1,
+                pytest.raises(
+                    ValueError, match="y must be two-dimensional, with shape"
+                ),
+            ),
+        ],
     )
-    @pytest.mark.parametrize("n_basis_a", [5])
-    @pytest.mark.parametrize("n_basis_b", [6])
-    def test_evaluate_on_grid_basis_size(
-        self, sample_size, n_basis_a, n_basis_b, basis_a, basis_b
+    def test_score_y_dimensionality(
+        self, delta_dim, expectation, poisson_population_GLM_model
     ):
         """
-        Test whether the number sample size output by evaluate_on_grid matches the sample size of the input.
+        Test the `score` method with y of different dimensionalities.
+        Ensure correct dimensionality for y.
         """
-        basis_a_obj = self.instantiate_basis(n_basis_a, basis_a)
-        basis_b_obj = self.instantiate_basis(n_basis_b, basis_b)
-        basis_obj = basis_a_obj + basis_b_obj
-        eval_basis = basis_obj.evaluate_on_grid(
-            *[sample_size] * basis_obj._n_input_dimensionality
-        )[-1]
-        assert eval_basis.shape[0] == sample_size
+        X, y, model, true_params, firing_rate = poisson_population_GLM_model
+        model.coef_ = true_params[0]
+        model.intercept_ = true_params[1]
+        if delta_dim == -1:
+            y = y[:, 0]
+        elif delta_dim == 1:
+            y = np.zeros((*y.shape, 1))
+        with expectation:
+            model.score(X, y)
 
-    @pytest.mark.parametrize("n_input", [0, 1, 2, 5, 6, 11, 30])
-    @pytest.mark.parametrize(
-        "basis_a",
-        [class_obj for _, class_obj in utils_testing.get_non_abstract_classes(basis)],
-    )
     @pytest.mark.parametrize(
-        "basis_b",
-        [class_obj for _, class_obj in utils_testing.get_non_abstract_classes(basis)],
+        "delta_n_features, expectation",
+        [
+            (-1, pytest.raises(ValueError, match="Inconsistent number of features")),
+            (0, does_not_raise()),
+            (1, pytest.raises(ValueError, match="Inconsistent number of features")),
+        ],
     )
-    @pytest.mark.parametrize("n_basis_a", [5])
-    @pytest.mark.parametrize("n_basis_b", [6])
-    def test_evaluate_on_grid_input_number(
-        self, n_input, basis_a, basis_b, n_basis_a, n_basis_b
+    def test_score_n_feature_consistency_x(
+        self, delta_n_features, expectation, poisson_population_GLM_model
     ):
         """
-        Test whether the number of inputs provided to `evaluate_on_grid` matches
-        the sum of the number of input samples required from each of the basis objects.
+        Test the `score` method for inconsistencies in features of X.
+        Ensure the number of features in X aligns with the model params.
         """
-        basis_a_obj = self.instantiate_basis(n_basis_a, basis_a)
-        basis_b_obj = self.instantiate_basis(n_basis_b, basis_b)
-        basis_obj = basis_a_obj + basis_b_obj
-        inputs = [20] * n_input
-        raise_exception = (
-            n_input
-            != basis_a_obj._n_input_dimensionality + basis_b_obj._n_input_dimensionality
-        )
-        if raise_exception:
-            with pytest.raises(
-                ValueError,
-                match=r"Input dimensionality mismatch\. This basis evaluation requires [0-9]+ inputs, "
-                r"[0-9]+ inputs provided instead.",
-            ):
-                basis_obj.evaluate_on_grid(*inputs)
-        else:
-            basis_obj.evaluate_on_grid(*inputs)
-
-
-class TestMultiplicativeBasis(CombinedBasis):
-    cls = basis.MultiplicativeBasis
+        X, y, model, true_params, firing_rate = poisson_population_GLM_model
+        model.coef_ = true_params[0]
+        model.intercept_ = true_params[1]
+        if delta_n_features == 1:
+            X = jnp.concatenate((X, jnp.zeros((X.shape[0], 1))), axis=1)
+        elif delta_n_features == -1:
+            X = X[..., :-1]
+        with expectation:
+            model.score(X, y)
 
     @pytest.mark.parametrize(
-        "samples", [[[0], []], [[], [0]], [[0], [0]], [[0, 0], [0, 0]]]
+        "is_fit, expectation",
+        [
+            (True, does_not_raise()),
+            (
+                False,
+                pytest.raises(ValueError, match="This GLM instance is not fitted yet"),
+            ),
+        ],
     )
-    def test_non_empty_samples(self, samples):
-        basis_obj = basis.MSplineBasis(5) * basis.MSplineBasis(5)
-        if any(tuple(len(s) == 0 for s in samples)):
-            with pytest.raises(
-                ValueError, match="All sample provided must be non empty"
-            ):
-                basis_obj.evaluate(*samples)
-        else:
-            basis_obj.evaluate(*samples)
+    def test_predict_is_fit(self, is_fit, expectation, poisson_population_GLM_model):
+        """
+        Test the `score` method on models based on their fit status.
+        Ensure scoring is only possible on fitted models.
+        """
+        X, y, model, true_params, firing_rate = poisson_population_GLM_model
+        if is_fit:
+            model.fit(X, y)
+        with expectation:
+            model.predict(X)
 
     @pytest.mark.parametrize(
-        "arraylike",
+        "delta_tp, expectation",
         [
-            [0, 0],
-            [[0], [0]],
-            [(0,), (0,)],
-            [np.array([0]), [0]],
-            [jax.numpy.array([0]), [0]],
+            (
+                -1,
+                pytest.raises(ValueError, match="The number of time-points in X and y"),
+            ),
+            (0, does_not_raise()),
+            (
+                1,
+                pytest.raises(ValueError, match="The number of time-points in X and y"),
+            ),
         ],
     )
-    def test_input_to_evaluate_is_arraylike(self, arraylike):
+    def test_score_time_points_x(
+        self, delta_tp, expectation, poisson_population_GLM_model
+    ):
         """
-        Checks that the sample size of the output from the evaluate() method matches the input sample size.
+        Test the `score` method for inconsistencies in time-points in X.
+        Ensure that the number of time-points in X and y matches.
         """
-        basis_obj = basis.MSplineBasis(5) * basis.MSplineBasis(5)
-        raise_exception = not all(
-            isinstance(a, (tuple, list, np.ndarray, jax.numpy.ndarray))
-            for a in arraylike
-        )
-        if raise_exception:
-            with pytest.raises(TypeError, match="Input samples must be array-like"):
-                basis_obj.evaluate(*arraylike)
-        else:
-            basis_obj.evaluate(*arraylike)
+        X, y, model, true_params, firing_rate = poisson_population_GLM_model
+        model.coef_ = true_params[0]
+        model.intercept_ = true_params[1]
+        X = jnp.zeros((X.shape[0] + delta_tp,) + X.shape[1:])
+        with expectation:
+            model.score(X, y)
 
-    @pytest.mark.parametrize("n_basis_a", [5, 6])
-    @pytest.mark.parametrize("n_basis_b", [5, 6])
-    @pytest.mark.parametrize("sample_size", [10, 1000])
     @pytest.mark.parametrize(
-        "basis_a",
-        [class_obj for _, class_obj in utils_testing.get_non_abstract_classes(basis)],
-    )
-    @pytest.mark.parametrize(
-        "basis_b",
-        [class_obj for _, class_obj in utils_testing.get_non_abstract_classes(basis)],
+        "delta_tp, expectation",
+        [
+            (
+                -1,
+                pytest.raises(ValueError, match="The number of time-points in X and y"),
+            ),
+            (0, does_not_raise()),
+            (
+                1,
+                pytest.raises(ValueError, match="The number of time-points in X and y"),
+            ),
+        ],
     )
-    def test_evaluate_returns_expected_number_of_basis(
-        self, n_basis_a, n_basis_b, sample_size, basis_a, basis_b
+    def test_score_time_points_y(
+        self, delta_tp, expectation, poisson_population_GLM_model
     ):
         """
-        Test whether the evaluation of the `MultiplicativeBasis` results in a number of basis
-        that is the product of the number of basis functions from two individual bases.
+        Test the `score` method for inconsistencies in time-points in y.
+        Ensure that the number of time-points in X and y matches.
         """
-        # define the two basis
-        basis_a_obj = self.instantiate_basis(n_basis_a, basis_a)
-        basis_b_obj = self.instantiate_basis(n_basis_b, basis_b)
+        X, y, model, true_params, firing_rate = poisson_population_GLM_model
+        model.coef_ = true_params[0]
+        model.intercept_ = true_params[1]
+        y = jnp.zeros((y.shape[0] + delta_tp,) + y.shape[1:])
+        with expectation:
+            model.score(X, y)
 
-        basis_obj = basis_a_obj * basis_b_obj
-        eval_basis = basis_obj.evaluate(
-            *[np.linspace(0, 1, sample_size)] * basis_obj._n_input_dimensionality
-        )
-        if eval_basis.shape[1] != basis_a_obj.n_basis_funcs * basis_b_obj.n_basis_funcs:
-            raise ValueError(
-                "Dimensions do not agree: The number of basis should match the first dimension of the evaluated basis."
-                f"The number of basis is {n_basis_a * n_basis_b}",
-                f"The first dimension of the evaluated basis is {eval_basis.shape[1]}",
-            )
-
-    @pytest.mark.parametrize("sample_size", [6, 30, 35])
-    @pytest.mark.parametrize("n_basis_a", [5, 6])
-    @pytest.mark.parametrize("n_basis_b", [5, 6])
-    @pytest.mark.parametrize(
-        "basis_a",
-        [class_obj for _, class_obj in utils_testing.get_non_abstract_classes(basis)],
-    )
     @pytest.mark.parametrize(
-        "basis_b",
-        [class_obj for _, class_obj in utils_testing.get_non_abstract_classes(basis)],
+        "score_type, expectation",
+        [
+            ("pseudo-r2-McFadden", does_not_raise()),
+            ("pseudo-r2-Cohen", does_not_raise()),
+            ("log-likelihood", does_not_raise()),
+            (
+                "not-implemented",
+                pytest.raises(
+                    NotImplementedError,
+                    match="Scoring method not-implemented not implemented",
+                ),
+            ),
+        ],
     )
-    def test_sample_size_of_evaluate_matches_that_of_input(
-        self, n_basis_a, n_basis_b, sample_size, basis_a, basis_b
+    def test_score_type_r2(
+        self, score_type, expectation, poisson_population_GLM_model
     ):
         """
-        Test whether the output sample size from the `MultiplicativeBasis` evaluate function matches the input sample size.
+        Test the `score` method for unsupported scoring types.
+        Ensure only valid score types are used.
         """
-        basis_a_obj = self.instantiate_basis(n_basis_a, basis_a)
-        basis_b_obj = self.instantiate_basis(n_basis_b, basis_b)
-        basis_obj = basis_a_obj * basis_b_obj
-        eval_basis = basis_obj.evaluate(
-            *[np.linspace(0, 1, sample_size)] * basis_obj._n_input_dimensionality
-        )
-        if eval_basis.shape[0] != sample_size:
+        X, y, model, true_params, firing_rate = poisson_population_GLM_model
+        model.coef_ = true_params[0]
+        model.intercept_ = true_params[1]
+        with expectation:
+            model.score(X, y, score_type=score_type)
+
+    def test_loglikelihood_against_scipy_stats(self, poisson_population_GLM_model):
+        """
+        Compare the model's log-likelihood computation against `jax.scipy`.
+        Ensure consistent and correct calculations.
+        """
+        X, y, model, true_params, firing_rate = poisson_population_GLM_model
+        # set model coeff
+        model.coef_ = true_params[0]
+        model.intercept_ = true_params[1]
+        model._initialize_feature_mask(X, y)
+        # get the rate
+        mean_firing = model.predict(X)
+        # compute the log-likelihood using jax.scipy
+        mean_ll_jax = jax.scipy.stats.poisson.logpmf(y, mean_firing).mean()
+        model_ll = model.score(X, y, score_type="log-likelihood")
+        if not np.allclose(mean_ll_jax, model_ll):
             raise ValueError(
-                f"Dimensions do not agree: The window size should match the second dimension of the evaluated basis."
-                f"The window size is {sample_size}",
-                f"The second dimension of the evaluated basis is {eval_basis.shape[0]}",
+                "Log-likelihood of PoissonModel does not match" "that of jax.scipy!"
             )
 
+    #######################
+    # Test model.predict
+    #######################
     @pytest.mark.parametrize(
-        "basis_a",
-        [class_obj for _, class_obj in utils_testing.get_non_abstract_classes(basis)],
-    )
-    @pytest.mark.parametrize(
-        "basis_b",
-        [class_obj for _, class_obj in utils_testing.get_non_abstract_classes(basis)],
+        "delta_dim, expectation",
+        [
+            (-1, pytest.raises(ValueError, match="X must be two-dimensional")),
+            (0, does_not_raise()),
+            (1, pytest.raises(ValueError, match="X must be two-dimensional")),
+        ],
     )
-    @pytest.mark.parametrize("n_input", [0, 1, 2, 3, 10, 30])
-    @pytest.mark.parametrize("n_basis_a", [5, 6])
-    @pytest.mark.parametrize("n_basis_b", [5, 6])
-    def test_number_of_required_inputs_evaluate(
-        self, n_input, n_basis_a, n_basis_b, basis_a, basis_b
+    def test_predict_x_dimensionality(
+        self, delta_dim, expectation, poisson_population_GLM_model
     ):
         """
-        Test whether the number of required inputs for the `evaluate` function matches
-        the sum of the number of input samples from the two bases.
+        Test the `predict` method with x input data of different dimensionalities.
+        Ensure correct dimensionality for x.
         """
-        basis_a_obj = self.instantiate_basis(n_basis_a, basis_a)
-        basis_b_obj = self.instantiate_basis(n_basis_b, basis_b)
-        basis_obj = basis_a_obj * basis_b_obj
-        raise_exception = (
-            n_input
-            != basis_a_obj._n_input_dimensionality + basis_b_obj._n_input_dimensionality
-        )
-        inputs = [np.linspace(0, 1, 20)] * n_input
-        if raise_exception:
-            with pytest.raises(
-                ValueError,
-                match="Input dimensionality mismatch. This basis evaluation requires [0-9]+ inputs,",
-            ):
-                basis_obj.evaluate(*inputs)
-        else:
-            basis_obj.evaluate(*inputs)
+        X, y, model, true_params, firing_rate = poisson_population_GLM_model
+        model.coef_ = true_params[0]
+        model.intercept_ = true_params[1]
+        model._initialize_feature_mask(X, y)
+        if delta_dim == -1:
+            X = np.zeros((X.shape[0],))
+        elif delta_dim == 1:
+            X = np.zeros((X.shape[0], X.shape[1], 1))
+        with expectation:
+            model.predict(X)
 
-    @pytest.mark.parametrize("sample_size", [11, 20])
-    @pytest.mark.parametrize(
-        "basis_a",
-        [class_obj for _, class_obj in utils_testing.get_non_abstract_classes(basis)],
-    )
     @pytest.mark.parametrize(
-        "basis_b",
-        [class_obj for _, class_obj in utils_testing.get_non_abstract_classes(basis)],
+        "delta_n_features, expectation",
+        [
+            (-1, pytest.raises(ValueError, match="Inconsistent number of features")),
+            (0, does_not_raise()),
+            (1, pytest.raises(ValueError, match="Inconsistent number of features")),
+        ],
     )
-    @pytest.mark.parametrize("n_basis_a", [5])
-    @pytest.mark.parametrize("n_basis_b", [6])
-    def test_evaluate_on_grid_meshgrid_size(
-        self, sample_size, n_basis_a, n_basis_b, basis_a, basis_b
+    def test_predict_n_feature_consistency_x(
+        self, delta_n_features, expectation, poisson_population_GLM_model
     ):
         """
-        Test whether the resulting meshgrid size matches the sample size input.
+        Test the `predict` method ensuring the number of features in x input data
+        is consistent with the model's `model.coef_`.
         """
-        basis_a_obj = self.instantiate_basis(n_basis_a, basis_a)
-        basis_b_obj = self.instantiate_basis(n_basis_b, basis_b)
-        basis_obj = basis_a_obj * basis_b_obj
-        res = basis_obj.evaluate_on_grid(
-            *[sample_size] * basis_obj._n_input_dimensionality
-        )
-        for grid in res[:-1]:
-            assert grid.shape[0] == sample_size
+        X, y, model, true_params, firing_rate = poisson_population_GLM_model
+        model.coef_ = true_params[0]
+        model.intercept_ = true_params[1]
+        model._initialize_feature_mask(X, y)
+        if delta_n_features == 1:
+            X = jnp.concatenate((X, jnp.zeros((X.shape[0], 1))), axis=1)
+        elif delta_n_features == -1:
+            X = X[..., :-1]
+        with expectation:
+            model.predict(X)
 
-    @pytest.mark.parametrize("sample_size", [11, 20])
     @pytest.mark.parametrize(
-        "basis_a",
-        [class_obj for _, class_obj in utils_testing.get_non_abstract_classes(basis)],
+        "is_fit, expectation",
+        [
+            (True, does_not_raise()),
+            (
+                False,
+                pytest.raises(ValueError, match="This GLM instance is not fitted yet"),
+            ),
+        ],
     )
+    def test_predict_is_fit(self, is_fit, expectation, poissonGLM_model_instantiation):
+        """
+        Test the `score` method on models based on their fit status.
+        Ensure scoring is only possible on fitted models.
+        """
+        X, y, model, true_params, firing_rate = poissonGLM_model_instantiation
+        if is_fit:
+            model.fit(X, y)
+        with expectation:
+            model.predict(X)
+
+    #######################
+    # Test model.simulate
+    #######################
     @pytest.mark.parametrize(
-        "basis_b",
-        [class_obj for _, class_obj in utils_testing.get_non_abstract_classes(basis)],
+        "delta_dim, expectation",
+        [
+            (-1, pytest.raises(ValueError, match="X must be two-dimensional")),
+            (0, does_not_raise()),
+            (1, pytest.raises(ValueError, match="X must be two-dimensional")),
+        ],
     )
-    @pytest.mark.parametrize("n_basis_a", [5])
-    @pytest.mark.parametrize("n_basis_b", [6])
-    def test_evaluate_on_grid_basis_size(
-        self, sample_size, n_basis_a, n_basis_b, basis_a, basis_b
+    def test_simulate_input_dimensionality(
+        self, delta_dim, expectation, poisson_population_GLM_model
     ):
         """
-        Test whether the number sample size output by evaluate_on_grid matches the sample size of the input.
+        Test the `simulate` method with input data of different dimensionalities.
+        Ensure correct dimensionality for input.
         """
-        basis_a_obj = self.instantiate_basis(n_basis_a, basis_a)
-        basis_b_obj = self.instantiate_basis(n_basis_b, basis_b)
-        basis_obj = basis_a_obj * basis_b_obj
-        eval_basis = basis_obj.evaluate_on_grid(
-            *[sample_size] * basis_obj._n_input_dimensionality
-        )[-1]
-        assert eval_basis.shape[0] == sample_size
+        X, y, model, true_params, firing_rate = poisson_population_GLM_model
+        model.coef_ = true_params[0]
+        model.intercept_ = true_params[1]
+        model._initialize_feature_mask(X, y)
+        if delta_dim == -1:
+            X = np.zeros(X.shape[:-1])
+        elif delta_dim == 1:
+            X = np.zeros(X.shape + (1,))
+        with expectation:
+            model.simulate(
+                random_key=jax.random.key(123),
+                feedforward_input=X,
+            )
 
-    @pytest.mark.parametrize("n_input", [0, 1, 2, 5, 6, 11, 30])
     @pytest.mark.parametrize(
-        "basis_a",
-        [class_obj for _, class_obj in utils_testing.get_non_abstract_classes(basis)],
+        "is_fit, expectation",
+        [
+            (True, does_not_raise()),
+            (
+                False,
+                pytest.raises(ValueError, match="This GLM instance is not fitted yet"),
+            ),
+        ],
     )
+    def test_simulate_is_fit(self, is_fit, expectation, poisson_population_GLM_model):
+        """
+        Test if the model raises a ValueError when trying to simulate before it's fitted.
+        """
+        X, y, model, true_params, firing_rate = poisson_population_GLM_model
+        if is_fit:
+            model.coef_ = true_params[0]
+            model.intercept_ = true_params[1]
+            model._initialize_feature_mask(X, y)
+        with expectation:
+            model.simulate(
+                random_key=jax.random.key(123),
+                feedforward_input=X,
+            )
+
     @pytest.mark.parametrize(
-        "basis_b",
-        [class_obj for _, class_obj in utils_testing.get_non_abstract_classes(basis)],
+        "delta_features, expectation",
+        [
+            (
+                -1,
+                pytest.raises(
+                    ValueError,
+                    match="Inconsistent number of features. spike basis coefficients has",
+                ),
+            ),
+            (0, does_not_raise()),
+            (
+                1,
+                pytest.raises(
+                    ValueError,
+                    match="Inconsistent number of features. spike basis coefficients has",
+                ),
+            ),
+        ],
     )
-    @pytest.mark.parametrize("n_basis_a", [5])
-    @pytest.mark.parametrize("n_basis_b", [6])
-    def test_evaluate_on_grid_input_number(
-        self, n_input, basis_a, basis_b, n_basis_a, n_basis_b
+    def test_simulate_feature_consistency_input(
+        self, delta_features, expectation, poisson_population_GLM_model
     ):
         """
-        Test whether the number of inputs provided to `evaluate_on_grid` matches
-        the sum of the number of input samples required from each of the basis objects.
-        """
-        basis_a_obj = self.instantiate_basis(n_basis_a, basis_a)
-        basis_b_obj = self.instantiate_basis(n_basis_b, basis_b)
-        basis_obj = basis_a_obj * basis_b_obj
-        inputs = [20] * n_input
-        raise_exception = (
-            n_input
-            != basis_a_obj._n_input_dimensionality + basis_b_obj._n_input_dimensionality
-        )
-        if raise_exception:
-            with pytest.raises(
-                ValueError,
-                match=r"Input dimensionality mismatch. This basis evaluation requires [0-9]+ inputs, "
-                r"[0-9]+ inputs provided instead.",
-            ):
-                basis_obj.evaluate_on_grid(*inputs)
-        else:
-            basis_obj.evaluate_on_grid(*inputs)
+        Test the `simulate` method ensuring the number of features in `feedforward_input` is
+        consistent with the model's expected number of features.
 
-    @pytest.mark.parametrize("basis_a", [basis.MSplineBasis])
-    @pytest.mark.parametrize("basis_b", [basis.OrthExponentialBasis])
-    @pytest.mark.parametrize("n_basis_a", [5])
-    @pytest.mark.parametrize("n_basis_b", [6])
-    @pytest.mark.parametrize("sample_size_a", [11, 12])
-    @pytest.mark.parametrize("sample_size_b", [11, 12])
-    def test_inconsistent_sample_sizes(
-        self, basis_a, basis_b, n_basis_a, n_basis_b, sample_size_a, sample_size_b
-    ):
-        """Test that the inputs of inconsistent sample sizes result in an exception when evaluate is called"""
-        raise_exception = sample_size_a != sample_size_b
-        basis_a_obj = self.instantiate_basis(n_basis_a, basis_a)
-        basis_b_obj = self.instantiate_basis(n_basis_b, basis_b)
-        basis_obj = basis_a_obj * basis_b_obj
-        if raise_exception:
-            with pytest.raises(
-                ValueError,
-                match=r"Sample size mismatch\. Input elements have inconsistent",
-            ):
-                basis_obj.evaluate(
-                    np.linspace(0, 1, sample_size_a), np.linspace(0, 1, sample_size_b)
-                )
-        else:
-            basis_obj.evaluate(
-                np.linspace(0, 1, sample_size_a), np.linspace(0, 1, sample_size_b)
+        Notes
+        -----
+        The total feature number `model.coef_.shape[1]` must be equal to
+        `feedforward_input.shape[2] + coupling_basis.shape[1]*n_neurons`
+        """
+        X, y, model, true_params, firing_rate = poisson_population_GLM_model
+        model.coef_ = true_params[0]
+        model.intercept_ = true_params[1]
+        model._initialize_feature_mask(X, y)
+        feedforward_input = jnp.zeros(
+            (
+                X.shape[0],
+                X.shape[1] + delta_features,
             )
+        )
+        with expectation:
+            model.simulate(
+                random_key=jax.random.key(123),
+                feedforward_input=feedforward_input,
+            )
+
+    def test_simulate_feedforward_glm(self, poissonGLM_model_instantiation):
+        """Test that simulate goes through"""
+        X, y, model, params, rate = poissonGLM_model_instantiation
+        model.coef_ = params[0]
+        model.intercept_ = params[1]
+        ysim, ratesim = model.simulate(jax.random.key(123), X)
+        # check that the expected dimensionality is returned
+        assert ysim.ndim == 1
+        assert ratesim.ndim == 1
+        # check that the rates and spikes has the same shape
+        assert ratesim.shape[0] == ysim.shape[0]
+        # check the time point number is that expected (same as the input)
+        assert ysim.shape[0] == X.shape[0]
 
+    @pytest.mark.parametrize(
+        "insert, expectation",
+        [
+            (0, does_not_raise()),
+            (np.nan, pytest.warns(UserWarning, match=r"The provided trees contain")),
+            (np.inf, pytest.warns(UserWarning, match=r"The provided trees contain")),
+        ],
+    )
+    def test_simulate_invalid_feedforward(
+        self, insert, expectation, poisson_population_GLM_model
+    ):
+        X, y, model, params, rate = poisson_population_GLM_model
+        model.coef_ = params[0]
+        model.intercept_ = params[1]
+        model._initialize_feature_mask(X, y)
+        X[0] = insert
+        with expectation:
+            model.simulate(jax.random.key(123), X)
+
+    #######################################
+    # Compare with standard implementation
+    #######################################
+    def test_deviance_against_statsmodels(self, poisson_population_GLM_model):
+        """
+        Compare fitted parameters to statsmodels.
+        Assesses if the model estimates are close to statsmodels' results.
+        """
+        X, y, model, true_params, firing_rate = poisson_population_GLM_model
+        # set model coeff
+        model.coef_ = true_params[0]
+        model.intercept_ = true_params[1]
+        # get the rate
+        dev = sm.families.Poisson().deviance(y, firing_rate)
+        dev_model = model.observation_model.deviance(firing_rate, y).sum()
+        if not np.allclose(dev, dev_model):
+            raise ValueError("Deviance doesn't match statsmodels!")
+
+    def test_compatibility_with_sklearn_cv(self, poisson_population_GLM_model):
+        X, y, model, true_params, firing_rate = poisson_population_GLM_model
+        param_grid = {"regularizer__solver_name": ["BFGS", "GradientDescent"]}
+        GridSearchCV(model, param_grid).fit(X, y)
+
+    @pytest.mark.parametrize(
+        "mask, expectation",
+        [
+            (np.array([0, 1, 1] * 5).reshape(5, 3), does_not_raise()),
+            ({"input_1": [0, 1, 0], "input_2": [1, 0, 1]},
+             pytest.raises(ValueError, match="'feature_mask' of 'populationGLM' must be a 2-dimensional array")),
+            ({"input_1": np.array([0, 1, 0]), "input_2": np.array([1, 0, 1])}, does_not_raise()),
+            ({"input_1": np.array([0, 1, 0]), "input_2": np.array([1, 0, 1.1])},
+             pytest.raises(ValueError, match="'feature_mask' must contain only 0s and 1s")),
+            (np.array([0.1, 1, 1] * 5).reshape(5, 3),
+             pytest.raises(ValueError, match="'feature_mask' must contain only 0s and 1s"))
+        ]
+    )
+    def test_feature_mask_setter(self, mask, expectation, poisson_population_GLM_model):
+        _, _, model, _, _ = poisson_population_GLM_model
+        with expectation:
+            model.feature_mask = mask
+
+    @pytest.mark.parametrize(
+        "mask, expectation",
+        [
+            (np.array([0, 1, 1] * 5).reshape(5, 3), does_not_raise()),
+            (np.array([0, 1, 1] * 4).reshape(4, 3), pytest.raises(ValueError, match="Inconsistent number of features")),
+            (np.array([0, 1, 1, 1] * 5).reshape(5, 4),  pytest.raises(ValueError, match="Inconsistent number of neurons")),
+            ({"input_1": np.array([0, 1, 0]), "input_2": np.array([1, 0, 1])},
+             pytest.raises(TypeError, match="feature_mask and X must have the same structure")),
+            ({"input_1": np.array([0, 1, 0, 1]), "input_2": np.array([1, 0, 1, 0])},
+             pytest.raises(TypeError, match="feature_mask and X must have the same structure")),
+        ]
+    )
+    @pytest.mark.parametrize("attr_name", ["fit", "predict", "score"])
+    def test_feature_mask_compatibility_fit(self, mask, expectation, attr_name, poisson_population_GLM_model):
+        X, y, model, true_params, firing_rate = poisson_population_GLM_model
+        model.feature_mask = mask
+        model.coef_ = true_params[0]
+        model.intercept_ = true_params[1]
+        with expectation:
+            if attr_name == "predict":
+                getattr(model, attr_name)(X)
+            else:
+                getattr(model, attr_name)(X, y)
+
+    @pytest.mark.parametrize(
+        "mask, expectation",
+        [
+            (np.array([0, 1, 1] * 5).reshape(5, 3),
+             pytest.raises(TypeError, match="feature_mask and X must have the same structure")),
+            (np.array([0, 1, 1] * 4).reshape(4, 3),
+             pytest.raises(TypeError, match="feature_mask and X must have the same structure")),
+            (np.array([0, 1, 1, 1] * 5).reshape(5, 4),
+             pytest.raises(TypeError, match="feature_mask and X must have the same structure")),
+            ({"input_1": np.array([0, 1, 0]), "input_2": np.array([1, 0, 1])}, does_not_raise()),
+            ({"input_1": np.array([0, 1, 0, 1]), "input_2": np.array([1, 0, 1, 0])},
+             pytest.raises(ValueError, match="Inconsistent number of neurons")),
+            ({"input_1": np.array([0, 1, 0])},
+             pytest.raises(TypeError, match="feature_mask and X must have the same structure")),
+            ({"input_1": np.array([0, 1, 0, 1])},
+             pytest.raises(TypeError, match="feature_mask and X must have the same structure"))
+        ]
+    )
+    @pytest.mark.parametrize("attr_name", ["fit", "predict", "score"])
+    def test_feature_mask_compatibility_fit_tree(self, mask, expectation, attr_name, poisson_population_GLM_model_pytree):
+        X, y, model, true_params, firing_rate = poisson_population_GLM_model_pytree
+        model.feature_mask = mask
+        model.coef_ = true_params[0]
+        model.intercept_ = true_params[1]
+        with expectation:
+            if attr_name == "predict":
+                getattr(model, attr_name)(X)
+            else:
+                getattr(model, attr_name)(X, y)
+
+    @pytest.mark.parametrize(
+        "regularizer",
+        [
+            nmo.regularizer.UnRegularized(solver_name="LBFGS", solver_kwargs={"stepsize": 0.1, "tol": 10**-14}),
+            nmo.regularizer.UnRegularized(solver_name="GradientDescent", solver_kwargs={"tol": 10 ** -14}),
+            nmo.regularizer.Ridge(solver_name="GradientDescent", regularizer_strength=0.001, solver_kwargs={"tol": 10**-14}),
+            nmo.regularizer.Ridge(solver_name="LBFGS", solver_kwargs={"stepsize": 0.1, "tol": 10 ** -14}),
+            nmo.regularizer.Lasso(regularizer_strength=0.001, solver_kwargs={"tol": 10**-14})
+        ]
+    )
+    @pytest.mark.parametrize(
+        "mask",
+        [
+            np.array([
+                [0, 0, 1],
+                [0, 1, 0],
+                [1, 1, 1],
+                [1, 0, 1],
+                [0, 1, 0],
+            ]),
+            {"input_1": np.array([0, 1, 0]), "input_2": np.array([1, 0, 1])}
+    ])
+    def test_masked_fit_vs_loop(self, regularizer, mask, poisson_population_GLM_model, poisson_population_GLM_model_pytree):
+        jax.config.update("jax_enable_x64", True)
+        if isinstance(mask, dict):
+            X, y, model, true_params, firing_rate = poisson_population_GLM_model_pytree
+
+            def map_neu(k, coef_):
+                key_ind = {"input_1": [0, 1, 2], "input_2": [3, 4]}
+                ind_array = np.zeros((0, ), dtype=int)
+                coef_stack = np.zeros((0, ), dtype=int)
+                for key, msk in mask.items():
+                    if msk[k]:
+                        ind_array = np.hstack((ind_array, key_ind[key]))
+                        coef_stack = np.hstack((coef_stack, coef_[key]))
+                return ind_array, coef_stack
+        else:
+            X, y, model, true_params, firing_rate = poisson_population_GLM_model
+
+            def map_neu(k, coef_):
+                ind_array = np.where(mask[:, k])[0]
+                coef_stack = coef_
+                return ind_array, coef_stack
+
+        mask_bool = jax.tree_util.tree_map(lambda x: np.asarray(x.T, dtype=bool), mask)
+        # fit pop glm
+        model.feature_mask = mask
+        model.regularizer = regularizer
+        model.fit(X, y)
+        coef_vectorized = np.vstack(jax.tree_util.tree_leaves(model.coef_))
+
+        coef_loop = np.zeros((5, 3))
+        intercept_loop = np.zeros((3, ))
+        # loop over neuron
+        for k in range(y.shape[1]):
+            model_single_neu = nmo.glm.GLM(regularizer=regularizer)
+            if isinstance(mask_bool, dict):
+                X_neu = {}
+                for key, xx in X.items():
+                    if mask_bool[key][k]:
+                        X_neu[key] = X[key]
+                X_neu = FeaturePytree(**X_neu)
+            else:
+                X_neu = X[:, mask_bool[k]]
+
+            model_single_neu.fit(X_neu, y[:, k])
+            idx, coef = map_neu(k, model_single_neu.coef_)
+            coef_loop[idx, k] = coef
+            intercept_loop[k] = np.array(model_single_neu.intercept_)[0]
+        print(f"\nMAX ERR: {np.abs(coef_loop - coef_vectorized).max()}")
+        assert np.allclose(coef_loop, coef_vectorized, atol=10**-5, rtol=0)
 
-@pytest.mark.parametrize(
-    "exponent", [-1, 0, 0.5, basis.RaisedCosineBasisLog(4), 1, 2, 3]
-)
-@pytest.mark.parametrize(
-    "basis_class",
-    [class_obj for _, class_obj in utils_testing.get_non_abstract_classes(basis)],
-)
-def test_power_of_basis(exponent, basis_class):
-    """Test if the power behaves as expected."""
-    raise_exception_type = not type(exponent) is int
-
-    if not raise_exception_type:
-        raise_exception_value = exponent <= 0
-    else:
-        raise_exception_value = False
-
-    basis_obj = CombinedBasis.instantiate_basis(5, basis_class)
-
-    if raise_exception_type:
-        with pytest.raises(TypeError, match=r"Exponent should be an integer\!"):
-            basis_obj**exponent
-    elif raise_exception_value:
-        with pytest.raises(
-            ValueError, match=r"Exponent should be a non-negative integer\!"
-        ):
-            basis_obj**exponent
-    else:
-        basis_pow = basis_obj**exponent
-        samples = np.linspace(0, 1, 10)
-        eval_pow = basis_pow.evaluate(*[samples] * basis_pow._n_input_dimensionality)
-
-        if exponent == 2:
-            basis_obj = basis_obj * basis_obj
-        elif exponent == 3:
-            basis_obj = basis_obj * basis_obj * basis_obj
 
-        assert np.allclose(
-            eval_pow, basis_obj.evaluate(*[samples] * basis_obj._n_input_dimensionality)
-        )
```

### Comparing `nemos-0.1.0/tests/utils_testing.py` & `nemos-0.1.1/tests/utils_testing.py`

 * *Files identical despite different names*

### Comparing `nemos-0.1.0/tox.ini` & `nemos-0.1.1/tox.ini`

 * *Files 13% similar despite different names*

```diff
@@ -10,17 +10,20 @@
 # Enable package caching
 package_cache = .tox/cache
 
 # Run both pytest and coverage since pytest was initialized with the --cov option in the pyproject.toml
 # while black, isort and flake8 are also i
 commands =
     black --check src
-    isort --check src
+    isort src --profile=black
+    isort docs/neural_modeling --profile=black
+    isort docs/background --profile=black
+    isort docs/neural_modeling --profile=black
     flake8 --config={toxinidir}/tox.ini src
-    pytest
+    pytest --cov=nemos --cov-report=xml
 
 [gh-actions]
 python =
        3.8: py38
        3.9: py39
        3.10: py310
```

